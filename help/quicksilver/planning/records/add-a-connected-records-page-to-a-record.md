---
title: Aggiungere una pagina Record collegati a un record
description: È possibile visualizzare informazioni da record o oggetti connessi aggiungendo a un record una scheda per la pagina Record connessi. In questo modo i record connessi in una vista tabella vengono aggiunti alla scheda.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 54ba4509269784ebe25fb5283b539c440454362a
workflow-type: tm+mt
source-wordcount: '1577'
ht-degree: 0%

---


# Aggiungere una pagina Record connessi a un record

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

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

1. (Facoltativo) Fare clic sul nome di un record o di un tipo di oggetto connesso nell&#39;elenco oppure cercarlo, quindi fare clic su di esso quando viene visualizzato nell&#39;elenco per creare la pagina per il record o il tipo di oggetto.

1. (Facoltativo e condizionale) Se più campi connessi del tipo di record per cui si sta creando la pagina vengono visualizzati, fare clic sul campo di cui si desidera visualizzare i record nella pagina record connessi.

   Alla pagina dei record connessi viene aggiunta una delle pagine seguenti:

   * Visualizzazione tabella di un tipo di record
   * Visualizzazione elenco di un tipo di oggetto progetto

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

   * In linea modificare qualsiasi record di Planning nella tabella della pagina dei record collegati.
   * Utilizzare uno degli elementi di visualizzazione riportati di seguito nella barra degli strumenti di una pagina di record connessa per gestire la visualizzazione tabella.

   * **Filtri**
   * **Ordina**. Non disponibile per i progetti.
   * **Raggruppamento**. Non disponibile per i progetti.
   * **Campi**, per visualizzare, nascondere o ridisporre i campi
   * **Altezza riga**. Non disponibile per i progetti.
   * **Ricerca**

     Per informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

     >[!NOTE]
     >
     >Non è possibile creare, modificare o eliminare campi nella visualizzazione per tabella della scheda di un record connesso.

   <!--No longer possible: 1. (Optional and conditional) When you create a connected records page for the following Workfront object types:
         * Portfolios
         * Programs
         * Groups
         * Companies
      Do any of the following in the table view of the connected records page: 
      * Click the name of a object. This opens the object's page in a new tab. 
      * Click **Connect** at the bottom of the table view to connect existing objects, select them from the connection box, then click outside the box to close it. The objects are automatically added to the table. The objects must exist before you can add them.
      For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
      * Select one of the objects in the table view, then click one of the following options in the blue bar at the bottom of the list: 
      * **View** to open the record page in a new tab
      * **Copy link** to copy a link to the record page
      * **Disconnect** to disconnect the object from the record you are viewing. 
      >[!TIP]
      >
      >You can select more than one record or object to disconnect them.
      -->
1. (Facoltativo e condizionale) Quando si crea una pagina dei record connessi per i progetti Workfront connessi, eseguire una delle operazioni seguenti:

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
   * Fare clic sul menu a discesa delle visualizzazioni e quindi su **Nuova visualizzazione** per aggiungere una nuova visualizzazione alla pagina, quindi eseguire le operazioni seguenti:
      1. Aggiungi **Nome visualizzazione**.
      1. Selezionare **Elenco** dall&#39;area **Tipo di visualizzazione**.
      1. Fai clic su **Crea**.
Al menu a discesa delle viste viene aggiunta una nuova vista a elenco.
      1. (Facoltativo) Passa il puntatore del mouse sul nome di una visualizzazione creata, fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su una delle seguenti opzioni:

         * **Rinomina**, per aggiungere un nuovo nome alla visualizzazione.
         * <span class="preview">**Condividi**</span>
Per ulteriori informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).
         * **Elimina**
Per informazioni, vedere [Eliminare le visualizzazioni dei record](/help/quicksilver/planning/views/delete-record-views.md).

           ![](assets/view-more-menu-projects-connected-records-page.png)
   * Fai clic sull&#39;icona **Filtro** ![Icona Filtro](assets/filter-icon.png) e utilizza il filtro per visualizzare progetti specifici.

     >[!TIP]
     >
     ><span class="preview">Per i campi di tipo persone, come **Proprietario** o **Sponsor**, è possibile utilizzare un carattere jolly per visualizzare i progetti a cui l&#39;utente connesso è assegnato a questi ruoli.</span>
     >
     >![Filtra con carattere jolly utente per la pagina dei record connessi al progetto](assets/filter-with-user-wildcard-project-connected-records-page.png)
     >
   * Fai clic sull&#39;icona **Colonne** ![Icona Colonne](assets/columns-icon.png) per nascondere o visualizzare le colonne nell&#39;elenco.
   * Fai clic sull&#39;icona **+** nell&#39;angolo superiore destro della vista tabella per aggiungere campi esistenti alla tabella. I campi devono esistere prima di poterli aggiungere.

     Viene visualizzata la casella **Gestione colonne**. Effettua le seguenti operazioni:

      1. Cerca un campo oggetto esistente nella colonna **Available**, quindi fai clic su **+** a destra del nome del campo per aggiungerlo alla colonna **Selected**.

         I campi selezionati vengono aggiunti alla vista tabella della pagina record connessi.
      1. Fare clic su **-** a destra di un campo nella colonna **Selected** per rimuoverlo dalla vista tabella.
      1. Fai clic su **Salva** per salvare la visualizzazione della tabella della pagina record connessa.
1. (Facoltativo) Fare doppio clic sul nome della scheda **Record connessi**

   Oppure

   Passa il puntatore del mouse sul nome della scheda, quindi fai clic su **Altro** ![Altro menu](assets/more-menu.png), quindi su **Rinomina** per rinominare la nuova scheda Visualizzazione connessa.


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