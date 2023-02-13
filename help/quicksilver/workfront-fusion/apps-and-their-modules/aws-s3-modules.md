---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli AWS S3
description: La [!DNL Adobe Workfront Fusion AWS] I moduli S3 consentono di eseguire operazioni sui bucket S3.
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1381'
ht-degree: 0%

---

# Moduli AWS S3

La [!DNL Adobe Workfront Fusion AWS] I moduli S3 consentono di eseguire operazioni sui bucket S3.

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

Per utilizzare [!UICONTROL AWS S3] moduli, è necessario disporre di un [!DNL Amazon Web Service] conto.

## Connetti [!DNL AWS] a [!DNL Workfront Fusion] {#connect-aws-to-workfront-fusion}

Connessione [!DNL AWS S3] a [!DNL Workfront Fusion] è necessario collegare il [!DNL AWS] account a [!DNL Workfront Fusion]. Per farlo, devi prima creare un utente API in [!DNL AWS] [!UICONTROL IAM].

1. Accedi al tuo [!DNL AWS] [!UICONTROL IAM] conto.
1. Passa a **[!UICONTROL Gestione di identità e accesso]** > **[!UICONTROL Gestione degli accessi]** > **[!UICONTROL Utenti]**.

1. Fai clic su **[!UICONTROL Aggiungi utente]**.
1. Immetti il nome del nuovo utente e seleziona il **[!UICONTROL Accesso programmatico]** in [!UICONTROL Tipo di accesso] sezione .
1. Fai clic su **[!UICONTROL Allegare direttamente le politiche esistenti]**, quindi cerca **[!UICONTROL AmazonS3FullAccess]** nella barra di ricerca. Fai clic su di esso quando viene visualizzato, quindi fai clic su **[!UICONTROL Successivo]**.

1. Scorri le altre finestre di dialogo, quindi fai clic su **[!UICONTROL Crea utente]**.
1. Copia i dati forniti **[!UICONTROL ID chiave di accesso]** e **[!UICONTROL Chiave di accesso segreta]**.

1. Vai a [!DNL Workfront Fusion] e aprire [!DNL AWS S3] del modulo **[!UICONTROL Creare una connessione]** finestra di dialogo.
1. Inserisci il [!UICONTROL ID chiave di accesso] e [!UICONTROL Chiave di accesso segreta] dal passaggio 7 ai rispettivi campi e fai clic su **[!UICONTROL Continua]** stabilire il collegamento.

Il collegamento è stato stabilito. È possibile procedere alla configurazione del modulo.

## [!DNL AWS S3] moduli e relativi campi

Quando si configura [!DNL AWS S3] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL AWS S3] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Azioni](#actions)
* [Ricerche](#searches)

### Azioni

* [[!UICONTROL Crea bucket]](#create-bucket)
* [[!UICONTROL Ottieni file]](#get-file)
* [[!UICONTROL Carica file]](#upload-file)
* [[!UICONTROL Effettuare una chiamata API]](#make-an-api-call)

#### [!UICONTROL Crea bucket]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL AWS] account a [!DNL Workfront Fusion], vedi <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connetti [!DNL AWS] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Inserisci il nome del nuovo bucket.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Seleziona l’endpoint regionale. Per ulteriori informazioni, consulta la discussione <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">endpoint regionali</a> nella documentazione di AWS.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni file]

Scarica un file da un bucket.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL AWS] account a [!DNL Workfront Fusion], vedi <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connetti [!DNL AWS] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Seleziona l’endpoint regionale. Per ulteriori informazioni, consulta la discussione <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">endpoint regionali</a> in [!DNL AWS] documentazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Seleziona il bucket da cui vuoi scaricare il file.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Path]</p> </td> 
   <td> <p>Immettere il percorso del file. Esempio: <code>/photos/2019/February/image023.jpg</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carica file]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL AWS] account a [!DNL Workfront Fusion], vedi <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connetti [!DNL AWS] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Seleziona l’endpoint regionale. Per ulteriori informazioni, consulta la discussione <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">endpoint regionali</a> in [!DNL AWS] documentazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Folder] (facoltativo) </p> </td> 
   <td> <p>Specifica la cartella di destinazione in cui caricare un file.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File di origine]</td> 
   <td> <p>Selezionare un file di origine da un modulo precedente o mappare il nome e i dati del file di origine.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Headers] (facoltativo)</p> </td> 
   <td> <p> Inserisci intestazioni di richiesta. Le intestazioni disponibili sono disponibili nella sezione <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] documentazione - oggetto [!UICONTROL PUT]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effettuare una chiamata API]

