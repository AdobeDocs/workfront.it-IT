---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Elenca i metadati per file o cartelle
description: Elenca i metadati per file o cartelle
author: Becky
feature: Workfront API
role: Developer
exl-id: 9c9f9222-59ac-4643-8297-d4939bec7e64
TQID: https://experienceleague.adobe.com/nZv42xMbDRJbkwR-lFKI6dAbeszSzGWAwn--qkKhVVM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 101
ht-degree: 12%

---

# Ottenere l’elenco elementi dei contenuti della cartella

Elenca i metadati per i file e le cartelle di una determinata cartella.

**URL**

GET /files

## Parametri di query

| Nome  | Descrizione |
|---|---|
| parentId  | ID cartella. Per ottenere i metadati della directory principale, utilizza il valore &quot;/&quot;. |
| max  | Numero massimo di elementi da restituire. Utilizzato per l’impaginazione. |
| offset  |  Offset pagina, utilizzato insieme a &quot;max&quot;. |


## Risposta

JSON contenente un elenco di file e cartelle. I metadati per ogni elemento sono gli stessi restituiti dall’endpoint /metadata.

**Esempio:** https://www.acme.com/api/files?parentId=123456

```
[ 
{
title:"Folder A",
kind:"folder"
id":"2lj23lkj",
viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ",
downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",
mimeType:"",
dateModified:"2014­06­05T17:39:45.251Z"
size: ""
},
{
title:"My Document",
kind:"file"
id":"da8cj234",
viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ",
downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",
mimeType:"image/png",
dateModified:"2014­06­05T17:39:45.251Z"
size: "32554694"
}
]
```
