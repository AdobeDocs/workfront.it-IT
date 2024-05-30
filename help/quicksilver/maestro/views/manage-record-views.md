---
title: Gestire le visualizzazioni record
description: È possibile visualizzare i record in una vista tabella, sequenza temporale o calendario quando si utilizza Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 1%

---

# Gestire le visualizzazioni record

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Dopo aver selezionato un tipo di record nell&#39;area di Adobe Workfront Planning, è possibile visualizzare tutti i record di quel tipo nelle seguenti visualizzazioni:

* Tabella

  Per ulteriori informazioni, consulta [Gestire la vista tabella](../views/manage-the-table-view.md).

* Timeline

  Per ulteriori informazioni, consulta [Gestire la visualizzazione della timeline](../views/manage-the-timeline-view.md).

* Calendario

  Per ulteriori informazioni, consulta [Gestire la visualizzazione calendario](/help/quicksilver/maestro/views/manage-the-calendar-view.md).

Questo articolo descrive le seguenti informazioni sulle visualizzazioni record:

* [Creare e modificare una vista](#create-or-edit-record-views)
* [Eliminare una visualizzazione](#delete-views)
* [Duplicare una vista](#duplicate-views)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->


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
<p>La tua organizzazione deve essere iscritta al programma beta chiuso di Adobe Workfront Planning. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
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
   <p>Gli amministratori di sistema possono accedere solo alle visualizzazioni create o condivise con loro. </p>
  </td>
  </tr>

<tr>
   <td role="rowheader">Configurazione del livello di accesso</td>
   <td> <p>Nessun controllo del livello di accesso per Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestire le autorizzazioni per la visualizzazione</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Modello di layout</td>
   <td> <p>L'amministratore di sistema deve aggiungere l'area Planning nel modello di layout. Per informazioni, consulta <a href="../access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Considerazioni durante l&#39;utilizzo delle visualizzazioni record

* Le visualizzazioni in Workfront Planning sono specifiche per il tipo di record. Non è possibile applicare la stessa visualizzazione a due tipi di record diversi.
* Le visualizzazioni create sono visibili solo a te e agli utenti con cui condividi le visualizzazioni.
* Quando si modifica o si elimina una visualizzazione, questa viene modificata ed eliminata per tutti gli utenti che dispongono di autorizzazioni per la visualizzazione.
* Ogni utente può creare un massimo di 100 visualizzazioni. È possibile visualizzare più di 100 visualizzazioni per un tipo di record, ma un utente può creare solo 100 visualizzazioni.
* È possibile condividere con altri le viste create. Per informazioni, consulta [Condividere le visualizzazioni](/help/quicksilver/maestro/access/share-views.md).
* I seguenti elementi sono univoci per ogni visualizzazione record:

   * Filtro
   * Raggruppamento
   * Ordina
   * Aspetto barra (per la visualizzazione timeline)

  <!-- some of these are not available in all of the views - edit above-->

  Ad esempio, quando si crea un filtro in una visualizzazione tabella, i risultati del filtro sono visibili solo nella visualizzazione selezionata e non in tutte le visualizzazioni associate al tipo di record.

  >[!NOTE]
  >
  > Poiché Adobe Workfront Planning è attualmente in stato beta, alcuni elementi di visualizzazione potrebbero non essere disponibili per tutte le visualizzazioni.

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
| Aprire la pagina del record dalla visualizzazione | ✓ | ✓ |    |


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

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## Duplicare una vista

Se si desidera mantenere più versioni di una visualizzazione e apportare lievi modifiche tra le versioni, è possibile duplicare una visualizzazione.

La duplicazione di una vista crea copie identiche di una vista esistente.

Le autorizzazioni di condivisione della vista originale non vengono trasferite alla vista duplicata.

{{step1-to-maestro}}

Per impostazione predefinita, viene aperta l&#39;ultima area di lavoro a cui si è effettuato l&#39;accesso.

Per informazioni sulla creazione delle aree di lavoro, consulta [Creare aree di lavoro](../architecture/create-workspaces.md).

1. Fare clic su una scheda del tipo di record. Per informazioni sulla creazione di un tipo di record, vedere [Crea tipi di record](../architecture/create-record-types.md).

   Per impostazione predefinita, tutti i record del tipo selezionato vengono visualizzati nella vista tabella.

1. Posizionare il puntatore del mouse sulla scheda della visualizzazione da duplicare e fare clic sul pulsante **Altro** menu ![](assets/more-menu.png) a destra del nome della visualizzazione, quindi fai clic su **Duplica**.

   ![](assets/view-more-menu-with-duplicate-option.png)


   La vista viene duplicata e il nome della nuova vista segue il seguente pattern: `Original view's name (Copy)`. La nuova scheda vista viene visualizzata alla fine di tutte le schede vista.

