---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Eliminare un documento o una cartella
description: Eliminare un documento o una cartella
author: John
feature: Workfront API
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: 9de8ee7fad2a3cb67c4fc6bfdff4d6ce50f15afd
workflow-type: tm+mt
source-wordcount: '82'
ht-degree: 6%

---


# Eliminare un documento o una cartella (non ancora implementato)

Elimina un documento o una cartella con l&#39;ID specificato nel sistema esterno. L’eliminazione di una cartella comporta anche l’eliminazione del contenuto della cartella.

## URL

PUT /delete

## Parametri query

| Nome  | Descrizione |
|---|---|
| documentId  | ID documento da eliminare |
| folderId  |  ID cartella da eliminare |



## risposta

Una stringa JSON che indica l’esito positivo o negativo, come specificato nella sezione Gestione degli errori di seguito.

### Esempio

PUT https://www.example.com/api/deleteid=1234
* return `status: “success”`

* return `status: “failure”, error: “File not found”`
