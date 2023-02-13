---
title: Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Come [!DNL Adobe Workfront] amministratore, puoi creare applicazioni OAuth2 per la tua istanza di [!DNL Workfront], che consente ad altre applicazioni di accedere a Workfront. Gli utenti possono quindi concedere l’autorizzazione a tali altre applicazioni per accedere ai propri dati Workfront. In questo modo, è possibile integrare Workfront con applicazioni a scelta, incluse le applicazioni interne.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: f7e3182776e6b62103cd755b2fbd5057efc95394
workflow-type: tm+mt
source-wordcount: '1917'
ht-degree: 6%

---

# Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni

Come [!DNL Adobe Workfront] amministratore, puoi creare applicazioni OAuth2 per la tua istanza di [!DNL Workfront], che consentono l&#39;accesso ad altre applicazioni [!DNL Workfront]. Gli utenti possono quindi concedere l&#39;autorizzazione a tali altre applicazioni per accedere ai loro [!DNL Workfront] dati. In questo modo, è possibile integrarsi con le applicazioni preferite, incluse quelle interne.

Quando crei un [!UICONTROL OAuth2] genera un ID client e un segreto client. Gli utenti possono quindi utilizzare l’ID client nelle chiamate API per integrarsi con l’applicazione creata.

>[!NOTE]
>
>Nel contesto di OAuth2, per &quot;creazione di un’app&quot; si intende il processo di creazione di questo tipo di collegamento di accesso tra un’app e un server come [!DNL Workfront].

