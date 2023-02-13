---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: http-modules
title: HTTP &gt; Creare un modulo di richiesta OAuth 2.0
description: Al fine di [!DNL Adobe Workfront Fusion] Per richiedere HTTP(S) ai server che richiedono un’autorizzazione OAuth 2.0, devi prima creare una connessione OAuth. [!DNL Adobe Workfront Fusion] assicura che tutte le chiamate effettuate con questa connessione abbiano le intestazioni di autorizzazione appropriate e aggiornino automaticamente i token associati quando necessario.
author: Becky
feature: Workfront Fusion
exl-id: 6c68c9b9-9f74-44a7-94ed-3785081b8331
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2172'
ht-degree: 0%

---

# [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] richiede un [!DNL Adobe Workfront Fusion] oltre a una licenza [!DNL Adobe Workfront] licenza.

Al fine di [!DNL Adobe Workfront Fusion] Per richiedere HTTP(S) ai server che richiedono un’autorizzazione OAuth 2.0, devi prima creare una connessione OAuth. [!DNL Adobe Workfront Fusion] assicura che tutte le chiamate effettuate con questa connessione abbiano le intestazioni di autorizzazione appropriate e aggiornino automaticamente i token associati quando necessario.

[!DNL Workfront Fusion] supporta i seguenti flussi di autenticazione OAuth 2.0:

* Flusso del codice di autorizzazione
* Flusso implicito

Altri flussi, come Flusso credenziali password proprietario risorsa e Flusso credenziali client, non sono supportati automaticamente tramite questo modulo.

