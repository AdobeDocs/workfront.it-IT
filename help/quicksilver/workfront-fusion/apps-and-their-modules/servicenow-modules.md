---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli ServiceNow
description: In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL ServiceNow], nonché collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1565'
ht-degree: 0%

---

# [!DNL ServiceNow] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!DNL ServiceNow], nonché collegarlo a più applicazioni e servizi di terze parti.

Se hai bisogno di istruzioni su come creare uno scenario, vedi [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Per informazioni sui moduli, consulta [Moduli in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Per utilizzare [!DNL ServiceNow] moduli, è necessario disporre di un [!DNL ServiceNow] conto.

## Connetti [!DNL ServiceNow] a [!DNL Workfront Fusion]

Per creare una connessione per [!DNL ServiceNow] moduli:

1. Fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] quando si inizia a configurare il primo [!DNL ServiceNow] modulo .
1. Immetti quanto segue:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome connessione]</p> </td> 
      <td>Immettere un nome per il nuovo [!DNL ServiceNow] connection</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Username]</p> </td> 
      <td>Inserisci il tuo [!DNL ServiceNow] nome utente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Password]</p> </td> 
      <td>Immetti la password di ServiceNow.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Instance]</p> </td> 
      <td> <p>Inserisci l'indirizzo del tuo [!DNL ServiceNow] account senza <code>https://</code> (solitamente <code>&lt;company>.service-now.com</code>).</p> </td> 
     </tr> 
    </tbody> 
   </table>

## [!UICONTROL ServiceNow] moduli e relativi campi

Quando si configura [!DNL ServiceNow] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL ServiceNow] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>Se è selezionato un record personalizzato in un &quot;[!UICONTROL Tipo di record]&quot;, il caricamento dei campi personalizzati potrebbe richiedere del tempo.
>
>Se non sono presenti record personalizzati, il menu a discesa sarà vuoto.

* [[!UICONTROL Registri di controllo]](#watch-records)
* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Leggi un record]](#read-a-record)
* [[!UICONTROL Disattivare un utente]](#deactivate-a-user)
* [[!UICONTROL Scaricare un allegato]](#download-an-attachment)
* [[!UICONTROL Caricare un allegato]](#upload-an-attachment)
* [[!UICONTROL Creare un record]](#create-a-record)
* [[!UICONTROL Aggiornare un record]](#update-a-record)
* [[!UICONTROL Eliminare un record]](#delete-a-record)
* [[!UICONTROL Cerca record]](#search-for-records)

### [!UICONTROL Registri di controllo]

Questo modulo trigger attiva uno scenario quando viene creato o aggiornato un record.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare il tuo account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo tabella]</td> 
   <td>Selezionare se la tabella che si desidera visualizzare è una tabella personalizzata o una tabella standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record che si desidera visualizzare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Selezionare il tipo di valori da visualizzare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td>Selezionare i campi che si desidera vengano generati dal modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Selezionare se si desidera visualizzare nuovi record o record aggiornati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata al [!DNL ServiceNow] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL ServiceNow] moduli.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare il tuo account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL relativo]</td> 
   <td> <p>Digita l’indirizzo sul server web con cui desideri interagire il modulo.</p> <p>Puoi digitare un URL relativo, il che significa che non devi includere il protocollo (ad esempio <code>http://</code>) all'inizio. Questo suggerisce al server web di verificare che l'interazione si verifichi sul server.</p> <p>Ad esempio: <code>[!DNL /api/conversations].create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Metodo]</td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Aggiungi la query per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Aggiungi il contenuto del corpo per la chiamata API sotto forma di un oggetto JSON standard.</p> <p>Nota:  <p>Quando si utilizzano istruzioni condizionali come <code>if</code> nel JSON, inserisci le virgolette al di fuori dell’istruzione condizionale.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Leggi un record]

Questo modulo di azione legge un [!DNL ServiceNow] registra utilizzando l&#39;ID di sistema.

Il modulo restituisce tutti i campi standard associati al record, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare il tuo account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>Immetti o mappa l'univoco [!DNL ServiceNow] ID del record che si desidera leggere nel modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo tabella]</td> 
   <td>Selezionare se il record che si desidera leggere si trova in una tabella personalizzata o in una tabella standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Seleziona il tipo di [!DNL ServiceNow] registrare che si desidera che il modulo legga.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Selezionare il tipo di valori da visualizzare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td>Selezionare i campi che si desidera vengano generati dal modulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Disattivare un utente]

Questo modulo di azione disattiva un utente in [!DNL ServiceNow] utilizzando l&#39;ID di sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare il tuo account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User System ID]</td> 
   <td> Immetti o mappa l'univoco [!DNL ServiceNow] ID dell’utente che desideri disattivare del modulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Scaricare un allegato]

Questo modulo di azione scarica un allegato in un [!DNL ServiceNow] record.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare il tuo account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment System ID]</td> 
   <td> Immetti o mappa l'univoco [!DNL ServiceNow] ID dell'allegato che desideri scaricare nel modulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Caricare un allegato]

Questo modulo di azione carica un allegato a un [!DNL ServiceNow] record.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare il tuo account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome tabella]</td> 
   <td>Immettere o mappare il nome della tabella in cui si desidera caricare l'allegato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL System ID]</td> 
   <td>Immetti o mappa l'univoco [!DNL ServiceNow] ID del sistema in cui si desidera caricare l'allegato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Immettere o mappare un nome per l'allegato</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenuto del file]</td> 
   <td>Immetti o mappa il file da caricare [!DNL ServiceNow].</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Creare un record]

Questo modulo di azione crea un nuovo [!DNL ServiceNow] record.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare il tuo account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo tabella]</td> 
   <td>Selezionare se si desidera creare un record in una tabella personalizzata o in una tabella standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Seleziona il tipo di [!DNL ServiceNow] registrare che si desidera creare il modulo. È quindi possibile compilare i campi disponibili per questo tipo di record.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Aggiornare un record]

