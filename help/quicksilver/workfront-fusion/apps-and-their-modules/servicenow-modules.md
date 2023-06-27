---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: apps-and-their-modules
title: Moduli ServiceNow
description: In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL ServiceNow], oltre a collegarlo a più applicazioni e servizi di terze parti.
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1613'
ht-degree: 1%

---

# [!DNL ServiceNow] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!DNL ServiceNow], oltre a collegarlo a più applicazioni e servizi di terze parti.

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

Da utilizzare [!DNL ServiceNow] moduli, è necessario disporre di un [!DNL ServiceNow] account.

## Connetti [!DNL ServiceNow] a [!DNL Workfront Fusion]

Per creare una connessione per [!DNL ServiceNow] moduli:

1. Clic **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] quando si inizia la configurazione della prima [!DNL ServiceNow] modulo.
1. Immetti quanto segue:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nome connessione]</p> </td> 
      <td>Immetti un nome per il nuovo [!DNL ServiceNow] connessione</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Username]</p> </td> 
      <td>Immetti il [!DNL ServiceNow] nome utente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Password]</p> </td> 
      <td>Immettere la password ServiceNow.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Instance]</p> </td> 
      <td> <p>Inserisci l’indirizzo del tuo [!DNL ServiceNow] account senza <code>https://</code> (in genere <code>&lt;company>.service-now.com</code>).</p> </td> 
     </tr> 
    </tbody> 
   </table>

## [!UICONTROL ServiceNow] moduli e relativi campi

Quando si configura [!DNL ServiceNow] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL ServiceNow] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>Se è selezionato un record personalizzato in un’&quot;[!UICONTROL Tipo di record]&quot;, il caricamento dei campi personalizzati potrebbe richiedere del tempo.
>
>Se non sono presenti record personalizzati, il menu a discesa sarà vuoto.

* [[!UICONTROL Osserva i record]](#watch-records)
* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Leggi un record]](#read-a-record)
* [[!UICONTROL Disattivare un utente]](#deactivate-a-user)
* [[!UICONTROL Scaricare un allegato]](#download-an-attachment)
* [[!UICONTROL Carica un allegato]](#upload-an-attachment)
* [[!UICONTROL Creare un record]](#create-a-record)
* [[!UICONTROL Aggiornare un record]](#update-a-record)
* [[!UICONTROL Eliminare un record]](#delete-a-record)
* [[!UICONTROL Cerca record]](#search-for-records)

### [!UICONTROL Osserva i record]

Questo modulo di attivazione attiva uno scenario quando viene creato o aggiornato un record.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di tabella]</td> 
   <td>Seleziona se la tabella da guardare è una tabella personalizzata o standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record che si desidera controllare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Selezionare il tipo di valori che si desidera visualizzare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td>Selezionare i campi che si desidera vengano generati dal modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td>Specificare se si desidera controllare i nuovi record o i record aggiornati.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione consente di effettuare una chiamata autenticata personalizzata al [!DNL ServiceNow] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL ServiceNow] moduli.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL relativo]</td> 
   <td> <p>Digita l’indirizzo sul server web con cui desideri che interagisca il modulo.</p> <p>Puoi digitare un URL relativo, il che significa che non devi includere il protocollo (ad esempio <code>http://</code>) all'inizio. Questo suggerisce al server web che l’interazione si sta verificando sul server.</p> <p>Ad esempio: <code>[!DNL /api/conversations].create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> </td> 
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

### [!UICONTROL Leggi un record]

Questo modulo di azione legge un [!DNL ServiceNow] registrare utilizzando l&#39;ID di sistema.

Il modulo restituisce tutti i campi standard associati al record, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>Inserisci o mappa l’univoco [!DNL ServiceNow] ID del record che desideri che il modulo legga.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di tabella]</td> 
   <td>Specificare se il record da leggere si trova in una tabella personalizzata o in una tabella standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Seleziona il tipo di [!DNL ServiceNow] che si desidera che il modulo legga.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Selezionare il tipo di valori che si desidera visualizzare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
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
   <td> <p>Per istruzioni sulla connessione dell'account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User System ID]</td> 
   <td> Inserisci o mappa l’univoco [!DNL ServiceNow] ID dell’utente che desideri disattivare il modulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Scaricare un allegato]

Questo modulo di azione scarica un allegato in una [!DNL ServiceNow] record.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment System ID]</td> 
   <td> Inserisci o mappa l’univoco [!DNL ServiceNow] ID dell’allegato che desideri scaricare dal modulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Carica un allegato]

Questo modulo di azione carica un allegato in un [!DNL ServiceNow] record.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome tabella]</td> 
   <td>Immettere o mappare il nome della tabella in cui si desidera caricare l'allegato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID sistema]</td> 
   <td>Inserisci o mappa l’univoco [!DNL ServiceNow] ID del sistema in cui desideri caricare l’allegato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome file]</td> 
   <td>Immettere o mappare un nome per l'allegato</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenuto file]</td> 
   <td>Inserisci o mappa il file in cui desideri caricare [!DNL ServiceNow].</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Creare un record]

