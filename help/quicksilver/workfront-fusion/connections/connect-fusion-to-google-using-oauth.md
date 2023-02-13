---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzo di un client OAuth personalizzato
description: È possibile utilizzare [!DNL Adobe Workfront Fusion] per connettersi a [!DNL Google Services] utilizzando un client OAuth personalizzato. Questa procedura richiede un [!DNL Google] conto.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzo di un client OAuth personalizzato

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

## Prerequisiti

È necessario un [!DNL Google] per effettuare la connessione.

## Crea un progetto in [!DNL Google Cloud Platform]

La seguente procedura è destinata a:

* Uso personale ([!DNL @gmail.com] e [!DNL @googlemail.com] utenti)
* Uso interno ([!DNL G Suite] utenti che preferiscono utilizzare un client OAuth personalizzato)

Per creare un progetto su [!DNL Google Cloud] Piattaforma:

1. Accedi a [[!DNL Google Cloud] Piattaforma](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) utilizzando [!DNL Google] credenziali.
1. Nel pannello a sinistra, fai clic su **[!UICONTROL Dashboard]**.
1. Fai clic su **[!UICONTROL Crea progetto]** nell&#39;angolo superiore destro dello schermo.
1. Inserisci il **[!UICONTROL Nome del progetto]**, quindi fai clic su **[!UICONTROL Crea]**.

1. Fai clic sul pulsante **[!UICONTROL Abilitare API e servizi]** nella parte superiore dello schermo.
1. In **[!UICONTROL Cercare API e servizi]** nella parte superiore dello schermo, digitare il nome del servizio che si desidera utilizzare, ad esempio [!DNL Gmail] API o [!DNL Google Drive] API).
1. Quando viene visualizzato, fai clic sull’API o sul servizio a cui desideri connetterti [!DNL Workfront Fusion].
1. Fai clic su **[!UICONTROL Abilita]** per abilitare l’API selezionata.
1. Ripeti i passaggi 6-8 per ogni API da abilitare.

   >[!NOTE]
   >
   >È necessario attivare [!DNL Google Drive] API e API di tutti [!DNL Google] app che desideri utilizzare (ad esempio [!DNL Google Sheets] API).

1. Nella schermata visualizzata, fai clic su **[!UICONTROL Creare le credenziali]** nell&#39;angolo in alto a destra.
1. Passa alla sezione . [Configurare le impostazioni di consenso OAuth](#configure-oauth-consent-settings) in questo articolo.

## Configura [!UICONTROL Consenso OAuth] impostazioni

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Schermata di consenso OAuth]**.
1. Seleziona **[!UICONTROL Esterno]**, quindi fai clic su **[!UICONTROL Crea]**.

   >[!NOTE]
   >
   >Non verrà addebitato alcun importo quando si seleziona questa opzione. Per ulteriori informazioni, consulta [!DNL Google]Informazioni sulle eccezioni ai requisiti di verifica.

1. Compila i campi richiesti come segue:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App name]</p> </td> 
      <td> <p>Immetti il nome dell’app che richiede il consenso.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">E-mail di supporto utente di [!UICONTROL]</td> 
      <td>Immetti un indirizzo e-mail in cui gli utenti possano contattarti per eventuali domande sul loro consenso durante la connessione a questa app.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Indirizzi e-mail]</td> 
      <td>Inserisci uno o più indirizzi e-mail che Google può utilizzare per notificare all’utente eventuali modifiche al progetto.</td> 
     </tr> 
    </tbody> 
   </table>

1. Sotto [!UICONTROL Domini autorizzati], fai clic su **[!UICONTROL Aggiungi dominio]** e immetti `workfrontfusion.com`.

1. Fai clic su **[!UICONTROL Salva e continua]**.
1. Fai clic su **[!UICONTROL Aggiungi o rimuovi ambiti]**.
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

Potrebbe essere necessario espandere l’elenco o passare alla pagina successiva dell’elenco per visualizzarli tutti.

1. Fai clic su **[!UICONTROL Aggiorna]**.
1. Fai clic su **[!UICONTROL Salva e continua]**.
1. (Facoltativo) Aggiungi eventuali utenti di test al progetto.
1. Fai clic su **[!UICONTROL Salva e continua]**.
1. Esamina le informazioni per verificarne l&#39;accuratezza, quindi fai clic su **[!UICONTROL Torna al dashboard]**.

   >[!NOTE]
   >
   >Non è necessario inviare la schermata di consenso e la domanda per la verifica tramite [!DNL Google].

