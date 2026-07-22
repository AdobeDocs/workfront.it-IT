---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Esempi di query di Data Connect
description: Query di esempio che è possibile utilizzare per acquisire familiarità con la sintassi e la struttura di tipi specifici di query.
author: Courtney
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/flDonZVaLR3bTF2aZcY9iy2ZnWbfrdhctL7J8esvxng
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: edee967a5c19d86fd471c4571a0b458f72bf370e
workflow-type: tm+mt
source-wordcount: 2201
ht-degree: 1%

---

# Esempi di query di Workfront Data Connect

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

La query utilizza le funzionalità di rilevamento degli eventi di modifica di Data Connect e determina la data in cui è stato attivato un evento con un nuovo valore di stato diverso da quello dell&#39;evento precedente. 

Esame della query dall’interno verso l’esterno: 

1. Calcola i record in cui lo stato precedente è diverso: 
   * Per ogni evento di modifica, utilizza la funzione lag() per identificare il valore precedente di stato. 

2. Filtrare solo i record modificati: 

   * Selezionare i record dal calcolo nel passaggio 1 in cui lo stato precedente != lo stato corrente. 

3. Calcola la marca temporale effettiva di inizio/fine e la durata in giorni: 

   * `<status_begin_effective_timestamp>`: calcolato nel passaggio 2. 

   * `<status_end_effective_timestamp>`: calcolato in base al successivo (lead()). `<status_begin_effective_timestamp>`: visualizzare lo stato solo se `<status_begin_effective_timestamp>` NON è NULL. 
   * `<status_duration_days>`: differenza dati tra `<status_begin_effective_timestamp>` e `<status_end_effective_timestamp>`. 

>[!NOTE]
>
>Si consiglia di utilizzare questa query come proprio &quot;View&quot; in PowerBI o Tableau. Se si desidera inserire altri campi da `<object>_event view`, unire di nuovo l&#39;output di questa query a `<object>_event view`. I campi di join sono i seguenti: <br>
>Per eventi_progetti: 
>`From projects_event p`>`Join <above query> c on c.projectid = p.projectid  `>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`

## Pianificazione: query con tipo di record singolo

In questo esempio viene illustrato come eseguire query sui dati di Workfront Planning per un singolo tipo di record memorizzato nel data lake di connessione dati.

### Scenario

La tua organizzazione utilizza Workfront Planning per monitorare le campagne. Ogni record di Campaign include un nome, uno stato, una data di inizio, una data di fine e un proprietario. Desideri richiamare un elenco di tutte le campagne attive e dei relativi dettagli chiave da utilizzare in una dashboard.

* I dati del tipo di record di pianificazione vengono memorizzati nella vista PLANNINGRECORD_CURRENT.
* Ogni riga rappresenta un singolo record e tutti i valori dei campi sono memorizzati in una colonna JSON denominata FIELD_VALUES.
* Il tipo di record è identificato dalla colonna RECORDTYPEID.
* L&#39;area di lavoro del record è identificata dalla colonna WORKSPACEID o dalla colonna WORKSPACENAME per un filtro leggibile.

### Query

```sql
SELECT
  recordid,
  FIELD_VALUES:"Name"::text AS campaign_name,
  FIELD_VALUES:"Status"::text AS campaign_status,
  FIELD_VALUES:"Start Date"::date AS start_date,
  FIELD_VALUES:"End Date"::date AS end_date,
  FIELD_VALUES:"Owner"::text AS owner
