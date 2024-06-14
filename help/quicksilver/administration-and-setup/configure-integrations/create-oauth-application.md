---
title: Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Come un [!DNL Adobe Workfront] amministratore, puoi creare applicazioni OAuth2 per la tua istanza di [!DNL Workfront], che consentono ad altre applicazioni di accedere a Workfront. Gli utenti possono quindi concedere a tali altre applicazioni l'autorizzazione di accesso ai propri dati Workfront. In questo modo, è possibile integrare Workfront con le applicazioni di propria scelta, incluse quelle interne.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '1956'
ht-degree: 6%

---

# Creare applicazioni OAuth2 per [!DNL Workfront] integrazioni

Come un [!DNL Adobe Workfront] amministratore, puoi creare applicazioni OAuth2 per la tua istanza di [!DNL Workfront], che consentono l&#39;accesso ad altre applicazioni [!DNL Workfront]. Gli utenti possono quindi concedere a tali altre applicazioni l&#39;autorizzazione ad accedere ai propri [!DNL Workfront] dati. In questo modo, è possibile eseguire l&#39;integrazione con le applicazioni di propria scelta, incluse quelle interne.

Quando crei un’ [!UICONTROL OAuth2] , si generano un ID client e un Segreto client. Gli utenti possono quindi utilizzare l’ID client nelle chiamate API per l’integrazione con l’applicazione creata.

>[!NOTE]
>
>Nel contesto di OAuth2, &quot;creazione di un&#39;app&quot; si riferisce al processo di creazione di questo tipo di collegamento di accesso tra un&#39;app e un server come [!DNL Workfront].

* Per istruzioni sulla configurazione e l’utilizzo dell’applicazione OAuth2 con le credenziali utente (flusso del codice di autorizzazione), consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso del codice di autorizzazione](../../wf-api/api/oauth-app-code-token-flow.md).
* Per istruzioni sulla configurazione e l’utilizzo dell’applicazione OAuth2 tramite l’autenticazione del server (flusso JWT), consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Per istruzioni sulla configurazione e l’utilizzo dell’applicazione OAuth2 tramite PKCE, consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td><p>Nuovo: [!UICONTROL Standard]</p>
   Oppure
   <p>Corrente:[!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> Devi essere un [!DNL Workfront] amministratore. </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

+++

## Panoramica di OAuth2

Immagina che un’applicazione debba richiamare alcune informazioni specifiche da [!DNL Workfront]. Un&#39;applicazione che richiede informazioni viene definita client. In questo esempio, il nome del client è ClientApp. ClientApp ha bisogno di accedere alle informazioni di un particolare utente e quindi deve accedere [!DNL Workfront] come tale utente. Se l’utente assegna a ClientApp il nome utente e la password, ClientApp potrebbe accedere a tutti i dati a cui l’utente può accedere. Si tratta di un rischio per la sicurezza, perché ClientApp richiede solo un set di informazioni piccolo e specifico.

Quando crei un’app OAuth2 per ClientApp, in pratica stai dicendo [!DNL Workfront] a cui ClientApp è consentito accedere [!DNL Workfront], ma solo se l’utente con l’account a cui accede ClientApp concede l’autorizzazione per l’accesso.

## Creare un’applicazione OAuth2

Quando crei un’applicazione OAuth2, scegli il tipo di applicazione che meglio soddisfa le esigenze della tua integrazione.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo di applicazione</th> 
   <th>Ideale per</th> 
   <th>Metodo di autenticazione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Applicazione machine-to-machine</p> </td> 
   <td> <p>Consigliato per CLI, daemon o script in esecuzione sul server</p> <p>Esempi:</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>Autenticazione tramite token web JSON con codifica per coppia di chiavi pubblica/privata.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Applicazione web a pagina singola</p> </td> 
   <td> <p>Consigliato per applicazioni per dispositivi mobili o applicazioni web a pagina singola</p> <p>Esempi:</p> 
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
   <td> <p>Consigliato per applicazioni lato server che gestiscono credenziali e token sul server</p> <p>Esempi:</p> 
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
>Puoi avere fino a un totale di dieci applicazioni OAuth2 alla volta.

* [Creare un’applicazione OAuth2 utilizzando l’autenticazione del server (flusso JWT)](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [Creare un&#39;applicazione OAuth2 utilizzando le credenziali utente (flusso del codice di autorizzazione)](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [Creare un’applicazione web OAuth2 a pagina singola utilizzando PKCE](#create-an-oauth2-single-page-web-application-using-pkce)

### Creare un’applicazione OAuth2 utilizzando l’autenticazione del server (flusso JWT) {#create-an-oauth2-application-using-server-authentication-jwt-flow}

{{step-1-to-setup}}

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth2]**.
1. Clic **[!UICONTROL Creare l’integrazione delle app]**.
Il **Nuova applicazione OAuth2** viene visualizzata la casella.
1. In **Nuova applicazione OAuth2** , seleziona **[!UICONTROL Applicazione machine-to-machine]**.
1. Immetti un nome per la nuova applicazione, ad esempio &quot;[!DNL Workfront] per ClientApp.&quot;
1. Fai clic su **[!UICONTROL Crea]**.
1. Compila i campi per la nuova app.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID client]</td> 
      <td> <p>Questo campo viene generato automaticamente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segreto client]</td> 
      <td> <p>Questo campo viene generato automaticamente</p> <p><b>IMPORTANTE</b>:  <p>Copiare il contenuto di questo campo in un altro file protetto prima di chiudere la pagina. La chiave segreta non sarà più visibile.</p> <p>Se perdi questa chiave, eliminala e crea un Segreto client.</p> 
        <ol> 
         <li value="1"> <p>Fai clic su <b>[!UICONTROL Elimina]</b> icona <img src="assets/delete.png"> per eliminare il segreto client corrente.</p> </li> 
         <li value="2"> <p>Clic <b>[!UICONTROL Aggiungi segreto client]</b> per generare un nuovo Segreto client.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Public Keys]</td> 
      <td> <p>Le app server-to-server utilizzano chiavi pubbliche e private per l'autenticazione. Esegui una delle operazioni seguenti:</p> 
       <ul> 
        <li> <p>Clic <b>[!UICONTROL Aggiungi una chiave pubblica]</b> e immettere la chiave pubblica dell'altra applicazione.</p> </li> 
        <li> <p>Clic <b>[!UICONTROL Genera una coppia di chiavi pubblica/privata]</b>, quindi condividi la chiave pubblica con l’altra applicazione.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Questo è lo stesso nome che hai assegnato all’app. Questo campo non può essere vuoto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td>Immetti una descrizione per l’integrazione.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Salva]**.

