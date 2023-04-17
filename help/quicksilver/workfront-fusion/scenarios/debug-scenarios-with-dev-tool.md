---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Scenari di debug con Adobe Workfront Fusion DevTool
description: Adobe Workfront Fusion DevTool consente di comprendere e risolvere gli scenari. DevTool aggiunge un pannello aggiuntivo agli strumenti per sviluppatori di Chrome. Utilizzando questo pannello di debug, puoi controllare tutte le esecuzioni manuali dello scenario, esaminare tutte le operazioni eseguite e visualizzare i dettagli di ogni chiamata API eseguita. Puoi vedere quale modulo, operazione o singola risposta ha causato l’errore e utilizzare tale conoscenza per perfezionare lo scenario.
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: c7946e975c82f54c1a20e716f73d0cf8053ee1a6
workflow-type: tm+mt
source-wordcount: '1622'
ht-degree: 0%

---

# Eseguire il debug degli scenari con [!DNL Adobe Workfront Fusion] DevTool

La [!DNL Adobe Workfront Fusion] DevTool consente di comprendere e risolvere gli scenari. DevTool aggiunge un pannello aggiuntivo al [!DNL Chrome Developer Tools]. Utilizzando questo pannello di debug, puoi controllare tutte le esecuzioni manuali dello scenario, esaminare tutte le operazioni eseguite e visualizzare i dettagli di ogni chiamata API eseguita. Puoi vedere quale modulo, operazione o singola risposta ha causato l’errore e utilizzare tale conoscenza per perfezionare lo scenario.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Installa il [!DNL Chrome] Estensione DevTool

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

Puoi aggiungere la [!DNL Workfront Fusion] DevTool a [!DNL Chrome] attraverso [!UICONTROL [!DNL Chrome] Archivio Web].

