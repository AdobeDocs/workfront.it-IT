---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Duplicati restituiti durante una ricerca paginata di grandi dimensioni
description: Duplicati restituiti durante una ricerca paginata di grandi dimensioni
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
TQID: https://experienceleague.adobe.com/1FXTHSro-rlUVHaajM1monR2Y-sxVHN6KIviogoXqRc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 111
ht-degree: 19%

---

# Duplicati restituiti durante una ricerca paginata di grandi dimensioni

## Problema

Quando si esegue una ricerca impaginata di grandi dimensioni nell’API per un oggetto, il cliente riceve voci duplicate e record mancanti.

## Soluzione

Quando l’ordine non è definito formalmente, si basa sull’ordine delle righe restituite dal database di Oracle, il che non garantisce alcun ordinamento deterministico. Ad esempio, due chiamate consecutive con la stessa query potrebbero restituire righe in un ordine diverso. Allo stesso modo, quando si esegue il paging, le righe possono essere assegnate in modo casuale a &quot;pagine&quot; diverse, generando duplicati. La soluzione più semplice consiste nell’aggiungere l’ordinamento per ID:

```
&ID_Sort=asc
```

