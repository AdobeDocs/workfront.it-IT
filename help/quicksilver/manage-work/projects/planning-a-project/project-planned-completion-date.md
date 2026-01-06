---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Impostare la data di completamento pianificata del progetto
description: La Data di completamento pianificata di un progetto è la data entro la quale il progetto è impostato per essere completato.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 996398c5-de92-445e-8e86-36b2efdcf6b5
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 4%

---

# Impostare la data di completamento pianificata del progetto

<!-- Audited: 4/2025 -->

La Data di completamento pianificata di un progetto è la data in cui il progetto è impostato per il completamento.

L&#39;Inizio pianificato e le Date di completamento pianificate di un progetto si basano sulle date delle attività del progetto. Questo articolo descrive come impostare manualmente o automaticamente la Data di completamento pianificata di un progetto. Per ulteriori informazioni sulla data di completamento pianificata di un&#39;attività, vedere [Panoramica sulla data di completamento pianificata dell&#39;attività](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

La data di completamento pianificata di un progetto può essere impostata manualmente o automaticamente, a seconda che il progetto sia pianificato dall’inizio o dalla data di completamento.

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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
   <p>Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il progetto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>
   New: Standard

   Or

   Current: Plan </p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Impostare manualmente la data di completamento pianificata di un progetto

È necessario impostare manualmente la data di completamento pianificata di un progetto quando si pianifica il progetto dalla data di completamento.

>[!NOTE]
>
>Quando imposti manualmente la Data di completamento pianificata di un progetto, Workfront calcola automaticamente la Data di inizio pianificata del progetto in base alla Durata di tutte le attività.


Per programmare un progetto dalla data di completamento:

{{step1-to-projects}}

1. Fai clic su **Nuovo progetto**, quindi seleziona **Nuovo progetto** dal menu a discesa.

   Per ulteriori informazioni sulla creazione di progetti, vedere l&#39;articolo [Creare un progetto](../../../manage-work/projects/create-projects/create-project.md).

1. Seleziona **Dettagli progetto** nel pannello a sinistra.

1. Fai clic sull&#39;icona **Modifica progetto** ![Icona Modifica](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png) nell&#39;angolo superiore destro, quindi seleziona **Panoramica** nel menu a discesa visualizzato.

1. Nella sezione **Date progetto**, fai clic sul campo **Modalità pianificazione**, quindi seleziona **Data completamento**.

1. Specifica la **data di completamento pianificata** del progetto.
1. Fai clic su **Salva modifiche**.

   Quando si iniziano ad aggiungere attività al progetto, la **Data inizio pianificata** del progetto viene calcolata in base alla durata totale di tutte le attività.

## Impostare automaticamente la data di completamento pianificata di un progetto

La data di completamento pianificata di un progetto viene calcolata automaticamente da Workfront quando si pianifica il progetto a partire dalla data di inizio.

Per programmare un progetto dalla data di inizio:

{{step1-to-projects}}

1. Fai clic su **Nuovo progetto**, quindi seleziona **Nuovo progetto** dal menu a discesa visualizzato.

   Per ulteriori informazioni sulla creazione di progetti, vedere l&#39;articolo [Creare un progetto](../../../manage-work/projects/create-projects/create-project.md).

1. Seleziona **Dettagli progetto** nel pannello a sinistra.

1. Fai clic sull&#39;icona **Modifica progetto** ![Icona Modifica](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png) nell&#39;angolo superiore destro, quindi seleziona **Panoramica** nel menu a discesa visualizzato.

1. Nella sezione **Date progetto**, fai clic sul campo **Modalità pianificazione**, quindi seleziona **Data inizio**.

1. Specifica la **Data inizio pianificata** del progetto.
1. Fai clic su **Salva modifiche**.

   Quando inizi ad aggiungere attività al progetto, la **Data di completamento pianificata** del progetto viene calcolata in base alla durata totale di tutte le attività.

   Per ulteriori informazioni sulla durata dell&#39;attività, vedere l&#39;articolo [Panoramica sulla durata dell&#39;attività e sul tipo di durata](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   La data di completamento pianificata del progetto coincide, in questo caso, con la data di completamento pianificata dell&#39;ultima attività del progetto.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>The Planned Completion Date of a task</h2>
<p>(NOTE: drafted because I created a new article, here: /Content/Manage work/Tasks/Task information/task-planned-completion-date.htm)</p>
<p>You can either specify the Planned Completion Date of a task, or you can leave it up to Workfront to calculate it depending on certain criteria. </p>
<ul>
<li><a href="#manually-set-the-planned-completion-date-of-a-task" class="MCXref xref">Manually set the Planned Completion Date of a task</a> </li>
<li><a href="#how-the-planned-completion-date-is-calculated-for-a-task" class="MCXref xref">How the Planned Completion Date is calculated for a task</a> </li>
</ul>
<p><strong>Manually set the Planned Completion Date of a task</strong></p>
<p>Setting the Planned Completion Date of a task depends on the type of Task Constraint you assign to the task. </p>
<p>You can manually set the Planned Completion Date when creating a task, as described in the article <a href="../../../manage-work/tasks/create-tasks/create-tasks-in-project.md" class="MCXref xref">Create tasks in a project</a>.</p>
<p>You can manually specify the Planned Completion Date when you select any of the following Task Constraints: </p>
<table border="1" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th> <p><strong>Task Constraint Type</strong> </p> </th>
<th> <p><strong>Effect of Manually Changing the Planned Completion Date</strong> </p> </th>
</tr>
</thead>
<tbody>
<tr>
<td> <p>Must Finish On</p> <p>Finish No Later Than</p> <p>Finish No Earlier Than</p> </td>
<td> <p><span class="s1">The Planned Start Date is adjusted in order to keep the Duration the same.</span> </p> </td>
</tr>
<tr>
<td> <p>Fixed Dates</p> </td>
<td> <p>The Duration is adjusted in order to keep the Planned Start Date the same.</p> </td>
</tr>
</tbody>
</table>
<p><strong>How the Planned Completion Date is calculated for a task</strong></p>
<p>When it is calculated automatically by the system, the following can influence the Planned Completion Date of a Task:</p>
<ul>
<li> <p>Task Constraint</p> <p>For more information about Task Constraints, see the article <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </li>
<li> <p>Task predecessor relationship</p> <p>For more information about task predecessors, see the article <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p> </li>
<li>Project Completion Date, when the project is scheduled from Completion Date.</li>
<li> <p>The time off schedule of the Primary Assignee of the task. </p> <p>When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the <strong>Consider user time off in task durations</strong> setting is selected for the <strong>User Time Off</strong> field. New projects inherit this setting from the Project Preferences area, but you can edit the setting at the project level. </p> <p>For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 2 marked for Time-off, the task Planned Completion Date becomes June 4. </p> <p>For information about the <strong>User Time Off</strong> preference, see the articles <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a> or <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li>
</ul>
<p>When set automatically, the Planned Completion Date is determined based on the following calculation: </p>
<p><code>Planned Completion Date = Planned Start Date + Duration</code> </p>
<p>For example, if your task has a start date of September 16 and a duration of 10 days, the Planned Completion Date is September 26.</p> <note type="note">
 The Update Type for the project must also be set to Automatic and On Change or Automatically in order for the Planned Hours and Duration to be automatically adjusted.
<br>For more information about the Update Type, see the article
<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.
</note>
</div>
-->
