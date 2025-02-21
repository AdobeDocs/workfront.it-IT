---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Aggiornamento dell’avanzamento dell’obiettivo in Obiettivi di Adobe Workfront
description: Devi rivedere periodicamente i tuoi obiettivi e aggiornarne i progressi per assicurarti che non rimangano indietro o non vengano raggiunti.
author: Alina
feature: Workfront Goals
exl-id: 5092f508-e52c-4934-a8c1-d0be04ecce13
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 0%

---

# Aggiornamento dell’avanzamento dell’obiettivo in Obiettivi di Adobe Workfront

Devi rivedere periodicamente i tuoi obiettivi e aggiornarne i progressi per assicurarti che non rimangano indietro o non vengano raggiunti.

<!--And: take this last sentence ^^ out when you update this for goal redesign production.-->

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
<li>Un piano Workfront di Ultimate che include gli obiettivi di Workfront per impostazione predefinita. </li></ul>
 <p>Oppure</p>
 <p>Fabbisogno di prodotto corrente: un piano Workfront e una licenza aggiuntiva per gli obiettivi Adobe Workfront. </p> <p>Per informazioni, vedere <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisiti per l'utilizzo degli obiettivi di Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Livello di accesso</td>
 <td> <p>Modifica accesso agli obiettivi</p></td>
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

## Prerequisiti

Prima di iniziare, devi avere un obiettivo attivo.

Non è possibile aggiornare l&#39;avanzamento di obiettivi che sono bozze, inattivi o chiusi.

## Considerazioni per l’aggiornamento degli obiettivi

Quando aggiorni l’avanzamento degli obiettivi, tieni presente quanto segue:

* Workfront Goals calcola automaticamente l&#39;avanzamento di un obiettivo quando si aggiorna l&#39;avanzamento dei relativi indicatori di avanzamento.

  >[!TIP]
  >
  >Non puoi aggiornare l’avanzamento direttamente su un obiettivo. È necessario aggiornare l’avanzamento degli indicatori di avanzamento dell’obiettivo (attività, risultati, progetti connessi), che a sua volta aggiorna l’avanzamento dell’obiettivo. Per aggiornare l’avanzamento dei progetti, devi aggiornare le attività del progetto.

  Vedi anche i seguenti articoli:

   * Per informazioni sull&#39;aggiunta di attività agli obiettivi, vedere [Aggiungere attività agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md).
   * Per informazioni sull&#39;aggiunta di risultati agli obiettivi, vedere [Aggiungere risultati agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   * Per informazioni sul modo in cui Workfront Goals calcola l&#39;avanzamento di un obiettivo, vedere [Panoramica sull&#39;avanzamento e sulla condizione dell&#39;obiettivo in Adobe Workfront Goals](../../workfront-goals/goal-management/calculate-goal-progress.md).

