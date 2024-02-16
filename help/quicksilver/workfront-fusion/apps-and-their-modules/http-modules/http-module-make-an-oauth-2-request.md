---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: http-modules
title: HTTP &gt; Creare un modulo di richiesta OAuth 2.0
description: Al fine di creare un [!DNL Adobe Workfront Fusion] richiesta HTTP(S) ai server che richiedono un’autorizzazione OAuth 2.0, devi innanzitutto creare una connessione OAuth. [!DNL Adobe Workfront Fusion] garantisce che tutte le chiamate effettuate con questa connessione dispongano delle intestazioni di autorizzazione appropriate e aggiornino automaticamente i token associati quando necessario.
author: Becky
feature: Workfront Fusion
exl-id: 6c68c9b9-9f74-44a7-94ed-3785081b8331
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '2236'
ht-degree: 0%

---

# [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] richiede un [!DNL Adobe Workfront Fusion] licenza oltre a un [!DNL Adobe Workfront] licenza.

Al fine di creare un [!DNL Adobe Workfront Fusion] richiesta HTTP(S) ai server che richiedono un’autorizzazione OAuth 2.0, devi innanzitutto creare una connessione OAuth. [!DNL Adobe Workfront Fusion] garantisce che tutte le chiamate effettuate con questa connessione dispongano delle intestazioni di autorizzazione appropriate e aggiornino automaticamente i token associati quando necessario.

[!DNL Workfront Fusion] supporta i seguenti flussi di autenticazione OAuth 2.0:

* Flusso codice di autorizzazione
* Flusso implicito

Altri flussi, come il flusso delle credenziali della password del proprietario della risorsa e il flusso delle credenziali del client, non sono automaticamente supportati da questo modulo.

