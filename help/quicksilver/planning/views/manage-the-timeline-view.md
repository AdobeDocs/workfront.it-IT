---
title: Gestire la visualizzazione della timeline
description: Accedere e modificare i record in una vista timeline nella pagina Tipo di record di Adobe Workfront Planning. Personalizza la timeline con filtri, raggruppamenti e impostazioni. Utilizzare la funzione Raggruppamento per visualizzare i record connessi.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '2620'
ht-degree: 0%

---

# Gestire la visualizzazione della timeline

{{planning-important-intro}}

È possibile visualizzare i record in una vista timeline quando si accede alla pagina del tipo di record in Adobe Workfront Planning.

Per informazioni sulle visualizzazioni record, vedere [Gestione visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).

## Requisiti di accesso

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
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
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
   <p>Autorizzazioni di visualizzazione per modificare temporaneamente le impostazioni di visualizzazione</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello di layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--OLD: 

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
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->


## Gestire una vista timeline {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

Durante la creazione di una vista timeline, tutti i record del tipo di record selezionato vengono visualizzati in una timeline cronologica.

Considera quanto segue:

* È possibile creare una visualizzazione Sequenza temporale solo se a un tipo di record sono associati almeno due campi data. Se a un tipo di record è associato uno o nessun campo data, l&#39;opzione della visualizzazione Timeline non è disponibile.

  Durante la creazione di una vista timeline, puoi scegliere uno dei seguenti campi di data:

   * Registra date
   * Registra campi generati dal sistema: Data di creazione, Data ultima modifica
   * Ricercare date da tipi di oggetto o record connessi.
* A seconda delle date associate ai record, alcuni record potrebbero non essere visualizzati nella visualizzazione della sequenza temporale nei seguenti scenari:

   * Quando le date di inizio e fine non hanno valori
   * Quando le date di inizio o fine non hanno valore
   * Quando la data di inizio è successiva alla data di fine

Per gestire una vista timeline:

1. Passare alla pagina del tipo di record per la quale si desidera visualizzare la sequenza temporale.
1. Creare una visualizzazione timeline come descritto nell&#39;articolo [Gestire le visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   Per impostazione predefinita, i record associati al tipo di record selezionato vengono visualizzati come barre in un indicatore cronologico e ordinati in ordine cronologico rispetto alla data di inizio.

   >[!TIP]
   >
   >    L&#39;ordinamento dei record nella timeline non è visibile nella visualizzazione Compatta.

1. (Facoltativo e condizionale) Quando il nome del record viene troncato, posizionare il puntatore del mouse su una barra dei record per visualizzare il nome completo del record e le informazioni aggiuntive.

1. Per spostarsi nella timeline, effettuate una delle seguenti operazioni:

   * Fate clic sulle icone sinistra e destra oppure utilizzate lo scorrimento orizzontale per spostarvi avanti e indietro nella timeline. L’aggiornamento della pagina mantiene l’intervallo di tempo selezionato.
   * Fai clic su **Oggi** per centrare la timeline fino alla data odierna.
   * Per aggiornare gli incrementi di tempo, selezionate una delle seguenti opzioni dal menu a discesa intervallo di tempo:

      * Anno
      * Trimestre
      * Mese
1. Fai clic su **Passa alla visualizzazione Standard** per visualizzare i record in righe separate <!--check to see if they updated the name of the setting here-->

   Oppure

   Fare clic su **Passa alla visualizzazione compatta** per visualizzare i record le cui date non si intersecano sulla stessa riga. <!--check to see if they updated the name of the setting here-->

   I record vengono visualizzati nella visualizzazione Compatta per impostazione predefinita.