* Devi creare gli obiettivi e attivarli prima di poter aggiornare il loro avanzamento.

  Vedi anche i seguenti articoli:

   * Per informazioni sulla creazione degli obiettivi, vedere [Creare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
   * Per informazioni sull&#39;attivazione degli obiettivi, vedere [Attivare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

  >[!IMPORTANT]
  >
  >Non è possibile aggiornare l’avanzamento degli obiettivi che sono bozza, chiusi o inattivi.

* La prima volta che aggiorni l’avanzamento di un risultato o di un’attività su un obiettivo, l’obiettivo cambia da Obiettivi nuovi e Workfront inizia a registrare l’avanzamento e gli aggiornamenti dello stato di avanzamento sull’obiettivo.

<!--

## Update goal progress by using Check-in in the Production environment

>[!IMPORTANT]
>
> <span class="preview"> The Check-in functionality has been removed from the Preview environment and will be removed from Workfront Goals with the 23.1 release. See the [Update goal progress in the Preview environment](#update-goal-progress-in-the-preview-environment) section in this article to update goal progress in Preview. </span>


You can check in on goals at the individual goal level, or you can check in on multiple goals from the Check-in section of Workfront Goals.

* [Update individual goals](#update-individual-goals) 
* [Update goals in the Check-in section](#update-goals-in-the-check-in-section)

### Update individual goals {#update-individual-goals}

When you check in on a goal at the goal level, you can update the progress of the results and activities that are assigned to you or other users.

For information about how to update additional information about results and activities, see [Edit results and activities in Adobe Workfront Goals](../../workfront-goals/results-and-activities/edit-results-and-activities.md).

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area.

   All goals display by default. 

1. (Optional) Click any of the following sections in the left panel to access a list of goals:

   * Goal Alignment 
   * Pulse 
   * Check-in

   Or

   From the Goal List, click the name of a goal to open the **Goal Details** panel on the right.

   >[!TIP]
   >
   >You must have Edit access to Goals in your Access Level to view the Check-in section or the Check in button.

1. Click **Check in**.

   ![Check in link](assets/check-in-link-inside-goal-details-highlighted-350x156.png)

   The progress of results and activities becomes editable.

1. Update the current progress on each of the results. Depending on what type of result you selected, you can do one of the following:

   * Update the quantity 
   * Update the currency amount
   * Update the percent complete

1. Update the percent complete on the Manual progress bar activity.

   >[!TIP]
   >
   >When you add projects as activities to your goals, you cannot manually update projects at the goal level. Workfront automatically updates project progress based on the project of their tasks. When the project percent complete updates in Workfront, the goal progress associated with the project also updates automatically.

1. Click **Back to Summary** to return to the Goal Details panel.

   Your goal progress updates as you update the results and activities of your goal. 

1. Click the **X icon** in the upper-right corner of the Goal Details panel to close it.

### Update goals in the Check-in section {#update-goals-in-the-check-in-section}

You can use the Check-in section to check in on goals when you want to quickly provide updates for several goals at the same time.

>[!TIP]
>
>You can access the Check-in section from any of the following sections:
>
>* Goal List 
>* Goal Alignment 
>* Pulse 
>

When you check in on a goal in the Check-in section, you can update the progress of the results and activities that are assigned only to you. You cannot update the progress of results and activities that are assigned to other users in this section.

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List section displays by default. 

1. Click Check-in in the left panel.

   Or

   (Conditional) If you are in the Goal List, Goal Alignment, or Pulse sections, click the **Check in** button in the upper-right of the screen. This opens the Check-in section.

   ![Check in button](assets/check-in-button-highlighted-350x102.png)

   Goals display in a list and results and activities are listed under each goal.

   ![Check in page](assets/check-in-page-with-show-all-aligned-goals-link-350x178.png)

1. (Optional) Click **Show all results**, **Show all activities**, or **Show all aligned goals** to the far right of the goal name to display all results, activities, and aligned goals of a goal whose progress you want to update.

   >[!CAUTION]
   >
   >You cannot directly update aligned goals, but you can update their results and activities.

1. Update the current progress on each of the results assigned to you. Depending on what type of result you selected, you can do one of the following:

   * Update the quantity 
   * Update the currency amount
   * Update the percent complete

   The result and the goal progress updated automatically and you receive a confirmation of your changes.

1. Update the percent complete on your Manual progress bar activity.

   >[!TIP]
   >
   >When you add projects as activities to your goals, you cannot manually update projects at the goal level. Workfront automatically updates project progress based on the project of their tasks. When the project percent complete updates in Workfront, the goal progress associated with the project also updates automatically.

   The activity and the goal progress updated automatically and you receive a confirmation of your changes.

1. (Optional) Add a comment for your goal, then click **Post** to save your comment.

-->

Per aggiornare lo stato di avanzamento degli obiettivi:

1. Fai clic sull&#39;icona **Menu principale** ![Icona Menu principale](assets/main-menu-icon.png) > **Obiettivi** nell&#39;angolo superiore destro.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Verrà aperto l&#39;elenco degli obiettivi. Per impostazione predefinita, vengono visualizzati tutti gli obiettivi a cui hai accesso.

   In alternativa, potete fare clic su Allineamento obiettivo (Goal Alignment) nel pannello sinistro.

1. Nell&#39;elenco Obiettivo fare clic sul nome di un obiettivo per aprire la pagina obiettivo.
1. Fai clic su **Indicatori di avanzamento** nel pannello a sinistra.

   Nell&#39;elenco Indicatori di avanzamento vengono visualizzati tutti gli indicatori di avanzamento per l&#39;obiettivo selezionato.

   >[!NOTE]
   >
   >  * Puoi aggiornare solo risultati e attività.
   >  * È necessario aggiornare gli indicatori di progresso degli obiettivi per bambini per mostrare il progresso sugli obiettivi per bambini.
   >  * È necessario aggiornare le attività sui progetti collegati per mostrare lo stato di avanzamento dei progetti.
   >   
   >    A sua volta, i progressi degli obiettivi secondari e dei progetti guidano l&#39;avanzamento dell&#39;obiettivo selezionato.


1. Per aggiornare l&#39;avanzamento di un risultato o di un&#39;attività, fare clic sul valore nella colonna **Avanzamento effettivo** del risultato o dell&#39;attività e digitare un numero per aggiornarne il valore, quindi premere Invio.

   ![Stato effettivo](assets/actual-progress-result-updating-highlighted-unshimmed.png)

   La barra di avanzamento per l’indicatore di avanzamento nella colonna Avanzamento e l’avanzamento dell’obiettivo nell’intestazione dell’obiettivo vengono aggiornati immediatamente.