Per ulteriori informazioni sull’autenticazione di OAuth 2.0, vedi [Framework di autorizzazione OAuth 2.0](https://tools.ietf.org/html/rfc6749).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr>
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Creazione di una connessione per un [!DNL OAuth] richiesta

* [Istruzioni generali per la creazione di una connessione nel modulo di richiesta HTTP > Make a OAuth 2.0](#general-instructions-for-creating-a-connection-in-the-http--make-an-oauth-20-request-module)
* [Istruzioni per la creazione di una connessione a Google in HTTP >[!UICONTROL Crea] un modulo di richiesta OAuth 2.0](#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)
* [Istruzioni per la connessione all’API di Microsoft Graph tramite HTTP > Crea un modulo di richiesta OAuth 2.0](#instructions-for-connecting-to-microsoft-graph-api-via-the-http--make-an-oauth-20-request-module)

### Istruzioni generali per la creazione di una connessione [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo

1. Crea un client OAuth nel [!DNL target] servizio con cui desideri [!DNL Adobe Workfront Fusion] per comunicare. Questa opzione si trova più probabilmente in [!UICONTROL Sviluppatore] sezione del servizio fornito.

   1. Quando crei un client, immetti l’URL appropriato nel `[!UICONTROL Redirect URL]` o `[!UICONTROL Callback URL]` campo:

      | Americhe / APAC | https://app.workfrontfusion.com/oauth/cb/oauth2 |
      |---|---|
      | EMEA | https://app-eu.workfrontfusion.com/oauth/cb/oauth2 |

   1. Dopo aver creato il client, il servizio fornito visualizza 2 chiavi: `[!UICONTROL Client ID]` e `[!UICONTROL Client Secret]`. Alcuni servizi li chiamano `[!UICONTROL App Key]` e `[!UICONTROL App Secret]` . Salvare la chiave e il segreto in una posizione sicura, in modo da poterli fornire durante la creazione della connessione in Workfront Fusion.

1. Trova il `[!UICONTROL Authorize URI]` e `[!UICONTROL Token URI]` nella documentazione API del servizio specificato. Si tratta di indirizzi URL attraverso i quali [!DNL Workfront Fusion] comunica con [!DNL target] servizio. Gli indirizzi servono per l’autorizzazione OAuth.

   >[!NOTE]
   >
   >Se il servizio utilizza il flusso implicito, sarà necessario solo il `[!UICONTROL Authorize URI]`.

   >[!INFO]
   >
   >**Esempio:** Indirizzo Yahoo:
   >
   >* URI autorizzazione:
   >
   >`https://api.login.yahoo.com/oauth2/request_auth`
   >
   >* URI token:
   >
   >`https://api.login.yahoo.com/oauth2/get_token`

1. (Condizionale) Se il servizio di destinazione utilizza ambiti (diritti di accesso), controlla in che modo il servizio separa i singoli ambiti e assicurati di impostare di conseguenza il separatore nelle impostazioni avanzate. Se il separatore non è impostato correttamente, [!DNL Workfront Fusion] la connessione non viene creata e viene visualizzato un errore di ambito non valido.
1. Dopo aver completato i passaggi precedenti, puoi iniziare a creare la connessione OAuth in [!DNL Workfront Fusion]. Aggiungi il modulo di elaborazione della richiesta e della risposta HTTP(S) OAuth 2.0 allo scenario.
1. Nel campo Connessione del modulo, fai clic su **[!UICONTROL Aggiungi]**.

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
      <td role="rowheader"> <p>[!UICONTROL Flow type]</p> </td> 
      <td> <p>Seleziona il flusso per ottenere i token.</p> 
       <ul> 
        <li><strong>[!UICONTROL Codice di autorizzazione]</strong>: Inserisci il <code>[!UICONTROL Authorize URI]</code> e <code>[!UICONTROL Token URI]</code> dalla documentazione API del servizio.</li> 
        <li><strong>[!UICONTROL Implicit]</strong>: Inserisci il <code>[!UICONTROL Authorize URI]</code> dalla documentazione API del servizio.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ambito [!UICONTROL] </td> 
      <td> <p>Aggiungi singoli ambiti. Puoi trovare queste informazioni nella documentazione per sviluppatori del servizio (API).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Separatore di ambito] </td> 
      <td> <p>Selezionare gli ambiti specificati sopra da separare. Puoi trovare queste informazioni nella documentazione per sviluppatori del servizio (API).</p> <p>Avviso: Se il separatore non è impostato correttamente, [!DNL Workfront Fusion] non riesce a creare la connessione e viene visualizzato un errore di ambito non valido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ID client [!UICONTROL] </td> 
      <td> <p>Immettere l'ID client. Hai ottenuto l’ID client quando hai creato un client OAuth nel servizio a cui desideri connetterti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segreto client]</td> 
      <td> <p> Inserisci il segreto client. Hai ottenuto il Segreto client quando hai creato un client OAuth nel servizio che desideri connettere.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Autorizza parametri]</p> </td> 
      <td> <p>Aggiungi eventuali parametri da includere nella chiamata di autorizzazione. I seguenti parametri standard vengono sempre inclusi automaticamente e non è necessario aggiungerli.</p> <p>Parametri standard:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL response_type]</strong> </p> <p> <code>code </code>per [!UICONTROL Authorization Code flow] e <code>token </code>per [!UICONTROL Implicit flow]</p> </li> 
        <li> <p><strong>[!UICONTROL redirect_uri]</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">Americhe / APAC</td> 
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
      <td role="rowheader"> <p>[!UICONTROL Access token parameters]</p> </td> 
      <td> <p>Aggiungi eventuali parametri da includere nella chiamata del token. I seguenti parametri standard vengono sempre inclusi automaticamente e non è necessario aggiungerli.</p> <p>Parametri standard:</p> 
       <ul> 
        <li><strong>[!UICONTROL Grant_type]</strong>: <code>authorization_code</code></li> 
        <li> <p><strong>[!UICONTROL redirect_uri]:</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">Americhe / APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li><strong>[!UICONTROL client_id]</strong>: L’ID client ricevuto durante la creazione dell’account viene incluso automaticamente nel corpo della richiesta</li> 
        <li><strong>client_secret</strong>: Il segreto client ricevuto durante la creazione dell’account viene incluso automaticamente nel corpo della richiesta</li> 
        <li><strong>codice</strong>: Codice restituito dalla richiesta di autorizzazione</li> 
       </ul> <p>Nota:  <p>Lo standard OAuth 2.0 supporta almeno 2 metodi di autenticazione client durante questo passaggio (<code>[!UICONTROL client_secret_basic]</code> e <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] invia automaticamente l'ID client specificato e il segreto tramite il <code>[!UICONTROL client_secret_post]</code> metodo . Pertanto, questi parametri vengono inclusi automaticamente come parte del corpo della richiesta del token. </p> <p>Per ulteriori informazioni sull’autenticazione di OAuth 2.0, vedi <a href="https://tools.ietf.org/html/rfc6749">Framework di autorizzazione OAuth 2.0</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Aggiorna parametri token]</p> </td> 
      <td> <p>Aggiungi eventuali parametri da includere nella chiamata del token. I seguenti parametri standard vengono sempre inclusi automaticamente e non è necessario aggiungerli.</p> <p>Parametri standard:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Grant_type]</strong>: <code>refresh_token</code></p> </li> 
        <li> <p><strong>[!UICONTROL refresh_token]</strong>: Il token di aggiornamento più recente ottenuto dal servizio a cui ti stai connettendo</p> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong>: L’ID client ricevuto durante la creazione dell’account viene incluso automaticamente nel corpo della richiesta</p> </li> 
        <li> <p><strong>[!UICONTROL client_secret]</strong>: Il segreto client ricevuto durante la creazione dell’account viene incluso automaticamente nel corpo della richiesta</p> </li> 
       </ul> <p>Nota:  <p>Lo standard OAuth 2.0 supporta almeno 2 metodi di autenticazione client durante questo passaggio (<code>[!UICONTROL client_secret_basic]</code> e <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] invia automaticamente l'ID client specificato e il segreto tramite il <code>[!UICONTROL client_secret_post]</code> metodo . Pertanto, questi parametri vengono inclusi automaticamente come parte del corpo della richiesta del token. </p> <p>Per ulteriori informazioni sull’autenticazione di OAuth 2.0, vedi <a href="https://tools.ietf.org/html/rfc6749">Framework di autorizzazione OAuth 2.0</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Intestazioni personalizzate]</p> </td> 
      <td> <p>Specifica eventuali chiavi e valori aggiuntivi da includere nell'intestazione dei passaggi [!UICONTROL Token] e R[!UICONTROL efresh Token].</p> <p>Nota:  <p>Lo standard OAuth 2.0 supporta almeno 2 metodi di autenticazione client durante questo passaggio (<code>[!UICONTROL client_secret_basic]</code> e <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] non supporta automaticamente il <code>[!UICONTROL client_secret_basic]</code> metodo . Se il servizio a cui ti connetti prevede la combinazione dell’ID client e del segreto client in un’unica stringa e quindi della codifica base64 nell’intestazione Autorizzazione, aggiungi qui l’intestazione e il valore chiave.</p> <p> Per ulteriori informazioni sull’autenticazione di OAuth 2.0, vedi <a href="https://tools.ietf.org/html/rfc6749">Framework di autorizzazione OAuth 2.0</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Token placement]</p> </td> 
      <td> <p>Seleziona se inviare il token nell’intestazione [!UICONTROL], nella stringa di query [!UICONTROL] o in entrambi quando ti connetti all’URL specificato.</p> <p>I token vengono inviati più comunemente nell’intestazione della richiesta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome token intestazione] </td> 
      <td> <p>Immetti il nome del token di autorizzazione nell'intestazione. Impostazione predefinita: <code>[!UICONTROL Bearer]</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome parametro stringa query] </td> 
      <td> <p>Immetti il nome del token di autorizzazione nella stringa query. Impostazione predefinita: <code>[!UICONTROL access_token]</code>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Continua]** per salvare le impostazioni di connessione.
