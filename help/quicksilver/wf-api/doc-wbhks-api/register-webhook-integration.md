---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Registrare un’integrazione Webhook
description: Registrare un’integrazione Webhook
author: Becky
feature: Workfront API
exl-id: 9a4f8dbe-967f-4a41-a42c-8e3acb604972
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 11%

---


# Registrare un’integrazione Webhook

Gli amministratori di Adobe Workfront possono aggiungere un’integrazione webhook personalizzata per la propria azienda andando in Configurazione > Documenti > Integrazioni personalizzate all’interno di Workfront. Dalla pagina Integrazione personalizzata in Configurazione, gli amministratori possono visualizzare un elenco delle integrazioni Webhook di documenti esistenti. Da questa pagina è possibile aggiungere, modificare, abilitare e disabilitare le integrazioni.

Per aggiungere un’integrazione, fai clic su **Aggiungi integrazione personalizzata**.

![](assets/webhooks-integration-350x230.png)

![](assets/webhooks-integration-2-350x220.png)

## Campi disponibili

Quando si aggiunge un’integrazione, l’amministratore immette i valori per i campi seguenti.

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
   <td>Nome dell'integrazione.</td> 
  </tr> 
  <tr> 
   <td>URL API base</td> 
   <td> <p>Posizione dell’API di callback. Quando effettui chiamate al sistema esterno, Workfront aggiungerà semplicemente il nome dell'endpoint a questo indirizzo. Ad esempio, se l’amministratore ha inserito l’URL API di base "https://www.mycompany.com/api/v1", Workfront utilizza il seguente URL per ottenere i metadati di un documento: https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
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
   <td> <p>(Solo OAuth2) L’URL completo utilizzato per l’autenticazione degli utenti. Workfront indicherà agli utenti questo indirizzo come parte del processo di provisioning di OAuth. Nota: Workfront aggiungerà un parametro "state" alla stringa query. Il provider deve restituire questo messaggio a Workfront aggiungendolo all’URI di reindirizzamento Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>URL endpoint token</td> 
   <td> <p>(Solo OAuth2) L’URL API completo utilizzato per recuperare i token OAuth2. Questo è ospitato dal provider webhook o dal provider di documenti esterno</p> </td> 
  </tr> 
  <tr> 
   <td>ID client</td> 
   <td>(Solo OAuth2) L’ID client OAuth2 per questa integrazione</td> 
  </tr> 
  <tr> 
   <td>Segreto client</td> 
   <td> <p>(Solo OAuth2) Il segreto client OAuth2 per questa integrazione</p> </td> 
  </tr> 
  <tr> 
   <td>URI reindirizzamento Workfront</td> 
   <td>(Solo OAuth2) Questo è un campo di sola lettura ed è generato da Workfront. Questo valore viene utilizzato per registrare l'integrazione con il provider di documenti esterno. Nota: Come descritto in precedenza per l'URL di autenticazione, il provider deve aggiungere il parametro "state" e il relativo valore alla stringa di query durante l'esecuzione del reindirizzamento.</td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td> <p>(Solo ApiKey) Utilizzato per effettuare chiamate API autorizzate al provider webhook. Chiave API rilasciata dal provider webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>
