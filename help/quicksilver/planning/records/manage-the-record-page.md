---
title: Gestire il layout della pagina record
description: È possibile modificare il layout dell'anteprima record e della pagina in Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 1ed84baeacda2717c4f58058fb754e7a79b48baf
workflow-type: tm+mt
source-wordcount: '2261'
ht-degree: 0%

---


# Gestire il layout della pagina record

<!--
<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

È possibile modificare il layout dell&#39;anteprima record e della pagina in Adobe Workfront Planning.

L&#39;anteprima del record è una visualizzazione ridotta della pagina del record visualizzata nella visualizzazione di un tipo di record.

Quando si modifica il layout di un&#39;anteprima record e di una pagina, le modifiche hanno effetto sulle caselle di anteprima e sulle pagine dei dettagli di tutti i record dello stesso tipo.

In questo articolo viene descritto come modificare il layout e l&#39;aspetto di una casella di anteprima del record o di una pagina di record. Per informazioni sulla modifica dei record, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

È necessario creare tipi di record e record prima di iniziare a modificare le pagine dei record.

Per informazioni, vedere i seguenti articoli:

* [Crea tipi di record](/help/quicksilver/planning/architecture/create-record-types.md)

* [Crea record](/help/quicksilver/planning/records/create-records.md)

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
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td>
   <td>
   <p>Contribuire o concedere autorizzazioni superiori a un’area di lavoro e a un tipo di record </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p> 
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
<p>Any</p>
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
   <td>
   <p>Standard</p>
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
   <td>
   <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> 
  </td>
  </tr>
 </tbody>
</table>-->

## Considerazioni sulla modifica delle pagine record

* Per impostazione predefinita, i dettagli e le pagine di anteprima di un record visualizzano tutti i campi associati al record.

* Non è possibile aggiungere nuovi campi per un record nella pagina di anteprima o dei dettagli. Per visualizzarli nelle pagine di anteprima e dettagli, è necessario aggiungere nuovi campi nella vista a tabella.

* È possibile aggiungere sezioni a un&#39;anteprima del record o a una pagina dei dettagli, per organizzare le informazioni in base a criteri comuni e semplificarne la ricerca.

* Le modifiche seguenti hanno effetto su tutti i record dello stesso tipo e sono visibili a tutti gli utenti che accedono a tali record:

   * Ridisposizione dei campi
   * Aggiunta o rimozione di sezioni

* Le modifiche apportate all&#39;anteprima del record sono immediatamente visibili nella pagina dei dettagli del record. Le modifiche apportate nella pagina record sono visibili anche nella casella di anteprima del record.

* L&#39;aggiunta di un&#39;immagine di copertina o di una miniatura a un record non fa parte del layout generale dell&#39;anteprima del record o della pagina. È possibile aggiungere immagini di copertina o miniature univoche a ciascun record. Per informazioni, vedere [Aggiungere un&#39;immagine di copertina a un record](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) e [Aggiungere una miniatura a un record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

## Aggiungere sezioni a una pagina o anteprima record

Quando si aggiungono sezioni a una pagina record, tenere presente quanto segue:

* Non esiste alcun limite al numero di sezioni che è possibile includere in una pagina.
* Impossibile avere una sezione vuota. È necessario disporre di almeno un campo in una sezione.
* È possibile trascinare i campi da una sezione all&#39;altra. Per ulteriori informazioni, vedere la sezione [Ridisponi campi nell&#39;anteprima record o nella pagina dei dettagli](#rearrange-fields-in-the-record-preview-or-details-page) in questo articolo.
* Quando rimuovi tutti i campi da una sezione, questa viene eliminata automaticamente e non può essere recuperata.

Per aggiungere una sezione a un&#39;anteprima record o a una pagina:

{{step1-to-planning}}

1. Fai clic sulla scheda di un’area di lavoro.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

1. In una visualizzazione di qualsiasi tipo fare clic sul nome di un record

   Oppure

   Nella vista tabella fare clic sull&#39;icona **Apri dettagli** ![Apri dettagli nel campo nome tabella](assets/open-details-icon-in-table-name-field.png) nella prima colonna.

   L&#39;anteprima del record viene visualizzata nella vista.

   ![Casella Dettagli](assets/details-box.png)

