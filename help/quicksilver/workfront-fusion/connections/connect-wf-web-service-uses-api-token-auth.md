---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Connetti [!DNL Adobe Workfront Fusion] a un servizio Web che utilizza l’autorizzazione token API
description: Alcuni servizi non consentono soluzioni di integrazione come [!DNL Adobe Workfront Fusion] per creare un’app facilmente utilizzabile nel tuo scenario.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---

# Connetti [!DNL Adobe Workfront Fusion] a un servizio Web che utilizza l’autorizzazione token API

Alcuni servizi non consentono soluzioni di integrazione come [!DNL Adobe Workfront Fusion] per creare un’app facilmente utilizzabile nel tuo scenario.

C&#39;è una soluzione a questa situazione. Puoi collegare il servizio desiderato (app) a [!DNL Workfront Fusion] utilizzo [!DNL Workfront Fusion]s [!UICONTROL HTTP] modulo .

Questo articolo spiega come collegare quasi tutti i servizi web a [!DNL Workfront Fusion] utilizzo di un token API Key/API.

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

## Connettersi a un servizio Web che utilizza un token API

La procedura di connessione del servizio tramite un token API è simile per la maggior parte dei servizi web.

1. Crea un&#39;applicazione sul sito web del servizio Web, come spiegato nella sezione [Creare una nuova applicazione e ottenere il token API](#create-a-new-application-and-obtain-the-api-token) in questo articolo.
1. Ottieni la chiave API o il token API.
1. Aggiungi [!DNL Workfront Fusion]s [!UICONTROL HTTP] > [!UICONTROL Richiedi] al tuo scenario.
1. Imposta il modulo in base alla documentazione API del servizio Web ed esegue lo scenario, come spiegato nella sezione . [Imposta la [!UICONTROL HTTP] modulo](#set-up-the-http-module) in questo articolo.

>[!NOTE]
>
>Useremo il [!DNL Pushover] servizio di notifica come esempio in tutto il presente articolo.

## Creare una nuova applicazione e ottenere il token API

>[!NOTE]
>
>Esistono diversi modi in cui i servizi web creano e distribuiscono chiavi API o token API. Per istruzioni su come ottenere una chiave API e un token per il servizio Web desiderato, visita il sito web del servizio e cerca &quot;chiave API&quot; o &quot;token API&quot;.
>
>Le istruzioni per ottenere una chiave API Pushover sono incluse solo come esempio di ciò che potresti trovare.

1. Accedi al tuo [!DNL Pushover] conto.
1. Fai clic su **[!UICONTROL Creare un token applicazione/API]** nella parte inferiore della pagina.
1. Compila le informazioni dell&#39;applicazione e fai clic su **[!UICONTROL Creare un’applicazione]**.
1. Memorizza il token API fornito in un luogo sicuro. Ne avrai bisogno per [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Richiedi] modulo per la connessione al servizio Web desiderato ([!DNL Pushover], in questo caso).

## Imposta la [!UICONTROL HTTP] modulo

Per collegare un servizio Web al [!DNL Workfront Fusion] in uno scenario, è necessario utilizzare [!UICONTROL HTTP] >[!UICONTROL Fai una richiesta] nello scenario e imposta il modulo in base alla documentazione API del servizio Web.

1. Aggiungi il [!UICONTROL HTTP] >[!UICONTROL Richiedi] al tuo scenario.
1. Per inviare un messaggio push con [!DNL Workfront Fusion], imposta il modulo HTTP come segue.

   >[!NOTE]
   >
   >Queste impostazioni del modulo corrispondono a [!DNL Pushover] documentazione API del servizio Web. Le impostazioni possono essere diverse per altri servizi Web. Ad esempio, il token API può essere inserito nel [!UICONTROL Intestazione] e non al [!UICONTROL Corpo] campo .

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>Il campo URL contiene l’endpoint che si trova nella documentazione API del servizio Web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL, Metodo]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>Il metodo utilizzato dipende dall’endpoint corrispondente. L’endpoint Pushover per il push dei messaggi utilizza il metodo POST .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
      <td> <p>Alcuni servizi web possono utilizzare le intestazioni per specificare l’autenticazione token API o altri parametri. Questo non è il caso nel nostro esempio, in quanto l’endpoint di Pushover per il push dei messaggi utilizza il corpo (vedi sotto) per tutti i tipi di richiesta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Query String]</p> </td> 
      <td> <p>Alcuni servizi web possono utilizzare una stringa di query per specificare altri parametri. Questo non è il caso nel nostro esempio come [!DNL Pushover] il servizio web utilizza [!UICONTROL Body] (vedi sotto) per tutti i tipi di richiesta.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Body Type]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>Questa impostazione ti consente di selezionare il tipo di contenuto JSON nel campo [!UICONTROL Content Type] (Tipo di contenuto JSON) riportato di seguito.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON è il tipo di contenuto richiesto dall’app [!UICONTROL Pushover]. Questo può differire da altri servizi web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Richiedi contenuto]</p> </td> 
      <td> <p>Inserisci il contenuto della richiesta [!UICONTROL Body] in formato JSON. Puoi utilizzare il modulo [!UICONTROL JSON] &gt; [!UICONTROL Crea JSON] come spiegato in <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">Corpo JSON mappato utilizzando il modulo [!UICONTROL JSON] &gt; [!UICONTROL Crea JSON]</a> in questo articolo. Oppure puoi immettere manualmente il contenuto JSON, come spiegato in <a href="#json-body-entered-manually" class="MCXref xref">Corpo JSON inserito manualmente</a> in questo articolo.</p> <p>Consulta la documentazione API del servizio Web per i parametri richiesti per quel servizio Web.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Corpo JSON inserito manualmente

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
   <td role="rowheader"> <p>[!UICONTROL utente]</p> </td> 
   <td> <p>Il tuo USER_KEY. Questo si trova nella [!DNL Pushover] dashboard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>Il token API/la chiave API generata hai creato il tuo [!DNL Pushover] app.</p> </td> 
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

## Corpo JSON mappato utilizzando [!UICONTROL JSON] >[!UICONTROL Creare JSON] modulo

La [!UICONTROL Creare JSON] Il modulo rende più semplice specificare JSON. Ti dà anche la possibilità di definire valori in modo dinamico.

Per ulteriori informazioni sui moduli JSON, vedi [Moduli JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Immetti o mappa i valori da cui desideri creare JSON.

   ![](assets/json-values-350x288.png)

1. Collega [!UICONTROL JSON] > [!UICONTROL Creare JSON] modulo per HTTP > Crea un modulo di richiesta.
1. Mappa la stringa JSON dal [!UICONTROL Creare JSON] al [!UICONTROL Contenuto della richiesta] nel campo [!UICONTROL HTTP] >[!UICONTROL Richiedi] modulo .

   Ora, quando esegui lo scenario, la notifica push viene inviata al dispositivo registrato nel tuo [!DNL Pushover] conto.