Per istruzioni sulla configurazione e l’utilizzo dell’applicazione OAuth2 con le credenziali utente (flusso del codice di autorizzazione), consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso JWT](../../wf-api/api/oauth-app-jwt-flow.md).

### Creare un&#39;applicazione OAuth2 utilizzando le credenziali utente (flusso del codice di autorizzazione) {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

{{step-1-to-setup}}

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth2]**.
1. Clic **[!UICONTROL Creare l’integrazione delle app]**.

   Il **Nuova applicazione OAuth2** visualizzazioni.
1. In **Nuova applicazione OAuth2** , seleziona **[!UICONTROL Applicazione web]**.
1. Immettete un nome per la nuova applicazione OAuth2, ad esempio &quot;[!DNL Workfront] per ClientApp.&quot;
1. Fai clic su **[!UICONTROL Crea]**.
1. Compila i campi per la nuova app.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID client]</td> 
      <td> <p>Questo campo viene generato automaticamente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segreto client]</td> 
      <td> <p>Questo campo viene generato automaticamente</p> <p><b>IMPORTANTE</b>:  <p>Copiare il contenuto di questo campo in un altro file protetto prima di chiudere la pagina. La chiave segreta non sarà più visibile.</p> <p>Se perdi questa chiave, eliminala e crea un Segreto client.</p> 
        <ol> 
         <li value="1"> <p>Fai clic su <b>[!UICONTROL Elimina]</b> icona <img src="assets/delete.png"> per eliminare il segreto client corrente.</p> </li> 
         <li value="2"> <p>Clic <b>[!UICONTROL Aggiungi segreto client]</b> per generare un nuovo Segreto client.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL di reindirizzamento]</td> 
      <td>Gli utenti verranno reindirizzati a questo percorso dopo l’autenticazione con [!DNL Workfront].</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Aggiorna rotazione token]</td> 
      <td>Abilita questa opzione affinché, ogni volta che viene utilizzato il token di aggiornamento, ne venga emesso uno nuovo. L’applicazione deve archiviare il nuovo token di aggiornamento dopo ogni aggiornamento.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Scadenza token di aggiornamento assoluto di [!UICONTROL]</td> 
      <td> <p>Seleziona il periodo di tempo per il quale desideri che esista un token di aggiornamento prima della scadenza. Quando scade, gli utenti devono accedere di nuovo all’integrazione. Seleziona "[!UICONTROL Nessuna scadenza]" se non desideri che il token di aggiornamento scada.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Scadenza token di aggiornamento inattività</td> 
      <td> <p>Seleziona il periodo di tempo dopo il quale, se l’utente non è stato attivo nel sistema, il token di aggiornamento scade. </p> <p>Ad esempio, se la scadenza del token di aggiornamento per inattività è di 6 mesi e l’utente non effettua l’accesso per 6 mesi, il token di aggiornamento scade anche se la scadenza del token di aggiornamento assoluto può essere impostata per un periodo più lungo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>Puoi aggiungere un logo per rendere questa app più identificabile. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Questo è lo stesso nome che hai assegnato all’app. Questo campo non può essere vuoto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td>Immetti una descrizione per l’integrazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL descrizione app]</td> 
      <td>Può trattarsi di un collegamento a una pagina "Chi siamo" o di una pagina con ulteriori informazioni sull’integrazione.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Salva]**.

