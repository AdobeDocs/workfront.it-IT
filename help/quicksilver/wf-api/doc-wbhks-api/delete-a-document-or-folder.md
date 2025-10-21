---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Eliminare un documento o una cartella
description: Eliminare un documento o una cartella
author: Becky
feature: Workfront API
role: Developer
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '75'
ht-degree: 8%

---


# Eliminare un documento o una cartella (non ancora implementato)

Elimina un documento o una cartella con l&#39;ID specificato nel sistema esterno. L’eliminazione di una cartella comporta anche l’eliminazione del contenuto della cartella.

## URL

PUT /delete

## Parametri di query

| Nome  | Descrizione |
|---|---|
| documentId  | ID documento da eliminare |
| folderId  |  ID cartella da eliminare |



## Risposta

Stringa JSON che indica l’esito positivo o negativo, come specificato nella sezione Gestione degli errori di seguito.

### Esempio

```
PUT https://www.example.com/api/deleteid=1234

* returns `status: "success"`

* returns `status: "failure", error: "File not found"`
```
