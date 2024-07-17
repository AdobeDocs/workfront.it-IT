---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formattare le date nei report in modalità testo
description: Le date possono essere configurate per la visualizzazione in diversi formati nei rapporti ed elenchi in Adobe Workfront. Per stabilire un formato data, è necessario modificare la riga formato valore del codice della modalità testo nella colonna.
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Formattare le date nei report in modalità testo

Le date possono essere configurate per la visualizzazione in diversi formati nei rapporti ed elenchi in Adobe Workfront. Per stabilire un formato data, è necessario modificare la riga `valueformat` del codice in modalità testo nella colonna.

`valueformat= [new date format]` Ad esempio, se si desidera che la data di completamento prevista venga visualizzata come MM/GG/AA, il codice sarà simile al seguente:

```
valueformat=atDate
valuefield=projectedCompletionDate
```

Se desideri visualizzare la Data di completamento pianificata come *Mese, GG, Anno*, il codice sarà simile al seguente:

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

Per ulteriori informazioni sull&#39;applicazione della formattazione condizionale nei report e negli elenchi di Workfront utilizzando la modalità testo, vedere [Utilizzare la formattazione condizionale in modalità testo](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

È possibile formattare le date utilizzando i seguenti

```
valueformat
```

 valori modalità testo:

| **Formato** | Esempio  | ***formato valore=*** |
|---|---|---|
| GG/MM/AA | 10/11/18 | `atDate` |
| DD/MM/YY | 10/11/18 12:00 pm | `longAtDate` |
| GG/MM/AA | 10/11/18 | `shortAtDate` |
| Mth, DD, YR | 11 ottobre 2018 | `mediumAtDate` |
| DW, mese, giorno, anno | lunedì 11 ottobre 2018 | `partialAtDate` |
| DW, Mth, Day, YR Time | Lun, 11 ottobre 2018 12:00 pm | `fullAtDate` |