1. Fai clic su [questo link](https://chrome.google.com/webstore/detail/workfront-fusion-devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn/related) per passare al [!DNL Workfront Fusion] DevTool nel [!UICONTROL [!DNL Chrome] Archivio Web].
1. Fai clic su [!UICONTROL Aggiungi a [!DNL Chrome]].
1. Nella finestra visualizzata, esamina le autorizzazioni. Se si è d&#39;accordo con le autorizzazioni, fare clic su [!UICONTROL Aggiungi estensione].

La [!DNL Workfront Fusion] L’estensione DevTool viene aggiunta al tuo [!DNL Chrome] estensioni.


## Individua il [!DNL Workfront Fusion] DevTool

Per utilizzare [!DNL Workfront Fusion] DevTool, devi aggiungere il [!DNL Workfront Fusion] Estensione DevTool al tuo [!DNL Chrome] , come descritto in [Installare l’estensione Chrome DevTool](#install-the-chrome-devtool-extension).

1. Apri il tuo [!DNL Workfront Fusion] scenario.
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
   >Si consiglia di ancorare [!DNL Chrome Developer Console] in basso per mantenere una visione migliore dei moduli.

1. Fai clic sul pulsante **[!DNL Workfront Fusion]** scheda in [!DNL Chrome Dev Tools].

## Utilizza la [!DNL Workfront Fusion] DevTool

Workfront Fusion DevTool è diviso in 3 sezioni principali. Puoi trovarli nel pannello a sinistra della finestra DevTool.

* [Flusso live](#live-stream)
* [Debugger scenario](#scenario-debugger)
* [Strumenti](#tools)

### Flusso live

Streaming live mostra cosa succede in background quando fai clic su Esegui una volta nello scenario.

1. Fai clic sul pulsante **[!UICONTROL Flusso live]** icona ![](assets/live-stream-icon.png) per aprire la sezione Streaming live .
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
      <td role="rowheader">Visualizza informazioni richieste</td> 
      <td> <p>È possibile visualizzare le seguenti informazioni per ogni modulo nel proprio scenario</p> 
       <ul> 
        <li> <p>Intestazioni di richiesta (URL dell’endpoint API, metodo http, ora e data in cui è stata chiamata la richiesta, intestazioni di richiesta e stringa di query)</p> </li> 
        <li> <p>Corpo della richiesta</p> </li> 
        <li> <p>Intestazioni di risposta</p> </li> 
        <li> <p>Corpo di risposta</p> </li> 
       </ul> <p>Per visualizzare queste informazioni, fai clic sulla scheda appropriata nel pannello di destra del [!DNL Workfront Fusion] DevTool.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Richieste e risposte di ricerca</p> </td> 
      <td> <p>Inserisci il termine di ricerca nel campo di ricerca nel pannello a sinistra del [!DNL Workfront Fusion] DevTool per visualizzare solo le richieste che contengono il termine di ricerca.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Rimuovi elenco di richieste </p> </td> 
      <td> <p>Fai clic sull’icona del cestino nell’angolo in alto a destra del pannello di sinistra di DevTool per cancellare l’elenco delle richieste registrate dal [!DNL Workfront Fusion] DevTool. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Abilita registrazione console</p> </td> 
      <td> <p>Fai clic sull’icona del computer <img src="assets/console-computer-icon.png"> nell'angolo in alto a destra del pannello sinistro di DevTool.</p> <p>L'accesso alla console è abilitato quando l'icona del computer è verde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Recupera la richiesta in formato JSON non elaborato o cURL</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>JSON grezzo</strong> </p> <p>Fai clic su <strong>[!UICONTROL Copia RAW]</strong> nell'angolo superiore destro del riquadro destro di DevTool.</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>Fai clic su <strong>[!UICONTROL Copia cURL]</strong> nell'angolo superiore destro del riquadro destro di DevTool.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Debugger scenario

Il debugger di scenario è utile per scenari più complessi. Mostra la cronologia dello scenario eseguito e consente di cercare i moduli in base al nome o all’ID.

1. Fai clic sul pulsante **[!UICONTROL Debugger scenario]** icona ![](assets/scenario-debugger-icon.png) per aprire il debugger dello scenario.
1. (Facoltativo) Immetti il termine di ricerca (nome o ID modulo) nel campo di ricerca nel riquadro a sinistra di [!DNL Workfront Fusion] DevTool nel [!UICONTROL Debugger scenario] sezione .
1. Fai doppio clic sul nome del modulo per aprire le relative impostazioni nell’editor di scenari.
1. Visualizza i dettagli della richiesta facendo clic sull&#39;operazione desiderata.

### Strumenti

La [!DNL Workfront Fusion] DevTool dispone di strumenti che semplificano la configurazione dello scenario.

1. Fai clic sul pulsante **[!UICONTROL Strumenti]** icona ![](assets/console-tools-icon.png) per aprire Strumenti.
1. Seleziona lo strumento da utilizzare
1. Configura i campi come descritto di seguito.
1. Fai clic su **[!UICONTROL Esegui]**.

Strumenti e relativi campi:

* [Attiva un modulo](#focus-a-module)
* [Trova moduli tramite mappatura](#find-modules-by-mapping)
* [Ottieni metadati app](#get-app-metadata)
* [Mappatura copia](#copy-mapping)
* [Copia Filtro](#copy-filter)
* [Scambia connessione](#swap-connection)
* [Variabile Swap](#swap-variable)
* [Scambia app](#swap-app)
* [Base 64](#base-64)
* [Nome modulo copia](#copy-module-name)
* [Origine Remoto](#remap-source)
* [Evidenzia app](#highlight-app)
* [Migra GS](#migrate-gs)

#### [!UICONTROL Attiva un modulo]

Apre le impostazioni del modulo specificato per ID.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Module ID]</td>
        <td>Immetti l’ID del modulo per il quale vuoi aprire le impostazioni.</td>
    </tr>
</table>

#### [!UICONTROL Trova moduli tramite mappatura]

Consente di cercare i valori dei moduli per un termine specificato. L’output contiene gli ID dei moduli che contengono il termine ricercato.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parola chiave]</td> 
   <td> <p> Inserisci il termine da cercare. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Usa solo valori]</p> </td> 
   <td> <p>Abilitare questa opzione per cercare solo i valori dei campi del modulo.</p> <p>Disattiva questa opzione per cercare anche i nomi dei campi del modulo.</p> <p>La ricerca viene eseguita tramite i parametri del nome e dell’etichetta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ottieni metadati app]

Recupera i metadati dell’app in base al nome o all’ID del modulo dell’app. Questa funzione è utile, ad esempio, quando devi conoscere la versione dell’app utilizzata nel tuo scenario.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Selezionare il modulo per il quale si desidera recuperare i metadati.</td>
    </tr>
</table>

#### [!UICONTROL Mappatura copia]

Copia i valori dal modulo di origine al modulo di destinazione.

>[!CAUTION]
>
>Assicurati di impostare i moduli sorgente e target corretti. Se selezioni un tipo diverso di modulo, i valori nel modulo di destinazione verranno eliminati.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Seleziona il modulo o immetti l’ID del modulo da cui vuoi copiare i valori dei campi.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Selezionare il modulo o immettere l'ID del modulo in cui si desidera inserire i valori del modulo di origine.</p> <p>Importante: I valori nel modulo di destinazione verranno sovrascritti.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copia Filtro]

Copia le impostazioni del filtro dal modulo di origine al modulo di destinazione.

>[!NOTE]
>
>L’azione di copia viene eseguita sul filtro posizionato sul lato sinistro del modulo selezionato.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Seleziona il modulo o immetti l’ID del modulo da cui vuoi copiare i valori del filtro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Selezionare il modulo o immettere l'ID del modulo in cui si desidera inserire i valori del filtro dal modulo di origine.</p> <p>Importante: I valori nel modulo di destinazione verranno sovrascritti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Mantieni impostazione route di fallback]</p> </td> 
   <td> <p>Il filtro sorgente viene impostato come percorso di fallback. Abilita questa opzione anche per impostare il filtro di destinazione come percorso di fallback.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scambia connessione]

Duplica una connessione dal modulo di origine a ogni modulo nello scenario della stessa app.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Seleziona il modulo o immetti l’ID del modulo da cui vuoi duplicare la connessione.</td>
    </tr>
</table>

#### [!UICONTROL Variabile Swap]

Cerca le variabili specificate nello scenario e le sostituisce con una nuova variabile.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variabile da trovare]</td> 
   <td> <p> Individua la pillola variabile che desideri sostituire dal modulo nello scenario e copiala in questo campo ([!UICONTROL Variabile in Trova]). Nel campo viene visualizzato con parentesi graffe doppie. Esempio: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sostituisci con]</p> </td> 
   <td> <p>Individua la pillola variabile con cui desideri sostituire la variabile dal modulo nel tuo scenario e copiala in questo campo ([!UICONTROL Variable to Find]). Nel campo viene visualizzato con parentesi graffe doppie. Esempio: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module]</p> </td> 
   <td> <p>Selezionare il modulo in cui si desidera sostituire la variabile. Se non è selezionato alcun modulo, la variabile verrà sostituita nell’intero scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Scambia app]

Sostituisce la versione dell&#39;app selezionata nello scenario con un&#39;altra versione dell&#39;app.

Questo può essere utilizzato, ad esempio, per aggiornare i moduli delle app Gmail e Email alla versione più recente.

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
   <td> <p>Seleziona l’app con cui sostituirla.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Base 64]

Consente di codificare i dati immessi in Base64 o di decodificare Base64. Alcune richieste sono codificate in Base64. Questo strumento può essere utile quando desideri cercare particolari dati nella richiesta codificata.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operation] </td> 
   <td> <p>Seleziona se codificare i dati dal campo [!UICONTROL Raw Data] a Base64 o decodificare Base64 in Raw Data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Raw Data]</p> </td> 
   <td> <p> Immettere i dati che si desidera codificare in Base64 o Base64 se si desidera decodificare in dati non elaborati, a seconda dell'opzione selezionata nel campo [!UICONTROL Operation] qui sopra.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Nome modulo copia]

Copia negli Appunti il nome del modulo selezionato.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Module] </td> 
   <td> <p>Selezionare il modulo di cui si desidera copiare il nome.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Origine Remoto]

Consente di modificare l&#39;origine di mappatura da un modulo a un altro.

È innanzitutto necessario aggiungere il modulo che si desidera utilizzare come modulo di origine alla route nello scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module] </td> 
   <td> <p> Seleziona il modulo da sostituire come origine di mappatura per altri moduli nello scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Selezionare il modulo che si desidera utilizzare come nuova origine di mappatura.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Modulo da modificare]</p> </td> 
   <td> <p>Seleziona il modulo per il quale desideri modificare la mappatura se non desideri modificare la mappatura nell’intero scenario. </p> </td> 
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
   <td role="rowheader">App [!UICONTROL da evidenziare] </td> 
   <td> <p> Seleziona l’app da evidenziare nello scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Versione] </p> </td> 
   <td> <p>Seleziona la versione dell’app da evidenziare.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Colore evidenziatore]</p> </td> 
   <td> <p> Immettere l'esadecimale a colori che si desidera utilizzare per evidenziare i moduli.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Migra GS]

Questo strumento è stato creato specialmente per l&#39;aggiornamento [!DNL Google Sheets] (legacy) moduli all’ultima versione [!DNL Google Sheets] versione. Aggiunge una nuova versione del modulo subito dopo la versione precedente del modulo nel percorso dello scenario.

Questo modulo non richiede l&#39;impostazione di parametri.