Questo modulo di azione crea un nuovo [!DNL ServiceNow] record.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare il tuo account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>Immetti o mappa l'univoco [!DNL ServiceNow] ID del record che si desidera aggiornare nel modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo tabella]</td> 
   <td>Selezionare se il record che si desidera aggiornare si trova in una tabella personalizzata o in una tabella standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Seleziona il tipo di [!DNL ServiceNow] registrare che si desidera aggiornare il modulo. È quindi possibile compilare i campi disponibili per questo tipo di record.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un incidente o un utente.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare il tuo account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Seleziona se desideri eliminare un incidente o un utente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL System ID]</td> 
   <td>Immetti o mappa l'univoco [!DNL ServiceNow] ID del record che si desidera eliminare dal modulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Cerca record]

Questo modulo cerca i record utilizzando i criteri selezionati.

Il modulo restituisce tutti i campi standard associati al record, insieme a eventuali campi e valori personalizzati a cui accede la connessione. Puoi mappare queste informazioni nei moduli successivi nello scenario .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare il tuo account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo tabella]</td> 
   <td>Selezionare se la tabella che si desidera cercare è una tabella personalizzata o una tabella standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record da cercare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Set di risultati]</td> 
   <td>Selezionare se si desidera che il modulo restituisca tutti i record corrispondenti ai criteri oppure solo il primo record corrispondente. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteggio massimo dei record]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di ricerca]</td> 
   <td> <p>Selezionare il tipo di ricerca che si desidera eseguire nel modulo</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Query avanzata]</strong> </p> 
      <ul> 
       <li> <p>Query di ricerca [!UICONTROL]</p> <p>Inserisci la query di ricerca personalizzata. Per informazioni su [!DNL ServiceNow] query di ricerca personalizzate, vedi <a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">Documentazione della query ServiceNow</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Semplice]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Criteri di ricerca]</p> <p>Immetti i criteri in base ai quali desideri eseguire la ricerca nel modulo. Per ulteriori informazioni sulla configurazione dei filtri di ricerca, consulta <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Aggiungere un filtro a uno scenario in Adobe Workfront Fusion</a>.</p> </li> 
       <li> <p>[!UICONTROL Ordina per]</p> <p>Indicare il campo in base al quale il modulo deve ordinare i risultati e se deve essere ordinato in ordine crescente o decrescente.</p> </li> 
      </ul> </li> 
    </ul> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Selezionare il tipo di valori da visualizzare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td>Selezionare i campi che si desidera che vengano generati dal modulo.</td> 
  </tr> 
 </tbody> 
</table>
