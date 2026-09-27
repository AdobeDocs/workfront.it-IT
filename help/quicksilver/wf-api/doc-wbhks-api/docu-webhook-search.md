---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Ricerca tramite webhook dei documenti
description: Ricerca tramite webhook dei documenti
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
TQID: 'https://experienceleague.adobe.com/flRrmTOPVSGP83tVYfKG9AZOT7CNZN4IeWZNsVwcOO4'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: 682536a8-4872-5ee6-a8a6-8012d713482c
    internal-label: Workfront API
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 12%
---
# Ricerca tramite webhook dei documenti

Restituisce i metadati per i file e le cartelle restituiti da una ricerca. Questa può essere implementata come ricerca full-text o come normale query di database. Adobe Workfront chiama l’endpoint /search quando l’utente esegue una ricerca dal browser di file esterno.

## URL

GET /search

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
   <td>query</td> 
   <td>Termine o frase di ricerca.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(facoltativo) ID della cartella da cui è stata eseguita la ricerca. Nota: questo è un segnaposto per una funzione futura in Workfront. Attualmente, Workfront non passa questo parametro. </p> </td> 
  </tr> 
  <tr> 
   <td>max</td> 
   <td>Numero massimo di elementi da restituire. Utilizzato per l’impaginazione.</td> 
  </tr> 
  <tr> 
   <td>offset</td> 
   <td> Offset pagina, utilizzato insieme a "max".</td> 
  </tr> 
 </tbody> 
</table>

 

## Risposta

JSON contenente un elenco di metadati per file e cartelle che corrispondono alla query. Che cosa costituisce una &quot;corrispondenza&quot; è determinato dal provider del webhook. Idealmente, dovrebbe eseguire una ricerca full-text. È anche possibile eseguire una ricerca basata sul nome del file.

**Esempio:**

Esempio: `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
