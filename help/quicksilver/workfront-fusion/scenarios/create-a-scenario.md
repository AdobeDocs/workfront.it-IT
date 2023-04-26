---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Creare uno scenario in Adobe Workfront Fusion
description: Le seguenti attività spiegano come creare un [!DNL Adobe Workfront Fusion] scenario.
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: a3fd1da2f0d144fe9d6444c038ac21baba3cd848
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Crea uno scenario in [!DNL Adobe Workfront Fusion]

Le seguenti attività spiegano come creare un [!DNL Adobe Workfront Fusion] scenario.

Per un esercizio che illustra come creare uno scenario di automazione, consulta [Crea uno scenario di automazione pratica in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

Per un esercizio che illustra come creare uno scenario di integrazione utilizzando i dati forniti, consulta [Creare uno scenario di integrazione pratica in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>Per creare uno scenario da un modello, vedi [Creare scenari con [!DNL Adobe Workfront Fusion] modelli](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro</p><p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro</p>    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Inizia a creare uno scenario

1. Fai clic su **[!UICONTROL Scenari]** ![](assets/scenarios-icon.png) nel pannello a sinistra.

1. Fai clic su **[!UICONTROL Creare un nuovo scenario]** nell’angolo superiore destro della pagina.
1. Nella schermata visualizzata (editor dello scenario), se stai creando un nuovo scenario, fai clic su **[!UICONTROL Nuovo scenario]** nell&#39;angolo in alto a sinistra e digitare un nome per lo scenario.
1. Continua su [Aggiungere un modulo in uno scenario](#add-a-module-in-a-scenario).

## Aggiungere un modulo in uno scenario

1. Per aggiungere il primo modulo allo scenario, fai clic sull’icona del punto interrogativo. ![](assets/question-mark-icon.gif)

   Oppure

   Per aggiungere altri moduli allo scenario, fare clic sull&#39;handle sul lato destro del modulo che si desidera che segua.

1. Nella casella visualizzata, trova e fai clic sull’app o sul servizio con cui vuoi iniziare.

   Tutte le app selezionate in precedenza vengono visualizzate nella casella per un facile accesso e nella **[!UICONTROL Preferiti]** nella parte inferiore dello schermo.

   Se fai clic su **[!UICONTROL Aggiungi un altro modulo]**, i moduli visualizzati dipendono da dove nello scenario in cui si sta aggiungendo il modulo. Alcuni moduli possono essere posizionati solo tra altri moduli e altri solo all’inizio dello scenario.

   >[!TIP]
   >
   >I due tipi più comuni di moduli sono azioni e trigger. Per ulteriori informazioni, consulta [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

1. Nell’elenco dei moduli visualizzati, fare clic sul primo modulo che si desidera aggiungere allo scenario.

   I moduli visualizzati dipendono dal punto in cui desideri aggiungere un modulo nel tuo scenario. Alcuni moduli possono essere posizionati solo tra altri moduli e altri solo all’inizio dello scenario.

   I due tipi più comuni di moduli sono azioni e trigger. Per ulteriori informazioni, consulta [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

1. Continua su [Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

Moduli Workfront Fusion che si connettono a un&#39;app (ad esempio [!DNL Workfront], [!DNL Salesforce]oppure [!DNL Jira)] la funzione [!UICONTROL Connessione] campo . Qui puoi specificare la connessione che desideri utilizzare per la connessione all’app in questo modulo. È possibile selezionare una connessione esistente dal menu a discesa oppure crearne una nuova.

Quando selezioni o crei una connessione per un’app in uno scenario, altri moduli per quell’app utilizzano automaticamente la stessa connessione, a meno che tu non ne selezioni una diversa quando configuri i moduli successivi.

Per ulteriori informazioni, consulta [Informazioni sulla connessione [!DNL Adobe Workfront Fusion] a un&#39;app o a un servizio](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

Creazione di una connessione all&#39;interno di una [!DNL Workfront Fusion] modulo:

1. Fai clic su **[!UICONTROL Aggiungi]** per aprire **[!UICONTROL Creare una connessione]** scatola.
1. (Facoltativo) Modificare il valore predefinito **[!UICONTROL Nome connessione]**.
1. (Condizionale) Se l’app richiede impostazioni di connessione avanzate, ad esempio un ID, una chiave o [!UICONTROL segreto], inserisci tali informazioni.

   Potrebbe essere necessario fare clic su **[!UICONTROL Mostra impostazioni avanzate]** per visualizzare i campi in cui è possibile inserire questo tipo di informazioni.

1. Fai clic su **[!UICONTROL Continua]**.
1. Nella finestra di accesso visualizzata, immetti le tue credenziali per accedere all’app se non lo hai già fatto.
1. (Condizionale) Se un **[!UICONTROL Consenti]** viene visualizzato il pulsante , esamina le azioni che il connettore sarà in grado di eseguire, quindi fai clic sul pulsante per collegare l’app a [!DNL Workfront Fusion].
1. Continua su [Configura il modulo](#configure-the-module).


## Configura il modulo

1. Nei campi sotto il campo Connessione configurare le impostazioni per il modulo, quindi fare clic su **[!UICONTROL OK]**.

   ![](assets/conf-settigs-mod-350x547.png)

   Queste impostazioni sono diverse per ogni modulo. Un titolo in grassetto indica un’impostazione obbligatoria.

   >[!TIP]
   >
   >Mentre lavori sullo scenario, puoi fare clic sul modulo per visualizzare questa casella di impostazioni in qualsiasi momento.
   >
   >
   >Se viene visualizzato un cerchio nero su un modulo, non è stata completata la configurazione delle relative impostazioni. Fai clic sul modulo per aprirlo e continuare la configurazione.
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. Se si aggiunge il primo modulo nello scenario, selezionare un&#39;opzione per indicare la posizione in cui si desidera avviare lo scenario ogni volta che viene eseguito.

   ![](assets/choose-where-start-350x194.png)

1. Ripeti i passaggi nelle sezioni [Aggiungere un modulo in uno scenario](#add-a-module-in-a-scenario) e [Configura il modulo](#configure-the-module) per aggiungere altri moduli allo scenario.

1. (Facoltativo) Copiare e incollare un modulo o un gruppo di moduli.

   Per ulteriori informazioni, consulta [Copiare moduli o scenari in Adobe Workfront Fusion](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. Continua su [Configurare e utilizzare lo scenario](#configure-and-work-with-your-scenario).

## Configurare e utilizzare lo scenario

1. Per configurare lo scenario, effettua una delle seguenti operazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Specificare quando e con quale frequenza verrà eseguito lo scenario</td> 
      <td> <p>Fai clic sull’icona dell’orologio. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Per ulteriori informazioni, consulta <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Pianifica uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Imposta un percorso</td> 
      <td> <p>Fai clic sull’icona a forma di chiave inglese <img src="assets/wrench-icon.gif"> tra i due moduli e utilizzare una delle seguenti opzioni. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Aggiungi un filtro a uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> 
       <ul> 
        <li><strong>[!UICONTROL Impostare un filtro]</strong>: Controlla quali bundle vengono utilizzati in determinati punti dello scenario.</li> 
        <li><strong>[!UICONTROL Scollega]</strong>: Rimuove un percorso.</li> 
        <li><strong>[!UICONTROL Aggiungere un router]</strong>: Aggiunge un router tra i moduli. </li> 
        <li><strong>[!UICONTROL Aggiungi un modulo]</strong>: Aggiunge un nuovo modulo tra i moduli.</li> 
        <li><strong>[!UICONTROL Aggiungi una nota]</strong>: Aggiunge una nota alla route.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configurare le impostazioni dello scenario</td> 
      <td>Fai clic sull'icona [!UICONTROL Scenario settings] . <img src="assets/gear-icon-settings.png"> Queste impostazioni sono destinate principalmente agli utenti avanzati. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Il pannello delle impostazioni dello scenario in [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configurare le impostazioni di Controllo del flusso</td> 
      <td> <p>Fai clic sull’icona [!UICONTROL Flow Control]. <img src="assets/flow-control-icon.gif"> È possibile impostare un'attività per ripetere un determinato numero di volte, convertire un array in una serie di bundle e unire diversi bundle in un unico bundle. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Controllo del flusso in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Migliorare lo scenario utilizzando strumenti avanzati</td> 
      <td>Fai clic sul pulsante [!DNL Tools] icona. <img src="assets/tools-icon.gif"> Puoi creare attivatori, azioni, aggregatori e trasformatori. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Strumenti</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Strumenti di analisi del testo dell’utente</td> 
      <td>Fai clic sul pulsante [!DNL Text parser] icona <img src="assets/text-parser-icon.gif">. È possibile recuperare elementi dal codice HTML, trovare ed estrarre elementi stringa che corrispondono a un pattern di ricerca, cercare e sostituire testo e dati "scraping" da un sito web. Per ulteriori informazioni, consulta <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Strumenti</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Per utilizzare lo scenario, effettua una delle seguenti operazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visualizza un registro degli eventi che si verificano quando lo scenario viene eseguito</td> 
      <td> <p>Fai clic sulla freccia [!UICONTROL Esci dalla modifica] <img src="assets/exit-editing-arrow.png"> nell'editor dello scenario per visualizzare la pagina dei dettagli Scenario. Il registro viene visualizzato nella parte inferiore della finestra o nell’angolo inferiore destro. Contiene informazioni su ogni fase ed eventuali errori riscontrati durante l'esecuzione dello scenario.</p> <p>Per tornare a lavorare con lo scenario in [!DNL scenario editor], fai clic in un punto qualsiasi della pagina dei dettagli Scenario .</p> <p>Per ulteriori informazioni sulla pagina dei dettagli dello scenario, consulta <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Dettagli scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accedere alle app e ai servizi più comunemente utilizzati</td> 
      <td> Fai clic su un’icona nella <strong>[!UICONTROL Preferiti]</strong> nella parte inferiore dello schermo. Le icone vengono visualizzate automaticamente in questa sezione quando aggiungi app e servizi al tuo scenario. Puoi anche fare clic sull’icona [!UICONTROL Aggiungi] <img src="assets/add-icon.gif"> per aggiungere manualmente app e servizi a questa area.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizzare un'animazione che mostra il flusso dei dati nello scenario</td> 
      <td>Fai clic sull’icona [!UICONTROL Explain flow] <img src="assets/explain-flow-airplane-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allineamento automatico del layout dei moduli </td> 
      <td>Fai clic sull’icona [!UICONTROL Auto align] <img src="assets/auto-align-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Digitare o visualizzare note sullo scenario</td> 
      <td>Fai clic sull’icona [!UICONTROL Notes] <img src="assets/notes-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rimuovere un modulo</td> 
      <td>Fai clic con il pulsante destro del mouse sul modulo, quindi fai clic su <strong>[!UICONTROL Elimina modulo]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Per eseguire il test dello scenario, fai clic su **[!UICONTROL Esegui una volta]**.

   È importante verificare che lo scenario venga eseguito come previsto prima di attivarlo. Una volta attivato, lo scenario verrà eseguito in base alla sua pianificazione. Se tutto non viene eseguito come previsto, vedi [Gestione degli errori in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. Al termine della modifica dello scenario (o in qualsiasi momento durante la modifica), fai clic sul pulsante [!UICONTROL Salva] nella parte inferiore della finestra ![](assets/save-icon.gif).

Per informazioni sull&#39;attivazione di uno scenario, vedi [Attiva o disattiva uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## Scelte rapide da tastiera per Workfront Fusion

Quando si crea o si modifica uno scenario, è possibile utilizzare le seguenti scelte rapide da tastiera:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p>Azione</p> </th> 
   <th>[!DNL Windows]</th> 
   <th> <p>[!DNL MacOS]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Save] </td> 
   <td>Ctrl+Maiusc+S</td> 
   <td><span style="font-weight: normal;">Comando+Maiusc+S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Esegui Una Volta]</td> 
   <td>Ctrl+Maiusc+Invio</td> 
   <td><span style="font-weight: normal;">Comando+Maiusc+Invio</span> </td> 
  </tr> 
 </tbody> 
</table>
