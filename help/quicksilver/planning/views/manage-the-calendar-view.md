---
title: Gestire la visualizzazione calendario
description: È possibile visualizzare i record e i relativi campi in una visualizzazione calendario. In questo articolo viene descritto come creare una visualizzazione calendario e modificarne o eliminarne una esistente.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: f97c989f57d864252adf6e24f8e6b03f56d26901
workflow-type: tm+mt
source-wordcount: '1594'
ht-degree: 5%

---

# Gestire la visualizzazione calendario

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

È possibile visualizzare i record e i relativi campi in una visualizzazione calendario dalla pagina del tipo di record.

Per informazioni sulle visualizzazioni di Adobe Workfront Planning e su come gestirle, vedere [Gestire le visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).

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
<p>Per poter accedere a Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
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
<p><span class="preview">Nell'ambiente di anteprima, per impostazione predefinita, Planning è abilitato per utenti standard e amministratori di sistema.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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


1. Aggiornate i seguenti elementi della vista come descritto nelle sottosezioni seguenti:
   * [Filtri](#add-filters)
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
1. Seleziona una vista calendario, quindi fai clic su **Filtri** nell&#39;angolo superiore destro della tabella.
1. Fai clic su **Aggiungi condizione** e aggiungi le seguenti informazioni:

   * **Selezionare un campo** da filtrare per <!-- the tip below might change-->

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