* Per istruzioni su come configurare e utilizzare l’applicazione OAuth2 con le credenziali utente (flusso di codice di autorizzazione), consulta [Configura e utilizza le applicazioni personalizzate OAuth 2 della tua organizzazione utilizzando il flusso di codice di autorizzazione](../../wf-api/api/oauth-app-code-token-flow.md).
* Per istruzioni su come configurare e utilizzare l’applicazione OAuth2 utilizzando l’autenticazione server (flusso JWT), consulta [Configura e utilizza le applicazioni personalizzate OAuth 2 della tua organizzazione utilizzando il flusso JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Per istruzioni su come configurare e utilizzare l’applicazione OAuth2 utilizzando PKCE, consulta [Configura e utilizza le applicazioni personalizzate OAuth 2 della tua organizzazione utilizzando il flusso PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> Devi essere un [!DNL Workfront] amministratore. </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Panoramica di OAuth2

Immagina che un&#39;applicazione debba estrarre alcune informazioni specifiche da [!DNL Workfront]. Un&#39;applicazione che richiede informazioni viene chiamata client. In questo esempio, il nome client è ClientApp. ClientApp deve accedere alle informazioni di un particolare utente e deve quindi accedere a [!DNL Workfront] come utente. Se l&#39;utente fornisce a ClientApp il nome utente e la password, ClientApp potrebbe accedere a tutti i dati a cui l&#39;utente può accedere. Questo è un rischio per la sicurezza, perché ClientApp richiede solo un set di informazioni piccolo e specifico.

Quando crei un’app OAuth2 per ClientApp, in sostanza racconti [!DNL Workfront] che ClientApp è autorizzato ad accedere a [!DNL Workfront], ma solo se l’utente il cui account ClientApp sta accedendo concede l’autorizzazione per l’accesso.

## Creare un’applicazione OAuth2

Quando crei un’applicazione OAuth2, scegli il tipo di applicazione che meglio soddisfa le esigenze dell’integrazione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo di applicazione</th> 
   <th>Migliore per</th> 
   <th>Metodo di autenticazione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Applicazione machine-to-machine</p> </td> 
   <td> <p>Ottimale per CLI, daemon o script in esecuzione sul server</p> <p>Esempi:</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>Autenticazione tramite token web JSON con codifica per coppia di chiavi pubblica/privata.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Applicazione web a pagina singola</p> </td> 
   <td> <p>Ideale per applicazioni web per dispositivi mobili o a pagina singola</p> <p>Esempi:</p> 
    <ul> 
     <li> <p>[!DNL Javascript]</p> </li> 
     <li> <p>[!DNL Angular]</p> </li> 
     <li> <p>[!DNL React]</p> </li> 
     <li> <p>[!DNL Vue]</p> </li> 
    </ul> </td> 
   <td> <p>Autenticazione tramite flusso Codice di autenticazione OAuth 2.0 con Proof Key for Code Exchange (PKCE).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Applicazione web</p> </td> 
   <td> <p>Ideale per le applicazioni lato server che gestiscono credenziali e token sul server</p> <p>Esempi:</p> 
    <ul> 
     <li> <p>[!DNL Go]</p> </li> 
     <li> <p>[!DNL Java]</p> </li> 
     <li> <p>[!DNL ASP.Net]</p> </li> 
     <li> <p>[!DNL Node.js]</p> </li> 
     <li> <p>[!DNL PHP]</p> </li> 
    </ul> </td> 
   <td> <p>Autenticazione tramite flusso Codice di autorizzazione OAuth 2.0.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Puoi avere fino a dieci applicazioni OAuth2 totali alla volta.

* [Creare un’applicazione OAuth2 utilizzando l’autenticazione del server (flusso JWT)](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [Creare un’applicazione OAuth2 utilizzando le credenziali utente (flusso di codice di autorizzazione)](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [Creare un’applicazione Web a pagina singola OAuth2 utilizzando PKCE](#create-an-oauth2-single-page-web-application-using-pkce)

### Creare un’applicazione OAuth2 utilizzando l’autenticazione del server (flusso JWT) {#create-an-oauth2-application-using-server-authentication-jwt-flow}

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Fai clic su **[!UICONTROL Creare un’integrazione app]**.
1. Nella finestra visualizzata, seleziona **[!UICONTROL Autenticazione server]**.
1. Immettere un nome per la nuova applicazione, ad esempio &quot;[!DNL Workfront] per ClientApp.&quot;
1. Fai clic su **[!UICONTROL Crea]**.
1. Compila i campi per la nuova app.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ID client [!UICONTROL]</td> 
      <td> <p>Questo campo viene generato automaticamente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client secret]</td> 
      <td> <p>Questo campo viene generato automaticamente</p> <p><b>IMPORTANTE</b>:  <p>Copiare il contenuto di questo campo in un altro file protetto prima di chiudere la pagina. Non potrai più vedere questa chiave segreta.</p> <p>Se perdi questa chiave, eliminala e crea un nuovo segreto client.</p> 
        <ol> 
         <li value="1"> <p>Fai clic sul pulsante <b>[!UICONTROL Elimina]</b> icona <img src="assets/delete.png"> per eliminare il segreto client corrente.</p> </li> 
         <li value="2"> <p>Fai clic su <b>[!UICONTROL Aggiungi segreto client]</b> per generare un nuovo segreto client.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Public Keys]</td> 
      <td> <p>Le app server-to-server utilizzano chiavi pubbliche e private per l'autenticazione. Esegui una delle operazioni seguenti:</p> 
       <ul> 
        <li> <p>Fai clic su <b>[!UICONTROL Aggiungi una chiave pubblica]</b> e immettere la chiave pubblica dall'altra applicazione.</p> </li> 
        <li> <p>Fai clic su <b>[!UICONTROL Generare una coppia di chiavi pubblica/privata]</b>, quindi condividi la chiave pubblica con l’altra applicazione.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Questo è lo stesso nome che hai dato all'app. Questo campo non può essere vuoto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td>Immetti una descrizione dell’integrazione.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Salva]**.

Per istruzioni su come configurare e utilizzare l’applicazione OAuth2 con le credenziali utente (flusso di codice di autorizzazione), consulta [Configura e utilizza le applicazioni personalizzate OAuth 2 della tua organizzazione utilizzando il flusso JWT](../../wf-api/api/oauth-app-jwt-flow.md).

### Creare un’applicazione OAuth2 utilizzando le credenziali utente (flusso di codice di autorizzazione) {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).
1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Fai clic su **[!UICONTROL Creare un’integrazione app]**.
1. Nella finestra visualizzata, seleziona **[!UICONTROL Autenticazione utente]**.
1. Immetti un nome per la nuova applicazione OAuth2, ad esempio &quot;[!DNL Workfront] per ClientApp.&quot;
1. Fai clic su **[!UICONTROL Crea]**.
1. Compila i campi per la nuova app.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ID client [!UICONTROL]</td> 
      <td> <p>Questo campo viene generato automaticamente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client secret]</td> 
      <td> <p>Questo campo viene generato automaticamente</p> <p><b>IMPORTANTE</b>:  <p>Copiare il contenuto di questo campo in un altro file protetto prima di chiudere la pagina. Non potrai più vedere questa chiave segreta.</p> <p>Se perdi questa chiave, eliminala e crea un nuovo segreto client.</p> 
        <ol> 
         <li value="1"> <p>Fai clic sul pulsante <b>[!UICONTROL Elimina]</b> icona <img src="assets/delete.png"> per eliminare il segreto client corrente.</p> </li> 
         <li value="2"> <p>Fai clic su <b>[!UICONTROL Aggiungi segreto client]</b> per generare un nuovo segreto client.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL di reindirizzamento]</td> 
      <td>Gli utenti verranno reindirizzati a questo percorso dopo l'autenticazione con [!DNL Workfront].</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Aggiorna rotazione token]</td> 
      <td>Abilita questa opzione affinché, ogni volta che viene utilizzato il token di aggiornamento, ne venga emesso uno nuovo. L’applicazione deve archiviare il nuovo token di aggiornamento dopo ogni aggiornamento.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Scadenza assoluta del token di aggiornamento]</td> 
      <td> <p>Selezionare il tempo di esistenza di un token di aggiornamento prima della scadenza. Quando scade, gli utenti devono accedere di nuovo all’integrazione. Selezionare "[!UICONTROL No expiration]" se non si desidera che il token di aggiornamento scada.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Scadenza token di aggiornamento inattività</td> 
      <td> <p>Selezionare il tempo dopo il quale, se l’utente non è stato attivo nel sistema, il token di aggiornamento scade. </p> <p>Ad esempio, se la scadenza del token di aggiornamento dell’inattività è di 6 mesi e l’utente non effettua l’accesso per sei mesi, il token di aggiornamento scade anche se la scadenza assoluta del token di aggiornamento può essere impostata per un periodo più lungo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Logo [!UICONTROL]</td> 
      <td>Puoi aggiungere un logo per rendere l’app più identificabile. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Questo è lo stesso nome che hai dato all'app. Questo campo non può essere vuoto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td>Immetti una descrizione dell’integrazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL App Description URL]</td> 
      <td>Può trattarsi di un collegamento a una pagina "Chi siamo" o a una pagina con ulteriori informazioni sull’integrazione.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Salva]**.

