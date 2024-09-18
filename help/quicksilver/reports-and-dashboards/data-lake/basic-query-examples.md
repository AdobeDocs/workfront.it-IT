---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Esempi di query di Data Connect
description: Query di esempio che è possibile utilizzare per acquisire familiarità con la sintassi e la struttura di tipi specifici di query.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 364b668f23f5437e5cca0c4cc4793b17d444fb56
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Esempi di query Workfront Data Connect

Per utilizzare al meglio i dati di Workfront Data Connect, questa pagina contiene query di esempio di base che è possibile utilizzare per acquisire familiarità con la sintassi e la struttura di tipi specifici di query.

## Query dati personalizzata

In questo esempio viene illustrato come comporre una query per restituire dati personalizzati in Workfront, ad esempio moduli personalizzati e campi personalizzati.

### Scenario

La tua organizzazione utilizza un modulo personalizzato denominato Integrazione finanziaria. Il modulo viene allegato a ogni progetto e contiene i campi seguenti:

* **Business Unit** - Campo personalizzato contenente una stringa.
* **ProjectID** - Campo personalizzato contenente una stringa numerica.
* **Nome progetto espanso** - Campo dati personalizzato calcolato che concatena i valori di Business Unit, ProjectID e il nome del progetto Workfront nativo in un&#39;unica stringa.

È necessario includere queste informazioni nella risposta per una query su Data Connect. I valori dei dati personalizzati per un record nel data lake sono contenuti in una colonna con titolo `parametervalues`. Questa colonna viene memorizzata come oggetto JSON.

### Query:

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

### Risposta:

La query precedente restituisce i dati seguenti:

* `projectid` - ID progetto Workfront nativo
* `parametervalues` - colonna in cui è memorizzato un oggetto JSON
* `name` - nome progetto Workfront nativo
* `Business Unit` - Valore di dati personalizzato incluso nell&#39;oggetto `parametervalues`
* `Project ID` - Valore di dati personalizzato incluso nell&#39;oggetto `parametervalues`
* `Expanded Project Name` - Valore di dati personalizzato incluso nell&#39;oggetto `parametervalues`

### Spiegazione:

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

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
