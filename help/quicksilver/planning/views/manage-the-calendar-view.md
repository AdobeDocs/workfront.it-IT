---
title: Gestire la visualizzazione calendario
description: È possibile visualizzare i record e i relativi campi in una visualizzazione calendario. In questo articolo viene descritto come creare una visualizzazione calendario e modificarne o eliminarne una esistente.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 798e9ee9862b34653730c07acc9c48b901b98e63
workflow-type: tm+mt
source-wordcount: '1847'
ht-degree: 4%

---

# Gestire la visualizzazione calendario

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

È possibile visualizzare i record e i relativi campi in una visualizzazione calendario dalla pagina del tipo di record.

Per informazioni sulle visualizzazioni di Adobe Workfront Planning e su come gestirle, vedere [Gestire le visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).

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
</table> -->

## Gestire una visualizzazione calendario {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Considera quanto segue:

* È possibile creare una visualizzazione Calendario solo se a un tipo di record sono associati almeno due campi data. Quando a un tipo di record è associato uno o nessun campo data, l&#39;opzione della visualizzazione Calendario non è attiva.

  È possibile selezionare i campi della data di record o i campi della data di ricerca dai tipi di oggetto o record collegati.
* Esistono i seguenti scenari:

   * Se le date di inizio e di fine non contengono valori, i record non vengono visualizzati nel calendario
   * Quando le date di inizio o fine non hanno un valore, il record viene visualizzato come evento di un giorno
   * Se la data di inizio è successiva alla data di fine, il record non viene visualizzato nel calendario.

Per gestire una vista calendario:

1. Passare alla pagina del tipo di record per la quale si desidera visualizzare il calendario.
1. Creare una visualizzazione calendario come descritto nell&#39;articolo [Gestire le visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).

   ![Esempio di visualizzazione calendario](assets/calendar-view-example.png)

   I record associati al tipo di record selezionato vengono visualizzati come barre in un calendario. Per impostazione predefinita, il colore delle barre corrisponde al colore dell&#39;icona del record.

1. Per spostarsi nel calendario, effettuare una delle seguenti operazioni:

   * Fare clic sulle icone sinistra e destra nell&#39;angolo superiore sinistro del calendario o utilizzare lo scorrimento orizzontale per spostarsi all&#39;indietro e in avanti nel calendario.
   * Fai clic su **Oggi** nell&#39;angolo superiore destro per centrare il calendario alla data odierna.
   * Per aggiornare gli incrementi di tempo, seleziona una delle seguenti opzioni dal menu a discesa dell’intervallo di tempo:

      * **Mese**: record visualizzati in un calendario mensile.

      * **Settimana**: i record vengono visualizzati nelle seguenti aree:

         * I record che si estendono su più giorni vengono visualizzati nella parte superiore del calendario.
         * I record che durano un giorno o meno vengono visualizzati nella metà inferiore della visualizzazione calendario. Se si è scelto di visualizzare l&#39;ora delle date di inizio e di fine, il record viene visualizzato all&#39;ora appropriata all&#39;interno del giorno in cui si verifica.

1. (Facoltativo) Fai clic sull&#39;icona **Schermo intero** ![Icona Apri schermo intero](assets/open-full-screen-icon.png) per aprire la visualizzazione a schermo intero, quindi sull&#39;icona **Esci da schermo intero** ![Icona Esci da schermo intero](assets/exit-full-screen-icon.png) o Esc sulla tastiera per uscire dallo schermo intero.

1. Per creare record nella vista calendario o modificare le date, effettuare una delle seguenti operazioni:

   * Fare doppio clic in un punto qualsiasi del calendario per creare un record.

     Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).

   * Fare clic sul margine sinistro o destro di una barra dei record, quindi trascinarlo e rilasciarlo in una nuova posizione. Se si ridimensionano le barre dei record, le date di inizio o di fine vengono aggiornate immediatamente.

   * Trascinare e rilasciare le barre dei record per aggiornarne la posizione e le date. Lo spostamento delle barre dei record ne aggiorna immediatamente le date di inizio e di fine.

     Per informazioni, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

