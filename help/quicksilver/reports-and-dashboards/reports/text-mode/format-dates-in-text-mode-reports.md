---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formattare le date nei report in modalità testo
description: Le date possono essere configurate per essere visualizzate in diversi formati nei rapporti e negli elenchi in Adobe Workfront. Per stabilire un formato data, è necessario modificare la riga value del codice della modalità testo nella colonna.
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 2%

---

# Formattare le date nei report in modalità testo

Le date possono essere configurate per essere visualizzate in diversi formati nei rapporti e negli elenchi in Adobe Workfront. Per stabilire un formato di data, è necessario modificare il `valueformat` riga del codice della modalità testo nella colonna .

`valueformat= [new date format]` Ad esempio, se desideri che la data di completamento prevista sia visualizzata come MM/GG/AA, il codice sarà simile al seguente:

```
valueformat=atDate
valuefield=projectedCompletionDate
```

Se si desidera visualizzare la data di completamento pianificata come *Mth, DD, Year*, il codice sarà simile al seguente:

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

Per ulteriori informazioni sull&#39;applicazione della formattazione condizionale nei rapporti e negli elenchi di Workfront utilizzando la modalità testo, consulta [Utilizzare la formattazione condizionale nella modalità Testo](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

È possibile formattare le date utilizzando quanto segue

```
valueformat
```

 valori della modalità testo:

| **Formato** | Esempio  | ***valueformat=*** |
|---|---|---|
| MM/GG/AA | 10/11/18 | `atDate` |
| GG/MM/AA | 11/10/18 12:00 | `longAtDate` |
| MM/GG/AA | 10/11/18 | `shortAtDate` |
| Mth, DD, YR | 11 ottobre 2018 | `mediumAtDate` |
| DW, Mth, Day, YR | lun, 11 ottobre 2018 | `partialAtDate` |
| DW, Mth, Day, Ytime | lun, 11 ottobre 2018 12:00 | `fullAtDate` |