FROM PLANNINGRECORD_CURRENT
WHERE WORKSPACEID = '<your_campaign_workspace_id>'
AND RECORDTYPEID = '<your_campaign_record_type_id>'
AND FIELD_VALUES:"Status"::text = 'Active'
ORDER BY start_date ASC
```

### Risposta

La query precedente restituisce i dati seguenti:

* **recordid**: ID record di Planning univoco per la campagna.
* **nome_campagna**: nome della campagna, estratto dall&#39;oggetto JSON FIELD_VALUES.
* **campaign_status**: stato corrente della campagna.
* **start_date**: la data di inizio della campagna, impostata su un tipo di dati data.
* **end_date**: data di fine della campagna, impostata su un tipo di dati data.
* **proprietario**: nome dell&#39;utente o del team assegnato come proprietario della campagna.

### Spiegazione

I record di pianificazione in Data Connect condividono una singola struttura di tabella indipendentemente dal tipo di record. La colonna RECORDTYPEID viene utilizzata per definire l&#39;ambito della query per un tipo di record specifico, in questo caso Campagne. Sostituire `<your_campaign_record_type_id>` con l&#39;ID del tipo di record che si desidera ricercare, disponibile nelle impostazioni del tipo di record di Workfront Planning oppure eseguendo una query su RECORDTYPE_CURRENT.

I valori dei campi vengono memorizzati come oggetto JSON nella colonna FIELD_VALUES e sono accessibili utilizzando la stessa sintassi di notazione dei due punti utilizzata per i dati del modulo personalizzato:

```
<field_column>:"<field_name>"::<data_type> AS <alias>
```

I riferimenti al nome del campo devono corrispondere esattamente al nome del campo definito nella configurazione del campo Tipo di record Planning, incluse le maiuscole, la spaziatura e le emoji.

>[!NOTE]
>
>Gli ID dei tipi di record di pianificazione si trovano nell&#39;URL quando si visualizza un tipo di record in Workfront Planning. È il percorso dell’URL che inizia con &quot;Rt...&quot;. I tipi di record si trovano anche con la seguente chiamata SQL in Data Connect:
>
>
>```sql
>SELECT
>ID AS recordtypeid,
>DISPLAYNAME AS record_type_name,
>WORKSPACEID
>FROM RECORDTYPE_CURRENT
>ORDER BY record_type_name ASC
>```

## Planning: query tipi di record connessi

In questo esempio viene illustrato come eseguire query sui dati tra due tipi di record di Planning connessi, ovvero un tipo di record padre e un tipo di record a cui è connesso.

### Scenario

La tua organizzazione collega i record di Campaign ai record Tattici in Workfront Planning. Desideri generare un rapporto che mostri ogni campagna insieme ai dettagli chiave delle relative tattiche associate. Vogliono mostrare in modo specifico il nome tattico, la priorità strategica e l’allocazione del budget in modo che la leadership possa rivedere l’attività della campagna organizzata per tattica.

In Connessione dati, le connessioni tra i tipi di record nativi di Planning vengono memorizzate direttamente nella colonna FIELD_VALUES_RAW di PLANNINGRECORD_CURRENT. Per un campo di riferimento denominato &quot;Tactics&quot;, il valore è un array JSON di oggetti record connessi, ciascuno dei quali contiene una proprietà ID con il RECORDID del record connesso. Utilizzare LATERAL FLATTEN di Snowflake per espandere l&#39;array nelle righe e unire il record al tipo di record connesso.

### Query

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  t.FIELD_VALUES:"Name"::text AS tactic_name,
  t.FIELD_VALUES:"Strategic Priority"::text AS strategic_priority,
  t.FIELD_VALUES:"Budget Allocation"::float AS budget_allocation
FROM PLANNINGRECORD_CURRENT c,
INNER JOIN REFERENCE_CURRENT R 
ON r.FROM_REFERENCEID = c.REFERENCE_IDS:"Tactics"::text
INNER JOIN PLANNINGRECORD_CURRENT t
-- Join to the Tactic record using the connected record ID from the array
ON t.RECORDID = r.TO_RECORDID
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
ORDER BY tactic_name, campaign_name
```

### Risposta

La query precedente restituisce i dati seguenti:

