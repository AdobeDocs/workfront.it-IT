---
title: Gestisci visualizzazioni record
description: È possibile visualizzare i record in una vista tabella, sequenza temporale o calendario quando si utilizza Adobe Workfront Planning. In questo articolo viene descritto come creare una visualizzazione e modificarne o eliminarne una esistente.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 3dfac5ada17248f5c67380b56b9a0969b10b73e6
workflow-type: tm+mt
source-wordcount: '1537'
ht-degree: 1%

---


# Gestire le visualizzazioni record

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Dopo aver selezionato un tipo di record nell&#39;area di Adobe Workfront Planning, è possibile visualizzare tutti i record di quel tipo nelle seguenti visualizzazioni:

* Tabella

  Per ulteriori informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

* Timeline

  Per ulteriori informazioni, vedere [Gestire la visualizzazione della sequenza temporale](/help/quicksilver/planning/views/manage-the-timeline-view.md).

* Calendario

  Per ulteriori informazioni, vedere [Gestire la visualizzazione del calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md).

Questo articolo descrive le seguenti informazioni sulle visualizzazioni record:

* [Creare e modificare una visualizzazione](#create-or-edit-record-views)
* [Eliminare una visualizzazione](#delete-views)
* [Duplicare una vista](#duplicate-views)
* [Attiva gli indicatori di presenza in tempo reale in una visualizzazione](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->


## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

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
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestire le autorizzazioni per una visualizzazione</p>  
   <p>Autorizzazioni di visualizzazione a una visualizzazione per modificare temporaneamente le impostazioni di visualizzazione o per duplicarla</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello layout</p></td> 
   <td> <p>Nell'ambiente di produzione, tutti gli utenti, inclusi gli amministratori di sistema, devono essere assegnati a un modello di layout che includa Planning.</p>
<p><span class="preview">Nell'ambiente di anteprima, per impostazione predefinita, Planning è abilitato per utenti standard e amministratori di sistema.</span></p></td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni durante l&#39;utilizzo delle visualizzazioni record

* Le visualizzazioni in Workfront Planning sono specifiche per il tipo di record. Non è possibile applicare la stessa visualizzazione a due tipi di record diversi.
* Le visualizzazioni create sono visibili solo a te e agli utenti con cui condividi le visualizzazioni.
* Quando si modifica o si elimina una visualizzazione, questa viene modificata ed eliminata per tutti gli utenti che dispongono di autorizzazioni per la visualizzazione.
* Ogni utente può creare un massimo di 100 visualizzazioni. È possibile visualizzare più di 100 visualizzazioni per un tipo di record, ma un utente può creare solo 100 visualizzazioni.
* È possibile condividere con altri le viste create. Per informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).
* I seguenti elementi sono univoci per ogni visualizzazione record:

   * Filtro
   * Raggruppamento
   * Ordina
   * Aspetto barra (per la visualizzazione timeline)

  <!-- some of these are not available in all of the views - edit above-->

  Ad esempio, quando si crea un filtro in una visualizzazione tabella, i risultati del filtro sono visibili solo nella visualizzazione selezionata e non in tutte le visualizzazioni associate al tipo di record.

  >[!NOTE]
  >
  > Alcuni elementi della vista potrebbero non essere disponibili per tutte le viste.


## Somiglianze e differenze tra le visualizzazioni record

La tabella seguente mostra le somiglianze e le differenze tra le viste tabella, timeline e calendario:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Funzionalità | Vista tabella | Vista timeline | Vista calendario |
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
| Condividere la visualizzazione con altri utenti | ✓ | ✓ | ✓ |
| Aprire la pagina del record dalla visualizzazione | ✓ | ✓ |    |
| Visualizza record per anno e trimestre |           | ✓ |    |
| Visualizza i record per mese |           | ✓ | ✓ |
| Visualizza record per settimana |           |               | ✓ |


## Creare o modificare le viste {#create-or-edit-views}

{{step1-to-planning}}


1. Fai clic sulla scheda di un’area di lavoro.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

   Per impostazione predefinita, tutti i record del tipo selezionato vengono visualizzati nella vista tabella.

1. Fare clic su **+ Visualizzazione** per aggiungere una nuova visualizzazione.
1. Selezionate uno dei seguenti tipi di vista:

   * Tabella
   * Timeline
   * Calendario

   Viene creata una nuova scheda con la vista selezionata.

   A seconda della larghezza dello schermo, nel menu **Altro** ![Altro](assets/more-menu.png) potrebbero essere visualizzate altre visualizzazioni.


>[!TIP]
>
>Quando si crea un tipo di record, per impostazione predefinita viene creata anche la vista tabella.
>
>Per creare una visualizzazione timeline o calendario, il tipo di record per il quale viene creata la visualizzazione deve avere almeno due campi data.
>
>In caso contrario, le opzioni Timeline (Timeline) e Calendario (Calendar) vengono disattivate.
>

![Elenco a discesa dei tipi di visualizzazione dall&#39;elenco dei tipi di record](assets/view-types-drop-down-from-record-type-list.png)

1. (Condizionale) Fai clic su **Avanti** durante la creazione di una visualizzazione calendario o sequenza temporale.

   Per impostazione predefinita, Workfront assegna alla visualizzazione uno dei seguenti nomi:

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   Il numero è un incremento generato automaticamente.

1. (Condizionale) Seleziona **Inizio** e **Fine** per i record che verranno visualizzati nella visualizzazione Timeline o Calendario.

   >[!TIP]
   >
   >    È possibile selezionare i campi della data di record o i campi della data di ricerca dai tipi di oggetto o record collegati. È necessario utilizzare gli aggregatori per i campi data (MAX o MIN) quando si selezionano i campi di ricerca come date di inizio e di fine per le visualizzazioni Timeline e Calendario. Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Fai clic su **Crea**.

   La vista viene visualizzata come una nuova scheda. Le visualizzazioni vengono visualizzate in ordine cronologico a partire dal momento in cui sono state create o condivise con te.
1. (Facoltativo) Fai clic sul menu **Altro** ![Altre visualizzazioni dell&#39;icona del punto di inserimento](assets/more-caret-down-icon-views.png) accanto all&#39;ultima visualizzazione per visualizzare tutte le visualizzazioni per il tipo di record selezionato.

   Visualizzazioni aggiuntive nel menu **Altro** dopo l&#39;ultima scheda della visualizzazione. Il numero accanto al menu **Altro** mostra il numero di visualizzazioni aggiuntive.
1. (Facoltativo) Per rinominare una visualizzazione dopo averla creata, fai clic sul menu a discesa Visualizza, quindi sul menu **Altro** ![Altro menu](assets/more-menu.png) > **Rinomina** per aggiornare il nome della visualizzazione

   Oppure

   Fare doppio clic sul nome della visualizzazione e iniziare a digitare il nuovo nome.  <!--ensure there is not another saving step here?!-->

1. (Facoltativo) Per gestire un tipo specifico di visualizzazione, vedi i seguenti articoli:

   * [Gestire la vista tabella](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [Gestire la visualizzazione della timeline](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [Gestire la visualizzazione calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md)


## Eliminare le viste

{{step1-to-planning}}

1. Fai clic sulla scheda di un’area di lavoro.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

   Per impostazione predefinita, tutti i record del tipo selezionato vengono visualizzati nella vista tabella.

1. Passa il puntatore del mouse su uno dei nomi della visualizzazione nella scheda della visualizzazione, quindi fai clic su **Altro** ![Altro menu](assets/more-menu.png) a sinistra del nome della visualizzazione, quindi fai clic su **Elimina**.
Per trovare la visualizzazione da eliminare, potrebbe essere necessario fare clic su **Altro** a sinistra dell&#39;ultima scheda.

1. Fai clic su **Elimina** per confermare. <!--ensure there is not another saving step here?!-->

   La vista viene eliminata per tutti gli utenti che possono accedere all’area dei record e non può essere recuperata.

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## Duplicare una vista

Se si desidera mantenere più versioni di una visualizzazione e apportare lievi modifiche tra le versioni, è possibile duplicare una visualizzazione.

La duplicazione di una vista crea copie identiche di una vista esistente.

Le autorizzazioni di condivisione della vista originale non vengono trasferite alla vista duplicata.

{{step1-to-planning}}

1. Fai clic sulla scheda di un’area di lavoro.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.
Per impostazione predefinita, tutti i record del tipo selezionato vengono visualizzati nella vista tabella.

1. Passa il puntatore del mouse sulla scheda della visualizzazione da duplicare e fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome della visualizzazione, quindi fai clic su **Duplica**.

   ![Visualizza altro menu con opzione duplicata](assets/view-more-menu-with-duplicate-option.png)


   La visualizzazione è duplicata e il nome della nuova visualizzazione segue il seguente schema: `Original view's name (Copy)`. La nuova scheda vista viene visualizzata alla fine di tutte le schede vista.

## Abilitare l&#39;indicatore di presenza in tempo reale in una visualizzazione

Per impostazione predefinita, nell&#39;angolo superiore destro di tutte le visualizzazioni record vengono visualizzati gli avatar di altri utenti che modificano le informazioni dei record contemporaneamente.

Quando si visualizza la vista tabella, è inoltre possibile visualizzare il campo che un altro utente sta modificando al momento della visualizzazione del record.

1. Passare a una pagina del tipo di record e aprire qualsiasi visualizzazione.
1. (Condizionale) Se altri utenti modificano contemporaneamente i record del tipo selezionato, i relativi avatar vengono visualizzati nell’angolo superiore destro della visualizzazione.
1. Fai clic sul menu a discesa accanto agli avatar, quindi seleziona l&#39;opzione **Mostra collaboratori**. L’opzione è selezionata per impostazione predefinita.

   ![Mostra/nascondi collaboratori selezionati](assets/show-collaborators-toggle-selected.png)

1. (Facoltativo) Apri una vista a tabella e il campo che un’altra persona sta modificando attivamente viene evidenziato nel colore corrispondente al contorno del proprio avatar nella vista a tabella.

   Se il colore di evidenziazione dell’avatar è grigio, l’utente ha interrotto la modifica attiva del record più di 30 secondi fa.

   ![Campo tabella indicatori in tempo reale e connessione avatar](assets/real-time-indicator-table-field-and-avatar-connection.png)

   >[!TIP]
   >
   >È possibile selezionare l&#39;opzione **Mostra collaboratori** da qualsiasi visualizzazione. Il campo attualmente modificato da altri utenti è evidenziato solo nella vista tabella.
