---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] tramite un client OAuth personalizzato
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 0%

---

# Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzando un client OAuth personalizzato

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Connettere Adobe Workfront Fusion a Google Services utilizzando un client OAuth personalizzato](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-fusion-to-google-using-oauth.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

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

## Prerequisiti

Per effettuare questa connessione è necessario un account [!DNL Google] esistente.

## Connettere Fusion ai servizi Google utilizzando un client OAuth personalizzato

Per creare questa connessione, devi creare e configurare un progetto sulla piattaforma Google Cloud, quindi configurare la connessione in Fusion in base a tale progetto.

* [Crea un progetto in  [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)
* [Configura [!UICONTROL Impostazioni consenso OAuth]](#configure-oauth-consent-settings)
* [Crea credenziali OAuth](#create-oauth-credentials)
* [Connetti a [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>Questa procedura è destinata:
>
>* Uso personale ([!DNL `@gmail.com`] e [!DNL `@googlemail.com`] utenti)
>* Uso interno ([!DNL Google Workspace] utenti che preferiscono utilizzare un client OAuth personalizzato)

### Crea un progetto su [!DNL Google Cloud Platform]

Per creare un progetto sulla piattaforma [!DNL Google Cloud]:

1. Accedi a [[!DNL Google Cloud] Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) utilizzando le tue credenziali [!DNL Google].
1. Nel pannello a sinistra, fai clic su **[!UICONTROL Dashboard]**.
1. Fai clic su **[!UICONTROL Crea progetto]** nell&#39;angolo superiore destro della schermata.
1. Immetti il **[!UICONTROL nome progetto]**, quindi fai clic su **[!UICONTROL Crea]**.

1. Fai clic sulla scheda **[!UICONTROL Abilita API e servizi]** nella parte superiore dello schermo.
1. Nel campo **[!UICONTROL Cerca API e servizi]** nella parte superiore della schermata, digitare il nome del servizio che si desidera utilizzare, ad esempio [!DNL Gmail] API o [!DNL Google Drive] API.
1. Quando viene visualizzato, fare clic sull&#39;API o sul servizio a cui si desidera connettersi [!DNL Workfront Fusion].
1. Fai clic su **[!UICONTROL Abilita]** per abilitare l&#39;API selezionata.
1. Ripeti i passaggi da 6 a 8 per ogni API che desideri abilitare.

   >[!NOTE]
   >
   >È necessario abilitare l&#39;API [!DNL Google Drive] e l&#39;API di tutte le app [!DNL Google] che si desidera utilizzare (ad esempio l&#39;API [!DNL Google Sheets]).

1. Nella schermata visualizzata, fai clic su **[!UICONTROL Crea credenziali]** nell&#39;angolo superiore destro.
1. Passa alla sezione [Configurare le impostazioni del consenso OAuth](#configure-oauth-consent-settings) in questo articolo.

### Configura impostazioni [!UICONTROL consenso OAuth]

1. Nel pannello a sinistra, fai clic sulla **[!UICONTROL schermata di consenso OAuth]**.
1. Seleziona **[!UICONTROL External]**, quindi fai clic su **[!UICONTROL Create]**.

   >[!NOTE]
   >
   >Selezionando questa opzione non verrà addebitato alcun importo. Per ulteriori informazioni, vedere le informazioni di [!DNL Google] sulle eccezioni ai requisiti di verifica.

1. Compila i campi obbligatori come segue:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome app]</p> </td> 
      <td> <p>Inserisci il nome dell’app che richiede il consenso.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL User support email]</td> 
      <td>Immetti un indirizzo e-mail che gli utenti dovranno contattare per eventuali domande sul consenso durante la connessione a questa app.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Indirizzi e-mail]</td> 
      <td>Immetti uno o più indirizzi e-mail che Google può utilizzare per informarti di eventuali modifiche al progetto.</td> 
     </tr> 
    </tbody> 
   </table>

1. In [!UICONTROL Domini autorizzati], fare clic su **[!UICONTROL Aggiungi dominio]** e immettere `workfrontfusion.com`.

1. Fai clic su **[!UICONTROL Salva e continua]**.
1. Fare clic su **[!UICONTROL Aggiungi o rimuovi ambiti]**.
1. Nel pannello a destra, abilita i seguenti ambiti:

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Servizio/API</th> 
      <th>Ambiti richiesti</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p>[!DNL Gmail]</p> </td> 
      <td> <p>https://mail.google.com/</p> <p>https://www.googleapis.com/auth/gmail.labels</p> <p>https://www.googleapis.com/auth/gmail.send</p> <p>https://www.googleapis.com/auth/gmail.readonly</p> <p>https://www.googleapis.com/auth/gmail.compose</p> <p>https://www.googleapis.com/auth/gmail.insert</p> <p>https://www.googleapis.com/auth/gmail.modify</p> <p>https://www.googleapis.com/auth/gmail.metadata</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!DNL Google Drive]</p> </td> 
      <td> <p>https://www.googleapis.com/auth/drive</p> <p>https://www.googleapis.com/auth/drive.readonly</p> </td> 
     </tr> 
    </tbody> 
   </table>

Potrebbe essere necessario espandere l&#39;elenco o passare alla pagina successiva dell&#39;elenco per visualizzarli tutti.

1. Fai clic su **[!UICONTROL Aggiorna]**.
1. Fai clic su **[!UICONTROL Salva e continua]**.
1. (Facoltativo) Aggiungi eventuali utenti di test al progetto.
1. Fai clic su **[!UICONTROL Salva e continua]**.
1. Verifica la precisione delle informazioni, quindi fai clic su **[!UICONTROL Torna al dashboard]**.

   >[!NOTE]
   >
   >Non è necessario inviare la schermata di consenso e la richiesta di verifica da [!DNL Google].

1. Continua con [Crea credenziali OAuth](#create-oauth-credentials).

### Crea credenziali OAuth

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Credenziali]**.

   >[!NOTE]
   >
   >Se non si tratta della prima API o del primo servizio ([!DNL Gmail] o [!DNL Google Drive]) abilitato, non è necessario creare nuove credenziali.

1. Fai clic su **[!UICONTROL Crea credenziali]** nella parte superiore dello schermo, quindi seleziona **[!UICONTROL ID client OAuth]** dal menu a discesa.

1. Compila i campi obbligatori come segue:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo di applicazione]</td> 
      <td> <p> [!UICONTROL Applicazione Web]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. In [!UICONTROL URI di reindirizzamento autorizzati], fare clic su **[!UICONTROL Aggiungi URI]** e immettere **uno** dei seguenti elementi:

   * Per [!DNL Gmail] o [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Per altre [!DNL Google] app: `https://app.workfrontfusion.com/oauth/cb/google`

1. Fai clic su **[!UICONTROL Crea]**.

   [!UICONTROL ID client] e [!UICONTROL Segreto client] vengono visualizzati.

1. Copiare l&#39;[!UICONTROL ID client] e il [!UICONTROL Segreto client] in un percorso sicuro. Le utilizzerai per stabilire una connessione in [!DNL Workfront Fusion].
1. Continua a [Connettiti a [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

### Connetti a [!DNL Google] in [!DNL Workfront Fusion]

Il processo di creazione di una connessione a [!DNL Google] varia a seconda che si stia utilizzando un modulo di un servizio [!DNL Google] (ad esempio [!DNL Google Sheets] o [!DNL Google Docs]) o che si stia effettuando la connessione a [!DNL Google] tramite [!UICONTROL HTTP] >[!UICONTROL Creare un modulo di richiesta OAuth2.0].

* [Connetti a  [!DNL Google]  in un servizio  [!DNL Google] ](#connect-to-google-in-a-google-service)
* [Connetti a [!DNL Google] nel modulo [!UICONTROL HTTP] > [!UICONTROL Crea una richiesta OAuth2.0]](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### Connetti a [!DNL Google] in un servizio [!DNL Google]

1. In [!DNL Workfront Fusion], individuare il modulo [!DNL Google] per il quale è necessario creare una connessione.
1. Fai clic su **[!UICONTROL Crea una connessione]**, quindi su **[!UICONTROL Mostra impostazioni avanzate]**.

1. Immetti [!UICONTROL ID client] e [!UICONTROL Segreto client] recuperati in [[!UICONTROL Crea credenziali OAuth]](#create-oauth-credentials) nei rispettivi campi, quindi fai clic su **[!UICONTROL Continua]**.

1. Accedi con il tuo account [!DNL Google].

   Viene visualizzata la finestra **[!UICONTROL L&#39;app non è verificata]**. Tieni presente che l’&quot;app&quot; indicata nel titolo della finestra è il client OAuth creato in precedenza.

1. Fai clic su **[!UICONTROL Avanzate]**, quindi fai clic su **[!UICONTROL Vai a [!DNL Workfront Fusion] (non sicuro)]** per consentire l&#39;accesso utilizzando il client OAuth personalizzato.

1. Fare clic su **[!UICONTROL Consenti]** per concedere l&#39;autorizzazione [!DNL Workfront Fusion].
1. Nella finestra visualizzata, fai di nuovo clic su **[!UICONTROL Consenti]** per confermare le scelte effettuate.

   È stata stabilita la connessione al servizio [!DNL Google] desiderato utilizzando un client OAuth personalizzato.

#### Connettiti a [!DNL Google] nel modulo [!UICONTROL HTTP] > [!UICONTROL Crea una richiesta OAuth2.0] {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Per istruzioni sulla connessione a [!DNL Google] nel modulo [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth2.0], vedere [Istruzioni per la creazione di una connessione a  [!DNL Google] nel modulo [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0]](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module) in [[!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0]](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Possibile messaggio di errore:[!UICONTROL [403] Accesso non configurato]

Se viene visualizzato il messaggio di errore [!UICONTROL `403 Access Not Configured`], devi abilitare l&#39;API corrispondente nella piattaforma Google Cloud. Per abilitare l&#39;API, segui i passaggi descritti nella sezione [Creare un progetto su [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) in questo articolo.
