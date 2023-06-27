---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Scenari di debug con Adobe Workfront Fusion DevTool
description: Adobe Workfront Fusion DevTool consente di comprendere e risolvere gli scenari. DevTool aggiunge un pannello aggiuntivo a Chrome Developer Tools. Utilizzando questo pannello di debugger, puoi controllare tutte le esecuzioni manuali dello scenario, esaminare tutte le operazioni eseguite e visualizzare i dettagli di ogni chiamata API eseguita. Puoi vedere quale modulo, operazione o singola risposta ha causato l’errore e sfruttare queste informazioni per perfezionare lo scenario.
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1670'
ht-degree: 0%

---

# Scenari di debug con [!DNL Adobe Workfront Fusion] DevTool

Il [!DNL Adobe Workfront Fusion] DevTool consente di comprendere e risolvere gli scenari. DevTool aggiunge un pannello aggiuntivo alla [!DNL Chrome Developer Tools]. Utilizzando questo pannello di debugger, puoi controllare tutte le esecuzioni manuali dello scenario, esaminare tutte le operazioni eseguite e visualizzare i dettagli di ogni chiamata API eseguita. Puoi vedere quale modulo, operazione o singola risposta ha causato l’errore e sfruttare queste informazioni per perfezionare lo scenario.

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!DNL Pro] o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro], [!UICONTROL [!DNL Workfront Fusion] per automazione lavoro]</p>
   </td>    </tr> 
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

## Installare [!DNL Chrome] Estensione DevTool

<!--
To use the [!DNL Workfront Fusion] DevTool, you first need to install it.

1. Click [this link](assets/workfront-fusion-devtool-2023-feb.zip) to download the extension.
1. When the files have downloaded, extract them to a folder of your choice.
1. Open a tab in [!DNL Chrome]
1. In the search bar of the tab, enter `chrome://extensions`.
1. Click the **[!UICONTROL Developer mode]** toggle at the upper-right of the screen to enable Developer mode. If the toggle to the right, developer mode is enabled.
1. Click **[!UICONTROL Load unpacked]**.
1. Select the folder containing the DevTool (where you extracted the files in step 2).

   Once unpacked, the DevTool appears among your other Chrome extensions.
   -->

È possibile aggiungere [!DNL Workfront Fusion] DevTool per [!DNL Chrome] tramite [!UICONTROL [!DNL Chrome] Archivio web].

1. Clic [questo collegamento](https://chrome.google.com/webstore/detail/workfront-fusion-devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn/related) per passare al [!DNL Workfront Fusion] DevTool su [!UICONTROL [!DNL Chrome] Archivio web].
1. Clic **[!UICONTROL Aggiungi a[!DNL Chrome]]**.
1. Nella finestra visualizzata, esaminare le autorizzazioni. Se si accettano le autorizzazioni, fare clic su **[!UICONTROL Aggiungi estensione]**.

Il [!DNL Workfront Fusion] L&#39;estensione DevTool è stata aggiunta al tuo [!DNL Chrome] estensioni.


## Individua il [!DNL Workfront Fusion] DevTool

Per utilizzare [!DNL Workfront Fusion] DevTool, è necessario aggiungere [!DNL Workfront Fusion] Estensione DevTool per [!DNL Chrome] come descritto in [Installare l’estensione Chrome DevTool](#install-the-chrome-devtool-extension).

1. Apri il [!DNL Workfront Fusion] scenario.
1. Aperto [!DNL Chrome Developer Tools]:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Mac]</td> 
      <td>Comando + Opzione + I</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Windows]</td> 
      <td> <p>Ctrl+Maiusc+I</p> <p> Oppure </p> <p>F12</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >È consigliabile ancorare [!DNL Chrome Developer Console] verso il basso per avere una visione migliore dei moduli.

1. Fai clic su **[!DNL Workfront Fusion]** scheda in [!DNL Chrome Dev Tools].

## Utilizza il [!DNL Workfront Fusion] DevTool

Workfront Fusion DevTool è suddiviso in 3 sezioni principali. Potete trovarli nel pannello sinistro della finestra DevTool.

