---
title: Chiama l'API REST di MS Graph tramite il  [!DNL Adobe Workfront Fusion] HTTP &gt; Crea un modulo di richiesta OAuth 2.0
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 1%

---

# Chiama l&#39;API REST di MS Graph  tramite [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Crea una richiesta OAuth 2.0]

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Chiama l&#39;API REST di MS Graph](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/call-the-ms-graph-rest-api.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

<!-- Audited: 3/2024-->

Molti servizi Web di [!DNL Microsoft] sono accessibili tramite [!DNL Microsoft Graph API]. È possibile creare una connessione a [!DNL Microsoft Graph API] utilizzando [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Creare una richiesta OAuth 2.0].

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> <p>Nuovo: [!UICONTROL Standard]</p><p>Oppure</p><p>Corrente: [!UICONTROL Work] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Corrente: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Legacy: qualsiasi </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Nuovo:</p> <ul><li>Piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Workfront]: l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Il piano [!DNL Workfront Fusion] è incluso.</li></ul>
   <p>Oppure</p>
   <p>Corrente: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Registra [!DNL Workfront Fusion] in [!DNL Microsoft Application Registration Portal]

Per creare una connessione a [!DNL Microsoft Graph REST API], è necessario prima registrare [!DNL Adobe Workfront Fusion].

1. Inizia a registrare una nuova applicazione come descritto in [Registra l&#39;app](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) nella documentazione di [!DNL Microsoft].

   Come parte della registrazione, [!DNL Microsoft] richiede le seguenti informazioni:

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Nome applicazione]</td>
        <td>Immettere un nome per l'applicazione, ad esempio "Applicazione [!DNL Workfront Fusion] personale".</td>
      </tr>
      <tr>
        <td>[!UICONTROL URL di reindirizzamento]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. Dopo aver completato la registrazione dell&#39;app, annota [!UICONTROL ID applicazione].

   >[!IMPORTANT]
   >
   >Per configurare la connessione in [!DNL Workfront Fusion] è necessario l&#39;ID applicazione.

1. Genera un [!UICONTROL segreto applicazione]. Prendi nota di questo segreto.

   Per istruzioni, consulta [Registrare l&#39;app](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) nella documentazione di [!DNL Microsoft].

   >[!IMPORTANT]
   >
   >Per configurare la connessione in [!DNL Workfront Fusion] è necessario il [!UICONTROL Segreto applicazione].

1. Configura le autorizzazioni per l’applicazione.

   Per informazioni specifiche su come individuare e configurare questi campi, vedere la sezione &quot;Configurare le autorizzazioni per Microsoft Graph&quot; in [Ottenere l&#39;accesso senza un utente](https://docs.microsoft.com/en-us/graph/auth-v2-service) nella documentazione di [!UICONTROL Microsoft].

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Quale tipo di autorizzazioni sono necessarie per l'applicazione?]</td> 
      <td>Selezionare <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Seleziona autorizzazioni]</td> 
      <td> <p>Seleziona le seguenti autorizzazioni:</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Qualsiasi altra autorizzazione richiesta dalle integrazioni (Esempio: <code>User.Read</code>)</p> </li> 
       </ul> <p><b>Importante</b>: per configurare la connessione in [!DNL Workfront Fusion] saranno necessarie le autorizzazioni selezionate.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Procedi a [Configurare la tua connessione [!DNL MS Graph API] in [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Configura la connessione [!DNL MS Graph API] in [!DNL Workfront Fusion]

Dopo aver registrato [!DNL Workfront Fusion] come descritto in [Registra [!DNL Workfront Fusion]  in  [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal), puoi configurare la connessione in [!UICONTROL HTTP] > [!UICONTROL Crea un modulo di richiesta Oauth 2.0].

1. Aggiungi un modulo [!UICONTROL HTTP] > [!UICONTROL Esegui una chiamata OAuth 2.0] allo scenario.
1. Fai clic su **[!UICONTROL Aggiungi]** accanto al campo [!UICONTROL connessione].
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
      <td> <p>Immettere le autorizzazioni selezionate al passaggio 4 di <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registra [!DNL Workfront Fusion] in [!DNL Microsoft Application Registration Portal]</a>.</p> <p>Per ogni ambito, fare clic su <b>[!UICONTROL Add]</b> e digitare l'autorizzazione.</p> <p>Esempio: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Separatore ambito]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID client]</td> 
      <td>Immetti l'ID applicazione [!UICONTROL] dal passaggio 2 in <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registra [!DNL Workfront Fusion] in [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segreto client]</td> 
      <td>Immettere il [!UICONTROL Segreto applicazione] generato al passaggio 3 in <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registra [!DNL Workfront Fusion] in [!DNL Microsoft Application Registration Portal]</a>.</td> 
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
      <td role="rowheader">[!UICONTROL Parametri token di accesso]</td> 
      <td>Non è necessario immettere alcun valore in questo campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Aggiorna parametri token]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Fare clic su <b>[!UICONTROL Add]</b>.</p> </li> 
        <li value="2"> <p>Nel campo <b>[!UICONTROL Key]</b>, immettere <code>scope</code>.</p> </li> 
        <li value="3"> <p>Nel campo <b>[!UICONTROL Valore]</b> immettere tutti gli ambiti [!UICONTROL] immessi nel campo di ambito, separati da spazi.</p> <p>Esempio: <code>offline_access openid User.Read</code></p> </li> 
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

1. Fai clic su **[!UICONTROL Continua]**.
1. Nella finestra visualizzata, fai clic su **[!UICONTROL Accetta]** per completare la connessione e tornare al modulo.
