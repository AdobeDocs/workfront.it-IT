---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Ottenere i metadati per un file o una cartella
description: Ottenere i metadati per un file o una cartella
author: Becky
feature: Workfront API
role: Developer
exl-id: 7b594df5-c87f-45d4-b84a-cae17171e906
TQID: https://experienceleague.adobe.com/H04UQeyhGw-FdXDwaRZs5PSXnN-YErVptHWn-78INYo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 263
ht-degree: 16%

---

# Ottenere i metadati per un file o una cartella

Restituisce i metadati per il file o la cartella specificata.

**URL**

GET /metadata?id=[ID documento o cartella]

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
   <td>ID</td> 
   <td>ID del file o della cartella, come indicato dal provider del webhook. È diverso dall’ID documento di Adobe Workfront. Per ottenere i metadati della directory principale, utilizza il valore "/".
   <p>Nota: la lunghezza massima per l’ID è di 255 caratteri.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Risposta

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome </th> 
   <th>Tipo </th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>titolo </td> 
   <td>Stringa </td> 
   <td>Nome del documento o della cartella</td> 
  </tr> 
  <tr> 
   <td>tipo </td> 
   <td>Stringa </td> 
   <td>Specifica se l'elemento è un file o una cartella (file o cartella)</td> 
  </tr> 
  <tr> 
   <td>ID</td> 
   <td>Stringa </td> 
   <td>ID del file o della cartella.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>Stringa </td> 
   <td> <p>Percorso URL utilizzato da un utente per visualizzare il documento in una finestra del browser. L’URL può essere ospitato dal provider di documenti o dal provider di archiviazione esterno nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>Stringa </td> 
   <td> <p>Percorso URL utilizzato da un utente per scaricare il documento in una finestra del browser. L’URL può essere ospitato dal provider di documenti o dal provider di archiviazione esterno nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>Stringa </td> 
   <td>Tipo MIME del file. (opzionale)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>Stringa </td> 
   <td>Ultima modifica del file (timestamp RFC 3339 formattato)</td> 
  </tr> 
  <tr> 
   <td>dimensione</td> 
   <td>Lungo</td> 
   <td> Dimensione del file in byte. (opzionale)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Booleano</td> 
   <td> Indica se il file o la cartella è di sola lettura per l'utente autenticato (facoltativo). </td> 
  </tr> 
 </tbody> 
</table>

**Esempio:** https://www.acme.com/api/metadata?id=12345
<pre>{<br>titolo:"Il mio documento",<br>tipo:"file"<br>id":"12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345",<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dateModified:"20140605T17:39:45.251Z",<br>dimensioni: "32554694"<br>}</pre>

>[!NOTE]
>
>La gestione degli errori deve essere coerente in tutte le chiamate API. Per informazioni dettagliate, consulta la sezione &quot;Gestione degli errori&quot; di seguito.
