---
title: Gestisci visualizzazioni record
description: È possibile visualizzare i record in una vista tabella, sequenza temporale o calendario quando si utilizza Adobe Workfront Planning. In questo articolo viene descritto come creare una visualizzazione e modificarne una esistente.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: a18b70b20e37f9751fbae2d4aad76e4905f976b2
workflow-type: tm+mt
source-wordcount: '1181'
ht-degree: 1%

---


# Gestire le visualizzazioni record

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

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
* [Attiva gli indicatori di presenza in tempo reale in una visualizzazione](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

Per ulteriori informazioni sulla gestione delle visualizzazioni record di Workfront Planning, vedere anche i seguenti articoli:

* [Eliminare le visualizzazioni record](/help/quicksilver/planning/views/delete-record-views.md)
* [Visualizzazioni record duplicate](/help/quicksilver/planning/views/duplicate-record-views.md)
* [Condividere le visualizzazioni](/help/quicksilver/planning/access/share-views.md)


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
<p>Qualsiasi pacchetto Workfront e Planning</p>
<p>Qualsiasi flusso di lavoro e qualsiasi pacchetto di Planning</p>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p> Standard per creare ed eliminare viste</p>
   <p>Collaboratore o versione successiva per aggiornare gli elementi di visualizzazione</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestire le autorizzazioni per una visualizzazione</p>  
   <p>Autorizzazioni di visualizzazione a una visualizzazione per modificare temporaneamente le impostazioni di visualizzazione o per duplicarla</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> Agli utenti con una licenza Light o Contributor deve essere assegnato un modello di layout che includa Planning.
   <p>Per impostazione predefinita, le aree Pianificazione sono attivate dagli utenti standard e dagli amministratori di sistema.</p></div></li></ul>
</td>
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
   <td><p> Standard to create and delete views</p>
   <p>Contributor or higher to update view elements</p>
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
   <td>   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings or to duplicate it</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>-->

## Considerazioni durante l&#39;utilizzo delle visualizzazioni record

* Le visualizzazioni in Workfront Planning sono specifiche per il tipo di record. Non è possibile applicare la stessa visualizzazione a due tipi di record diversi.
* Le visualizzazioni create sono visibili solo a te e agli utenti con cui condividi le visualizzazioni.
* Quando si modifica o si elimina una visualizzazione, questa viene modificata ed eliminata per tutti gli utenti che dispongono di autorizzazioni per la visualizzazione.
* Ogni utente può creare un massimo di 100 visualizzazioni. È possibile visualizzare più di 100 visualizzazioni per un tipo di record, ma un utente può creare solo 100 visualizzazioni.
* Anche se alcuni elementi di visualizzazione possono essere applicati a più viste per lo stesso record, essi sono univoci per ciascuna vista record:

   * Filtro
   * Ordina (per la vista tabella)
   * Colori riga (per la vista tabella)
   * Campi (per la vista tabella)
   * Raggruppamento (per la vista timeline)
   * Raggruppamento (per le viste tabella e timeline)
   * Aspetto della barra (per le visualizzazioni Timeline e Calendario)
   * Altezza riga (per la tabella e la visualizzazione calendario mensile)

  Ad esempio, quando si crea un filtro in una vista tabella, i risultati del filtro sono visibili solo nella vista selezionata (vista tabella) e non in tutte le viste associate al tipo di record.

  >[!TIP]
  >
  >Alcuni elementi della vista non sono disponibili per tutte le viste.


## Somiglianze e differenze tra le visualizzazioni record

La tabella seguente mostra le somiglianze e le differenze tra le viste tabella, timeline e calendario:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Funzione | Vista tabella | Vista timeline | Vista calendario |
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
| Raggruppa record | ✓ | ✓ |  |
| Ordinare i record | ✓ |              |  |
| Record codice colore | ✓ | ✓ | ✓ |
| Raggruppamenti di codici colore |           | ✓ |  |
| Cerca record specifici | ✓ | ✓ |  |
| Condividere la visualizzazione con altri utenti | ✓ | ✓ | ✓ |
| Aprire la pagina del record dalla visualizzazione | ✓ | ✓ |    |
| Visualizza record per anno e trimestre |           | ✓ |    |
| Visualizza i record per mese |           | ✓ | ✓ |
| Visualizza record per settimana |           |               | ✓ |
| Esportare informazioni da una vista | ✓ |               |    |
| Visualizza a schermo intero | ✓ | ✓ | ✓ |
| Crea record nella visualizzazione | ✓ | ✓ | ✓ |
| Suddividere i record in base alle relative connessioni |          | ✓ |    |

## Creare o modificare le viste {#create-or-edit-views}

{{step1-to-planning}}


1. Fai clic sulla scheda di un’area di lavoro.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

   Per impostazione predefinita, tutti i record del tipo selezionato vengono visualizzati nella vista tabella.

1. Fai clic sull&#39;icona a discesa ![Icona a discesa](assets/drop-down-icon.png) accanto al nome della visualizzazione corrente, quindi fai clic su **+Nuova visualizzazione**.

1. Selezionate uno dei seguenti tipi di vista:

   * Tabella
   * Timeline
   * Calendario

1. Scegli un tipo di visualizzazione, quindi fai clic su **Crea**. Viene aggiunta una nuova vista al menu a discesa.

   >[!TIP]
   >
   >Quando si crea un tipo di record, per impostazione predefinita viene creata anche la vista tabella.
   >
   >Per creare una visualizzazione timeline o calendario, il tipo di record per il quale viene creata la visualizzazione deve avere almeno due campi data.
   >
   >In caso contrario, le opzioni Timeline (Timeline) e Calendario (Calendar) vengono disattivate.
   >  

   ![Crea riquadro di visualizzazione](assets/create-view-box.png)

1. (Facoltativo) Per modificare una visualizzazione esistente, fai clic sul menu a discesa a destra del nome della visualizzazione corrente, quindi digita il nome di una visualizzazione nel campo **Cerca** e premi Invio sulla tastiera.
1. (Facoltativo) Dal menu a discesa della vista, trascina le viste in ordine di preferenza.

   ![Elenco a discesa dei tipi di visualizzazione dall&#39;elenco dei tipi di record](assets/view-types-drop-down-from-record-type-list.png)

1. (Condizionale) Fai clic su **Avanti** durante la creazione di una visualizzazione calendario o sequenza temporale.

   Per impostazione predefinita, Workfront assegna alla visualizzazione uno dei seguenti nomi:

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   Il numero è un incremento generato automaticamente.

1. (Condizionale) Seleziona **Inizio** e **Fine** per i record che verranno visualizzati nella visualizzazione Timeline o Calendario.

   >[!NOTE]
   >
   >    È possibile selezionare i campi della data di record o i campi della data di ricerca dai tipi di oggetto o record collegati.
   >
   >È necessario utilizzare gli aggregatori per i campi data (MAX o MIN) quando si selezionano i campi di ricerca durante la connessione dei tipi di record. Solo l&#39;aggiunta degli aggregatori consente di utilizzare le date delle connessioni come date di inizio e di fine per le visualizzazioni Timeline e Calendario.
   >
   >Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Fai clic su **Crea**.

   La vista viene visualizzata come una nuova scheda. Le visualizzazioni vengono visualizzate in ordine cronologico a partire dal momento in cui sono state create o condivise con te.
1. (Facoltativo) Fai clic sul menu **Altro** ![Altre visualizzazioni dell&#39;icona del punto di inserimento](assets/more-caret-down-icon-views.png) accanto all&#39;ultima visualizzazione per visualizzare tutte le visualizzazioni per il tipo di record selezionato.

   Visualizzazioni aggiuntive nel menu **Altro** dopo l&#39;ultima scheda della visualizzazione. Il numero accanto al menu **Altro** mostra il numero di visualizzazioni aggiuntive.
1. (Facoltativo) Per rinominare una visualizzazione dopo averla creata, fai clic sul menu a discesa Visualizza, quindi sul menu **Altro** ![Altro menu](assets/more-menu.png) > **Rinomina** per aggiornare il nome della visualizzazione

   Oppure

   Fare doppio clic sul nome della visualizzazione e iniziare a digitare il nuovo nome.  <!--ensure there is not another saving step here?!-->

1. (Facoltativo) Fai clic sull&#39;icona **Schermo intero** ![Icona Apri schermo intero](assets/open-full-screen-icon.png) per aprire una visualizzazione a schermo intero, quindi sull&#39;icona **Esci da schermo intero** ![Icona Esci da schermo intero](assets/exit-full-screen-icon.png) o su Esc nella tastiera per uscire dallo schermo intero.

1. (Facoltativo) Per gestire un tipo specifico di visualizzazione, vedi i seguenti articoli:

   * [Gestire la vista tabella](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [Gestire la visualizzazione della timeline](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [Gestire la visualizzazione calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md)

## Abilitare l&#39;indicatore di presenza in tempo reale in una visualizzazione

Per verificare se altri utenti stanno modificando i record contemporaneamente, seguire gli indicatori di presenza in tempo reale nella visualizzazione.

Per impostazione predefinita, nell&#39;angolo superiore destro di tutte le visualizzazioni record vengono visualizzati gli avatar di altri utenti che modificano le informazioni dei record contemporaneamente.

Quando si visualizza la vista tabella, è inoltre possibile visualizzare il campo che un altro utente sta modificando al momento della visualizzazione del record.

Per ulteriori informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).



<!--## Add a view as a favorite - this is not possible yet-->