1. Continua a [Configurazione del modulo di richiesta OAuth 2.0](#oauth-20-request-module-setup).

### Istruzioni per la creazione di una connessione a [!DNL Google] in [!UICONTROL HTTP] >[!UICONTROL Creare un modulo di richiesta OAuth 2.0]

L’esempio seguente mostra come utilizzare il [!UICONTROL HTTP] > [!UICONTROL Creare un OAuth 2.0] modulo di richiesta a cui connettersi [!DNL Google].

1. Assicurati di aver creato un progetto, configurato le impostazioni OAuth e generato le credenziali come descritto in [Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzo di un client OAuth personalizzato](../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).
1. Apri [!UICONTROL HTTP] >[!UICONTROL Effettuare una richiesta OAuth 2.0] modulo .
1. Fai clic su **[!UICONTROL Aggiungi]** accanto alla casella di connessione.
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
      <td role="rowheader"> <p>[!UICONTROL Flow type]</p> </td> 
      <td> <p>[!UICONTROL Codice di autorizzazione]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URI autorizzazione]</td> 
      <td><code>https://accounts.google.com/o/oauth2/v2/auth</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://www.googleapis.com/oauth2/v4/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ambito [!UICONTROL] </td> 
      <td> <p>Aggiungi singoli ambiti. Per ulteriori informazioni sugli ambiti, vedi <a href="https://developers.google.com/identity/protocols/oauth2/scopes">Ambiti OAuth 2.O per [!DNL Google] API</a> in [!DNL Google] documentazione.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Separatore di ambito] </td> 
      <td> <p>[!UICONTROL SPACE]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ID client [!UICONTROL] </td> 
      <td> <p>Inserisci il tuo [!DNL Google] ID client. </p> <p>Per creare un ID client, vedi <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">Creare credenziali OAuth</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] a [!DNL Google Services] utilizzo di un client OAuth personalizzato</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segreto client]</td> 
      <td> <p>Inserisci il tuo [!DNL Google] Segreto client. </p> <p>Per creare un segreto client, vedi <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">Creare credenziali OAuth</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] a [!DNL Google] Servizi che utilizzano un client OAuth personalizzato</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Autorizza parametri]</p> </td> 
      <td> <p>Aggiungi <code>[!UICONTROL access_type]</code> - <code>[!UICONTROL offline] </code>coppia chiave-valore.</p> <p> <img src="assets/google-authentication-http.png"> </p> <p>Nota: Se riscontri problemi di autenticazione, ad esempio con l’aggiornamento dei token, prova ad aggiungere il <code>[!UICONTROL prompt] </code>- <code>[!UICONTROL consent] </code>coppia chiave-valore.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Continua]** per salvare le impostazioni di connessione.
