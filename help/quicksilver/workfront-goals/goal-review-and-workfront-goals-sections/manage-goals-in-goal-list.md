---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Gestione degli obiettivi nell’elenco Obiettivi di Adobe Workfront
description: Dopo che tu o altri utenti avete creato gli obiettivi, puoi esaminarne l’avanzamento e le informazioni nell’Elenco obiettivi. Per informazioni sulla creazione degli obiettivi, consulta Creare gli obiettivi in Obiettivi di Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 2%

---

# Gestione degli obiettivi nell’elenco Obiettivi di Adobe Workfront

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

Dopo che tu o altri utenti avete creato gli obiettivi, puoi esaminarne l’avanzamento e le informazioni nell’Elenco obiettivi. Per informazioni sulla creazione degli obiettivi, vedere [Creare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

## Requisiti di accesso

Per eseguire le azioni descritte in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
 <td> <p>Modifica accesso agli obiettivi</p>  </td>
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

## Gestione degli obiettivi nell’elenco Obiettivi

Puoi visualizzare e gestire gli obiettivi nelle seguenti sezioni di Obiettivi di Workfront:

* Elenco obiettivi
* Allineamento obiettivi

Ogni sezione mostra gli obiettivi in formati leggermente diversi. La sezione utilizzata dipende dallo scopo che si desidera raggiungere mentre si lavora con gli obiettivi.

Per ulteriori informazioni, consulta [Panoramica delle sezioni sugli obiettivi di Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

Questo articolo descrive come rivedere gli obiettivi nell’elenco Obiettivo.

Quando rivedi l’elenco degli obiettivi, considera quanto segue:

* Puoi visualizzare gli obiettivi che tu o chiunque altro nella tua organizzazione hai creato nell’Elenco obiettivi. Per poter modificare gli obiettivi, è necessario disporre delle autorizzazioni di gestione.

<!--

### Manage the Goal List in the Production environment

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List section displays by default. You can view goals regardless of their status, period, or owner, by default.

   The list of goals contains the following columns with information about each goal, result, or activity: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> 
       <div> 
        <p role="rowheader">Name </p> 
       </div> </td> 
      <td>The name of the goal, result, or activity.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Owner</td> 
      <td>The name of the goal, result, or activity owner. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Period</td> 
      <td>The time period for which the goal is scheduled.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progress </td> 
      <td> <p>The progress indicator for the goal includes the following:</p> 
       <ul> 
      <li> <p>The progress label. </p> <p>For information, see <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Overview of goal progress and condition in Adobe Workfront Goals</a>. </p> </li> 
      <li> <p>The percent complete of the goal, activity, or result. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Status (includes alignment icon)</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
      <td> <p>The status of the goal which can be one of the following:</p> 
       <ul> 
        <li>Active</li> 
        <li>Draft</li> 
        <li>Inactive</li> 
        <li>Closed</li> 
       </ul> <p>For information about goal status, see <a href="../../workfront-goals/goal-management/goal-status-overview.md" class="MCXref xref">Goal status overview in Adobe Workfront Goals</a>. </p> <p>The alignment icon appears on goals that are aligned to other goals. For information about aligning goals, see <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">Align goals by connecting them in Adobe Workfront Goals</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Use the filters in the upper-right corner of the goal list to select only goals that are important to you. For information about using filters in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md)
1. Click any of the fields in the column headers to sort it by that field.

   An arrow displays to the right of the field by which the list is sorted.

   ![Goal list with goal expanded](assets/goal-list-with-goal-expanded-+-result-+-activity-350x117.png)

1. (Optional) Click the field in the column again to sort the same column in a descending order. 
1. Click the right-pointing arrow to the left of the goal name to expand a goal

   Or

   Click the right-pointing arrow ![Right-pointing arrow](assets/right-pointing-arrow.png) in the header of the list to expand all the goals in the list and view additional information about each goal, including any of the following:

   * Results names, owners, and progress

     For information about results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   
   * Activity names, owners, and progress

     For information about activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

1. Click the name of a goal to open the **Goal Details** panel on the right and review more information about the goal as well as manage it. For information about reviewing individual goals, see [Update goals in the Goal details section in Adobe Workfront Goals](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. (Optional) Expand the **Goals per page** drop-down menu and select from the following options to display additional goals:

   * 20  
      
      This is the default selection. 
   * 50
   * 100

1. Click **Print** to export a list of goals, results, and activities to a .pdf file.

   >[!TIP]
   >
   >* When printing a list of goals, the file produced contains only the information displayed on the screen. Items eliminated by filtering a list of goals do not display in the .pdf file.
   >* When you do not expand the goals in the list before printing the list, the .pdf file displays only goals without their results and activities.

   For more information, see [Print the Goal List in Adobe Workfront Goals](../../workfront-goals/goal-management/print-the-goal-list.md). 

1. Click the **Alignment icon** ![Alignment icon](assets/align-icon.png) next to an aligned to open the goal's card in the Goal Alignment section. For more information, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).
-->

Per gestire gli obiettivi nell&#39;elenco Obiettivi:

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **Goals**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   La sezione Elenco obiettivi viene visualizzata per impostazione predefinita. Per impostazione predefinita, è possibile visualizzare gli obiettivi indipendentemente dal loro stato, periodo o proprietario.

   L’elenco degli obiettivi contiene i seguenti campi con informazioni su ciascun obiettivo:

   * **Nome**: nome dell&#39;obiettivo.
   * **Proprietario**: nome del proprietario dell&#39;obiettivo.
   * **Periodo**: il periodo di tempo per il quale è pianificato l&#39;obiettivo.
   * **Stato**: lo stato dell&#39;obiettivo può essere uno dei seguenti:
      * Attiva
      * Bozza
      * Inattiva
      * Chiuso

     Per informazioni sullo stato dell&#39;obiettivo, vedere [Panoramica sullo stato dell&#39;obiettivo in Obiettivi di Adobe Workfront](../goal-management/goal-status-overview.md).

     L&#39;icona di allineamento viene visualizzata sugli obiettivi allineati ad altri obiettivi. Per informazioni sull&#39;allineamento degli obiettivi, vedere [Allineare gli obiettivi collegandoli in Obiettivi di Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md).

   * **Condizione**: rappresentazione visiva dell&#39;avanzamento dell&#39;obiettivo nel periodo di tempo assegnato per il completamento.

     La condizione di un obiettivo può essere una delle seguenti:

      * Nuovo
      * Puntuale
      * A Rischio
      * In difficoltà

     Per informazioni sulle condizioni dell&#39;obiettivo, vedere [Panoramica sull&#39;avanzamento e sulla condizione dell&#39;obiettivo in Obiettivi di Adobe Workfront](../goal-management/calculate-goal-progress.md).

   * **Avanzamento**: indicatore di avanzamento per l&#39;obiettivo espresso come valore percentuale. Il colore dell’indicatore di avanzamento corrisponde al colore della condizione dell’obiettivo.

     Per informazioni, consulta [Calcolare l&#39;avanzamento dell&#39;obiettivo in Obiettivi di Adobe Workfront](../goal-management/calculate-goal-progress.md).

1. Fai clic sull&#39;icona del filtro ![icona Filtro](assets/filter-icon.png) nell&#39;angolo superiore destro dell&#39;elenco di obiettivi e applica i filtri per visualizzare solo gli obiettivi che ti interessano.

   Per informazioni sull&#39;utilizzo dei filtri negli obiettivi di Workfront, vedere [Informazioni sui filtri negli obiettivi di Adobe Workfront](../goal-management/filter-information-wf-goals.md).

1. Fare clic su uno dei campi nelle intestazioni di colonna per ordinare l&#39;elenco in base a tale campo.
A destra del campo in base al quale viene ordinato l&#39;elenco viene visualizzata una freccia.

1. (Facoltativo) Fai di nuovo clic sul campo nella colonna per ordinare la stessa colonna in ordine decrescente.
1. Fai clic sul nome di un obiettivo per aprirne la pagina.
1. Seleziona un obiettivo nell’elenco, quindi fai clic su una delle seguenti opzioni nella parte superiore dell’elenco:
   * Icona **Modifica** ![Icona Modifica](assets/edit-icon.png) per modificare le informazioni sull&#39;obiettivo. Per informazioni, consulta [Modificare gli obiettivi in Obiettivi di Adobe Workfront](../goal-management/edit-goals.md).
   * Icona **Condividi** ![Icona Condividi](assets/share-icon.png) per condividere l&#39;obiettivo con altri utenti. Per informazioni, consulta [Condividere un obiettivo negli Obiettivi di Adobe Workfront](../workfront-goals-settings/share-a-goal.md).
   * **Apri allineamento** icona ![Apri icona allineamento](assets/align-icon-unshimmed.png) per aprire l&#39;area Allineamento obiettivo. Questa opzione viene visualizzata solo quando l&#39;obiettivo selezionato è allineato a un altro obiettivo.
   * **Elimina** icona ![Elimina icona](assets/delete-icon.png) per eliminare l&#39;obiettivo, quindi fai clic su **Elimina** per confermare.  Per informazioni, consulta [Eliminare e disattivare gli obiettivi in Obiettivi di Adobe Workfront](../goal-management/delete-and-deactivate-goals.md).