1. (Facoltativo) Fai clic sull&#39;icona **Apri in una nuova scheda** ![Apri i dettagli in una nuova scheda](assets/open-details-in-a-new-tab-icon.png) nell&#39;angolo superiore destro dell&#39;anteprima del record per aprire la pagina del record in una nuova scheda.

   Viene visualizzata la pagina del record. Per impostazione predefinita, viene visualizzata la scheda Dettagli (Details).

   ![Pagina dettagli](assets/details-page.png)

1. Nella scheda **Dettagli** dell&#39;anteprima del record o della pagina, passa il puntatore del mouse sullo spazio vuoto a sinistra dei campi, quindi fai clic sull&#39;icona **Aggiungi sezione** ![Aggiungi sezione](assets/add-section-icon.png) per aggiungere una sezione.
1. Fare clic nel nome della sezione e sostituire **Sezione senza titolo** con un nome, quindi fare clic su Invio. I campi visualizzati sotto la sezione fanno automaticamente parte della nuova sezione.
1. Inizia a trascinare i campi nella nuova sezione, come descritto nella sezione [Ridisponi i campi nell&#39;anteprima del record o nella pagina dei dettagli](#rearrange-fields-in-the-record-preview-or-details-page) in questo articolo.

1. (Facoltativo) Passa il puntatore del mouse sul nome di una sezione e fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png).

   ![Altre opzioni di menu per la sezione nella pagina record](assets/more-menu-options-for-section-on-record-page.png)
1. (Facoltativo) Per modificare la sezione, effettuate una delle seguenti operazioni:

   * Fai clic su **Rinomina** per rinominare la sezione

     >[!TIP]
     >
     > È possibile rinominare una sezione in linea facendo clic sul nome.

   * Fai clic su **Sposta su** per spostare la sezione in alto di una posizione

     Oppure

     Fare clic su **Sposta in basso** per spostare la sezione in basso di una posizione.
Tutti i campi della sezione vengono spostati insieme alla sezione.

   * Fai clic su **Elimina** per eliminare la sezione. La sezione viene eliminata e non può essere recuperata. Tutti gli utenti che accedono ai record di questo tipo non visualizzeranno più la sezione eliminata.

1. Fare clic sulla freccia rivolta verso il basso a sinistra del nome di una sezione per comprimerla oppure sulla freccia rivolta verso destra per espanderla.
Per impostazione predefinita, tutte le sezioni vengono espanse.

1. (Facoltativo) Fai clic sull&#39;icona **grab** ![Grab icon](assets/grab-icon.png) a sinistra del nome di una sezione, quindi trascinala e rilasciala nella posizione desiderata.

   La nuova posizione della sezione viene aggiornata sia nell&#39;anteprima che nella pagina di tutti i record dello stesso tipo per tutti gli utenti che visualizzano i record.

   Tutte le modifiche apportate alle sezioni e all&#39;ordine dei campi vengono salvate automaticamente.

1. (Facoltativo) Fai clic sull&#39;icona del menu **Esporta** ![Esporta nella pagina dei dettagli del record](assets/export-icon-in-record-details-page.png) per esportare la scheda Dettagli in un file Word o PDF. Per ulteriori informazioni, vedere [Esportare i dettagli di un record](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Facoltativo) Fai clic sulla scheda **Connessioni** accanto alla scheda **Dettagli**. Potrebbe essere necessario fare clic su **Altro** prima di fare clic sulla scheda **Connessioni**.

   Tutti i record o gli oggetti connessi al record selezionato vengono visualizzati con i nomi del tipo di record o dell&#39;applicazione a cui appartengono.

   ![Scheda Connessioni nel record di Workfront Planning](assets/connections-tab-on-record-in-workfront-planning.png)

1. (Facoltativo) Selezionare l&#39;impostazione **Mostra tutti i record** nell&#39;angolo superiore destro della scheda Connessioni. Vengono visualizzati tutti i tipi di record connessi, inclusi quelli che non dispongono ancora di record connessi. Per impostazione predefinita, l&#39;interruttore è deselezionato e i tipi di record senza record collegati sono nascosti.

1. (Facoltativo) Fai clic su **Connetti** per aggiungere altri record ai tipi di record connessi. Per ulteriori informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

1. (Facoltativo) Passa il puntatore del mouse su una scheda record, quindi fai clic sull&#39;icona Disconnetti record **-**, quindi fai clic su **Disconnetti**. <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
Si verificano le seguenti situazioni:
   * Il record non è più connesso all&#39;oggetto Workfront.
   * L&#39;oggetto Workfront viene inoltre rimosso dal campo connesso del record da Workfront Planning.
   * Vengono eliminati anche i valori dei campi di ricerca di Workfront connessi al record Planning.

