---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Ottenere una miniatura per un documento
description: Ottenere una miniatura per un documento
author: Becky
feature: Workfront API
role: Developer
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '50'
ht-degree: 6%

---


# Ottenere una miniatura per un documento

Restituisce i byte delle miniature non elaborati per un documento.

**URL**

GET/miniatura

## Parametri di query

| Nome  | Descrizione |
|---|---|
| id  | ID del documento. |
| dimensione  |  Larghezza della miniatura. |


## Risposta

Byte delle miniature non elaborati.

**Esempio:**: https://www.acme.com/api/thumbnail?id=123456