1. Continua a [Creare credenziali OAuth](#create-oauth-credentials).

## Creare credenziali OAuth

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Credenziali]**.

   >[!NOTE]
   >
   >Se non è la prima API o servizio ([!DNL Gmail] o [!DNL Google Drive]) è stata abilitata, non è necessario creare nuove credenziali.

1. Fai clic su **[!UICONTROL Creare le credenziali]** vicino alla parte superiore dello schermo, quindi seleziona **[!UICONTROL ID client OAuth]** dal menu a discesa.

1. Compila i campi richiesti come segue:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo di applicazione]</td> 
      <td> <p> [!UICONTROL Web application]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. Sotto [!UICONTROL URI di reindirizzamento autorizzati], fai clic su **[!UICONTROL Aggiungi URI]** e immetti **uno** dei seguenti elementi:

   * Per [!DNL Gmail] o [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Per altri [!DNL Google] app: `https://app.workfrontfusion.com/oauth/cb/google`

1. Fai clic su **[!UICONTROL Crea]**.

   La [!UICONTROL ID client] e [!UICONTROL Segreto client] visualizzazione.

1. Copia il [!UICONTROL ID client] e [!UICONTROL Segreto client] in una posizione sicura. Le utilizzerai per creare una connessione in [!DNL Workfront Fusion].
1. Continua a [Connetti a [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

## Connetti a [!DNL Google] in [!DNL Workfront Fusion]

Processo di creazione di una connessione a [!DNL Google] differisce a seconda che si utilizzi un modulo da un [!DNL Google] il servizio [!DNL Google Sheets] o [!DNL Google Docs]) o se ti connetti a [!DNL Google] tramite [!UICONTROL HTTP] >[!UICONTROL Creare un OAuth2.0] modulo di richiesta.

* [Connetti a [!DNL Google] in [!DNL Google] servizio](#connect-to-google-in-a-google-service)
* [Connetti a [!DNL Google] in [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth2.0] modulo](#connect-to-google-in-the-http--make-an-oauth20-request-module)

### Connetti a [!DNL Google] in [!DNL Google] servizio

1. In [!DNL Workfront Fusion], individua la [!DNL Google] modulo per il quale è necessario creare una connessione.
1. Fai clic su **[!UICONTROL Creare una connessione]**, quindi fai clic su **[!UICONTROL Mostra impostazioni avanzate]**.

1. Inserisci il [!UICONTROL ID client] e [!UICONTROL Segreto client] hai recuperato in [[!UICONTROL Creare credenziali OAuth]](#create-oauth-credentials) nei rispettivi campi, quindi fai clic su **[!UICONTROL Continua]**.

1. Accedi con il tuo [!DNL Google] conto.

   La **[!UICONTROL Questa app non è verificata]** viene visualizzata la finestra . L’&quot;app&quot; menzionato nel titolo della finestra è il client OAuth che hai creato in precedenza.

1. Fai clic su **[!UICONTROL Avanzate]**, quindi fai clic su **[!UICONTROL Vai a [!DNL Workfront Fusion] (non sicuro)]** per consentire l’accesso tramite il client OAuth personalizzato.

1. Fai clic su **[!UICONTROL Consenti]** concedere [!DNL Workfront Fusion] autorizzazione.
1. Nella finestra visualizzata, fai clic su **[!UICONTROL Consenti]** di nuovo per confermare le scelte.

   Il collegamento al [!DNL Google] è stabilito il servizio che utilizza un client OAuth personalizzato.

### Connetti a [!DNL Google] in [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth2.0] modulo {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Per istruzioni su come collegarsi a [!DNL Google] in [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth2.0] modulo, vedi [Istruzioni per la creazione di una connessione a [!DNL Google] in [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instruct) in [[!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Possibile messaggio di errore:[!UICONTROL [403] Accesso non configurato]

Se la [!UICONTROL [403] Accesso non configurato] viene visualizzato un messaggio di errore, è necessario abilitare l’API corrispondente nella piattaforma Google Cloud. Per abilitare l’API, segui i passaggi descritti nella sezione . [Crea un progetto in [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) in questo articolo.
