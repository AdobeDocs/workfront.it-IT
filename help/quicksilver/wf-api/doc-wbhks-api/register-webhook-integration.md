---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Registrare un’integrazione webhook
description: Registrare un’integrazione webhook
author: Becky
feature: Workfront API
role: Developer
exl-id: 9a4f8dbe-967f-4a41-a42c-8e3acb604972
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 11%

---


# Registrare un’integrazione webhook

Gli amministratori di Adobe Workfront possono aggiungere un’integrazione di webhook personalizzata per la propria società da Configurazione > Documenti > Integrazioni personalizzate in Workfront. Dalla pagina Integrazione personalizzata all’interno di Configurazione, gli amministratori possono visualizzare un elenco delle integrazioni dei webhook dei documenti esistenti. Da questa pagina è possibile aggiungere, modificare, abilitare e disabilitare le integrazioni.

Per aggiungere un&#39;integrazione, fare clic su **Aggiungi integrazione personalizzata**.

![Aggiungi integrazione personalizzata](assets/webhooks-integration-2-350x220.png)

## Campi disponibili

Quando aggiungi un’integrazione, l’amministratore immetterà i valori per i seguenti campi.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome Campo</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nome</td> 
   <td>Il nome di questa integrazione.</td> 
  </tr> 
  <tr> 
   <td>URL API base</td> 
   <td> <p>Posizione dell’API di callback. Quando effettui chiamate al sistema esterno, Workfront si limita ad aggiungere il nome dell’endpoint a questo indirizzo. Ad esempio, se l’amministratore ha immesso l’URL API di base, "https://www.mycompany.com/api/v1", Workfront utilizza il seguente URL per ottenere i metadati di un documento: https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
  </tr> 
  <tr> 
   <td>Parametri di richiesta</td> 
   <td> <p>Valori opzionali da accodare alla stringa di interrogazione di ogni chiamata API. Ad esempio, tipo_di_accesso </p> </td> 
  </tr> 
  <tr> 
   <td>Tipo di autenticazione</td> 
   <td>OAuth2 o ApiKey</td> 
  </tr> 
  <tr> 
   <td>URL autenticazione</td> 
   <td> <p>(Solo OAuth2) L’URL completo utilizzato per l’autenticazione dell’utente. Workfront sposterà gli utenti a questo indirizzo come parte del processo di provisioning OAuth. Nota: Workfront aggiungerà un parametro "state" alla stringa di query. Il provider deve restituire questa proprietà a Workfront aggiungendola all'URI di reindirizzamento di Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>URL endpoint token</td> 
   <td> <p>(Solo OAuth2) L’URL API completo utilizzato per recuperare i token OAuth2. È ospitato dal provider del webhook o dal provider di documenti esterno</p> </td> 
  </tr> 
  <tr> 
   <td>ID client</td> 
   <td>(Solo OAuth2) L'ID client OAuth2 per questa integrazione</td> 
  </tr> 
  <tr> 
   <td>Segreto client</td> 
   <td> <p>(Solo OAuth2) Il segreto client OAuth2 per questa integrazione</p> </td> 
  </tr> 
  <tr> 
   <td>URI reindirizzamento Workfront</td> 
   <td>(Solo OAuth2) Questo è un campo di sola lettura ed è generato da Workfront. Questo valore viene utilizzato per registrare questa integrazione con il provider di documenti esterno. Nota: come descritto in precedenza per l’URL di autenticazione, il provider deve aggiungere il parametro "state" e il relativo valore alla stringa di interrogazione durante l’esecuzione del reindirizzamento.</td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td> <p>(Solo ApiKey) Utilizzato per effettuare chiamate API autorizzate al provider del webhook. Chiave API rilasciata dal provider del webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>
