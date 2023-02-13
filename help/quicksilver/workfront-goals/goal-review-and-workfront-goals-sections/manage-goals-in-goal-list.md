---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Gestire gli obiettivi nell’elenco degli obiettivi di Adobe Workfront
description: Dopo aver creato gli obiettivi, puoi esaminarne lo stato di avanzamento e le informazioni nell’Elenco obiettivi. Per informazioni sulla creazione degli obiettivi, consulta Creare obiettivi in Obiettivi di Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 2%

---

# Gestire gli obiettivi nell’elenco degli obiettivi di Adobe Workfront

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

Dopo aver creato gli obiettivi, puoi esaminarne lo stato di avanzamento e le informazioni nell’Elenco obiettivi. Per informazioni sulla creazione degli obiettivi, vedi [Creare obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

## Requisiti di accesso

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>
-->

Per eseguire le azioni descritte in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica sulle licenze di Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td> <p>Devi acquistare una licenza aggiuntiva per la funzionalità Obiettivi di Adobe Workfront per accedere alla descritta in questo articolo. </p> <p>Per informazioni, consulta <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisiti per l'utilizzo degli obiettivi di Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Visualizzare o accedere in modo più rapido agli obiettivi</p> <p><b>NOTA</b><p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Concedere l’accesso agli obiettivi di Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> 
    <div> 
     <p>Visualizza o autorizzazioni superiori per gli obiettivi</p> 
     <p>Per informazioni sulla condivisione degli obiettivi, vedi <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Condividere un obiettivo in Obiettivi di Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario disporre dei seguenti elementi prima di poter iniziare:

* Modello di layout che include l’area Obiettivi del menu principale.

## Gestire gli obiettivi nell’elenco obiettivi

Puoi visualizzare e gestire gli obiettivi nelle seguenti sezioni degli obiettivi di Workfront:

* Elenco obiettivi
* Allineamento obiettivo

Ogni sezione visualizza gli obiettivi in formati leggermente diversi. La sezione che utilizzi dipende dallo scopo che desideri raggiungere mentre lavori con gli obiettivi.

Per ulteriori informazioni, consulta [Panoramica delle sezioni Obiettivi di Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

Questo articolo descrive come rivedere gli obiettivi nell&#39;Elenco obiettivi.

Quando rivedi l’Elenco obiettivi, considera quanto segue:

* Puoi visualizzare gli obiettivi che tu o chiunque altro nella tua organizzazione hai creato nell’Elenco obiettivi. Per poter modificare gli obiettivi, devi disporre delle autorizzazioni di gestione .

<!--

### Manage the Goal List in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner, then click **Goals**.

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

   ![](assets/goal-list-with-goal-expanded-+-result-+-activity-350x117.png)

1. (Optional) Click the field in the column again to sort the same column in a descending order. 
1. Click the right-pointing arrow to the left of the goal name to expand a goal

   Or

   Click the right-pointing arrow ![](assets/right-pointing-arrow.png) in the header of the list to expand all the goals in the list and view additional information about each goal, including any of the following:

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

1. Click the **Alignment icon** ![](assets/align-icon.png) next to an aligned to open the goal's card in the Goal Alignment section. For more information, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).
-->

Per gestire gli obiettivi nell’Elenco obiettivi:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png)  nell&#39;angolo in alto a destra, quindi fai clic su **Obiettivi**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   La sezione Elenco obiettivi viene visualizzata per impostazione predefinita. Per impostazione predefinita, puoi visualizzare gli obiettivi indipendentemente dal loro stato, periodo o proprietario.

   L’elenco degli obiettivi contiene i campi seguenti con informazioni su ciascun obiettivo:

   * **Nome**: Nome dell&#39;obiettivo.
   * **Proprietario**: Nome del proprietario dell&#39;obiettivo.
   * **Punto**: Periodo di tempo per il quale l&#39;obiettivo è pianificato.
   * **Stato**: Lo stato dell’obiettivo può essere uno dei seguenti:
      * Attivi
      * Bozza
      * Inattiva
      * Chiuso

      Per informazioni sullo stato dell&#39;obiettivo, consulta [Panoramica sullo stato dell&#39;obiettivo negli obiettivi di Adobe Workfront](../goal-management/goal-status-overview.md).

      L’icona di allineamento viene visualizzata sugli obiettivi allineati ad altri obiettivi. Per informazioni sull&#39;allineamento degli obiettivi, vedi [Allineare gli obiettivi collegandoli negli obiettivi di Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md).

   * **Condizione**: Una rappresentazione visiva del progresso dell’obiettivo entro il periodo di tempo allocato per il completamento dell’obiettivo.

      La condizione di un obiettivo può essere una delle seguenti:

      * Nuovo
      * Puntuale
      * A Rischio
      * In difficoltà

      Per informazioni sulle condizioni dell&#39;obiettivo, vedi [Panoramica dell’avanzamento e della condizione dell’obiettivo in Obiettivi di Adobe Workfront](../goal-management/calculate-goal-progress.md).

   * **Avanzamento**: Indicatore di avanzamento per l&#39;obiettivo come valore percentuale. Il colore dell’indicatore di avanzamento corrisponde al colore della condizione dell’obiettivo.

      Per informazioni, consulta [Calcolo dell’avanzamento dell’obiettivo negli obiettivi di Adobe Workfront](../goal-management/calculate-goal-progress.md).



1. Fai clic sull’icona del filtro ![](assets/filter-icon.png) nell’angolo in alto a destra dell’elenco degli obiettivi e applica i filtri per visualizzare solo gli obiettivi che sono importanti per te.

   Per informazioni sull&#39;utilizzo dei filtri negli obiettivi di Workfront, vedi [Filtrare le informazioni negli obiettivi di Adobe Workfront](../goal-management/filter-information-wf-goals.md).

1. Fai clic su uno dei campi nelle intestazioni di colonna per ordinare l’elenco in base a tale campo.
Viene visualizzata una freccia a destra del campo in base al quale viene ordinato l’elenco.

1. (Facoltativo) Fai nuovamente clic sul campo nella colonna per ordinare la stessa colonna in ordine decrescente.
1. Fai clic sul nome di un obiettivo per aprire la pagina dell’obiettivo.
1. Seleziona un obiettivo nell’elenco, quindi fai clic su una delle seguenti opzioni nella parte superiore dell’elenco:
   * **Modifica** icona ![](assets/edit-icon.png) per modificare le informazioni sull’obiettivo. Per informazioni, consulta [Modificare gli obiettivi in Obiettivi di Adobe Workfront](../goal-management/edit-goals.md).
   * **Condividi** icona ![](assets/share-icon.png) condividere l&#39;obiettivo con altre persone. Per informazioni, consulta [Condividere un obiettivo in Obiettivi di Adobe Workfront](../workfront-goals-settings/share-a-goal.md).
   * **Allineamento aperto** icona ![](assets/align-icon-unshimmed.png) per aprire l&#39;area di allineamento obiettivo. Questa opzione viene visualizzata solo quando l’obiettivo selezionato è allineato a un altro obiettivo.
   * **Elimina** icona ![](assets/delete-icon.png) per eliminare l&#39;obiettivo, quindi fai clic su **Elimina** per confermare.  Per informazioni, consulta [Eliminare e disattivare gli obiettivi in Obiettivi di Adobe Workfront](../goal-management/delete-and-deactivate-goals.md).





