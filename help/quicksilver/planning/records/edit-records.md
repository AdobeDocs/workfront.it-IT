---
title: Modifica record
description: È possibile modificare le informazioni del record in Adobe Workfront Planning. È necessario creare i tipi di record prima di iniziare a creare e modificare i record.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '2940'
ht-degree: 0%

---


# Modifica record

<!--keep the choice values information in yellow till Jan 2026-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

È possibile modificare le informazioni sui record in Adobe Workfront Planning modificando i valori dei campi associati ai record.

È necessario creare i tipi di record prima di iniziare a creare e modificare i record.

Per informazioni, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

Per informazioni sulla creazione di record, vedere [Crea record](/help/quicksilver/planning/records/create-records.md).

&lt;!— menziona qui che i campi nella visualizzazione Dettagli sono gli stessi di quelli nella visualizzazione tabella — questo articolo è collegato da Gestisci visualizzazioni record uno per fare riferimento a queste informazioni—>

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi pacchetto Workfront e Planning</p> <p>Qualsiasi flusso di lavoro e qualsiasi pacchetto di Planning</p>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Contribuire o concedere autorizzazioni superiori a un’area di lavoro e a un tipo di record  </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p> </td> 
  </tr>   
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> <p>Standard</p> 
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> -->

## Considerazioni sulla modifica dei record

* Se si dispone delle autorizzazioni necessarie per l&#39;area di lavoro, è possibile modificare i record creati o quelli creati da altri utenti.
* È possibile modificare i campi record dalle seguenti aree:

   * Anteprima del record in una visualizzazione record
   * Pagina dettagli record
   * In linea, in una vista a tabella.
   * La vista calendario e la vista timeline quando si ridimensionano o si trascinano i record. In questo modo vengono aggiornate le date dei record.

* Quando un utente modifica un record in una visualizzazione, le modifiche sono immediatamente visibili in tutte le visualizzazioni e le pagine dei record a tutti gli altri utenti.

* I seguenti tipi di campi vengono aggiornati automaticamente e non è possibile modificarne i valori manualmente:
   * Campi collegati da altri record
   * Campi di tipo formula
   * Campi di sistema (Creato da, Data di creazione, Autore ultima modifica, Data ultima modifica)
* Se i record visualizzati sono collegati ad altri record, le nuove informazioni dei record che si sta modificando verranno applicate ai record collegati in tutte le aree di lavoro in cui il record è collegato.
* Non è possibile modificare i record in blocco. <!--this will probably change-->
* Gli URL vengono riconosciuti come collegamenti nei tipi di campi di testo a riga singola solo quando iniziano con: http://, https://, ftp:// o www. .
* È possibile aggiungere un&#39;immagine di copertina a ogni record. L&#39;immagine è univoca per ogni record e non si applica a tutti i record contemporaneamente.
* È possibile modificare l&#39;ordine dei campi in una pagina record e aggiungere un&#39;immagine di copertina per un record. Per ulteriori informazioni, vedere [Gestire il layout della pagina record](/help/quicksilver/planning/records/manage-the-record-page.md).
* È possibile modificare le date di inizio e di fine di un record ridimensionando o riposizionando i record nelle visualizzazioni Timeline e Calendario.

  Non è possibile ridimensionare o riposizionare i record quando la data di inizio e la data di fine scelte per il record sono di sola lettura. Ad esempio, l&#39;utilizzo di campi di ricerca o di formula per le date di inizio e di fine di un record non consente di ridimensionare o riposizionare il record in una visualizzazione timeline e calendario. <!--this also repeats below, for the timeline and the calendar views; also update there, if this changes-->

## Modifica record

È possibile modificare un record dalle seguenti aree:

