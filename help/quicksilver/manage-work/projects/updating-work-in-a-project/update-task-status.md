---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aggiorna Stato Attività
description: È possibile aggiornare lo stato di un'attività per informare gli altri utenti sulla posizione dell'attività (e del progetto complessivo) e sul relativo avanzamento.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 1%

---

# Aggiorna stato attività

<!--Audited: 10/2024-->

È possibile aggiornare lo stato di un&#39;attività per informare gli altri utenti sulla posizione dell&#39;attività (e del progetto complessivo) e sul relativo avanzamento.

Gli stati predefiniti sono Nuovo (New), In corso (In Progress) e Completo (Complete). Il tuo amministratore Adobe Workfront può aggiungere stati personalizzati per la tua organizzazione. Per ulteriori informazioni, vedere [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

È possibile aggiornare manualmente gli stati delle attività oppure consentire a Workfront di aggiornarli automaticamente quando si verificano determinate azioni.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Nuovo: Standard</p> 
   Oppure
   <p>Corrente: Lavoro o versione successiva</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Attività</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per l’attività</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sull&#39;aggiornamento dello stato delle attività

* Quando si contrassegna un&#39;attività come Completata, la percentuale di completamento dell&#39;attività viene aggiornata al 100%.
* Esistono i seguenti scenari per le attività padre:
   * Non è possibile aggiornare lo stato di un&#39;attività padre a Completo quando la modalità di completamento riepilogo del progetto è impostata su Automatico e le sottoattività non sono completate.
   * È possibile aggiornare lo stato di un&#39;attività padre impostandolo su Completo quando la modalità di completamento riepilogo del progetto è impostata su Manuale e le sottoattività sono completate o incomplete.

  Per ulteriori informazioni, vedere [Modifica progetti](../manage-projects/edit-projects.md).

## Aggiorna manualmente lo stato delle attività

È possibile aggiornare lo stato dell&#39;attività nelle seguenti aree:

* L&#39;intestazione dell&#39;attività nella pagina dell&#39;attività.
* Casella Modifica attività durante la modifica di un&#39;attività.
* La sezione Dettagli attività nella pagina dell&#39;attività.
* In un elenco di attività o in un report quando il campo Stato è visibile nella visualizzazione.
* Nel pannello Riepilogo dell’attività.

Per aggiornare manualmente lo stato dell&#39;attività nell&#39;intestazione dell&#39;attività:

1. Passare a un&#39;attività per la quale si desidera aggiornare lo stato.
1. Nell&#39;intestazione dell&#39;attività fare clic sul campo **Stato** e selezionare un nuovo stato.
1. Per fornire un&#39;indicazione visiva del completamento dell&#39;attività, trascina la bolla sotto **Percentuale completata** nell&#39;intestazione dell&#39;attività.

   Oppure

   Fai doppio clic all&#39;interno della bolla **Percent Complete** per immettere manualmente una nuova percentuale.

   ![](assets/percent-complete-status-widgets-task-header.png)

1. (Facoltativo) Per fornire ulteriori informazioni sull&#39;aggiornamento, effettuare una delle seguenti operazioni:

   * Per aggiungere una nota sull&#39;aggiornamento, vai alla sezione **Aggiornamenti** e fai clic su **Nuovo commento**, quindi digita una nota.

     ![Aggiunta di un aggiornamento a un&#39;attività](assets/add-update-to-task.png)

   * Per notificare l&#39;aggiornamento ad alcuni utenti, digitarne il nome nel campo **Assegna tag a persone o team** visualizzato quando si digita un commento. Per ulteriori informazioni, consulta [Assegnare tag ad altri in occasione di aggiornamenti](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Per aggiornare la data di conferma dell&#39;attività, fare clic su **Dettagli attività**, quindi modificare il campo **Data conferma**. Per informazioni, vedere [Modifica attività](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md).


   >[!IMPORTANT]
   >
   >  Solo gli assegnatari delle attività possono aggiornare la Data di conferma.

<!--old functionality in old commenting: 

1. Go to a task that you are assigned to for which you want to update the status.
1. Click the **Status** field in the task header and select a new status. 
1. (Optional) Do any of the following to provide additional information about the update, then click **Update** or, if the task has the **Complete** status, click **Done:**

   * To add a note about the update, go to the **Updates** area and click **Start a new update**, then type your note.  

   * To notify certain users about the update, type their names in the **Notify** box that appears when you type a note about the update. For more information, see [Tag others on updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md). 
   * To update the condition of the task, click **Select Condition** to the right of the **Notify** box (these appear when you type a note about the update), then select the condition that best reflects the current condition of the task.
   
   * To update the Commit Date of the task, expand the **Commit Date** drop-down calendar, and select a new Commit Date. 
   * To provide a visual indication of task completion, drag the bubble under Percent Complete or double-click it to enter a percent value.   
     ![](assets/drag-the-progress-bar-350x155.png)-->

## Aggiorna automaticamente lo stato delle attività

Workfront aggiorna automaticamente lo stato esistente di un&#39;attività a un altro stato quando si verificano le azioni elencate nella tabella seguente.

>[!NOTE]
>
>Gli stati riportati nella tabella seguente sono stati di sistema predefiniti. L’amministratore di Workfront o un amministratore di gruppo può rinominare gli stati nell’istanza di Workfront. Per informazioni sulla creazione e la gestione degli stati in Workfront, vedere [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Azione</b></td> 
   <td><b>Stato originale</b></td> 
   <td><b>Nuovo stato</b></td> 
  </tr> 
  <tr> 
   <td>Aggiorna la percentuale di completamento dell'attività al 100%</td> 
   <td>Nuovo o in corso</td> 
   <td>Completato</td> 
  </tr> 
  <tr> 
   <td>Aggiorna la percentuale di completamento dell'attività da 100% a un numero inferiore</td> 
   <td>Completato</td> 
   <td>In corso</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Fare clic sul pulsante Avvia attività per accettare di lavorare su un'attività assegnata a te</span> </td> 
   <td><span>Nuovo</span> </td> 
   <td> <p>Qualsiasi stato associato al pulsante Avvia attività nelle impostazioni del team predefinito.</p> <p>Per informazioni sulla sostituzione del pulsante Lavoraci con un pulsante Avvia attività, vedere <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Sostituire il pulsante Lavoraci con un pulsante Avvia</a></span>.</p> <p>Suggerimento: <span>Facendo clic</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">sul pulsante Annulla</span> dopo aver fatto clic su Avvia attività, lo stato viene ripristinato su Nuovo. </p> </td> 
  </tr> 
 </tbody> 
</table>
