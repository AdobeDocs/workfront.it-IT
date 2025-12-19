---
title: Aggiungere una pagina Record collegati a un record
description: È possibile visualizzare informazioni da record o oggetti connessi aggiungendo a un record una scheda per la pagina Record connessi. In questo modo i record connessi in una vista tabella vengono aggiunti alla scheda.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '2743'
ht-degree: 0%

---


# Aggiungere una pagina Record connessi a un record

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

È possibile visualizzare informazioni da record o oggetti connessi aggiungendo una scheda per una pagina Record connessi a un record in Adobe Workfront Planning. In questo modo i record connessi in una vista tabella vengono aggiunti alla scheda.

Quando si aggiunge una pagina Record connessi a un record, tenere presente quanto segue:

* È possibile aggiungere una pagina Record collegati a un record dopo aver connesso tipi di record o di oggetti al tipo di record dalla relativa vista tabella.

* È possibile aggiungere una pagina Record collegati dall&#39;area di anteprima di un record o dalla pagina del record.

* <span class="preview">È possibile avere una sola pagina di record connessi per un tipo di record specifico.</span>

  <span class="preview">Ad esempio, se si crea una pagina di record connessi per una campagna e si desidera visualizzare i relativi utenti tipo connessi, è possibile disporre di una sola pagina di record connessi per gli utenti tipo.</span>

* Nelle pagine Record collegati vengono visualizzati solo gli oggetti o i record collegati di un oggetto o di un tipo di record. Nella pagina non vengono visualizzati tutti i record di quel tipo.

* A seconda dell&#39;oggetto o del tipo di record visualizzato nella pagina record connessi, è possibile visualizzarli utilizzando le visualizzazioni seguenti:

   * È possibile visualizzare i record di Planning connessi nelle seguenti viste:
      * Tabella
      * <span class="preview">Timeline</span>
      * <span class="preview">Calendario</span>
   * È possibile visualizzare i progetti Workfront connessi nella vista a elenco.

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

1. Aggiungi **Nome pagina**, fai clic su **Pagina record connessi** per il **Tipo pagina**, quindi fai clic su **Crea**.
1. (Facoltativo) Fare clic sul nome di un record o di un tipo di oggetto connesso nell&#39;elenco oppure cercarlo, quindi fare clic su di esso quando viene visualizzato nell&#39;elenco per creare la pagina per il record o il tipo di oggetto.

   >[!TIP]
   >
   ><span class="preview">È possibile creare una pagina di record connessi per tipo di record. Se un tipo di record connesso dispone già di una pagina, non verrà più visualizzato come opzione.</span>
   >

1. (Facoltativo e condizionale) Se più campi collegati del record o del tipo di oggetto per cui si sta creando la pagina vengono visualizzati, fare clic sul campo di cui si desidera visualizzare i record o gli oggetti nella pagina dei record connessi dall&#39;elenco **Seleziona campo di riferimento**.

   ![Seleziona elenco campi di riferimento](assets/select-reference-field-list-on-connected-records-page.png)

   Alla pagina dei record connessi viene aggiunta una delle pagine seguenti:

   * Visualizzazione tabella di un tipo di record
   * Visualizzazione elenco di un tipo di oggetto progetto

   I record o i progetti connessi al record corrente vengono visualizzati nella vista a tabella o a elenco.

   >[!TIP]
   >
   >È necessario aggiungere i record connessi nella tabella o nell&#39;area Dettagli di un record prima di visualizzarli in una pagina dei record connessi. In caso contrario, la tabella o l&#39;elenco sono vuoti.

   I primi cinque campi dei record connessi vengono visualizzati per impostazione predefinita. Per impostazione predefinita, non viene visualizzato alcun campo di ricerca.

   ![Visualizzazione tabella connessa al pubblico nei dettagli della campagna](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Condizionale) A seconda del tipo di record visualizzato nella pagina record connesso, eseguire una delle operazioni seguenti:

   * Gestisci record di Planning
