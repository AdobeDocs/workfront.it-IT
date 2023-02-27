---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Ottenere il contenuto di un documento tramite Webhook
description: Restituisce i byte non elaborati di un documento
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '53'
ht-degree: 7%

---

# Ottenere il contenuto di un documento tramite Webhook

Restituisce i byte non elaborati di un documento

## URL

GET/download

## Parametri query

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome </th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td> ID del documento.</td> 
  </tr> 
 </tbody> 
</table>

## risposta

Byte non elaborati del documento.

**Esempio:**:  [https://www.acme.com/api/download?id=123456](https://www.acme.com/api/download?id=123456)
