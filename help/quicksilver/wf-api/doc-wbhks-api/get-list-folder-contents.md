---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Elenca metadati per file o cartelle
description: Elenca metadati per file o cartelle
author: Becky
feature: Workfront API
exl-id: 9c9f9222-59ac-4643-8297-d4939bec7e64
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 5%

---


# Ottieni elenco elementi del contenuto della cartella

Elenca i metadati per i file e le cartelle di una determinata cartella.

**URL**

GET /files

## Parametri query

| Nome  | Descrizione |
|---|---|
| parentId  | ID cartella. Per ottenere i metadati della directory principale, utilizza il valore ‘/’. |
| max  | Il numero massimo di elementi da restituire. Utilizzato per l’impaginazione. |
| offset  |  L’offset della pagina, utilizzato insieme a &quot;max&quot;. |


## risposta

JSON contenente un elenco di file e cartelle. I metadati per ogni elemento sono gli stessi restituiti dall&#39;endpoint /metadata.

**Esempio:** https://www.acme.com/api/files?parentId=123456

```
[ 
{
title:"Folder A",
kind:"folder"
id":"2lj23lkj",
viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ”,
downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",
mimeType:"",
dateModified:"2014­06­05T17:39:45.251Z"
size: ""
},
{
title:"My Document",
kind:"file"
id":"da8cj234",
viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ”,
downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",
mimeType:"image/png",
dateModified:"2014­06­05T17:39:45.251Z"
size: "32554694"
}
]
```
