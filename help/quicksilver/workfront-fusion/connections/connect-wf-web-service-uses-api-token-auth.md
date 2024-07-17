---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Connetti [!DNL Adobe Workfront Fusion] a un servizio Web che utilizza l'autorizzazione token API
description: Alcuni servizi non consentono alle soluzioni di integrazione come  [!DNL Adobe Workfront Fusion]  di creare un'app che puoi facilmente utilizzare nel tuo scenario.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: e61dc6646e221cffb30aad055663dcf8fd3299e2
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# Connetti [!DNL Adobe Workfront Fusion] a un servizio Web che utilizza l&#39;autorizzazione token API

Alcuni servizi non consentono alle soluzioni di integrazione come [!DNL Adobe Workfront Fusion] di creare un&#39;app che puoi facilmente utilizzare nel tuo scenario.

Esiste una soluzione a questa situazione. È possibile connettere il servizio desiderato (app) a [!DNL Workfront Fusion] utilizzando il modulo [!UICONTROL HTTP] di [!DNL Workfront Fusion].

Questo articolo spiega come connettere quasi tutti i servizi Web a [!DNL Workfront Fusion] utilizzando una chiave API o un token API.

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
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connettersi a un servizio Web che utilizza un token API

La procedura di connessione del servizio tramite un token API è simile per la maggior parte dei servizi web.

1. Creare un&#39;applicazione nel sito Web del servizio Web, come descritto nella sezione [Creare una nuova applicazione e ottenere il token API](#create-a-new-application-and-obtain-the-api-token) in questo articolo.
1. Ottieni la chiave API o il token API.
1. Aggiungi il modulo [!UICONTROL HTTP] di [!DNL Workfront Fusion] > [!UICONTROL Invia una richiesta] allo scenario.
1. Configura il modulo in base alla documentazione API del servizio Web ed esegui lo scenario, come spiegato nella sezione [Configura il modulo [!UICONTROL HTTP]](#set-up-the-http-module) in questo articolo.

>[!NOTE]
>
>Il servizio di notifica [!DNL Pushover] verrà utilizzato come esempio in questo articolo.

## Creare una nuova applicazione e ottenere il token API

>[!NOTE]
>
>Esistono molti modi diversi in cui i servizi web creano e distribuiscono chiavi API o token API. Per istruzioni su come ottenere una chiave API e un token per il servizio web desiderato, visita il sito web del servizio e cerca &quot;Chiave API&quot; o &quot;Token API&quot;.
>
>Stiamo includendo istruzioni per ottenere una chiave API push solo come esempio di ciò che potresti trovare.

1. Accedi al tuo account [!DNL Pushover].
1. Fai clic su **[!UICONTROL Crea un token di applicazione/API]** nella parte inferiore della pagina.
1. Compila le informazioni sull&#39;applicazione e fai clic su **[!UICONTROL Crea un&#39;applicazione]**.
1. Memorizza il token API fornito in un luogo sicuro. Sarà necessario per il modulo [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Richiedi] per connettersi al servizio Web desiderato ([!DNL Pushover], in questo caso).

## Configura il modulo [!UICONTROL HTTP]

Per connettere un servizio Web allo scenario [!DNL Workfront Fusion], è necessario utilizzare il modulo [!UICONTROL HTTP] >[!UICONTROL Richiedi] nello scenario e configurare il modulo in base alla documentazione API del servizio Web.

1. Aggiungi il modulo [!UICONTROL HTTP] >[!UICONTROL Invia una richiesta] allo scenario.
1. Per inviare un messaggio push tramite [!DNL Workfront Fusion], configurare il modulo HTTP come segue.

   >[!NOTE]
   >
   >Queste impostazioni del modulo corrispondono alla documentazione API del servizio Web [!DNL Pushover]. Le impostazioni possono essere diverse per altri servizi web. Ad esempio, il token API può essere inserito nell&#39;intestazione [!UICONTROL Header] e non nel campo [!UICONTROL Body].

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>Il campo URL contiene l’endpoint che puoi trovare nella documentazione API del servizio web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>Il metodo utilizzato dipende dall’endpoint corrispondente. L’endpoint Pushover per la trasmissione dei messaggi utilizza il metodo POST.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
      <td> <p>Alcuni servizi web possono utilizzare le intestazioni per specificare l’autenticazione del token API o altri parametri. Questo non avviene nel nostro esempio, poiché l’endpoint di push dei messaggi utilizza il corpo (vedi sotto) per tutti i tipi di richiesta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Stringa Di Query]</p> </td> 
      <td> <p>Alcuni servizi web possono utilizzare una stringa di query per specificare altri parametri. Questo non avviene nel nostro esempio, in quanto il servizio Web [!DNL Pushover] utilizza [!UICONTROL Body] (vedi sotto) per tutti i tipi di richiesta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Body Type]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>Questa impostazione consente di selezionare il tipo di contenuto JSON nel campo [!UICONTROL Content Type] sottostante.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Tipo di contenuto]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON è il tipo di contenuto richiesto dall'app [!UICONTROL Pushover]. Questo può differire da altri servizi web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Contenuto richiesta]</p> </td> 
      <td> <p>Immetti il contenuto della richiesta [!UICONTROL Body] in formato JSON. È possibile utilizzare il modulo [!UICONTROL JSON] &gt; [!UICONTROL Crea JSON] come spiegato in <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">Corpo JSON mappato utilizzando il modulo [!UICONTROL JSON] &gt; [!UICONTROL Crea JSON]</a> in questo articolo. Oppure puoi immettere il contenuto JSON manualmente, come spiegato in <a href="#json-body-entered-manually" class="MCXref xref">Corpo JSON immesso manualmente</a> in questo articolo.</p> <p>Per informazioni sui parametri richiesti per il servizio Web, consulta la documentazione API del servizio Web.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Corpo JSON immesso manualmente

Specifica parametri e valori nel formato JSON.

>[!INFO]
>
>**Esempio:**
>
>```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>"token":"123459evz8aepwtxydndydgyumbfx",
>"message":"Hello World!",
>"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL user]</p> </td> 
   <td> <p>USER_KEY. È disponibile nel dashboard [!DNL Pushover].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>Il token API/chiave API generato ha creato l'app [!DNL Pushover].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL message] </td> 
   <td> <p>Il contenuto testuale della notifica push inviata ai dispositivi.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL title] </td> 
   <td> <p>(Facoltativo) Titolo del messaggio. Se non viene immesso alcun valore, viene utilizzato il nome dell’app. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Corpo JSON mappato utilizzando il modulo [!UICONTROL JSON] >[!UICONTROL Crea JSON]

Il modulo [!UICONTROL Crea JSON] semplifica la specifica del JSON. Consente inoltre di definire i valori in modo dinamico.

Per ulteriori informazioni sui moduli JSON, vedi [Moduli JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Immetti o mappa i valori da cui desideri creare il JSON.

   ![](assets/json-values-350x288.png)

1. Connetti il modulo [!UICONTROL JSON] > [!UICONTROL Crea JSON] al modulo HTTP > Crea una richiesta.
1. Mappa la stringa JSON dal modulo [!UICONTROL Crea JSON] al campo [!UICONTROL Richiedi contenuto] nel modulo [!UICONTROL HTTP] >[!UICONTROL Crea richiesta].

   Ora, quando esegui lo scenario, la notifica push viene inviata al dispositivo registrato nel tuo account [!DNL Pushover].
