---
title: Crea record
description: Quando si utilizza Adobe Workfront Planning, un record è un'istanza di un tipo di record. È possibile creare record univoci per ogni tipo di record in Workfront Planning aggiungendoli manualmente alla vista tabella, importandoli da un elenco, duplicandoli o creandoli durante la connessione ad altri record.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 61cad7dc76ba04ea84ff0bd5052182f040f7b4d9
workflow-type: tm+mt
source-wordcount: '1336'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Crea record

{{planning-important-intro}}

In Adobe Workfront Planning, un record è un&#39;istanza di un tipo di record.

È possibile creare record eseguendo una delle operazioni seguenti:

* Aggiungerli dalla pagina del tipo di record nella visualizzazione tabella
* Copiare e incollare un elenco di record da un elenco esterno
* Duplicale
* Crearli mentre li si connette da altri record

In questo articolo viene descritto come creare record.

Per informazioni sulla gestione dei record nelle viste tabella o sequenza temporale, vedere gli articoli seguenti:

* [Gestire la vista tabella](/help/quicksilver/planning/views/manage-the-table-view.md)
* [Gestire la visualizzazione della timeline](/help/quicksilver/planning/views/manage-the-timeline-view.md)

## Requisiti di accesso

<!--Updated for GA-->

+++ Espandere per visualizzare i requisiti di accesso per Workfront Planning.

Per accedere a Workfront Planning, è necessario disporre dei seguenti elementi:

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
   <td role="rowheader"><p>Piano di pianificazione Adobe Workfront*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su ciò che è incluso in ogni piano di Workfront Planning, vedere <a href="https://business.adobe.com/products/workfront/pricing.html">Determinazione prezzi e packaging di Adobe Workfront</a>. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata di Adobe per Workfront</a>. </p> 
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
   <p>Modificare l'accesso in Workfront per i tipi di oggetto che si desidera creare (progetti e portafogli) quando si collegano i record. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td> <p>Consente di gestire le autorizzazioni per l'area di lavoro a cui si desidera aggiungere record. </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
   <p>Gestisci le autorizzazioni per gli oggetti Workfront (portfolio) per aggiungere oggetti figlio (progetti).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello di layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--OLD info: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p>  
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Adobe Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements for Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

+++


## Creare record aggiungendoli a un tipo di record <!--in a record type table (I don't think you can create them elsewhere right now)-->

È possibile creare record nella vista tabella di una pagina del tipo di record.

Per informazioni sulla modifica delle informazioni sui record, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro in cui si desidera aggiungere i record.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record. Per informazioni sulla creazione di un tipo di record, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

   La pagina del tipo di record viene visualizzata nella visualizzazione a cui si è effettuato l&#39;ultimo accesso. Per impostazione predefinita, nella vista tabella viene visualizzata una pagina del tipo di record.
Tutti i record del tipo selezionato vengono visualizzati nella vista.

