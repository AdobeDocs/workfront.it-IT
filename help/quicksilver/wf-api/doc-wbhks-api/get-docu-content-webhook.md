---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Ottenere contenuti di documenti tramite webhook
description: Restituisce i byte non elaborati di un documento
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
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