1. Aggiornate i seguenti elementi della vista come descritto nelle sottosezioni seguenti:
   * [Filtri](#add-filters)
   * [Altezza riga](#modify-row-height)
   * [Impostazioni](#edit-the-calendar-view-settings)

   <!--* [Grouping](#add-grouping)-->
   <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### Aggiungere filtri

È possibile ridurre la quantità di informazioni visualizzate sullo schermo utilizzando i filtri.

Quando si lavora con i filtri nella vista calendario, considera quanto segue:

<!-- this list is almost identical to the one for the table view - update both-->

* I filtri creati per una visualizzazione calendario funzionano indipendentemente dai filtri di qualsiasi altra visualizzazione applicata allo stesso tipo di record.

* I filtri sono univoci per la vista selezionata. A due visualizzazioni calendario dello stesso tipo di record possono essere applicati filtri diversi.

* Due utenti che visualizzano la stessa vista calendario visualizzano lo stesso filtro attualmente applicato.

* Non è possibile denominare i filtri creati per una visualizzazione calendario.

* Se si rimuovono i filtri, questi verranno rimossi da tutti coloro che accedono allo stesso tipo di record e che visualizzano la stessa visualizzazione.

* È possibile filtrare in base ai campi record o ai campi di ricerca connessi.

* Puoi filtrare per campi di ricerca che visualizzano più valori.

Per aggiungere un filtro a una vista calendario:

1. Creare una visualizzazione calendario per una pagina del tipo di record, come descritto nell&#39;articolo [Gestire le visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).
1. Seleziona una vista calendario, quindi fai clic su **Filtri** nella barra degli strumenti del calendario.
1. Fai clic su **Aggiungi condizione** e aggiungi le seguenti informazioni:

   * **Selezionare un campo** per <span class="preview">cercare un campo o </span> fare clic sul menu a discesa per visualizzare un elenco di campi e selezionarlo dall&#39;elenco

   * **Seleziona un&#39;opzione** (o un modificatore di filtro) per definire il tipo di condizione che il campo deve soddisfare

     Nella tabella seguente vengono visualizzati i modificatori disponibili per ogni tipo di campo.

     <table>
        <thead>
        <tr>
            <th><b>Tipo di campo</b></th>
            <th><b>Modificatori</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>Linea singola, paragrafo, formula </td>
            <td><p>Contiene</p>
            <p>Non contiene</p>
            <p>È</p>
            <p>Non è</p>
            <p>È vuoto</p>
            <p>Non è vuoto</p></td>
        </tr>
        <tr><td>Selezione singola</td>
            <td><p>È</p>
            <p>Non è</p>
            <p>È uno qualsiasi di</p>
            <p>Non è nessuno di</p>
            <p>È vuoto</p>
            <p>Non è vuoto</p></td>
        </tr>
        <tr>
            <td>Selezione multipla, Persone</td>
            <td><p>Ha uno qualsiasi di</p>
            <p>Ha tutti</p>
            <p>È esattamente</p>
            <p>Non ha nessuno di</p>
            <p>È vuoto</p>
            <p>Non è vuoto</p></td>
        </tr>
        <tr>
            <td>Numero, Percentuale, Valuta</td>
            <td><p>=</p>
            <p>≠</p>
            <p> &lt; </p>
            <p>&gt;</p>
            <p>≤</p>
            <p>≥</p>
            <p>È vuoto</p>
            <p>Non è vuoto</p></td>
        </tr>
        <tr>
            <td>Data</td>
            <td><p>È</p>
            <p>Non è</p>
            <p>È dopo il</p>
            <p>È prima del</p>
            <p>È compreso tra</p><p>Non è compreso tra</p>
            <p>È vuoto</p><p>Non è vuoto</p></td>
        </tr>

     <tr>
            <td>Casella di controllo</td>
            <td><p>È</p>
        </tr>
        </tbody>
        </table>

   * Selezionare un valore per il campo selezionato.

   ![Visualizzazione tabella interfaccia utente filtro](assets/filter-ui-table-view.png)

   Non esiste alcun limite al numero di condizioni di filtro che è possibile aggiungere.

1. (Facoltativo) Fai clic su **Aggiungi condizione** per aggiungere un&#39;altra opzione di filtro e ripetere i passaggi precedenti. Il numero di filtri applicati viene visualizzato a sinistra dell’icona Filtri.
1. Fai clic sugli operatori seguenti per indicare come vengono unite e devono essere applicate le condizioni del filtro:

   * **AND**: tutte le condizioni specificate devono essere soddisfatte.
   * **OR**: è necessario soddisfare una delle condizioni specificate. Questa è l&#39;opzione predefinita.

   1. (Facoltativo) Aggiungi altri operatori **AND** o **OR** tra più raggruppamenti di condizioni.

      ![Filtri multilivello nelle visualizzazioni](assets/multi-tiered-filters-in-views.png)

   L’elenco dei record viene filtrato automaticamente.  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. (Facoltativo) Fai clic sull&#39;icona **x** per rimuovere una condizione di filtro.
1. (Facoltativo) Fai clic su **Filtri** per chiudere la casella dei filtri. <!--right now you cannot "clear all" for filters, but this might come later-->


### Modifica altezza riga

È possibile modificare l&#39;altezza della riga di una cella del calendario per aumentare o diminuire il numero di barre dei record visualizzate in ogni cella.

Il numero di record visualizzati nel calendario varia a seconda del numero di campi visualizzati sulle barre dei record.

>[!TIP]
>
>Questa impostazione è disponibile solo quando si visualizza il calendario per mese.


1. Creare una visualizzazione calendario per una pagina del tipo di record, come descritto nell&#39;articolo [Gestire le visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).
1. (Facoltativo) Visualizza la visualizzazione calendario per mese, quindi fai clic su **Altezza riga** nella barra degli strumenti del calendario.
1. Scegli una delle seguenti opzioni:

   <table>
    <thead>
    <tr>
        <th><b>Opzione Altezza riga</b></th>
        <th><b>Numero massimo predefinito di record</b></th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td>Piccola</td>
        <td><p>Contiene:</p>

   <ul><li>2 record che visualizzano 1 campo</li>
    <li>1 record che visualizza più di 1 campo</li></ul>
        </td>
    </tr>
    <tr><td>Standard</td>
        <td><p>Contiene:</p>

   <ul><li>4 record che visualizzano 1 campo</li>
    <li>2 record che visualizzano più di 1 campo</li></ul>
        </td>
    </tr>
    <tr>
        <td>Canale</td>
        <td><p>Contiene:</p>

   <ul><li>8 record che visualizzano 1 campo</li>
    <li>4 record che visualizza più di 1 campo</li></ul>
        </td>
    </tr>
    <tr>
        <td>Alta</td>
        <td><p>Contiene:</p>

   <ul><li>12 record che visualizzano 1 campo</li>
    <li>6 record con più di 1 campo</li></ul>
        </td>
    </tr>
    <tr>
        <td>Adatta al contenuto</td>
        <td><p>Tutti i record sono visibili, fino a 500 record</p></td>
    </tr>
    </tbody>
    </table>

1. (Facoltativo) Fare clic su **altro** se sono presenti record non visibili nel calendario.

</span>

### Modificare le impostazioni della vista calendario

Aggiorna le impostazioni della vista calendario per indicare cosa e come vengono visualizzate le informazioni nella vista.

1. Creare una visualizzazione calendario per un tipo di record, come descritto nell&#39;articolo [Gestione visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).
1. Fare clic su **Impostazioni**.
1. Fai clic su **Data e ora** nel pannello a sinistra, quindi seleziona una **Data di inizio** e una **Data di fine** da visualizzare nel calendario. È possibile scegliere le date di inizio e di fine predefinite oppure scegliere qualsiasi campo data disponibile.

   Le barre che rappresentano i record iniziano nella data indicata per la data di inizio e terminano nella data corrispondente alla data di fine.

   >[!NOTE]
   >
   >* I record privi di valori per le date di inizio o di fine o con una data di inizio successiva alla data di fine non vengono visualizzati nella visualizzazione calendario.
   >
   >* Se si visualizzano record aggiuntivi utilizzando l&#39;opzione Raggruppamento, le date di inizio e di fine corrispondono a quelle del record principale. Non è possibile scegliere le date di inizio e di fine per i record connessi in quest&#39;area.

1. Fare clic su **Stile barra** nel pannello sinistro per indicare le informazioni da visualizzare sulle barre dei record.

   Il campo principale (o titolo) del record, come definito nella vista tabella del record, è selezionato per impostazione predefinita.
   <!--adjust this when the primary field is released??-->

1. (Facoltativo e condizionale) Se hai aggiunto miniature ai record, seleziona l&#39;opzione **Miniatura** per visualizzare l&#39;immagine associata ai record nella barra dei record.

   >[!NOTE]
   >
   >    È necessario aggiungere le miniature nella vista tabella prima di poterle visualizzare nella vista calendario. Per ulteriori informazioni, vedere [Aggiungere una miniatura a un record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. Fai clic su **Aggiungi campo**, quindi fai clic nella casella **Cerca campi** e fai clic sul campo che desideri aggiungere.

   >[!TIP]
   >
   >   * È necessario creare i campi prima di aggiungerli alle barre dei record.
   > 
   >   * È necessario selezionare almeno un campo. **Nome** è selezionato per impostazione predefinita.
   >
   >   * Puoi aggiungere fino a 5 campi.

   A destra viene visualizzata un&#39;anteprima dell&#39;aspetto delle barre nel calendario.

   ![Sezione stile barra nelle impostazioni della visualizzazione calendario](assets/bar-style-section-in-calendar-view-settings-with-preview.png)

1. Fai clic su **Colore** nel pannello a sinistra per personalizzare i colori dei record nel calendario.

   ![Impostazioni del pannello colori nella vista calendario](assets/color-panel-on-calendar-view-settings.png)

1. Nella sezione **Imposta il colore del record su**, selezionare una delle opzioni seguenti per impostare un colore per i record:

   * **Tipo di record**: il colore delle barre dei record nel calendario corrisponde al colore del tipo di record selezionato. Questa è l&#39;opzione predefinita.
   * **Valori campo**: il colore dei record corrisponde al colore di un campo specificato.
   * **Nessuno**: i record vengono visualizzati in una barra bianca.

1. (Condizionale) Se hai selezionato **Valori campo** per i colori del record, seleziona un campo dal menu a discesa **Corrispondenza colore del record con**.

   ![Menu a discesa del selettore dei campi per la visualizzazione del calendario](assets/field-selector-drop-down-menu-calendar-view.png)

   Nel menu a discesa vengono visualizzati solo i campi con opzioni codificate a colori.

   Ad esempio, i campi a selezione multipla o a selezione singola possono avere opzioni codificate con colori.

   Se non si dispone di un campo con opzioni codificate a colori per il tipo di record selezionato, questa opzione viene disattivata.


1. Fai clic su **Salva**.

   I record vengono visualizzati nella vista calendario con le specifiche selezionate.