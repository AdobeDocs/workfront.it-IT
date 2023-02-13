---
title: Moduli ampliati
description: In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!UICONTROL Ampliamento], nonché collegarlo a più applicazioni e servizi di terze parti.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1538'
ht-degree: 1%

---

# [!DNL Widen] moduli

In un [!DNL Adobe Workfront Fusion] puoi automatizzare i flussi di lavoro che utilizzano [!UICONTROL Ampliamento], nonché collegarlo a più applicazioni e servizi di terze parti.

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

Per utilizzare [!UICONTROL Ampliamento] moduli, è necessario disporre di un [!UICONTROL Ampliamento] conto.

## Connetti [!DNL Widen] a [!DNL Workfront Fusion] {#connect-widen-to-workfront-fusion}

Puoi creare una connessione al tuo [!DNL Widen] account direttamente dall&#39;interno di un [!DNL Widen] modulo .

1. In qualsiasi [!DNL Widen] modulo, fai clic su **[!UICONTROL Aggiungi]** accanto al [!UICONTROL Connessione] campo .
1. Seleziona la [!DNL Widen] dominio a cui si desidera connettersi.
1. Immetti il token per il tuo [!DNL Widen] conto. Per istruzioni su come individuare il token, consulta la [[!DNL Widen] Domande frequenti sulle API](https://community.widen.com/collective/s/article/API-FAQs).
1. Fai clic su **[!UICONTROL Continua]** per creare la connessione e tornare al modulo .

## [!DNL Widen] moduli e relativi campi

Quando si configura [!DNL Widen] moduli, [!DNL Workfront Fusion] visualizza i campi elencati di seguito. Oltre a questi, ulteriori [!DNL Widen] potrebbero essere visualizzati, a seconda di fattori quali il livello di accesso nell’app o nel servizio. Un titolo in grassetto in un modulo indica un campo obbligatorio.

Se trovi il pulsante mappa sopra un campo o una funzione, puoi utilizzarlo per impostare variabili e funzioni per quel campo. Per ulteriori informazioni, consulta [Mappare informazioni da un modulo a un altro in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Moduli trigger](#trigger-modules)
* [Moduli azione](#action-modules)
* [Moduli di ricerca](#search-modules)

### Moduli trigger

#### [!UICONTROL Visualizzare le risorse]

Questo modulo di attivazione avvia uno scenario quando una risorsa viene creata o aggiornata.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni su come collegare le [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo evento]</td> 
   <td> <p>Seleziona se visualizzare le nuove risorse o le risorse aggiornate.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Espandi]</td> 
   <td> <p>Oltre ai campi delle risorse, seleziona le proprietà che desideri includere nell’output del modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td>Selezionare i campi che si desidera includere nell'output del modulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immetti o mappa il numero massimo di risorse con cui desideri che il modulo funzioni durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Moduli azione

* [[!UICONTROL Chiamata API personalizzata]](#custom-api-call)
* [[!UICONTROL Leggi le informazioni sulle risorse]](#read-asset-info)
* [[!UICONTROL Aggiungere risorse alle raccolte]](#add-assets-to-collections)
* [[!UICONTROL Rimuovere risorse dalla raccolta]](#remove-assets-from-collection)
* [[!UICONTROL Aggiornare i metadati delle risorse]](#update-asset-metadata)
* [[!UICONTROL Scarica file]](#download-file)
* [[!UICONTROL Carica] un file](#upload-a-file)

#### [!UICONTROL Chiamata API personalizzata]

Questo modulo di azione ti consente di effettuare una chiamata autenticata personalizzata al [!DNL Widen] API. In questo modo, puoi creare un’automazione del flusso di dati che non può essere eseguita dall’altro [!DNL Widen] moduli.

Quando si configura questo modulo, vengono visualizzati i campi seguenti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Per istruzioni su come collegare le [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Seleziona se desideri utilizzare la versione più recente del [!DNL Widen] API o versione 1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Immetti o mappa l’URL per la chiamata API.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Metodo]</td> 
   <td> <p>Seleziona il metodo di richiesta HTTP necessario per configurare la chiamata API. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">metodi di richiesta HTTP in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Aggiungi le intestazioni della richiesta sotto forma di un oggetto JSON standard.</p> <p>Ad esempio: <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] aggiunge le intestazioni di autorizzazione.</p> </td> 
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

#### [!UICONTROL Leggi le informazioni sulle risorse]

Questo modulo di azione recupera una singola risorsa dal relativo ID univoco.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni su come collegare le [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>Immetti o mappa l’ID della risorsa per la quale desideri leggere le informazioni.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Espandi]</td> 
   <td> <p>Oltre ai campi delle risorse, seleziona le proprietà che desideri includere nell’output del modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td>Selezionare i campi che si desidera includere nell'output del modulo.</td> 
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
  <td> <p>Per istruzioni su come collegare le [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collections ID]</td> 
   <td> <p>Per ogni raccolta a cui desideri aggiungere le risorse:</p> 
    <ol> 
     <li value="1"> <p> Fai clic su <strong>[!UICONTROL Aggiungi]</strong>.</p> </li> 
     <li value="2"> <p>Immetti o mappa l' [!UICONTROL Collection ID].</p> </li> 
     <li value="3"> <p>Fai clic su <strong>[!UICONTROL Aggiungi elemento]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID [!UICONTROL Assets]</td> 
   <td> <p>Per ogni risorsa che desideri aggiungere a una raccolta:</p> 
    <ol> 
     <li value="1"> <p> Fai clic su <strong>[!UICONTROL Aggiungi]</strong>.</p> </li> 
     <li value="2"> <p>Immetti o mappa l’ID risorsa.</p> </li> 
     <li value="3"> <p>Fai clic su <strong>[!UICONTROL Aggiungi elemento]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immetti o mappa il numero massimo di risorse con cui desideri che il modulo funzioni durante ogni ciclo di esecuzione degli scenari.</p> </td> 
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
  <td> <p>Per istruzioni su come collegare le [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collections ID]</td> 
   <td> <p>Per ogni raccolta da cui desideri rimuovere le risorse:</p> 
    <ol> 
     <li value="1"> <p> Fai clic su <strong>[!UICONTROL Aggiungi]</strong>.</p> </li> 
     <li value="2"> <p>Immetti o mappa l'ID raccolta.</p> </li> 
     <li value="3"> <p>Fai clic su <strong>[!UICONTROL Aggiungi elemento]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID risorsa</td> 
   <td> <p>Per ogni risorsa da rimuovere da una raccolta:</p> 
    <ol> 
     <li value="1"> <p> Fai clic su <strong>[!UICONTROL Aggiungi]</strong>.</p> </li> 
     <li value="2"> <p>Immetti o mappa l’ID risorsa.</p> </li> 
     <li value="3"> <p>Fai clic su <strong>[!UICONTROL Aggiungi elemento]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immetti o mappa il numero massimo di risorse con cui desideri che il modulo funzioni durante ogni ciclo di esecuzione degli scenari.</p> </td> 
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
  <td> <p>Per istruzioni su come collegare le [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>Immetti o mappa l’ID della risorsa in cui desideri aggiornare i metadati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di metadati]</td> 
   <td> <p>Seleziona il tipo di metadati per i metadati da aggiornare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>Seleziona i campi di metadati da aggiornare. Per ciascun campo, immettere il nuovo valore del campo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immetti o mappa il numero massimo di risorse con cui desideri che il modulo funzioni durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scarica file]

Questo modulo di azione scarica una risorsa dal tuo [!DNL Widen] conto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni su come collegare le [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>Immetti o mappa l’ID della risorsa da scaricare.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Caricare un file]

Questo modulo di azione carica un file nel tuo [!DNL Widen] conto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni su come collegare le [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carica profilo]</td> 
   <td> <p>Seleziona il profilo di caricamento da utilizzare nel modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload Method]</td> 
   <td> <p>Seleziona la modalità di caricamento del file.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Da File]</strong> </p> <p>Selezionare o mappare il file di origine da un modulo precedente.</p> </li> 
     <li> <p><strong>[!UICONTROL Per URL]</strong> </p> <p>Immetti o mappa l’URL del file da caricare.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Immetti o mappa un nome per il file caricato.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo di metadati]</td> 
   <td>Seleziona il tipo di metadati per il file da caricare.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>Seleziona i campi di metadati da includere nel caricamento del file. Per ciascun campo, immetti il [!UICONTROL value] del campo.</td> 
  </tr> 
 </tbody> 
</table>

### Moduli di ricerca

* [[!UICONTROL Leggere le risorse di raccolta]](#read-collection-assets)
* [[!UICONTROL Cercare risorse]](#search-assets)

#### [!UICONTROL Leggere le risorse di raccolta]

Questo modulo di azione recupera un elenco di risorse all’interno di una raccolta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni su come collegare le [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID raccolta [!UICONTROL]</td> 
   <td> <p>Immetti o mappa l’ID della raccolta contenente le risorse da leggere.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td>Immettere o mappare il numero del primo elemento da elencare. Questo è un modo per impaginare i record.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina per]</td> 
   <td> <p>Seleziona la proprietà in base alla quale vuoi ordinare le risorse. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>Seleziona se ordinare le risorse in ordine crescente o decrescente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td>Selezionare i campi che si desidera includere nell'output del modulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cercare risorse]

Questo modulo di ricerca recupera un elenco di risorse che corrispondono a criteri di ricerca specifici.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Per istruzioni su come collegare le [!DNL Widen] account a [!DNL Workfront Fusion], vedi <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connetti [!DNL Widen] a [!DNL Workfront Fusion] </a> in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ricerca query]</td> 
   <td> <p>Immetti i criteri in base ai quali desideri cercare le risorse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordina per]</td> 
   <td> <p>Seleziona la modalità di ordinamento delle risorse. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>Seleziona se ordinare le risorse in ordine crescente o decrescente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Includi eliminato]</td> 
   <td>Abilita questa opzione per includere le risorse eliminate nella ricerca.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Include archived]</p> </td> 
   <td> <p>Abilita questa opzione per includere nella ricerca le risorse archiviate.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Testo del documento di ricerca]</td> 
   <td>Abilita questa opzione per includere il testo del documento nella ricerca oppure false per includere solo le risorse per le quali il titolo corrisponde ai criteri di ricerca.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Immettere o mappare il numero massimo di record che si desidera restituire dal modulo durante ogni ciclo di esecuzione degli scenari.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Offset]</td> 
   <td>Immettere o mappare il numero del primo elemento per il quale si desidera recuperare i dettagli. Questo è un modo per impaginare i record.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scorrimento]</td> 
   <td>Abilita questa opzione per consentire lo scorrimento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Espandi]</td> 
   <td> <p>Oltre ai campi delle risorse, seleziona le proprietà che desideri includere nell’output del modulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Uscite]</td> 
   <td>Selezionare i campi che si desidera includere nell'output del modulo.</td> 
  </tr> 
 </tbody> 
</table>
