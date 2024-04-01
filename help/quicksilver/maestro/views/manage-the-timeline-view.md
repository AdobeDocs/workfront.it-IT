---
title: Gestire la visualizzazione della timeline
description: È possibile visualizzare i record in una vista timeline quando si accede alla pagina del tipo di record in Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: 7fe24704cead460762322b4f26bf37431e9744ca
workflow-type: tm+mt
source-wordcount: '1714'
ht-degree: 0%

---

# Gestire la visualizzazione della timeline

<!--
title: Manage the timeline view in Adobe Maestro
description: You can display records in a timeline view, when accessing the record type page in Adobe Maestro. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

È possibile visualizzare i record in una vista timeline quando si accede alla pagina del tipo di record in Adobe Workfront Planning.

Per informazioni sulle visualizzazioni record, vedere [Gestire le visualizzazioni record](../views/manage-record-views.md).

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
<p>La tua organizzazione deve essere iscritta al programma beta di Adobe Workfront Planning. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
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
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning </p>  
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


## Gestire una vista timeline {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

Durante la creazione di una vista timeline, tutti i record del tipo di record selezionato vengono visualizzati in una timeline cronologica.

Considera quanto segue:

* È possibile creare una visualizzazione Sequenza temporale solo se a un tipo di record sono associati almeno due campi data. Se a un tipo di record è associato uno o nessun campo data, l&#39;opzione della visualizzazione Timeline non è disponibile.
* A seconda delle date associate ai record, alcuni record potrebbero non essere visualizzati nella visualizzazione della sequenza temporale nei seguenti scenari:

   * Quando le date di inizio e fine non hanno valori
   * Quando le date di inizio o fine non hanno valore
   * Quando la data di inizio è successiva alla data di fine

Per gestire una vista timeline:

