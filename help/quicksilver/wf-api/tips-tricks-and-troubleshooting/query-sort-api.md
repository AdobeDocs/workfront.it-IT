---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Ordinamento dei risultati della query nell’API
description: Ordinamento dei risultati della query nell’API
author: Becky
feature: Workfront API
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# Ordinamento dei risultati della query nell’API

Puoi ordinare i risultati in base a qualsiasi campo se aggiungi quanto segue alla chiamata API:

```
&entryDate_Sort=asc
```

Ad esempio, se si desidera ordinare per attività Data inizio pianificata, rimuovere `entryDate` e sostituirlo con `plannedCompletionDate`.

Questo funziona per la maggior parte dei campi in Adobe Workfront.