Per informazioni, vedere la sezione [Gestire la pagina dei record connessi per i record di Planning](#manage-the-connected-records-page-for-planning-records) in questo articolo.
   * Gestire i progetti Workfront
Per informazioni, vedere la sezione [Gestire la pagina dei record connessi per i progetti Workfront](#manage-the-connected-records-page-for-workfront-projects) in questo articolo.

1. (Facoltativo) Fare doppio clic sul nome della scheda **Record connessi**

   Oppure

   Passa il puntatore del mouse sul nome della scheda, quindi fai clic su **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su **Rinomina** per rinominare la scheda della pagina dei nuovi record connessi.

1. (Facoltativo) Passa il puntatore del mouse sul nome della scheda della pagina dei record connessi, fai clic su **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su **Elimina** per rimuoverlo dalla scheda.

### Gestione della pagina dei record connessi per i record di Planning

La gestione della pagina dei record connessi per i record di Planning varia a seconda dell&#39;ambiente utilizzato.

#### Gestione della pagina dei record connessi per i record di Planning nell&#39;ambiente di produzione

Quando si crea una pagina dei record connessi per i record di Planning connessi nell&#39;ambiente di produzione, eseguire le operazioni seguenti: <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

1. Passare a una pagina del tipo di record e fare clic sul nome di un record. Verrà aperta la pagina di anteprima del record.
1. Fare clic sulla scheda di una pagina di record connessi in cui vengono visualizzati i record di Planning.
I record collegati al record selezionato vengono visualizzati nella vista tabella.
1. Fai clic su **Connetti** nella parte inferiore della visualizzazione tabella per connettere i record esistenti, selezionarli dalla casella di connessione, quindi fai clic all&#39;esterno della casella per chiuderla. I record vengono aggiunti automaticamente alla tabella e collegati al record selezionato. I record devono esistere prima di poterli aggiungere.

   Per ulteriori informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

1. Modificare le informazioni dei record collegati in linea nella vista tabella.
1. Passa il puntatore del mouse sul nome di un record connesso, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png)

   Oppure

   Selezionare uno dei record, quindi fare clic su una delle opzioni seguenti nella barra blu nella parte inferiore dell&#39;elenco:

   * **Visualizza** per aprire la pagina record in una nuova scheda
   * **Copia collegamento** per copiare un collegamento nella pagina record
   * **Modifica miniatura** per aprire la casella **Miniatura record** e modificare l&#39;immagine miniatura del record
   * **Duplicato** per duplicare il record connesso. Il record duplicato è anche collegato al record corrente.
   * **Inserire un record superiore o inferiore** per aggiungere nuovi record al tipo di record connesso. Anche i nuovi record aggiunti qui sono collegati al record corrente. Questa opzione non è disponibile nella barra blu quando si seleziona un record nella tabella.
   * **Elimina** per eliminare il record. Se si elimina un record connesso, questo viene eliminato dal relativo tipo di record e da qualsiasi posizione in cui il record è connesso. I record eliminati vengono spostati nel contenitore **Eliminati di recente** del relativo tipo di record.

     Per informazioni sulla modifica dei record nella vista tabella, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

     >[!TIP]
     >
     >È possibile selezionare più record o oggetti per eliminarli.
     >

1. Modifica in linea qualsiasi record della tabella nella pagina dei record connessi.
1. Utilizzare uno degli elementi di visualizzazione riportati di seguito nella barra degli strumenti di una pagina di record connessa per gestire la visualizzazione tabella.

   * **Filtri**
   * **Ordina**
   * **Raggruppamento**
   * **Campi**, per visualizzare, nascondere o ridisporre i campi
   * **Altezza riga**
   * **Ricerca**

   Per informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >Non è possibile creare, modificare o eliminare campi nella visualizzazione per tabella della scheda di un record connesso.
   >

<div class="preview">

#### Gestire la pagina dei record collegati per i record di Planning nell&#39;ambiente di anteprima

Quando si crea una pagina dei record connessi per i record di Planning connessi nell&#39;ambiente di anteprima, eseguire le operazioni seguenti: <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

1. Passare a una pagina del tipo di record e fare clic sul nome di un record. Verrà aperta la pagina di anteprima del record.
1. Fare clic sulla scheda di una pagina di record connessi in cui vengono visualizzati i record di Planning.
I record collegati al record selezionato vengono visualizzati nella vista tabella.
1. Fare clic su **Connetti record** nell&#39;angolo superiore destro della pagina dei record connessi per connettere i record esistenti, selezionarli dalla casella di connessione, quindi fare clic all&#39;esterno della casella per chiuderla. I record vengono aggiunti automaticamente alla tabella e collegati al record selezionato. I record devono esistere prima di poterli aggiungere.

   Per ulteriori informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

1. Fai clic su **Nuova riga** nella parte inferiore della tabella per aggiungere nuovi record. I nuovi record vengono automaticamente connessi ai record selezionati.
1. Modificare le informazioni dei record collegati in linea nella vista tabella.
1. Passa il puntatore del mouse sul nome di un record connesso, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png)

   Oppure

   Selezionare uno dei record, quindi fare clic su una delle opzioni seguenti nella barra blu nella parte inferiore dell&#39;elenco:

   * **Visualizza** per aprire la pagina record in una nuova scheda
   * **Copia collegamento** per copiare un collegamento nella pagina record
   * **Modifica miniatura** per aprire la casella **Miniatura record** e modificare l&#39;immagine miniatura del record
   * **Duplicato** per duplicare il record connesso. Il record duplicato è anche collegato al record corrente.
   * **Inserire un record superiore o inferiore** per aggiungere nuovi record al tipo di record connesso. Anche i nuovi record aggiunti qui sono collegati al record corrente. Questa opzione non è disponibile nella barra blu quando si seleziona un record nella tabella.
   * **Elimina** per eliminare il record. Se si elimina un record connesso, questo viene eliminato dal relativo tipo di record e da qualsiasi posizione in cui il record è connesso. I record eliminati vengono spostati nel contenitore **Eliminati di recente** del relativo tipo di record.

     Per informazioni sulla modifica dei record nella vista tabella, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

     >[!TIP]
     >
     >È possibile selezionare più record o oggetti per eliminarli.

