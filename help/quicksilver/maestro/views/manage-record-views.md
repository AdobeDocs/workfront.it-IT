---
title: Gestire le visualizzazioni record
description: È possibile visualizzare i record in una vista tabella, timeline o calendario quando si utilizzano le funzionalità di pianificazione di Adobe Workfront.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: b795ceccb3f72eb64269062823199be9c8511860
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 1%

---

# Gestire le visualizzazioni record

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

Dopo aver selezionato un tipo di record nell&#39;area delle funzionalità di pianificazione di Adobe Workfront, è possibile visualizzare tutti i record di quel tipo nelle seguenti viste:

* Tabella

  Per ulteriori informazioni, consulta [Gestire la vista tabella](../views/manage-the-table-view.md).

* Timeline

  Per ulteriori informazioni, consulta [Gestire la visualizzazione della timeline](../views/manage-the-timeline-view.md).

* Calendario

  Per ulteriori informazioni, consulta [Gestire la visualizzazione calendario](/help/quicksilver/maestro/views/manage-the-calendar-view.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
<p>La tua organizzazione deve essere iscritta al programma beta chiuso delle funzionalità di pianificazione di Adobe Workfront. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>piano Adobe Workfront</p></td>
   <td>
<p>Qualsiasi</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td>
   <td>
   <p>Qualsiasi</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Configurazione del livello di accesso</td>
   <td> <p>Non sono disponibili controlli del livello di accesso per le funzionalità di pianificazione di Workfront</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestire le autorizzazioni per la visualizzazione</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Modello di layout</td>
   <td> <p>L’amministratore di sistema deve aggiungere l’area Maestro nel modello di layout. Per informazioni, consulta <a href="../access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Considerazioni durante l&#39;utilizzo delle visualizzazioni record

* Le visualizzazioni nell&#39;area delle funzionalità di pianificazione di Workfront sono specifiche per il tipo di record. Non è possibile applicare la stessa visualizzazione a due tipi di record diversi.
* Le visualizzazioni create sono visibili solo a te e agli utenti con cui condividi le visualizzazioni.
* La creazione di viste per i tipi di record operativi è identica alla creazione di viste per i tipi di record della tassonomia.
* Quando si modifica o si elimina una visualizzazione, questa viene modificata ed eliminata per tutti gli utenti che dispongono di autorizzazioni per la visualizzazione.
* I seguenti elementi sono univoci per ogni visualizzazione record:

   * Filtro
   * Raggruppamento
   * Ordina

  <!-- some of these are not available in all of the views - edit above-->

  Ad esempio, quando si crea un filtro in una vista tabella, i risultati del filtro sono visibili solo nella vista selezionata e non in tutte le viste elencate nel menu a discesa Vista.

  >[!NOTE]
  >
  > Poiché le funzionalità di pianificazione di Adobe Workfront sono attualmente in stato beta, alcuni elementi della vista potrebbero non essere disponibili per tutte le viste.

Questo articolo descrive le seguenti informazioni sulle visualizzazioni record:

* [Creare e modificare una vista](#create-or-edit-record-views)
* [Eliminare una visualizzazione](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
* [Condividere una visualizzazione](#share-a-view)

## Somiglianze e differenze tra le visualizzazioni record

La tabella seguente mostra le somiglianze e le differenze tra le viste tabella, timeline e calendario:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Funzionalità | Vista tabella | Vista Timeline | Vista calendario |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| Visualizzare i record in un elenco o in una tabella | ✓ |              | |
| Visualizza tutti i campi come colonne nella tabella per impostazione predefinita | ✓ |              |    |
| Nascondere o mostrare campi o colonne | ✓ |               |    |
| Modifica i valori dei campi per ogni record | ✓ |               |             |
| Aggiungere record come nuove righe nella visualizzazione | ✓ |               |        |
| Aggiungere campi come nuove colonne nella visualizzazione | ✓ |               |         |
| Copiare le righe da un elenco esterno e incollarle in una tabella | ✓ |               |          |
| Visualizzare i record in una timeline |            | ✓ |             |
| Filtra record | ✓ | ✓ |           |
| Visualizzare i record in un calendario |           |              | ✓ |
| Raggruppa record | ✓ | ✓ |
| Ordinare i record | ✓ |              |
| Record codice colore |           | ✓ | ✓ |
| Raggruppamenti di codici colore |           | ✓ |
| Cerca record specifici | ✓ | ✓ |
| Condividi visualizzazione | ✓ | ✓ | ✓ |
| Aprire la pagina Dettagli del record dalla visualizzazione | ✓ | ✓ |    |


## Creare o modificare le viste {#create-or-edit-views}

{{step1-to-maestro}}


Per impostazione predefinita, viene aperta l&#39;ultima area di lavoro a cui si è effettuato l&#39;accesso. Per informazioni sulla creazione delle aree di lavoro, consulta [Creare aree di lavoro](../architecture/create-workspaces.md).

1. Fare clic su una scheda del tipo di record. Per informazioni sulla creazione di un tipo di record, vedere [Crea tipi di record](../architecture/create-record-types.md).

   Per impostazione predefinita, tutti i record del tipo selezionato vengono visualizzati nella vista tabella.

<!--
1. Click **+ View** to add a new view. 
1. Select from the following types of views: 

    * Table
    * Timeline
    * Calendar

    A new tab is created with the selected view. 

    Depending on the width of your screen, additional views might display in the **More** menu ![](assets/more-menu.png).   
-->

>[!TIP]
>
>Quando si crea un tipo di record, per impostazione predefinita viene creata anche la vista tabella.
>
>Per creare una visualizzazione timeline o calendario, il tipo di record per il quale viene creata la visualizzazione deve avere almeno due campi data. In caso contrario, le opzioni Timeline (Timeline) e Calendario (Calendar) vengono disattivate.
>

1. Fai clic su **Visualizza** e selezionare un menu a discesa esistente **Vista tabella** ![](assets/table-view-icon.png) o fai clic su **Crea vista > Tabella** per creare una vista tabella

   Oppure

   Seleziona un elemento esistente **Vista Timeline** ![](assets/timeline-view-icon.png) o fai clic su **Crea vista > Timeline** per creare una vista timeline.

   Oppure

   Seleziona un elemento esistente **Vista calendario** ![](assets/calendar-view-icon.png) o fai clic su **Crea vista > Calendario** per creare una vista calendario.

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    Per creare una visualizzazione timeline o calendario, il tipo di record per il quale viene creata la visualizzazione deve avere almeno due campi data. In caso contrario, le opzioni Timeline o Calendario risultano inattive.

1. (Condizionale) Fai clic su **Successivo**, durante la creazione di una visualizzazione timeline o calendario.

   Per impostazione predefinita, Workfront assegna alla visualizzazione uno dei seguenti nomi:

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   Il numero è un incremento generato automaticamente.

1. (Condizionale) Seleziona il **Inizio** e **Date di fine** per i record che verranno visualizzati nella visualizzazione timeline o calendario.
1. Fai clic su **Crea**.

   <!--add for view redesign: The view displays as a new tab. Views display in the chronological order from when they were created or shared with you. -->
<!--1. (Optional) Click the **More** menu ![](assets/more-caret-down-icon-views.png) next to the last view to view all views for the selected record type. 

    Additional views display under the **More** menu after the last view tab. The number next to the **More** menu shows the number of additional views. -->
1. (Facoltativo) Per rinominare una vista dopo la sua creazione, fai clic sul menu a discesa Vista, quindi fai clic su **Altro** menu ![](assets/more-menu.png) > **Rinomina** per aggiornare il nome della vista. <!--ensure there is not another saving step here?!-->
   <!--1. (Optional) To rename a view after it is created, double-click the view name and start typing the new name, or click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Rename**.-->
1. (Facoltativo) Per gestire un tipo specifico di visualizzazione, vedi i seguenti articoli:

   * [Gestire la vista tabella](../views/manage-the-table-view.md)
   * [Gestire la visualizzazione della timeline](../views/manage-the-timeline-view.md)
   * [Gestire la visualizzazione calendario](/help/quicksilver/maestro/views/manage-the-calendar-view.md)


## Eliminare le viste

{{step1-to-maestro}}

Per impostazione predefinita, viene aperta l&#39;ultima area di lavoro a cui si è effettuato l&#39;accesso. Per informazioni sulla creazione delle aree di lavoro, consulta [Creare aree di lavoro](../architecture/create-workspaces.md).

1. Fare clic su una scheda del tipo di record.

   Per informazioni sulla creazione di un tipo di record, vedere [Crea tipi di record](../architecture/create-record-types.md).

   Per impostazione predefinita, tutti i record del tipo selezionato vengono visualizzati nella vista tabella.

<!--1. Hover over one the of the view's names in the view tab, then click **More** ![](assets/more-menu.png) to the left of the view name, then click **Delete**. (********delete the instructions in the point below but keep the last step***********)
First, you might need to click **More** to the left of the last tab to find the view you want to delete. -->

1. Fai clic sul menu a discesa delle viste, passa il puntatore del mouse su una delle viste nell’elenco, quindi fai clic sul pulsante **Altro** menu ![](assets/more-menu.png) > **Elimina**.
1. Clic **Elimina** per confermare. <!--ensure there is not another saving step here?!-->

   La vista viene eliminata per tutti gli utenti che possono accedere all’area dei record e non può essere recuperata.

## Condividere una visualizzazione

Per informazioni sulla condivisione delle visualizzazioni, vedi [Condividere le visualizzazioni](/help/quicksilver/maestro/access/share-views.md).

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->