Per istruzioni sulla configurazione e l’utilizzo dell’applicazione OAuth2 con le credenziali utente (flusso del codice di autorizzazione), consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso del codice di autorizzazione](../../wf-api/api/oauth-app-code-token-flow.md).

### Creare un’applicazione web OAuth2 a pagina singola utilizzando PKCE {#create-an-oauth2-single-page-web-application-using-pkce}

{{step-1-to-setup}}

1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Sistema]**, quindi seleziona **[!UICONTROL Applicazioni OAuth2]**.
1. Clic **[!UICONTROL Creare l’integrazione delle app]**.

   Il **Nuova applicazione OAuth2** viene visualizzata la casella.
1. In **Nuova applicazione OAuth2** , seleziona **[!UICONTROL Applicazione Web a pagina singola]**.
1. Immetti un nome per il nuovo [!UICONTROL OAuth2] , ad esempio &quot;[!DNL Workfront] per ClientApp.&quot;
1. Fai clic su **[!UICONTROL Crea]**.
1. Compila i campi per la nuova app.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID client]</td> 
      <td> <p>Questo campo viene generato automaticamente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL di reindirizzamento]</td> 
      <td>Gli utenti verranno reindirizzati a questo percorso dopo l’autenticazione con Workfront.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Ruota token di aggiornamento ogni volta che viene utilizzato]</td> 
      <td>Abilita questa opzione affinché, ogni volta che viene utilizzato il token di aggiornamento, ne venga emesso uno nuovo. L’applicazione deve archiviare il nuovo token di aggiornamento dopo ogni aggiornamento.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL scadenza assoluta]</td> 
      <td> <p>Seleziona il periodo di tempo per il quale desideri che esista un token di aggiornamento prima della scadenza. Quando scade, gli utenti devono accedere di nuovo all’integrazione. Seleziona "[!UICONTROL Nessuna scadenza]" se non desideri che il token di aggiornamento scada.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL scadenza inattività]</td> 
      <td> <p>Seleziona il periodo di tempo dopo il quale, se l’utente non è stato attivo nel sistema, il token di aggiornamento scade. </p> <p>Ad esempio, se la scadenza del token di aggiornamento per inattività è di 6 mesi e l’utente non effettua l’accesso per 6 mesi, il token di aggiornamento scade anche se la scadenza del token di aggiornamento assoluto può essere impostata per un periodo più lungo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>Puoi aggiungere un logo per rendere questa app più identificabile. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Questo è lo stesso nome che hai assegnato all’app. Questo campo non può essere vuoto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td>Immetti una descrizione per l’integrazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome sviluppatore]</td> 
      <td>Questo è il nome dello sviluppatore che sta configurando l’applicazione OAuth2.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL Indirizzo e-mail sviluppatore]</td> 
      <td>Questo è l’indirizzo e-mail dello sviluppatore che sta configurando l’applicazione OAuth2.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL URL criteri di privacy]</td> 
      <td>Questo è il collegamento in cui l’organizzazione memorizza l’informativa sulla privacy.</td> 
     </tr>


   </tbody> 
   </table>

   <!-- removed this from the table, and added "Developer name" and following rows:
   [!UICONTROL App Description URL]</td> 
      <td>This can be a link to an "About us" page or a page with more information about the integration.> -->