* [Live Stream](#live-stream)
* [Scenario Debugger](#scenario-debugger)
* [Strumenti](#tools)

### Live Stream

Live Stream mostra cosa accade in background quando fai clic su Esegui una volta nello scenario.

1. Fai clic su **[!UICONTROL Live Stream]** icona ![](assets/live-stream-icon.png) per aprire la sezione Live Stream.
1. Effettua una delle seguenti operazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Azione</th> 
      <th>Istruzioni</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visualizza informazioni richiesta</td> 
      <td> <p>Puoi visualizzare le seguenti informazioni per ogni modulo nello scenario</p> 
       <ul> 
        <li> <p>Intestazioni di richiesta (URL dell’endpoint API, metodo http, ora e data in cui è stata chiamata la richiesta, intestazioni di richiesta e stringa di query)</p> </li> 
        <li> <p>Corpo della richiesta</p> </li> 
        <li> <p>Intestazioni di risposta</p> </li> 
        <li> <p>Corpo risposta</p> </li> 
       </ul> <p>Per visualizzare queste informazioni, fai clic sulla scheda appropriata nel pannello a destra della sezione [!DNL Workfront Fusion] DevTool</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Ricercare richieste e risposte</p> </td> 
      <td> <p>Immetti il termine di ricerca nel campo di ricerca nel pannello a sinistra della [!DNL Workfront Fusion] DevTool per visualizzare solo le richieste che contengono il termine di ricerca.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Rimuovi elenco di richieste </p> </td> 
      <td> <p>Fai clic sull’icona cestino nell’angolo in alto a destra del pannello a sinistra di DevTool per cancellare l’elenco delle richieste registrate da [!DNL Workfront Fusion] DevTool </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Abilita registrazione console</p> </td> 
      <td> <p>Fare clic sull'icona del computer <img src="assets/console-computer-icon.png"> nell'angolo superiore destro del pannello sinistro di DevTool.</p> <p>La registrazione nella console è abilitata quando l’icona del computer è verde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Recuperare la richiesta nel formato Raw JSON o in cURL</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>JSON raw</strong> </p> <p>Clic <strong>[!UICONTROL Copia RAW]</strong> nell'angolo superiore destro del riquadro destro di DevTool.</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>Clic <strong>[!UICONTROL Copy cURL]</strong> nell'angolo superiore destro del riquadro destro di DevTool.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Scenario Debugger

Scenario Debugger è utile per scenari più complessi. Visualizza la cronologia dello scenario eseguito e consente di cercare i moduli in base al nome o all’ID.

1. Fai clic su **[!UICONTROL Scenario Debugger]** icona ![](assets/scenario-debugger-icon.png) per aprire Scenario Debugger.
1. (Facoltativo) Immetti il termine di ricerca (nome o ID modulo) nel campo di ricerca nel riquadro a sinistra di [!DNL Workfront Fusion] DevTool in [!UICONTROL Scenario Debugger] sezione.
1. Fai doppio clic sul nome del modulo per aprirne le impostazioni nell’editor scenario.
1. Per visualizzare i dettagli della richiesta, fai clic sull’operazione desiderata.

### Strumenti

Il [!DNL Workfront Fusion] DevTool offre strumenti che semplificano la configurazione dello scenario.

1. Fai clic su **[!UICONTROL Strumenti]** icona ![](assets/console-tools-icon.png) per aprire Strumenti.
1. Selezionare lo strumento che si desidera utilizzare
1. Configura i campi come descritto di seguito.
1. Clic **[!UICONTROL Esegui]**.

Strumenti e relativi campi:

* [Mettere a fuoco un modulo](#focus-a-module)
* [Trova moduli per mappatura](#find-modules-by-mapping)
* [Ottieni metadati app](#get-app-metadata)
* [Copia mappatura](#copy-mapping)
* [Copia Filtro](#copy-filter)
* [Scambia connessione](#swap-connection)
* [Scambia variabile](#swap-variable)
* [Scambia app](#swap-app)
* [Base 64](#base-64)
* [Copia nome modulo](#copy-module-name)
* [Rimappatura origine](#remap-source)
* [Evidenzia app](#highlight-app)
* [Migra GS](#migrate-gs)

#### [!UICONTROL Mettere a fuoco un modulo]

Apre le impostazioni del modulo specificato in base all&#39;ID.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Module ID]</td>
        <td>Immettere l'ID del modulo per il quale si desidera aprire le impostazioni.</td>
    </tr>
</table>

#### [!UICONTROL Trova moduli per mappatura]

Consente di cercare i valori dei moduli per un termine specificato. L’output contiene ID di moduli che contengono il termine cercato.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Parola chiave [!UICONTROL]</td> 
   <td> <p> Immettere il termine che si desidera cercare. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Usa solo valori]</p> </td> 
   <td> <p>Abilita questa opzione per eseguire ricerche solo nei valori dei campi modulo.</p> <p>Disattiva questa opzione per eseguire ricerche anche nei nomi dei campi modulo.</p> <p>La ricerca viene eseguita tramite i parametri name ed label.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni metadati app]

Recupera i metadati dell’app in base al nome o all’ID del modulo dell’app. Questa funzione è utile, ad esempio, quando devi conoscere la versione dell’app utilizzata nel tuo scenario.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Seleziona il modulo per il quale desideri recuperare i metadati.</td>
    </tr>
</table>

#### [!UICONTROL Copia mappatura]

Copia i valori dal modulo di origine al modulo di destinazione.

>[!CAUTION]
>
>Assicurati di impostare i moduli di origine e di destinazione corretti. Se selezioni un tipo diverso di modulo, i valori nel modulo di destinazione verranno eliminati.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Seleziona il modulo o immetti l’ID del modulo da cui desideri copiare i valori dei campi.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Modulo Di Destinazione]</p> </td> 
   <td> <p>Seleziona il modulo o immetti l’ID del modulo in cui desideri inserire i valori del modulo sorgente.</p> <p>Importante: i valori nel modulo di destinazione verranno sovrascritti.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copia Filtro]

Copia le impostazioni del filtro dal modulo di origine al modulo di destinazione.

>[!NOTE]
>
>L&#39;azione di copia viene eseguita sul filtro posizionato sul lato sinistro del modulo selezionato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Seleziona il modulo o immetti l’ID del modulo da cui desideri copiare i valori del filtro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Modulo Di Destinazione]</p> </td> 
   <td> <p>Seleziona il modulo o immetti l’ID del modulo in cui desideri inserire i valori del filtro dal modulo sorgente.</p> <p>Importante: i valori nel modulo di destinazione verranno sovrascritti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Mantieni route di fallback]</p> </td> 
   <td> <p>Il filtro di origine viene impostato come route di fallback. Abilita questa opzione per impostare anche il filtro di destinazione impostato come route di fallback.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scambia connessione]

Duplica una connessione dal modulo di origine a ogni modulo nello scenario della stessa app.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Seleziona il modulo o immetti l’ID del modulo da cui desideri duplicare la connessione.</td>
    </tr>
</table>

#### [!UICONTROL Scambia variabile]

Cerca le variabili specificate nello scenario e le sostituisce con una nuova variabile.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variabile da trovare]</td> 
   <td> <p> Individua la pillola di variabile che desideri sostituire dal modulo nello scenario e copiala in questo campo ([!UICONTROL Variabile da trovare]). Nel campo, viene visualizzato con parentesi graffe doppie. Esempio: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sostituisci Con]</p> </td> 
   <td> <p>Individua la pillola di variabile con cui desideri sostituire la variabile dal modulo nello scenario e copiala in questo campo ([!UICONTROL Variabile da trovare]). Nel campo, viene visualizzato con parentesi graffe doppie. Esempio: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module]</p> </td> 
   <td> <p>Seleziona il modulo in cui desideri sostituire la variabile. Se non è selezionato alcun modulo, la variabile verrà sostituita nell’intero scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scambia app]

Sostituisce la versione dell’app selezionata nello scenario con un’altra versione dell’app.

Può essere utilizzato, ad esempio, per aggiornare i moduli delle app Gmail ed E-mail alla versione più recente.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL App da sostituire]</td> 
   <td> <p> Seleziona l’app da sostituire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sostituisci con]</p> </td> 
   <td> <p>Seleziona l’app con cui desideri sostituirla.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Base 64]

Consente di codificare i dati immessi in Base64 o di decodificare Base64. Alcune richieste sono codificate in Base64. Questo strumento può essere utile quando desideri cercare dati particolari nella richiesta codificata.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operation] </td> 
   <td> <p>Specificare se si desidera codificare i dati dal campo [!UICONTROL Raw Data] in Base64 o decodificare Base64 in Dati non elaborati.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dati Non Elaborati]</p> </td> 
   <td> <p> Immettere i dati che si desidera codificare in Base64 o Base64 se si desidera decodificare in dati non elaborati, a seconda dell'opzione selezionata nel campo Operazione [!UICONTROL] precedente.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copia nome modulo]

Copia negli Appunti il nome del modulo selezionato.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Module] </td> 
   <td> <p>Seleziona il modulo di cui desideri copiare il nome.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rimappatura origine]

