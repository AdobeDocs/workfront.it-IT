---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Ottenere informazioni sul servizio
description: Ottenere informazioni sul servizio
author: John
feature: Workfront API
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: 5cb65c3a0c3ffd374c4002867c9c48985378e03c
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 4%

---


# Ottenere informazioni sul servizio (non ancora implementato)

>[!NOTE]
>
>La data di rilascio di questa funzione deve ancora essere determinata.

Restituisce informazioni sul servizio, ad esempio caratteristiche e funzionalità. Adobe Workfront utilizzerà queste informazioni per personalizzare l’interfaccia utente in Workfront. Ad esempio, se l’implementazione del webhook contiene alcune azioni personalizzate, JSON deve elencare tali operazioni nel JSON. Gli utenti potranno quindi richiamare queste azioni da Workfront.

**URL**

GET /serviceInfo

## Parametri query

Nessuno. Inoltre, le chiamate a questo endpoint non devono richiedere l&#39;autenticazione.

## risposta

JSON contenente informazioni su questo servizio

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome</th> 
   <th>Tipo </th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion </td> 
   <td>Stringa </td> 
   <td>Versione webhook implementata da questo servizio. Questo è il numero di versione elencato nella parte superiore di questa specifica.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>Stringa </td> 
   <td>Numero di versione interno del servizio. Questo numero è determinato dal provider di servizi webhook e viene utilizzato solo a scopo informativo.<br><br></td> 
  </tr> 
  <tr> 
   <td>editore </td> 
   <td>Stringa </td> 
   <td>Nome dell'azienda che fornisce l'implementazione del webhook.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Stringa </td> 
   <td>Elenco contenente gli endpoint API implementati dal servizio. Questo può essere utilizzato per garantire che l'interfaccia utente in Workfront rifletta le funzionalità offerte dal provider webhook. Ogni elemento dell’elenco deve includere il nome dell’endpoint (ad esempio "search").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Stringa</td> 
   <td>  <p>Elenco contenente le operazioni personalizzate implementate da questo webhook. Ogni voce dell’elenco include un nome e un nome visualizzato. Il nome visualizzato verrà visualizzato nel menu a discesa "Azioni documento" in Workfront. Facendo clic sull’elemento nel menu a discesa si richiama l’azione nel webhook chiamando l’endpoint /customAction .</p></td> 
  </tr> 
 </tbody> 
</table>

**Esempio:** `https://www.acme.com/api/serviceInfo`

return

```
{
webhook version: “1.2”, version: “1.0”, publisher: “Acme, LLC”, availableEndpoints: [“files”, “metadata”, “search”, “download”
“thumbnail”, “uploadInit”, “upload” ], customActions [
{
name: “archive”, displayName: “Archive” 
}, 
{name: “doSomethingElse”, displayName: “Do Something” }, 
] 
}
```