Per ulteriori informazioni sull’autenticazione OAuth 2.0, consulta [Framework di autorizzazione OAuth 2.0](https://tools.ietf.org/html/rfc6749).

>[!NOTE]
>
>Se ti stai connettendo a un prodotto di Adobe che al momento non dispone di un connettore dedicato, ti consigliamo di utilizzare il modulo Adobe Authenticator.
>
>Per ulteriori informazioni, consulta [Modulo Adobe Authenticator](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md).

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

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Creazione di una connessione per un [!DNL OAuth] richiesta

* [Istruzioni generali per la creazione di una connessione in HTTP > Creare un modulo di richiesta OAuth 2.0](#general-instructions-for-creating-a-connection-in-the-http--make-an-oauth-20-request-module)
* [Istruzioni per la creazione di una connessione a Google in HTTP >[!UICONTROL Marca] un modulo di richiesta OAuth 2.0](#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)
* [Istruzioni per la connessione all’API di Microsoft Graph tramite HTTP > Creare un modulo di richiesta OAuth 2.0](#instructions-for-connecting-to-microsoft-graph-api-via-the-http--make-an-oauth-20-request-module)

### Istruzioni generali per la creazione di una connessione in [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo

1. Creare un client OAuth in [!DNL target] servizio con cui desideri [!DNL Adobe Workfront Fusion] per comunicare. Questa opzione si trova probabilmente in [!UICONTROL Sviluppatore] del servizio specificato.

   1. Quando crei un client, immetti l’URL appropriato nella sezione `[!UICONTROL Redirect URL]` o `[!UICONTROL Callback URL]` campo:

      | Americhe/APAC | https://app.workfrontfusion.com/oauth/cb/oauth2 |
      |---|---|
      | EMEA | https://app-eu.workfrontfusion.com/oauth/cb/oauth2 |

   1. Dopo aver creato il client, il servizio specificato visualizza 2 chiavi: `[!UICONTROL Client ID]` e `[!UICONTROL Client Secret]`. Alcuni servizi li chiamano `[!UICONTROL App Key]` e `[!UICONTROL App Secret]` . Salvare la chiave e il segreto in un percorso sicuro, in modo da poterli fornire quando si crea la connessione in Workfront Fusion.

1. Trova il `[!UICONTROL Authorize URI]` e `[!UICONTROL Token URI]` nella documentazione API del servizio specificato. Si tratta di indirizzi URL attraverso i quali [!DNL Workfront Fusion] comunica con [!DNL target] servizio. Gli indirizzi vengono utilizzati per l’autorizzazione OAuth.

   >[!NOTE]
   >
   >Se il servizio utilizza il flusso implicito, sarà necessario solo il `[!UICONTROL Authorize URI]`.

   >[!INFO]
   >
   >**Esempio:** Indirizzi Yahoo:
   >
   >* URI autorizzazione:
   >
   >`https://api.login.yahoo.com/oauth2/request_auth`
   >
   >* URI token:
   >
   >`https://api.login.yahoo.com/oauth2/get_token`

1. (Condizionale) Se il servizio di destinazione utilizza ambiti (diritti di accesso), controlla in che modo il servizio separa i singoli ambiti e assicurati di impostare di conseguenza il separatore nelle impostazioni avanzate. Se il separatore non è impostato correttamente, [!DNL Workfront Fusion] non riesce a creare la connessione e viene visualizzato un errore di ambito non valido.
1. Dopo aver completato i passaggi precedenti, puoi iniziare a creare la connessione OAuth in [!DNL Workfront Fusion]. Aggiungi il modulo di elaborazione delle richieste e delle risposte HTTP(S) OAuth 2.0 allo scenario.
1. Nel campo Connection del modulo, fai clic su **[!UICONTROL Aggiungi]**.

1. Compila i campi seguenti per creare una connessione:

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome connessione] </td> 
      <td> <p>Immettere il nome della connessione.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Tipo di flusso]</p> </td> 
      <td> <p>Seleziona il flusso per ottenere i token.</p> 
       <ul> 
        <li><strong>[!UICONTROL Codice autorizzazione]</strong>: immetti il <code>[!UICONTROL Authorize URI]</code> e <code>[!UICONTROL Token URI]</code> dalla documentazione API del servizio.</li> 
        <li><strong>[!UICONTROL implicito]</strong>: immetti il <code>[!UICONTROL Authorize URI]</code> dalla documentazione API del servizio.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ambito] </td> 
      <td> <p>Aggiungere singoli ambiti. Puoi trovare queste informazioni nella documentazione per gli sviluppatori (API) del servizio specificato.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Separatore ambito] </td> 
      <td> <p>Seleziona gli ambiti inseriti sopra da separare con. Puoi trovare queste informazioni nella documentazione per gli sviluppatori (API) del servizio specificato.</p> <p>Avvertenza: se il separatore non è impostato correttamente, [!DNL Workfront Fusion] impossibile creare la connessione. si riceve un errore di ambito non valido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID client] </td> 
      <td> <p>Immetti l'ID client. Hai ottenuto l’ID client quando hai creato un client OAuth nel servizio che desideri connettere.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segreto client]</td> 
      <td> <p> Immetti il segreto client. Il segreto client è stato ottenuto quando hai creato un client OAuth nel servizio che desideri connettere.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Autorizza parametri]</p> </td> 
      <td> <p>Aggiungi eventuali parametri da includere nella chiamata di autorizzazione. I seguenti parametri standard sono sempre inclusi automaticamente e non è necessario aggiungerli.</p> <p>Parametri standard:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL tipo_risposta]</strong> </p> <p> <code>code </code>per [!UICONTROL Codice di autorizzazione flusso] e <code>token </code>per [!UICONTROL Flusso implicito]</p> </li> 
        <li> <p><strong>[!UICONTROL redirect_uri]</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">Americhe/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong> </p> <p> ID client ricevuto al momento della creazione dell’account</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Parametri token di accesso]</p> </td> 
      <td> <p>Aggiungi eventuali parametri da includere nella chiamata del token. I seguenti parametri standard sono sempre inclusi automaticamente e non è necessario aggiungerli.</p> <p>Parametri standard:</p> 
       <ul> 
        <li><strong>[!UICONTROL grant_type]</strong>: <code>authorization_code</code></li> 
        <li> <p><strong>[!UICONTROL redirect_uri]:</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">Americhe/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li><strong>[!UICONTROL client_id]</strong>: l’ID client ricevuto al momento della creazione dell’account viene incluso automaticamente nel corpo della richiesta</li> 
        <li><strong>client_secret</strong>: il segreto client ricevuto durante la creazione dell’account viene incluso automaticamente nel corpo della richiesta</li> 
        <li><strong>codice</strong>: codice restituito dalla richiesta di autorizzazione</li> 
       </ul> <p>Nota:  <p>Lo standard OAuth 2.0 supporta almeno 2 metodi di autenticazione client durante questo passaggio (<code>[!UICONTROL client_secret_basic]</code> e <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] invia automaticamente l'ID client e il segreto specificati tramite <code>[!UICONTROL client_secret_post]</code> metodo. Pertanto, questi parametri vengono automaticamente inclusi nel corpo della richiesta del token. </p> <p>Per ulteriori informazioni sull’autenticazione OAuth 2.0, consulta <a href="https://tools.ietf.org/html/rfc6749">Framework di autorizzazione OAuth 2.0</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Aggiorna parametri token]</p> </td> 
      <td> <p>Aggiungi eventuali parametri da includere nella chiamata del token. I seguenti parametri standard sono sempre inclusi automaticamente e non è necessario aggiungerli.</p> <p>Parametri standard:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL grant_type]</strong>: <code>refresh_token</code></p> </li> 
        <li> <p><strong>[!UICONTROL refresh_token]</strong>: token di aggiornamento più recente ottenuto dal servizio a cui ti stai connettendo</p> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong>: l’ID client ricevuto al momento della creazione dell’account viene incluso automaticamente nel corpo della richiesta</p> </li> 
        <li> <p><strong>[!UICONTROL client_secret]</strong>: il segreto client ricevuto durante la creazione dell’account viene incluso automaticamente nel corpo della richiesta</p> </li> 
       </ul> <p>Nota:  <p>Lo standard OAuth 2.0 supporta almeno 2 metodi di autenticazione client durante questo passaggio (<code>[!UICONTROL client_secret_basic]</code> e <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] invia automaticamente l'ID client e il segreto specificati tramite <code>[!UICONTROL client_secret_post]</code> metodo. Pertanto, questi parametri vengono automaticamente inclusi nel corpo della richiesta del token. </p> <p>Per ulteriori informazioni sull’autenticazione OAuth 2.0, consulta <a href="https://tools.ietf.org/html/rfc6749">Framework di autorizzazione OAuth 2.0</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Intestazioni personalizzate]</p> </td> 
      <td> <p>Specifica le chiavi e i valori aggiuntivi da includere nell'intestazione dei passaggi [!UICONTROL Token] e R[!UICONTROL efresh Token].</p> <p>Nota:  <p>Lo standard OAuth 2.0 supporta almeno 2 metodi di autenticazione client durante questo passaggio (<code>[!UICONTROL client_secret_basic]</code> e <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] non supporta automaticamente <code>[!UICONTROL client_secret_basic]</code> metodo. Se il servizio a cui ti stai connettendo prevede che l’ID client e il segreto client vengano combinati in una singola stringa e quindi codificati in base64 nell’intestazione Autorizzazione, devi aggiungere qui l’intestazione e il valore della chiave.</p> <p> Per ulteriori informazioni sull’autenticazione OAuth 2.0, consulta <a href="https://tools.ietf.org/html/rfc6749">Framework di autorizzazione OAuth 2.0</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Token placement]</p> </td> 
      <td> <p>Seleziona se inviare il token nell'intestazione [!UICONTROL], nella stringa di query [!UICONTROL] o in entrambe durante la connessione all'URL specificato.</p> <p>I token vengono generalmente inviati nell’intestazione della richiesta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome token intestazione] </td> 
      <td> <p>Immetti il nome del token di autorizzazione nell’intestazione. Predefinito: <code>[!UICONTROL Bearer]</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome parametro stringa query] </td> 
      <td> <p>Immetti il nome del token di autorizzazione nella stringa di query. Predefinito: <code>[!UICONTROL access_token]</code>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Continua]** per salvare le impostazioni di connessione.
