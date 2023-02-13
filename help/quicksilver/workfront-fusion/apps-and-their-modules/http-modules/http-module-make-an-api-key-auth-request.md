---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: http-modules
title: HTTP &gt; Effettuare una richiesta di autorizzazione della chiave API
description: Questo [!DNL Adobe Workfront Fusion] il modulo action invia una richiesta HTTPS a un URL specificato che richiede un’autorizzazione di autenticazione della chiave API ed elabora la risposta.
author: Becky
feature: Workfront Fusion
exl-id: 70bf87c7-6d51-4ef4-9dce-80ad004e613f
source-git-commit: 58db2129dd764d24b0a681735c2405be402d8b43
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 0%

---

# HTTP >[!UICONTROL Effettuare una richiesta di autorizzazione della chiave API]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] richiede un [!DNL Adobe Workfront Fusion] oltre a una licenza Adobe Workfront.

Questo [!DNL Adobe Workfront Fusion] il modulo action invia una richiesta HTTPS a un URL specificato che richiede un’autorizzazione di autenticazione della chiave API ed elabora la risposta.

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

Per informazioni su [!UICONTROL Adobe Workfront Fusion] licenze, vedi [Licenze Adobe Workfront Fusion](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!UICONTROL HTTP] >[!UICONTROL Effettuare una richiesta di autorizzazione della chiave API] configurazione del modulo

Quando configuri le [!UICONTROL HTTP] >[!UICONTROL Effettuare una richiesta di autorizzazione della chiave API] modulo, [!DNL Adobe Workfront Fusion] visualizza i campi elencati di seguito. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Credentials]</td> 
   <td> <p>Seleziona la chiave che contiene le credenziali di autenticazione della chiave API. Per aggiungere una nuova chiave, fai clic su <strong>[!UICONTROL Aggiungi]</strong> e configura le seguenti informazioni:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nome chiave]</strong></p> <p>Immetti un nome per questo set di credenziali API.</p> </li> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>Immetti la chiave API .</p> </li> 
     <li> <p><strong>[!UICONTROL Inserimento chiave API]</strong> </p> <p>Seleziona se inserire la chiave API nell’intestazione o nella query della chiamata API.</p> </li> 
     <li> <p><strong>[!UICONTROL API Key parameter name]</strong> </p> <p>Immetti il nome in base al quale la chiamata API identifica la chiave API, ad esempio "apiKey" o "X-API-Key". Puoi trovare queste informazioni nella documentazione del servizio Web a cui il modulo si sta connettendo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valuta tutti gli stati come errori (ad eccezione di 2xx e 3xx)] </td> 
   <td> <p>Utilizza questa opzione per configurare la gestione degli errori.</p> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Gestione degli errori in Adobe Workfront Fusion</a>.</p> </td> 
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
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>Il tipo di corpo non elaborato è generalmente adatto per la maggior parte delle richieste di corpo HTTP, anche in situazioni in cui la documentazione per gli sviluppatori non specifica i dati da inviare.</p> <p>Specifica un modulo per l’analisi dei dati nel campo [!UICONTROL Content type] (Tipo di contenuto).</p> <p>Nonostante il tipo di contenuto selezionato, il modulo immette i dati in qualsiasi formato stabilito o richiesto dalla documentazione per gli sviluppatori.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>Questo tipo di corpo è costituito da dati di POST che utilizzano <code>application/x-www-form-urlencoded</code>.</p> <p>Per <code>[!UICONTROL application/x-www-form-urlencoded]</code>, il corpo del messaggio HTTP inviato al server è essenzialmente una stringa di interrogazione. Le chiavi e i valori sono codificati in coppie chiave-valore separate da <code>&amp;</code> e con un <code>=</code> tra la chiave e il valore. </p> <p>Per i dati binari, utilizza <code>[!UICONTROL multipart/form-data]</code> invece.</p> 
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
   <td> <p>Specifica il timeout della richiesta in secondi (1-300). Il valore predefinito è 40 secondi.</p> </td> 
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
   <td> <p> Abilita questa opzione per richiedere una versione compressa del sito web.</p> <p>Aggiunge un <code>[!UICONTROL Accept-Encoding]</code> intestazione per richiedere contenuto compresso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Utilizzare Mutual TLS]</td> 
   <td> <p>Abilita questa opzione per utilizzare Mutual TLS nella richiesta HTTP.</p> <p>Per ulteriori informazioni su Mutual TLS, vedi <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Utilizzare Mutual TLS nei moduli HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