Per una discussione dettagliata [!DNL Amazon S3] API, vedi [[!DNL Amazon S3] [!UICONTROL REST] Introduzione API](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL AWS] account a [!DNL Workfront Fusion], vedi <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connetti [!DNL AWS] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Region] </td> 
   <td> <p>Seleziona l’endpoint regionale. Per ulteriori informazioni, consulta la discussione <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">endpoint regionali</a> in [!DNL AWS] documentazione.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>URL Immettere un URL host. Il percorso deve essere relativo a<code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL, Metodo]</td> 
   <td> <p>Seleziona il metodo di richiesta [!UICONTROL HTTP] necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi un'intestazione di richiesta. Puoi utilizzare le seguenti intestazioni di richiesta comuni. Per ulteriori intestazioni di richiesta fare riferimento a <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] Documentazione API</a>.</p> <p>[!DNL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> 
    <table style="table-layout:auto">
     <col> 
     <col> 
     <thead> 
      <tr> 
       <th>Nome intestazione</th> 
       <th> <p> Descrizione</p> </th> 
      </tr> 
     </thead> 
     <tbody> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Length]</p> </td> 
       <td> <p>Lunghezza del messaggio (senza le intestazioni) in base alla RFC 2616. Questa intestazione è necessaria per [!UICONTROL PUT]s e le operazioni che caricano XML, come log e ACL.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Type]</p> </td> 
       <td> <p>Il tipo di contenuto della risorsa, nel caso in cui il contenuto della richiesta sia nel corpo. Esempio: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>Il riepilogo MD5 a 128 bit codificato base64 del messaggio (senza le intestazioni) in base alla RFC 1864. Puoi utilizzare questa intestazione come controllo dell’integrità del messaggio per verificare che i dati siano gli stessi che sono stati inviati originariamente. Anche se opzionale, si consiglia di utilizzare il meccanismo [!UICONTROL Content-MD5] come controllo dell’integrità end-to-end. Per ulteriori informazioni sull'autenticazione della richiesta REST [!UICONTROL REST], vai a <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">Autenticazione REST</a> in <i>[!DNL Amazon] Guida per gli sviluppatori di servizi di storage semplici</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Date]</p> </td> 
       <td> <p>Data e ora correnti in base al richiedente. Esempio: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Quando specifichi la <code>Authorization </code>è necessario specificare <code>x-amz-date</code> o <code>Date </code>intestazione.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL previsto]</p> </td> 
       <td> <p>Quando l'applicazione utilizza [!UICONTROL 100-continue], non invia il corpo della richiesta fino a quando non riceve una conferma. Se il messaggio viene rifiutato in base alle intestazioni, il corpo del messaggio non viene inviato. Puoi utilizzare questa intestazione solo se invii un corpo.</p> <p>Valori validi: [!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
       <td> <p>Per le richieste in stile percorso, il valore è <code>s3.amazonaws.com</code>. Per le richieste in stile virtuale, il valore è <code>BucketName.s3.amazonaws.com</code>. Per ulteriori informazioni, consulta <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">Hosting virtuale</a> in <i>[!DNL Amazon] Guida per gli sviluppatori di servizi di storage semplici</i>.</p> <p>Questa intestazione è necessaria per HTTP 1.1 (la maggior parte dei toolkit aggiunge automaticamente questa intestazione); facoltativo per le richieste HTTP/1.0.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>Quando si utilizza la versione 4 della firma per autenticare la richiesta, questa intestazione fornisce un hash del payload della richiesta. Durante il caricamento di un oggetto nei blocchi, imposta il valore su <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> per indicare che la firma copre solo le intestazioni e che non è presente alcun payload. Per ulteriori informazioni, consulta <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">Calcoli delle firme per l’intestazione Autorizzazione: Trasferimento del payload in più blocchi (caricamento con blocchi) ([!DNL AWS] Firma versione 4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-date]</p> </td> 
       <td> <p>Data e ora correnti in base al richiedente. Esempio: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Quando specifichi la <code>Authorization </code>è necessario specificare <code>x-amz-date</code> o <code>Date </code>intestazione. Se specifichi entrambi, il valore specificato per <code>x-amz-date</code> l’intestazione ha la precedenza.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>Questa intestazione può essere utilizzata nei seguenti scenari:</p> 
        <ul> 
         <li>Fornire token di sicurezza per [!DNL Amazon DevPay] operazioni. Ogni richiesta che utilizza [!DNL Amazon DevPay] richiede due <code>x-amz-security-token</code> intestazioni: uno per il token prodotto e uno per il token utente. Quando [!DNL Amazon S3] riceve una richiesta autenticata e confronta la firma calcolata con la firma fornita. Intestazioni multivalore formattate in modo errato utilizzate per calcolare una firma possono causare problemi di autenticazione.</li> 
         <li>Fornire un token di sicurezza quando si utilizzano credenziali di sicurezza temporanee. Quando esegui richieste utilizzando le credenziali di sicurezza temporanee ottenute da IAM, devi fornire un token di sicurezza utilizzando questa intestazione. Per ulteriori informazioni sulle credenziali di sicurezza temporanee, vedere Esecuzione delle richieste.</li> 
        </ul> <p>Questa intestazione è necessaria per le richieste che utilizzano [!DNL Amazon DevPay] e le richieste firmate utilizzando le credenziali di sicurezza temporanee.</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query String]</td> 
   <td> <p>Aggiungi le stringhe di query desiderate, ad esempio parametri o campi modulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:   <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Ricerche

* [[!UICONTROL File elenco]](#list-files)
* [[!UICONTROL Cartelle elenco]](#list-folders)

#### [!UICONTROL File elenco]

Restituisce un elenco di file da una posizione specificata.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL AWS] account a [!DNL Workfront Fusion], vedi <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connetti [!DNL AWS] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Seleziona l’endpoint regionale. Per ulteriori informazioni, consulta la discussione <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">endpoint regionali</a> in [!DNL AWS] documentazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Seleziona la [!DNL Amazon S3] bucket in cui si desidera cercare i file.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (facoltativo)</p> </td> 
   <td> <p> Percorso di una cartella in cui cercare i file, ad esempio <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cartelle elenco]

Restituisce un elenco di cartelle da una posizione specificata.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Per istruzioni su come collegare le [!DNL AWS] account a [!DNL Workfront Fusion], vedi <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connetti [!DNL AWS] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Seleziona l’endpoint regionale. Per ulteriori informazioni, consulta la discussione <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">endpoint regionali</a> nella documentazione di AWS.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Seleziona la [!DNL Amazon S3] bucket che si desidera cercare nelle cartelle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (facoltativo)</p> </td> 
   <td> <p> Percorso di una cartella in cui cercare le cartelle, ad esempio <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