* **campaign_id**: ID univoco del record di pianificazione per la campagna.
* **nome_campagna**: nome del record della campagna.
* **campaign_status**: stato corrente della campagna.
* **tactic_name**: nome del record tattico connesso.
* **priorità_strategica**: il valore del campo Priorità strategica dal record Tattica connesso.
* **budget_allocation**: il valore del campo Allocazione budget dal record tattico connesso, espresso come float.

### Spiegazione - KP modificato

Le connessioni tra i tipi di record nativi di Planning vengono memorizzate in una tabella di join REFERENCE_CURRENT.  La tabella di join REFERENCE_CURRENT viene utilizzata per i join tra RecordType.   Quando si esegue l&#39;unione tra RecordType, è necessario utilizzare il campo TO_RECORDID.

La colonna REFERENCE_ID nella vista PLANNINGRECORD contiene un elenco di tutti i campi REFERENCEID applicabili a tale record di pianificazione. Puoi accedere all’ID utilizzando la stessa notazione JSON di field_value.

```
<reference_ids>:"<reference_name>"::text
```

La vista REFERENCE_CURRENT contiene uno o più record in cui TO_RECORDID punta ad altri campi di pianificazione `recordId` nelle viste PLANNINGRECORD_*.

Per unire un altro campo REFERENCE a record di pianificazione aggiuntivi, alla query precedente verrà aggiunto lo stesso pattern di unione di REFERENCE_CURRENT e PLANNINGRECORD_*.


## Pianificazione: tipo di record unito alla query dati di Workfront Workflow

In questo esempio viene illustrato come unire un tipo di record Workfront Planning a un oggetto flusso di lavoro Workfront nativo, in questo caso un progetto, utilizzando la funzione di connessione nativa di Planning, che memorizza i riferimenti agli oggetti esterni nella vista REFERENCE_CURRENT.

### Scenario

La tua organizzazione collega i record di Campaign in Workfront Planning ai progetti Workfront utilizzando la funzione di connessione nativa di Planning. Desideri generare un rapporto combinato che mostri i dettagli della campagna e i dati di esecuzione live del progetto collegato, in particolare la percentuale di completamento corrente del progetto, la data di completamento pianificata e il proprietario del progetto assegnato, in modo che i responsabili delle campagne possano tenere traccia dell’avanzamento della consegna senza uscire dal contesto dell’area di lavoro di pianificazione.

### Query

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  conn.TO_EXTERNALID AS linked_project_id,
  p.name AS project_name,
  p.percentcomplete AS project_percent_complete,
  p.plannedcompletiondate AS project_planned_completion,
  p.ownerid AS project_owner_id,
  u.name AS project_owner_name
