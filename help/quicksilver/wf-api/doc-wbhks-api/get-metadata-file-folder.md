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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 2%

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
   <td>id</td> 
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
   <td>id</td> 
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
   <td> Indica se il file o la cartella è di sola lettura per l'utente autenticato.(opzionale) </td> 
  </tr> 
 </tbody> 
</table>

**Esempio:** https://www.acme.com/api/metadata?id=12345
<pre>{<br>titolo:"Il mio documento",<br>tipo:"file"<br>id":"12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345",<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dateModified:"20140605T17:39:45.251Z",<br>dimensioni: "32554694"<br>}</pre>

>[!NOTE]
>
>La gestione degli errori deve essere coerente in tutte le chiamate API. Per informazioni dettagliate, consulta la sezione &quot;Gestione degli errori&quot; di seguito.