## Ridisporre i campi nella scheda Dettagli del record

{{step1-to-planning}}

1. Fai clic sulla scheda di un’area di lavoro.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

1. In una visualizzazione di qualsiasi tipo fare clic sul nome di un record

   Oppure

   Nella vista tabella fare clic sull&#39;icona **Apri dettagli** ![Apri dettagli nel campo nome tabella](assets/open-details-icon-in-table-name-field.png) nella prima colonna.

   L&#39;anteprima del record viene visualizzata nella vista.

   ![Casella Dettagli](assets/details-box.png)

1. (Facoltativo) Fai clic sull&#39;icona **Apri in una nuova scheda** ![Apri la casella dei dettagli in una nuova scheda](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> nell&#39;angolo superiore destro dell&#39;anteprima del record per aprire la pagina del record in una nuova scheda.

   Per impostazione predefinita viene aperta la scheda **Dettagli** del record.

   ![Pagina dettagli](assets/details-page.png)

1. Nella scheda **Dettagli** del record, fai clic sull&#39;icona **grab** ![Grab icon](assets/grab-icon.png) a sinistra di un nome di campo, quindi trascinalo e rilascialo nel punto desiderato.

   >[!TIP]
   >
   >È possibile trascinare i campi in un&#39;altra sezione.
   >È necessario disporre di almeno un campo in una sezione.
   >

   La nuova posizione del campo viene aggiornata sia nell&#39;anteprima che nella pagina di tutti i record dello stesso tipo per tutti gli utenti che visualizzano i record.

   Tutte le modifiche apportate al layout dell&#39;anteprima record o del salvataggio automatico della pagina.

## Aggiungere una pagina Record connessi a un record

È possibile visualizzare informazioni da record o oggetti connessi aggiungendo a un record una scheda per la pagina Record connessi. In questo modo i record connessi in una vista tabella vengono aggiunti alla scheda.

Quando si aggiunge una pagina Record connessi a un record, tenere presente quanto segue:

* È possibile aggiungere una pagina Record collegati a un record dopo aver connesso tipi di record o di oggetti al tipo di record dalla vista tabella di un tipo di record.

* È possibile aggiungere una pagina Record collegati dall&#39;area di anteprima di un record o dalla pagina del record.

* Nelle pagine Record collegati vengono visualizzati solo gli oggetti o i record collegati di un oggetto o di un tipo di record in una visualizzazione tabella. Nella pagina non vengono visualizzati tutti i record di quel tipo.

* È possibile aggiungere pagine Record collegati per i tipi di oggetto o record connessi seguenti:

   * Tipi di record di Workfront Planning
   * Progetti, programmi, portfolio, gruppi o aziende di Workfront. È possibile visualizzare gli oggetti Workfront connessi anche se non si dispone delle autorizzazioni necessarie per accedervi in Workfront.

  >[!NOTE]
  >
  > Non è possibile aggiungere una pagina Record connessi per i record AEM Assets connessi.

Per aggiungere una pagina Record connessi:

1. Fare clic sul nome del record per aprirlo da qualsiasi visualizzazione di una pagina del tipo di record.
1. Fare clic su **Aggiungi pagina** da una delle seguenti aree:

   * Finestra di anteprima del record
   * Pagina dei dettagli del record, dopo aver fatto clic sull&#39;icona **Apri in una nuova scheda** ![Apri i dettagli in una nuova scheda](assets/open-details-in-a-new-tab-icon.png) nell&#39;angolo superiore destro della pagina di anteprima.

   Viene visualizzata la casella **Crea pagina**.

   ![Aggiungi record connessi a pagina modale](assets/add-connection-view-page-modal.png)

1. Aggiungi **Nome pagina**, fai clic su **Pagina record connessi**, quindi fai clic su **Crea**.

   Una nuova pagina di record connessi viene aggiunta come nuova scheda alla pagina del record.

   I record connessi al record corrente vengono visualizzati nella vista tabella.

   >[!TIP]
   >
   >È necessario aggiungere i record connessi nella tabella o nell&#39;area Dettagli di un record prima di visualizzarli in una pagina dei record connessi.

   <!--All fields of the connected record display in the table view of the connected record's tab.-->

   I primi cinque campi dei record connessi vengono visualizzati per impostazione predefinita. <!--No lookup fields display by default.-->

   ![Visualizzazione tabella connessa al pubblico nei dettagli della campagna](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Facoltativo) Cercare o fare clic sul nome di un record o di un tipo di oggetto connesso nell&#39;elenco.

