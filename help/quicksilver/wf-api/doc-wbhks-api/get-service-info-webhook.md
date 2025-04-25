---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Ottieni informazioni sul servizio
description: Ottieni informazioni sul servizio
author: Becky
feature: Workfront API
role: Developer
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 2%

---


# Ottieni informazioni sul servizio (non ancora implementato)

>[!NOTE]
>
>La data di rilascio di questa funzione non è ancora stata determinata.

Restituisce informazioni sul servizio, ad esempio caratteristiche e funzionalità. Adobe Workfront utilizzerà queste informazioni per personalizzare l’interfaccia utente in Workfront. Ad esempio, se l’implementazione del webhook contiene alcune azioni personalizzate, il JSON deve elencare tali operazioni nel JSON. Gli utenti potranno quindi richiamare queste azioni da Workfront.

**URL**

GET /serviceInfo

## Parametri di query

Nessuno. Inoltre, le chiamate a questo endpoint non devono richiedere l’autenticazione.

## Risposta

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
   <td>Versione del webhook implementata da questo servizio. Il numero di versione riportato nella parte superiore della specifica.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>Stringa </td> 
   <td>Numero di versione interno per questo servizio. Questo numero è determinato dal provider di servizi webhook ed è utilizzato solo a scopo informativo.<br><br></td> 
  </tr> 
  <tr> 
   <td>editore </td> 
   <td>Stringa </td> 
   <td>Il nome della società che fornisce l’implementazione del webhook.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Stringa </td> 
   <td>Elenco contenente gli endpoint API implementati da questo servizio. Questa può essere utilizzata per garantire che l’interfaccia utente di Workfront rifletta le funzionalità offerte dal provider del webhook. Ogni elemento nell’elenco deve includere il nome del punto finale (ad esempio "search").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Stringa</td> 
   <td>  <p>Elenco contenente le operazioni personalizzate implementate da questo webhook. Ogni voce di elenco include un nome e un nome visualizzato. Il nome visualizzato verrà visualizzato nel menu a discesa "Azioni documento" in Workfront. Facendo clic sull’elemento nel menu a discesa, l’azione viene richiamata nel webhook chiamando l’endpoint /customAction.</p></td> 
  </tr> 
 </tbody> 
</table>

**Esempio:** `https://www.acme.com/api/serviceInfo`

restituisce

```
{
webhook version: "1.2", version: "1.0", publisher: "Acme, LLC", availableEndpoints: ["files", "metadata", "search", "download"
"thumbnail", "uploadInit", "upload" ], customActions [
{
name: "archive", displayName: "Archive" 
}, 
{name: "doSomethingElse", displayName: "Do Something" }, 
] 
}
```
