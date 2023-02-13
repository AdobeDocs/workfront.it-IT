---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Duplicati restituiti durante una ricerca impaginata di grandi dimensioni
description: Duplicati restituiti durante una ricerca impaginata di grandi dimensioni
author: John
feature: Workfront API
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# Duplicati restituiti durante una ricerca impaginata di grandi dimensioni

## Problema

Quando si esegue una ricerca impaginata di grandi dimensioni nell’API per un oggetto, il cliente riceve voci duplicate e record mancanti.

## Soluzione

Quando l&#39;ordine non è definito formalmente, ci affidiamo all&#39;ordine delle righe restituite dal database Oracle, che non garantisce alcun ordine deterministico. Ad esempio, due chiamate consecutive con la stessa query potrebbero restituire righe in un ordine diverso. Allo stesso modo, quando si esegue il paging, le righe possono essere assegnate in modo casuale a diverse &quot;pagine&quot;, generando duplicati. La soluzione più semplice è l&#39;aggiunta dell&#39;ordinamento per ID:

```
&ID_Sort=asc
```