Per istruzioni su come configurare e utilizzare l’applicazione OAuth2 con le credenziali utente (flusso di codice di autorizzazione), consulta [Configura e utilizza le applicazioni personalizzate OAuth 2 della tua organizzazione utilizzando il flusso di codice di autorizzazione](../../wf-api/api/oauth-app-code-token-flow.md).

### Creare un’applicazione Web a pagina singola OAuth2 utilizzando PKCE {#create-an-oauth2-single-page-web-application-using-pkce}

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).
1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth]**.
1. Fai clic su **[!UICONTROL Creare un’integrazione app]**.
1. Nella finestra visualizzata, seleziona **[!UICONTROL Applicazione web a pagina singola]**.
1. Immettere un nome per il nuovo [!UICONTROL OAuth2] applicazione, ad esempio &quot;[!DNL Workfront] per ClientApp.&quot;
1. Fai clic su **[!UICONTROL Crea]**.
1. Compila i campi per la nuova app.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ID client [!UICONTROL]</td> 
      <td> <p>Questo campo viene generato automaticamente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL di reindirizzamento]</td> 
      <td>Gli utenti verranno reindirizzati a questo percorso dopo l'autenticazione con Workfront.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Aggiorna rotazione token]</td> 
      <td>Abilita questa opzione affinché, ogni volta che viene utilizzato il token di aggiornamento, ne venga emesso uno nuovo. L’applicazione deve archiviare il nuovo token di aggiornamento dopo ogni aggiornamento.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Scadenza assoluta del token di aggiornamento]</td> 
      <td> <p>Selezionare il tempo di esistenza di un token di aggiornamento prima della scadenza. Quando scade, gli utenti devono accedere di nuovo all’integrazione. Selezionare "[!UICONTROL No expiration]" se non si desidera che il token di aggiornamento scada.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Scadenza token di aggiornamento inattività]</td> 
      <td> <p>Selezionare il tempo dopo il quale, se l’utente non è stato attivo nel sistema, il token di aggiornamento scade. </p> <p>Ad esempio, se la scadenza del token di aggiornamento dell’inattività è di 6 mesi e l’utente non effettua l’accesso per sei mesi, il token di aggiornamento scade anche se la scadenza assoluta del token di aggiornamento può essere impostata per un periodo più lungo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Logo [!UICONTROL]</td> 
      <td>Puoi aggiungere un logo per rendere l’app più identificabile. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Questo è lo stesso nome che hai dato all'app. Questo campo non può essere vuoto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td>Immetti una descrizione dell’integrazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL App Description URL]</td> 
      <td>Può trattarsi di un collegamento a una pagina "Chi siamo" o a una pagina con ulteriori informazioni sull’integrazione.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Salva]**.

