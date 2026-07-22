---
title: Gestire la vista tabella
description: È possibile visualizzare i record e i relativi campi in una vista tabella quando si accede alla pagina del tipo di record in Adobe Workfront Planning. In questo articolo viene descritto come creare o modificare una modifica della vista tabella e come abilitare gli indicatori di presenza in tempo reale per la vista.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0dd723b5-d674-4626-8fc2-7da41f3b7f35
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/oajBrzqCNgufbSJPP0Wx8aI14d8VM7IFr-Hn1ed7Wks
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: ce4f0de26be9a0b239c2464c97a3b47038be9108
workflow-type: tm+mt
source-wordcount: 3684
ht-degree: 2%

---

# Gestire la vista tabella

<!--
<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->


{{planning-important-intro}}

È possibile visualizzare i record e i relativi campi in una vista tabella quando si accede alla pagina del tipo di record in Adobe Workfront Planning.

Per informazioni sulle visualizzazioni record e su come gestirle, vedere [Gestione delle visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).

Questo articolo descrive le seguenti informazioni:

* [Creare o modificare colonne e righe in una vista tabella](#manage-a-table-view)
* [Abilita indicatori di presenza in tempo reale per la vista tabella](#enable-the-real-time-presence-indicator)

Per informazioni sull&#39;esportazione della vista tabella in un file Excel o CSV, vedere [Esportare i record dalla vista tabella](/help/quicksilver/planning/records/export-records-from-the-table-view.md).

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
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p> Standard per creare ed eliminare viste</p>
   <p>Collaboratore o versione successiva per aggiornare gli elementi di visualizzazione</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>   <p>Gestire le autorizzazioni per una visualizzazione</p>  
   <p>Autorizzazioni di visualizzazione a una visualizzazione per modificare temporaneamente le impostazioni di visualizzazione o per duplicarla</p> </td> 
  </tr> 
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

<!--
Old:
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
</table>
-->

## Modificare i record utilizzando la vista tabella

È possibile modificare le informazioni del record nella vista tabella.

Per ulteriori informazioni sulla modifica dei record nella vista tabella, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

## Gestire una vista tabella {#manage-a-table-view}

<!--********** MAYBE THIS IS VALID ONLY WHEN WE REPLACE THE NAVIGATION ?????????*********-->

<!-- In the Preview environment, the table view has been replaced with the list view. *******************-->

<!--
*******************IF THEY REPLACE THE LIST VIEW (IN PROJECTS AND FORMS) WITH THE NEW LIST, THEN JUST UPDATE THAT ARTICLE - "MANAGE THE LIST VIEW" - AND ADD A LINK TO IT HERE; IF NOT, THEN ADD THE SPECIFICS OF THE VIEW HERE**************
-->

Durante la creazione di una vista tabella, tutti i record del tipo selezionato vengono visualizzati in una tabella. Ogni riga è un record univoco e ogni colonna è un campo record. Tutti i campi e tutti i record vengono visualizzati per impostazione predefinita.

Per gestire una vista tabella:

1. Creare una visualizzazione tabella come descritto nell&#39;articolo [Gestire le visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).

   ![Esempio di vista tabella](assets/table-view-example-g-list.png)

1. (Facoltativo) Fai clic su **Altezza riga**, quindi seleziona una delle seguenti opzioni per modificare l&#39;altezza delle righe della tabella:
   * Piccola
   * Standard
   * Canale
   * Alta

1. (Facoltativo) Fai clic sull&#39;icona **Schermo intero** ![Icona Apri schermo intero](assets/open-full-screen-icon.png) per aprire la visualizzazione a schermo intero, quindi sull&#39;icona **Esci da schermo intero** ![Icona Esci da schermo intero](assets/exit-full-screen-icon.png) o Esc sulla tastiera per uscire dallo schermo intero.

1. Aggiornate i seguenti elementi della vista come descritto nelle sottosezioni seguenti:
   * [Colonne (o campi)](#add-columns-or-fields)
   * [Righe (o record)](#add-rows-or-records)
   * [Filtri](#add-filters)
   * [Ordina](#add-a-sort)
   * [Raggruppamento](#add-groupings)
   * [Colori riga](#add-row-colors)
   * [Indicatore di presenza in tempo reale](#enable-the-real-time-presence-indicator)


### Aggiungi colonne (o campi) {#add-columns-1}

Nelle intestazioni di colonna di una vista tabella vengono visualizzati i campi associati ai record della vista. I campi visualizzati nella vista a tabella vengono visualizzati anche nella sezione Dettagli di un record.

Per ulteriori informazioni, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

L&#39;aggiunta di colonne a una visualizzazione è identica all&#39;aggiunta di campi a un tipo di record.

È possibile aggiungere fino a 500 campi (o colonne) in una visualizzazione tabella.

1. Passare a una pagina del tipo di record e fare clic su una scheda della vista tabella oppure fare clic su **+ Vista** per aggiungere una nuova vista, quindi scegliere **Tabella**.

1. Inizia ad aggiungere campi (o colonne), come descritto nell&#39;articolo [Crea campi](/help/quicksilver/planning/fields/create-fields.md).

   Le colonne aggiunte sono visibili a tutti gli utenti che accedono al tipo di record e vengono aggiunte come nuovi campi nella pagina del record.

1. (Facoltativo) Fai clic sull&#39;icona **Campi** ![Icona Campi](assets/fields-icon.png) nella barra degli strumenti, cerca un campo, quindi deseleziona l&#39;opzione a destra del nome del campo per nasconderlo.

1. Per riordinare le colonne della tabella, effettuare una delle seguenti operazioni:

   * Prendi l’intestazione della colonna e trascinala nella posizione desiderata. La colonna spostata viene visualizzata brevemente con uno sfondo blu finché non vengono apportate altre modifiche alla tabella.

   * Fai clic su **Campi** nella barra degli strumenti della tabella, trascina i campi nell&#39;ordine desiderato, quindi fai clic all&#39;esterno della casella **Visibilità campi e ordine** per chiuderla.

     ![Barra degli strumenti di visualizzazione tabella dei campi espansa](assets/fields-setting-table-view-toolbar-expanded.png)

     >[!TIP]
     >
     >* Per impostazione predefinita, il campo Nome è sempre il primo campo della visualizzazione tabella. Questo è considerato un campo primario.
     >
     >* Non è possibile spostare il campo Nome in un&#39;altra posizione, a meno che non si indichi un altro campo come campo principale. Per ulteriori informazioni, continuare con il passaggio 5. <!--**********************accurate?**************-->
     >
     >

   * Sostituire il campo nella prima colonna con un altro campo modificando il campo principale. Per ulteriori informazioni, continuare con il passaggio 5. <!--**********************accurate?**************-->

1. (Facoltativo) Posizionare il puntatore del mouse su un nome di campo nell&#39;intestazione di colonna di un campo che non viene visualizzato nella prima colonna della tabella, fare clic sulla freccia rivolta verso il basso a destra del nome del campo, quindi fare clic su **Imposta come campo principale**.

   ![Imposta come opzione campo primario nella vista tabella](assets/set-as-primary-field-option-table-view.png)


1. Fai clic su **Imposta campo** per confermare.

   Il campo diventa un campo primario, ovvero viene visualizzato come prima colonna della visualizzazione tabella. Il campo primario precedente si sposta sulla seconda colonna.

   I campi primari diventano il titolo e la visualizzazione del record nell&#39;area dell&#39;intestazione della pagina del record e ovunque vengano visualizzati i record. Ad esempio, il titolo del record viene visualizzato in campi collegati e in tutte le visualizzazioni. Per ulteriori informazioni sui campi primari, vedere [Panoramica campo primario](/help/quicksilver/planning/fields/primary-field-overview.md).

   >[!TIP]
   >
   >Fai clic sull&#39;icona **informazioni** ![Icona informazioni](assets/info-icon.png) a destra del nome del campo in una colonna per visualizzarne **Descrizione**.

1. Fate clic sulle linee di separazione delle colonne e trascinatele nel punto desiderato per aumentare la larghezza delle colonne.

   >[!TIP]
   >
   >Le modifiche apportate alla larghezza e all’ordine delle colonne sono permanenti e visibili a tutti gli utenti che accedono alla stessa visualizzazione.

1. Passa il puntatore del mouse sull&#39;intestazione della colonna, quindi fai clic sulla freccia rivolta verso il basso, quindi fai clic su **Nascondi campo**

   Oppure

   Fare clic su **Campi** nella barra degli strumenti della tabella e deselezionare l&#39;interruttore associato ai campi o alle colonne che si desidera nascondere. Viene visualizzata la casella **Visibilità campi e ordine**.

   >[!TIP]
   >
   >Il numero di campi nascosti viene visualizzato a sinistra dell’icona Campi nella barra degli strumenti.
   >
   >Per impostazione predefinita, i campi nascosti non vengono visualizzati nella casella di anteprima **Dettagli** del record. Tutti i campi vengono visualizzati nella pagina Dettagli del record. Per informazioni, vedere [Gestire il layout della pagina record](/help/quicksilver/planning/records/manage-the-record-page.md).


1. Fai clic sull&#39;icona **Campi** e seleziona l&#39;interruttore associato ai campi che desideri visualizzare nelle colonne della tabella. Tutti i campi vengono visualizzati per impostazione predefinita.

1. Per trovare rapidamente i record che corrispondono a una parola chiave, eseguire le operazioni seguenti:

   1. Nella casella **Ricerca** ![Icona ricerca](assets/search-icon.png) inizia a digitare una parola chiave associata a qualsiasi campo di un record visualizzato sullo schermo. Accanto all’elemento da cercare viene visualizzato il numero di corrispondenze corrette e viene evidenziato il campo con la corrispondenza corretta.

      ![Casella di ricerca con struttura blu dei risultati nella vista tabella](assets/search-box-with-results-blue-outline-g-table.png)

      È possibile utilizzare qualsiasi parola o carattere speciale visibile sullo schermo.

      Non è possibile utilizzare parole chiave associate a campi nascosti nella visualizzazione Tabella.

   1. Premi **Invio** sulla tastiera per passare al successivo campo trovato.

   1. (Facoltativo) Se sono presenti più corrispondenze, fare clic sulle frecce su e giù a destra della parola chiave di ricerca per trovare tutte le corrispondenze nella tabella.

   1. Fare clic sull&#39;icona **x** nella casella di ricerca per deselezionare la parola chiave di ricerca.

1. Per i campi numerici, di valuta, di percentuale e di formula formattati come qualsiasi di questi tipi di campo, espandere il menu a discesa dell&#39;aggregatore nella parte inferiore delle colonne e selezionare una delle opzioni seguenti:

   * **SOMMA**: visualizza il totale di tutte le celle della colonna. Questa è la selezione predefinita.
   * **MIN**: visualizza il valore più basso da tutte le celle della colonna.
   * **MAX**: visualizza il valore più alto di tutte le celle della colonna.
   * **MEDIA**: visualizza il valore medio di tutte le celle della colonna.

   Quando si lavora con gli aggregatori, tenere presente quanto segue:

   * La riga dell&#39;aggregatore nella colonna è bloccata e fa parte delle impostazioni di visualizzazione.
   * In qualità di gestore delle viste, puoi scegliere l’aggregatore che verrà condiviso con la vista quando la condividi con altri utenti.
   * In qualità di visualizzatore, puoi modificare l’aggregatore, ma non viene salvato con la visualizzazione.
   * Le visualizzazioni condivise pubbliche vengono condivise con gli aggregatori salvati che non possono essere modificati.

### Aggiungi righe (o record) {#add-rows-1}

Le righe di una vista tabella visualizzano i singoli record del tipo di record selezionato. L&#39;aggiunta di righe è identica alla creazione di record.

È possibile avere fino a 50.000 record o righe per un tipo di record.

1. Passare a una pagina del tipo di record e selezionare una visualizzazione tabella oppure fare clic su **+ Visualizzazione** per aggiungere una nuova visualizzazione, quindi scegliere **Tabella**.

1. Inizia ad aggiungere record (o righe), come descritto nell&#39;articolo [Crea record](/help/quicksilver/planning/records/create-records.md).

   I record aggiunti nella vista tabella vengono salvati immediatamente e sono visibili a tutti gli utenti che dispongono di autorizzazioni di visualizzazione o di livello superiore per l&#39;area di lavoro.

   Al nuovo record viene aggiunta anche un&#39;immagine miniatura predefinita.

1. (Facoltativo) Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del record, quindi fai clic su **Modifica miniatura** per modificare la miniatura.
1. Fai clic su **Campi** nella parte superiore della tabella, quindi seleziona l&#39;interruttore per il campo **Miniatura** per visualizzarlo a sinistra del campo primario. Per impostazione predefinita è deselezionato.

   Per informazioni, vedere [Aggiungere una miniatura a un record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

<!--
For July 23: you might need to add some spacing below:
1. <span class="preview">(Optional) Click **Fields** at the top of the table, then click **Color** to display the color of a record to the left of its primary field. Colors are assigned randomly by default for each new record. The **Color** setting is deselected by default.</span>
1. <span class="preview"> (Optional and conditional) If you turned on the **Color** setting, click the color bar to the left of the record's primary field and select a color from the **Swatches** or **Custom** tabs, then click outside the box to close it. The color is applied immediately.</span>
    <span class="preview">
    ![Record color coding color picker box](assets/color-picker-for-record-color-coding.png)
    </span>
-->

### Aggiungere filtri {#add-filters-1}

I filtri consentono di ridurre la quantità di informazioni visualizzate sullo schermo.

I filtri consentono di ridurre la quantità di informazioni visualizzate sullo schermo.

Quando si lavora con i filtri nella vista a tabella, considera quanto segue:

<!-- this list is almost identical to the one for the table view - update both-->

* I filtri creati per la vista tabella funzionano in modo indipendente dai filtri nella vista timeline se applicati allo stesso tipo di record.

* I filtri sono univoci per la vista selezionata. A due visualizzazioni tabella dello stesso tipo di record possono essere applicati filtri diversi. Due utenti che osservano la stessa vista tabella visualizzano lo stesso filtro attualmente applicato.

* Non è possibile denominare i filtri generati e applicati a una vista tabella.

* La rimozione dei filtri li rimuove da chiunque acceda allo stesso tipo di record utilizzato e utilizza la stessa visualizzazione utilizzata.

* È possibile filtrare in base ai campi record o ai campi di ricerca connessi.

* Puoi filtrare per campi di ricerca che visualizzano più valori.

* È possibile fare riferimento a un campo fino a 4 livelli di distanza dal tipo di record corrente. Ad esempio, se si crea un filtro per un tipo di record Attività e l&#39;attività è connessa al tipo di record Prodotto connesso al tipo di record Campagna connesso a un progetto Workfront, è possibile fare riferimento al budget del progetto nel filtro che si sta creando per il tipo di record Attività.

Per aggiungere un filtro a una vista tabella:

1. Creare una visualizzazione tabella per una pagina del tipo di record, come descritto nell&#39;articolo [Gestione visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).
1. Seleziona una vista tabella, quindi fai clic su **Filtri** nell&#39;angolo superiore destro della tabella.
1. Fai clic su **Aggiungi condizione** e aggiungi le seguenti informazioni:

   * Cerca un campo e selezionalo quando viene visualizzato nell’elenco.

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


<!--***************** at production, paste here the information from the Production section above *******************-->

### Aggiungi un ordinamento {#sort-information-1}

Applicando un ordinamento, è possibile organizzare le informazioni in un determinato ordine.

Quando si ordinano i record nella vista tabella, tenere presente quanto segue:

<!--*********** if this is available for the timeline view, update both when you update one ****************-->

* L&#39;ordinamento è univoco per la visualizzazione selezionata. A due viste tabella dello stesso tipo di record possono essere applicati criteri di ordinamento diversi. Due utenti che visualizzano la stessa vista tabella visualizzano lo stesso ordinamento attualmente applicato.

* Non è possibile denominare le ordinazioni create e applicate a una vista tabella.

* L’ordinamento creato viene mantenuto anche quando ci si sposta.

* È possibile ordinare in base al numero di campi visualizzato nella visualizzazione per tabella di un tipo di record.

* Non è possibile ordinare in base ai campi record connessi, ma è possibile ordinare in base ai campi di ricerca dei tipi di record connessi.

* Quando si ordina in base a campi di ricerca con più valori (che non sono stati riepilogati da un aggregatore), il primo valore viene utilizzato per l’ordinamento.

* Se si rimuovono i criteri di ordinamento, questi verranno rimossi da chiunque acceda allo stesso tipo di record utilizzato e utilizzerà la stessa visualizzazione utilizzata.

* È possibile fare riferimento a un campo fino a 4 livelli di distanza dal tipo di record corrente. Ad esempio, se si crea un ordinamento per un tipo di record Attività e l&#39;Attività è connessa al tipo di record Prodotto connesso al tipo di record Campagna connesso a un progetto Workfront, è possibile fare riferimento allo Stato del progetto nell&#39;ordinamento che si sta creando per il tipo di record Attività.

Per ordinare i record, eseguire le operazioni seguenti:

1. Creare una visualizzazione tabella come descritto nell&#39;articolo [Gestire le visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).
1. Fai clic sull&#39;icona **Ordina** ![Ordina icona](assets/sort-icon.png) nella parte superiore della tabella

   Oppure

   Passa il puntatore del mouse sul nome di una colonna nella vista tabella, fai clic sulla freccia rivolta verso il basso a destra del nome dell&#39;intestazione della colonna, quindi fai clic su **Ordina**.

1. (Condizionale) Se si fa clic su **Ordina** nella parte superiore della tabella, verrà visualizzata la casella **Ordina record per**. Fare clic su uno dei campi suggeriti oppure fare clic su **Scegliere un campo diverso** e cercare un campo diverso, quindi fare clic su di esso quando viene visualizzato nell&#39;elenco.

   L&#39;ordinamento viene applicato automaticamente alla vista tabella e i record vengono visualizzati in base ai criteri selezionati.

1. (Facoltativo) Fai clic su **Aggiungi condizione** e ripeti i passaggi precedenti per ordinare in base ai campi aggiuntivi.

   Il numero di campi in base ai quali si esegue l’ordinamento viene visualizzato a sinistra dell’icona Ordina nell’angolo superiore destro della barra degli strumenti. È possibile scegliere solo i campi che vengono visualizzati nelle colonne della vista tabella.
1. (Condizionale) Se hai fatto clic sull&#39;icona **Ordina** nella parte superiore della tabella, seleziona l&#39;ordine in cui desideri ordinare il campo nella casella **Ordina record per**. Le opzioni per l’ordinamento dipendono dal tipo di campo in base al quale si sta eseguendo l’ordinamento.

   >[!TIP]
   >
   >Le selezioni seguenti non sono disponibili quando si accede all’ordinamento dall’intestazione della colonna.

   Scegli una tra le opzioni seguenti:

   * Campi data:
     * Dal primo all’ultimo
     * Dal più recente al meno recente
   * Testo, paragrafo, campi di selezione, persone, ID record:
     * Alfabetico da A a Z
     * Inverti Z alfabetico in A
   * Campi di numero, percentuale e valuta:
     * Crescente da 0 a 9
     * Decrescente da 9 a 0
   * Campi casella di controllo:
     * Prima selezione
     * Deselezionato per primo

   Il campo viene aggiunto come selezione di ordinamento nell&#39;icona **Ordina** nella parte superiore della tabella.

1. (Facoltativo) Nella casella **Ordina record per**, fare clic sull&#39;icona **x** a destra di un campo di ordinamento per rimuovere l&#39;ordinamento

   Oppure

   Fare clic su **Cancella tutto** per rimuovere tutti i campi dall&#39;ordinamento.

1. Fare clic all&#39;esterno della casella **Ordina record per** per chiuderla.

   ![Ordinamento nella vista tabella](assets/sorting-in-table-view-g-list.png)

   Le informazioni visualizzate nella tabella vengono ordinate in base ai criteri selezionati.

   I campi selezionati per l’ordinamento visualizzano un’icona di ordinamento seguita da un numero che indica l’ordine in cui viene applicato l’ordinamento.

### Aggiungi raggruppamenti {#add-groupings-1}

<!--
***********************this section exists in the timeline view too, but the display is slightly different, so I kept both procedures; consider updating both sections if any updates to groupings are introduced***************
-->

È possibile raggruppare i record in base a informazioni simili quando si applica un raggruppamento a una visualizzazione.

Considera i seguenti aspetti:

* Potete applicare i raggruppamenti sia nella vista tabella che nella vista timeline. I raggruppamenti della vista tabella sono indipendenti da quelli della vista timeline dello stesso tipo di record.
* È possibile applicare 3 livelli di raggruppamento in una visualizzazione. I record vengono raggruppati in base all&#39;ordine dei raggruppamenti selezionati.
&lt;!—*************** * È possibile applicare fino a 4 livelli di raggruppamento quando si utilizza l’API. —per il momento, controlla questo ******************—>
* I raggruppamenti sono univoci per la vista selezionata. A due visualizzazioni tabella dello stesso tipo di record possono essere applicati raggruppamenti diversi. Due utenti che visualizzano la stessa vista tabella visualizzano lo stesso raggruppamento attualmente applicato.
* Non è possibile denominare i raggruppamenti creati per una vista tabella.
* Se si rimuovono i raggruppamenti, questi verranno rimossi da tutti coloro che accedono allo stesso tipo di record e che visualizzano la stessa visualizzazione.
* È possibile modificare i record elencati in un raggruppamento.
* È possibile eseguire il raggruppamento in base ai campi record o ai campi di ricerca connessi.
* Quando si esegue il raggruppamento per campi di ricerca con più valori (che non sono stati riepilogati da un aggregatore), i record vengono raggruppati per ogni combinazione univoca di valori di campo.
* È possibile fare riferimento a un campo fino a 4 livelli di distanza dal tipo di record corrente. Ad esempio, se si crea un raggruppamento per un tipo di record Attività e l&#39;attività è connessa al tipo di record Prodotto connesso al tipo di record Campagna connesso a un progetto Workfront, è possibile fare riferimento allo stato del progetto nel raggruppamento che si sta creando per il tipo di record Attività.
* I raggruppamenti sono elencati in ordine alfabetico dei relativi valori.
  <!--********************* checking into this: * You can apply up to 4 levels of grouping when using the API. ******************-->

Per aggiungere un raggruppamento:

1. Creare una visualizzazione tabella per un tipo di record, come descritto nell&#39;articolo [Gestire le visualizzazioni record](/help/quicksilver/planning/views/manage-record-views.md).
1. Fai clic su **Raggruppamento** nell&#39;angolo superiore destro della visualizzazione tabella.

   ![Raggruppamento della vista tabella dell&#39;interfaccia utente con campi collegati](assets/grouping-ui-table-view-with-linked-fields.png)

1. Fare clic su uno dei campi suggeriti oppure fare clic su **Scegli un campo diverso**, cerca un campo diverso e quindi fare clic su di esso quando viene visualizzato nell&#39;elenco.

   Il raggruppamento viene applicato automaticamente alla tabella e i record vengono visualizzati sotto la linea di separazione di raggruppamento.

1. (Facoltativo) Fai clic su **Aggiungi condizione** e ripeti i passaggi precedenti per aggiungere fino a 3 raggruppamenti.

   Il numero di campi selezionati per il raggruppamento viene visualizzato accanto all’icona Raggruppamento.

   ![Raggruppamento applicato nella vista tabella](assets/grouping-applied-in-table-view.png)

1. (Facoltativo) Nella casella **Raggruppa record per**, fai clic sull&#39;icona **x** a destra di un campo selezionato per il raggruppamento per rimuovere il raggruppamento.

1. Fare clic all&#39;esterno della casella **Raggruppa record per** per chiuderla.
1. (Facoltativo) Fai clic su **+ Nuovo record** alla fine di qualsiasi raggruppamento per aggiungere nuovi record, quindi aggiorna la pagina per aggiungere il nuovo record al raggruppamento appropriato.

1. Per espandere o comprimere i raggruppamenti, fai clic sull&#39;icona **Raggruppamento**, quindi **Espandi tutto** o **Comprimi tutto**. Questo espande tutti i raggruppamenti e i sottogruppi nella vista tabella.

   ![Espandere e comprimere tutti i pulsanti nella visualizzazione della tabella della casella di raggruppamento](assets/expand-collapse-all-buttons-on-grouping-box-table-view.png)

   <!--
    ******** NOT POSSIBLE **********
    1. Right-click any of the grouping headers in the table view, then click one of the following options:
        * **Expand group**
        * **Collapse group**
        * **Expand all**
        * **Collapse all**
        * **Expand subgroups**
        * **Collapse subgroups**
        Depending on the number of groupings you apply to the view, some options might not be available.
    ********* NOT POSSIBLE ABOVE **********
   -->

### Aggiungi colori riga

1. (Facoltativo) Fai clic su **Colori riga** per definire le condizioni e configurare colori diversi per le righe della tabella.

1. Fai clic su **Aggiungi colore**, quindi cerca un campo e selezionalo quando viene visualizzato nell&#39;elenco. Questo è il campo di cui si desidera definire il colore di una riga o del campo primario.

   Ad esempio, per visualizzare le campagne con lo stato Attivo in verde, seleziona **Stato**, quindi scegli un modificatore e un valore per il campo.

1. Fare clic sul menu a discesa del selettore colore nell&#39;angolo superiore sinistro della condizione selezionata per scegliere il colore della condizione, quindi fare clic all&#39;esterno della casella del selettore colore per chiuderlo.

   ![Casella colori riga con stato Attivo selezionato e scelta colore predefinita](assets/row-colors-box-with-active-status-selected-default-color-choice-gtable.png)

1. (Facoltativo) Fai clic su **Aggiungi condizione** per aggiungere altri campi e valori al primo set di condizioni

   Oppure

   Fare clic su **Aggiungi colore** per aggiungere un nuovo insieme di condizioni e identificare un nuovo colore.

   Ad esempio, è possibile visualizzare le campagne con lo stato Pianificazione in giallo definendo un nuovo set di condizioni.

   ![Casella colori riga con colori personalizzati dello stato Attivo e Pianificazione](assets/row-colors-box-with-active-and-planning-status-custom-colors-gtable.png)

   >[!TIP]
   >
   >Quando sono selezionati due campi diversi, l’ultima regola si applica prima per determinare quali colori verranno applicati alle righe.


1. (Facoltativo) Attiva l&#39;impostazione **Applica all&#39;intera riga** nell&#39;angolo superiore destro della casella **Colori riga**. L’intera riga in cui viene soddisfatta la condizione viene visualizzata automaticamente nel colore selezionato.

   >[!NOTE]
   >
   >* Se l&#39;impostazione **Applica all&#39;intera riga** è disattivata, nel colore selezionato verrà visualizzato solo lo sfondo della cella del campo principale. L&#39;impostazione è disattivata per impostazione predefinita.
   >
   >* L&#39;impostazione Applica all&#39;intera riga viene disattivata quando si applicano i raggruppamenti alla tabella.

1. Fare clic all&#39;esterno della casella **Colori riga** per chiuderla. I colori vengono applicati automaticamente.

   >[!TIP]
   >
   >Se si sceglie di applicare il colore solo a una cella, viene evidenziato solo il campo Principale.


### Abilita indicatore di presenza in tempo reale

Per impostazione predefinita, nell&#39;angolo superiore destro di tutte le visualizzazioni record vengono visualizzati gli avatar di altri utenti che modificano le informazioni dei record contemporaneamente.

Quando si visualizza la vista tabella, è inoltre possibile visualizzare il campo che un altro utente sta modificando al momento della visualizzazione del record.

1. Passare a una pagina del tipo di record e aprire qualsiasi visualizzazione.
1. (Condizionale) Se altri utenti modificano contemporaneamente i record del tipo selezionato, i relativi avatar vengono visualizzati nell’angolo superiore destro della visualizzazione.
1. Fai clic sul menu a discesa accanto agli avatar, per attivare l&#39;impostazione **Mostra collaboratori**. L&#39;impostazione è attivata per impostazione predefinita.

   ![Mostra/nascondi collaboratori selezionati](assets/show-collaborators-toggle-selected.png)

   >[!TIP]
   >
   >È possibile selezionare l&#39;opzione **Mostra collaboratori** da qualsiasi visualizzazione. Il campo attualmente modificato da altri utenti è evidenziato solo nella vista tabella.

1. (Facoltativo) Apri una vista a tabella e il campo che un’altra persona sta modificando attivamente viene evidenziato nel colore corrispondente al contorno del proprio avatar nella vista a tabella.

   Se il colore di evidenziazione dell’avatar è grigio, l’utente ha interrotto la modifica attiva del record più di 30 secondi fa.

   ![Campo tabella indicatori in tempo reale e connessione avatar](assets/real-time-indicator-table-field-and-avatar-connection.png)

   <!--maybe include a screen shot after release if they update the UI text in this list of users-->

1. (Facoltativo) Fai clic sul triangolo nell’angolo superiore destro della cella che contiene il campo modificato da altri. Viene visualizzato un elenco degli utenti che stanno modificando il campo.

>[!TIP]
>
>Gli indicatori di presenza in tempo reale visualizzano gli utenti che stanno modificando un campo in qualsiasi punto di Workfront Planning. Ciò include la vista tabella o l&#39;area Dettagli del record.

<!--*********** at production, paste here the information from the Production section above ****************-->

<!--
Old information, before July 2026 when the table was replaced with the GTable/ list: 

## Manage the table view in the Production environment

When creating a table view, all records of the selected type display in a table. Each row is a unique record and each column is a record field. All fields and all records display by default. 

To manage a table view: 

1. Create a table view, as described in the article [Manage record views](/help/quicksilver/planning/views/manage-record-views.md).

    ![Table view example](assets/table-view-example.png)

1. (Optional) Click **Row height**, then select from the following options to modify the height of the table rows: 
    * Short
    * Standard
    * Medium
    * Tall 

1. (Optional) Click the **Full screen** icon ![Open full screen icon](assets/open-full-screen-icon.png) to open the view in full screen, then the **Exit full screen** icon ![Exit full screen icon](assets/exit-full-screen-icon.png) or Escape on your keyboard to exit the full screen.

1. Update the following view elements as described in the subsections below:
    * [Columns (or fields)](#add-columns-or-fields)
    * [Rows (or records)](#add-rows-or-records)
    * [Filters](#add-filters) 
    * [Sort](#add-a-sort) 
    * [Grouping](#add-groupings)
    * [Row colors](#add-row-colors)
    * [Real-time presence indicator](#enable-the-real-time-presence-indicator)


### Add columns (or fields) {#add-columns}

The column headers of a table view display fields associated with the records in the view. Fields displayed in the table view also display in the Details section of a record. 

For more information, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

*************** this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default.

Adding columns to a view is identical to adding fields to a record type.  

You can add up to 500 fields (or columns) in a table view. 

1. Go to a record type page and click a table view tab, or click **+ View** to add a new view, then choose **Table**. 

1. Start adding fields (or columns), as described in the article [Create fields](/help/quicksilver/planning/fields/create-fields.md). 

    The columns you add are visible to all users who access the record type and are added as new fields on the record's page.

1. (Optional) Click the **Fields** icon ![Fields icon](assets/fields-icon.png) in the toolbar, search for a field, then unselect the toggle to the right of the field name to hide the field. 
   
1. Do one of the following to reorder columns in the table:

    * Grab the column header and drag and drop it in the desired position. The column you moved briefly displays with a blue background until you make other adjustments to the table. 

    * Click **Fields** in the table's toolbar, then drag and drop the fields in the desired order, then click outside the **Fields visibility and order** box to close it.
        
        ![Fields setting table view toolbar expanded](assets/fields-setting-table-view-toolbar-expanded.png)

        >[!TIP]
        >
        >* The Name field is always the first field in the table view, by default. This is considered a primary field. 
        >
        >* You cannot move the Name field to another position, unless you designate another field as the primary field. For more information, continue with Step 4. 
        >
        >
 
    * Replace the field in the first column with another field by changing the primary field. For more information, continue to step 4. 

1. (Optional) Hover over a field name in the column header of any field that does not display in the first column of the table, click the downward-pointing arrow to the right of the field name, then click **Set as primary field**. 
    
    ![Set as primary field option in table view](assets/set-as-primary-field-option-table-view.png)

1. Click **Set field** to confirm. 

    The field becomes a primary field which means it displays as the first column of the table view. The previous primary field moves to the second column.

    Primary fields become the record's title and display in the header area of the record's page, and everywhere where the records display. For example, the record title displays in connected fields and all views. For more information about primary fields, see [Primary field overview](/help/quicksilver/planning/fields/primary-field-overview.md). 

1. Click and drag the column separation lines and drop them in the desired spot to increase the width of the columns. 

    >[!TIP]
    >
    >The changes you make to the column width and order are permanent and visible to all users who access the record type. 

1. Hover over the column header, then click the downward-pointing arrow, then click **Hide field**

    Or

    Click **Fields** in the table toolbar and disable the toggle associated with the fields (or columns) you want to hide. The **Fields visibility and order** box displays.

    >[!TIP]
    >
    >The number of hidden fields displays to the left of the Fields icon in the toolbar.
    >
    >By default, hidden fields do not display in the record's **Details** preview box. All fields display in the record's Details page. For information, see [Manage the record page layout](/help/quicksilver/planning/records/manage-the-record-page.md).


1. Click the **Fields** icon and enable the toggle associated with the fields you want to display in the columns of the table. All fields display by default.

1. Do the following to quickly find records that match a keyword:

    1. In the **Search** box ![Search icon](assets/search-icon.png) and start typing a keyword associated with any field of a record that displays on the screen. The number of correct matches displays next to the search item and the field with the correct match is highlighted. 

        ![Search box with results blue outline in table view](assets/search-box-with-results-blue-outline-table-view.png)

        You can use any word or special character that is visible on the screen. 
    
        You cannot use keywords that are associated with fields that are hidden in the table view. 

    1. Press **Enter** on your keyboard to go to the next found field. 

    1. (Optional) If there is more than one match, click the up and down arrows to the right of the search keyword to find all the matches in the table. 

    1. Click the **x** icon in the search box to clear the search keyword. 
   

### Add rows (or records) {#add-rows}

The rows of a table view display individual records of the selected record type. 

You can have up to 50,000 records (or rows) for . 

1. Go to a record type page and click a table view tab, or click **+ View** to add a new view, then choose **Table**. 

1. Start adding records (or rows), as described in the article [Create records](/help/quicksilver/planning/records/create-records.md). 

    The records you add in the table view are saved immediately and are visible to all users who have View or higher permissions to the workspace. 

    A thumbnail image is also added to the record.

1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name, then click **Edit thumbnail** to add a new thumbnail to the new record. 

1. Click **Fields** at the top of the table, then select the toggle for the **Thumbnail** field to display it to the left of the primary field. 
    
    For information, see [Add a thumbnail to a record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. (Optional) Select one or multiple records in a row, then drag and drop the **handle** icon ![Handle icon](assets/handle-icon.png) to the left of the record to reorder the rows. 

    >[!NOTE]
    >
    >You cannot reorder rows if you apply at least one sort to the table view. 
    >
    >The changes you make to the row order are visible to all users who access the record type

********* this section below links from the timeline view; consider splitting them if they become different

### Add filters {#add-filters}

Filters help you reduce the amount of information displayed on the screen.

Consider the following when working with filters in the table view: 

********** this list is almost identical to the one for the table view - update both

* The filters you create for the table view work independently from the filters in the timeline view when applied to the same record type. 

* The filters are unique to the view that you select. Two table views of the same record type can have different filters applied to them. Two users looking at the same table view see the same filter that is currently applied. 

* You cannot name the filters you build and apply to a table view.

* Removing filters removes them from anyone accessing the same record type as you and uses the same view as you use.

* You can filter by connected record fields or lookup fields. 

* You can filter by lookup fields that display multiple values. 

* You can reference a field that is up to 4 levels away from the current record type. For example, if you are creating a filter for an Activity record type, and the Activity is connected to the Product record type which is connected to the Campaign record type which is connected to a Workfront Project, you can reference the project's Budget in the filter you are creating for the Activity record type. 

To add a filter to a table view: 

1. Create a table view for a record type page, as described in the article [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 
1. Select a table view, then click **Filters** in the upper-right corner of the table.    
1. Click **Add condition** and add the following information: 

    * Search for a field and select it when it displays in the list.

    * **Select an option** (or a filter modifier) to define what kind of condition the field must meet

        The table below displays the available modifiers for each type of field.

        <table>
        <thead>
        <tr>
            <th><b>Field type</b></th>
            <th><b>Modifiers</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>Single-line, Paragraph, Formula </td>
            <td><p>Contains</p>
            <p>Does not contain</p>
            <p>Is</p>
            <p>Is not</p>
            <p>Is empty</p>
            <p>Is not empty</p></td>
        </tr>
        <tr><td>Single-select</td>
            <td><p>Is</p>
            <p>Is not</p>
            <p>Is any of</p>
            <p>Is none of</p>
            <p>Is empty</p>
            <p>Is not empty</p></td>
        </tr>
        <tr>
            <td>Multi-select, People</td>
            <td><p>Has any of</p>
            <p>Has all of</p>
            <p>Is exactly</p>
            <p>Has none of</p>
            <p>Is empty</p>
            <p>Is not empty</p></td>
        </tr>
        <tr>
            <td>Number, Percentage, Currency</td>
            <td><p>=</p>
            <p>≠</p>
            <p> < </p>
            <p>></p>
            <p>≤</p>
            <p>≥</p>
            <p>Is empty</p>
            <p>Is not empty</p></td>
        </tr>
        <tr>
            <td>Date</td>
            <td><p>Is</p>
            <p>Is not</p>
            <p>Is after</p>
            <p>Is before</p>
            <p>Is between</p><p>Is not between</p>
            <p>Is empty</p><p>Is not empty</p></td>
        </tr>

        <tr>
            <td>Checkbox</td>
            <td><p>Is</p>
        </tr>
        </tbody>
        </table> 

    * Select a value for the field selected. 

     ![Filter UI table view](assets/filter-ui-table-view.png)

    There is no limit to how many filtering conditions you can add.

1. (Optional) Click **Add condition** to add another filtering option and repeat the above steps. The number of filters applied displays to the left of the Filters icon. 
1. Click the following operators to indicate how the filter conditions are joined and should be applied:

    * **AND**: All specified conditions must be met. 
    * **OR**: Any of the specified conditions must be met. This is the default option.

    1. (Optional) Add additional **AND** or **OR** operators between multiple condition groupings.

        ![Multi-tiered filters in views](assets/multi-tiered-filters-in-views.png)

    The list of records is filtered automatically.  
    ************at this time, you can't name and save the filter - but will this change?!
    *********** asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!

1. (Optional) Click the **x** icon to remove a filter condition.
1. (Optional) Click **Filters** to close the filters box. ************right now you cannot "clear all" for filters, but this might come later

### Add a sort {#sort-information} 

By applying a sort, you can organize information in a given order. 

You can sort the following information:

* All records in a table view. *********or timeline view. ***********verify this is the case for the timeline view*********************
*********** * All groupings. - this is not available yet

Consider the following when sorting records in the table view: 

******** if this is available for the timeline view, update both when you update one

* Sorting is unique to the view that you select. Two table views of the same record type can have different sorting criteria applied to them. Two users looking at the same table view see the same sorting that is currently applied. 

* You cannot name the sortings you build and apply to a table view.

* The sorting you create is preserved when you navigate away.

* You can sort by as many fields as you see displayed in the table view of a record type.

* You cannot sort by connected record fields, but you can sort by lookup fields from connected record types. 

* When you sort by lookup fields with multiple values (that have not been summarized by an aggregator), the first value is used for sorting. 

* Removing sorting criteria removes them from anyone accessing the same record type as you and uses the same view as you use.

* You can reference a field that is up to 4 levels away from the current record type. For example, if you are creating a sort for an Activity record type, and the Activity is connected to the Product record type which is connected to the Campaign record type which is connected to a Workfront Project, you can reference the project's Status in the sort you are creating for the Activity record type. 

To sort *****ungrouped (add this when sorting for groupings will be available ************* records, do the following:

1. Create a table view, as described in the article [Manage record views](/help/quicksilver/planning/views/manage-record-views.md).
1. Click the **Sort** icon ![Sort icon](assets/sort-icon.png) in the upper-right corner of the table
    
    Or

    Hover over the name of a column in the table view, click the downward-pointing arrow to the right of the column header name, then click **Sort by this field**. The field is added as a sorting selection in the Sort icon in the upper-right corner of the table view.

1. (Conditional) In the **Sort records by** box, click one of the suggested fields, or click **Choose a different field** and search for a different field, then click it when it displays in the list. 

    The sorting is applied automatically to the table view and records display sorted by your selected criteria. 

    *********** add a step that you can rearrange the sorting fields here, when this will be possible
    
1. (Optional) Click **Add condition**, and repeat the above steps to sort by additional fields.  

    The number of fields that you are sorting by displays to the left of the Sort icon in the upper-right corner of the toolbar. You can choose only fields that display in the columns of the table view.

1. (Optional) In the **Sort records by** box, click the **x** icon to the right of a sorting field to remove the sort

    Or

    Click **Clear all** to remove all fields from the sort. 

1. Click outside the **Sort records by** box to close it. 

    ![Sorting in table view](assets/sorting-in-table-view.png)

    The information displayed in the table is sorted according to your selected criteria. 
    
    The fields selected for the sort display a sorting icon followed by a number that indicates the order in which the sorting is applied. 

### Add groupings {#add-groupings}

***********  this section exists in the timeline view too, but the display is slightly different, so I kept both steps; consider updating both sections if any updates to groupings are introduced

You can group records by similar information when applying  a grouping to a view.

Consider the following:

* You can apply groupings both in the table and timeline views. The groupings of the table view are independent from those in the timeline view of the same record type.
* You can apply 3 levels of grouping in a view. The records are grouped in the order of groupings that you select. 
*********** * You can apply up to 4 levels of grouping when using the API. ********** checking on this one for now********** 
* The groupings are unique to the view that you select. Two table views of the same record type can have different groupings applied to them. Two users looking at the same table view see the same grouping that is currently applied. 
* You cannot name the groupings you build for a table view.
* Removing groupings removes them from anyone accessing the same record type as you and who displays the same view as you do. 
* You can edit records listed under a grouping. 
* You can group by connected record fields or lookup fields. 
* When you group by lookup fields with multiple values (that have not been summarized by an aggregator), records are grouped by each unique combination of field values.  
* You can reference a field that is up to 4 levels away from the current record type. For example, if you are creating a grouping for an Activity record type, and the Activity is connected to the Product record type which is connected to the Campaign record type which is connected to a Workfront Project, you can reference the project's Status in the grouping you are creating for the Activity record type. 
* Groupings are listed in the alphabetical order of their values. 
********** checking into this: * You can apply up to 4 levels of grouping when using the API. 
*********** checking also into this: * You cannot group by a Paragraph-type field.

To add a grouping:

1. Create a timeline view for a record type, as described in the article [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 
1. Click **Grouping** in the upper-right corner of the table view.

    ![Grouping UI table view with linked fields](assets/grouping-ui-table-view-with-linked-fields.png)

1. Click one of the suggested fields, or click **Choose a different field**, search for a different field, then click it when it displays in the list.

    The grouping is applied automatically to the table and records display under the grouping separation line.
    
1. (Optional) Click **Add condition** and repeat the above steps to add up to 3 groupings. 

    The number of fields selected for the grouping displays next to the Grouping icon. 

    ![Grouping applied in table view](assets/grouping-applied-in-table-view.png)

1. (Optional) Inside the **Group records by** box, click the **x** icon to the right of a field selected for the grouping to remove the grouping.  

1. Click outside the **Group records by** box to close it. 
1. (Optional) Click **+ New record** at the end of any grouping to add new records, then refresh your page to add the new record to the appropriate grouping. ********* this might need to be changed when they add the Refresh button on the toolbar of the table view

1. To expand or collapse groupings, do one of the following:

    1. Click the **Grouping** icon, then **Expand all**, or **Collapse all**. This expands all the groupings and subgroupings in the table view. 

        ![Expand and collapse all buttons on grouping box table view](assets/expand-collapse-all-buttons-on-grouping-box-table-view.png)

    1. Right-click any of the grouping headers in the table view, then click one of the following options:
        * **Expand group**
        * **Collapse group**
        * **Expand all**
        * **Collapse all**
        * **Expand subgroups**
        * **Collapse subgroups**

        Depending on the number of groupings you apply to the view, some options might not be available.
   
************ ************
 this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************


### Add row colors

1. (Optional) Click **Row colors** to define conditions and choose configure diferent colors for table rows.

1. Click **Add color**, then search for a field then select it when it displays in the list. This is the field whose value you want to determine the color of a row.

    For example, to display campaigns with a status of Active in green, select **Status**, then choose a modifier and a value for the field. 

    ![Row colors box with Active status selected and default color choice](assets/row-colors-box-with-active-status-selected-default-color-choice.png)

1. Click the drop-down menu for the color picker in the upper-left corner of the condition you selected, to pick the color for the condition, then click outside the color picker box to close it. 

    ![Drop-down color picker menu in Row colors box highlighted](assets/drop-down-color-picker-menu-in-row-colors-box-highlighted.png)

1. (Optional) Click **Add condition** to add more fields and values to the first set of conditions 

    Or

    Click **Add color** to add a new set of conditions and identify a new color. 
    
    For example, you can display campaigns in a Planning status in yellow by defining a new set of conditions. 

    ![Row colors box with Active and Planning status custom colors](assets/row-colors-box-with-active-and-planning-status-custom-colors.png)

1. (Optional) Turn on the **Apply to the entire row** setting in the upper-right corner of the Row colors box. The entire row where the condition is met automatically displays in the selected color. 

    >[!NOTE]
    >
    >* If the Apply to the entire row setting is turned off, only the left side of the Primary field displays a narrow color indicator with the selected color. The setting is turned off by default.
    >
    >* You cannot apply row colors to an entire row when you have at least one grouping selected in the table view. The role color only applies to the left of the primary field cell when grouping are applied to the table. 

1. Click outside the **Row colors** box to close it. The colors are applied automatically.

### Enable the real-time presence indicator

The avatars of other users who are editing record information at the same time as you display in the upper-right corner of all record views, by default.

When you display the table view, you can also view which field another user is editing at the time you are viewing the record. 

1. Go to a record type page and open any view.
1. (Conditional) If there are other users editing the records of the selected type at the same time, their avatars display in the upper-right corner of the view. 
1. Click the drop-down menu next to the avatars, the turn on the **Show collaborators** setting. The setting is on by default. 

    ![Show collaborators toggle selected](assets/show-collaborators-toggle-selected.png)

    >[!TIP]
    >
    >You can select the **Show collaborators** toggle from any view. The field currently edited by others is outlined only in the table view. 

1. (Conditional) Open a table view, and the field which another person is actively editing is highlighted in the color corresponding to the outline of their avatar in the table view. 

    If the highlight color of the avatar is gray, the user stopped actively editing the record more than 30 seconds ago. 

    ![Real-time indicator table field and avatar connection](assets/real-time-indicator-table-field-and-avatar-connection.png)

    **** maybe include a screen shot after release if they update the UI text in this list of users

1. (Optional) Click the triangle in the upper-right corner of the cell that contains the field edited by others. A list of users currently editing the field displays.

>[!TIP]
>
>Real-time presence indicators display users that are currently editing a field anywhere in Workfront Planning. This includes either the table view or the Details area of the record.

-->






