---
product-previous: workfront-goals
navigation-topic: goal-management
title: Aggiornare gli obiettivi nel pannello Dettagli obiettivo in Obiettivi di Adobe Workfront
description: Per aggiornare le informazioni per i singoli obiettivi, accedi al pannello Dettagli obiettivo.
author: Alina
feature: Workfront Goals
exl-id: e9df0d98-05a1-4977-b7f1-426b8f5b3eae
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 1%

---

# Aggiornare gli obiettivi nella sezione dei dettagli Obiettivo in Obiettivi di Adobe Workfront

<!--drafted for the goal redesign:
- change the title for Production to Update goals in the Goal details section in Adobe Workfront Goals. 
- update the description in the metadata above
-->

Per aggiornare le informazioni per i singoli obiettivi, accedi al pannello Dettagli obiettivo.

>[!NOTE]
>
>Non è possibile aggiornare obiettivi con stato Chiuso.


## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> 
   <p>Per il nuovo piano e la nuova struttura delle licenze:
  <ul><li>Un piano Ultimate </li></ul>
   </p>
<p>Per il piano corrente e la struttura delle licenze: 
<ul><li> A Pro o superiore </li>
  <li>Una licenza Adobe Workfront Goals oltre a una licenza Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licenza Adobe Workfront*</td>
 <td>
 <p>Nuova licenza: Collaboratore o versione successiva</p>
 Oppure
 <p>Licenza corrente: richiesta o successiva</p> <p>Per ulteriori informazioni, vedere <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica delle licenze di Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Prodotto*</td>
 <td>
 <p> Nuovo requisito del prodotto, uno dei seguenti: </p>
<ul>
<li>Un piano Select o Prime Adobe Workfront e un’ulteriore licenza Adobe Workfront Goals.</li>
<li>Un piano Workfront Ultimate che include gli obiettivi Workfront per impostazione predefinita. </li></ul>
 <p>Oppure</p>
 <p>Fabbisogno di prodotto corrente: un piano Workfront e una licenza aggiuntiva per gli obiettivi Adobe Workfront. </p> <p>Per informazioni, vedere <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisiti per l'utilizzo degli obiettivi di Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Livello di accesso*</td>
 <td> <p>Modifica accesso agli obiettivi</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorizzazioni oggetto</td>
 <td>
  <div>
  <p>Visualizza o autorizzazioni superiori per l’obiettivo per visualizzarlo</p>
  <p>Gestire le autorizzazioni per l’obiettivo per modificarlo</p>
  <p>Per informazioni sulla condivisione degli obiettivi, vedere <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Condividere un obiettivo in Obiettivi di Workfront</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l’area Obiettivi nel menu principale. </p>  
</td>
  </tr>
</tbody>
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Aggiornare gli obiettivi nella sezione Dettagli obiettivo

Puoi accedere a un singolo obiettivo da un elenco di obiettivi.

<!--

Updating goals in the Goal Details panel differs depending on where you access the goal from. 

### Update goals in the Goal Details panel in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Goals area in Workfront. 

1. Click the name of a goal in the Goal List, then click the name of a goal.

   This opens the Goal Details panel on the right.
   ![](assets/goal-details-summary-tab-350x294.png)

   >[!TIP]
   >
   >You can also click the name of a goal in the Goal Alignment, Check-in, or Pulse sections. 
   >
   ><!-- drafted for goal redesign:
   >Add this to the TIP above with goal redesign: 
   >
   >The Check-in and Pulse sections have been removed from the Preview environment.
   >

1. On the Summary tab, click the **More icon** ![](assets/more-icon.png), then click any of the following options:

   1. **Edit**. For information about editing goals, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
   1. **Copy**. For information about copying goals, see [Copy goals in Adobe Workfront Goals](../../workfront-goals/goal-management/copy-goals.md).
   1. **Activate**. This option is available only for drafted and inactive goals.

      For information about activating goals, see [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md). 
   
   1. **Close**, then click**Close Goal**. This option is available only for active goals.

      For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. **Deactivate**. This option is available only for active goals. This deactivates the goal immediately.

      For information about deactivating goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).
   
   1. **Delete**, then click **Yes, Delete**.

      For information about deleting goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

      >[!NOTE]
      >
      >Deleted goals cannot be recovered.

   1. **Reopen**, then click **Reopen**. This option is available only for closed goals that are from a current time period.

      For information about reopening goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. (Conditional) If you clicked any of the options between steps a-i above except Delete or Reopen, click **Save**.    
   
      (!--ensure this is accurate)--)