1. (Facoltativo e condizionale) Nella vista tabella della pagina dei record connessi eseguire una delle operazioni seguenti quando si visualizzano i record di Planning connessi o qualsiasi oggetto di Workfront ad eccezione dei progetti: <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

   * Fare clic sul nome di un record. Verrà aperta la pagina del record in una nuova scheda.

   * Fai clic su **Connetti** nella parte inferiore della visualizzazione tabella per connettere altri record, quindi fai clic all&#39;esterno della casella di connessione per chiuderla. I nuovi record vengono aggiunti automaticamente alla tabella.

     Per informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).
   * Modificare le informazioni dei record collegati in linea nella vista tabella.

   * Passa il puntatore del mouse sul nome di un record connesso, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png)

     Oppure

     Selezionare uno dei record, quindi fare clic su una delle opzioni seguenti nella barra blu nella parte inferiore dell&#39;elenco:

      * **Visualizza** per aprire la pagina record in una nuova scheda
      * **Copia collegamento** per copiare un collegamento nella pagina record
      * **Modifica miniatura** per aprire la casella **Miniatura record** e modificare l&#39;immagine miniatura del record
      * **Duplicato** per duplicare il record connesso. Il record duplicato è anche collegato al record corrente.
      * **Inserire un record superiore o inferiore** per aggiungere nuovi record al tipo di record connesso. Anche i nuovi record aggiunti qui sono collegati al record corrente. Questa opzione non è disponibile nella barra blu quando si seleziona un record nella tabella.
      * **Elimina** per eliminare il record. Se si elimina un record connesso, questo viene eliminato dal relativo tipo di record e da qualsiasi posizione in cui il record è connesso.

     Per informazioni sulla modifica dei record nella vista tabella, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

     >[!TIP]
     >
     >È possibile selezionare più record o oggetti per eliminarli.

   * In linea modificare qualsiasi record di Planning nella tabella della pagina Record connessi.

     Tutti gli altri oggetti di Workfront vengono visualizzati in una vista tabella di sola lettura e non è possibile modificarli.

1. (Facoltativo e condizionale) Nella vista a tabella della pagina record connessi, eseguire una delle operazioni seguenti quando si visualizzano progetti Workfront connessi:

   * Fare clic su **Connetti record** nell&#39;angolo superiore destro della pagina dei record connessi per connettere i progetti esistenti.

   Per informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).
   * Modifica in linea le informazioni sul progetto nella tabella.
   * Fai clic su **Nuova riga** per creare un progetto senza modello. Il nuovo progetto viene immediatamente connesso al record corrente.

     Per ulteriori informazioni, vedere [Creare oggetti Workfront da Workfront Planning durante la connessione ai record](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
   * Passa il puntatore del mouse su un progetto e fai clic sul menu **Altro** [Altro menu](assets/more-menu.png)

     Oppure

     Seleziona uno o più progetti e osserva la barra blu nella parte inferiore dell’elenco, quindi fai clic su una delle seguenti opzioni:

      * **Elimina** per eliminare il progetto. Quando si elimina un progetto, questo viene disconnesso dal record e spostato nel Cestino di Workfront.
      * **Disconnetti** per disconnettere il progetto dal record. Se si disconnette un progetto, verranno rimossi anche tutti i valori dei campi di ricerca dal record corrente.

1. (Facoltativo) Fare doppio clic sul nome della scheda **Record connessi**

   Oppure

   Passa il puntatore del mouse sul nome della scheda, quindi fai clic su **Altro** ![Altro menu](assets/more-menu.png), quindi su **Rinomina** per rinominare la nuova scheda Visualizzazione connessa.
1. (Facoltativo) Per gestire la vista tabella, utilizzare uno degli elementi di visualizzazione riportati di seguito nella barra degli strumenti di una pagina di record connessa:

   * Filtri
   * Ordina
   * Raggruppamento
   * Campi, per visualizzare, nascondere o ridisporre i campi
   * Altezza riga
   * Ricerca

   Per informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >Non è possibile creare, modificare o eliminare campi nella visualizzazione per tabella della scheda di un record connesso.

1. (Facoltativo) Passa il puntatore del mouse sul nome della scheda della pagina Record connessi, fai clic su **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su **Elimina** per rimuoverlo dalla scheda.

<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