Questo modulo di azione crea un nuovo [!DNL ServiceNow] record.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di tabella]</td> 
   <td>Specificare se si desidera creare un record in una tabella personalizzata o standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Seleziona il tipo di [!DNL ServiceNow] che si desidera creare nel modulo. È quindi possibile compilare i campi disponibili per questo tipo di record.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Aggiornare un record]

Questo modulo di azione crea un nuovo [!DNL ServiceNow] record.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>Inserisci o mappa l’univoco [!DNL ServiceNow] ID del record che desideri aggiornare nel modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di tabella]</td> 
   <td>Specificare se il record da aggiornare si trova in una tabella personalizzata o in una tabella standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Seleziona il tipo di [!DNL ServiceNow] che desideri aggiornare il modulo. È quindi possibile compilare i campi disponibili per questo tipo di record.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminare un record]

Questo modulo di azione elimina un incidente o un utente.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Specificare se si desidera eliminare un incidente o un utente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID sistema]</td> 
   <td>Inserisci o mappa l’univoco [!DNL ServiceNow] ID del record che desideri eliminare dal modulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Cerca record]

Questo modulo cerca i record utilizzando i criteri selezionati.

Il modulo restituisce tutti i campi standard associati al record, insieme a tutti i campi e i valori personalizzati a cui la connessione accede. Puoi mappare queste informazioni nei moduli successivi nello scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione dell'account ServiceNow a [!DNL Workfront Fusion], vedi <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Connetti [!DNL ServiceNow] a [!UICONTROL Workfront Fusion]</a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di tabella]</td> 
   <td>Seleziona se la tabella da cercare è una tabella personalizzata o standard.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di record]</td> 
   <td>Selezionare il tipo di record che si desidera cercare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Set di risultati]</td> 
   <td>Specificare se si desidera che il modulo restituisca tutti i record che corrispondono ai criteri oppure solo il primo record corrispondente. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conteggio massimo dei record]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo di ricerca [!UICONTROL]</td> 
   <td> <p>Seleziona il tipo di ricerca da eseguire nel modulo</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Advanced query]</strong> </p> 
      <ul> 
       <li> <p>Query di ricerca [!UICONTROL]</p> <p>Immettere la query di ricerca personalizzata. Per informazioni su [!DNL ServiceNow] query di ricerca personalizzate, vedi <a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">Documentazione sulle query ServiceNow</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL semplice]</strong> </p> 
      <ul> 
       <li> <p>Criteri di ricerca di [!UICONTROL]</p> <p>Immettere i criteri in base ai quali si desidera eseguire la ricerca nel modulo. Per ulteriori informazioni sulla configurazione dei filtri di ricerca, consulta <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Aggiungere un filtro a uno scenario in Adobe Workfront Fusion</a>.</p> </li> 
       <li> <p>[!UICONTROL Ordina per]</p> <p>Indica per quale campo desideri che il modulo ordini i risultati e se devono essere ordinati in ordine crescente o decrescente.</p> </li> 
      </ul> </li> 
    </ul> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Selezionare il tipo di valori che si desidera visualizzare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td>Selezionare i campi che si desidera vengano generati dal modulo.</td> 
  </tr> 
 </tbody> 
</table>
