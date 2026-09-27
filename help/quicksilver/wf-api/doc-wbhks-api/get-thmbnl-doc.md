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
TQID: 'https://experienceleague.adobe.com/-LE1gxQ9aViRNuN0sI14HlZaIcLc6Mmm8XmS1zaRCFQ'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: 682536a8-4872-5ee6-a8a6-8012d713482c
    internal-label: Workfront API
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '55'
ht-degree: 45%
---
# Ottenere una miniatura per un documento

Restituisce i byte delle miniature non elaborati per un documento.

**URL**

GET /thumbnail

## Parametri di query

| Nome  | Descrizione |
|---|---|
| ID  | ID del documento. |
| dimensione  |  Larghezza della miniatura. |


## Risposta

Byte delle miniature non elaborati.

**Esempio:**: https://www.acme.com/api/thumbnail?id=123456