* [Vista tabella](#edit-a-record-inline-in-the-table-view-of-a-record-type)
* [Vista timeline](#edit-a-record-in-the-timeline-view-of-a-record-type)
* [Vista calendario](#edit-a-record-in-the-calendar-view-of-a-record-type)
* [Anteprima del record in una visualizzazione](#edit-a-record-from-the-records-preview-in-a-view)
* [Pagina del record](#edit-a-record-from-the-records-page)
* [Un oggetto Workfront nella sezione Planning](#edit-a-record-from-a-workfront-object-in-the-planning-section)

Per modificare le date dei record, eseguire le operazioni seguenti:

* [Ridimensionare le barre dei record nella visualizzazione Timeline e Calendario]

### Modificare un record in linea nella vista tabella di un tipo di record

Quando si modificano i record dalla vista tabella, viene indicato quale campo viene modificato da altri utenti al momento della visualizzazione del record.

Per ulteriori informazioni, vedere [Gestire le visualizzazioni dei record](/help/quicksilver/planning/views/manage-record-views.md).

Quando si aggiunge un nuovo record dopo l&#39;ultimo record di un raggruppamento o di un sottogruppo, Workfront aggiorna automaticamente i campi inclusi nei raggruppamenti per i nuovi record. Se necessario, è possibile modificare manualmente questi campi e i record potrebbero essere rimossi dal raggruppamento.

Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera modificare i record

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.
1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.
1. (Condizionale) Fare clic sulla scheda di una visualizzazione tabella oppure fare clic su **+ Visualizzazione** per creare una visualizzazione tabella. La vista tabella deve essere quella predefinita, a meno che il tipo di record non sia stato visualizzato in un altro tipo di vista all&#39;ultimo accesso.

   I record associati al tipo di record selezionato vengono visualizzati nella vista tabella.
1. Fare clic all&#39;interno della riga di un record per iniziare a modificare le informazioni sul record in linea.

   ![Modifica campo paragrafo record con visualizzazione tabella di formattazione](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!TIP]
   >
   >  Non è possibile modificare le informazioni per i campi seguenti, in quanto sono di sola lettura e Workfront li aggiorna automaticamente:
   >  
   >  * Campi collegati creati mediante la connessione di tipi di record. Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Campi dei tipi seguenti: Creato da, Data di creazione, Ultima modifica da, Data ultima modifica, Campi formula.

1. (Facoltativo e condizionale) Quando modifichi un campo di tipo Paragrafo, utilizza le seguenti **opzioni di formattazione Rich Text**:

   * Grassetto
   * Corsivo
   * Sottolineato
   * Aggiungi un collegamento
   * Aggiungere un elenco puntato
   * Aggiungere un elenco numerato

   ![Barra degli strumenti RTF nel campo paragrafo](assets/rich-text-toolbar-on-paragraph-field.png)

1. (Facoltativo) Fare doppio clic su un campo record connesso per aggiungere record o oggetti connessi a un altro record. Per ulteriori informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).
1. Premi **Invio** sulla tastiera o fai clic all&#39;esterno di una riga per salvare le modifiche. Le modifiche vengono salvate automaticamente. Un indicatore **Salvato** viene visualizzato brevemente nell&#39;angolo superiore destro della visualizzazione tabella per indicare che le modifiche sono state salvate.


1. (Facoltativo) Per copiare e incollare informazioni da un campo all&#39;altro, effettuare una delle seguenti operazioni:

   * Copiare uno o più valori esistenti di un campo, quindi incollarli in un campo dello stesso tipo in un altro record
   * Fare clic sull&#39;intestazione di una colonna per selezionarla e copiarla, quindi fare clic sull&#39;intestazione di un&#39;altra colonna e incollare il contenuto della colonna copiata. Le colonne devono contenere tipi di campo simili.
   * Con il tasto Maiusc premuto, fai clic su per selezionare più righe in una tabella, copia le informazioni nelle righe selezionate, quindi fai clic su una riga diversa e incolla le informazioni selezionate nella nuova riga e nelle righe successive.
   * Copiare le informazioni da una cella, quindi selezionare più celle e incollare le stesse informazioni in più celle. È possibile selezionare più celle e incollare le stesse informazioni in più celle da righe e colonne adiacenti.
   * Selezionare l&#39;angolo inferiore destro di una cella esistente contenente le informazioni da copiare, quindi trascinarlo e rilasciarlo nelle celle adiacenti in cui si desidera incollare le stesse informazioni. Tutte le celle devono contenere lo stesso tipo di informazioni.

     ![Angolo inferiore destro trascinabile per copia e incolla nella vista tabella](assets/dragable-lower-right-corner-for-copy-paste-in-table-view.png)


   * Copiare una o più celle da un&#39;origine esterna, ad esempio un file di Excel, quindi incollarle in uno dei seguenti tipi di campi:

      * Campi di connessione di Workfront Planning.
      * Campi Persone. Sono supportati solo i campi con un valore.

     Non è possibile copiare informazioni da un&#39;origine esterna e incollarle in altri tipi di campi, inclusi i campi di connessione di Workfront o di altre applicazioni.

   >[!NOTE]
   >
   >Considera quanto segue:
   >
   >* Utilizza le seguenti scelte rapide da tastiera per copiare e incollare le informazioni:
   >   * Copia: CTRL + C (⌘ + C per Mac)
   >   * Incolla: CTRL + V (⌘ + V per Mac)
   >
   >* Non è possibile copiare e incollare i valori dei campi nella pagina record. Questa funzionalità è supportata solo nella vista tabella di un tipo di record.
   >* Non è possibile copiare e incollare valori di campo per i tipi di campo seguenti:
   >
   >    * Campi di ricerca creati durante la connessione di tipi di record. È possibile copiare e incollare campi record collegati. Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).
   >    * Campi dei seguenti tipi: Creato da, Data di creazione, Ultima modifica da, Data ultima modifica

1. (Facoltativo) Utilizzare le seguenti scelte rapide da tastiera per annullare o ripetere la modifica o la copia e l&#39;incollamento delle informazioni del record:

   * CTRL + Z (⌘ + Z per Mac) per annullare una modifica
   * CTRL + MAIUSC + Z (⌘ + MAIUSC + Z per Mac) per ripristinare una modifica

   >[!TIP]
   >
   >    È possibile utilizzare più volte le scelte rapide da tastiera in una riga per annullare più modifiche.

1. (Facoltativo) Aggiungi una miniatura a un record. Per informazioni, vedere [Aggiungere una miniatura a un record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).


### Modificare un record nella visualizzazione timeline di un tipo di record

<!--add another step about drag and drop here when that is available-->

1. Aprire la pagina del tipo di record in una visualizzazione timeline. Per informazioni, vedere [Gestire la visualizzazione della sequenza temporale](/help/quicksilver/planning/views/manage-the-timeline-view.md).

1. Passa il puntatore del mouse sulle estremità della barra di un record, fai clic su e trascina il margine fino a un&#39;altra data. In questo modo viene aggiornata automaticamente la data di inizio o di fine del record.

   ![Barra a sinistra nella visualizzazione della sequenza temporale da ridimensionare](assets/left-end-bar-handle-to-resize-timeline-view.png)

1. Fare clic su una barra dei record e trascinarla in un&#39;altra posizione per aggiornare la cronologia e le date. Le date di inizio e fine del record vengono aggiornate automaticamente.

   >[!IMPORTANT]
   >
   >Non è possibile trascinare e rilasciare le estremità di una barra dei record, né trascinare e rilasciare il record in un&#39;altra data quando le date di inizio e di fine scelte per il record sono di sola lettura. Ad esempio, l&#39;utilizzo di campi di ricerca o di formula per le date di inizio e di fine di un record non consente di ridimensionare o riposizionare il record in una visualizzazione indicatore cronologico. <!--this also repeats in Considerations and in editing in the calendar view; also update there, if this changes-->

1. Fare clic sulla barra di un record per aprire l&#39;area dei dettagli e modificare tutti i campi.

   Per informazioni, vedere la sezione [Modificare un record dall&#39;anteprima del record in una visualizzazione](#edit-a-record-from-the-records-preview-in-a-view) in questo articolo.

### Modificare un record nella vista calendario di un tipo di record

<!--add another step about drag and drop here when that is available-->

1. Aprire la pagina del tipo di record in una visualizzazione calendario. Per informazioni, vedere [Gestire la visualizzazione del calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md).
1. (Facoltativo) Passa il puntatore del mouse sulle estremità della barra di un record nella visualizzazione calendario, quindi fai clic su e trascina i margini fino a un&#39;altra data. In questo modo viene aggiornata automaticamente la data di inizio o di fine del record.

   ![Barra a sinistra nella visualizzazione calendario per ridimensionare](assets/left-end-bar-handle-to-resize-calendar-monthly-view.png)

1. Fare clic su una barra dei record e trascinarla in un&#39;altra posizione per aggiornare la cronologia e le date. Le date di inizio e fine del record vengono aggiornate automaticamente.

   >[!IMPORTANT]
   >
   >Non è possibile trascinare e rilasciare le estremità di una barra dei record, né trascinare e rilasciare il record in un&#39;altra data quando le date di inizio e di fine scelte per il record sono di sola lettura. Ad esempio, l&#39;utilizzo di campi di ricerca o di formula per le date di inizio e di fine di un record non consente di ridimensionare o riposizionare il record in una visualizzazione calendario. <!--this also repeats in Considerations and in editing in the timeline view; also update there, if this changes-->

1. Fare clic sulla barra di un record per aprire l&#39;area dei dettagli e modificare tutti i campi.

   Per informazioni, vedere la sezione [Modificare un record dall&#39;anteprima del record in una visualizzazione](#edit-a-record-from-the-records-preview-in-a-view) in questo articolo.

### Modificare un record dall&#39;anteprima del record in una visualizzazione

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera modificare i record

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

1. In una visualizzazione di qualsiasi tipo, fare clic sul record

   Oppure

   Nella vista tabella fare clic sull&#39;icona **Apri dettagli** ![Apri dettagli nel campo nome tabella](assets/open-details-icon-in-table-name-field.png) nella prima colonna. L&#39;anteprima del record viene visualizzata nella vista.

   ![Casella Dettagli](assets/details-box.png)

1. (Facoltativo) Fai clic sul menu **Altro** a destra del titolo del record, quindi fai clic su **Rinomina**. Il campo visualizzato come titolo del record verrà aggiornato.

   Il titolo del record è il campo principale del record visualizzato in una vista a tabella. Per informazioni, vedere [Panoramica del campo primario](/help/quicksilver/planning/fields/primary-field-overview.md).

1. Inizia a modificare le informazioni del campo nell’anteprima del record.

   >[!TIP]
   >
   >  Non è possibile modificare le informazioni per i campi seguenti, in quanto sono di sola lettura e Workfront li aggiorna automaticamente:
   >  
   >  * Ricercare campi da altri record creati tramite la connessione di tipi di record. Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Campi dei tipi seguenti: Creato da, Data di creazione, Ultima modifica da, Data ultima modifica, Campi formula.

1. (Facoltativo) Fare clic su **Aggiungi copertina** per aggiungere una copertina al record. Per ulteriori informazioni, vedere [Aggiungere una copertina a un record](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

1. (Facoltativo) Passa il puntatore sull&#39;icona della miniatura, quindi fai clic su **Altro** ![Altro menu](assets/more-menu.png) > **Modifica miniatura** per aggiungere un&#39;immagine di miniatura. Per informazioni, vedere [Aggiungere una miniatura a un record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

   Workfront salva automaticamente le modifiche.

1. (Facoltativo) Fai clic sull&#39;**indicatore in tempo reale** ![icona indicatore in tempo reale](assets/real-time-indicator-icon.png) nell&#39;angolo superiore destro della casella di anteprima del record, quindi abilita l&#39;impostazione **Mostra collaboratori** per evidenziare i campi modificati in tempo reale da altri utenti.

   In quest’area vengono visualizzati i nomi e gli avatar di tutti gli utenti che accedono contemporaneamente al record.

   Quando l’impostazione è disattivata, gli avatar e i nomi sono elencati nell’area dell’indicatore in tempo reale e i campi in fase di modifica non vengono evidenziati.

   ![Indicatore di tempo reale: casella di anteprima record espansa](assets/real-time-indicator-expanded-record-preview-box.png)

1. (Facoltativo) Fai clic sull&#39;icona del menu **Esporta** ![Esporta nella pagina dei dettagli del record](assets/export-icon-in-record-details-page.png) per esportare i dettagli del record. Per informazioni, vedere [Esportare i dettagli di un record](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Facoltativo) Fai clic sull&#39;icona **Apri in una nuova scheda** ![Apri i dettagli in una nuova scheda](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> nell&#39;angolo superiore destro dell&#39;anteprima del record per aprire la pagina del record in una nuova scheda. Continua a modificare il record come descritto in [Modifica un record dalla sezione della pagina del record](#edit-a-record-from-the-records-page) in questo articolo.

### Modificare un record dalla pagina del record

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera modificare i record

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

1. Esegui una delle operazioni seguenti:

   * Da qualsiasi visualizzazione, accedere all&#39;anteprima del record come descritto nella sezione [Modificare un record dall&#39;anteprima del record in una visualizzazione](#edit-a-record-from-the-records-preview-in-a-view) di questo articolo, quindi fare clic sull&#39;icona **Apri in una nuova scheda** ![Apri i dettagli in una nuova scheda icona](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> nell&#39;angolo superiore destro dell&#39;anteprima del record per aprire la pagina del record in una nuova scheda.

   * Dalla visualizzazione **Tabella**, passa il puntatore sul nome di un record, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su **Visualizza**

     ![Menu contestuale per riga record](assets/contextual-menu-for-record-row.png)

     Viene visualizzata la pagina del record.

     ![Pagina dettagli](assets/details-page.png)

1. (Facoltativo) Fai clic sul menu **Altro** a destra del titolo del record, quindi fai clic su **Rinomina**. Il campo visualizzato come titolo del record verrà aggiornato.

   Il titolo del record è il campo principale del record visualizzato in una vista a tabella. Per informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

1. Fare clic su un campo modificabile nella pagina record per modificarlo.

   >[!TIP]
   >
   >  Non è possibile modificare le informazioni per i campi seguenti, in quanto sono di sola lettura e Workfront li aggiorna automaticamente:
   >  
   >  * Campi collegati creati mediante la connessione di tipi di record. Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Campi dei tipi seguenti: Creato da, Data di creazione, Ultima modifica da, Data ultima modifica, Campi formula.

1. (Facoltativo) Per visualizzare la descrizione di un campo, fai clic sull’icona delle informazioni a destra di qualsiasi campo visualizzato.
1. (Facoltativo) Fai clic su **Aggiungi copertina** per aggiungere una copertina al record

   Oppure

   Passa il puntatore del mouse sull&#39;immagine di copertina esistente, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) > **Carica** per aggiungere una nuova immagine di copertina per il record.

   Per ulteriori informazioni, vedere [Aggiungere una copertina a un record](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

1. (Facoltativo) Passa il puntatore del mouse su una miniatura esistente o sull&#39;**icona miniatura** ![icona Miniatura record nella pagina dei dettagli](assets/record-thumbnail-icon-on-details-page.png), quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) > **Modifica miniatura** per aggiungere una miniatura per il record.

   Per ulteriori informazioni, vedere [Aggiungere una miniatura a un record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

   Workfront salva automaticamente le modifiche.

1. (Facoltativo) Fai clic sull&#39;**indicatore in tempo reale** ![icona indicatore in tempo reale](assets/real-time-indicator-icon.png) nell&#39;angolo superiore destro della pagina del record, quindi abilita l&#39;impostazione **Mostra collaboratori** per evidenziare i campi modificati in tempo reale da altri utenti.

   In quest’area vengono visualizzati i nomi e gli avatar di tutti gli utenti che accedono contemporaneamente al record.

   Quando l’impostazione è disattivata, gli avatar e i nomi sono elencati nell’area dell’indicatore in tempo reale e i campi in fase di modifica non vengono evidenziati.

   ![Casella di anteprima record espanso indicatore in tempo reale](assets/real-time-indicator-expanded-record-preview-box.png)

1. (Facoltativo) Fai clic sull&#39;icona del menu **Esporta** ![Esporta nella pagina dei dettagli del record](assets/export-icon-in-record-details-page.png) per esportare i dettagli del record. Per informazioni, vedere [Esportare i dettagli di un record](/help/quicksilver/planning/records/export-the-record-page.md).


## Modificare un record da un oggetto Workfront nella sezione Planning

Dopo aver collegato i record agli oggetti di Workfront, è possibile modificare i record di Workfront Planning in Workfront dalla sezione Planning dell&#39;oggetto.

Per ulteriori informazioni, vedere [Gestire le connessioni record dagli oggetti Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

## Modifica le impostazioni dei campi a selezione singola o multipla durante l’aggiornamento dei relativi valori

<!--some of this information is also available in Edit fields article - update both when necessary-->

Quando si aggiornano le informazioni in un campo a selezione singola o multipla, è possibile aggiungere nuove scelte al campo senza dover modificare il campo.

>[!IMPORTANT]
>
>La funzionalità descritta in questa sezione è disponibile solo nella vista tabella. Non è disponibile in altre aree in cui vengono visualizzati campi a selezione singola o multipla.

**ESEMPIO**

È possibile che sia presente un campo a selezione singola denominato Stato con le opzioni Nuovo e Chiuso e che si desideri aggiungere una scelta per uno stato In corso. È possibile aggiungere la scelta eseguendo una delle operazioni seguenti:

* Modifica del campo. Per informazioni, vedere [Modifica campi](/help/quicksilver/planning/fields/edit-fields.md)
* Aggiunta di una nuova opzione durante la modifica del record nella vista tabella, come descritto di seguito.

Per aggiungere una nuova scelta a un campo di selezione esistente durante la modifica di un record:

1. Passare a una pagina del tipo di record e aprire la visualizzazione tabella.
1. Aggiungere come nuova colonna il campo a selezione singola o multipla a cui si desidera aggiungere una scelta nella vista a tabella. Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).
1. Inizia a modificare il campo in linea facendo doppio clic sulla cella del campo.
1. Digitare il nome della scelta che si desidera aggiungere, quindi fare clic su **Aggiungi scelta**.

   ![Aggiungi la scelta nel campo a selezione singola nella vista tabella](assets/add-choice-in-table-view-for-single-select-field.png)

   La nuova scelta viene aggiunta immediatamente al campo a selezione singola.

   <span class="preview">A ogni scelta viene aggiunto anche un nuovo valore. Puoi utilizzare i valori di scelta nelle chiamate API o in altre integrazioni. Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md). </span>

