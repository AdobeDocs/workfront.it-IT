---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Ricerca tramite webhook documenti
description: Ricerca tramite webhook documenti
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 5%

---

# Ricerca tramite webhook documenti

Restituisce i metadati per i file e le cartelle restituiti da una ricerca. Questa può essere implementata come ricerca full-text o come normale query di database. Adobe Workfront chiama l’endpoint /search quando l’utente esegue una ricerca dal browser di file esterno.

## URL

GET/ricerca

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

 

## risposta

JSON contenente un elenco di metadati per file e cartelle che corrispondono alla query. Che cosa costituisce una &quot;corrispondenza&quot; è determinato dal provider del webhook. Idealmente, dovrebbe eseguire una ricerca full-text. È anche possibile eseguire una ricerca basata sul nome del file.

**Esempio:**

Esempio:  `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