1. Click **Align to another goal** in the upper-right of the Summary tab, then specify the name of a goal in the **Align to** **another goal** field that you want to align the current goal to. The current goal becomes the child of the goal you align it to. For information about child and parent goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md). 
1. Click **Add results**. Results drive the progress of your goal. For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).

1. Click **Add activities**. Activities drive the progress of your goal. For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 

1. Click the **Updates** tab. Here, you can view goal comments and review the entire editing history of the goal, activities, and results, to understand who changed what and when.

   ![](assets/goal-details-updates-tab-350x280.png)

1. (Optional) Deselect any of the following options if you want to not display them in the Updates tab.&nbsp;They are selected by default: 

   | Option |Description  |
   |---|---|
   | Progress Updates |Displays information about the history of progress updates on results and activities.  |
   | Comments |Displays comments made by users on the goal.  |
   | Editing History |Displays information about creating and updating the goal, results, and activities.  |

1. (Optional) Click **Details** under a progress or an editing history update to display additional information about the update.

   ![](assets/update-details-in-updates-tab-expanded-highlighted-350x139.png)

-->



1. Fai clic sul nome di un obiettivo nell’Elenco obiettivi, quindi fai clic sul nome di un obiettivo.

   Verrà aperta la sezione **Dettagli obiettivo** a sinistra.

   ![](assets/goal-page-unshimmed.png)

1. Fai clic sull&#39;icona **Modifica** ![](assets/edit-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **Modifica tutto** o **Panoramica**

   Oppure

   Inizia a digitare le informazioni in uno dei campi modificabili nella sezione Dettagli obiettivo. La sezione diventa modificabile.

   >[!IMPORTANT]
   >
   >Non tutti i campi visualizzati nella sezione Dettagli obiettivo possono essere modificati. In Workfront alcuni campi vengono calcolati e sono di sola lettura.

1. Aggiorna o controlla i campi seguenti:

   * **Descrizione**: aggiungi o aggiorna le informazioni sull&#39;obiettivo.
   * **Avanzamento**: indica la percentuale di completamento dell&#39;obiettivo. Non è possibile aggiornare manualmente l’avanzamento di un obiettivo. L&#39;obiettivo &quot;progresso&quot; è il calcolo di tutti gli indicatori di progresso.
   * **Condizione**: indica se l&#39;obiettivo è nuovo e non è stato ancora aggiornato, se è in arrivo per essere completato in tempo o in ritardo. Non è possibile aggiornare la condizione di un obiettivo. La condizione dell&#39;obiettivo viene calcolata automaticamente da Workfront.\
     Per ulteriori informazioni sulla condizione e sull’avanzamento dell’obiettivo, consulta
     [Panoramica dell&#39;avanzamento e della condizione dell&#39;obiettivo negli obiettivi di Adobe Workfront](../goal-management/calculate-goal-progress.md).
   * **Stato**: impossibile aggiornare manualmente lo stato di un obiettivo. Per ulteriori informazioni, consulta [Panoramica sullo stato degli obiettivi in Obiettivi di Adobe Workfront](../goal-management/goal-status-overview.md).
   * **Proprietario obiettivo**: fare clic per aggiornare il nome del proprietario dell&#39;obiettivo. Inizia a digitare il nome di un utente, team, gruppo o il nome dell’organizzazione, quindi selezionalo quando viene visualizzato nell’elenco. Puoi avere un solo proprietario per un obiettivo.
   * **Obiettivo principale**: inizia a digitare il nome di un obiettivo da impostare come principale dell&#39;obiettivo selezionato. L’avanzamento dell’obiettivo selezionato aggiornerà automaticamente l’avanzamento dell’obiettivo principale.

     >[!TIP]
     >
     >Non è possibile aggiornare le seguenti informazioni su un obiettivo principale:
     >    * Periodo obiettivo principale
     >    * Avanzamento obiettivo principale
     >    * Proprietario obiettivo principale.
     >      
     >È necessario aggiornare queste informazioni sull&#39;obiettivo principale stesso.

   * **Periodo**: fare clic per aggiornare il periodo di tempo per l&#39;obiettivo\
     Oppure\
     Seleziona **Abilita date personalizzate** per specificare le date di **Inizio** e **Fine** dell&#39;obiettivo.
   * **Note di chiusura**: questo campo è visibile solo per gli obiettivi con stato Chiuso. Non è possibile modificare gli obiettivi chiusi. La riapertura di un obiettivo chiuso elimina definitivamente le note di chiusura.


