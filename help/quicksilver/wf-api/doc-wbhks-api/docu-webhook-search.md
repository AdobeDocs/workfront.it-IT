---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Ricerca tramite Webhook di documenti
description: Ricerca tramite Webhook di documenti
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 4%

---

# Ricerca tramite Webhook di documenti

Restituisce i metadati per i file e le cartelle restituiti da una ricerca. Può essere implementato come ricerca full-text o come normale query di database. Adobe Workfront chiama l&#39;endpoint /search quando l&#39;utente esegue una ricerca dal browser file esterno.

## URL

GET /search

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
   <td>query</td> 
   <td>Il termine o la frase di ricerca.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(facoltativo) ID cartella da cui viene eseguita la ricerca. Nota: Segnaposto per una funzione futura in Workfront. Attualmente, workfront non trasmette questo parametro. </p> </td> 
  </tr> 
  <tr> 
   <td>max</td> 
   <td>Il numero massimo di elementi da restituire. Utilizzato per l’impaginazione.</td> 
  </tr> 
  <tr> 
   <td>offset</td> 
   <td> L’offset della pagina, utilizzato insieme a "max".</td> 
  </tr> 
 </tbody> 
</table>

 

## risposta

JSON contenente un elenco di metadati per file e cartelle corrispondenti alla query. Ciò che costituisce un &quot;match&quot; è determinato dal provider webhook. Idealmente, dovrebbe effettuare una ricerca full-text. Anche eseguire una ricerca basata sul nome del file funziona.

**Esempio:**

Esempio:  `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