1. Per trovare rapidamente i record che corrispondono a una parola chiave, eseguire le operazioni seguenti:

   1. Fai clic sull&#39;icona **Ricerca** ![](assets/search-icon.png) e inizia a digitare una parola chiave associata a qualsiasi campo di un record visualizzato sullo schermo. Il numero di corrispondenze corrette viene visualizzato accanto all’elemento di ricerca e viene evidenziato il record con la corrispondenza corretta.

      ![](assets/search-box-and-results-timeline-view.png)

      È possibile utilizzare qualsiasi parola o carattere speciale visibile sullo schermo.

      Non è possibile utilizzare parole chiave associate a campi che non vengono visualizzati nella visualizzazione timeline.

   1. Premi Invio sulla tastiera per passare al successivo campo trovato.
   1. (Facoltativo) Se sono presenti più corrispondenze, fare clic sulle frecce su e giù a destra della parola chiave di ricerca per trovare tutte le corrispondenze nella tabella.
   1. Fare clic sull&#39;icona **x** nella casella di ricerca per deselezionare la parola chiave di ricerca.

1. Aggiornate i seguenti elementi della vista come descritto nelle sottosezioni seguenti:
   * [Filtri](#add-filters)
   * [Raggruppamento](#add-grouping)
   * [Impostazioni](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not yet in timeline; also check the anchor and make sure it's correct-->

1. (Facoltativo) Fai clic su **Raggruppamento** per visualizzare i record connessi nella timeline.

   Per informazioni, vedere la sezione [Utilizzare la funzionalità di raggruppamento per visualizzare i record connessi nella visualizzazione della sequenza temporale](#break-down-connected-records-in-the-timeline-view)

### Aggiungere filtri

È possibile ridurre la quantità di informazioni visualizzate sullo schermo utilizzando i filtri.

Quando si lavora con i filtri nella vista timeline, considera quanto segue:

<!-- this list is almost identical to the one for the table view - update both-->

* I filtri creati per una visualizzazione timeline funzionano in modo indipendente dai filtri di qualsiasi altra visualizzazione applicata allo stesso tipo di record.

* I filtri sono univoci per la vista selezionata. A due visualizzazioni timeline dello stesso tipo di record possono essere applicati filtri diversi.

* Due utenti che visualizzano la stessa visualizzazione timeline visualizzano lo stesso filtro attualmente applicato.

* Non è possibile assegnare un nome ai filtri creati per una vista timeline.

* Se si rimuovono i filtri, questi verranno rimossi da tutti coloro che accedono allo stesso tipo di record e che visualizzano la stessa visualizzazione.

* L’aggiunta di filtri nella vista timeline è identica all’aggiunta di filtri nella vista tabella.

  Per ulteriori informazioni, vedere la sezione &quot;Aggiungere filtri&quot; nell&#39;articolo [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

* È possibile filtrare in base ai campi record o ai campi di ricerca connessi.
* Puoi filtrare per campi di ricerca che visualizzano più valori.


### Aggiungi raggruppamento

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

È possibile raggruppare i record in base a informazioni simili quando si applica un raggruppamento a una visualizzazione.

L’aggiunta di raggruppamenti nella vista timeline è simile all’aggiunta di raggruppamenti nella vista tabella.

Quando si lavora con i raggruppamenti nella vista timeline, tenete presente quanto segue:

* Potete applicare i raggruppamenti sia nella vista tabella che nella vista timeline. I raggruppamenti della vista tabella sono indipendenti da quelli della vista timeline dello stesso tipo di record.
* È possibile applicare 3 livelli di raggruppamento in una visualizzazione. I record vengono raggruppati in base all&#39;ordine dei raggruppamenti selezionati.
&lt;!—* È possibile applicare fino a 4 livelli di raggruppamento quando si utilizza l’API. —controllare questo per il momento—>
* I raggruppamenti sono univoci per la vista selezionata. A due visualizzazioni tabella dello stesso tipo di record possono essere applicati raggruppamenti diversi. Due utenti che visualizzano la stessa vista tabella visualizzano lo stesso raggruppamento attualmente applicato.
* Non è possibile denominare i raggruppamenti creati per una vista tabella.
* Se si rimuovono i raggruppamenti, questi verranno rimossi da tutti coloro che accedono allo stesso tipo di record e che visualizzano la stessa visualizzazione.
* È possibile modificare i record elencati in un raggruppamento.
* È possibile eseguire il raggruppamento in base ai campi record o ai campi di ricerca connessi.
* Quando si esegue il raggruppamento per campi di ricerca con più valori (che non sono stati riepilogati da un aggregatore), i record vengono raggruppati per ogni combinazione univoca di valori di campo.
* È possibile fare riferimento a un campo fino a 4 livelli di distanza dal tipo di record corrente. Ad esempio, se si crea un raggruppamento per un tipo di record Attività e l&#39;attività è connessa al tipo di record Prodotto connesso al tipo di record Campagna connesso a un progetto Workfront, è possibile fare riferimento allo stato del progetto nel raggruppamento che si sta creando per il tipo di record Attività.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

Per aggiungere un raggruppamento nella vista timeline:

1. Creare una visualizzazione timeline per un tipo di record, come descritto nell&#39;articolo [Gestire le visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).
1. Fai clic su **Raggruppamento** nell&#39;angolo superiore destro della visualizzazione della timeline.

   ![](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. Fare clic su uno dei campi suggeriti oppure fare clic su **Scegli un campo diverso**, cerca un campo diverso e quindi fare clic su di esso quando viene visualizzato nell&#39;elenco.

   Il raggruppamento viene applicato automaticamente alla timeline e i record vengono visualizzati nella casella di raggruppamento.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Facoltativo) Ripeti i passaggi precedenti per aggiungere fino a 3 raggruppamenti.

   Il numero di campi selezionati per il raggruppamento viene visualizzato accanto all’icona Raggruppamento.

   <!-- update screen shot with view redesign-->

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Facoltativo) Nella casella **Raggruppa record per**, fai clic sull&#39;icona **x** a destra di un campo selezionato per il raggruppamento per rimuovere il raggruppamento

   Oppure

   Fare clic su **Cancella tutto** per rimuovere tutti i campi.

1. Fare clic all&#39;esterno della casella **Raggruppa record per** per chiuderla.
1. (Facoltativo) Fai clic su **Impostazioni**, quindi su **Colore** per impostare i raggruppamenti del codice colore. Per ulteriori informazioni, vedere la sezione [Modificare le impostazioni della visualizzazione della sequenza temporale](#edit-the-timeline-view-settings) in questo articolo.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Modificare le impostazioni della vista timeline {#edit-the-timeline-view-settings}

Aggiornate le impostazioni della vista timeline per indicare cosa e come vengono visualizzate le informazioni nella sezione timeline della vista.

1. Creare una visualizzazione timeline per un tipo di record, come descritto nell&#39;articolo [Gestire le visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).
1. Fare clic su **Impostazioni**.
1. Fai clic su **Data e ora** nel pannello a sinistra, quindi seleziona una **Data di inizio** e una **Data di fine** da visualizzare sulla timeline. È possibile scegliere le date di inizio e di fine predefinite oppure scegliere qualsiasi campo data disponibile. Le barre che rappresentano i record iniziano nella data indicata per la data di inizio e terminano nella data corrispondente alla data di fine.

   >[!NOTE]
   >
   >I record privi di valori per le date di inizio o di fine o con una data di inizio successiva alla data di fine non vengono visualizzati nella visualizzazione della sequenza temporale.

1. Fare clic su **Stile barra** nel pannello sinistro per indicare i campi da visualizzare sulle barre dei record.

   Il campo principale (o titolo) del record, come definito nella vista tabella del record, è selezionato per impostazione predefinita. <!--adjust this when the primary field is released??-->

1. (Facoltativo e condizionale) Se ai record sono state aggiunte miniature, selezionare l&#39;opzione Miniatura per visualizzare l&#39;immagine associata ai record nella barra dei record.

   >[!NOTE]
   >
   >    Prima di poter visualizzare le miniature nella vista timeline, dovete aggiungerle alla vista tabella. Per ulteriori informazioni, vedere [Aggiungere una miniatura a un record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. Fai clic su **Aggiungi campo** per aggiungere fino a 4 campi alle barre dei record.
1. Fare clic all&#39;interno della casella **Cerca campi** e selezionare il campo che si desidera aggiungere.

   >[!TIP]
   >
   >   * È necessario creare i campi prima di aggiungerli alle barre dei record.
   > 
   >   * È necessario selezionare almeno un campo. **Nome** è selezionato per impostazione predefinita.

   Sulla destra viene visualizzata un&#39;anteprima dell&#39;aspetto delle barre sulla timeline.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Fai clic su **Colore** nel pannello a sinistra per personalizzare i colori dei record e dei raggruppamenti nella timeline.

   ![](assets/color-tab-timeline-view.png)

1. (Condizionale e facoltativo) Se hai aggiunto un raggruppamento alla visualizzazione della timeline, seleziona una delle seguenti opzioni per impostare un colore per il raggruppamento nella sezione **Imposta colore di raggruppamento**:

   * **Predefinito (grigio)**: il colore dei raggruppamenti è impostato su grigio. Questa è l&#39;impostazione predefinita.
   * **Valori campo**: il colore dei raggruppamenti corrisponde al colore del campo in base al quale eseguire il raggruppamento.

     >[!NOTE]
     >
     >    * È possibile far corrispondere il colore solo ai campi con opzioni codificate per colore. Ad esempio, è possibile associare il colore ai campi Stato oppure ai campi con opzioni associate ai colori.
     >    
     >    * Non è possibile associare il colore ai campi di ricerca da tipi di record o oggetti collegati.


   Ad esempio, i campi a selezione multipla o a selezione singola possono avere opzioni codificate con colori.

   Se si raggruppa per campi senza opzioni codificate per colore, il colore di raggruppamento rimane grigio.

   >[!TIP]
   >
   >Se non hai aggiunto i raggruppamenti alla vista timeline, questa sezione non viene visualizzata.

1. Nella sezione **Imposta colore record** selezionare una delle opzioni seguenti per impostare un colore per i record:

   * **Tipo di record**: il colore dei record corrisponde al colore del tipo di record selezionato. Questa è l&#39;opzione predefinita.
   * **Valori campo**: il colore dei record corrisponde al colore di un campo specificato. Continuare con il passaggio 10. <!--ensure this stays accurate-->
   * **Raggruppamento**: il colore dei record corrisponde a quello indicato per i raggruppamenti. Questa opzione è disattivata se non avete applicato raggruppamenti alla vista timeline.
   * **Nessuno**: i record vengono visualizzati in una barra bianca.

1. (Condizionale) Se hai selezionato **Valori campo** per i colori del record, seleziona un campo dal menu a discesa **Corrispondenza colore del record con**.

   ![](assets/field-selector-drop-down-menu-timeline-view.png)

   Nel menu a discesa vengono visualizzati solo i campi con opzioni codificate a colori.

   Ad esempio, i campi a selezione multipla o a selezione singola possono avere opzioni codificate con colori.

   Se non si dispone di un campo con opzioni codificate a colori per il tipo di record selezionato, questa opzione viene disattivata.

1. Fai clic su **Salva**.

   I record vengono visualizzati nella vista timeline con le specifiche selezionate.

### Utilizzare la funzione Raggruppamento per visualizzare i record collegati nella vista timeline

È possibile visualizzare i record connessi nella visualizzazione della sequenza temporale di un record utilizzando la funzione Raggruppamento. La suddivisione dei record in base alle relative connessioni consente di visualizzare le timeline degli altri record connessi e di comprendere in che modo potrebbero influire sulle prestazioni e sulle scadenze dei record.

#### Considerazioni durante l’utilizzo della funzione di raggruppamento

* È possibile visualizzare i record o gli oggetti connessi sotto i record del tipo di record selezionato nella vista timeline.
* Utilizzando la funzione Raggruppamento (Breakdown), potete visualizzare quanto segue nella vista timeline:
   * Record di Workfront Planning connessi al tipo di record selezionato.
   * Tipi di oggetto Workfront o risorse di Experience Manager connesse al tipo di record selezionato.
   * Record di Workfront Planning o oggetti di un&#39;altra applicazione connessi a record connessi al tipo di record selezionato.

     Ad esempio, puoi collegare le campagne ai portfolio. Inoltre, è possibile collegare un altro tipo di record, prodotti, con progetti e con campagne. Quando crei la visualizzazione timeline della campagna, puoi suddividere le campagne per portfolio, prodotti e progetti.

* Non è possibile visualizzare tipi di oggetto connessi solo a oggetti di Workfront in Workfront, ma non connessi a un tipo di record di Workfront Planning. È possibile visualizzare solo gli oggetti o i tipi di record connessi in Workfront Planning.

  Le attività, ad esempio, sono collegate ai progetti in Workfront. La funzione Raggruppamento consente di visualizzare i progetti connessi alle campagne in Planning, ma non i task collegati ai progetti in Workfront.

  Se si desidera visualizzare sia i portafogli che i progetti nella visualizzazione della sequenza temporale di un tipo di record di Workfront Planning, è necessario che entrambi siano collegati al record di Planning o a un record connesso al record di Planning di cui si sta gestendo la visualizzazione della sequenza temporale.
* È possibile visualizzare solo i tipi di record associati ad almeno due campi data.
* I campi data per i tipi di record che si desidera visualizzare nella visualizzazione timeline devono essere visibili nella visualizzazione per tabella del tipo di record selezionato, come campi di ricerca.
* Le date di inizio e di fine dei tipi di record che si desidera visualizzare nella vista timeline devono essere in ordine cronologico. Ad esempio, se un record ha una data di inizio 31 gennaio e una data di fine 1 gennaio, non viene visualizzato nella visualizzazione della sequenza temporale. Per ulteriori informazioni, vedere la sezione [Gestire una visualizzazione della sequenza temporale](#manage-a-timeline-view) in questo articolo.
* È possibile includere nella suddivisione di un record un limite di 5 tipi di record.

#### Suddividere i record connessi nella visualizzazione timeline

1. Creare una visualizzazione timeline per un tipo di record, come descritto nell&#39;articolo [Gestire le visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).
1. (Condizionale) Se visualizzi la visualizzazione della sequenza temporale in modalità Standard, fai clic su **Raggruppamento**.
1. Espandere la casella **Selezionare un tipo di record collegato** e selezionare un tipo di record connesso. <!--add a new screen shot - submitted a bug to remove the "the"-->

   ![](assets/breakdown-picker-and-button-on-timeline.png)

   >[!TIP]
   >
   >    Se non si dispone di record connessi o se i record connessi non dispongono di almeno due campi data, la casella **Seleziona un tipo di record collegato** non è disponibile.

1. Scegli una **Data inizio** e un **Campo data fine**.

   >[!TIP]
   >
   >    Le date di inizio e di fine devono essere sequenziali. Se la data di fine è precedente alla data di inizio, nella sequenza temporale non verrà visualizzato alcun record.

   Una freccia rivolta a destra viene visualizzata sulla barra del record selezionato nella timeline, se sono collegati ad altri record.
1. Fare clic sulla freccia rivolta a destra per espandere un tipo di record e visualizzare le connessioni.

   ![](assets/campaigns-broken-down-by-programs-in-timeline-highlighted.png)

1. (Facoltativo) Ripeti i passaggi precedenti per aggiungere altri record connessi.