Consente di cambiare l&#39;origine di mappatura da un modulo all&#39;altro.

È innanzitutto necessario aggiungere il modulo che si desidera utilizzare come modulo di origine al ciclo di lavorazione nello scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module] </td> 
   <td> <p> Seleziona il modulo da sostituire come origine di mappatura per altri moduli nello scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Modulo Di Destinazione]</p> </td> 
   <td> <p>Selezionare il modulo da utilizzare come nuova origine di mappatura.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Modulo [!UICONTROL da modificare]</p> </td> 
   <td> <p>Selezionare il modulo per il quale si desidera modificare il mapping se non si desidera modificare il mapping nell'intero scenario. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Evidenzia app]

Evidenzia i moduli dell’app specificata nel tuo scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL App da evidenziare] </td> 
   <td> <p> Seleziona l’app da evidenziare nello scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL versione] </p> </td> 
   <td> <p>Seleziona la versione dell’app che desideri evidenziare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Colore evidenziazione]</p> </td> 
   <td> <p> Immettere l'esadecimale del colore da utilizzare per evidenziare i moduli.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Migra GS]

Questo strumento è stato creato appositamente per l&#39;aggiornamento [!DNL Google Sheets] (legacy) ai più recenti [!DNL Google Sheets] versione. Aggiunge una nuova versione del modulo subito dopo la versione legacy del modulo nel percorso dello scenario.

Questo modulo non richiede l’impostazione di alcun parametro.
