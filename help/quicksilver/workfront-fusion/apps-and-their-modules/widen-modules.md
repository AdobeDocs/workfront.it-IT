---
title: Amplia moduli
description: In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!UICONTROL Widen], oltre a collegarlo a più applicazioni e servizi di terze parti.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 1%

---

# [!DNL Widen] moduli

In un [!DNL Adobe Workfront Fusion] scenario, puoi automatizzare i flussi di lavoro che utilizzano [!UICONTROL Widen], oltre a collegarlo a più applicazioni e servizi di terze parti.

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

Da utilizzare [!UICONTROL Widen] moduli, è necessario disporre di un [!UICONTROL Widen] account.

## Connetti [!DNL Widen] a [!DNL Workfront Fusion] {#connect-widen-to-workfront-fusion}

Puoi creare una connessione al tuo [!DNL Widen] account direttamente dall&#39;interno di un [!DNL Widen] modulo.

1. In qualsiasi [!DNL Widen] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo.
1. Seleziona la [!DNL Widen] dominio a cui desideri connetterti.
1. Immetti il token per il [!DNL Widen] account. Per istruzioni su come individuare questo token, vedi [[!DNL Widen] Domande frequenti sulle API](https://community.widen.com/collective/s/article/API-FAQs).
1. Clic **[!UICONTROL Continua]** per creare la connessione e tornare al modulo.

## [!DNL Widen] moduli e relativi campi

Quando si configura [!DNL Widen] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Widen] I campi potrebbero essere visualizzati in base a fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se viene visualizzato il pulsante Mappa sopra un campo o una funzione, è possibile utilizzarlo per impostare variabili e funzioni per tale campo. Per ulteriori informazioni, consulta [Mappare le informazioni da un modulo all’altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Moduli di attivazione](#trigger-modules)
* [Moduli azione](#action-modules)
* [Cerca moduli](#search-modules)

### Moduli di attivazione

#### [!UICONTROL Visualizzare le risorse]

Questo modulo di attivazione avvia uno scenario quando una risorsa viene creata o aggiornata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni sulla connessione [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo evento]</td> 
   <td> <p>Seleziona se desideri controllare le nuove risorse o le risorse aggiornate.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>Seleziona le proprietà da includere nell’output del modulo oltre ai campi della risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td>Selezionare i campi da includere nell'output del modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di risorse con cui si desidera che il modulo funzioni durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Moduli azione

* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Leggi informazioni risorsa]](#read-asset-info)
* [[!UICONTROL Aggiungere risorse alle raccolte]](#add-assets-to-collections)
* [[!UICONTROL Rimuovere risorse dalla raccolta]](#remove-assets-from-collection)
* [[!UICONTROL Aggiornare i metadati delle risorse]](#update-asset-metadata)
* [[!UICONTROL Scarica file]](#download-file)
* [[!UICONTROL Carica] un file](#upload-a-file)

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione consente di effettuare una chiamata autenticata personalizzata al [!DNL Widen] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Widen] moduli.

Durante la configurazione di questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni sulla connessione [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL versione API]</td> 
   <td>Seleziona se desideri utilizzare la versione più recente del [!DNL Widen] API o versione 1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Inserisci o mappa l’URL per la chiamata API.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] aggiunge automaticamente le intestazioni di autorizzazione.</p> </td> 
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

#### [!UICONTROL Leggi informazioni risorsa]

Questo modulo di azione recupera una singola risorsa in base al suo ID univoco.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni sulla connessione [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa]</td> 
   <td> <p>Immetti o mappa l’ID della risorsa per la quale desideri leggere le informazioni.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>Seleziona le proprietà da includere nell’output del modulo oltre ai campi della risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td>Selezionare i campi da includere nell'output del modulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiungere risorse alle raccolte]

Questo modulo di azione aggiunge una o più risorse alle raccolte.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni sulla connessione [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID Raccolte]</td> 
   <td> <p>Per ogni raccolta a cui desideri aggiungere le risorse:</p> 
    <ol> 
     <li value="1"> <p> Clic <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Immetti o mappa l'ID raccolta [!UICONTROL].</p> </li> 
     <li value="3"> <p>Clic <strong>[!UICONTROL Add item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assets ID]</td> 
   <td> <p>Per ogni risorsa da aggiungere a una raccolta:</p> 
    <ol> 
     <li value="1"> <p> Clic <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Inserisci o mappa l’ID risorsa.</p> </li> 
     <li value="3"> <p>Clic <strong>[!UICONTROL Add item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di risorse con cui si desidera che il modulo funzioni durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rimuovere risorse dalla raccolta]

Questo modulo di azione rimuove una o più risorse dalle raccolte.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni sulla connessione [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID Raccolte]</td> 
   <td> <p>Per ogni raccolta da cui vuoi rimuovere le risorse:</p> 
    <ol> 
     <li value="1"> <p> Clic <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Immetti o mappa l'ID raccolta.</p> </li> 
     <li value="3"> <p>Clic <strong>[!UICONTROL Add item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID risorse</td> 
   <td> <p>Per ogni risorsa da rimuovere da una raccolta:</p> 
    <ol> 
     <li value="1"> <p> Clic <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Inserisci o mappa l’ID risorsa.</p> </li> 
     <li value="3"> <p>Clic <strong>[!UICONTROL Add item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di risorse con cui si desidera che il modulo funzioni durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aggiornare i metadati delle risorse]

Questo modulo di azione aggiorna i campi di metadati di una risorsa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni sulla connessione [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa]</td> 
   <td> <p>Inserisci o mappa l’ID della risorsa in cui desideri aggiornare i metadati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo metadati]</td> 
   <td> <p>Seleziona il tipo di metadati per i metadati da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Metadati di [!UICONTROL]</td> 
   <td>Seleziona i campi di metadati da aggiornare. Immettere il nuovo valore per ogni campo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di risorse con cui si desidera che il modulo funzioni durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scarica file]

Questo modulo di azione scarica una risorsa dal tuo [!DNL Widen] account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni sulla connessione [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID risorsa]</td> 
   <td> <p>Inserisci o mappa l’ID della risorsa da scaricare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Carica un file]

Questo modulo di azione carica un file nel tuo [!DNL Widen] account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni sulla connessione [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carica profilo]</td> 
   <td> <p>Seleziona il profilo di caricamento che desideri utilizzare per il modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload Method]</td> 
   <td> <p>Seleziona la modalità di caricamento del file.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Da File]</strong> </p> <p>Seleziona o mappa il file di origine da un modulo precedente.</p> </li> 
     <li> <p><strong>[!UICONTROL Per URL]</strong> </p> <p>Inserisci o mappa l’URL del file da caricare.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nome file]</td> 
   <td>Inserisci o mappa un nome per il file caricato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo metadati]</td> 
   <td>Seleziona il tipo di metadati per il file da caricare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Metadati di [!UICONTROL]</td> 
   <td>Seleziona i campi di metadati da includere nel caricamento del file. Per ogni campo, immettere il valore [!UICONTROL] per il campo.</td> 
  </tr> 
 </tbody> 