1. Modifica in linea qualsiasi record della tabella nella pagina dei record connessi.
1. Utilizzare uno degli elementi di visualizzazione riportati di seguito nella barra degli strumenti di una pagina di record connessa per gestire la visualizzazione tabella.

   * **Filtri**
   * **Ordina**
   * **Raggruppamento**
   * **Campi**, per visualizzare, nascondere o ridisporre i campi
   * **Altezza riga**
   * **Ricerca**

   Per informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >Non è possibile creare, modificare o eliminare campi nella visualizzazione per tabella della scheda di un record connesso.
   >

1. Fare clic sul menu a discesa delle visualizzazioni e quindi su **Nuova visualizzazione** per aggiungere una nuova visualizzazione alla pagina, quindi eseguire le operazioni seguenti:

   1. Aggiungi **Nome visualizzazione**.
   1. Nell&#39;area **Tipo di visualizzazione** selezionare uno dei tipi di visualizzazione seguenti:

      * Tabella
Per informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md)
      * Timeline
Per informazioni, vedere [Gestire la visualizzazione della sequenza temporale](/help/quicksilver/planning/views/manage-the-timeline-view.md).
      * Calendario
Per informazioni, vedere [Gestire la visualizzazione del calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md).

        Per ulteriori informazioni, vedere la sezione [Gestire più visualizzazioni dalla pagina dei record connessi](#manage-multiple-views-from-the-connected-records-page) in questo articolo.

   1. Fai clic su **Crea**.
Una nuova vista viene aggiunta al menu a discesa delle viste.

   1. (Facoltativo) Passa il puntatore del mouse sul nome di una visualizzazione creata, fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su una delle seguenti opzioni:

      * **Rinomina**, per aggiungere un nuovo nome alla visualizzazione.
      * **Condividi**

        Per ulteriori informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).

        >[!NOTE]
        >
        >Non è possibile condividere una visualizzazione Sistema creata da Workfront.

      * **Elimina**
Per informazioni, vedere [Eliminare le visualizzazioni dei record](/help/quicksilver/planning/views/delete-record-views.md).

        ![](assets/view-more-menu-projects-connected-records-page.png)

</div>

### Gestione della pagina dei record collegati per i progetti Workfront

Quando si crea una pagina record connessi per progetti Workfront connessi, eseguire le operazioni seguenti:

1. Passare a una pagina del tipo di record e fare clic sul nome di un record. Verrà aperta la pagina di anteprima del record.
1. Fare clic sulla scheda di una pagina relativa ai record connessi in cui sono visualizzati i progetti Workfront.
I progetti connessi al record selezionato vengono visualizzati nella vista a elenco.
1. Fare clic su **Connetti record** nell&#39;angolo superiore destro della pagina dei record connessi per connettere i progetti esistenti.

   Per informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).
1. Modifica in linea le informazioni sul progetto nella tabella.
1. Fai clic su **Nuova riga** per creare un progetto senza modello. Il nuovo progetto viene automaticamente connesso al record corrente.

   Per ulteriori informazioni, vedere [Creare oggetti Workfront da Workfront Planning durante la connessione ai record](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md).

1. Passa il puntatore del mouse sul nome di un progetto nell&#39;elenco e fai clic sul menu **Altro** [Altro menu](assets/more-menu.png)

   Oppure

   Seleziona uno o più progetti e osserva la barra blu nella parte inferiore dell’elenco, quindi fai clic su una delle seguenti opzioni:

   * **Elimina** per eliminare il progetto. Quando si elimina un progetto, questo viene disconnesso dal record e spostato nel Cestino di Workfront. Gli amministratori di Workfront possono recuperare i progetti eliminati fino a 30 giorni dopo la loro eliminazione.
   * **Disconnetti** per disconnettere il progetto dal record. Se si disconnette un progetto, verranno rimossi anche tutti i valori dei campi di ricerca dal record corrente.

     >[!TIP]
     >
     >È possibile selezionare più progetti per disconnetterli o eliminarli.
     >

1. Fare clic sul menu a discesa delle visualizzazioni e quindi su **Nuova visualizzazione** per aggiungere una nuova visualizzazione alla pagina, quindi eseguire le operazioni seguenti:

   1. Aggiungi **Nome visualizzazione**.
   1. Selezionare **Elenco** dall&#39;area **Tipo di visualizzazione**.
   1. Fai clic su **Crea**.
