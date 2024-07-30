---
title: Modifica record
description: È possibile modificare le informazioni del record in Adobe Workfront Planning. È necessario creare i tipi di record prima di iniziare a creare e modificare i record.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '1711'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Modifica record

{{planning-important-intro}}

È possibile modificare le informazioni sui record in Adobe Workfront Planning modificando i valori dei campi associati ai record.

È necessario creare i tipi di record prima di iniziare a creare e modificare i record.

Per informazioni, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

Per informazioni sulla creazione di record, vedere [Crea record](/help/quicksilver/planning/records/create-records.md).

&lt;!— menziona qui che i campi nella visualizzazione Dettagli sono gli stessi di quelli nella visualizzazione tabella — questo articolo è collegato da Gestisci visualizzazioni record uno per fare riferimento a queste informazioni—>

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per Workfront Planning.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Prodotto</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>L'organizzazione deve essere iscritta alla fase di accesso anticipato per Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>piano Adobe Workfront</p></td>
   <td>
<p>Qualsiasi</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td>
   <td>
   <p>Nuovo: Standard</p>
   Oppure
   <p>Corrente: Piano</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td>
   <td> <p>Nessun controllo di accesso per Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Autorizzazioni Contribute o superiori per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L'amministratore del Workfront o del gruppo deve aggiungere l'area Planning nel modello di layout. Per informazioni, vedere <a href="/help/quicksilver/planning/access/access-overview.md">Panoramica dell'accesso</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sulla modifica dei record

* Se si dispone delle autorizzazioni necessarie per l&#39;area di lavoro, è possibile modificare i record creati o quelli creati da altri utenti.
* È possibile modificare i campi record dalle seguenti aree:

   * Anteprima del record in una visualizzazione record
   * Pagina del record
   * In linea, in una vista a tabella.

* Quando un utente modifica un record in una visualizzazione, le modifiche sono immediatamente visibili in tutte le visualizzazioni e le pagine dei record a tutti gli altri utenti.

* I seguenti tipi di campi vengono aggiornati automaticamente e non è possibile modificarne i valori manualmente:
   * Campi collegati da altri record
   * Campi di tipo formula
   * Campi di sistema (Creato da, Data di creazione, Autore ultima modifica, Data ultima modifica)
* Se i record visualizzati sono collegati ad altri record, le nuove informazioni dei record che si sta modificando verranno applicate ai record collegati.
* Non è possibile modificare i record in blocco. <!--this will probably change-->
* Gli URL vengono riconosciuti come collegamenti nei tipi di campi di testo a riga singola solo quando iniziano con: http://, https://, ftp:// o www. .
* È possibile aggiungere un&#39;immagine di copertina a ogni record. L&#39;immagine è univoca per ogni record e non si applica a tutti i record contemporaneamente.
* È possibile modificare l&#39;ordine dei campi in una pagina record e aggiungere un&#39;immagine di copertina per un record. Per ulteriori informazioni, vedere [Gestire il layout della pagina record](/help/quicksilver/planning/records/manage-the-record-page.md).

## Modifica record

È possibile modificare un record dalle seguenti aree:

