---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Creare uno scenario in Adobe Workfront Fusion
description: Le attività seguenti spiegano come creare uno scenario  [!DNL Adobe Workfront Fusion] .
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: ee2283ac159ca26ca473cac28ec4bed85d1dea04
workflow-type: tm+mt
source-wordcount: '1406'
ht-degree: 0%

---

# Crea uno scenario in [!DNL Adobe Workfront Fusion]

Le attività seguenti spiegano come creare uno scenario [!DNL Adobe Workfront Fusion].

Per un esercizio di esercitazione che illustra la creazione di uno scenario di automazione, vedere [Creare uno scenario di automazione di esercitazione in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

Per un esercizio che illustra la creazione di uno scenario di integrazione utilizzando i dati forniti, vedere [Creare uno scenario di integrazione dell&#39;esercitazione in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>Per creare uno scenario da un modello, vedi [Creare scenari con [!DNL Adobe Workfront Fusion] modelli](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>piano Adobe Workfront</td>  
      <td>Qualsiasi</td>  
    </tr>  
    <tr>  
      <td>Licenza Adobe Workfront</td>  
      <td>
        Nuovo: Standard<br>
        Oppure<br>
        Corrente: Lavoro o versione successiva
      </td>  
    </tr>  
    <tr>  
      <td>Licenza Adobe Workfront Fusion</td>  
      <td> 
        Corrente: nessun requisito di licenza Workfront Fusion.<br>
        Oppure<br>
        Legacy: qualsiasi
      </td>  
    </tr>  
    <tr>  
      <td>Prodotto</td>  
      <td> 
        Nuovo: Seleziona o imposta il piano Workfront: la tua organizzazione deve acquistare Adobe Workfront Fusion.<br>
        Ultimate Workfront Plan: Workfront Fusion è incluso.<br>
        Oppure<br>
        Corrente: la tua organizzazione deve acquistare Adobe Workfront Fusion.
      </td>  
    </tr> 
  </tbody>  
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Inizia a creare uno scenario

1. Fai clic su **[!UICONTROL Scenari]** ![](assets/scenarios-icon.png) nel pannello a sinistra.

1. Fai clic su **[!UICONTROL Crea un nuovo scenario]** nell&#39;angolo superiore destro della pagina.
1. Nella schermata visualizzata (editor scenario), se stai creando un nuovo scenario, fai clic su **[!UICONTROL Nuovo scenario]** nell&#39;angolo superiore sinistro e digita un nome per lo scenario.
1. Continua con [Aggiungi un modulo in uno scenario](#add-a-module-in-a-scenario).

## Aggiungere un modulo in uno scenario

1. Per aggiungere il primo modulo allo scenario, fai clic sull’icona del punto interrogativo. ![](assets/question-mark-icon.gif)

   Oppure

   Per aggiungere altri moduli allo scenario, fai clic sulla maniglia a destra del modulo che desideri che segua.

1. Nella casella visualizzata, individua e fai clic sull’app o sul servizio con cui vuoi iniziare.

   Tutte le app selezionate in precedenza vengono visualizzate nella casella per accedervi facilmente e nella sezione **[!UICONTROL Preferiti]** nella parte inferiore dello schermo.

   Se fai clic su **[!UICONTROL Aggiungi un altro modulo]**, i moduli visualizzati dipendono dalla posizione nello scenario in cui stai aggiungendo il modulo. Alcuni moduli possono essere posizionati solo tra altri moduli, altri solo all’inizio dello scenario.

   >[!TIP]
   >
   >I due tipi più comuni di moduli sono le azioni e i trigger. Per ulteriori informazioni, vedere [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

1. Nell’elenco dei moduli visualizzati, fai clic sul primo modulo che desideri aggiungere allo scenario.

   I moduli visualizzati dipendono dalla posizione in cui desideri aggiungere un modulo nello scenario. Alcuni moduli possono essere posizionati solo tra altri moduli, altri solo all’inizio dello scenario.

   I due tipi più comuni di moduli sono le azioni e i trigger. Per ulteriori informazioni, vedere [Tipi di moduli](../../workfront-fusion/modules/module-types.md).

1. Continua su [Connetti l&#39;app o il servizio Web del modulo a [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## Connetti l&#39;app o il servizio Web del modulo a [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

I moduli di Workfront Fusion che si connettono a un&#39;app (ad esempio [!DNL Workfront], [!DNL Salesforce] o [!DNL Jira)] presentano il campo [!UICONTROL Connessione]. Qui puoi specificare la connessione da utilizzare per il modulo per la connessione all’app. Puoi selezionare una connessione esistente dal menu a discesa, oppure crearne una nuova.

Quando selezioni o crei una connessione per un’app in uno scenario, gli altri moduli per tale app utilizzano automaticamente la stessa connessione, a meno che non ne selezioni una diversa durante la configurazione dei moduli successivi.

Per ulteriori informazioni, vedere [Panoramica delle connessioni](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

Per creare una connessione all&#39;interno di un modulo [!DNL Workfront Fusion]:

1. Fai clic su **[!UICONTROL Aggiungi]** per aprire la casella **[!UICONTROL Crea una connessione]**.
1. (Facoltativo) Modificare il nome predefinito della connessione ****.
1. (Condizionale) Se l&#39;app richiede impostazioni di connessione avanzate, ad esempio un ID, una chiave o un [!UICONTROL segreto], immetti tali informazioni.

   Potrebbe essere necessario fare clic su **[!UICONTROL Mostra impostazioni avanzate]** per visualizzare i campi in cui è possibile immettere questo tipo di informazioni.

1. Fai clic su **[!UICONTROL Continua]**.
1. Nella finestra di accesso visualizzata, inserisci le credenziali per accedere all’app, se non lo hai già fatto.
1. (Condizionale) Se viene visualizzato un pulsante **[!UICONTROL Consenti]**, esamina le azioni che il connettore potrà eseguire, quindi fai clic sul pulsante per connettere l&#39;app a [!DNL Workfront Fusion].
1. Continuare a [Configurare il modulo](#configure-the-module).


## Configurare il modulo

1. Nei campi seguenti il campo Connessione, configura le impostazioni per il modulo, quindi fai clic su **[!UICONTROL OK]**.

   ![](assets/conf-settigs-mod-350x547.png)

   Queste impostazioni sono diverse per ogni modulo. Un titolo in grassetto indica un’impostazione obbligatoria.

   >[!TIP]
   >
   >Mentre lavori sullo scenario, puoi fare clic sul modulo per visualizzare questa casella di impostazioni in qualsiasi momento.
   >
   >
   >Se in un modulo viene visualizzato un cerchio nero, la configurazione delle relative impostazioni non è stata completata. Fai clic sul modulo per aprirlo e continuare la configurazione.
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. Se stai aggiungendo il primo modulo nello scenario, seleziona un’opzione per indicare dove desideri che lo scenario venga avviato ogni volta che viene eseguito.

   ![](assets/choose-where-start-350x194.png)

1. Ripeti i passaggi nelle sezioni [Aggiungi un modulo in uno scenario](#add-a-module-in-a-scenario) e [Configura il modulo](#configure-the-module) per aggiungere altri moduli allo scenario.

1. (Facoltativo) Copiare e incollare un modulo o un gruppo di moduli.

   Per ulteriori informazioni, vedere [Copiare moduli o scenari in Adobe Workfront Fusion](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. Continua a [Configurare e utilizzare lo scenario](#configure-and-work-with-your-scenario).

## Configurare e utilizzare lo scenario

1. Per configurare lo scenario, effettua una delle seguenti operazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Specifica quando e con quale frequenza verrà eseguito lo scenario</td> 
      <td> <p>Fai clic sull’icona dell’orologio. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Per ulteriori informazioni, vedere <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Pianificare uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Impostare un ciclo di lavorazione</td> 
      <td> <p>Fare clic sull'icona chiave inglese <img src="assets/wrench-icon.gif"> tra i due moduli e utilizzare una delle opzioni seguenti. Per ulteriori informazioni, vedere <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Aggiungere un filtro a uno scenario in [!DNL Adobe Workfront Fusion]</a>.</p> 
       <ul> 
        <li><strong>[!UICONTROL Configura un filtro]</strong>: controlla quali bundle vengono utilizzati in determinati punti dello scenario.</li> 
        <li><strong>[!UICONTROL Unlink]</strong>: rimuove una route.</li> 
        <li><strong>[!UICONTROL Aggiungi un router]</strong>: aggiunge un router tra i moduli. </li> 
        <li><strong>[!UICONTROL Aggiungi un modulo]</strong>: aggiunge un nuovo modulo tra i moduli.</li> 
        <li><strong>[!UICONTROL Aggiungi una nota]</strong>: aggiunge una nota alla route.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configurare le impostazioni dello scenario</td> 
      <td>Fai clic sull'icona [!UICONTROL Scenario settings] (Impostazioni scenario). <img src="assets/gear-icon-settings.png"> Queste impostazioni sono destinate principalmente agli utenti avanzati. Per ulteriori informazioni, vedere <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Il pannello delle impostazioni dello scenario in [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configurare le impostazioni di Controllo del flusso</td> 
      <td> <p>Fare clic sull'icona [!UICONTROL Flow Control]. <img src="assets/flow-control-icon.gif"> È possibile impostare un'attività per ripetere un determinato numero di volte, convertire un array in una serie di bundle e unire più bundle in un singolo bundle. Per ulteriori informazioni, vedere <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Controllo del flusso in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Migliorare lo scenario utilizzando strumenti avanzati</td> 
      <td>Fare clic sull'icona [!DNL Tools]. <img src="assets/tools-icon.gif"> È possibile creare trigger, azioni, aggregatori e trasformatori. Per ulteriori informazioni, vedere <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Strumenti</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Strumenti di analisi del testo utente</td> 
      <td>Fare clic sull'icona [!DNL Text parser] <img src="assets/text-parser-icon.gif">. Puoi recuperare elementi dal codice HTML, trovare ed estrarre elementi stringa che corrispondono a un pattern di ricerca, cercare e sostituire testo e dati di tipo "scrape" da un sito web. Per ulteriori informazioni, vedere <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Strumenti</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Effettua una delle seguenti operazioni per lavorare con lo scenario:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visualizza un registro degli eventi che si verificano durante l’esecuzione dello scenario</td> 
      <td> <p>Fare clic sulla freccia [!UICONTROL Esci dalla modifica] <img src="assets/exit-editing-arrow.png"> nell'editor scenari per visualizzare la pagina dei dettagli dello scenario. Il registro viene visualizzato nella parte inferiore della finestra o nell'angolo inferiore destro. Contiene informazioni su ciascuna fase e sugli eventuali errori riscontrati durante l’esecuzione dello scenario.</p> <p>Per tornare a utilizzare lo scenario in [!DNL scenario editor], fare clic in un punto qualsiasi della pagina dei dettagli dello scenario.</p> <p>Per ulteriori informazioni sulla pagina dei dettagli dello scenario, vedere <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Dettagli dello scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accedi alle app e ai servizi più comunemente utilizzati</td> 
      <td> Fare clic su un'icona nella sezione <strong>[!UICONTROL Preferiti]</strong> nella parte inferiore dello schermo. Le icone vengono visualizzate automaticamente in questa sezione quando aggiungi app e servizi allo scenario. È inoltre possibile fare clic sull'icona [!UICONTROL Add] <img src="assets/add-icon.gif"> per aggiungere manualmente app e servizi a quest'area.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizzare un’animazione che mostra il modo in cui i dati scorrono nello scenario</td> 
      <td>Fare clic sull'icona [!UICONTROL Explain flow] <img src="assets/explain-flow-airplane-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allineamento automatico del layout dei moduli </td> 
      <td>Fare clic sull'icona [!UICONTROL Allineamento automatico] <img src="assets/auto-align-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Digita o visualizza le note sullo scenario</td> 
      <td>Fare clic sull'icona [!UICONTROL Notes] <img src="assets/notes-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rimuovere un modulo</td> 
      <td>Fare clic con il pulsante destro del mouse sul modulo, quindi scegliere <strong>[!UICONTROL Elimina modulo]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Per eseguire il test dello scenario, fare clic su **[!UICONTROL Esegui una volta]**.

   È importante verificare che lo scenario venga eseguito come previsto prima di attivarlo. Una volta attivato, lo scenario viene eseguito in base alla sua pianificazione. Se tutto non funziona come previsto, vedi [Gestione degli errori in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. Al termine della modifica dello scenario o in qualsiasi momento durante la modifica, fare clic sull&#39;icona [!UICONTROL Salva] nella parte inferiore della finestra ![](assets/save-icon.gif).

Per informazioni sull&#39;attivazione di uno scenario, vedere [Attivare o disattivare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## Scelte rapide da tastiera per lo scenario Workfront Fusion

Durante la creazione o la modifica di uno scenario è possibile utilizzare le seguenti scelte rapide da tastiera:

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
   <td role="rowheader">[!UICONTROL Salva] </td> 
   <td>Ctrl+Maiusc+S</td> 
   <td><span style="font-weight: normal;">Cmd+Maiusc+S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Una Volta]</td> 
   <td>CTRL+MAIUSC+INVIO</td> 
   <td><span style="font-weight: normal;">Cmd+Maiusc+Invio</span> </td> 
  </tr> 
 </tbody> 
</table>