## Configurare e utilizzare l’applicazione OAuth2 creata

L’ulteriore configurazione e utilizzo dell’applicazione OAuth2 creata richiede alcune conoscenze tecniche, comprese le chiamate API.

* Per istruzioni su come configurare e utilizzare l’applicazione OAuth2 con le credenziali utente (flusso di codice di autorizzazione), consulta [Configura e utilizza le applicazioni personalizzate OAuth 2 della tua organizzazione utilizzando il flusso di codice di autorizzazione](../../wf-api/api/oauth-app-code-token-flow.md).
* Per istruzioni su come configurare e utilizzare l’applicazione OAuth2 utilizzando l’autenticazione server (flusso JWT), consulta [Configura e utilizza le applicazioni personalizzate OAuth 2 della tua organizzazione utilizzando il flusso JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Per istruzioni su come configurare e utilizzare l’applicazione OAuth2 utilizzando PKCE, consulta [Configura e utilizza le applicazioni personalizzate OAuth 2 della tua organizzazione utilizzando il flusso PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Processi OAuth2 per il flusso di codice di autorizzazione

>[!NOTE]
>
>Gli utenti accedono al [!UICONTROL OAuth2] tramite l’API. Questa sezione descrive le funzionalità in termini generali ed è fornita solo a scopo informativo.
>
>Per istruzioni specifiche sull’utilizzo dell’applicazione OAuth2, comprese chiamate API specifiche, vedi [Configura e utilizza le applicazioni personalizzate OAuth 2 della tua organizzazione utilizzando il flusso di codice di autorizzazione](../../wf-api/api/oauth-app-code-token-flow.md).

### Autorizzazione con un codice di autorizzazione e un token di accesso {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp richiede alcune informazioni da [!DNL Workfront]quindi invia una richiesta al [!DNL Workfront] API `/authorize` punto finale. La richiesta include [!UICONTROL response_type] `code`, che indica che la richiesta deve restituire un codice di autorizzazione.
1. Questo attivatore [!DNL Workfront] per inviare un prompt di autenticazione all’utente. L’utente può immettere le proprie credenziali nel prompt, che fornisce [!DNL Workfront] autorizzazione per comunicare con ClientApp. Se l&#39;utente ha già effettuato l&#39;accesso [!DNL Workfront], questo passaggio può essere ignorato.
1. La [!DNL Workfront] API invia un codice di autorizzazione a ClientApp.
1. ClientApp invia le seguenti informazioni in una richiesta al [!DNL Workfront] API `/token`   punto finale:

   * Il codice di autorizzazione inviato a ClientApp nel passaggio 3. Questo identifica l&#39;istanza specifica di autorizzazione utente.
   * Segreto client generato al momento della configurazione dell’app ClientApp OAuth2 in [!DNL Workfront]. Ciò consente [!DNL Workfront] per sapere che la richiesta proviene da ClientApp.

1. Se il codice di autorizzazione e il segreto del cliente sono corretti, [!DNL Workfront] invia un token di accesso a ClientApp. Questo token di accesso viene inviato direttamente da [!DNL Workfront] a ClientApp e non può essere visualizzato, copiato o utilizzato da nessun altro utente o applicazione client.
1. ClientApp invia il token di accesso a [!DNL Workfront] insieme alla richiesta specifica di informazioni.
1. Poiché il token di accesso è corretto, [!DNL Workfront] invia le informazioni a ClientApp.

#### Aggiornamento dei token di accesso

Per la sicurezza, i token di accesso scadono dopo un breve periodo di tempo. Per ottenere nuovi token di accesso senza dover immettere sempre le credenziali, [!DNL OAuth2] utilizza i token di aggiornamento. I token di aggiornamento sono memorizzati dal client.

Il processo per l’acquisizione di un token di aggiornamento è lo stesso della procedura descritta nella sezione [Autorizzazione con un codice di autorizzazione e un token di accesso](#authorizing-with-an-authorization-code-and-access-token). La richiesta di codice di autorizzazione include l&#39;ambito `offline_access`, che indica che la richiesta deve restituire un token di richiesta insieme al codice di autorizzazione.
