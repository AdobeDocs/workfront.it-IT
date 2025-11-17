---
title: Aggiungere una pagina Record collegati a un record
description: È possibile visualizzare informazioni da record o oggetti connessi aggiungendo a un record una scheda per la pagina Record connessi. In questo modo i record connessi in una vista tabella vengono aggiunti alla scheda.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 48bfeb3b950ca1149a919aa204d77db6aa501e01
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 1%

---


# Aggiungere una pagina Record connessi a un record

È possibile visualizzare informazioni da record o oggetti connessi aggiungendo a un record una scheda per la pagina Record connessi. In questo modo i record connessi in una vista tabella vengono aggiunti alla scheda.

Quando si aggiunge una pagina Record connessi a un record, tenere presente quanto segue:

* È possibile aggiungere una pagina Record collegati a un record dopo aver connesso tipi di record o di oggetti al tipo di record dalla vista tabella di un tipo di record.

* È possibile aggiungere una pagina Record collegati dall&#39;area di anteprima di un record o dalla pagina del record.

* Nelle pagine Record collegati vengono visualizzati solo gli oggetti o i record collegati di un oggetto o di un tipo di record in una visualizzazione tabella. Nella pagina non vengono visualizzati tutti i record di quel tipo.

* È possibile aggiungere pagine Record collegati per i tipi di oggetto o record connessi seguenti:

   * Tipi di record di Workfront Planning
   * Progetti, programmi, portfolio, gruppi o aziende di Workfront. È possibile visualizzare gli oggetti Workfront connessi anche se non si dispone delle autorizzazioni necessarie per accedervi in Workfront.

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