FROM WORKFRONT.PLANNING.PLANNINGRECORD_CURRENT c
-- Join to the references table to find Workfront Project connections
INNER JOIN WORKFRONT.PLANNING.REFERENCE_CURRENT conn
ON conn.REFERENCE_ID = c.REFERENCE_IDS:"ProjectId"::text
-- Join to the Workfront Projects table on the external ID
INNER JOIN WORKFRONT.WF.PROJECTS_CURRENT p
ON p.projectid = conn.TO_EXTERNALID
-- Join to Users to resolve the project owner name
LEFT JOIN WORKFRONT.WF.USERS_CURRENT u
ON u.userid = p.ownerid
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
AND p.completiontype != 'CPL' -- Exclude completed projects
ORDER BY campaign_name
```

### Risposta

La query precedente restituisce i dati seguenti:

* **campaign_id**: ID univoco del record di pianificazione per la campagna.
* **nome_campagna**: nome del record della campagna.
* **campaign_status**: lo stato corrente della campagna, da Planning.
* **linked_project_id**: ID del progetto Workfront da REFERENCE_CURRENT.TO_EXTERNALID, che identifica il progetto Workfront connesso.
* **nome_progetto**: nome del progetto Workfront nativo di PROJECTS_CURRENT.
* **project_percent_complete**: valore percentuale di completamento corrente del progetto.
* **project_planned_completion**: data di completamento pianificata del progetto Workfront collegato.
* **project_owner_id**: ID utente Workfront del proprietario del progetto.
* **nome_proprietario_progetto**: nome visualizzato del proprietario del progetto, risolto unendo a USERS_CURRENT.

### Spiegazione

Le connessioni da un tipo di record Planning a un oggetto flusso di lavoro Workfront nativo vengono memorizzate in REFERENCE_CURRENT. Ogni riga di questa visualizzazione rappresenta un collegamento direzionale: TO_EXTERNALID contiene l&#39;ID dell&#39;oggetto Workfront connesso. Le righe che rappresentano le connessioni Workfront sono identificate da `TO_EXTERNALCONNECTIONNAME = 'workfront'` e un valore TO_EXTERNALOBJECTNAME corrispondente al codice API del tipo di oggetto Workfront, ad esempio PROJ per progetti.

La colonna REFERENCE_ID nelle tabelle PLANNINGRECORD contiene un elenco di tutti i campi REFERENCEID applicabili a tale record.  Puoi accedere all’ID utilizzando la stessa notazione JSON di field_value.\
Un singolo REFERENCE_ID nella tabella PLANNINGRECORD_CURRENT può contenere uno o più collegamenti di riferimento nella tabella REFERENCE_CURRENT che collegano oggetti di un tipo di oggetto specifico nella tabella Workfront.

```
<reference_ids>:"<reference_name>"::text
```

Si noti che le viste di Planning (PLANNINGRECORD_CURRENT, REFERENCE_CURRENT) risiedono nello schema WORKFRONT.PLANNING, mentre le viste native di Workfront Workflow (PROJECTS_CURRENT, USERS_CURRENT, ecc.) risiede nello schema WORKFRONT.WF. I join tra schemi richiedono nomi di tabella completi.

La query esegue tre join:

1. **Record di Planning per la tabella dei riferimenti:** REFERENCE_CURRENT è unito a `TO_RECORDID = c.RECORDID` per trovare tutte le connessioni provenienti da ogni record di Campaign. I filtri su `TO_EXTERNALCONNECTIONNAME = 'workfront'` e `TO_EXTERNALOBJECTNAME = 'PROJ'` restringono i risultati alle righe che rappresentano connessioni specifiche ai progetti Workfront.
1. **La tabella dei riferimenti ai progetti Workfront:** TO_EXTERNALID contiene l&#39;ID progetto Workfront nativo per il progetto connesso. Viene aggiunto direttamente a `PROJECTS_CURRENT.projectid` per recuperare i dati del progetto live.
1. **Progetti per utenti:** Un LEFT JOIN a USERS_CURRENT risolve la chiave esterna ownerid nel progetto in un nome leggibile. In questo caso viene utilizzato LEFT JOIN per includere nei risultati i progetti a cui non è stato assegnato alcun proprietario.

>[!NOTE]
>
>Quando si esegue il join di tabelle esterne a Planning, NON utilizzare il campo TO_RECORDID nella query.  Non è necessario quando si esegue il join a tabelle esterne.
>
>Questo modello può essere applicato a qualsiasi oggetto di Workfront Workflow a cui Planning supporta la connessione, ad esempio Progetti, Portfolio o Programmi, modificando il filtro TO_EXTERNALOBJECTNAME nel codice API dell&#39;oggetto appropriato (ad esempio, PORT per Portfolio o PRGM per Programmi) e unendolo alla tabella WORKFRONT.WF corrispondente. Fare riferimento al dizionario dati di Workfront Data Connect per i nomi corretti delle colonne ID e tabella per ogni tipo di oggetto.

Per unire un altro campo REFERENCE ad altri record esterni, alla query precedente verrà aggiunto lo stesso pattern di unione a REFERENCE_CURRENT e alle viste del flusso di lavoro di Workfront.

I valori dei record External e Planningpossono essere uniti nella stessa query unendo più volte alla tabella REFERENCE_CURRENT e utilizzando la serie di join appropriata.


<!--
## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.
-->
