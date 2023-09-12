---
title: Gestire la visualizzazione della timeline
description: È possibile visualizzare i record in una visualizzazione timeline quando si accede alla pagina del tipo di record in Adobe Maestro.
hidefromtoc: true
hide: true
source-git-commit: bac066b90c7fd69ffd423988c4cf736c16807f2b
workflow-type: tm+mt
source-wordcount: '1078'
ht-degree: 1%

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

>[!IMPORTANT]
>
>Attualmente, Adobe Maestro fa parte di un programma beta chiuso aperto a un numero limitato di clienti.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

È possibile visualizzare i record in una visualizzazione timeline quando si accede alla pagina del tipo di record in Adobe Maestro.

Per informazioni sulle visualizzazioni Maestro, consulta [Gestire le visualizzazioni record in Adobe Maestro](../views/manage-record-views.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> prodotto Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>La tua organizzazione deve essere iscritta al programma beta chiuso Adobe Maestro. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
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
   <td role="rowheader">Livello di accesso</td>
   <td> <p>Qualsiasi</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modello di layout</td>
   <td> <p>L’amministratore di sistema deve aggiungere l’area Maestro nel modello di layout. Per informazioni, consulta <a href="../access/grant-access.md">Concedere l’accesso a Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Gestire una vista timeline {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

Durante la creazione di una vista timeline, tutti i record del tipo di record selezionato vengono visualizzati in una timeline cronologica.

Considera quanto segue:

* È possibile creare una visualizzazione Sequenza temporale solo se a un tipo di record sono associati almeno due campi data. Se a un tipo di record è associato uno o nessun campo data, l&#39;opzione della visualizzazione Timeline non è disponibile.
* A seconda delle date associate ai record, alcuni record potrebbero non essere visualizzati nella visualizzazione della sequenza temporale nei seguenti scenari:

   * Quando le date di inizio e fine non hanno valori
   * Quando le date di inizio o fine non hanno valore
   * Quando la data di inizio è successiva alla data di fine

<!--these are NOT available now because there won't be a table for the timeline view for the near future, per Andy: 
* The records displayed in the timeline view also display in a view-only table to the left of the timeline. 
* Each row in the table and each bar on the timeline represent the same record. 
* Each column in the table is a record field. The columns of this table are preconfigured and cannot be customized. 
* Only a limited number of fields (or columns) display in the timeline view table. 
* You cannot do the following in a timeline view:
     * Add rows or records
     * Add columns or fields
     * Edit record information
-->

Durante la creazione di una vista timeline, per impostazione predefinita tutti i record del tipo di record selezionato vengono visualizzati in una timeline come barre.

Per gestire una vista timeline:

1. Passare alla pagina del tipo di record per la quale si desidera visualizzare la sequenza temporale.
1. Creare una visualizzazione timeline come descritto nell’articolo [Gestire le visualizzazioni record](../views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   I record associati al tipo di record selezionato vengono visualizzati in una sequenza temporale cronologica sotto forma di barre.

1. Per spostarsi nella timeline, effettuate una delle seguenti operazioni:

   * Fate clic sulle icone sinistra e destra oppure utilizzate lo scorrimento orizzontale per spostarvi avanti e indietro nella timeline.
   * Clic **Oggi** per centrare la timeline fino alla data odierna.
   * Per aggiornare gli incrementi di tempo, seleziona una delle seguenti opzioni dal menu a discesa dell’intervallo di tempo:

      * Anno
      * Trimestre
      * Mese
1. Clic **Passa a Standard** visualizzazione per visualizzare i record in righe separate <!--check to see if they updated the name of the setting here-->

   Oppure

   Clic **Passa alla visualizzazione Compatta** per visualizzare i record le cui date non si intersecano sulla stessa riga. <!--check to see if they updated the name of the setting here-->

   I record vengono visualizzati nella visualizzazione Compatta per impostazione predefinita.

1. Aggiornate i seguenti elementi della vista come descritto nelle sottosezioni seguenti:
   * [Filtri](#add-filters)
   * [Raggruppamento](#add-grouping)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->
   * [Impostazioni](#edit-the-timeline-view-settings)

### Aggiungere filtri

I filtri consentono di ridurre la quantità di informazioni visualizzate sullo schermo.

Quando si lavora con i filtri nella vista timeline, considera quanto segue:

<!-- this list is almost identical to the one for the table view - update both-->

* I filtri creati per la visualizzazione timeline funzionano in modo indipendente dai filtri nella visualizzazione tabella se applicati allo stesso tipo di record.

* I filtri sono univoci per la vista selezionata. A due visualizzazioni timeline dello stesso tipo di record possono essere applicati filtri diversi. Due utenti che visualizzano la stessa visualizzazione timeline visualizzano lo stesso filtro attualmente applicato.

* Non è possibile assegnare un nome ai filtri generati e applicati a una vista timeline.

* La rimozione dei filtri li rimuove da chiunque acceda allo stesso tipo di record utilizzato e utilizza la stessa visualizzazione utilizzata.

L’aggiunta di filtri nella vista timeline è identica all’aggiunta di filtri nella vista tabella.

Per ulteriori informazioni, consulta la sezione &quot;Aggiungere filtri&quot; nell’articolo [Gestire la vista tabella](../views/manage-the-table-view.md).

### Aggiungi raggruppamento

<!-- if groupings are identical between the table and the timeline, consider replacing this section with this: 

Adding groupings in the timeline view is identical to adding filters in the table view. 

For more information, see the "Add filters" section in the article [Manage the table view](../views/manage-the-table-view.md). -->


È possibile raggruppare i record in base a informazioni simili quando si applica un raggruppamento a una visualizzazione.

Quando si lavora con i raggruppamenti nella vista timeline, tenete presente quanto segue:

* Potete applicare i raggruppamenti sia nella vista tabella che nella vista timeline. I raggruppamenti della vista tabella sono indipendenti da quelli della vista timeline dello stesso tipo di record.
* Potete applicare 3 livelli di raggruppamento in una vista Maestro. I record vengono raggruppati in base all&#39;ordine dei raggruppamenti selezionati.
* Puoi applicare fino a 4 livelli di raggruppamento quando utilizzi l’API.

Per aggiungere un raggruppamento:

1. Creare una visualizzazione timeline come descritto nell’articolo [Gestire le visualizzazioni record](../views/manage-record-views.md).
1. Clic **Raggruppamento**.

   ![](assets/grouping-ui-timeline-view.png)

1. Fai clic su uno dei campi suggeriti oppure fai clic su **Scegli un campo diverso** e cerca un campo diverso, quindi fai clic su di esso quando viene visualizzato nell’elenco.

   >[!TIP]
   >
   >Non è possibile selezionare campi collegati.

   Il raggruppamento viene applicato automaticamente alla timeline e i record vengono visualizzati nella casella di raggruppamento. Il numero di elementi in un raggruppamento viene visualizzato sulla riga di raggruppamento.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Facoltativo) Ripeti i passaggi precedenti per aggiungere fino a 3 raggruppamenti.

   Il numero di raggruppamenti applicati viene visualizzato a sinistra dell’icona Raggruppamento nell’angolo superiore destro della barra degli strumenti.

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Facoltativo) Fai clic su **x** a destra di un raggruppamento per rimuovere il raggruppamento

   Oppure

   Clic **Cancella tutto** per rimuovere tutti i raggruppamenti.

1. Fai clic all’esterno del **Raggruppa record per** per chiuderlo.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Modificare le impostazioni della vista timeline {#edit-the-timeline-view-settings}

Aggiornate le impostazioni della vista timeline per indicare le informazioni visualizzate nella sezione timeline della vista.

1. Creare una visualizzazione timeline come descritto nell’articolo [Gestire le visualizzazioni record](../views/manage-record-views.md).
1. Clic **Impostazioni**.
1. Clic **Data e ora** nel pannello a sinistra, seleziona un’ **Data di inizio** e un **Data di fine** per visualizzare sulla timeline. È possibile scegliere le date di inizio e di fine predefinite oppure scegliere qualsiasi campo data disponibile. Le barre che rappresentano i record iniziano nella data indicata per la data di inizio e terminano nella data corrispondente alla data di fine.

   >[!NOTE]
   >
   >    I record privi di valori per le date di inizio o di fine o con una data di inizio successiva alla data di fine non vengono visualizzati nella visualizzazione della sequenza temporale.


1. Clic **Dettagli record** per indicare i campi che si desidera visualizzare sulle schede record.

   Il campo Nome è selezionato per impostazione predefinita.

1. Clic **Aggiungi campo** per aggiungere fino a 4 campi alle barre dei record.
1. Fai clic all’interno del **Campi ricerca** e fare clic sul campo da aggiungere.

   >[!TIP]
   >
   >   * È necessario creare i campi prima di aggiungerli alle barre dei record.
   > 
   >   * È necessario selezionare almeno un campo. **Nome** è selezionato per impostazione predefinita.

   Sulla destra viene visualizzata un&#39;anteprima dell&#39;aspetto delle barre sulla timeline.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Fai clic su **Salva**.

   I record vengono visualizzati nella vista timeline con le specifiche selezionate.


