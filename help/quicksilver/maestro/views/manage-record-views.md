---
title: Gestire le visualizzazioni record
description: È possibile visualizzare i record in una vista tabella, timeline o calendario quando si utilizzano le funzionalità di pianificazione di Adobe Workfront.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: e881aa57b5175ce5b559180a2713de0c607b3b1d
workflow-type: tm+mt
source-wordcount: '949'
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
| Filtra record | ✓ | ✓ | ✓ |
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

1. Clic **+ Visualizza** per aggiungere una nuova visualizzazione.
1. Selezionate uno dei seguenti tipi di vista:

   * Tabella
   * Timeline
   * Calendario

   Viene creata una nuova scheda con la vista selezionata.

   A seconda della larghezza dello schermo, è possibile che nella **Altro** menu ![](assets/more-menu.png).


>[!TIP]
>
>Quando si crea un tipo di record, per impostazione predefinita viene creata anche la vista tabella.
>
>Per creare una visualizzazione timeline o calendario, il tipo di record per il quale viene creata la visualizzazione deve avere almeno due campi data. In caso contrario, le opzioni Timeline (Timeline) e Calendario (Calendar) vengono disattivate.
>

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

   La vista viene visualizzata come una nuova scheda. Le visualizzazioni vengono visualizzate in ordine cronologico a partire dal momento in cui sono state create o condivise con te.
1. (Facoltativo) Fai clic su **Altro** menu ![](assets/more-caret-down-icon-views.png) accanto all&#39;ultima visualizzazione per visualizzare tutte le visualizzazioni per il tipo di record selezionato.

   Visualizzazioni aggiuntive sotto **Altro** dopo l&#39;ultima scheda di visualizzazione. Il numero accanto al **Altro** mostra il numero di visualizzazioni aggiuntive.
1. (Facoltativo) Per rinominare una vista dopo la sua creazione, fai clic sul menu a discesa Vista, quindi fai clic su **Altro** menu ![](assets/more-menu.png) > **Rinomina** per aggiornare il nome della vista

   Oppure

   Fare doppio clic sul nome della visualizzazione e iniziare a digitare il nuovo nome.  <!--ensure there is not another saving step here?!-->

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

1. Passa il puntatore del mouse su uno dei nomi della vista nella scheda vista, quindi fai clic su **Altro** ![](assets/more-menu.png) a sinistra del nome della visualizzazione, quindi fai clic su **Elimina**.
Innanzitutto, potrebbe essere necessario fare clic su **Altro** a sinistra dell&#39;ultima scheda per trovare la vista da eliminare.

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