</table>

### Cerca moduli

* [[!UICONTROL Lettura delle risorse della raccolta]](#read-collection-assets)
* [[!UICONTROL Cercare risorse]](#search-assets)

#### [!UICONTROL Lettura delle risorse della raccolta]

Questo modulo di azione recupera un elenco di risorse all’interno di una raccolta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni sulla connessione [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID raccolta]</td> 
   <td> <p>Inserisci o mappa l’ID della raccolta che contiene le risorse da leggere.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td>Immettere o mappare il numero del primo elemento da elencare. Questo è un modo per impaginare i record.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina per]</td> 
   <td> <p>Seleziona la proprietà in base alla quale desideri ordinare le risorse. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>Seleziona se desideri ordinare le risorse in modo crescente o decrescente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td>Selezionare i campi da includere nell'output del modulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cercare risorse]

Questo modulo di ricerca recupera un elenco di risorse che corrispondono ai criteri di ricerca specifici.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni sulla connessione [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query di ricerca [!UICONTROL]</td> 
   <td> <p>Inserire i criteri in base ai quali si desidera cercare le risorse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina per]</td> 
   <td> <p>Seleziona la modalità di ordinamento delle risorse. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>Seleziona se desideri ordinare le risorse in modo crescente o decrescente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include eliminato]</td> 
   <td>Abilita questa opzione per includere le risorse eliminate nella ricerca.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Include archiviato]</p> </td> 
   <td> <p>Abilita questa opzione per includere le risorse archiviate nella ricerca.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cerca testo documento]</td> 
   <td>Abilita questa opzione per includere il testo del documento nella ricerca oppure false per includere solo le risorse il cui titolo corrisponde ai criteri di ricerca.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che il modulo deve restituire durante ogni ciclo di esecuzione dello scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Offset]</td> 
   <td>Immettere o mappare il numero del primo elemento per il quale si desidera recuperare i dettagli. Questo è un modo per impaginare i record.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scroll]</td> 
   <td>Abilita questa opzione per consentire lo scorrimento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>Seleziona le proprietà da includere nell’output del modulo oltre ai campi della risorsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td>Selezionare i campi da includere nell'output del modulo.</td> 
  </tr> 
 </tbody> 
</table>