1. Passare alla pagina del tipo di record per la quale si desidera visualizzare la sequenza temporale.
1. Creare una visualizzazione timeline come descritto nell’articolo [Gestire le visualizzazioni record](../views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   Per impostazione predefinita, i record associati al tipo di record selezionato vengono visualizzati come barre in un indicatore cronologico e ordinati in ordine cronologico rispetto alla data di inizio.

   >[!TIP]
   >
   >    L&#39;ordinamento dei record nella timeline non è visibile nella visualizzazione Compatta.


1. Per spostarsi nella timeline, effettuate una delle seguenti operazioni:

   * Fate clic sulle icone sinistra e destra oppure utilizzate lo scorrimento orizzontale per spostarvi avanti e indietro nella timeline.
   * Clic **Oggi** per centrare la timeline fino alla data odierna.
   * Per aggiornare gli incrementi di tempo, selezionate una delle seguenti opzioni dal menu a discesa intervallo di tempo:

      * Anno
      * Trimestre
      * Mese
1. Clic **Passa a Standard** visualizzazione per visualizzare i record in righe separate <!--check to see if they updated the name of the setting here-->

   Oppure

   Clic **Passa alla visualizzazione Compatta** per visualizzare i record le cui date non si intersecano sulla stessa riga. <!--check to see if they updated the name of the setting here-->

   I record vengono visualizzati nella visualizzazione Compatta per impostazione predefinita.

1. Per trovare rapidamente i record che corrispondono a una parola chiave, eseguire le operazioni seguenti:

   1. Fai clic su **Ricerca** icona ![](assets/search-icon.png) e iniziare a digitare una parola chiave associata a qualsiasi campo di un record visualizzato sullo schermo. Il numero di corrispondenze corrette viene visualizzato accanto all’elemento di ricerca e viene evidenziato il record con la corrispondenza corretta.

      ![](assets/search-box-and-results-timeline-view.png)

      È possibile utilizzare qualsiasi parola o carattere speciale visibile sullo schermo.

      Non è possibile utilizzare parole chiave associate a campi che non vengono visualizzati nella visualizzazione timeline.

   1. Premi Invio sulla tastiera per passare al successivo campo trovato.
   1. (Facoltativo) Se sono presenti più corrispondenze, fare clic sulle frecce su e giù a destra della parola chiave di ricerca per trovare tutte le corrispondenze nella tabella.
   1. Fai clic su **x** nella casella di ricerca per deselezionare la parola chiave di ricerca.

1. Aggiornate i seguenti elementi della vista come descritto nelle sottosezioni seguenti:
   * [Filtri](#add-filters)
   * [Raggruppamento](#add-grouping)
   * [Impostazioni](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->

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

  Per ulteriori informazioni, consulta la sezione &quot;Aggiungere filtri&quot; nell’articolo [Gestire la vista tabella](../views/manage-the-table-view.md).

* È possibile filtrare in base ai campi record o ai campi di ricerca connessi, ma non per i campi che consentono il collegamento a più record.

### Aggiungi raggruppamento

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

È possibile raggruppare i record in base a informazioni simili quando si applica un raggruppamento a una visualizzazione.

L’aggiunta di raggruppamenti nella vista timeline è simile all’aggiunta di raggruppamenti nella vista tabella.

Quando si lavora con i raggruppamenti nella vista timeline, tenete presente quanto segue:

* Potete applicare i raggruppamenti sia nella vista tabella che nella vista timeline. I raggruppamenti della vista tabella sono indipendenti da quelli della vista timeline dello stesso tipo di record.
* È possibile applicare 3 livelli di raggruppamento in una visualizzazione. I record vengono raggruppati in base all&#39;ordine dei raggruppamenti selezionati.
* Puoi applicare fino a 4 livelli di raggruppamento quando utilizzi l’API.
* I raggruppamenti sono univoci per la vista selezionata. A due visualizzazioni timeline dello stesso tipo di record possono essere applicati raggruppamenti diversi. Due utenti che visualizzano la stessa visualizzazione timeline visualizzano lo stesso raggruppamento attualmente applicato.
* Non è possibile denominare i raggruppamenti creati per una vista timeline.
* Se si rimuovono i raggruppamenti, questi verranno rimossi da tutti coloro che accedono allo stesso tipo di record e che visualizzano la stessa visualizzazione.
* È possibile raggruppare in base ai campi record o ai campi di ricerca connessi, ma non per i campi che consentono il collegamento a più record.

Per aggiungere un raggruppamento nella vista timeline:

1. Creare una visualizzazione timeline per un tipo di record, come descritto nell’articolo [Gestire le visualizzazioni record](../views/manage-record-views.md).
1. Clic **Raggruppamento** nell&#39;angolo superiore destro della vista timeline.

   ![](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. Fai clic su uno dei campi suggeriti oppure fai clic su **Scegli un campo diverso**, cerca un campo diverso, quindi fai clic su di esso quando viene visualizzato nell’elenco.

   Il raggruppamento viene applicato automaticamente alla timeline e i record vengono visualizzati nella casella di raggruppamento.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Facoltativo) Ripeti i passaggi precedenti per aggiungere fino a 3 raggruppamenti.

   Il numero di campi selezionati per il raggruppamento viene visualizzato accanto all’icona Raggruppamento.

   <!-- update screen shot with view redesign-->

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Facoltativo) All&#39;interno del **Raggruppa record per** , fare clic sul pulsante **x** a destra di un campo selezionato per il raggruppamento per rimuovere il raggruppamento

   Oppure

   Clic **Cancella tutto** per rimuovere tutti i campi.

1. Fai clic all’esterno del **Raggruppa record per** per chiuderlo.
1. (Facoltativo) Fai clic su **Impostazioni**, quindi **Colore** ai raggruppamenti dei codici colore. Per ulteriori informazioni, vedere [Modificare le impostazioni della vista timeline](#edit-the-timeline-view-settings) in questo articolo.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Modificare le impostazioni della vista timeline {#edit-the-timeline-view-settings}

Aggiornate le impostazioni della vista timeline per indicare cosa e come vengono visualizzate le informazioni nella sezione timeline della vista.

1. Creare una visualizzazione timeline per un tipo di record, come descritto nell’articolo [Gestire le visualizzazioni record](../views/manage-record-views.md).
1. Clic **Impostazioni**.
1. Clic **Data e ora** nel pannello a sinistra, seleziona un’ **Data di inizio** e un **Data di fine** per visualizzare sulla timeline. È possibile scegliere le date di inizio e di fine predefinite oppure scegliere qualsiasi campo data disponibile. Le barre che rappresentano i record iniziano nella data indicata per la data di inizio e terminano nella data corrispondente alla data di fine.

   >[!NOTE]
   >
   >I record privi di valori per le date di inizio o di fine o con una data di inizio successiva alla data di fine non vengono visualizzati nella visualizzazione della sequenza temporale.

1. Clic **Stile barra** nel pannello a sinistra, per indicare i campi che si desidera visualizzare sulle barre dei record.

   Il campo Nome è selezionato per impostazione predefinita. <!--adjust this when the primary field is released??-->

1. (Facoltativo e condizionale) Se ai record sono state aggiunte miniature, selezionare l&#39;opzione Miniatura per visualizzare l&#39;immagine associata ai record nella barra dei record.

   >[!NOTE]
   >
   >    Prima di poter visualizzare le miniature nella vista timeline, dovete aggiungerle alla vista tabella. Per ulteriori informazioni, consulta [Aggiungi miniature ai record](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).

1. Clic **Aggiungi campo** per aggiungere fino a 4 campi alle barre dei record.
1. Fai clic all’interno del **Campi ricerca** e fare clic sul campo da aggiungere.

   >[!TIP]
   >
   >   * È necessario creare i campi prima di aggiungerli alle barre dei record.
   > 
   >   * È necessario selezionare almeno un campo. **Nome** è selezionato per impostazione predefinita.

   Sulla destra viene visualizzata un&#39;anteprima dell&#39;aspetto delle barre sulla timeline.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Clic **Colore** nel pannello sinistro, per personalizzare i colori dei record e dei raggruppamenti nella timeline.

   ![](assets/color-tab-timeline-view.png)

1. (Condizionale e facoltativo) Se avete aggiunto un raggruppamento alla vista timeline, selezionate una delle seguenti opzioni per impostare un colore per il raggruppamento nella **Imposta colore di raggruppamento** sezione:

   * **Predefinito (grigio)**: il colore dei raggruppamenti è impostato sul grigio. Questa è l&#39;impostazione predefinita.
   * **Valori campo**: il colore dei raggruppamenti corrisponde al colore del campo in base al quale vengono raggruppati.
È possibile associare il colore dei raggruppamenti solo ai campi con opzioni codificate per colore.

   Ad esempio, i campi a selezione multipla o a selezione singola possono avere opzioni codificate con colori.

   Se si raggruppa per campi senza opzioni codificate per colore, il colore di raggruppamento rimane grigio.

   >[!TIP]
   >
   >Se non hai aggiunto i raggruppamenti alla vista timeline, questa sezione non viene visualizzata.

1. In **Imposta colore record** selezionare una delle opzioni seguenti per impostare un colore per i record:

   * **Tipo di record**: il colore dei record corrisponde al colore del tipo di record selezionato. Questa è l&#39;opzione predefinita.
   * **Valori campo**: il colore dei record corrisponde al colore di un campo specificato. Continuare con il passaggio 10. <!--ensure this stays accurate-->
   * **Raggruppamento**: il colore dei record corrisponde al colore indicato per i raggruppamenti. Questa opzione è disattivata se non avete applicato raggruppamenti alla vista timeline.
   * **Nessuno**: i record vengono visualizzati su una barra bianca.

1. (Condizionale) Se hai selezionato **Valori campo** per i colori del record, selezionare un campo dal **Associa il colore del record a** menu a discesa.

   ![](assets/field-selector-drop-down-menu-timeline-view.png)

   Nel menu a discesa vengono visualizzati solo i campi con opzioni codificate a colori.

   Ad esempio, i campi a selezione multipla o a selezione singola possono avere opzioni codificate con colori.

   Se non si dispone di un campo con opzioni codificate a colori per il tipo di record selezionato, questa opzione viene disattivata.

1. Fai clic su **Salva**.

   I record vengono visualizzati nella vista timeline con le specifiche selezionate.
