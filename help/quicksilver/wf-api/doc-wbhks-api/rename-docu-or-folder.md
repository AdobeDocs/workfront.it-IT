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
TQID: https://experienceleague.adobe.com/-HmJkcMckTK6upblNcqX5LZkdYQxoWPDeuHkFjJarh4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 81
ht-degree: 29%

---

# Rinominare un documento o una cartella (non ancora implementato)

Rinomina un documento o una cartella con l&#39;ID specificato nel sistema esterno.

**URL**

PUT /rename

## Parametri di query

| Nome  | Descrizione |
|---|---|
| ID | ID documento o cartella da rinominare |
| name  | Nuovo nome del documento o della cartella |


## Risposta

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
