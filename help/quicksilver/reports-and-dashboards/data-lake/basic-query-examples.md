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
source-git-commit: 16809b2d1801dd7aa4ab1f452e4687601fc1ac59
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Esempi di query Workfront Data Connect

Per utilizzare al meglio i dati di Workfront Data Connect, questa pagina contiene query di esempio di base che è possibile utilizzare per acquisire familiarità con la sintassi e la struttura di tipi specifici di query.

## Query dati personalizzata

In questo esempio viene illustrato come comporre una query per restituire dati personalizzati in Workfront, ad esempio moduli personalizzati e campi personalizzati.

### Scenario

La tua organizzazione, PeopleSoft, utilizza un modulo personalizzato denominato Integrazione finanziaria. Il modulo viene allegato a ogni progetto e contiene i campi seguenti:

* **Business Unit PeopleSoft** - Campo personalizzato contenente una stringa.
* **PeopleSoft ProjectID** - Campo personalizzato contenente una stringa numerica.
* **Nome progetto espanso**: campo dati personalizzato calcolato che concatena i valori di PeopleSoft Business Unit, PeopleSoft ProjectID e il nome del progetto Workfront nativo in una singola stringa.

È necessario includere queste informazioni nella risposta per una query su Data Connect. I valori dei dati personalizzati per un record nel data lake sono contenuti in una colonna con titolo `parameterValues`. Questa colonna viene memorizzata come oggetto JSON.

### Query:

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:PeopleSoft Business Unit" :: int as PeopleSoftBusinessUnit,
    parametervalues:"DE:PeopleSoft Project ID" :: int as PeopleSoftProjectID,
    parametervalues:"DE:Expanded Project Name" :: text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Risposta

La query precedente restituisce i dati seguenti:

* `projectid` - ID progetto Workfront nativo
* `parametervalues` - colonna in cui è memorizzato un oggetto JSON
* `name` - nome progetto Workfront nativo
* `PeopleSoft Business Unit` - Valore di dati personalizzato incluso nell&#39;oggetto `parametervalues`
* `PeopleSoft Project ID` - Valore di dati personalizzato incluso nell&#39;oggetto `parametervalues`
* `Expanded Project Name` - Valore di dati personalizzato incluso nell&#39;oggetto `parametervalues`

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
