---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzo di un client OAuth personalizzato
description: È possibile utilizzare [!DNL Adobe Workfront Fusion] per connettersi a [!DNL Google Services] utilizzo di un client OAuth personalizzato. Questa procedura richiede un [!DNL Google] account.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '947'
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

## Prerequisiti

È necessario un [!DNL Google] per effettuare questa connessione.

## Crea un progetto su [!DNL Google Cloud Platform]

La seguente procedura è destinata a:

* Uso personale ([!DNL @gmail.com] e [!DNL @googlemail.com] utenti)
* Uso interno ([!DNL G Suite] utenti che preferiscono utilizzare un client OAuth personalizzato)

Per creare un progetto su [!DNL Google Cloud] Piattaforma

1. Accedi a [[!DNL Google Cloud] Piattaforma](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) utilizzando [!DNL Google] credenziali.
1. Nel pannello a sinistra, fai clic su **[!UICONTROL Dashboard]**.
1. Clic **[!UICONTROL Crea progetto]** nell&#39;angolo superiore destro dello schermo.
1. Inserisci il **[!UICONTROL Nome progetto]**, quindi fai clic su **[!UICONTROL Crea]**.

1. Fai clic su **[!UICONTROL Abilitare API e servizi]** nella parte superiore dello schermo.
1. In **[!UICONTROL Ricerca di API e servizi]** nella parte superiore della schermata, digita il nome del servizio che desideri utilizzare (ad esempio [!DNL Gmail] API o [!DNL Google Drive] API).
1. Quando viene visualizzato, fai clic sull’API o sul servizio a cui desideri connetterti [!DNL Workfront Fusion].
1. Clic **[!UICONTROL Abilita]** per abilitare l’API selezionata.
1. Ripeti i passaggi da 6 a 8 per ogni API che desideri abilitare.

   >[!NOTE]
   >
   >Devi abilitare [!DNL Google Drive] API e l’API di tutti [!DNL Google] app che desideri utilizzare (ad esempio [!DNL Google Sheets] API).

1. Nella schermata visualizzata, fai clic su **[!UICONTROL Crea credenziali]** nell’angolo superiore destro.
1. Passa alla sezione [Configurare le impostazioni di consenso OAuth](#configure-oauth-consent-settings) in questo articolo.

## Configura [!UICONTROL Consenso OAuth] impostazioni

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Schermata di consenso OAuth]**.
1. Seleziona **[!UICONTROL Esterno]**, quindi fai clic su **[!UICONTROL Crea]**.

   >[!NOTE]
   >
   >Selezionando questa opzione non verrà addebitato alcun importo. Per ulteriori informazioni, consulta [!DNL Google]informazioni di su eccezioni ai requisiti di verifica.

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

1. Sotto [!UICONTROL Domini autorizzati], fai clic su **[!UICONTROL Aggiungi dominio]**, e immetti `workfrontfusion.com`.

1. Clic **[!UICONTROL Salva e continua]**.
1. Clic **[!UICONTROL Aggiungere o rimuovere ambiti]**.
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

1. Clic **[!UICONTROL Aggiorna]**.
1. Clic **[!UICONTROL Salva e continua]**.
1. (Facoltativo) Aggiungi eventuali utenti di test al progetto.
1. Clic **[!UICONTROL Salva e continua]**.
1. Verifica la precisione delle informazioni, quindi fai clic su **[!UICONTROL Torna alla dashboard]**.

   >[!NOTE]
   >
   >Non è necessario inviare la schermata di consenso e la richiesta di verifica entro il [!DNL Google].

1. Continua con [Crea credenziali OAuth](#create-oauth-credentials).

## Crea credenziali OAuth

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Credenziali]**.

   >[!NOTE]
   >
   >Se non si tratta della prima API o del primo servizio ([!DNL Gmail] o [!DNL Google Drive]) è stata attivata, non è necessario creare nuove credenziali.

1. Clic **[!UICONTROL Crea credenziali]** nella parte superiore dello schermo, quindi seleziona **[!UICONTROL ID client OAuth]** dal menu a discesa.

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

1. Sotto [!UICONTROL URI di reindirizzamento autorizzati], fai clic su **[!UICONTROL Aggiungi URI]** e immetti **uno** dei seguenti elementi:

   * Per [!DNL Gmail] o [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Per altri [!DNL Google] app: `https://app.workfrontfusion.com/oauth/cb/google`

1. Fai clic su **[!UICONTROL Crea]**.

   Il [!UICONTROL ID client] e [!UICONTROL Segreto client] visualizzazione.

1. Copia il [!UICONTROL ID client] e [!UICONTROL Segreto client] in un luogo sicuro. Le utilizzerai per effettuare una connessione in [!DNL Workfront Fusion].
1. Continua con [Connetti a [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

## Connetti a [!DNL Google] in [!DNL Workfront Fusion]

Processo di creazione di una connessione a [!DNL Google] varia a seconda che si utilizzi un modulo di da un [!DNL Google] servizio (ad esempio [!DNL Google Sheets] o [!DNL Google Docs]) o se ti stai connettendo a [!DNL Google] tramite [!UICONTROL HTTP] >[!UICONTROL Creare un OAuth2.0] modulo di richiesta.

* [Connetti a [!DNL Google] in un [!DNL Google] servizio](#connect-to-google-in-a-google-service)
* [Connetti a [!DNL Google] nel [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth2.0] modulo](#connect-to-google-in-the-http--make-an-oauth20-request-module)

### Connetti a [!DNL Google] in un [!DNL Google] servizio

1. In entrata [!DNL Workfront Fusion], individua [!DNL Google] modulo di cui hai bisogno per creare una connessione.
1. Clic **[!UICONTROL Creare una connessione]**, quindi fai clic su **[!UICONTROL Mostra impostazioni avanzate]**.

1. Inserisci il [!UICONTROL ID client] e [!UICONTROL Segreto client] recuperato in [[!UICONTROL Crea credenziali OAuth]](#create-oauth-credentials) nei rispettivi campi, quindi fai clic su **[!UICONTROL Continua]**.

1. Accedi con il [!DNL Google] account.

   Il **[!UICONTROL Questa app non è verificata]** viene visualizzata la finestra. Tieni presente che l’&quot;app&quot; indicata nel titolo della finestra è il client OAuth creato in precedenza.

1. Clic **[!UICONTROL Avanzate]**, quindi fai clic su **[!UICONTROL Vai a [!DNL Workfront Fusion] (non sicuro)]** per consentire l’accesso utilizzando il client OAuth personalizzato.

1. Clic **[!UICONTROL Consenti]** da concedere [!DNL Workfront Fusion] autorizzazione.
1. Nella finestra visualizzata, fai clic su **[!UICONTROL Consenti]** per confermare le scelte.

   La connessione al [!DNL Google] è stato stabilito un servizio che utilizza un client OAuth personalizzato.

### Connetti a [!DNL Google] nel [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth2.0] modulo {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Per istruzioni sulla connessione a [!DNL Google] nel [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth2.0] modulo, vedi [Istruzioni per la creazione di una connessione a [!DNL Google] nel [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instruct) in [[!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Possibile messaggio di errore:[!UICONTROL [403] Accesso non configurato]

Se il [!UICONTROL [403] Accesso non configurato] viene visualizzato un messaggio di errore, è necessario abilitare l’API corrispondente nella piattaforma Google Cloud. Per abilitare l’API, segui i passaggi descritti nella sezione [Crea un progetto su [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) in questo articolo.