1. Fai clic su **[!UICONTROL Salva]**.

## Configurare e utilizzare l’applicazione OAuth2 creata

L’ulteriore configurazione e utilizzo dell’applicazione OAuth2 creata richiede alcune conoscenze tecniche, tra cui le chiamate API.

* Per istruzioni sulla configurazione e l’utilizzo dell’applicazione OAuth2 con le credenziali utente (flusso del codice di autorizzazione), consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso del codice di autorizzazione](../../wf-api/api/oauth-app-code-token-flow.md).
* Per istruzioni sulla configurazione e l’utilizzo dell’applicazione OAuth2 tramite l’autenticazione del server (flusso JWT), consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Per istruzioni sulla configurazione e l’utilizzo dell’applicazione OAuth2 tramite PKCE, consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Processi OAuth2 per il flusso del codice di autorizzazione

>[!NOTE]
>
>Gli utenti accedono a [!UICONTROL OAuth2] tramite l&#39;API. Questa sezione descrive la funzionalità in termini generali ed è fornita solo a scopo informativo.
>
>Per istruzioni specifiche sull’utilizzo dell’applicazione OAuth2, incluse chiamate API specifiche, consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso del codice di autorizzazione](../../wf-api/api/oauth-app-code-token-flow.md).

### Autorizzazione con codice di autorizzazione e token di accesso {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp richiede alcune informazioni da [!DNL Workfront], quindi invia una richiesta al [!DNL Workfront] API `/authorize` endpoint. La richiesta include [!UICONTROL response_type] `code`, che indica che la richiesta deve restituire un codice di autorizzazione.
1. Questo trigger [!DNL Workfront] per inviare una richiesta di autenticazione all&#39;utente. L’utente può immettere le proprie credenziali nel prompt, che da [!DNL Workfront] autorizzazione per comunicare con ClientApp. Se l’utente ha già effettuato l’accesso a [!DNL Workfront], questo passaggio può essere saltato.
1. Il [!DNL Workfront] L’API invia un codice di autorizzazione a ClientApp.
1. ClientApp invia le seguenti informazioni in una richiesta a [!DNL Workfront] API `/token`   endpoint:

   * Il codice di autorizzazione inviato a ClientApp nel passaggio 3. Questo identifica l’istanza specifica dell’autorizzazione utente.
   * Segreto client generato durante la configurazione dell&#39;app ClientApp OAuth2 in [!DNL Workfront]. Ciò consente [!DNL Workfront] per sapere che la richiesta proviene da ClientApp.

1. Se il codice di autorizzazione e il segreto client sono corretti, [!DNL Workfront] invia un token di accesso a ClientApp. Questo token di accesso viene inviato direttamente da [!DNL Workfront] su ClientApp e non possono essere visualizzate, copiate o utilizzate da altri utenti o applicazioni client.
1. ClientApp invia il token di accesso a [!DNL Workfront] insieme alla richiesta specifica di informazioni.
1. Poiché il token di accesso è corretto, [!DNL Workfront] invia le informazioni a ClientApp.

#### Aggiornamento dei token di accesso

Per motivi di sicurezza, i token di accesso scadono dopo un breve periodo di tempo. Per ottenere nuovi token di accesso senza dover immettere ogni volta le credenziali, [!DNL OAuth2] utilizza i token di aggiornamento. I token di aggiornamento vengono memorizzati dal client.

Il processo di acquisizione di un token di aggiornamento è lo stesso descritto nella sezione [Autorizzazione con codice di autorizzazione e token di accesso](#authorizing-with-an-authorization-code-and-access-token). La richiesta del codice di autorizzazione include l&#39;ambito `offline_access`, che indica che la richiesta deve restituire un token di richiesta insieme al codice di autorizzazione.
