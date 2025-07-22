---
title: Crea record
description: Quando si utilizza Adobe Workfront Planning, un record è un'istanza di un tipo di record. È possibile creare record univoci per ogni tipo di record in Workfront Planning aggiungendoli manualmente alla vista tabella, importandoli da un elenco, duplicandoli o creandoli durante la connessione ad altri record.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 948ca1f8a91e20616b5a42876df8432e85737b2d
workflow-type: tm+mt
source-wordcount: '2388'
ht-degree: 0%

---


# Crea record

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

In Adobe Workfront Planning, un record è un&#39;istanza di un tipo di record.

È possibile creare record eseguendo una delle operazioni seguenti:

* [Creare record utilizzando il pulsante Nuovo record o Richiedi record da qualsiasi visualizzazione del tipo di record](#create-records-using-the-new-record-or-request-record-button-from-any-record-type-view)
* [Creare record aggiungendoli in linea dalla vista tabella del tipo di record](#create-records-by-adding-them-inline-from-the-record-type-table-view)

<!--
* [Create records by adding them in the record type timeline view](#create-records-by-adding-them-in-the-record-type-timeline-view)-->

* [Copiare e incollare un elenco di record da un elenco esterno](#create-records-by-copying-and-pasting-them-from-an-external-list)
* [Duplicare record da una vista tabella](#create-records-by-duplicating-them)
* [Crea record durante la connessione da altri record](#create-records-as-you-connect-them)
* [Creare record inviando un modulo di richiesta a un tipo di record](#create-records-by-submitting-a-request-form-to-a-record-type)
* [Creare record importando informazioni da un file CSV o Excel](#create-records-by-importing-records-from-a-csv-or-excel-file)
* [Creare record utilizzando le automazioni](#create-records-by-using-automations)

Per informazioni sulla gestione dei record nelle viste tabella o sequenza temporale, vedere gli articoli seguenti:

* [Gestire la vista tabella](/help/quicksilver/planning/views/manage-the-table-view.md)
* [Gestire la visualizzazione della timeline](/help/quicksilver/planning/views/manage-the-timeline-view.md)

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Prodotti</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td> 
   <td> 
<p>Uno dei seguenti piani di Workfront:</p> 
<ul><li>Seleziona</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td> Standard
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p> 
   <p>Modificare l'accesso in Workfront per i tipi di oggetto che si desidera creare (progetti, programmi e portafogli) quando si collegano i record. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td> <p>Autorizzazioni Contribute o superiori per l'area di lavoro e il tipo di record in cui si desidera aggiungere record. </p>
   <p>Visualizza o autorizzazioni superiori per l'area di lavoro e il tipo di record per creare record utilizzando il pulsante Richiedi record nella pagina record</p>
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
   <p>Gestisci le autorizzazioni per gli oggetti Workfront (portfolio) per aggiungere oggetti figlio (progetti).</p>
   </td> 
  </tr>

</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare record utilizzando il pulsante Nuovo record o Richiedi record da qualsiasi visualizzazione del tipo di record

Gli utenti con autorizzazioni di visualizzazione per l&#39;area di lavoro e il tipo di record possono creare record solo utilizzando il pulsante Richiedi record nella pagina Tipo di record.

Gli utenti con le autorizzazioni Contribute e Manage per l&#39;area di lavoro e il tipo di record possono creare record utilizzando il pulsante Nuovo record nella pagina del tipo di record.


>[!IMPORTANT]
>
>Un manager dell&#39;area di lavoro deve creare un modulo di richiesta per il tipo di record affinché gli utenti con autorizzazioni di visualizzazione possano aggiungere record utilizzando un modulo di richiesta. In caso contrario, gli utenti con autorizzazioni di visualizzazione non potranno creare record.

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro in cui si desidera aggiungere i record.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record. Per informazioni sulla creazione di un tipo di record, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

   La pagina del tipo di record viene visualizzata nella visualizzazione a cui si è effettuato l&#39;ultimo accesso. Per impostazione predefinita, nella vista tabella viene visualizzata una pagina del tipo di record.
Tutti i record del tipo selezionato vengono visualizzati nella vista.

1. (Condizionale) Da qualsiasi vista, fai clic su quanto segue nell’angolo superiore destro dello schermo, a seconda dell’area di lavoro e delle autorizzazioni per il tipo di record:

   * Fare clic su **Nuovo record** se si dispone delle autorizzazioni Contribute o di livello superiore per l&#39;area di lavoro e il tipo di record

     Oppure

   * Fare clic su **Richiedi record** se si dispone delle autorizzazioni di visualizzazione per l&#39;area di lavoro e il tipo di record.

1. (Condizionale) Se hai fatto clic su **Nuovo record**, effettua le seguenti operazioni:

   1. Fare clic su uno dei modi seguenti per creare un record, quindi fare clic su **Continua**:

      * **Aggiungi manualmente**. Viene visualizzata la casella di anteprima del record.\
        Aggiungere informazioni sul record come descritto in [Creare i record aggiungendoli in linea dalla sezione della tabella dei tipi di record](#create-records-by-adding-them-inline-from-the-record-type-table-view) in questo articolo, a partire dal passaggio 6. <!--insure this stays accurate-->
      * **Carica da file**
Aggiungere record come descritto nell&#39;articolo [Creare record importando informazioni da un file CSV o Excel](/help/quicksilver/planning/records/import-file-to-create-records.md), a partire dal passaggio 6. <!--ensure this stays accurate-->
      * **Invia una richiesta**
Viene aperto il modulo di richiesta del tipo di record.

        Per poter aggiungere un record utilizzando un modulo di richiesta, il manager dell’area di lavoro deve creare un modulo di richiesta.

        >[!TIP]
        >
        >Alcuni tipi di record possono avere più maschere. Fai clic su uno per aprirlo.

        Aggiungere il record, come descritto nell&#39;articolo [Inviare le richieste di Adobe Workfront Planning per la creazione dei record](/help/quicksilver/planning/requests/submit-requests.md), a partire dal passaggio 6. <!--ensure this stays accurate-->

      ![Tre modi per creare record a scelta modale](assets/three-ways-to-create-records-choice-modal.png)

1. (Condizionale) Se hai fatto clic su **Record richiesta**, effettua le seguenti operazioni:

   1. (Condizionale) Se il tipo di record dispone di più moduli di richiesta, fare clic su uno per selezionarlo.
   2. Continuare ad aggiungere informazioni nel modulo per creare il record, come descritto nell&#39;articolo [Inviare richieste di Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md), a partire dal passaggio 6. <!--ensure this stays accurate-->

1. (Condizionale) Esamina i nuovi record.

   A seconda della modalità di aggiunta del record, possono verificarsi alcuni degli eventi seguenti:

   * Al tipo di record viene aggiunto un nuovo record, a meno che non si sia scelto di aggiungerlo utilizzando un modulo di richiesta con un processo di approvazione. L&#39;approvazione deve essere concessa da tutti gli approvatori prima della creazione del record.
   * Se si aggiungono record utilizzando un foglio di calcolo CSV o Excel, al tipo di record verranno aggiunti più record.
   * Se la richiesta è stata aggiunta inviando un modulo di richiesta, nella scheda Pianificazione dell&#39;area Richieste Workfront viene aggiunta una nuova richiesta.

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    The following items are created in Workfront Planning:

    * A read-only record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Planning record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Planning records you're linking from. 
   
-->

## Creare record aggiungendoli in linea dalla vista tabella del tipo di record

È possibile creare record nella vista tabella di una pagina del tipo di record quando vengono aggiunti in linea.

Per informazioni sulla modifica delle informazioni sui record, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro in cui si desidera aggiungere i record.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record. Per informazioni sulla creazione di un tipo di record, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

   La pagina del tipo di record viene visualizzata nella visualizzazione a cui si è effettuato l&#39;ultimo accesso. Per impostazione predefinita, nella vista tabella viene visualizzata una pagina del tipo di record.
I record del tipo selezionato vengono visualizzati nella vista.

1. (Condizionale) Nella vista a tabella, effettuate una delle seguenti operazioni:

   * Fare clic su **Nuovo record** nell&#39;ultima riga della tabella o dopo l&#39;ultimo record di un raggruppamento

     >[!TIP]
     >
     >Quando si aggiunge un nuovo record dopo l&#39;ultimo record di un raggruppamento o di un sottogruppo, Workfront compila automaticamente i campi inclusi nei raggruppamenti. Se necessario, è possibile modificare manualmente questi campi e i record potrebbero essere rimossi dal raggruppamento.

   * Fai clic su **Maiusc + Invio** sulla tastiera da qualsiasi colonna o riga della tabella. In questo modo viene aggiunta una riga vuota sotto il record iniziale.
   * Passa il puntatore del mouse sul campo principale di un record, fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del campo, quindi fai clic su **Inserisci record sopra** o **Inserisci record sotto**.

   ![Aggiunta di una nuova campagna nella riga della tabella](assets/adding-a-new-campaign-in-table-row.png)

   Workfront carica automaticamente una miniatura in ogni nuovo record. In seguito sarà possibile modificare queste immagini. Per informazioni, vedere [Aggiungere un&#39;immagine di copertina a un record](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

   Nella tabella viene aggiunto un nuovo record.

1. Fare clic sul campo principale del nuovo record

   Oppure

   Fai clic sull&#39;icona **Apri dettagli** ![Apri icona dettagli nel campo nome tabella](assets/open-details-icon-in-table-name-field.png) a sinistra del nome del record.

   Nella tabella viene visualizzata la casella di anteprima.

1. Iniziare a digitare informazioni sul nuovo record nei campi visualizzati nella casella di anteprima.

   >[!NOTE]
   >
   >  * Non esistono campi obbligatori per i record. È tuttavia consigliabile aggiungere informazioni per il campo principale di un record, in quanto è utile identificare i record quando si collegano tra loro record. Per ulteriori informazioni sui campi primari, vedere [Gestire la visualizzazione tabella](/help/quicksilver/planning/views/manage-the-table-view.md) e [Panoramica campo primario](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * I campi che fanno riferimento ad altri tipi di record o campi calcolati sono campi di sola lettura.

1. (Condizionale) Quando si aggiungono record nella tabella, prima di aprire la casella di anteprima del record, continuare ad aggiungere informazioni su ogni riga, quindi fare clic su **Invio** sulla tastiera per salvare le modifiche.

   Oppure

   Fare clic sul nome del nuovo record o sull&#39;icona **Apri dettagli** ![Apri icona dettagli nel campo nome tabella](assets/open-details-icon-in-table-name-field.png) a sinistra del nome del record per aprire la casella di anteprima e modificare le informazioni del record nell&#39;area dei dettagli.

   >[!TIP]
   >
   >Puoi accedere all&#39;icona **Apri dettagli** solo dal campo del nome del record quando il campo Nome è un campo primario.

1. (Facoltativo) Dalla casella di anteprima del record, fare clic sull&#39;icona **Apri in una nuova scheda** ![Apri i dettagli in una nuova scheda icona](assets/open-details-in-a-new-tab-icon.png) nell&#39;angolo superiore destro per aprire la pagina del record in una nuova scheda. Continuare a modificare il record nella pagina record. Per informazioni, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

   Workfront salva automaticamente le modifiche.

1. (Facoltativo) Se si apre la pagina del record, chiudere la casella di anteprima o fare clic sulla freccia indietro a sinistra del nome del record.

1. (Facoltativo) Nella vista tabella, utilizzare le seguenti scelte rapide da tastiera per annullare o ripristinare l&#39;aggiunta di nuovi record o delle relative informazioni durante l&#39;aggiunta nella vista tabella:

   * CTRL + Z (⌘ + Z per Mac) per annullare una modifica
   * CTRL + MAIUSC + Z (⌘ + MAIUSC + Z per Mac) per ripristinare una modifica

<!--<div class="preview">

## Create records by adding them in the record type timeline view

You can create records in the timeline view of a record type page, by double-clicking in the timeline. 

For information about creating a timeline view, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).

{{step1-to-planning}}
  
1. Click the workspace where you want to add records.

    The workspace opens and the record types display as cards.

1. Click a record type card. 

    The record type page opens in the view that you last accessed. 

1. Click to open a timeline view, or create a timeline view, first. 

    >[!NOTE]
    >
    >You can create a timeline view only if there are at least two date fields associated with the record type.
1. Double-click anywhere in the timeline. 

    A new record box opens. 

    ![New record box on timeline with unnamed record bar](assets/new-record-small-box-on-timeline.png)
1. Update the following information:

    * **Name**: Enter the name of the record. If you leave it empty, Workfront names it **Untitled** by default. The name will not be visible in the record bar if left empty. 
    * **Record date fields**: Update the dates of the record. 
        
        The names of the date fields are customized according to the fields selected for the Start and End dates when the timeline view was created.

        By default, date values are preselected depending on how you display the timeline view. The following scenarios exist:

        * By **Year**: The record start and end dates span a month.
        * By **Quarter**: The record start and end dates span a week. 
        * By **Month**: The record start and end dates span three days.

1. (Optional) Click one of the following icons: 

    * **Expand** ![Expand icon](assets/expand-icon.png) to open the record details in the preview window. 
    * **Delete** ![Delete icon](assets/delete-icon.png) to delete the record.
    * **Close**  ![Close icon](assets/close-icon.png) to close the new record box. 

    The record is added to the timeline as well as to the table and calendar views immediately, unless you clicked the **Delete** icon. 

1. (Optional) Click the record bar in the timeline to open the record's details window and update its information, delete it, or add comments. 

    >[!TIP]
    >
    >By default, Workfront associates the record with a thumbnail and a cover image.
    >
    >The thumbnail displays in the timeline view only when it is enabled in the Settings of the view. 

</div>-->

## Creare record copiandoli e incollandoli da un elenco esterno

1. Iniziare a creare record nella visualizzazione Tabella, come descritto nella sezione [Creare record aggiungendoli manualmente a un tipo di record](#create-records-by-manually-adding-them-to-a-record-type) in questo articolo.

   Verificare che nella vista tabella siano presenti le colonne o i campi che si desidera compilare con le nuove informazioni del record.

1. Fare clic su **Nuovo &lt; Nome tipo di record >** nell&#39;ultima riga della tabella per aggiungere alla tabella tutte le nuove righe desiderate per i nuovi record.

   Aggiungere ad esempio 10 righe alla vista tabella se si desidera incollare le informazioni relative a 10 nuovi record da un&#39;altra applicazione.

1. In un&#39;altra applicazione creare un elenco di record che si desidera importare.

   Ad esempio, puoi utilizzare un foglio di calcolo Excel per creare l’elenco.

   L’elenco deve contenere informazioni in formato tabulare.

   >[!TIP]
   >
   > Le colonne dell’elenco devono contenere informazioni relative ai campi esistenti in Workfront.
   >
   > Assicurati di avere già creato i campi desiderati in Workfront e che le informazioni nel foglio siano visualizzate nel formato corretto che corrisponde a quello di ciascun campo in Workfront.

1. In un&#39;altra applicazione, selezionare più righe e colonne, quindi incollare le informazioni nella vista tabella del tipo di record, a partire dal primo nuovo record.

   Nell&#39;area Workfront Planning vengono importate le seguenti informazioni:

   * Le righe contengono i nuovi record
   * Nelle colonne vengono inserite le informazioni relative ai campi dei record.

## Creare record duplicandoli

Per informazioni sulla duplicazione dei record, vedere [Record duplicati](/help/quicksilver/planning/records/copy-or-duplicate-records.md).

## Creare i record durante la connessione

È possibile creare i seguenti tipi di oggetto quando si collegano da altri record:

* Record di Workfront Planning
* Oggetti Workfront

In questa sezione viene descritto come creare record di Workfront Planning durante la connessione da altri record.

>[!NOTE]
>
>La creazione di progetti e portafogli di Workfront quando vengono collegati ai record di Workfront Planning è simile alla creazione di record di Planning quando vengono collegati da altri record.
>
>Per informazioni sulla creazione di oggetti Workfront da Workfront Planning, vedere [Creare oggetti Workfront da Workfront Planning durante la connessione ai record](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md).

Prima di poter aggiungere nuovi record collegandoli da quelli esistenti, è necessario disporre dei seguenti elementi:

* Tipi di record collegati. Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).
* Record.
* L&#39;accesso e le autorizzazioni corretti in Workfront Planning e Workfront, come descritto nella sezione [Requisiti di accesso](#access-requirements) in questo articolo.

Per creare i record durante la connessione da altri record:

1. Avviare la connessione dei record di Workfront Planning, come descritto nell&#39;articolo [Connetti record](/help/quicksilver/planning/records/connect-records.md). È possibile collegare record dalle seguenti aree:

   * Un campo di connessione nelle seguenti aree di Workfront Planning:

      * Vista tabella
      * Pagina dei dettagli o casella di anteprima di un record

   * Campo di connessione nella sezione Pianificazione di un progetto, portfolio o programma in Workfront.

     Per informazioni, vedere [Gestire le connessioni record dagli oggetti Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

1. (Condizionale) Se non riesci a trovare un record durante il tentativo di connessione, fai clic su **+ Aggiungi**

   Oppure
Inizia a digitare un nome, quindi fai clic su **+ Aggiungi**. Il pulsante **+ Aggiungi** è seguito dal nome del tipo di record a cui ti stai connettendo. Ad esempio, &quot;Aggiungi marchi&quot; quando si aggiunge un marchio a una campagna esistente. Il nome digitato segue anche il pulsante Aggiungi.

   ![Pulsante Aggiungi per creare record nel contesto evidenziato](assets/add-button-to-create-records-in-context-highlighted.png)

   Il record viene creato e aggiunto al campo record connesso.

   >[!IMPORTANT]
   >
   >* In Workfront è possibile creare solo progetti, portfolio e programmi quando si collegano da un record.
   >
   >* Non è possibile creare gruppi o società quando si collegano da un record in Workfront Planning.
   > 

1. (Facoltativo) Passare alla visualizzazione tabella del tipo di record di cui è stato creato il record. Nell&#39;ultima riga della visualizzazione viene visualizzato un nuovo record.
1. (Facoltativo) Inizia ad aggiungere informazioni per il nuovo record nella vista tabella
Oppure
Fai clic sul nome per aprire la pagina dei dettagli e aggiungere informazioni.

## Creare record inviando un modulo di richiesta a un tipo di record

Dopo che un utente ha creato un modulo di richiesta per un tipo di record e ha condiviso con sé un collegamento, è possibile inviare una richiesta per creare un record per tale tipo di record.

Per informazioni, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Sia gli utenti di Workfront che quelli esterni all&#39;organizzazione possono inviare richieste ai tipi di record di Planning e creare record, se dispongono di un collegamento al modulo di richiesta.

Per informazioni, vedere [Inviare le richieste di Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md).

## Creare record durante l&#39;importazione di tipi di record da un file CSV o Excel

È possibile importare record quando si importano tipi di record utilizzando un file CSV o Excel.

Per informazioni, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

## Creare record importando record da un file CSV o Excel

È possibile importare record per i tipi di record esistenti quando si importano informazioni da un file CSV o Excel.

Per informazioni, vedere [Creare record importando informazioni da un file CSV o Excel](/help/quicksilver/planning/records/import-file-to-create-records.md).

## Creare record utilizzando le automazioni

In Workfront Planning è possibile configurare automazioni che, se attivate, creano record quando attivate da un record di Planning. I record creati vengono automaticamente connessi ai record da cui si sta attivando l’automazione.

È possibile configurare e attivare l&#39;automazione nella pagina del record in Workfront Planning. Il record connesso creato viene inserito nel campo connesso del tipo di record da cui viene eseguita l&#39;automazione.

Per informazioni, vedere [Creare oggetti utilizzando le automazioni dei record di Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).



