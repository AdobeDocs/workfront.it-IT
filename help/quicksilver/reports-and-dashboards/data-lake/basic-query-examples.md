---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Esempi di query di Data Connect
description: Query di esempio che è possibile utilizzare per acquisire familiarità con la sintassi e la struttura di tipi specifici di query.
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: c8a25bcc8c9b56a649ca7764918c86f9cdd5b3e2
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Esempi di query Workfront Data Connect

Per utilizzare al meglio i dati di Workfront Data Connect, questa pagina contiene query di esempio di base che è possibile utilizzare per acquisire familiarità con la sintassi e la struttura di tipi specifici di query.

## Query dati personalizzata

In questo esempio viene illustrato come comporre una query per restituire dati personalizzati in Workfront, ad esempio moduli personalizzati e campi personalizzati.

### Scenario

La tua organizzazione utilizza un modulo personalizzato denominato Integrazione finanziaria. Il modulo viene allegato a ogni progetto e contiene i campi seguenti:

* **Business Unit**: campo personalizzato contenente una stringa.
* **ProjectID**: campo personalizzato contenente una stringa numerica.
* **Nome progetto espanso**: campo dati personalizzato calcolato che concatena i valori di Business Unit, ProjectID e il nome del progetto Workfront nativo in una singola stringa.

È necessario includere queste informazioni nella risposta per una query su Data Connect. I valori dei dati personalizzati per un record nel data lake sono contenuti in una colonna con titolo `parametervalues`. Questa colonna viene memorizzata come oggetto JSON.

### Query

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit"::int as BusinessUnit,
    parametervalues:"DE:Project ID"::int as ProjectID,
    parametervalues:"DE:Expanded Project Name"::text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Risposta

La query precedente restituisce i dati seguenti:

* `projectid`: ID progetto Workfront nativo.
* `parametervalues`: colonna che memorizza un oggetto JSON.
* `name`: nome progetto Workfront nativo.
* `Business Unit`: valore di dati personalizzato incluso nell&#39;oggetto `parametervalues`.
* `Project ID`: valore di dati personalizzato incluso nell&#39;oggetto `parametervalues`.
* `Expanded Project Name`: valore di dati personalizzato incluso nell&#39;oggetto `parametervalues`.

### Spiegazione

Quando si esegue una query sull&#39;oggetto JSON `parametervalues`, è possibile accedere a ogni campo dati personalizzato come colonna utilizzando quanto segue:

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>` è il nome dell&#39;oggetto JSON nella tabella di cui viene eseguita la query. Nel caso di dati personalizzati, questo sarà sempre `parametervalues`.
* `<parameter_name>` è la stringa `parametername` trovata nello strumento di configurazione del modulo, anche se potrebbe non corrispondere sempre a questo valore.

>[!NOTE]
>
>Se il nome del parametro viene modificato nello strumento di configurazione del modulo di Workfront, verrà rappresentato come una nuova colonna nell’oggetto JSON. Pertanto, è consigliabile non modificare il nome di una colonna una volta creata nello strumento di configurazione del modulo. Tuttavia, l’etichetta può essere modificata senza influire sull’oggetto JSON.
>
>Se la stringa di testo per il nome del parametro non è corretta, la colonna restituirà un valore NULL anziché un errore.

* `<data_type>` converte il valore restituito dall&#39;oggetto JSON in un tipo di dati appropriato per il campo. Se si sceglie un tipo di dati non compatibile per il valore restituito, si verificherà un errore di mancata corrispondenza del tipo di dati. I tipi di dati possibili includono:

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)` (ad esempio, `Number(32,4)` restituirebbe 1234.0987)
   * `date`
   * `timestamp`

* `<column_name>` è l&#39;etichetta creata per ogni colonna di dati personalizzata.

>[!NOTE]
>
>Solo i parametri a cui sono assegnati valori nel modulo verranno inclusi nell’oggetto JSON. Se un campo dati personalizzato è vuoto nel modulo, non verrà visualizzato.

## Tempo nella query di stato

Questo esempio illustra come misurare il tempo trascorso da un progetto negli stati assegnati in precedenza. Può essere facilmente adattato per misurare il tempo di attività o problema in uno stato, oppure può essere adattato per misurare quanto tempo un oggetto ha avuto qualsiasi altro attributo (inclusi i valori di dati personalizzati) applicato.

### Scenario

La leadership della tua organizzazione ritiene che tu stia passando troppo tempo in ogni fase del tuo ciclo di vita lavorativa. Prima di formulare raccomandazioni per migliorare il processo, è necessario creare una misurazione di base della frequenza con cui lo stato di un progetto cambia nel tempo e del numero di giorni in cui un progetto rimane nello stato specificato.

