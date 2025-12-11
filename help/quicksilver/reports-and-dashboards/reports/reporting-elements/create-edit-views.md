---
product-area: reporting
navigation-topic: reporting-elements
title: Creare o modificare viste in Adobe Workfront
description: È possibile personalizzare il tipo di informazioni visualizzate sullo schermo utilizzando le viste. In Adobe Workfront è possibile utilizzare diversi tipi di visualizzazioni.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 0c0ffbeefb0eed8d1ca2a6e68ed19b40080726df
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 4%

---

# Creare o modificare viste in Adobe Workfront

<!-- Audited: 11/2024 -->

È possibile personalizzare il tipo di informazioni visualizzate sullo schermo utilizzando le viste. In Adobe Workfront è possibile utilizzare diversi tipi di visualizzazioni.

In questo articolo viene descritto come creare e modificare le visualizzazioni standard per elenchi e report.

Per ulteriori informazioni, vedere [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</strong></td> 
   <td> 
    <p>Collaboratore o versione successiva</p>
    <p>Richiedi o superiore</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Modifica l’accesso a Rapporti, Dashboard, Calendari per creare una visualizzazione in un rapporto</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un report per creare o modificare una visualizzazione in un report</p> <p>Gestire le autorizzazioni per una visualizzazione per modificarla</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Creare o personalizzare una visualizzazione

Il processo di creazione o personalizzazione di una vista varia a seconda che si stia creando o personalizzando una vista standard o una vista Agile o una vista Bacheca.

* [Creare o personalizzare una visualizzazione standard](#create-or-customize-a-standard-view)
* [Creare o personalizzare una visualizzazione Agile](#create-or-customize-an-agile-view)

### Creare o personalizzare una visualizzazione standard {#create-or-customize-a-standard-view}

Potete creare una nuova vista standard oppure personalizzare una vista standard esistente creata in precedenza.

1. Fare clic sul menu a discesa **Visualizza** in qualsiasi elenco in cui si desidera creare o personalizzare una visualizzazione.

1. Fare clic sul pulsante **+ Nuova visualizzazione** per creare una nuova visualizzazione.
Oppure
Fai clic sull&#39;icona **Modifica** ![Modifica](assets/edit-icon.png) visualizzata al passaggio del mouse a destra di una visualizzazione esistente che desideri modificare.
Viene visualizzata la finestra di dialogo **Personalizza visualizzazione**.

1. Nella sezione **Anteprima colonna** eseguire una delle operazioni seguenti:

   * Modificare il valore di una colonna facendo clic sul titolo della colonna e selezionando un nuovo campo.
   * Aggiungere una colonna facendo clic su **Aggiungi colonna**, digitare il nome della colonna che si desidera aggiungere, quindi fare clic su di essa quando viene visualizzata nell&#39;elenco a discesa.
   * Modificare l&#39;ordine di visualizzazione delle colonne trascinando il titolo della colonna in una nuova posizione.

   * Nell&#39;area **Impostazioni colonna** fare clic su **Riepiloga colonna per** e scegliere la modalità di visualizzazione dei dati nella colonna. Questa opzione è disponibile per i seguenti tipi di colonna:
     <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Campi data</strong></td> 
           <td><ul>
           <li>Massimo</li>
         <li>Minimo</li>
           </ul></td> 
          </tr> 
          <tr>
           <td role="rowheader"><strong>Campi valuta</strong></td> 
           <td><ul>
           <li>Conteggio</li>
         <li>Sum</li>
           <li>Medio</li>
         <li>Massimo</li>
           <li>Minimo</li>
         </ul></td> 
          </tr> 
         <tr>
           <td role="rowheader"><strong>Campi stringa e booleani</strong></td> 
           <td><ul><li>Conteggio</li></ul>
           <p>Nota: Workfront in genere non consiglia di riepilogare un campo booleano in base al conteggio, perché il valore sarà sempre true/false.</p></td> 
          </tr> 
         </tbody> 
        </table>

     >[!NOTE]
     >
     >Le eccezioni riportate di seguito si applicano agli oggetti padre, ad esempio i task padre, quando si riepilogano i valori dei campi seguenti nei raggruppamenti:
     >   
     > * Tutti i campi relativi al numero e alla divisa, ad eccezione delle ore effettive (ad esempio Costo manodopera pianificato/effettivo, Costo spesa pianificato/effettivo, Costo pianificato/effettivo, Ore pianificate), riepilogano i valori solo per le attività figlio e per le attività autonome. Non riepilogano i valori per le attività padre o i padri dei padri.
     > * Ore effettive riepiloga i valori per le attività padre principale e le attività autonome; non riepiloga i numeri per le attività padre o figlio.
     > * I campi dati personalizzati per i valori numerici e di valuta riepilogano tutte le attività: padri, figli, padri e attività autonome.
     >
     >Per ulteriori informazioni sull&#39;utilizzo dei raggruppamenti in un report, vedere l&#39;articolo [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Facoltativo) Fare clic su **Opzioni avanzate** per specificare le seguenti informazioni per la colonna:

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Etichetta colonna personalizzata</strong></td> 
           <td><p>Specifica un’etichetta personalizzata per la colonna. Questa etichetta sostituisce quella predefinita. Per evitare problemi di compatibilità, si consiglia di utilizzare solo caratteri UTF-8.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Formato campo</strong></td> 
           <td>Selezionare il formato in cui si desidera visualizzare i valori per i campi della colonna.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Mostra questa colonna quando in un dashboard</strong></td> 
           <td><p>Selezionare questa opzione per visualizzare questa colonna in un dashboard quando il report viene visualizzato affiancato a un altro report. Se questa opzione non è selezionata, questa colonna non viene visualizzata quando si visualizza il report su un dashboard in cui i report vengono visualizzati affiancati.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Regole colonna</strong></td> 
           <td><p>Fare clic su <strong>+ Aggiungi una regola per questa colonna</strong> per definire una regola per la colonna. Dopo aver aggiunto una regola, è possibile definire stili di campo e di testo per la visualizzazione dei campi corrispondenti alla regola. Fai clic su <strong>Aggiungi regola</strong> dopo aver completato la definizione della regola.</p></td> 
          </tr> 
         </tbody> 
        </table>

        Per ulteriori informazioni sulla formattazione condizionale delle visualizzazioni nei report, vedere l&#39;articolo [Utilizzare la formattazione condizionale in modalità testo](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

1. (Condizionale) Se hai selezionato **Opzioni avanzate**, fai clic su **Fine**.

1. Fai clic su **Salva visualizzazione** per creare una nuova visualizzazione o per sostituire la visualizzazione corrente con le modifiche.\
   Oppure\
   Fai clic su **Salva come nuova visualizzazione** per salvare le modifiche come nuova visualizzazione.

   >[!TIP]
   >
   >**Salva come nuova visualizzazione** è l&#39;unica opzione disponibile quando si personalizza una visualizzazione predefinita di Workfront.

   Il modo in cui la vista viene salvata dipende dal tuo accesso. Se la vista è stata creata in origine, è possibile salvare le modifiche; in caso contrario, viene richiesto di salvare una versione. Le modifiche apportate alla visualizzazione hanno un impatto sugli utenti con cui la visualizzazione è stata condivisa.

### Creare o personalizzare una visualizzazione Agile {#create-or-customize-an-agile-view}

Le visualizzazioni Agile, dette anche visualizzazioni bacheca, vengono visualizzate solo per gli elenchi di attività e problemi di un progetto.

Sono preconfigurati, ma puoi modificarne alcune impostazioni.

Per ulteriori informazioni sulle visualizzazioni Agile o Bacheca, consulta l&#39;articolo [Gestione di un progetto in Visualizzazione Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

<!-- Legacy Agile views were deprecated with 25.3. This is old: 

>[!NOTE]
>
>This procedure only applies to the legacy Agile view, not to the board view of a project.

To create or customize an Agile view:

1. Go to the list of tasks on a project.
1. Click the **Board** icon ![Board icon](assets/board-icon-for-agile-view.png), and then click **Use legacy agile** on the board view.

1. (Conditional) To customize an existing Agile view:

   1. Click the **View** drop-down menu, then select the Agile view you want to customize.  
      You cannot customize the default Agile view.
   
   1. Click the **View** drop-down menu again, then click **Customize View**.  
      ![Customize view](assets/view-agile-customize.png)

1. (Conditional) To create a new Agile view, click **New View**.  
   The **Customize Agile View** dialog box displays.  

1. In the **Customize Agile View** dialog box, specify a name for the Agile view.  
   We recommend that you include the word "Agile" in your view name, so users know this is an Agile view.  
   This name is displayed in the **View** drop-down menu when selecting a view.

1. Define the status columns to display on the story board in the agile view. These are the task statuses that are defined by the Workfront administrator, as described in [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Only system statuses are available to use on the Agile story board. If a status is available only for an individual group you are a member of, the status is not available on the agile story board. Furthermore, tasks that are in a status that is available only to a custom group are not visible when viewing the project in an Agile view.

   Users can move stories among these status columns on the Agile story board.  
   When defining status columns, you can do the following:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Reorder status columns:</strong> </td> 
      <td> Drag a status column to the order where you want it to appear.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Remove status columns:</strong> </td> 
      <td>Click the (x) icon on the column that you want to remove.<br>You cannot remove the "New" status unless a custom status has been added to the view and that custom status equates with "New."<br>For information about creating a custom status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Add status columns:</strong> </td> 
      <td> <p>Click the <strong>Plus</strong> icon, then select the status you want to add.<br>All default system statuses are displayed, as well as any custom statuses that have been shared with you.<br>You can configure up to 10 statuses to display.</p></td> 
     </tr> 
    </tbody> 
   </table>

   *********   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       *************

1. In the **Associate Card Color to** area, select from the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Story:</strong> </td> 
      <td>Any subtasks match the color of the parent task, so that the colors of all stories in any given swimlane are the same.<br>Colors are randomly assigned to tasks when they are created if the task does not have any subtasks or does not have a parent task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Free Form:</strong> </td> 
      <td> All cards are displayed as blue by default until a user changes the color manually, as described in the article <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorize stories by color on the Scrum board</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority:</strong> </td> 
      <td> <p> Colors are associated with the story priority, as follows:</p> 
       <ul> 
        <li>High = Red</li> 
        <li>Medium = Yellow</li> 
        <li>Low = Green<br>If your Workfront administrator has configured custom priorities for your Workfront system, the highest priority is red, the second-highest is yellow, and the remaining are green.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Task Owner:</strong> </td> 
      <td> All stories with the same primary assignee are the same color.<br>The primary assignee is the user who was first assigned to the task. </td> 
     </tr> 
    </tbody> 
   </table>

1. In the **Additional Fields** area, click **Add Field**, then select the field you want to add to story cards. (These are the same fields you can add when creating customizing a view or creating columns for a report.)  
   Repeat this process to add up to three additional fields to the story cards.  
   When you add fields to story cards, fields are view-only and display only when the field is populated.

   By default, the following types of data is displayed on the story card:

   * Story name with a link directly to the task
   * The project name with a link directly to the project  
     This link is displayed only when using the agile view on an iteration; it is not displayed when using an Agile view on a project.
   * The task description
   * Current commitment
   * View and edit the percent complete either by adjusting the percent complete itself or by adjusting the number of points or hours that are complete
   * Assigned Users

   You can display additional data (including custom data) on story cards. You might want to display additional fields on story cards for any number of reasons. For example, you might want to display the Customer ID if you are working on stories for multiple customers within the project, or you might want to display the Task Start Date.

1. Click **Save**.  
   Your access dictates how the view is saved. If you created the view originally, you can save the changes; otherwise, you are prompted to save a version. Keep in mind that changes you make to the view impact users with whom the view has been shared.

1. (Optional) Click the **List** icon to return to the list of tasks.

-->
