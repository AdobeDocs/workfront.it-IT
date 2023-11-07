---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Duplicati restituiti durante una ricerca impaginata di grandi dimensioni
description: Duplicati restituiti durante una ricerca impaginata di grandi dimensioni
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# Duplicati restituiti durante una ricerca impaginata di grandi dimensioni

## Problema

Quando si esegue una ricerca impaginata di grandi dimensioni nell’API per un oggetto, il cliente riceve voci duplicate e record mancanti.

## Soluzione

Quando l’ordine non è definito formalmente, si basa sull’ordine delle righe restituite dal database Oracle, che non garantisce alcun ordinamento deterministico. Ad esempio, due chiamate consecutive con la stessa query potrebbero restituire righe in un ordine diverso. Allo stesso modo, quando si esegue il paging, le righe possono essere assegnate in modo casuale a &quot;pagine&quot; diverse, generando duplicati. La soluzione più semplice consiste nell’aggiungere l’ordinamento per ID:

```
&ID_Sort=asc
```