1. Continua con [Configurazione del modulo di richiesta OAuth 2.0](#oauth-20-request-module-setup).

### Istruzioni per la creazione di una connessione a [!DNL Google] nel [!UICONTROL HTTP] >[!UICONTROL Creare un modulo di richiesta OAuth 2.0]

L&#39;esempio seguente mostra come utilizzare il [!UICONTROL HTTP] > [!UICONTROL Creare un OAuth 2.0] modulo di richiesta a cui connettersi [!DNL Google].

1. Assicurati di aver creato un progetto, configurato le impostazioni OAuth e generato le credenziali come descritto in [Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzo di un client OAuth personalizzato](../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).
1. Apri [!UICONTROL HTTP] >[!UICONTROL Effettuare una richiesta OAuth 2.0] modulo.
1. Clic **[!UICONTROL Aggiungi]** accanto alla casella di connessione.
1. Immetti i seguenti valori:

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome connessione] </td> 
      <td> <p>Immettere il nome della connessione.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Tipo di flusso]</p> </td> 
      <td> <p>[!UICONTROL Codice autorizzazione]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autorizza URI]</td> 
      <td><code>https://accounts.google.com/o/oauth2/v2/auth</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://www.googleapis.com/oauth2/v4/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ambito] </td> 
      <td> <p>Aggiungere singoli ambiti. Per ulteriori informazioni sugli ambiti, consulta <a href="https://developers.google.com/identity/protocols/oauth2/scopes">Ambiti OAuth 2.O per [!DNL Google] API</a> nel [!DNL Google] documentazione.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Separatore ambito] </td> 
      <td> <p>[!UICONTROL SPACE]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID client] </td> 
      <td> <p>Immetti il [!DNL Google] ID client. </p> <p>Per creare un ID client, consulta <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">Crea credenziali OAuth</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] a [!DNL Google Services] utilizzo di un client OAuth personalizzato</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segreto client]</td> 
      <td> <p>Immetti il [!DNL Google] Segreto client. </p> <p>Per creare un segreto client, vedi <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">Crea credenziali OAuth</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] a [!DNL Google] Servizi che utilizzano un client OAuth personalizzato</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Autorizza parametri]</p> </td> 
      <td> <p>Aggiungi <code>[!UICONTROL access_type]</code> - <code>[!UICONTROL offline] </code>coppia chiave-valore.</p> <p> <img src="assets/google-authentication-http.png"> </p> <p>Nota: in caso di problemi di autenticazione, ad esempio con l’aggiornamento del token, prova ad aggiungere <code>[!UICONTROL prompt] </code>- <code>[!UICONTROL consent] </code>coppia chiave-valore.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Continua]** per salvare le impostazioni di connessione.
