---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Creare una cartella con gli hook di documenti
description: Creare una cartella con gli hook di documenti
author: John
feature: Workfront API
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
source-git-commit: 1b11a4c5f0fdf1987e9f02f7aa06ec6ec36426d3
workflow-type: tm+mt
source-wordcount: '66'
ht-degree: 7%

---


# Creare una cartella con gli hook di documenti

Crea una cartella in una determinata directory.

## URL

POST /createFolder

## Parametri query

| **Nome** | **Descrizione** |
|---|---|
| parentId  | ID cartella in cui creare la cartella |
| name  | Nome della nuova cartella |




**Risposta**

I metadati della cartella appena creata, come definito dall&#39;endpoint /metadata.

## Esempio

```
POST https://www.acme.com/api/createFolder
­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------
parentId=1234
name=New Folder 
-------------------------------
```

return

```
{title:"New Folder",br /> kind:"folder"
 id":"5678",
 viewLink:"”,
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
