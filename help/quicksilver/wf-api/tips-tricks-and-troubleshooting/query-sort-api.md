---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Ordinamento dei risultati della query nell’API
description: Ordinamento dei risultati della query nell’API
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: 5936982217adc6cfcaf9e400bfff67a1496d3a78
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# Ordinamento dei risultati della query nell’API

Puoi ordinare i risultati in base a qualsiasi campo se aggiungi quanto segue alla chiamata API:

```
&entryDate_Sort=asc
```

Se ad esempio si desidera ordinare in base alla data di completamento pianificata dell&#39;attività, rimuovere `entryDate` e sostituirlo con `plannedCompletionDate`.

```
&plannedCompletionDate_Sort=asc
```

Questo funziona per la maggior parte dei campi in Adobe Workfront.
