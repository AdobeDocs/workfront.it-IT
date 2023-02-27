---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Rinomina un documento o una cartella (non ancora implementata)
description: Rinominare un documento o una cartella
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 6%

---


# Rinomina un documento o una cartella (non ancora implementata)

Rinomina un documento o una cartella con l&#39;ID specificato nel sistema esterno.

**URL**

PUT/rinomina

## Parametri query

| Nome  | Descrizione |
|---|---|
| id | ID del documento o della cartella da rinominare |
| name  | Nuovo nome del documento o della cartella |


## risposta

Una stringa JSON che indica l’esito positivo o negativo, come specificato nella sezione Gestione degli errori di seguito.

**Esempio:** PUT https://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

return

```
{status: “success”
 }returns
 {
 status: “failure”, error: “Folder cannot be renamed because a folder with that name already exists.”
 }
```