1. Continua a [Configurazione del modulo di richiesta OAuth 2.0](#oauth-20-request-module-setup).

### Istruzioni per la connessione a [!DNL Microsoft Graph API] tramite [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo

Per istruzioni su [!DNL Microsoft Graph API], vedi [Chiama il [!DNL MS Graph REST API] tramite [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Effettuare una richiesta OAuth 2.0] modulo](../../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md).

## Configurazione del modulo di richiesta OAuth 2.0

Quando hai stabilito un [!DNL Oauth 2]Connessione .0 come descritto in [Creazione di una connessione per un [!DNL OAuth] richiesta](#creating-a-connection-for-an-oauth-request), continua a configurare il modulo come desiderato. Tutti i token di autorizzazione vengono inclusi automaticamente in questa richiesta e in qualsiasi altra richiesta che utilizza la stessa connessione.

Quando configuri le [!UICONTROL HTTP] >[!UICONTROL Effettuare una richiesta OAuth 2.0] modulo, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<!--
<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per informazioni sulla configurazione di una connessione, vedi <a href="#creating-a-connection-for-an-oauth-request" class="MCXref xref">Creazione di una connessione per una richiesta OAuth</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valuta tutti gli stati come errori (ad eccezione di 2xx e 3xx]) </td> 
   <td> <p>Utilizza questa opzione per configurare la gestione degli errori.</p> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Gestione degli errori in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Inserisci l’URL a cui desideri inviare una richiesta, ad esempio un endpoint API, un sito web e così via.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL, Metodo]</p> </td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard. Ad esempio: <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Immetti le coppie chiave-valore della query desiderate.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Body type]</p> </td> 
   <td> <p>Il corpo HTTP è il numero di byte di dati trasmessi in un messaggio di transazione HTTP immediatamente successivo alle intestazioni, se ce ne sono.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>Il tipo di corpo non elaborato è generalmente adatto per la maggior parte delle richieste di corpo HTTP, anche in situazioni in cui la documentazione per gli sviluppatori non specifica i dati da inviare.</p> <p>Specifica un modulo per l’analisi dei dati nel campo [!UICONTROL Content type] (Tipo di contenuto).</p> <p>Nonostante il tipo di contenuto selezionato, i dati vengono immessi in qualsiasi formato stabilito o richiesto dalla documentazione per gli sviluppatori.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>Questo tipo di corpo è costituito dai dati di POST che utilizzano <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>Per <code>[!UICONTROL application/x-www-form-urlencoded]</code>, il corpo del messaggio HTTP inviato al server è essenzialmente una stringa di interrogazione. Le chiavi e i valori sono codificati in coppie chiave-valore separate da <code>&amp;</code> e con un <code>=</code> tra la chiave e il valore. </p> <p>Per i dati binari, <code>use [!UICONTROL multipart/form-data]</code> invece.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Esempio: </b></span></span> 
       <p>Esempio del formato di richiesta HTTP risultante:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>I [!UICONTROL Multipart/form-data] sono una richiesta HTTP multipart utilizzata per inviare file e dati. Viene comunemente utilizzato per caricare i file sul server.</p> <p>Aggiungi i campi da inviare nella richiesta. Ogni campo deve contenere una coppia chiave-valore.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Testo]</strong> </p> <p>Immetti la chiave e il valore da inviare all’interno del corpo della richiesta.</p> </li> 
       <li> <p><strong>[!UICONTROL File]</strong> </p> <p>Immetti la chiave e specifica il file di origine che desideri inviare nel corpo della richiesta.</p> <p>Mappa il file da caricare dal modulo precedente (ad esempio [!UICONTROL HTTP] &gt;[!UICONTROL Get a File] o [!UICONTROL Google Drive] &gt;[!UICONTROL Scarica un file)], oppure immetti manualmente il nome del file e i dati del file.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Parse response]</p> </td> 
   <td> <p>Abilita questa opzione per analizzare automaticamente le risposte e convertire le risposte JSON e XML in modo da non dover utilizzare i moduli [!UICONTROL JSON] &gt; [!UICONTROL Parse JSON] o [!UICONTROL XML] &gt; [!UICONTROL Parse XML].</p> <p>Prima di poter utilizzare contenuti JSON o XML analizzati, esegui il modulo una volta manualmente in modo che il modulo possa riconoscere il contenuto della risposta e consentirti di mapparlo nei moduli successivi.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timeout] </td> 
   <td> <p>Immetti il timeout della richiesta in secondi (1-300). Il valore predefinito è 40 secondi.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Condividi cookie con altri moduli HTTP]</td> 
   <td> <p> Abilita questa opzione per condividere i cookie dal server con tutti i moduli HTTP nel tuo scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Certificato autofirmato]</td> 
   <td> <p> Carica il certificato se desideri utilizzare TLS utilizzando il certificato autofirmato.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rifiuta le connessioni che utilizzano certificati non verificati (autofirmati)] </td> 
   <td> <p>Abilita questa opzione per rifiutare le connessioni che utilizzano certificati TLS non verificati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Segui reindirizzamento]</td> 
   <td> <p> Abilita questa opzione per seguire i reindirizzamenti URL con risposte 3xx.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Segui tutti i reindirizzamenti] </td> 
   <td> <p>Abilita questa opzione per seguire i reindirizzamenti URL con tutti i codici di risposta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Disattiva la serializzazione di più chiavi della stringa di query come array]</p> </td> 
   <td> <p>Per impostazione predefinita, [!DNL Workfront Fusion] gestisce più valori per la stessa chiave di parametro della stringa di query URL degli array. Ad esempio: <code>www.test.com?foo=bar&amp;foo=baz</code> viene convertito in <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. Attiva questa opzione per disabilitare questa funzione. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Richiedi contenuto compresso]</td> 
   <td> <p> Abilita questa opzione per richiedere una versione compressa del sito web.</p> <p>Questo aggiunge un <code>[!UICONTROL Accept-Encoding]</code> intestazione per richiedere contenuto compresso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Utilizzare Mutual TLS]</td> 
   <td> <p>Abilita questa opzione per utilizzare Mutual TLS nella richiesta HTTP.</p> <p>Per ulteriori informazioni su Mutual TLS, vedi <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Utilizzare Mutual TLS nei moduli HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
