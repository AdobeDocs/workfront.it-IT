---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Rinominare un documento o una cartella (non ancora implementato)
description: Rinominare un documento o una cartella
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 8%

---


# Rinominare un documento o una cartella (non ancora implementato)

Rinomina un documento o una cartella con l&#39;ID specificato nel sistema esterno.

**URL**

PUT /rename

## Parametri di query

| Nome  | Descrizione |
|---|---|
| id | ID documento o cartella da rinominare |
| name  | Nuovo nome del documento o della cartella |


## risposta

Stringa JSON che indica l’esito positivo o negativo, come specificato nella sezione Gestione degli errori di seguito.

**Esempio:** PUT https://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

restituisce

```
{status: "success"
 }returns
 {
 status: "failure", error: "Folder cannot be renamed because a folder with that name already exists."
 }
```