Al menu a discesa delle viste viene aggiunta una nuova vista a elenco.

      Per ulteriori informazioni, vedere la sezione [Gestire più visualizzazioni dalla pagina dei record connessi](#manage-multiple-views-from-the-connected-records-page) in questo articolo.

   1. (Facoltativo) Passa il puntatore del mouse sul nome di una visualizzazione creata, fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su una delle seguenti opzioni:
      * **Rinomina**, per aggiungere un nuovo nome alla visualizzazione.
      * <span class="preview">**Condividi**</span>

        Per ulteriori informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).

        >[!NOTE]
        >
        >Non è possibile condividere una visualizzazione Sistema creata da Workfront.

      * **Elimina**
Per informazioni, vedere [Eliminare le visualizzazioni dei record](/help/quicksilver/planning/views/delete-record-views.md).

        ![](assets/view-more-menu-projects-connected-records-page.png)

   1. Fai clic sull&#39;icona **Filtro** ![Icona Filtro](assets/filter-icon.png) e utilizza il filtro per visualizzare progetti specifici.

      >[!TIP]
      >
      ><span class="preview">Per i campi di tipo persone, come **Proprietario** o **Sponsor**, è possibile utilizzare un carattere jolly per visualizzare i progetti a cui l&#39;utente connesso è assegnato a questi ruoli.</span>
      >
      >![Filtra con carattere jolly utente per la pagina dei record connessi al progetto](assets/filter-with-user-wildcard-project-connected-records-page.png)
      >

   1. Fai clic sull&#39;icona **Colonne** ![Icona Colonne](assets/columns-icon.png) per nascondere o visualizzare le colonne nell&#39;elenco.
   1. Fai clic sull&#39;icona **+** nell&#39;angolo superiore destro della vista tabella per aggiungere campi esistenti alla tabella. I campi devono esistere prima di poterli aggiungere.

      Viene visualizzata la casella **Gestione colonne**. Effettua le seguenti operazioni:

      1. Cerca un campo oggetto esistente nella colonna **Available**, quindi fai clic su **+** a destra del nome del campo per aggiungerlo alla colonna **Selected**.

         I campi selezionati vengono aggiunti alla vista tabella della pagina record connessi.
      1. Fare clic su **-** a destra di un campo nella colonna **Selected** per rimuoverlo dalla vista tabella.
      1. Fai clic su **Salva** per salvare la visualizzazione della tabella della pagina record connessa.


<div class="preview">

## Gestire più visualizzazioni dalla pagina dei record collegati

È possibile aggiungere e gestire più tipi di visualizzazione dalla pagina record connessi di un record.

Le visualizzazioni create nella pagina Record collegati di un tipo di record sono disponibili ovunque in Workfront Planning, dove viene visualizzata la pagina del tipo di record. Le visualizzazioni create per lo stesso tipo di record in qualsiasi altro punto di Workfront Planning sono accessibili anche in tutte le pagine di record collegate di quel tipo di record.

Per gestire più visualizzazioni dalla pagina dei record collegati:

1. Dalla pagina record connessi di un record, fare clic sul menu a discesa a destra del nome della visualizzazione, quindi fare clic su **Nuova visualizzazione** per aggiungere una visualizzazione, quindi selezionare una delle opzioni seguenti:

   * **Tabella**. Per ulteriori informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).
   * **Timeline**. Per ulteriori informazioni, vedere [Gestire la visualizzazione della sequenza temporale](/help/quicksilver/planning/views/manage-the-timeline-view.md).
   * **Calendario**. Per ulteriori informazioni, vedere [Gestire la visualizzazione del calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md).

1. (Facoltativo) Passa il puntatore del mouse sul nome di una visualizzazione nella pagina Record connessi, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su una delle seguenti opzioni:

   * **Rinomina**
   * **Condividi**. Per ulteriori informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).

   >[!TIP]
   >
   >La condivisione delle visualizzazioni dalle pagine Record connessi consente di renderle accessibili agli utenti in tutte le aree di Workfront Planning in cui viene visualizzata la visualizzazione.
   >Inoltre, se una visualizzazione è condivisa da qualsiasi altra area di Workfront Planning, è disponibile anche per gli stessi utenti nelle pagine Record connessi.

   * **Esporta**
   * **Duplicato**. Per ulteriori informazioni, vedere [Visualizzazioni record duplicate](/help/quicksilver/planning/views/duplicate-record-views.md).

     >[!TIP]
     >
     >La duplicazione di una visualizzazione dalle pagine Record collegati la rende disponibile in tutte le altre aree di Workfront Planning quando si visualizzano gli stessi tipi di record.

</div>

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
      TIP      
      You can select more than one record or object to disconnect them.
      -->