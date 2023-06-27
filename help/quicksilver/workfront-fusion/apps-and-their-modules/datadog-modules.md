---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Datadog
description: In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano Datadog, nonché collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 1%

---

# [!DNL Datadog] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL Datadog], oltre a collegarlo a più applicazioni e servizi di terze parti.

Per istruzioni sulla creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Da utilizzare [!DNL Datadog] moduli, è necessario disporre di un [!DNL Datadog] account.

## Connetti [!DNL Datadog] a [!DNL Workfront Fusion] {#connect-datadog-to-workfront-fusion}

### Recuperare la chiave API e la chiave dell’applicazione {#retrieve-your-api-key-and-application-key}

Per collegare [!DNL Datadog] account a [!DNL Workfront Fusion] è necessario recuperare una chiave API e una chiave dell’applicazione dal file [!DNL Datadog] account.

1. Accedi al tuo [!DNL Datadog] account.
1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Integrazioni]**, quindi fai clic su **[!UICONTROL API]**.
1. Nella schermata principale, fai clic su **[!UICONTROL Chiavi API]**.
1. Passa il puntatore del mouse sulla barra viola per visualizzare la chiave API.
1. Copia la chiave API in un percorso sicuro.
1. Nella schermata principale, fai clic su **[!UICONTROL Chiavi applicazione]**.
1. Passa il cursore del mouse sulla barra viola per visualizzare il tasto dell’applicazione.
1. Copiare la chiave dell&#39;applicazione in un percorso sicuro.

### Creare una connessione a [!DNL Datadog] in [!DNL Workfront Fusion]

Puoi creare una connessione al tuo [!DNL Datadog] account direttamente dall&#39;interno di un [!UICONTROL Datadog] modulo.

1. In qualsiasi [!UICONTROL Datadog] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo.
1. Compila i campi del modulo come segue:

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipo di connessione [!UICONTROL]</td> 
      <td> <p> Seleziona [!UICONTROL [!DNL Datadog] Applicazione] per ottenere l'accesso completo a [!DNL Datadog] API.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome connessione]</td> 
      <td> <p> Immettere un nome per la connessione.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Domain] </td> 
      <td> <p>Seleziona il dominio a cui desideri connetterti (USA o UE).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API Key]</td> 
      <td> <p> Immetti il [!DNL Datadog] Chiave API. </p> <p>Per istruzioni sul recupero della chiave API, consulta <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Recuperare la chiave API e la chiave dell’applicazione</a> in questo articolo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Chiave Applicazione]</td> 
      <td> <p> Immetti il [!DNL Datadog] chiave dell'applicazione. </p> <p>Per istruzioni sul recupero della chiave dell'applicazione, vedere <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Recuperare la chiave API e la chiave dell’applicazione</a> in questo articolo.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

## [!DNL Datadog] moduli e relativi campi

Quando si configura [!DNL Datadog] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Datadog] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Azioni

* [[!UICONTROL Pubblica punti serie temporali]](#post-timeseries-points)
* [[!UICONTROL Effettuare una chiamata API]](#make-an-api-call)

#### [!UICONTROL Pubblica punti serie temporali]

Il modulo consente di registrare dati di serie temporali che possono essere tracciati su [!DNL Datadog]Dashboard di.

Il limite per i payload compressi è di 3,2 megabyte (3200000) e 62 megabyte (62914560) per i payload decompressi.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Datadog] account a [!DNL Workfront Fusion], vedi <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Datadog] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Series]</td> 
   <td> <p>Aggiungere serie temporali alle quali si desidera inviare [!DNL Datadog].</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Metric]</strong> </p> <p>Immetti il nome della serie temporale.</p> </li> 
     <li> <p><strong>[!UICONTROL Type]</strong> </p> <p>Seleziona il tipo di metrica.</p> </li> 
     <li> <p><strong>[!UICONTROL Interval]</strong> </p> <p> Se il tipo di metrica è tasso o conteggio, definisci l’intervallo corrispondente.</p> </li> 
     <li> <p><strong>[!UICONTROL Punti]</strong> </p> <p>Aggiungere punti relativi a una metrica.</p> <p>Questo è un array JSON di punti. Ogni punto ha il formato: <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>Nota:  <p>Il timestamp deve essere in secondi.</p> <p>Il timestamp deve essere corrente. Corrente è definita come non più di 10 minuti nel futuro o più di 1 ora nel passato.</p> <p> Il formato del valore numerico deve essere un valore mobile.</p> </p> <p>Questo campo deve contenere almeno 1 elemento.</p> </li> 
     <li> <p><strong>[!UICONTROL Host]</strong> </p> <p>Immetti il nome dell’host che ha prodotto la metrica.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effettuare una chiamata API]

Questo modulo di azione ti consente di eseguire una chiamata API personalizzata.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Datadog] account a [!DNL Workfront Fusion], vedi <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Datadog] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Inserisci un percorso relativo a <code>https://api.datadoghq.com/api/</code>. Esempio:<code> /v1/org</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stringa Di Query]</td> 
   <td> <p>Aggiungi la query per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali quali <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Esempio:** La seguente chiamata API restituisce tutti i dashboard nel tuo [!DNL Datadog] account:

URL: `/v1/dashboard`

Metodo: `GET`

![](assets/datadog-api-example.png)

Il risultato si trova nell’Output del modulo in Bundle > Corpo > dashboard.

Nel nostro esempio, sono state restituite 3 dashboard:

![](assets/datadog-api-response-example.png)
