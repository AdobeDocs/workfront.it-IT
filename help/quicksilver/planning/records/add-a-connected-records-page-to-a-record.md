---
title: Aggiungere una pagina Record collegati a un record
description: È possibile visualizzare informazioni da record o oggetti connessi aggiungendo a un record una scheda per la pagina Record connessi. In questo modo i record connessi in una vista tabella vengono aggiunti alla scheda.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 5b1993d49ff675b3bab1d470bc756b987fe19d1c
workflow-type: tm+mt
source-wordcount: '1513'
ht-degree: 1%

---


# Aggiungere una pagina Record connessi a un record

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

È possibile visualizzare informazioni da record o oggetti connessi aggiungendo una scheda per una pagina Record connessi a un record in Adobe Workfront Planning. In questo modo i record connessi in una vista tabella vengono aggiunti alla scheda.

Quando si aggiunge una pagina Record connessi a un record, tenere presente quanto segue:

* È possibile aggiungere una pagina Record collegati a un record dopo aver connesso tipi di record o di oggetti al tipo di record dalla vista tabella di un tipo di record.

* È possibile aggiungere una pagina Record collegati dall&#39;area di anteprima di un record o dalla pagina del record.

* Nelle pagine Record collegati vengono visualizzati solo gli oggetti o i record collegati di un oggetto o di un tipo di record. Nella pagina non vengono visualizzati tutti i record di quel tipo.

* È possibile visualizzare gli oggetti in una pagina di record collegati nella vista tabella.

<!--replace the above bullet with this: 

* You can display the objects in a connected records page in the following types of views:

   * Table
   * <span class="preview">Timeline</span>
   * <span class="preview">Calendar</span>

* <span class="preview">You can create one page per one object or record type. For example, you cannot create two connected record pages for connected projects or tactics.</span>

-->

* È possibile aggiungere pagine Record collegati per i tipi di oggetto o record connessi seguenti:

   * Tipi di record di Workfront Planning
   * Progetti Workfront

     Puoi visualizzare i progetti Workfront collegati anche se non disponi delle autorizzazioni necessarie per accedervi in Workfront.

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
<td> 
   <p> Prodotti aggiuntivi</p> </td> 
   <td> 
   <p> Oltre ad Adobe Workfront, per aggiungere una pagina di record connessa per gli oggetti delle seguenti applicazioni è necessario disporre dei seguenti elementi:</p>
   <ul><li><p>Una licenza Adobe Experience Manager Assets e un’integrazione tra AEM Assets e Workfront per collegare le risorse AEM ai tipi di record Planning.</p>
   <p>Per informazioni, consulta <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront for Experience Manager Assets and Assets Essentials: article index</a>. </p></li>
   <li><p> Una licenza Adobe GenStudio for Performance Marketing per collegare i tipi di record ai marchi GenStudio</p>
   <p>Per informazioni, vedere <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">Introduzione ad Adobe GenStudio for Performance Marketing</a>.</p></li></ul>
   </td> 
  </tr>

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

## Aggiungere una pagina Record connessi a un record

Prima di aggiungere una pagina record connessa a un record, è necessario collegare i tipi di record ad altri tipi di record o progetti Workfront.

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

1. (Facoltativo) Fare clic sul nome di un record o di un tipo di oggetto connesso nell&#39;elenco oppure cercarlo, quindi fare clic su di esso quando viene visualizzato nell&#39;elenco.

1. (Facoltativo e condizionale) Se nella visualizzazione tabella o nella pagina dei dettagli del record sono presenti più campi collegati, fare clic sul campo di cui si desidera visualizzare i record nella pagina record collegati.

   La visualizzazione tabella del tipo di record connesso selezionato viene aggiunta alla pagina record connessi.

1. (Facoltativo e condizionale) Quando si crea una pagina dei record connessi per i record di Planning connessi, eseguire una delle operazioni seguenti: <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

   * Fare clic sul nome di un record. Verrà aperta la pagina del record in una nuova scheda.
   * Fai clic su **Connetti** nella parte inferiore della visualizzazione tabella per connettere i record esistenti, selezionarli dalla casella di connessione, quindi fai clic all&#39;esterno della casella per chiuderla. I record vengono aggiunti automaticamente alla tabella. I record devono esistere prima di poterli aggiungere.

   Per ulteriori informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).
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