* [Dalla vista tabella di un tipo di record](#edit-a-record-inline-in-the-table-view-of-a-record-type)
* [Dall&#39;anteprima del record in una visualizzazione](#edit-a-record-from-the-records-preview-in-a-view)
* [Dalla pagina del record](#edit-a-record-from-the-records-page)
* [Da un oggetto Workfront nella sezione Planning](#edit-a-record-from-a-workfront-object-in-the-planning-section)

### Modificare un record in linea nella vista tabella di un tipo di record

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera modificare i record

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.
1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.
1. (Condizionale) Fare clic sulla scheda di una visualizzazione tabella oppure fare clic su **+ Visualizzazione** per creare una visualizzazione tabella. La vista tabella deve essere quella predefinita, a meno che il tipo di record non sia stato visualizzato in un altro tipo di vista all&#39;ultimo accesso.

   I record associati al tipo di record selezionato vengono visualizzati nella vista tabella.
1. Fare clic all&#39;interno della riga di un record per iniziare a modificare le informazioni sul record in linea.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!TIP]
   >
   >  Non è possibile modificare le informazioni per i campi seguenti, in quanto sono di sola lettura e Workfront li aggiorna automaticamente:
   >  
   >  * Campi collegati creati mediante la connessione di tipi di record. Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Campi dei tipi seguenti: Creato da, Data di creazione, Ultima modifica da, Data ultima modifica, Campi formula.

1. (Facoltativo e condizionale) Quando modifichi un campo di tipo Paragrafo, utilizza le seguenti **opzioni di formattazione Rich Text**:

   * Bold
   * Italic
   * Sottolinea
   * Aggiungi un collegamento
   * Aggiungere un elenco puntato
   * Aggiungere un elenco numerato

   ![](assets/rich-text-toolbar-on-paragraph-field.png)

1. (Facoltativo) Fare doppio clic su un campo record connesso per aggiungere record o oggetti connessi a un altro record. Per ulteriori informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).
1. Premi **Invio** sulla tastiera o fai clic all&#39;esterno di una riga per salvare le modifiche. Le modifiche vengono salvate automaticamente. Un indicatore **Salvato** viene visualizzato brevemente nell&#39;angolo superiore destro della visualizzazione tabella per indicare che le modifiche sono state salvate.


1. (Facoltativo) Per copiare e incollare informazioni da un campo all&#39;altro, effettuare una delle seguenti operazioni:

   * Copiare uno o più valori esistenti di un campo, quindi incollarli in un campo dello stesso tipo in un altro record
   * Fare clic sull&#39;intestazione di una colonna per selezionarla e copiarla, quindi fare clic sull&#39;intestazione di un&#39;altra colonna e incollare il contenuto della colonna copiata. Le colonne devono contenere tipi di campo simili.
   * Con il tasto Maiusc premuto, fai clic su per selezionare più righe in una tabella, copia le informazioni nelle righe selezionate, quindi fai clic su una riga diversa e incolla le informazioni selezionate nella nuova riga e nelle righe successive.
   * Copiare le informazioni da una cella, quindi selezionare più celle e incollare le stesse informazioni in più celle. È possibile selezionare più celle e incollare le stesse informazioni in più celle da righe e colonne adiacenti.
   * Selezionare l&#39;angolo inferiore destro di una cella esistente contenente le informazioni da copiare, quindi trascinarlo e rilasciarlo nelle celle adiacenti in cui si desidera incollare le stesse informazioni. Tutte le celle devono contenere lo stesso tipo di informazioni.

     ![](assets/dragable-lower-right-corner-for-copy-paste-in-table-view.png)

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
   >
   >    * Campi collegati (o campi di ricerca) creati mediante la connessione di tipi di record. È possibile copiare e incollare campi record collegati. Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).
   >    * Campi dei seguenti tipi: Creato da, Data di creazione, Ultima modifica da, Data ultima modifica

1. (Facoltativo) Utilizzare le seguenti scelte rapide da tastiera per annullare o ripetere la modifica o la copia e l&#39;incollamento delle informazioni del record:

   * CTRL + Z (⌘ + Z per Mac) per annullare una modifica
   * CTRL + MAIUSC + Z (⌘ + MAIUSC + Z per Mac) per ripetere una modifica

   >[!TIP]
   >
   >    È possibile utilizzare più volte le scelte rapide da tastiera in una riga per annullare più modifiche.

1. (Facoltativo) Aggiungi una miniatura a un record. Per informazioni, vedere [Aggiungere una miniatura a un record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

### Modificare un record dall&#39;anteprima del record in una visualizzazione

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera modificare i record

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

1. In una visualizzazione di qualsiasi tipo, fare clic sul record

   Oppure

   Nella vista tabella fare clic sull&#39;icona ![](assets/open-details-icon-in-table-name-field.png) **Apri dettagli** nella prima colonna. L&#39;anteprima del record viene visualizzata nella vista.

   ![](assets/details-box.png)

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

1. (Facoltativo) Passa il puntatore sull&#39;icona della miniatura, quindi fai clic su **Altro** ![](assets/more-menu.png) > **Modifica miniatura** per aggiungere un&#39;immagine di miniatura. Per informazioni, vedere [Aggiungere una miniatura a un record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

   Workfront salva automaticamente le modifiche.

1. (Facoltativo) Fai clic sull&#39;icona **Apri in una nuova scheda** ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> nell&#39;angolo superiore destro dell&#39;anteprima del record per aprire la pagina del record in una nuova scheda. Continua a modificare il record come descritto in [Modifica un record dalla sezione della pagina del record](#edit-a-record-from-the-records-page) in questo articolo.

### Modificare un record dalla pagina del record

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera modificare i record

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

1. Esegui una delle operazioni seguenti:

   * Da qualsiasi visualizzazione, accedere all&#39;anteprima del record come descritto nella sezione [Modificare un record dall&#39;anteprima del record in una visualizzazione](#edit-a-record-from-the-records-preview-in-a-view) in questo articolo, quindi fare clic sull&#39;icona **Apri in una nuova scheda** ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> nell&#39;angolo superiore destro dell&#39;anteprima del record per aprire la pagina del record in una nuova scheda.

   * Dalla visualizzazione **Tabella**, passa il puntatore del mouse sul nome di un record, quindi fai clic sul menu **Altro** ![](assets/more-menu.png), quindi fai clic su **Visualizza**

     ![](assets/contextual-menu-for-record-row.png)

     Viene visualizzata la pagina del record.

     ![](assets/details-page.png)

1. (Facoltativo) Fai clic sul menu **Altro** a destra del titolo del record, quindi fai clic su **Rinomina**. Il campo visualizzato come titolo del record verrà aggiornato.

   Il titolo del record è il campo principale del record visualizzato in una vista a tabella. Per informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

1. Fare clic su un campo modificabile nella pagina record per modificarlo.

   >[!TIP]
   >
   >  Non è possibile modificare le informazioni per i campi seguenti, in quanto sono di sola lettura e Workfront li aggiorna automaticamente:
   >  
   >  * Campi collegati creati mediante la connessione di tipi di record. Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Campi dei tipi seguenti: Creato da, Data di creazione, Ultima modifica da, Data ultima modifica, Campi formula.

1. (Facoltativo) Fai clic su **Aggiungi copertina** per aggiungere una copertina al record

   Oppure

   Passa il puntatore del mouse sull&#39;immagine di copertina esistente, quindi fai clic sul menu **Altro** ![](assets/more-menu.png) > **Carica** per aggiungere una nuova immagine di copertina per il record.

   Per ulteriori informazioni, vedere [Aggiungere una copertina a un record](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

1. (Facoltativo) Passa il puntatore del mouse su una miniatura esistente o sull&#39;**icona miniatura** ![](assets/record-thumbnail-icon-on-details-page.png), quindi fai clic sul menu **Altro** ![](assets/more-menu.png) > **Modifica miniatura** per aggiungere una miniatura per il record.

   Per ulteriori informazioni, vedere [Aggiungere una miniatura a un record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

   Workfront salva automaticamente le modifiche.

## Modificare un record da un oggetto Workfront nella sezione Planning

Dopo aver collegato i record agli oggetti di Workfront, è possibile modificare i record di Workfront Planning in Workfront dalla sezione Planning dell&#39;oggetto.

Per ulteriori informazioni, vedere [Gestire i record nella sezione Pianificazione degli oggetti Adobe Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).