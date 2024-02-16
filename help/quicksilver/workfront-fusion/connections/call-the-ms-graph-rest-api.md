---
title: Chiamare l’API REST di MS Graph tramite [!DNL Adobe Workfront Fusion] HTTP &gt; Creare un modulo di richiesta OAuth 2.0
description: Chiamare l’API REST di MS Graph tramite [!DNL Adobe Workfront Fusion] HTTP &gt; Creare un modulo di richiesta OAuth 2.0
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# Chiama il[!UICONTROL  API REST di MS Graph] tramite [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo

Molti [!DNL Microsoft] i servizi web sono accessibili tramite il [!DNL Microsoft Graph API]. Questo articolo descrive come creare una connessione a tale API utilizzando [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o versione successiva</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Registrati [!DNL Workfront Fusion] nel [!DNL Microsoft Application Registration Portal]

Per creare una connessione al [!DNL Microsoft Graph REST API], è necessario prima registrarsi [!DNL Adobe Workfront Fusion].

1. Inizia la registrazione di una nuova applicazione come descritto in [Registrare l’app](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) nel [!DNL Microsoft] documentazione.

   Nell&#39;ambito della registrazione, [!DNL Microsoft] richiede le seguenti informazioni:

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Nome applicazione]</td>
        <td>Immettere un nome per l'applicazione, ad esempio "My [!DNL Workfront Fusion] applicazione."</td>
      </tr>
      <tr>
        <td>[!UICONTROL URL di reindirizzamento]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. Una volta completata la registrazione dell’app, annota quanto segue: [!UICONTROL ID applicazione].

   >[!IMPORTANT]
   >
   >Per configurare la connessione in è necessario disporre dell&#39;ID applicazione [!DNL Workfront Fusion].

1. Genera un [!UICONTROL Segreto applicazione]. Prendi nota di questo segreto.

   Per istruzioni, consulta [Registrare l’app](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) nel [!DNL Microsoft] documentazione.

   >[!IMPORTANT]
   >
   >Avrai bisogno di [!UICONTROL Segreto applicazione] per configurare la connessione in [!DNL Workfront Fusion].

1. Configura le autorizzazioni per l’applicazione.

   Per informazioni specifiche su come individuare e configurare questi campi, consulta la sezione &quot;Configurare le autorizzazioni per Microsoft Graph&quot; in [Accedi senza un utente](https://docs.microsoft.com/en-us/graph/auth-v2-service) nel [!UICONTROL Microsoft] documentazione.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Quale tipo di autorizzazioni sono necessarie per l'applicazione?]</td> 
      <td>Seleziona <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Seleziona autorizzazioni]</td> 
      <td> <p>Seleziona le seguenti autorizzazioni:</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Qualsiasi altra autorizzazione richiesta dalle integrazioni (ad esempio: <code>User.Read</code>)</p> </li> 
       </ul> <p>Importante: per configurare la connessione in sono necessarie le autorizzazioni selezionate [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Procedi a [Configurare [!DNL MS Graph API] connessione in [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Configurare [!DNL MS Graph API] connessione in [!DNL Workfront Fusion]

Dopo la registrazione [!DNL Workfront Fusion] come discusso in [Registrati [!DNL Workfront Fusion] nel [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal), è possibile configurare la connessione in [!UICONTROL HTTP] >[!UICONTROL Creare un Oauth 2.0] modulo di richiesta.

1. Aggiungi un [!UICONTROL HTTP] >[!UICONTROL Effettuare una chiamata OAuth 2.0] al tuo scenario.
1. Clic **[!UICONTROL Aggiungi]** accanto al [!UICONTROL connessione] campo.
1. Configura i campi di connessione come segue:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome connessione]</td> 
      <td>Immettere un nome per la connessione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Tipo di flusso]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autorizza URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ambito]</td> 
      <td> <p>Immetti le autorizzazioni selezionate al passaggio 4 di <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrati [!DNL Workfront Fusion] nel [!DNL Microsoft Application Registration Portal]</a>.</p> <p>Per ogni ambito, fare clic su <b>[!UICONTROL Add]</b> e digita l’autorizzazione.</p> <p>Esempio: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Separatore ambito]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID client]</td> 
      <td>Immetti l'ID applicazione [!UICONTROL] dal passaggio 2 in <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrati [!DNL Workfront Fusion] nel [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segreto client]</td> 
      <td>Immettere il [!UICONTROL Segreto applicazione] generato al passaggio 2 in <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrati [!DNL Workfront Fusion] nel [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autorizza parametri]</td> 
      <td> <p>Aggiungi i seguenti parametri di autorizzazione:</p> 
       <ul> 
        <li> <p>[!UICONTROL Key]:<code> response_mode</code> Valore [!UICONTROL]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL Key]: <code>prompt </code>Valore [!UICONTROL]: <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parametri token di accesso]</td> 
      <td>Non è necessario immettere alcun valore in questo campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Aggiorna parametri token]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Clic <b>[!UICONTROL Add]</b>.</p> </li> 
        <li value="2"> <p>In <b>[!UICONTROL Key]</b> campo, immetti <code>scope</code>.</p> </li> 
        <li value="3"> <p>In <b>Valore [!UICONTROL]</b> , immettere tutti gli [!UICONTROL scope]i immessi nel campo di ambito, separati da spazi.</p> <p>Esempio: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Intestazioni personalizzate]</td> 
      <td>Non è necessario immettere alcun valore in questo campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Placement]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Continua]**.
1. Nella finestra visualizzata, fai clic su **[!UICONTROL Accetta]** per completare la connessione e tornare al modulo.
