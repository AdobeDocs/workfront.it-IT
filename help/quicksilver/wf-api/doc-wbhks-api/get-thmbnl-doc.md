---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Ottenere una miniatura di un documento
description: Ottenere una miniatura di un documento
author: Becky
feature: Workfront API
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 7%

---


# Ottenere una miniatura di un documento

Restituisce i byte delle miniature non elaborati di un documento.

**URL**

GET /thumbnail

## Parametri query

| Nome  | Descrizione |
|---|---|
| id  | ID del documento. |
| size  |  Larghezza della miniatura. |


## risposta

I byte delle miniature non elaborati.

**Esempio:**: https://www.acme.com/api/thumbnail?id=123456
