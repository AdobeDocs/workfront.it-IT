---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Connetti [!DNL Adobe Workfront Fusion] a un servizio web che utilizza l’autorizzazione del token API
description: Alcuni servizi non consentono soluzioni di integrazione come [!DNL Adobe Workfront Fusion] per creare un’app che puoi facilmente utilizzare nel tuo scenario.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Connetti [!DNL Adobe Workfront Fusion] a un servizio web che utilizza l’autorizzazione del token API

Alcuni servizi non consentono soluzioni di integrazione come [!DNL Adobe Workfront Fusion] per creare un’app che puoi facilmente utilizzare nel tuo scenario.

Esiste una soluzione a questa situazione. Puoi collegare il servizio desiderato (app) a [!DNL Workfront Fusion] utilizzo [!DNL Workfront Fusion]di [!UICONTROL HTTP] modulo.

Questo articolo spiega come connettere quasi tutti i servizi web a [!DNL Workfront Fusion] utilizzando una chiave API/token API.

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

## Connettersi a un servizio Web che utilizza un token API

La procedura di connessione del servizio tramite un token API è simile per la maggior parte dei servizi web.

1. Creare un’applicazione sul sito web del servizio web, come descritto nella sezione [Creare una nuova applicazione e ottenere il token API](#create-a-new-application-and-obtain-the-api-token) in questo articolo.
1. Ottieni la chiave API o il token API.
1. Aggiungi [!DNL Workfront Fusion]di [!UICONTROL HTTP] > [!UICONTROL Fai una richiesta] al tuo scenario.
1. Configura il modulo in base alla documentazione API del servizio web ed esegui lo scenario, come spiegato nella sezione [Configurare [!UICONTROL HTTP] modulo](#set-up-the-http-module) in questo articolo.

>[!NOTE]
>
>Utilizzeremo [!DNL Pushover] servizio di notifica come esempio in questo articolo.

## Creare una nuova applicazione e ottenere il token API

>[!NOTE]
>
>Esistono molti modi diversi in cui i servizi web creano e distribuiscono chiavi API o token API. Per istruzioni su come ottenere una chiave API e un token per il servizio web desiderato, visita il sito web del servizio e cerca &quot;Chiave API&quot; o &quot;Token API&quot;.
>
>Stiamo includendo istruzioni per ottenere una chiave API push solo come esempio di ciò che potresti trovare.

1. Accedi al tuo [!DNL Pushover] account.
1. Clic **[!UICONTROL Creare un token di applicazione/API]** nella parte inferiore della pagina.
1. Compila le informazioni sulla richiesta e fai clic su **[!UICONTROL Creare un’applicazione]**.
1. Memorizza il token API fornito in un luogo sicuro. Ne avrai bisogno per [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Fai una richiesta] per connettersi al servizio web desiderato ([!DNL Pushover], in questo caso).

## Configurare [!UICONTROL HTTP] modulo

Per collegare un servizio Web al [!DNL Workfront Fusion] scenario, è necessario utilizzare il [!UICONTROL HTTP] >[!UICONTROL Fai una richiesta] nello scenario e configura il modulo in base alla documentazione API del servizio web.

1. Aggiungi il [!UICONTROL HTTP] >[!UICONTROL Fai una richiesta] al tuo scenario.
1. Per inviare un messaggio push tramite [!DNL Workfront Fusion], imposta il modulo HTTP come segue.

   >[!NOTE]
   >
   >Queste impostazioni del modulo corrispondono a [!DNL Pushover] documentazione API del servizio web. Le impostazioni possono essere diverse per altri servizi web. Ad esempio, il token API può essere inserito nel [!UICONTROL Intestazione] e non al [!UICONTROL Corpo] campo.

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
      <td> <p>Alcuni servizi web possono utilizzare una stringa di query per specificare altri parametri. Questo non è il caso nel nostro esempio in quanto [!DNL Pushover] Il servizio Web utilizza [!UICONTROL Body] (vedi sotto) per tutti i tipi di richiesta.</p> </td> 
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
      <td> <p>Immetti il contenuto della richiesta [!UICONTROL Body] in formato JSON. Puoi utilizzare il modulo [!UICONTROL JSON] &gt; [!UICONTROL Crea JSON] come spiegato in <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">Corpo JSON mappato utilizzando il modulo [!UICONTROL JSON] &gt; [!UICONTROL Crea JSON]</a> in questo articolo. Oppure puoi immettere il contenuto JSON manualmente, come spiegato in <a href="#json-body-entered-manually" class="MCXref xref">Corpo JSON immesso manualmente</a> in questo articolo.</p> <p>Per informazioni sui parametri richiesti per il servizio Web, consulta la documentazione API del servizio Web.</p> </td> 
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
>
>
"token":"123459evz8aepwtxydndydgyumbfx",
>
>
"message":"Hello World!",
>
>
"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL user]</p> </td> 
   <td> <p>USER_KEY. Questo si trova nel tuo [!DNL Pushover] dashboard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>Token API/Chiave API generata Hai creato il tuo [!DNL Pushover] app.</p> </td> 
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

## Corpo JSON mappato utilizzando [!UICONTROL JSON] >[!UICONTROL Crea JSON] modulo

Il [!UICONTROL Crea JSON] rende più semplice specificare JSON. Consente inoltre di definire i valori in modo dinamico.

Per ulteriori informazioni sui moduli JSON, vedi [Moduli JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Immetti o mappa i valori da cui desideri creare il JSON.

   ![](assets/json-values-350x288.png)

1. Connetti [!UICONTROL JSON] > [!UICONTROL Crea JSON] nel modulo HTTP > Make a Request.
1. Mappa la stringa JSON da [!UICONTROL Crea JSON] al modulo [!UICONTROL Richiedi contenuto] campo in [!UICONTROL HTTP] >[!UICONTROL Fai una richiesta] modulo.

   Ora, quando esegui lo scenario, la notifica push viene inviata al dispositivo che è stato registrato nel [!DNL Pushover] account.