1. (Condizionale) A seconda della vista visualizzata, effettuate una delle seguenti operazioni:

   * Dalla vista tabella:

      * Fai clic su **Nuovo record** nell&#39;ultima riga della tabella

      * Fai clic su **Maiusc + Invio** sulla tastiera da qualsiasi colonna o riga della tabella. In questo modo viene aggiunta una riga vuota sotto il record iniziale.
      * Passa il puntatore del mouse sul campo principale di un record, fai clic sul menu **Altro** ![](assets/more-menu.png) a destra del campo, quindi fai clic su **Inserisci record sopra** o su **Inserisci record sotto**.

     ![](assets/adding-a-new-campaign-in-table-row.png)

   * Da qualsiasi vista:

      * Fai clic su **Nuovo record** nell&#39;angolo superiore destro della pagina. Viene visualizzata la casella di anteprima del record.

     Workfront carica automaticamente una miniatura e un&#39;immagine di copertina in ogni nuovo record. In seguito sarà possibile modificare queste immagini. Per informazioni, vedere i seguenti articoli:

      * [Aggiungere una copertina a un record](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
      * [Aggiungere una miniatura a un record](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

1. Iniziare a digitare informazioni sul nuovo record nei campi visualizzati nella casella di anteprima.

   >[!NOTE]
   >
   >  * Non esistono campi obbligatori per i record. È tuttavia consigliabile aggiungere informazioni per il campo principale di un record, in quanto è utile identificare i record quando si collegano tra loro record. Per ulteriori informazioni sui campi primari, vedere [Gestire la visualizzazione tabella](/help/quicksilver/planning/views/manage-the-table-view.md) e [Panoramica campo primario](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * I campi che fanno riferimento ad altri tipi di record o campi calcolati sono campi di sola lettura.

1. (Condizionale) Quando aggiungi record nella tabella, continua ad aggiungere informazioni su ogni riga, quindi fai clic su **Invio** sulla tastiera per salvare le modifiche.

   Oppure

   Fare clic sul nome del nuovo record o sull&#39;icona **Apri dettagli** ![](assets/open-details-icon-in-table-name-field.png) a sinistra del nome del record. Nella tabella viene visualizzata un&#39;anteprima con le informazioni dettagliate del record.

   >[!TIP]
   >
   >Puoi accedere all&#39;icona **Apri dettagli** solo dal campo del nome del record quando il campo Nome è un campo primario.

1. Iniziare a modificare le informazioni del record nell&#39;anteprima del record. Workfront salva automaticamente le modifiche.
1. (Facoltativo) Fai clic sull&#39;icona **Apri in una nuova scheda** ![](assets/open-details-in-a-new-tab-icon.png) nell&#39;angolo superiore destro dell&#39;anteprima del record per aprire la pagina del record in una nuova scheda. Continuare a modificare il record nella pagina record. Per informazioni, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

1. (Facoltativo) Utilizzare le seguenti scelte rapide da tastiera per annullare o ripetere l&#39;aggiunta di nuovi record o delle relative informazioni quando questi vengono aggiunti nella vista tabella:

   * CTRL + Z (⌘ + Z per Mac) per annullare una modifica
   * CTRL + MAIUSC + Z (⌘ + MAIUSC + Z per Mac) per ripetere una modifica

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

È possibile creare record o oggetti Workfront quando vengono collegati da altri record.

Prima di aggiungere nuovi record o oggetti Workfront collegandoli da record esistenti, è necessario disporre dei seguenti elementi:

* Tipi di record collegati. Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).
* Record collegati. Per informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).
* L&#39;accesso e le autorizzazioni corretti in Workfront Planning e Workfront, come descritto nella sezione [Requisiti di accesso](#access-requirements) in questo articolo.

>[!NOTE]
>
>La creazione di progetti e portafogli di Workfront quando vengono collegati ai record di Workfront Planning è simile alla creazione di record di Planning quando vengono collegati da altri record.

Per creare i record durante la connessione da altri record:

1. Avviare la connessione dei record di Workfront Planning, come descritto nell&#39;articolo [Connetti record](/help/quicksilver/planning/records/connect-records.md).
1. (Condizionale) Se non è possibile trovare un record quando si tenta di aggiungerlo dal campo record connesso di un altro record, cercare un record, quindi fare clic su **+ Aggiungi**. Il pulsante **+ Aggiungi** è seguito dal nome del tipo di record da cui si sta effettuando la connessione.

   ![](assets/add-button-to-create-records-in-context-highlighted.png)

   Il record viene creato e aggiunto al campo record connesso.
1. (Facoltativo) Passare alla visualizzazione tabella del tipo di record di cui è stato creato il record. Nell&#39;ultima riga della visualizzazione viene visualizzato un nuovo record.
1. (Facoltativo) Inizia ad aggiungere informazioni per il nuovo record nella vista tabella
Oppure
Fai clic sul nome per aprire la pagina dei dettagli e aggiungere informazioni.

