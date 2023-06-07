---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Ottenere contenuti di documenti tramite webhook
description: Restituisce i byte non elaborati di un documento
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: 54d1753b9062b6d4910e4478c1f072b7fedc87eb
workflow-type: tm+mt
source-wordcount: '43'
ht-degree: 13%

---

# Ottenere contenuti di documenti tramite webhook

Restituisce i byte non elaborati di un documento

## URL

GET/download

## Parametri di query

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

**Esempio**:  `https://www.acme.com/api/download?id=123456`
