---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-adobe-creative-cloud
title: Utilizzare l’estensione Workfront per Illustrator e InDesign
description: Puoi utilizzare l’estensione Workfront per esportare in Workfront i contenuti digitali salvati e creati in Adobe Illustrator e Adobe InDesign. In questo modo si velocizza il processo di revisione e approvazione dei documenti.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 40945eac-e8de-42af-b6ba-f3082c208e02
source-git-commit: 147a5b5d508e1ea01d18d981f9157439a643cf55
workflow-type: tm+mt
source-wordcount: '3056'
ht-degree: 0%

---

# Utilizzare l’estensione Workfront per Illustrator e InDesign

>[!IMPORTANT]
>
>Stiamo sostituendo l’estensione Workfront per Illustrator e InDesign con [plug-in di Creative Cloud aggiornati](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md). A partire dalla fine del 2022, questa estensione non sarà più supportata ed è disponibile così come è.


Puoi utilizzare l’estensione Workfront per esportare in Workfront i contenuti digitali salvati e creati in Adobe Illustrator e Adobe InDesign. In questo modo si velocizza il processo di revisione e approvazione dei documenti.

L’estensione Workfront è supportata per Adobe Creative Cloud 2017 e versioni successive nelle seguenti applicazioni:

* InDesign
* Illustrator
* Photoshop

   >[!NOTE]
   >
   >Si consiglia di utilizzare il nuovo [Adobe Workfront per Photoshop](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md) plugin.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>È necessario disporre di una licenza Adobe Creative Cloud oltre a una licenza Workfront.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Modificare l’accesso all’oggetto con cui si desidera interagire.</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Accedi all’estensione Workfront da Illustrator o InDesign {#log-in-to-workfront-extension-from-illustrator-or-indesign}

Quando effettui l’accesso a Workfront da una delle applicazioni Adobe supportate, accedi a tutte le applicazioni Adobe supportate.

1. Vai all&#39;applicazione Adobe in cui desideri utilizzare l&#39;estensione Workfront.

   Per un elenco dei formati supportati per ciascuna applicazione supportata, vedere [Formati di file esportati supportati](#supported-exported-file-formats) in questo articolo.

1. Fai clic su **Finestra** > **Estensioni** > Workfront.

1. (Facoltativo) Trascina il pannello Workfront nella posizione in cui lo desideri visualizzare nell’applicazione Adobe.
1. Segui le istruzioni per accedere a Workfront.

   >[!NOTE]
   >
   >* Workfront si connette a Adobe Creative Cloud utilizzando OAuth 2.0, uno standard sicuro utilizzato dalla maggior parte delle integrazioni basate su web per l’autenticazione e l’autorizzazione degli utenti.
   >* Quando viene richiesto di immettere il [dominio o host] del tuo account Workfront, digita questo formato: *la tua azienda&#39;sDomain.my.workfront.com*. Il dominio della tua azienda è in genere il nome della tua azienda.


   Viene visualizzato un elenco di elementi di lavoro assegnati se il progetto è in uno stato corrente. Se un elenco non viene visualizzato, accedi a Workfront.

   I compiti personali sono elencati in **Nessun progetto**.

## Caricare un file in un progetto, un&#39;attività o un problema Workfront {#upload-a-file-to-a-workfront-project-task-or-issue}

È possibile caricare un file dal file system del computer o esportare un file attualmente aperto in un&#39;applicazione Adobe Creative Cloud in un progetto, un&#39;attività o un problema Workfront. 

Quando carichi o esporti un file da Adobe Creative Cloud, considera quanto segue:

* Il livello di accesso deve consentire il caricamento di documenti in Workfront. Per ulteriori informazioni, consulta [Concedere l’accesso ai documenti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).
* È necessario disporre delle autorizzazioni per caricare i documenti nell&#39;elemento in cui lo si desidera. Per ulteriori informazioni, consulta [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* Il file viene caricato nell&#39;area Documenti dell&#39;oggetto Workfront selezionato.
* Impossibile esportare un documento nell&#39;area Documenti del menu principale ![](assets/main-menu-icon.png) da un&#39;applicazione Adobe Creative Cloud.

Questa sezione spiega quanto segue:

* [Caricare un file](#upload-a-file)
* [Esporta un file attualmente aperto in Illustrator o InDesign](#export-a-file-currently-open-in-illustrator-or-indesign)
* [Caricare una nuova versione di un file da Illustrator o InDesign](#upload-a-new-version-of-a-file-from-illustrator-or-indesign)

### Caricare un file {#upload-a-file}

Puoi caricare i file in un progetto, un&#39;attività o un problema senza uscire dall&#39;applicazione Adobe Creative Cloud.

1. Se non trovi l&#39;estensione Workfront quando apri l&#39;applicazione Adobe Creative Cloud, fai clic su **Finestra** > **Estensioni** > Workfront.

   Viene visualizzato un elenco di elementi di lavoro assegnati se il progetto è in uno stato corrente. Se un elenco non viene visualizzato, accedi a Workfront.

   I compiti personali sono elencati in **Nessun progetto**.

1. Fai clic sul nome del progetto, dell’attività o del problema a cui desideri caricare il file.

   Per cercare il problema, digita il nome nel **Ricerca** casella e selezione **Progetto**, **Attività** oppure **Problema** dal menu a discesa a destra del **Ricerca** scatola. Se il nome dell&#39;elemento di lavoro non viene visualizzato nell&#39;elenco, premere **Invio** per cercare tutti gli elementi Workfront a cui hai accesso per la visualizzazione.

1. Fai clic su **Seleziona** nell&#39;angolo in basso a destra dell&#39;estensione Workfront.
1. In **Fare clic per selezionare il formato** scegliere il formato in cui salvare il file in Workfront dal menu a discesa.

   Per un elenco dei formati supportati per ciascuna applicazione supportata, vedere [Formati di file esportati supportati](#supported-exported-file-formats) in questo articolo.

1. (Condizionale) Se l&#39;elemento di lavoro in cui si desidera caricare il file include cartelle di documenti, selezionare una cartella di documenti nella cartella **Fare clic per selezionare una cartella di documento** campo , quindi fai clic su **Seleziona**.

1. Fai clic su **Caricare un file locale**.
1. In **Apri file** trovare il file nel file system, quindi fare clic su **Apri**.

1. (Facoltativo) Digitare un nuovo nome per il file. 

   ![](assets/rename-file-uploading.png)

1. Fai clic su **Carica**.

   In Workfront, il documento è ora elencato nell&#39;area Documenti per il progetto, l&#39;attività o il problema specificato.  

1. (Facoltativo) Fare clic sul nome del documento per aprire la relativa pagina Dettagli documento in Workfront.

   Workfront si apre in una nuova scheda del browser.

### Esporta un file attualmente aperto in Illustrator o InDesign {#export-a-file-currently-open-in-illustrator-or-indesign}

1. In un’applicazione Adobe Creative Cloud supportata, apri un file da esportare in Workfront. 
1. Se l&#39;estensione Workfront non è visualizzata, fai clic su **Finestra** > **Estensioni** > Workfront.

   Viene visualizzato un elenco di elementi di lavoro assegnati se il progetto è in uno stato corrente. Se un elenco non viene visualizzato, accedi a Workfront.

   I compiti personali sono elencati in **Nessun progetto**.

1. Fare clic sul nome del progetto, dell&#39;attività o del problema a cui si desidera esportare il file.

   Per cercare il problema, digita il nome nel **Ricerca** casella e selezione **Progetto**, **Attività** oppure **Problema** dal menu a discesa a destra del **Ricerca** scatola. Se il nome dell&#39;elemento di lavoro non viene visualizzato nell&#39;elenco, premere **Invio** per cercare tutti gli elementi Workfront a cui hai accesso per la visualizzazione.

1. In **Fare clic per selezionare il formato** scegliere il formato in cui salvare il file in Workfront dal menu a discesa.

   Per un elenco dei formati supportati per ciascuna applicazione supportata, vedere [Formati di file esportati supportati](#supported-exported-file-formats) in questo articolo.

1. (Condizionale) Se l&#39;elemento di lavoro in cui si desidera caricare il file include cartelle di documenti, selezionare una cartella di documenti nella cartella **Fare clic per selezionare una cartella di documento** campo , quindi fai clic su **Seleziona**.
1. (Facoltativo) Per rinominare il documento, fare clic sul nome del documento e digitare un nuovo nome.

   ![](assets/rename-doc-exporting.png)

1. Fai clic su **Esporta**. 

   Viene visualizzato un messaggio per confermare che il documento è stato esportato correttamente in Workfront.

   In Workfront, il documento è elencato nell&#39;area Documenti dell&#39;oggetto specificato in Workfront.

1. (Facoltativo) Fai clic sul nome del documento per accedervi in Workfront.

   ![adobe_document_with_name_highlight.PNG](assets/adobe-document-with-name-highlight-350x251.png)

   Workfront si apre in una nuova scheda del browser.

### Caricare una nuova versione di un file da Illustrator o InDesign {#upload-a-new-version-of-a-file-from-illustrator-or-indesign}

1. Se desideri esportare un file su cui stai lavorando in un’applicazione Adobe supportata come nuova versione di un file in Workfront, apri il file nell’applicazione Adobe. 
1. Se l&#39;estensione Workfront non è visualizzata, fai clic su **Finestra** > **Estensioni** > Workfront.

   Viene visualizzato un elenco di elementi di lavoro assegnati se il progetto è in uno stato corrente. Se un elenco non viene visualizzato, accedi a Workfront.

   I compiti personali sono elencati in **Nessun progetto**.

1. Fare clic sul nome del progetto, dell&#39;attività o del problema in cui è elencato il documento esistente.

   Per cercare il problema, digita il nome nel **Ricerca** casella e selezione **Progetto**, **Attività** oppure **Problema** dal menu a discesa a destra del **Ricerca** scatola. Se il nome dell&#39;elemento di lavoro non viene visualizzato nell&#39;elenco, premere **Invio** per cercare tutti gli elementi Workfront a cui hai accesso per la visualizzazione.

   Tutti i documenti caricati in progetti, attività o problemi vengono visualizzati in un elenco, indipendentemente dal fatto che siano stati caricati dall&#39;applicazione Adobe.

1.  
1. In **Fare clic per selezionare il formato** scegliere il formato in cui salvare il file in Workfront dal menu a discesa.

   Questo è necessario se si esporta un file aperto nell&#39;applicazione Adobe. Per un elenco dei formati supportati per ciascuna applicazione supportata, vedere [Formati di file esportati supportati](#supported-exported-file-formats) in questo articolo.

1. Se si esporta un file aperto nell&#39;applicazione Adobe come nuova versione del documento Workfront selezionato, fare clic su **Esporta**.

   Oppure

   Se si desidera caricare un file dal file system del computer come nuova versione del documento Workfront selezionato, fare clic su **Caricare un file locale**, trova il file nella casella visualizzata, fai clic su **Apri**, quindi fai clic su **Carica**.

1. (Facoltativo) Fai clic sul nome del documento per visualizzarne la nuova versione in Workfront. 

   >[!NOTE]
   >
   >Il nome del documento in Workfront viene compilato per impostazione predefinita e non può essere modificato. Né viene modificato nel nome del file caricato o esportato come nuova versione.
   >
   >
   >![](assets/doc-name-cant-be-changed.png)

## Commento su un documento Workfront da Illustrator o InDesign {#comment-on-a-workfront-document-from-illustrator-or-indesign}

È possibile aggiungere commenti direttamente a un documento Workfront all&#39;interno di un&#39;applicazione Adobe. In Workfront, i commenti vengono visualizzati nell&#39;area Aggiornamenti del documento e nell&#39;area Aggiornamenti per l&#39;elemento Workfront in cui viene salvato il documento. 

1. Apri una delle applicazioni di Adobe supportate.
1. Se l&#39;estensione Workfront non è visualizzata, fai clic su **Finestra** > **Estensioni** > Workfront.

   Viene visualizzato un elenco di elementi di lavoro assegnati se il progetto è in uno stato corrente. Se un elenco non viene visualizzato, accedi a Workfront.

   I compiti personali sono elencati in **Nessun progetto**.

1. Fare clic sul progetto, sull&#39;attività o sul problema in cui è elencato il documento esistente.

   Per cercare il problema, digita il nome nel **Ricerca** casella e selezione **Progetto**, **Attività** oppure **Problema** dal menu a discesa a destra del **Ricerca** scatola. Se il nome dell&#39;elemento di lavoro non viene visualizzato nell&#39;elenco, premere **Invio** per cercare tutti gli elementi Workfront a cui hai accesso per la visualizzazione.

1. Fare clic sul nome del documento esistente, quindi fare clic su **Seleziona** nell&#39;angolo in basso a destra dell&#39;estensione Workfront.
1. Fai clic sul pulsante **Commento** , quindi digita l&#39;aggiornamento nella casella visualizzata.

1. (Facoltativo) Per includere altri utenti o team Workfront nel commento, inizia a digitare il nome di un utente o di un team nel **Notifica a persone o team** quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.
1. (Facoltativo) Per richiedere l&#39;approvazione del documento, selezionare **Effettuare una richiesta di approvazione**.
1. Fai clic su **Aggiorna**.

   Un aggiornamento viene pubblicato nella scheda Aggiornamenti del documento. Gli utenti Workfront che includi nel commento ricevono una notifica in-app e, a seconda della configurazione di Workfront, potrebbero ricevere anche una notifica e-mail.

   Per ulteriori informazioni sulle notifiche in Workfront, vedi [Visualizzare e gestire le notifiche in-app](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md). 

   Per ulteriori informazioni sulla ricezione delle notifiche e-mail, consulta [Notifiche Adobe Workfront](../../workfront-basics/using-notifications/wf-notifications.md).

## Richiedere l’approvazione di un documento da Illustrator o InDesign

È possibile richiedere l’approvazione di un documento Workfront direttamente da un’applicazione Adobe.

È possibile richiedere l&#39;approvazione di un documento da parte delle seguenti entità:

* Un utente Workfront
* Un utente esterno senza un account Workfront

È possibile richiedere un&#39;approvazione su un documento da un&#39;applicazione Adobe nei seguenti modi:

* Allegando un approvatore al documento.
* Commentando un documento, informare la persona quando si fa un commento. e allegarle come approvatore al documento.

   Per informazioni sulla richiesta di approvazione quando si commenta un documento, vedere [Commento su un documento Workfront da Illustrator o InDesign](#comment-on-a-workfront-document-from-illustrator-or-indesign) in questo articolo.

Per richiedere un&#39;approvazione su un documento da un&#39;applicazione di Adobe:

1. Apri una delle applicazioni di Adobe supportate.
1. Se l&#39;estensione Workfront non è visualizzata, fai clic su **Finestra** > **Estensioni** > Workfront.

   Viene visualizzato un elenco di elementi di lavoro assegnati se il progetto è in uno stato corrente. Se un elenco non viene visualizzato, accedi a Workfront.

   I compiti personali sono elencati in **Nessun progetto**.

1. Fare clic sul progetto, sull&#39;attività o sul problema in cui è elencato il documento esistente, quindi fare clic sul nome del documento esistente.

   Per cercare il problema, digita il nome nel **Ricerca** casella e selezione **Progetto**, **Attività** oppure **Problema** dal menu a discesa a destra del **Ricerca** scatola. Se il nome dell&#39;elemento di lavoro non viene visualizzato nell&#39;elenco, premere **Invio** per cercare tutti gli elementi Workfront a cui hai accesso per la visualizzazione.

1. Fare clic sul nome del documento esistente, quindi fare clic su **Seleziona** nell&#39;angolo in basso a destra dell&#39;estensione Workfront.
1. Fai clic sul pulsante **Approvazione** scheda .
1. Per aggiungere un approvatore, nella **Inizia a digitare una casella di nome** eseguire una delle operazioni seguenti:

   * Digitare il nome di un approvatore, quindi selezionarlo quando viene visualizzato nell&#39;elenco.

      ![](assets/adobe-cc-adding-a-doc-approver-350x189.png)

   * Digita l’indirizzo e-mail di un utente esterno.

1. Fai clic su **Richiesta approvazione**.

   Gli utenti Workfront che includi nel commento o aggiungi come approvatore ricevono una notifica in-app e, a seconda della configurazione di Workfront, potrebbero ricevere anche una notifica e-mail.\
   Gli utenti esterni ricevono una notifica e-mail dalla quale possono prendere una decisione sull’approvazione.

   Per informazioni sulle notifiche in Workfront, vedi [Visualizzare e gestire le notifiche in-app](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md). Per informazioni sulla ricezione delle notifiche e-mail, vedi [Notifiche Adobe Workfront](../../workfront-basics/using-notifications/wf-notifications.md).

## Generare una bozza da Illustrator o InDesign {#generate-a-proof-from-illustrator-or-indesign}

Se l&#39;organizzazione utilizza modelli di flusso di lavoro automatizzato, è possibile generare una bozza per un documento creato in un&#39;applicazione Adobe senza uscire dall&#39;applicazione. Per informazioni sulla creazione delle bozze, consulta [Creazione di bozze](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md). Per informazioni sui modelli di flusso di lavoro automatizzato, consulta [Modelli di flusso di lavoro automatizzati](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md#automate) in [Panoramica del flusso di lavoro automatizzato](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

1. Apri una delle applicazioni di Adobe supportate.
1. Se l&#39;estensione Workfront non è visualizzata, fai clic su **Finestra** > **Estensioni** > Workfront.

   Viene visualizzato un elenco di elementi di lavoro assegnati se il progetto è in uno stato corrente. Se un elenco non viene visualizzato, accedi a Workfront.

   I compiti personali sono elencati in **Nessun progetto**.

1. Se il documento è già caricato in Workfront, seleziona il progetto, l’attività o il problema nell’estensione Workfront in cui è elencato il documento, quindi fai clic sul nome del documento.

   Oppure

   Caricare un documento di Adobe in un oggetto Workfront, come descritto nella sezione [Caricare un file in un progetto, un&#39;attività o un problema Workfront](#upload-a-file-to-a-workfront-project-task-or-issue) in questo articolo, fare clic sul nome del documento.

1. In **Fare clic per selezionare il formato** scegliere il formato in cui salvare il file in Workfront dal menu a discesa.

   Alcuni formati non sono disponibili dopo l’abilitazione della funzionalità di correzione nel passaggio successivo a questo. Per ulteriori informazioni, consulta [Formati di file esportati supportati](#supported-exported-file-formats) in questo articolo.

1. Fai clic su **Carica come nuova bozza** per abilitarlo.
1. Seleziona la **Modello di flusso di lavoro** si desidera che gli utenti utilizzino durante la revisione del documento.

   L’amministratore di Workfront imposta i modelli di flusso di lavoro automatizzato, come descritto in . In caso di domande, rivolgiti all’amministratore.

   1. Aggiungi almeno uno **Nuovo destinatario** in ogni fase del modello di flusso di lavoro.

      È possibile iniziare a digitare un nome e selezionarlo quando lo si visualizza nell’elenco a discesa visualizzato.

   1. Specifica la **Ruolo di prova** e la frequenza **Avvisi e-mail** per ogni destinatario aggiunto.

   1. (Facoltativo) In **Notifica e-mail** seleziona se inviare una notifica e-mail con un messaggio personalizzato facoltativo relativo alla bozza a tutti i destinatari della bozza aggiunti.

1. Fai clic su **Crea bozza**.

   Puoi visualizzare l’avanzamento del processo di creazione delle prove. Al termine della generazione viene visualizzato un avviso. Puoi aprire l’attività in cui hai creato la bozza ed è elencata lì.

## Carica una nuova versione di una bozza senza uscire da Illustrator o InDesign

1. Fare clic su un documento esistente con una bozza, quindi fare clic su **Seleziona** nell&#39;angolo in basso a destra.
1. Fai clic su **Carica come nuova versione di prova** per abilitarlo.
1. (Facoltativo) Seleziona la **Modello di flusso di lavoro** desideri che gli utenti utilizzino durante la revisione della nuova versione.

   Se non selezioni un modello diverso, il modello selezionato per la versione precedente rimane attivo. Inoltre, se hai modificato il modello per la versione precedente, le modifiche sono effettive per la nuova versione.

   L’amministratore di Workfront imposta i modelli di flusso di lavoro automatizzato, come descritto in . In caso di domande, rivolgiti all’amministratore.

   1. Aggiungi almeno uno **Nuovo destinatario** in ogni fase del modello di flusso di lavoro.

      È possibile iniziare a digitare un nome e selezionarlo quando lo si visualizza nell’elenco a discesa visualizzato.

   1. Specifica la **Ruolo di prova** e la frequenza **Avvisi e-mail** per ogni destinatario aggiunto.
   1. (Facoltativo) In **Notifica e-mail** seleziona se inviare una notifica e-mail con un messaggio personalizzato facoltativo relativo alla bozza a tutti i destinatari della bozza aggiunti.

1. Fai clic su **Crea nuova versione di prova**.

   Puoi visualizzare l’avanzamento del processo di creazione delle prove. Al termine della generazione viene visualizzato un avviso. Puoi aprire l’attività in cui hai creato la bozza ed è elencata lì.

## Esci dall’estensione Workfront

1. Nell’applicazione Adobe, fai clic su **Finestra** > **Estensioni** > Workfront.

1. Fai clic sul pulsante **Altro** menu ![](assets/more-menu.png) nell’angolo superiore destro del pannello.

1. (Facoltativo) Fai clic su **Feedback** per aprire un breve sondaggio e inviare a Workfront i vostri commenti su Workfront for Adobe Creative Cloud. 
1. Fai clic su **Logout**.\
   Viene visualizzata la schermata Accesso. Per informazioni sull&#39;accesso, vedi [Accedi all’estensione Workfront da Illustrator o InDesign](#log-in-to-workfront-extension-from-illustrator-or-indesign) in questo articolo.

## Formati di file esportati supportati {#supported-exported-file-formats}

* [Formati di file esportati supportati per Adobe InDesign](#supported-exported-file-formats-for-adobe-indesign)
* [Formati di file esportati supportati per Adobe Illustrator](#supported-exported-file-formats-for-adobe-illustrator)

### Formati di file esportati supportati per Adobe InDesign  {#supported-exported-file-formats-for-adobe-indesign}

Workfront supporta i seguenti formati di file per l’esportazione di un file da InDesign a Workfront:

* EPS - PostScript incapsulato
* EPUB - Pubblicazione elettronica a layout fisso
* EPUB - Pubblicazione elettronica a scorrimento &#42;
* HTML - Linguaggio di markup HyperText
* IDML - InDesign Markup Language &#42;
* JPG, JPEG - Joint Photographic Experts Group
* PDF - Adobe Portable Document File
* PNG - Grafica di rete portatile
* SWF - Flash Player &#42;
* XML - Extensible Markup Language &#42;

&#42; Questo formato di file non è disponibile quando **Carica una nuova bozza** è abilitato (per informazioni su questa opzione, consulta [Generare una bozza da Illustrator o InDesign](#generate-a-proof-from-illustrator-or-indesign) in questo articolo). Se questo formato di file è già selezionato prima dell&#39;attivazione **Carica una nuova bozza**, il formato del file viene modificato in PDF. È possibile selezionare un formato diverso dall’elenco.

### Formati di file esportati supportati per Adobe Illustrator  {#supported-exported-file-formats-for-adobe-illustrator}

Workfront supporta i seguenti formati di file per l’esportazione di un file da Illustrator a Workfront:

* DWG - Disegno AutoCAD, File di interscambio AutoCAD &#42;
* JPG, JPEG - Joint Photographic Experts Group
* PNG - Grafica di rete portatile
* Documento PSD - Photoshop
* SWF - Flash Player &#42;
* TIFF - Formato file immagine con tag

&#42; Questo formato di file non è disponibile quando **Carica una nuova bozza** è abilitato (per informazioni su questa opzione, consulta [Generare una bozza da Illustrator o InDesign](#generate-a-proof-from-illustrator-or-indesign) in questo articolo). Se questo formato di file è già selezionato prima dell&#39;attivazione **Carica una nuova bozza**, il formato del file viene modificato in PNG. È possibile selezionare un formato diverso dall’elenco.
