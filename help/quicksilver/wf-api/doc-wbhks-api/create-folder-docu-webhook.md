---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Creare una cartella con i webhook dei documenti
description: Creare una cartella con i webhook dei documenti
author: Becky
feature: Workfront API
role: Developer
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '66'
ht-degree: 9%

---


# Creare una cartella con i webhook dei documenti

Crea una cartella in una determinata directory.

## URL

POST /createFolder

## Parametri di query

| **Nome** | **Descrizione** |
|---|---|
| parentId  | ID cartella in cui creare la cartella |
| nome  | Nome della nuova cartella |




**Risposta**

I metadati per la cartella appena creata, come definito dall’endpoint /metadata.

## Esempio

```
POST https://www.acme.com/api/createFolder
­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------
parentId=1234
name=New Folder 
-------------------------------
```

restituisce

```
{title:"New Folder",br /> kind:"folder"
 id":"5678",
 viewLink:"",
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
