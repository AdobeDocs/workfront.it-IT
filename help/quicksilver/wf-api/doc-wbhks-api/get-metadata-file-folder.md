---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Ottenere metadati per un file o una cartella
description: Ottenere metadati per un file o una cartella
author: Becky
feature: Workfront API
exl-id: 7b594df5-c87f-45d4-b84a-cae17171e906
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 6%

---


# Ottenere metadati per un file o una cartella

Restituisce i metadati per il file o la cartella specificati.

**URL**

GET /metadata?id=[ID documento o cartella]

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
   <td>id</td> 
   <td>ID del file o della cartella, a cui fa riferimento il provider webhook. È diverso dall’ID del documento di Adobe Workfront. Per ottenere i metadati della directory principale, utilizza il valore ‘/’.
   <p>Nota: La lunghezza massima per l'ID è di 255 caratteri.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## risposta

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
   <td>title </td> 
   <td>Stringa </td> 
   <td>Nome del documento o della cartella</td> 
  </tr> 
  <tr> 
   <td>gentile </td> 
   <td>Stringa </td> 
   <td>Specifica se l'elemento è un file o una cartella ("file" o "cartella")</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>Stringa </td> 
   <td>ID del file o della cartella.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>Stringa </td> 
   <td> <p>Percorso URL utilizzato da un utente per visualizzare il documento in una finestra del browser. L'URL può essere ospitato dal provider di documenti o dal provider di archiviazione esterno nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>Stringa </td> 
   <td> <p>Percorso URL utilizzato da un utente per scaricare il documento in una finestra del browser. L'URL può essere ospitato dal provider di documenti o dal provider di archiviazione esterno nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>Stringa </td> 
   <td>Il tipo MIME del file. (opzionale)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>Stringa </td> 
   <td>L’ultima volta che questo file è stato modificato (data e ora formattata RFC 3339)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
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
<pre>{<br>titolo:"Il mio documento",<br>tipo:"file"<br>id":"12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345",<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dataModificata:"20140605T17:39:45,251Z",<br>dimensioni: "32554694"<br>}</pre>

>[!NOTE]
>
>La gestione degli errori deve essere coerente in tutte le chiamate API. Per ulteriori informazioni, consulta la sezione &quot;Gestione degli errori&quot; di seguito.
