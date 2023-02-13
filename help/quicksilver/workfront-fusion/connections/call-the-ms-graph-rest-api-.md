---
title: Chiama l’API REST di MS Graph tramite [!DNL Adobe Workfront Fusion] HTTP &gt; Creare un modulo di richiesta OAuth 2.0
description: Chiama l’API REST di MS Graph tramite [!DNL Adobe Workfront Fusion] HTTP &gt; Creare un modulo di richiesta OAuth 2.0
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 1%

---

# Chiama il[!UICONTROL  API REST di MS Graph] tramite [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo

Molti [!DNL Microsoft] i servizi web sono accessibili tramite [!DNL Microsoft Graph API]. Questo articolo descrive come creare una connessione a tale API utilizzando [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo .

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr>
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Registro [!DNL Workfront Fusion] in [!DNL Microsoft Application Registration Portal]

Per creare una connessione a [!DNL Microsoft Graph REST API], è necessario prima registrarsi [!DNL Adobe Workfront Fusion].

1. Inizia la registrazione di una nuova applicazione come descritto in [Registra l&#39;app](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) in [!DNL Microsoft] documentazione.

   Come parte della registrazione, [!DNL Microsoft] richiede le seguenti informazioni:

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

1. Una volta completata la registrazione dell’app, prendi nota della [!UICONTROL ID applicazione].

   >[!IMPORTANT]
   >
   >Per impostare la connessione in è necessario l&#39;ID applicazione [!DNL Workfront Fusion].

1. Genera un [!UICONTROL Segreto applicazione]. Prendi nota di questo segreto.

   Per istruzioni, consulta [Registra l&#39;app](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) in [!DNL Microsoft] documentazione.

   >[!IMPORTANT]
   >
   >Avrai bisogno di [!UICONTROL Segreto applicazione] per impostare la connessione in [!DNL Workfront Fusion].

1. Configura le autorizzazioni per l&#39;applicazione.

   Per informazioni specifiche su come individuare e configurare questi campi, consulta la sezione &quot;Configurare le autorizzazioni per Microsoft Graph&quot; in [Ottenere l&#39;accesso senza un utente](https://docs.microsoft.com/en-us/graph/auth-v2-service) in [!UICONTROL Microsoft] documentazione.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Che tipo di autorizzazioni richiede la tua applicazione?]</td> 
      <td>Seleziona <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Selezionare le autorizzazioni]</td> 
      <td> <p>Seleziona le seguenti autorizzazioni:</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Eventuali altre autorizzazioni richieste dalle integrazioni (esempio: <code>User.Read</code>)</p> </li> 
       </ul> <p>Importante: Per impostare la connessione in è necessario disporre delle autorizzazioni selezionate [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Procedi a [Configura le [!DNL MS Graph API] connessione [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Configura le [!DNL MS Graph API] connessione [!DNL Workfront Fusion]

Dopo la registrazione [!DNL Workfront Fusion] discussi in [Registro [!DNL Workfront Fusion] in [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal), è possibile configurare la connessione in [!UICONTROL HTTP] >[!UICONTROL Crea un Oauth 2.0] modulo di richiesta.

1. Aggiungi un [!UICONTROL HTTP] >[!UICONTROL Effettuare una chiamata OAuth 2.0] al tuo scenario.
1. Fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL connection] campo .
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
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Flow type]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URI autorizzazione]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ambito [!UICONTROL]</td> 
      <td> <p>Immetti le autorizzazioni selezionate al passaggio 4 di <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registro [!DNL Workfront Fusion] in [!DNL Microsoft Application Registration Portal]</a>.</p> <p>Per ogni ambito, fai clic su <b>[!UICONTROL Aggiungi]</b> e digita l'autorizzazione.</p> <p>Esempio: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Separatore di ambito]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ID client [!UICONTROL]</td> 
      <td>Immetti l’ [!UICONTROL Application ID] dal passaggio 2 in <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registro [!DNL Workfront Fusion] in [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segreto client]</td> 
      <td>Inserisci il [!UICONTROL Application Secret] generato al punto 2 in <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registro [!DNL Workfront Fusion] in [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autorizza parametri]</td> 
      <td> <p>Aggiungi i seguenti parametri di autorizzazione:</p> 
       <ul> 
        <li> <p>[!UICONTROL Key]:<code> response_mode</code> [!UICONTROL Value]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL Key]: <code>prompt </code>[!UICONTROL Value]: <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Access token parameters]</td> 
      <td>Non è necessario inserire nulla in questo campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Aggiorna parametri token]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Fai clic su <b>[!UICONTROL Aggiungi]</b>.</p> </li> 
        <li value="2"> <p>In <b>[!UICONTROL Key]</b> campo, immettere <code>scope</code>.</p> </li> 
        <li value="3"> <p>In <b>[!UICONTROL Value]</b> immetti tutti gli [!UICONTROL scope]s immessi nel campo ambito, separati da spazi.</p> <p>Esempio: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Intestazioni personalizzate]</td> 
      <td>Non è necessario inserire nulla in questo campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Placement]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Continua]**.
1. Nella finestra visualizzata, fai clic su **[!UICONTROL Accetta]** per completare la connessione e tornare al modulo .