1. (Facoltativo e condizionale) Quando si crea una pagina di record connessi per i seguenti tipi di oggetti di Workfront:

   * Portfolio
   * Programmi
   * Gruppi
   * Aziende

   Eseguire una delle operazioni seguenti nella visualizzazione tabella della pagina dei record collegati:

   * Fare clic sul nome di un oggetto. Verrà aperta la pagina dell&#39;oggetto in una nuova scheda.
   * Fare clic su **Connetti** nella parte inferiore della visualizzazione tabella per connettere gli oggetti esistenti, selezionarli dalla casella di connessione, quindi fare clic all&#39;esterno della casella per chiuderla. Gli oggetti vengono aggiunti automaticamente alla tabella. Gli oggetti devono esistere prima di poterli aggiungere.

   Per ulteriori informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

   * Selezionate uno degli oggetti nella vista tabella, quindi fate clic su una delle seguenti opzioni nella barra blu nella parte inferiore dell&#39;elenco:

   * **Visualizza** per aprire la pagina record in una nuova scheda
   * **Copia collegamento** per copiare un collegamento nella pagina record
   * **Disconnetti** per disconnettere l&#39;oggetto dal record visualizzato.

   >[!TIP]
   >
   >È possibile selezionare più record o oggetti per disconnetterli.

1. (Facoltativo e condizionale) Quando si crea una pagina dei record connessi per i progetti Workfront connessi:

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

     >[!TIP]
     >
     >È possibile selezionare più progetti per disconnetterli o eliminarli.
   * Fai clic sull&#39;icona **+** nell&#39;angolo superiore destro della vista tabella per aggiungere campi esistenti alla tabella. I campi devono esistere prima di poterli aggiungere.

     Viene visualizzata la casella **Gestione colonne**. Effettua le seguenti operazioni:

      1. Cerca un campo oggetto esistente nella colonna **Available**, quindi fai clic su **+** a destra del nome del campo per aggiungerlo alla colonna **Selected**.

         I campi selezionati vengono aggiunti alla vista tabella della pagina record connessi.
      1. Fare clic su **-** a destra di un campo nella colonna **Selected** per rimuoverlo dalla vista tabella.
      1. Fai clic su **Salva** per salvare la visualizzazione della tabella della pagina record connessa.

1. (Facoltativo) Fare doppio clic sul nome della scheda **Record connessi**

   Oppure

   Passa il puntatore del mouse sul nome della scheda, quindi fai clic su **Altro** ![Altro menu](assets/more-menu.png), quindi su **Rinomina** per rinominare la nuova scheda Visualizzazione connessa.
1. (Facoltativo) Per gestire la vista tabella, utilizzare uno degli elementi di visualizzazione riportati di seguito nella barra degli strumenti di una pagina di record connessa:

   * Filtri
   * Ordina. Non disponibile per i progetti.
   * Raggruppamento. Non disponibile per i progetti.
   * Colonne, per visualizzare, nascondere o ridisporre i campi
   * Altezza riga. Non disponibile per i progetti.
   * Ricerca

   Per informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >Non è possibile creare, modificare o eliminare campi nella visualizzazione per tabella della scheda di un record connesso.

   <!--1. <span class="preview">(Optional) Click the dropdown menu to the right of the view name, then click **New view** to add a view. For more information, see the section [Manage multiple views from the connected records page](#manage-multiple-views-from-the-connected-records-page) in this article. </span>-->

1. (Facoltativo) Passa il puntatore del mouse sul nome della scheda della pagina Record connessi, fai clic su **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su **Elimina** per rimuoverlo dalla scheda.

<!--
<div class="preview">

## Manage multiple views from the connected records page

You can add and manage multiple view types from the connected records page of a record. 

The views you create in the Connected records page of a record type are available everywhere in Workfront Planning where that record type page displays. Views created for the same record type anywhere else in Workfront Planning are also accessible in all connected records pages of that record type. 

To manage multiple views from the connected records page: 

1. From the connected records page of a record, click the dropdown menu to the right of the view name, then click **New view** to add a view, then select from the following options: 

   * **Table**. For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 
   * **Timeline**. For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).
   * **Calendar**. For more information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md). 

1. (Optional) Hover over the name of a view in the Connected records page, then click the **More** menu ![More menu](assets/more-menu.png), then click one of the following: *************check to make sure these are all possible*********

   * **Rename**
   * **Share**. For more information, see [Share views](/help/quicksilver/planning/access/share-views.md).

   >[!TIP]
   >
   >Sharing views from Connected records pages makes them accessible to users in all areas of Workfront Planning where the view displays. 
   >Also, if a view is shared from any other area of Workfront Planning, it is also available to the same users in Connected records pages. 

   * **Export** 
   * **Duplicate**. For more information, see [Duplicate record views](/help/quicksilver/planning/views/duplicate-record-views.md).

      >[!TIP]
      >
      >Duplicating a view from Connected records pages makes it available in all other areas of Workfornt planning, when viewing the same record types. 

</div> -->