1. Continua con [Configurazione del modulo di richiesta OAuth 2.0](#oauth-20-request-module-setup).

### Istruzioni per la connessione a [!DNL Microsoft Graph API] tramite [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo

Per istruzioni relative a [!DNL Microsoft Graph API], vedi [Chiama il [!DNL MS Graph REST API] tramite [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo](../../../workfront-fusion/connections/call-the-ms-graph-rest-api.md).

## Configurazione del modulo di richiesta OAuth 2.0

Quando hai stabilito un [!DNL Oauth 2]connessione .0 come descritto in [Creazione di una connessione per un [!DNL OAuth] richiesta](#creating-a-connection-for-an-oauth-request), continua a configurare il modulo come desiderato. Tutti i token di autorizzazione vengono inclusi automaticamente in questa richiesta e in qualsiasi altra richiesta che utilizza la stessa connessione.

Quando si configura [!UICONTROL HTTP] >[!UICONTROL Effettuare una richiesta OAuth 2.0] modulo, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<!--
<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per informazioni sulla configurazione di una connessione, vedere <a href="#creating-a-connection-for-an-oauth-request" class="MCXref xref">Creazione di una connessione per una richiesta OAuth</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valuta tutti gli stati come errori (tranne 2xx e 3xx]) </td> 
   <td> <p>Utilizza questa opzione per configurare la gestione degli errori.</p> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Gestione degli errori in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Immetti l’URL a cui desideri inviare una richiesta, ad esempio un endpoint API, un sito web, ecc.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard. Ad esempio: <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query]</td> 
   <td> <p> Immetti le coppie chiave-valore di query desiderate.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo di corpo]</p> </td> 
   <td> <p>Il corpo HTTP è costituito dai byte di dati trasmessi in un messaggio di transazione HTTP immediatamente dopo le intestazioni, se ve ne sono altre da utilizzare.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>Il tipo di corpo Raw è generalmente adatto per la maggior parte delle richieste HTTP body, anche in situazioni in cui la documentazione per gli sviluppatori non specifica i dati da inviare.</p> <p>Specificare un tipo di analisi dei dati nel campo [!UICONTROL Content type].</p> <p>Nonostante il tipo di contenuto selezionato, i dati vengono immessi in qualsiasi formato stabilito o richiesto dalla documentazione per gli sviluppatori.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>Questo tipo di corpo deve POST i dati utilizzando <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>Per <code>[!UICONTROL application/x-www-form-urlencoded]</code>, il corpo del messaggio HTTP inviato al server è essenzialmente una stringa di query. Le chiavi e i valori sono codificati in coppie chiave-valore separate da <code>&amp;</code> e con un <code>=</code> tra chiave e valore. </p> <p>Per i dati binari: <code>use [!UICONTROL multipart/form-data]</code> invece.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Esempio: </b></span></span> 
       <p>Esempio del formato di richiesta HTTP risultante:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>[!UICONTROL Multipart/form-data] è una richiesta multipart HTTP utilizzata per inviare file e dati. Viene comunemente utilizzato per caricare file sul server.</p> <p>Aggiungi i campi da inviare nella richiesta. Ogni campo deve contenere una coppia chiave-valore.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Text]</strong> </p> <p>Immetti la chiave e il valore da inviare nel corpo della richiesta.</p> </li> 
       <li> <p><strong>[!UICONTROL File]</strong> </p> <p>Immetti la chiave e specifica il file di origine da inviare nel corpo della richiesta.</p> <p>Mappa il file che desideri caricare dal modulo precedente (ad esempio [!UICONTROL HTTP] &gt;[!UICONTROL Ottieni un file] o [!UICONTROL Google Drive] &gt;[!UICONTROL Scarica un file)], oppure immetti manualmente il nome del file e i dati del file.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Analizza risposta]</p> </td> 
   <td> <p>Abilita questa opzione per analizzare automaticamente le risposte e convertire le risposte JSON e XML in modo da non dover utilizzare i moduli [!UICONTROL JSON] &gt; [!UICONTROL Parse JSON] o [!UICONTROL XML] &gt; [!UICONTROL Parse XML].</p> <p>Prima di poter utilizzare contenuti JSON o XML analizzati, esegui il modulo una volta manualmente in modo che possa riconoscere il contenuto della risposta e consentirti di mapparlo nei moduli successivi.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timeout] </td> 
   <td> <p>Immetti il timeout della richiesta in secondi (1-300). Il valore predefinito è 40 secondi.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Condividi i cookie con altri moduli HTTP]</td> 
   <td> <p> Abilita questa opzione per condividere i cookie dal server con tutti i moduli HTTP nel tuo scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Self-signed certificate]</td> 
   <td> <p> Carica il certificato se desideri utilizzare TLS con il certificato autofirmato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rifiuta le connessioni che utilizzano certificati non verificati (autofirmati)] </td> 
   <td> <p>Abilita questa opzione per rifiutare le connessioni che utilizzano certificati TLS non verificati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Follow redirect]</td> 
   <td> <p> Abilita questa opzione per seguire i reindirizzamenti URL con risposte 3xx.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Segui tutti i reindirizzamenti] </td> 
   <td> <p>Abilita questa opzione per seguire i reindirizzamenti URL con tutti i codici di risposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Disattiva la serializzazione di più chiavi di stringa di query come matrici]</p> </td> 
   <td> <p>Per impostazione predefinita, [!DNL Workfront Fusion] gestisce più valori per la stessa chiave di parametro della stringa di query URL come array. Ad esempio: <code>www.test.com?foo=bar&amp;foo=baz</code> verrà convertito in <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. Attiva questa opzione per disabilitare questa funzione. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Richiedi contenuto compresso]</td> 
   <td> <p> Abilita questa opzione per richiedere una versione compressa del sito web.</p> <p>Questo aggiunge un <code>[!UICONTROL Accept-Encoding]</code> per richiedere contenuti compressi.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Usa TLS reciproco]</td> 
   <td> <p>Abilita questa opzione per utilizzare Mutual TLS nella richiesta HTTP.</p> <p>Per ulteriori informazioni su Mutual TLS, vedi <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Utilizzare Mutual TLS nei moduli HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
