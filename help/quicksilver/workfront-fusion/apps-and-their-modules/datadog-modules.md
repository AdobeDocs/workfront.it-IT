---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli Datadog
description: La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione. Questo articolo è stato dichiarato obsoleto, ma contiene un collegamento al nuovo articolo che descrive questa funzionalità.
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%

---

# [!DNL Datadog] moduli

>[!IMPORTANT]
>
>La documentazione di Adobe Workfront Fusion è stata spostata in una nuova posizione.
>
>Le informazioni contenute in questo articolo sono ora disponibili nell’articolo:
>
>* [Moduli Datadog](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/datadog-modules.html)
>
>Aggiorna eventuali segnalibri.
>
>Questo articolo non è più in fase di aggiornamento e verrà rimosso nel prossimo futuro.

In uno scenario [!DNL Adobe Workfront Fusion], è possibile automatizzare i flussi di lavoro che utilizzano [!DNL Datadog] e collegarlo a più applicazioni e servizi di terze parti.

Se hai bisogno di istruzioni per la creazione di uno scenario, consulta [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, vedere [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Prerequisiti

Per utilizzare i moduli [!DNL Datadog], è necessario disporre di un account [!DNL Datadog].

## Informazioni API Datadog

Il connettore Datadog utilizza quanto segue:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Tag API</td> 
   <td>1.0.11</td> 
  </tr>
 </tbody> 
 </table>

## Connetti [!DNL Datadog] a [!DNL Workfront Fusion] {#connect-datadog-to-workfront-fusion}

### Recuperare la chiave API e la chiave dell’applicazione {#retrieve-your-api-key-and-application-key}

Per connettere l&#39;account [!DNL Datadog] a [!DNL Workfront Fusion] è necessario recuperare una chiave API e una chiave applicazione dall&#39;account [!DNL Datadog].

1. Accedi al tuo account [!DNL Datadog].
1. Nel pannello di navigazione a sinistra, fai clic su **[!UICONTROL Integrazioni]**, quindi su **[!UICONTROL API]**.
1. Nella schermata principale, fai clic su **[!UICONTROL Chiavi API]**.
1. Passa il puntatore del mouse sulla barra viola per visualizzare la chiave API.
1. Copia la chiave API in un percorso sicuro.
1. Nella schermata principale, fai clic su **[!UICONTROL Chiavi applicazione]**.
1. Passa il cursore del mouse sulla barra viola per visualizzare il tasto dell’applicazione.
1. Copiare la chiave dell&#39;applicazione in un percorso sicuro.

### Crea una connessione a [!DNL Datadog] in [!DNL Workfront Fusion]

Puoi creare una connessione al tuo account [!DNL Datadog] direttamente da un modulo [!UICONTROL Datadog].

1. In qualsiasi modulo [!UICONTROL Datadog], fai clic su **[!UICONTROL Aggiungi]** accanto al campo [!UICONTROL Connessione].
1. Compila i campi del modulo come segue:

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipo di connessione [!UICONTROL]</td> 
      <td> <p> Selezionare l'opzione [!UICONTROL [!DNL Datadog] Application] per accedere completamente all'API [!DNL Datadog].</p> </td> 
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
      <td> <p> Immetti la tua chiave API [!DNL Datadog]. </p> <p>Per istruzioni sul recupero della chiave API, consulta <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Recuperare la chiave API e la chiave dell'applicazione</a> in questo articolo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Chiave Applicazione]</td> 
      <td> <p> Immetti la chiave dell'applicazione [!DNL Datadog]. </p> <p>Per istruzioni sul recupero della chiave dell'applicazione, vedere <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Recuperare la chiave dell'API e la chiave dell'applicazione</a> in questo articolo.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

## [!DNL Datadog] moduli e relativi campi

Quando configuri [!DNL Datadog] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Insieme a questi, potrebbero essere visualizzati ulteriori campi di [!DNL Datadog], a seconda di fattori quali il livello di accesso nell&#39;app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, vedere [Mappare le informazioni da un modulo all&#39;altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Azioni

* [[!UICONTROL Pubblica punti serie temporali]](#post-timeseries-points)
* [[!UICONTROL Effettuare una chiamata API]](#make-an-api-call)

#### [!UICONTROL Pubblica punti serie temporali]

Il modulo ti consente di pubblicare dati di serie temporali che possono essere tracciati nei dashboard di [!DNL Datadog].

Il limite per i payload compressi è di 3,2 megabyte (3200000) e 62 megabyte (62914560) per i payload decompressi.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Datadog] a [!DNL Workfront Fusion], vedere <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Datadog] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Series]</td> 
   <td> <p>Aggiungere serie temporali da inviare a [!DNL Datadog].</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Metrica]</strong> </p> <p>Immetti il nome della serie temporale.</p> </li> 
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
   <td> <p>Per istruzioni sulla connessione dell'account [!DNL Datadog] a [!DNL Workfront Fusion], vedere <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Connessione di [!DNL Datadog] a [!DNL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Immettere un percorso relativo a <code>https://api.datadoghq.com/api/</code>. Esempio:<code> /v1/org</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, vedere <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>Aggiungi il contenuto body per la chiamata API sotto forma di oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserire le virgolette al di fuori dell'istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Esempio:** La seguente chiamata API restituisce tutti i dashboard nel tuo account [!DNL Datadog]:

URL: `/v1/dashboard`

Metodo: `GET`

![](assets/datadog-api-example.png)

Il risultato si trova nell’Output del modulo in Bundle > Corpo > dashboard.

Nel nostro esempio, sono state restituite 3 dashboard:

![](assets/datadog-api-response-example.png)