Stai per utilizzare la visualizzazione dati PROJECTS_EVENT per richiamare un elenco di ogni modifica di stato rispetto all’oggetto del progetto. Confronterai il nuovo stato con lo stato precedente, acquisirai l’intervallo di tempo effettivo per lo stato assegnato in precedenza e quindi calcolerai i giorni trascorsi in tale stato.

Utilizzando questo output non elaborato del tempo trascorso in ogni stato per progetto, puoi iniziare a creare visualizzazioni o aggregare ulteriormente i dati per generare le medie della durata dello stato in base allo stato, al tipo di progetto o al tempo dell’anno. Questa linea di base viene quindi utilizzata per impostare un benchmark da misurare per soddisfare le aspettative della leadership.

La query seguente utilizza la visualizzazione dati Data Connect PROJECTS_EVENTS per confrontare ogni evento di modifica dello stato del progetto e visualizzare il tempo nello stato.

### Query

```
-- Calculate the begin/end effective timestamp and duration in days 

SELECT 

    projectid, 
    name as project_name, 
    prev_status as previous_status, 
    status, 
    status_change_date as status_begin_effective_timestamp, 
    case 
        when status_change_date is null then NULL
        else
            nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp) 
    end as status_end_effective_timestamp, 
    datediff('DAYS',status_change_date, nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp)) as status_duration_days 

FROM 
    ( -- Filter to just the records that have changed 
     SELECT projectid, 
        name, 
        prev_status, 
        status, 
        begin_effective_timestamp as status_change_date    
     FROM 
        (  -- Calculate records where previous status is different 
          SELECT DISTINCT  
           pe.projectid, 
           pe.name AS name, 
           pe.STATUS, 
           nvl(lag(pe.STATUS) over (partition by pe.projectid order by pe.BEGIN_EFFECTIVE_TIMESTAMP), status) prev_status, 
           begin_effective_timestamp 

          FROM projects_event pe 
         -- Set any WHERE conditions to limit the results as needed 
         --WHERE 
            -- pe.PROJECTID = '5ebe…c1e1' 
        ) 
        WHERE prev_status != status 
    ) 
    order by status_change_date; 
```

### Risposta

La query precedente restituisce i dati seguenti:

* `PROJECTID`: ID progetto Workfront associato all&#39;evento di modifica dello stato.
* `PROJECT_NAME`: nome del progetto Workfront.
* `PREVIOUS_STATUS`: stato del progetto immediatamente prima della modifica.
* `STATUS`: lo stato del progetto dopo la modifica.
* `STATUS_BEGIN_EFFECTIVE_TIMESTAMP`: il timestamp dell&#39;evento di modifica quando è stato impostato lo stato precedente.
* `STATUS_END_EFFECTIVE_TIMESTAMP`: il timestamp dell&#39;evento di modifica quando è stato impostato il valore di stato aggiornato.
* `STATUS_DURATION_DAYS`: differenza (in giorni) tra il timestamp effettivo finale e il timestamp effettivo iniziale.

### Spiegazione

La query utilizza le funzionalità di rilevamento degli eventi di modifica di Data Connect.  Determina la data di attivazione di un evento con un nuovo valore di stato diverso da quello dell’evento precedente. 

Esame della query dall’interno verso l’esterno: 

1. Calcola i record in cui lo stato precedente è diverso: 
   * Per ogni evento di modifica, utilizza la funzione lag() per identificare il valore precedente di stato. 

2. Filtrare solo i record modificati: 

   * Selezionare i record dal calcolo nel passaggio 1 in cui lo stato precedente.= stato corrente. 

3. Calcola la marca temporale effettiva di inizio/fine e la durata in giorni: 

   * `<status_begin_effective_timestamp>`: calcolato nel passaggio 2. 

   * `<status_end_effective_timestamp>`: calcolato in base al successivo (lead()). `<status_begin_effective_timestamp>`: visualizzare lo stato solo se `<status_begin_effective_timestamp>` NON è NULL. 
   * `<status_duration_days>`: differenza dati tra `<status_begin_effective_timestamp>` e `<status_end_effective_timestamp>`. 

>[!NOTE]
>
>Si consiglia di utilizzare questa query come proprio &quot;View&quot; in PowerBI o Tableau.  Se si desidera importare altri campi da `<object>_event view`, unire l&#39;output di questa query di nuovo a `<object>_event view`.  I campi di join sono i seguenti: <br>
>&#x200B;>Per projects_event: 
>&#x200B;>`From projects_event p`
>&#x200B;>`Join <above query> c on c.projectid = p.projectid  `
>&#x200B;>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`



<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
