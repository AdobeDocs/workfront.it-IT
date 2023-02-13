---
product-area: templates
navigation-topic: templates-navigation-topic
title: Modificare i modelli di progetto
description: È possibile modificare i modelli di progetto per riflettere le modifiche apportate ai processi e alle impostazioni del progetto.
author: Alina
feature: Work Management
exl-id: da0fca31-6a50-4862-ad9a-a453ef968773
source-git-commit: dcdcf21903d0fceb3c05039689bb87ae4c834d07
workflow-type: tm+mt
source-wordcount: '4704'
ht-degree: 3%

---

# Modificare i modelli di progetto

<!--drafted
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 
-->

<!--
<The Resource Pools part also duplicates in the "Working with Resource Pools" article</p>
-->

È possibile modificare i modelli di progetto per riflettere le modifiche apportate ai processi e alle impostazioni del progetto. Dopo aver aggiornato e salvato le modifiche in un modello, le nuove modifiche saranno visibili nei nuovi progetti quando i progetti vengono creati utilizzando il modello. Le modifiche apportate al modello non si riflettono sul progetto che utilizza attualmente quel modello.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modificare l’accesso ai modelli</p> <p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni sull’accesso ai modelli, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Concedere l’accesso ai modelli</a>. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> 
    <ul> 
     <li> <p>Autorizzazioni di Contribute a un modello per modificarlo nella scheda Dettagli modello</p> </li> 
     <li> <p>Gestire le autorizzazioni per un modello per modificarlo nella casella Modifica modello</p> </li> 
    </ul> <p> Per informazioni sulle autorizzazioni del modello, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Condividere un modello</a>. </p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Modificare un modello {#edit-a-template}

<!--
Editing a template differs depending on what environment you choose. 

### Edit a template in the Production environment {#edit-a-template-in-the-production-environment} 

1. Go to the template you want to edit.
1. (Conditional) To edit limited information about the template,  click **Template Details** in the left panel, then go to the areas listed in the left panel to edit information for each area. 
1. To edit information in the Details section, click the **Edit** icon ![](assets/edit-icon.png), then select from any of the areas below, or click **Edit all** to edit information in all areas:

   * Overview
   * Custom Forms

     Names of customs forms display only if there are custom forms attached to the object.
   
   * Finance

   >[!TIP]
   >
   >For information about all fields that display in the Details area, continue with editing all fields using the Edit Template box below.

1. (Conditional) To edit all information about the template, click the **More** menu ![](assets/qs-more-icon-on-an-object.png) next to the name of the template, then click **Edit**.

   The **Edit Template** box opens. The sections in this box contain the same fields available in  the Template Details section .

1. Consider editing information in any of the following sections:

   * [Overview](#overview) 
   * [Finance](#finance) 
   * [Portfolio](#portfolio) 
   * [Settings](#settings) 
   * [Access](#access) 
   * [Custom Forms](#custom-forms) 
   * [Tasks](#tasks) 
   * [Issues](#issues) 
   * [Comment](#comment)

### Overview {#overview}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Overview**.

   ![](assets/edit-template-overview-with-tasks-and-issues-350x210.png)

1. Update the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong></td> 
      <td>Specify a name for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong></td> 
      <td>Add additional information about the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Active</strong></td> 
      <td><p>Select this checkbox if you want the template to be active. Other users can find this template and attach it to projects when creating projects. Deselect this checkbox if you want to deactivate templates that are no longer used. Deactivated templates cannot be attached to projects. This is enabled by default. </p><p><b>TIP</b>
      
      You can deactivate a template from the template header as described in the [Activate or deactivate a template](#activate-or-deactivate-a-template) section in this article.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong></td> 
      <td>Specify a web link that relates to information about this template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schedule From</strong></td> 
      <td><p>Specify whether the project using this template is scheduled from the <strong>Start Date</strong>, or from the <strong>Completion Date</strong>. This selection determines the planned dates of the future tasks on the project using this template. </p><p>Select from the following: </p> 
       <ul> 
        <li><p><strong>Schedule From Start Date</strong>: The Start Date of the template is actually the Start Day. When you schedule a template from Start Date, Adobe Workfront calculates the Completion Day of the template based on the Duration of all the template tasks. The Start Day of the template becomes the Planned Start Date of the future project.</p></li> 
        <li><p><strong>Schedule from Completion Date</strong>: The Completion Date of the template is actually the Completion Day. When you schedule a template from Completion Date, Workfront calculates the Start Day of the template based on the Duration of all the template tasks. The Completion Day of the template becomes the Planned Completion Date of the future project. </p></li> 
       </ul><p>For more information about the Start and Completion Days of template tasks, see <a href="../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md" class="MCXref xref">Overview of Start and Completion Days in a template</a>. </p><p>The Schedule From setting for templates is similar to that of projects. Your Workfront administrator selects the default Schedule From setting for the projects in your system. For information about setting project defaults, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condition Type</strong></td> 
      <td><p>Select between the following Condition Types:</p> 
       <ul> 
        <li><strong>Manual:</strong> The project owner sets the Condition of the project on the project manually. <strong></strong></li> 
        <li><strong>Progress Status:</strong> Workfront automatically sets the Condition of the future project based on the Progress Status of tasks on the Critical Path. For more information about understanding Progress Status, see <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Task Progress Status overview</a>.</li> 
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority</strong></td> 
      <td><p>This is just a visual flag for you which allows you to prioritize your future projects. Select from the following options:</p> 
       <ul> 
        <li><p><strong>None</strong></p></li> 
        <li><p><strong>Low</strong></p></li> 
        <li><p><strong>Normal</strong></p></li> 
        <li><p><strong>High</strong></p></li> 
        <li><p><strong>Urgent</strong></p></li> 
       </ul><p><p>Depending on the Project Preferences selected by your Workfront administrator, the names of priorities might be different for you. For more information about editing priorities, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Create and customize priorities</a>.</p></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Owner</strong></td> 
      <td><p>The user who is designated as the Template Owner must be a Workfront active user. </p><p>Consider the following about the user designated as the Template Owner: </p> 
       <ul> 
        <li>They are automatically given Manage permissions to the template. </li> 
        <li>They are added to the project team and are automatically given Manage permissions to the project created from the template. </li> 
        <li>They become the Project Owner, when the project is created from this template. </li> 
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Sponsor</strong></td> 
      <td><p>The user specified in this field becomes the Project Sponsor, when the template is added to the project. This user is added to the project team and is automatically given view permissions to the project. The user who is designated as the Template Sponsor must be a Workfront active user. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Manager</strong></td> 
      <td><p>The specified users are automatically given manage permissions to the future projects and can assign resources to the tasks and issues of the projects. You can specify more than one Resource Manager. </p></td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>Group</strong></td> 
      <td><p>In the drop-down list, select the group that you want to be associated with projects created from the template. It can be a group of any level. </p><p>You can make sure you are selecting the right group by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.</p> <p><b>NOTES</b>
      
    <ul> 
    <li><p>In the Projects area on a group's page, when someone creates a project using a template that doesn't have a group selected, the system associates the currently open group with the project.</p><p>This is different from other areas where the system associates a user's Home Group with the project when the user creates the project using a template that doesn't have a group selected.</p>
    </li> 
      <li><p>If a user selects a template that has a group selected while creating a project—or while converting a task or issue to a project—the user can choose a different group for the project.</p></li> 
      <li>Though this field is available in templates only in the new Adobe Workfront experience, you can see it in lists and reports both there and in Adobe Workfront Classic. </li> 
      </ul> </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Company</strong></td> 
      <td><p>Specify the Company that you want to associate with the template. Only active companies display in the list.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Finance {#finance}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Finance**.

   ![](assets/edit-template-finance-with-tasks-and-issues-350x259.png)

1. Update the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Performance Index Method</strong></td> 
      <td><p>Specify whether the Earned Value metrics of the future project are calculated using hours or costs. For more information about the Performance Index Method, see <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Set the Performance Index Method (PIM)</a>. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Budget</strong></td> 
      <td><p>Specify a Budget for the projects that are created from this template.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fixed Cost</strong></td> 
      <td><p>Specify the Fixed Cost for the projects that are created from this template. This is different than the Labor Cost which comes from the hours on the project and the Expense Cost which comes from the amount of expenses on the project. The Fixed Cost of a project is taken into account when calculating the Net Value of a project and it is part of the Budgeted Cost.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fixed Revenue</strong></td> 
      <td><p>Specify the Fixed Revenue for the projects that are created from this template.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Currency</strong></td> 
      <td><p>Specify the currency for the future project, if it is different than the default currency of your system. This field is not visible if you have only the default currency in the system.<br>For more information about currency, see <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Require time to be approved for this project</strong></td> 
      <td><p>Select this option to require the Project Owner of the future project created from this template to approve time logged on the project. If you are using Billing Records and you select this option, only the approved hours on the project appear as available billable hours for the Billing Records. Approving time on the project is independent of approving timesheets. For more information about requiring time to be approved on a project, see <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">Require time to be approved for a project</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Portfolio {#portfolio}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Portfolio**.

   ![](assets/edit-template-portfolio-with-tasks-and-issues-350x228.png)

1. Update the following fields:

   <table style="table-layout:auto">
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Portfolio</strong></td> 
      <td><p>Specify a Portfolio for the projects that are created from this template. You must create a Portfolio first, before it appears in the drop-down list. </p><p>Only active portfolios display in the list. For more information about creating portfolios, see <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Create a portfolio </a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Program</strong></td> 
      <td><p>If you selected a Portfolio for the template, specify a <strong>Program</strong> for the future project. Some Portfolios might not have Programs. You must create a Program first, before it appears in this drop-down list. Only active programs display in the list.</p><p>For more information about creating programs, see <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">Create a program</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planned Benefit</strong></td> 
      <td><p>Specify the Planned Benefit of the projects that are created from this template. The Planned Benefit is used in the Business Case of the project and the Portfolio Optimizer. </p><p>For more information about the Planned Benefit of a project, see <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Overview of project Planned Benefit</a>. The Planned Benefit of a project is taken into account when the Net Value of a project is calculated. </p><p>For more information about using the Portfolio Optimizer, see <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">Manage projects in the Portfolio Optimizer</a> </p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Settings {#settings}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Settings**.

   ![](assets/edit-template-settings-with-tasks-and-issues-350x336.png)

1. Update the following fields: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Milestone Path</strong> </td> 
      <td> <p>Select a Milestone Path for the template. Only active milestone paths display in the list.<br>For more information about Milestone Paths, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Create a milestone path</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Mode</strong> </td> 
      <td> <p>Controls how the future project will be marked as Complete. <br>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Automatic</strong>: The project is marked Complete when all the tasks and issues are completed.</p> </li> 
        <li> <p><strong>Manual</strong>: You have to manually select the Complete status for the project, when all the tasks and issues are completed. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Summary Completion Mode</strong> </td> 
      <td> <p>Controls how the parent tasks on the future project are marked as Complete. <br>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Automatic</strong>: The parent tasks are marked Complete and they update their percent complete automatically, as the children tasks are completed and the percent complete of the children is updated. </p> </li> 
        <li> <p><strong>Manual</strong>: You have to manually update the percent complete and the status of the parent tasks, independently of what changes are made to the children tasks. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Update Type</strong> </td> 
      <td> <p>Controls when the changes you make to the timeline of the future project are saved on the project. </p> 
       <b>EXAMPLE </b> 
        <p>The following changes to the project trigger an update to the timeline of the project:</p> 
        <ul> 
         <li> <p>update the dates of tasks</p> </li> 
         <li> <p>change predecessor relationships<br></p> </li> 
         <li> <p>change parent-child relationships</p> </li> 
         <li> <p>add or remove assignments in addition to changing the task constraint or duration type.</p> </li> 
        </ul> 
       </div> <p>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Automatic and On Change</strong> (Default setting): The future project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on (On Change). The project timeline is also updated each night (Automatic).<br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you perform an action on a task or project that triggers a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer recalculations display briefly as a question mark (between 1 and 5 seconds, or up to a minute for large projects). This indicates that the recalculation is not yet finished, and the dates are subject to change.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Change Only</strong>: The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Automatic Only</strong>: The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on. However, be aware that you chose this setting, as the project will not update at the same time that the changes are made.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Manual Only</strong>: The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculate project timelines</a>.<br></p> </li> 
       </ul> <p>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schedule</strong> </td> 
      <td> <p>Select a schedule for your template. This will become the schedule of the project that is created from this template. This should be the same schedule assigned to most people that are working on the project. You must create a schedule before you can assign it to a template.<br>For more information about creating schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>. <br>If you have not created custom schedules in your system, the Default Schedule is selected. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>User Time Off</strong> </td> 
      <td> <p>Determines whether the time off of the Primary Assignee of a task adjusts the task planned dates. When you attach the template to an existing project, and the template has a different setting for this field than the project, the setting on the project remains unchanged. The default option for this setting for a new template is the same as the system-level project preference. </p> <p>For information about the project preferences at the System level, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> <p>For information about how this setting affects the task dates on a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.<br>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Consider user time off in task durations</strong>: When selecting this option, the planned dates of the tasks on the project created from this template adjust according to the time off of the Primary Assignee of the task, if the time off occurs during the duration of the task. </p> </li> 
        <li> <p><strong>Ignore user time off in task durations</strong>: When selecting this option, the planned dates of the tasks on the project created from this template remain as originally planned, even if the Primary Assignee of the task has time off during the duration of the task. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Leveling Mode</strong> </td> 
      <td> <p>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Manual</strong>: you must manually level your resources on the project created from this template (this is the default setting)</p> </li> 
        <li> <p><strong>Automatic:</strong> Workfront levels the resources on the future project. <br>For more information about Resource Leveling, see <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">Level Resources in the Gantt Chart </a>. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Risk</strong> </td> 
      <td> <p>Define the level of risk of the projects created from this template. The risk is just an indicator of how risky a project can be. You can prioritize the execution of your projects based on the level of risk.<br>Consider selecting from the following levels of risk:<br></p> 
       <ul> 
        <li> <p><strong>Very Low</strong> </p> </li> 
        <li> <p><strong>Low</strong> </p> </li> 
        <li> <p><strong>Medium</strong> </p> </li> 
        <li> <p><strong>High</strong> </p> </li> 
        <li> <p><strong>Very High</strong> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Pools</strong> </td> 
      <td> <p>Specify the resource pools associated with the template. Resource pools are collections of users that are needed at the same time for the completion of a project. For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> <p> <p><b>NOTE</b> 
      
      When you edit templates in bulk, only the resource pools that are common to all the templates selected appear in this field. If the templates selected have no shared resource pools, this field will be empty. The resource pools you specify here will overwrite the templates' individual resource pools.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approval Process</strong> </td> 
      <td> <p>Select the approval process you want to associate with the template. Your Workfront administrator or a user with administrative access to Approval Processes must define system-level or group-level project approval processes before you can associate them with a template. For more information about creating approval processes, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Create an approval process for work items</a>.</p> <p>Consider the following when adding approval processes: </p> 
      <ul> 
      <li>Only active approval processes display in the list. </li> 
      <li> <p>System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the template does not display in the list.</p> <p><b>IMPORTANT</b> 
      
      If the group associated with the template changes, the group-specific approval process becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">How group and approval process changes affect assigned approval processes</a>. </p> </li> 
      <li> <p>If you added a single-use approval process, it displays as "Custom" in this field. For information, see <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associate a new or existing approval process with work</a>. </p> 
      </li> 
      <li> <p>When bulk-editing templates, the following scenarios exist:</p> 
      <ul> 
         <li> <p>When you select templates from the same group, both system-level and group-level approval processes display in this field.</p> </li> 
         <li> <p>When you select templates from different groups, only system-level approval processes display in this field.</p> </li> 
         <li> <p>When any of the templates has a single-use approval process attached, it is replaced by the system-level you select. </p> </li> 
      </ul> </li> 
      </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Filter Hour Types</strong> </td> 
      <td> <p>Consider the following:</p> <p>Select <strong>No</strong> to make all project-specific hour types available on the future project. (This is the default selection)</p> <p>Or</p> <p>Select <strong>Yes</strong> to make only a subset of the project-specific hour types available on the future project, then select the hour types you want to make available. (Hold the Shift key to select multiple hour types.)</p> <p>If you select this option, only the hour types you select are made available to select when logging hours on the project (or on tasks and issues within the project). You must select at least one hour type; if you select this option and you do not select any hour types, all hour types are made available on the project.</p> <p>The same hour type selections must be made at the individual user level in order for the user to see these hour type options on the project. </p> <p>For more information about defining hour types at the user level, see the section <a href="../../../timesheets/create-and-manage-timesheets/log-time.md#understa" class="MCXref xref">Log time</a> in <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Log time</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Reminder Notification</strong> </td> 
      <td>Select the Reminder Notification that should be associated with the future project. You must configure Reminder Notifications for projects for this field to appear during editing a template. <br>For more information about configuring Reminder Notifications, see <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Set up reminder notifications</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.  
   Or
1. Click **Save Changes**.

### Access {#access}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Access**.

   ![](assets/edit-template-access-with-tasks-and-issues-350x241.png)

   The Access you specify for your template will become the Access of users associated with the project when the template is used to create a project.

   Specify the following **Access** information for the template:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>When someone is assigned to a task</strong> </td> 
      <td> <p>Select from <strong>View</strong>, <strong>Contribute,</strong> or <strong>Manage</strong> access to a task. The user assigned to a task is automatically granted this access to the task. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Also grant access to the project</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the project. The user assigned to a task is automatically granted this access to the project, as well. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone is assigned to an issue</strong> </td> 
      <td> <p>Select from <strong>View</strong>, <strong>Contribute,</strong> or <strong>Manage</strong> access to an issue. The user assigned to an issue is automatically granted this access to the issue. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Also grant access to the project</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the project. The user assigned to an issue is automatically granted this access to the project, as well. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone submits a request: Give them access</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the request. When they submit a request to the project, they are granted this access to the request they submitted. For more information, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>People from the same company will inherit the same permissions for all requests</strong> </td> 
      <td> <p>Select this field if you want people from the same company to have the same access to all the requests on the project, whether they submitted them or not.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone is given access to this project: Give them access to ...</strong> </td> 
      <td> <p>Select the access options that you want users to have on the project, if the project is shared with them. Select the specific options for their access, if they are designated as <strong>Viewers</strong>, <strong>Contributors</strong>, or <strong>Managers</strong> when sharing the project with them. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Custom Forms {#custom-forms}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Custom Forms**.

   ![edit_tempate_custom_forms.png](assets/edit-tempate-custom-forms-tasks-with-issues-sections-350x136.png)

1. Select the custom form or forms that you want to associate with the template. You must build the custom forms before they are available to select in this field.

   Only active custom forms display in the list. For more information about building custom forms, see [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   You can add up to ten custom forms to a template.

   The forms will be added to the project that is created from this template. 

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Tasks {#tasks}

You can define the defaults that will be associated with all the new tasks when you add them to a project that is created from the template.

For information about how these settings affect creating new tasks, see [Create tasks overview](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Tasks**.

   ![](assets/edit-template-with-tasks-and-issue-sections-350x144.png)

1. In the **Task Default Approval Process** box, select the Approval Process you want to associate with all new tasks when you add them to a project created from this template. You must create an Approval Process for tasks before you can associate it with tasks. Only active approval processes display in the list. For more information about creating Approval Processes, see [Creating Approval Processes](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
1. In the **Task Default Custom Forms** box, select the custom form or forms that you want to associate with all new tasks when you add them to a project created from this template. You must build the custom forms before they are available to select in this field. Only active custom forms display in the list. For more information about building custom forms, see [Creating Custom Forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). You can associate up to ten custom forms with a task.
1. (Optional) **Select Use Work Effort to automatically calculate task Planned Hours** if you want to enable managing task effort by using&nbsp;Work Effort instead of Planned Hours in the project created from the template.
1. (Conditional and optional) If you selected Use Work Effort to automatically calculate task Planned Hours, click the drop-down menu to update the percentage for each level of Work Effort. The following percentage values are the defaults:
 
   | Work Effort level |Percentage value|
   |---|---|
   | Small |25% |
   | Medium |50% |
   | Large |75% |

  For information about using Work Effort to manage the effort on tasks on projects, see [Work Effort overview](../../../manage-work/tasks/task-information/work-effort.md).

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Issues {#issues}

By editing issue settings, you can prevent users from adding issues inline in the future project created from the template.

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Issues**.

   ![](assets/edit-template-box-with-issues-nwe-350x171.png)

1. (Optional) Deselect the **Allow users to add issues inline** option. It is enabled by default.

   When disabling this option users cannot add issues inline to the project or the tasks in the Issues section, when the project is created from the template.

   >[!TIP]
   >
   >Disable this option if you want to enforce users to complete the New Issue Fields or the custom forms associated with new issues.

   When disabling this option, users with permissions to add issues to the project created from the template can do so by using the New Issue button or a request queue associated with the project.

   For more information about configuring issue settings on projects, see the [Issue Settings](../../../manage-work/projects/manage-projects/edit-projects.md#issue) section in the article [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

   For information about creating issues on projects, see [Create issues](../../../manage-work/issues/manage-issues/create-issues.md). 

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Comment {#comment}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Comment**.

   ![edit_templates_comment.png](assets/edit-templates-comment-with-tasks-and-issues-350x177.png)

1. Specify a comment that you want to display in the updates stream of the template in the available field.

   This comment is visible for everyone with View access to the template and with access to view Notes.

1. Click **Save Changes**.

   Your changes will be submitted for this template.

   Now, when you use this template to create a project all these settings will transfer to the new project.


   <!--drafted section below for the edit template story: 
   remove this tag and add the Preview blurb at the top of this article in yellow, if it's not already there. Keep the "div class" tags below until 23.1 production: 


### Edit a template in the Preview environment {#edit-a-template-in-the-preview-environment}
-->

1. Passa al modello da modificare.
1. (Condizionale) Per modificare informazioni limitate sul modello, fai clic su **Dettagli modello** nel pannello a sinistra, vai alle aree elencate nel pannello a sinistra per modificare le informazioni di ogni area.
1. Per modificare le informazioni nella sezione Dettagli, fai clic sul pulsante **Modifica** icona ![](assets/edit-icon.png), quindi seleziona una delle aree sottostanti, oppure fai clic su **Modifica tutto** per modificare le informazioni in tutte le aree:

   * Panoramica
   * Moduli personalizzati

   I nomi dei moduli doganali vengono visualizzati solo se all’oggetto sono associati moduli personalizzati.

   * Finanz
   >[!TIP]
   >
   >Per informazioni su tutti i campi visualizzati nell’area Dettagli, continuare a modificare tutti i campi utilizzando la casella Modifica modello riportata di seguito.

1. (Condizionale) Per modificare tutte le informazioni sul modello, fai clic sul pulsante **Altro** menu ![](assets/qs-more-icon-on-an-object.png) accanto al nome del modello, quindi fai clic su **Modifica**.

   La **Modifica modello** si apre la casella. Le sezioni di questa casella contengono gli stessi campi disponibili nella sezione Dettagli modello .

1. È consigliabile modificare le informazioni in una delle sezioni seguenti:

   * [Nome Modello](#template-name)
   * [Panoramica](#overview-preview)
   * [Finanz](#finance-preview)
   * [Moduli personalizzati](#custom-forms-preview)
   * [Impostazione progetto](#project-settings)
   * [Impostazioni attività](#task-settings)
   * [Impostazioni problema](#issue-settings)
   * [Accesso](#access-preview)


### Nome Modello{#template-name}

1. Inizia a modificare il modello come descritto sopra.
1. In **Modifica modello** casella, fai clic su **Nome modello**.
1. (Facoltativo) Continua a modificare le sezioni seguenti, a seconda delle informazioni che desideri modificare

   Oppure

   Fai clic su **Salva**.



### Panoramica {#overview-preview}

1. Inizia a modificare il modello come descritto sopra.
1. In **Modifica modello** casella, fai clic su **Panoramica**.

   ![](assets/edit-template-box-overview-section.png)

1. Aggiorna i campi seguenti:

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
         <tr> 
         <td role="rowheader"><strong>Descrizione</strong></td> 
         <td>Aggiungi ulteriori informazioni sul modello.</td> 
       </tr> 
         <tr> 
         <td role="rowheader"><strong>Priorità</strong></td> 
         <td><p>Questo è solo un flag visivo che consente di assegnare priorità ai progetti futuri. Seleziona tra le seguenti opzioni:</p> 
         <ul> 
         <li><p><strong>Nessuno</strong></p></li> 
         <li><p><strong>Basso</strong></p></li> 
         <li><p><strong>Normal</strong></p></li> 
         <li><p><strong>Alta</strong></p></li> 
         <li><p><strong>Urgente</strong></p></li> 
         </ul><p><p>A seconda delle preferenze del progetto selezionate dall’amministratore di Workfront, i nomi delle priorità potrebbero essere diversi. Per ulteriori informazioni sulle priorità di modifica, vedi <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Creare e personalizzare le priorità</a>.</p></p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>URL</strong></td> 
         <td>Specifica un collegamento web relativo alle informazioni su questo modello.</td> 
       </tr>
       <tr> 
       <td role="rowheader"><strong>Tipo di Condizione</strong></td> 
       <td><p>Seleziona tra i seguenti tipi di condizioni:</p> 
         <ul> 
         <li><strong>Manuale:</strong> Il proprietario del progetto imposta manualmente la condizione del progetto sul progetto. <strong></strong></li> 
         <li><strong>Stato di avanzamento:</strong> Workfront imposta automaticamente la condizione del progetto futuro in base allo stato di avanzamento delle attività nel percorso critico. Per ulteriori informazioni sullo stato di avanzamento, consulta <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Panoramica sullo stato dell'avanzamento dell'attività</a>.</li> 
       </ul>
         </td> 
         </tr> 
       <tr> 
         <td role="rowheader"><strong>Modalità Schedule</strong></td> 
         <td><p>Specifica se il progetto che utilizza questo modello è programmato dalla <strong>Data di inizio</strong>o dal <strong>Data completamento</strong>. Questa selezione determina le date pianificate delle attività future sul progetto utilizzando questo modello. </p><p>Seleziona una delle seguenti opzioni: </p> 
       <ul> 
       <li><p><strong>Pianificazione dalla data di inizio</strong>: La data di inizio del modello è in realtà il giorno di inizio. Quando si pianifica un modello dalla data di inizio, Adobe Workfront calcola il giorno di completamento del modello in base alla durata di tutte le attività del modello. Il giorno di inizio del modello diventa la data di inizio pianificata del progetto futuro.</p></li> 
       <li><p><strong>Pianificazione da data di completamento</strong>: La data di completamento del modello è in realtà il giorno di completamento. Quando si pianifica un modello dalla data di completamento, Workfront calcola il giorno iniziale del modello in base alla durata di tutte le attività del modello. Il giorno di completamento del modello diventa la data di completamento pianificata del progetto futuro. </p></li> 
       </ul><p>Per ulteriori informazioni sui giorni di inizio e di completamento delle attività del modello, vedere <a href="../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md" class="MCXref xref">Panoramica dei giorni di inizio e di completamento in un modello</a>. </p><p>L’impostazione Pianifica da per i modelli è simile a quella dei progetti. L’amministratore di Workfront seleziona l’impostazione predefinita da per i progetti nel sistema. Per informazioni sull’impostazione dei valori predefiniti del progetto, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze del progetto a livello di sistema</a>.</p></td> 
       </tr>

   <tr> 
         <td role="rowheader"><strong>Portfolio</strong></td> 
         <td><p>Specifica un Portfolio per i progetti creati da questo modello. È necessario creare prima un Portfolio prima di visualizzarlo nell’elenco a discesa. </p><p>Nell’elenco vengono visualizzati solo i portfolio attivi. Per ulteriori informazioni sulla creazione dei portfolio, consulta <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Creare un portfolio </a>.</p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Programma</strong></td> 
         <td><p>Se hai selezionato un Portfolio per il modello, specifica un <strong>Programma</strong> per il progetto futuro. Alcuni Portfoli potrebbero non disporre di Programmi. È necessario creare prima un programma prima di visualizzarlo in questo elenco a discesa. Nell’elenco vengono visualizzati solo i programmi attivi.</p><p>Per ulteriori informazioni sulla creazione di programmi, consulta <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">Crea un programma</a>.</p></td> 
       </tr>  
       <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
         <td role="rowheader"><strong>Gruppo</strong></td> 
         <td><p>Nell’elenco a discesa , seleziona il gruppo da associare ai progetti creati dal modello. Può essere un gruppo di qualsiasi livello. </p><p>Per selezionare il gruppo di destra, posiziona il cursore sopra di esso e fai clic sull’icona delle informazioni <img src="assets/info-icon.png"> viene visualizzato accanto a esso. Viene visualizzata una descrizione comandi che elenca le informazioni sul gruppo, ad esempio la gerarchia dei gruppi al di sopra di esso e i relativi amministratori.</p> <p><b>NOTE</b>

   <ul> 
       <li><p>Nell’area Progetti della pagina di un gruppo, quando un utente crea un progetto utilizzando un modello per il quale non è selezionato un gruppo, il sistema associa il gruppo attualmente aperto al progetto.</p><p>Questo è diverso da altre aree in cui il sistema associa un gruppo Home di un utente al progetto quando l’utente crea il progetto utilizzando un modello in cui non è selezionato alcun gruppo.</p></li> 
       <li><p>Se un utente seleziona un modello per il quale è stato selezionato un gruppo durante la creazione di un progetto o durante la conversione di un'attività o di un problema in un progetto, può scegliere un gruppo diverso per il progetto.</p></li> 
       <li>Anche se questo campo è disponibile nei modelli solo nella nuova esperienza Adobe Workfront, è possibile visualizzarlo negli elenchi e nei rapporti sia lì che in Adobe Workfront Classic. </li> 
         </ul> </p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Azienda</strong></td> 
         <td><p>Specifica la società da associare al modello. Nell’elenco vengono visualizzate solo le società attive.</p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Proprietario del modello</strong></td> 
         <td><p>L’utente designato come proprietario del modello deve essere un utente attivo di Workfront. </p><p>Considera quanto segue sull'utente designato come proprietario del modello: </p> 
         <ul> 
         <li>Gli vengono assegnate automaticamente le autorizzazioni Manage (Gestisci) per il modello. </li> 
         <li>Vengono aggiunti al team di progetto e ricevono automaticamente le autorizzazioni di gestione per il progetto creato dal modello. </li> 
         <li>Diventano Proprietario del progetto quando il progetto viene creato da questo modello. </li> 
         </ul></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Sponsor modello</strong></td> 
         <td><p>L’utente specificato in questo campo diventa sponsor del progetto quando il modello viene aggiunto al progetto. Questo utente viene aggiunto al team del progetto e riceve automaticamente le autorizzazioni di visualizzazione per il progetto. L’utente designato come sponsor del modello deve essere un utente attivo di Workfront. </p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Responsabile risorse</strong></td> 
         <td><p>Gli utenti specificati ricevono automaticamente le autorizzazioni di gestione per i progetti futuri e possono assegnare risorse alle attività e ai problemi dei progetti. È possibile specificare più di un Resource Manager. </p></td> 
       </tr> 
      </table>

1. (Facoltativo) Continua a modificare le sezioni seguenti, a seconda delle informazioni che desideri modificare.

   Oppure

   Fai clic su **Salva**.

### Finanz {#finance-preview}

1. Inizia a modificare il modello come descritto sopra.
1. In **Modifica modello** casella, fai clic su **Finanza**.

   ![](assets/edit-template-box-finance-section.png)

1. Aggiorna i campi seguenti:

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody>
       <tr> 
         <td role="rowheader"><strong> Valuta</strong></td> 
         <td><p>Specifica la valuta per il progetto futuro, se è diversa dalla valuta predefinita del sistema. Questo campo non è visibile se nel sistema è presente solo la valuta predefinita.<br>Per ulteriori informazioni sulla valuta, consulta <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Imposta i tassi di cambio</a>.</p></td> 
       </tr>
       <tr> 
       <td role="rowheader"><strong>Bdg</strong></td> 
       <td><p>Specificare un budget per i progetti creati da questo modello.</p></td> 
       </tr>  
       <tr> 
         <td role="rowheader"><strong>Metodo Indicizzazione Performance</strong></td> 
         <td><p>Scegli in che modo Workfront calcolerà le metriche del valore realizzato del progetto futuro. Scegli una delle seguenti opzioni:
         <ul>
         <li>Basato su Ore</li>
         <li>Basato su Costo</li>
         </ul>

   Per ulteriori informazioni sul metodo dell&#39;indice delle prestazioni, vedi <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Impostare il metodo Performance Index (PIM)</a>. </p></td>
   </tr> 
         <tr> 
         <td role="rowheader"><strong>Benef Pian</strong></td> 
         <td><p>Specifica il benefit pianificato dei progetti creati da questo modello. Il vantaggio pianificato viene utilizzato nel Business Case del progetto e in Portfoli Optimizer. </p><p>Per ulteriori informazioni sul beneficio pianificato di un progetto, consulta <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Panoramica del progetto Vantaggio pianificato</a>. Quando si calcola il valore netto di un progetto, si tiene conto del beneficio pianificato di un progetto. </p><p>Per ulteriori informazioni sull'utilizzo di Portfoli Optimizer, vedi <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">Gestisci progetti in Portfoli Optimizer</a> </p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Costo Fisso</strong></td> 
         <td><p>Specifica il costo fisso per i progetti creati da questo modello. Questo è diverso dal costo del lavoro che deriva dalle ore del progetto e dal costo della spesa che deriva dall'importo delle spese del progetto. Il costo fisso di un progetto viene preso in considerazione quando si calcola il valore netto di un progetto e fa parte del costo preventivato.</p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Reddito Fisso</strong></td> 
       <td><p>Specifica i ricavi fissi per i progetti creati da questo modello.</p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Richiede l'approvazione del tempo per questo progetto</strong></td> 
       <td><p>Selezionare questa opzione per richiedere al proprietario del progetto futuro creato da questo modello di approvare il tempo di accesso al progetto. Se si utilizzano i record di fatturazione e si seleziona questa opzione, solo le ore approvate sul progetto vengono visualizzate come ore fatturabili disponibili per i record di fatturazione. L’approvazione del tempo di esecuzione del progetto è indipendente dall’approvazione dei fogli presenze. Per ulteriori informazioni sulla richiesta di tempo per l'approvazione di un progetto, consulta <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">Richiedi tempo per l’approvazione di un progetto</a>.</p></td> 
       </tr> 
       </tbody> 
      </table>

1. (Facoltativo) Continua a modificare le sezioni seguenti, a seconda delle informazioni che desideri modificare.

   Oppure

   Fai clic su **Salva**.

### Moduli personalizzati {#custom-forms-preview}

1. Inizia a modificare il modello come descritto sopra.
1. In **Modifica modello** casella, fai clic su **Forms personalizzato**.

   ![](assets/edit-template-box-custom-forms-section.png)

   I nomi dei moduli personalizzati già allegati al modello vengono visualizzati nel pannello a sinistra.

1. Fai clic all’interno del **Aggiungi modulo personalizzato** e selezionare il modulo o i moduli personalizzati che si desidera associare al modello. È necessario creare i moduli personalizzati prima che siano disponibili per la selezione in questo campo.

   Nell’elenco vengono visualizzati solo i moduli personalizzati attivi. Per ulteriori informazioni sulla creazione di moduli personalizzati, vedere [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   È possibile aggiungere fino a dieci moduli personalizzati a un modello.

   I moduli verranno aggiunti al progetto creato a partire da questo modello.

1. (Facoltativo) Aggiornare le informazioni in uno qualsiasi dei campi dei moduli personalizzati. Le informazioni verranno trasferite ai progetti che verranno creati dal modello.

1. (Facoltativo) Fai clic sul pulsante **x** a destra del nome di un modulo personalizzato, quindi fare clic su **Rimuovi** per rimuoverlo dal modello.

1. (Facoltativo) Continua a modificare la sezione seguente, a seconda delle informazioni da modificare.

   Oppure

   Fai clic su **Salva**.

### Impostazione progetto {#project-settings}

1. Inizia a modificare il modello come descritto sopra.
1. In **Modifica modello** casella, fai clic su **Impostazioni progetto**.

   ![](assets/edit-template-box-project-settings-section.png)

1. Aggiorna i campi seguenti:

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
       <tr> 
       <td role="rowheader"><strong>Percorso milestone</strong> </td> 
       <td> <p>Selezionare un percorso Milestone per il modello. Nell’elenco vengono visualizzati solo i percorsi di cardine attivi.<br>Per ulteriori informazioni sui percorsi Milestone, consulta <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Creare un percorso cardine</a>.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Modalità di completamento</strong> </td> 
         <td> <p>Controlla in che modo il progetto futuro verrà contrassegnato come Completo. <br>Seleziona tra le seguenti opzioni:</p> 
         <ul> 
         <li> <p><strong>Automatico</strong>: Il progetto viene contrassegnato come Completo quando vengono completate tutte le attività e i problemi.</p> </li> 
         <li> <p><strong>Manuale</strong>: È necessario selezionare manualmente lo stato Completa per il progetto, al termine di tutte le attività e i problemi. </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Modalità di completamento riepilogo</strong> </td> 
       <td> <p>Controlla il modo in cui le attività principali del progetto futuro vengono contrassegnate come completate. <br>Seleziona tra le seguenti opzioni:</p> 
       <ul> 
       <li> <p><strong>Automatico</strong>: Le attività principali sono contrassegnate come completate e aggiornano automaticamente la percentuale di completamento, quando le attività figlio vengono completate e la percentuale di completamento delle attività figlio viene aggiornata. </p> </li> 
       <li> <p><strong>Manuale</strong>: È necessario aggiornare manualmente la percentuale di completamento e lo stato delle attività principali, indipendentemente dalle modifiche apportate alle attività figlio. </p> </li> 
       </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Tipo Aggiornamento</strong> </td> 
         <td> <p>Controlla quando le modifiche apportate alla timeline del progetto futuro vengono salvate nel progetto. </p> 
         <b>ESEMPIO </b> 
         <p>Le seguenti modifiche al progetto attivano un aggiornamento della timeline del progetto:</p> 
         <ul> 
         <li> <p>aggiornare le date delle attività</p> </li> 
         <li> <p>cambiare le relazioni predecessori<br></p> </li> 
         <li> <p>modificare le relazioni padre-figlio</p> </li> 
         <li> <p>aggiungere o rimuovere le assegnazioni oltre a modificare il vincolo di attività o il tipo di durata.</p> </li> 
         </ul> 
         </div> <p>Seleziona tra le seguenti opzioni:<br></p> 
         <ul> 
         <li> <p><strong>Automatico e On Change</strong> (Impostazione predefinita): La timeline del progetto viene aggiornata ogni volta che si verifica una modifica nel progetto o in un altro progetto da cui dipende la timeline (In seguito a modifica). La timeline del progetto viene aggiornata ogni notte (automatica).<br>Questa è l’impostazione consigliata per questo campo, in quanto assicura che la timeline del progetto sia sempre aggiornata.<br>Quando esegui un'azione su un'attività o su un progetto che attiva il ricalcolo della timeline, vengono visualizzate immediatamente tutte le date disponibili, consentendo di continuare a lavorare. Nei progetti con più di 100 attività, le date che richiedono un ricalcolo più lungo vengono visualizzate brevemente sotto forma di punto interrogativo (tra 1 e 5 secondi, o fino a un minuto per i progetti di grandi dimensioni). Questo indica che il ricalcolo non è ancora completato e che le date sono soggette a modifiche.<br></p> </li> 
         </ul> 
         <ul> 
         <li> <p><strong>Cambia solo</strong>: La timeline del progetto viene aggiornata ogni volta che si verifica una modifica nel progetto o in un altro progetto da cui dipende la timeline. È possibile selezionare questa opzione se si verificano raramente modifiche nel progetto o in altri progetti da cui dipende la timeline.<br></p> </li> 
         </ul> 
         <ul> 
         <li> <p><strong>Solo automatico</strong>: La tempistica del progetto viene aggiornata ogni notte; non viene aggiornato immediatamente dopo le modifiche.<br>È possibile selezionare questa opzione se si verificano più modifiche quotidiane nel progetto o in altri progetti da cui dipende la timeline. Tuttavia, tieni presente che hai scelto questa impostazione, poiché il progetto non verrà aggiornato contemporaneamente alle modifiche apportate.<br></p> </li> 
         </ul> 
         <ul> 
         <li> <p><strong>Solo manuale</strong>: La timeline del progetto viene aggiornata solo quando selezioni l’opzione Ricalcola timeline , come descritto in <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Ricalcolare le timeline dei progetti</a>.<br></p> </li> 
         </ul> <p>È possibile selezionare questa opzione se si apportano più modifiche al progetto contemporaneamente e si desidera che il ricalcolo della timeline si verifichi dopo che sono state apportate tutte le modifiche (anziché dopo ogni singola modifica).</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Pianificazione</strong> </td> 
         <td> <p>Seleziona una pianificazione per il modello. Questo diventerà la pianificazione del progetto creato da questo modello. Questa deve essere la stessa pianificazione assegnata alla maggior parte delle persone che lavorano sul progetto. È necessario creare una pianificazione prima di poterla assegnare a un modello.<br>Per ulteriori informazioni sulla creazione delle pianificazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creare una pianificazione</a>. <br>Se nel sistema non sono state create pianificazioni personalizzate, viene selezionata l'opzione Pianificazione predefinita. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Indisponibilità utente</strong> </td> 
         <td> <p>Determina se l'ora dell'assegnatario principale di un'attività regola le date pianificate dell'attività. Quando alleghi il modello a un progetto esistente e il modello presenta un’impostazione diversa per questo campo rispetto al progetto, l’impostazione del progetto rimane invariata. L'opzione predefinita per questa impostazione per un nuovo modello è la stessa della preferenza di progetto a livello di sistema. </p> <p>Per informazioni sulle preferenze del progetto a livello di sistema, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze del progetto a livello di sistema</a>. </p> <p>Per informazioni su come questa impostazione influisce sulle date delle attività di un progetto, consulta <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Modifica progetti</a>.<br>Seleziona tra le seguenti opzioni:<br></p> 
         <ul> 
         <li> <p><strong>Considerare il tempo di inattività dell'utente nelle durate delle attività</strong>: Quando si seleziona questa opzione, le date pianificate delle attività sul progetto creato da questo modello si adeguano in base al tempo di esecuzione dell'assegnatario principale dell'attività, se il tempo di inattività si verifica durante la durata dell'attività. </p> </li> 
         <li> <p><strong>Ignora il tempo di inattività dell'utente nelle durate dell'attività</strong>: Quando si seleziona questa opzione, le date pianificate delle attività sul progetto creato da questo modello rimangono come originariamente pianificato, anche se l'Assegnatario principale dell'attività ha un tempo di inattività durante la durata dell'attività. </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Modalità Livellamento Risorse</strong> </td> 
         <td> <p>Seleziona tra le seguenti opzioni:<br></p> 
         <ul> 
         <li> <p><strong>Manuale</strong>: devi livellare manualmente le risorse sul progetto creato da questo modello (questa è l’impostazione predefinita)</p> </li> 
         <li> <p><strong>Automatico:</strong> Workfront livella le risorse sul progetto futuro. <br>Per ulteriori informazioni sul livellamento delle risorse, consulta <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">Risorse di livello nel diagramma di Gantt </a>. </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Rischio</strong> </td> 
         <td> <p>Definire il livello di rischio dei progetti creati da questo modello. Il rischio è solo un indicatore di quanto un progetto possa essere rischioso. Puoi assegnare priorità all’esecuzione dei progetti in base al livello di rischio.<br>Prendi in considerazione la scelta tra i seguenti livelli di rischio:<br></p> 
         <ul> 
         <li> <p><strong>Bassisimo</strong> </p> </li> 
         <li> <p><strong>Basso</strong> </p> </li> 
         <li> <p><strong>Medio</strong> </p> </li> 
         <li> <p><strong>Alta</strong> </p> </li> 
         <li> <p><strong>Altissimo</strong> </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Gruppi di risorse</strong> </td> 
         <td> <p>Specifica i pool di risorse associati al modello. I pool di risorse sono insiemi di utenti necessari allo stesso tempo per il completamento di un progetto. Per ulteriori informazioni sui pool di risorse, consulta <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Panoramica dei pool di risorse </a>.</p> <p> <p><b>NOTA</b>

   Quando modifichi modelli in blocco, in questo campo vengono visualizzati solo i pool di risorse comuni a tutti i modelli selezionati. Se i modelli selezionati non dispongono di pool di risorse condivise, questo campo sarà vuoto. I pool di risorse qui specificati sovrascriveranno i singoli pool di risorse dei modelli.</p> </p> </td>
   </tr>
       <tr> 
         <td role="rowheader"><strong>Filtra il tipo di ore</strong> </td> 
         <td> <p>Considera quanto segue:</p> <p>Seleziona <strong>No</strong> per rendere disponibili nel progetto futuro tutti i tipi di ora specifici per il progetto. (Questa è la selezione predefinita)</p> <p>Oppure</p> <p>Seleziona <strong>Sì</strong> per rendere disponibile nel progetto futuro solo un sottoinsieme dei tipi di ora specifici del progetto, seleziona i tipi di ora che desideri rendere disponibili. Tenete premuto il tasto Maiusc per selezionare più tipi di ora.</p> <p>Se selezioni questa opzione, solo i tipi di ora selezionati vengono resi disponibili per selezionare durante la registrazione delle ore sul progetto (o su attività e problemi all’interno del progetto). Selezionare almeno un tipo di ora; se selezioni questa opzione e non selezioni alcun tipo di ora, nel progetto vengono resi disponibili tutti i tipi di ora.</p> <p>Per visualizzare queste opzioni relative al tipo di ora nel progetto, è necessario effettuare le selezioni dello stesso tipo di ora a livello di singolo utente. </p> <p>Per ulteriori informazioni sulla definizione dei tipi di ora a livello di utente, consulta la sezione <a href="../../../timesheets/create-and-manage-timesheets/log-time.md#understa" class="MCXref xref">Tempo di log</a> in <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Tempo di log</a>.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Processo di approvazione</strong> </td> 
         <td> <p>Selezionare il processo di approvazione da associare al modello. Per poter essere associati a un modello, l’amministratore di Workfront o un utente con accesso amministrativo ai processi di approvazione deve definire processi di approvazione a livello di sistema o di gruppo. Per ulteriori informazioni sulla creazione dei processi di approvazione, consulta <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Creazione di un processo di approvazione per gli elementi di lavoro</a>.</p> <p>Quando si aggiungono processi di approvazione, considera quanto segue: </p> 
         <ul> 
         <li>Nell’elenco vengono visualizzati solo i processi di approvazione attivi. </li> 
         <li> <p>Nell'elenco vengono visualizzati i processi di approvazione a livello di sistema e di gruppo. Un processo di approvazione associato a un gruppo diverso da quello del modello non viene visualizzato nell'elenco.</p> <p><b>IMPORTANTE</b>

   Se il gruppo associato al modello cambia, il processo di approvazione specifico per il gruppo diventa un processo di approvazione a uso singolo. Per ulteriori informazioni su come le modifiche apportate al gruppo del progetto o al processo di approvazione influiscono sulle impostazioni di approvazione, vedere <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">Effetti delle modifiche al processo di approvazione e di gruppo sui processi di approvazione assegnati</a>. </p> </li>
   <li> <p>Se hai aggiunto un processo di approvazione per uso singolo, in questo campo viene visualizzato come "Personalizzato". Per informazioni, consulta <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associa un processo di approvazione nuovo o esistente al lavoro</a>. </p> 
         </li> 
         <li> <p>Quando si modificano in serie i modelli, esistono i seguenti scenari:</p> 
         <ul> 
            <li> <p>Quando si selezionano modelli dello stesso gruppo, in questo campo vengono visualizzati sia i processi di approvazione a livello di sistema che quelli a livello di gruppo.</p> </li> 
            <li> <p>Quando si selezionano modelli da gruppi diversi, in questo campo vengono visualizzati solo i processi di approvazione a livello di sistema.</p> </li> 
            <li> <p>Quando uno dei modelli presenta un processo di approvazione a uso singolo allegato, viene sostituito dal livello di sistema selezionato. </p> </li> 
         </ul> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Notifica promemoria</strong> </td> 
         <td>Selezionare la notifica del promemoria da associare al progetto futuro. È necessario configurare le notifiche dei promemoria per i progetti per questo campo affinché venga visualizzato durante la modifica di un modello. <br>Per ulteriori informazioni sulla configurazione delle notifiche dei promemoria, vedi <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Impostare le notifiche dei promemoria</a>.</td> 
       </tr> 
       </tbody> 
      </table>

1. (Facoltativo) Continua a modificare le sezioni seguenti, a seconda delle informazioni che desideri modificare.\
   Oppure
1. Fai clic su **Salva**.

### Impostazioni attività {#task-settings}

È possibile definire i valori predefiniti che verranno associati a tutte le nuove attività quando le si aggiunge a un progetto creato dal modello.

Per informazioni su come queste impostazioni influiscono sulla creazione di nuove attività, consulta [Panoramica sulla creazione di attività](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. Inizia a modificare il modello come descritto sopra.
1. In **Modifica modello** casella, fai clic su **Impostazioni attività**.

   ![](assets/edit-template-box-tax-settings-section.png)

1. In **Processo di approvazione predefinito dell&#39;attività** selezionare il processo di approvazione che si desidera associare a tutte le nuove attività quando le si aggiunge a un progetto creato da questo modello. È necessario creare un processo di approvazione per le attività prima di associarlo alle attività. Nell’elenco vengono visualizzati solo i processi di approvazione attivi. Per ulteriori informazioni sulla creazione dei processi di approvazione, consulta [Creazione di processi di approvazione](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
1. In **Forms personalizzato predefinito dell&#39;attività** selezionare il modulo o i moduli personalizzati che si desidera associare a tutte le nuove attività quando si aggiungono a un progetto creato da questo modello. È necessario creare i moduli personalizzati prima che siano disponibili per la selezione in questo campo. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi. Per ulteriori informazioni sulla creazione di moduli personalizzati, vedere [Creazione di un Forms personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). È possibile associare fino a dieci moduli personalizzati a un’attività.
1. (Facoltativo) Seleziona **Utilizzare gli sforzi di lavoro per calcolare automaticamente le ore pianificate delle attività** se si desidera abilitare la gestione dello sforzo dell&#39;attività utilizzando l&#39;impegno di lavoro invece di Ore pianificate nel progetto creato dal modello.
1. (Condizionale e facoltativo) Se si seleziona Usa impegno lavoro per calcolare automaticamente le ore pianificate delle attività, fare clic sul menu a discesa per aggiornare la percentuale per ogni livello di sforzo di lavoro. I valori percentuali seguenti sono i valori predefiniti:

   | Livello di sforzo di lavoro | Valore percentuale |
   |---|---|
   | Piccolo | 25% |
   | Medio | 50% |
   | Grande | 75% |

   Per informazioni sull&#39;utilizzo dello sforzo di lavoro per gestire lo sforzo sulle attività relative ai progetti, vedere [Panoramica sullo sforzo di lavoro](../../../manage-work/tasks/task-information/work-effort.md).

1. (Facoltativo) Continua a modificare la sezione seguente, a seconda delle informazioni da modificare.

   Oppure

   Fai clic su **Salva**.

### Impostazioni problema {#issue-settings}

Modificando le impostazioni dei problemi, puoi impedire agli utenti di aggiungere problemi in linea nel progetto futuro creato dal modello.

1. Inizia a modificare il modello come descritto sopra.
1. In **Modifica modello** casella, fai clic su **Impostazioni dei problemi**.

   ![](assets/edit-template-box-issue-settings-section.png)

1. (Facoltativo) Deseleziona la **Consenti agli utenti di aggiungere problemi in linea** opzione . È attivata per impostazione predefinita.

   Quando si disabilita questa opzione, gli utenti non possono aggiungere problemi in linea al progetto o alle attività nella sezione Problemi, quando il progetto viene creato dal modello.

   >[!TIP]
   >
   >Disabilita questa opzione se desideri che gli utenti compilino i campi Nuovo problema o i moduli personalizzati associati ai nuovi problemi.

   Quando disattivi questa opzione, gli utenti con autorizzazioni per aggiungere problemi al progetto creato dal modello possono farlo utilizzando il pulsante Nuovo problema o una coda di richiesta associata al progetto.

   Per ulteriori informazioni sulla configurazione delle impostazioni dei problemi nei progetti, consulta la sezione [Impostazioni dei problemi](../../../manage-work/projects/manage-projects/edit-projects.md#issue) sezione dell&#39;articolo [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

   Per informazioni sulla creazione di problemi relativi ai progetti, consulta [Creare problemi](../../../manage-work/issues/manage-issues/create-issues.md).

1. (Facoltativo) Continua a modificare la sezione seguente, a seconda delle informazioni da modificare.

   Oppure

   Fai clic su **Salva**.

### Accesso {#access-preview}

1. Inizia a modificare il modello come descritto sopra.
1. In **Modifica modello** casella, fai clic su **Accesso**.

   ![](assets/edit-template-box-access-section.png)

   L’accesso specificato per il modello diventerà l’accesso degli utenti associati al progetto quando il modello viene utilizzato per creare un progetto.

   Specifica quanto segue **Accesso** informazioni per il modello:

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
       <tr> 
         <td role="rowheader"><strong>Quando un utente viene assegnato a un'attività</strong> </td> 
         <td> <p>Seleziona da <strong>Visualizza</strong>, <strong>Contribuisci,</strong> o <strong>Gestisci</strong> accesso a un'attività. L’accesso all’attività viene concesso automaticamente all’utente assegnato a un’attività. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Concedere anche l’accesso al progetto</strong> </td> 
         <td> <p> Seleziona da <strong>Visualizza</strong>, <strong>Collaborare</strong>oppure <strong>Gestisci</strong> accesso al progetto. Anche all’utente assegnato a un’attività viene concesso automaticamente questo accesso al progetto. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Quando un utente viene assegnato a un problema</strong> </td> 
         <td> <p>Seleziona da <strong>Visualizza</strong>, <strong>Contribuisci,</strong> o <strong>Gestisci</strong> accesso a un problema. All’utente assegnato a un problema viene automaticamente concesso questo accesso al problema. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Concedere anche l’accesso al progetto</strong> </td> 
         <td> <p> Seleziona da <strong>Visualizza</strong>, <strong>Collaborare</strong>oppure <strong>Gestisci</strong> accesso al progetto. Anche all’utente assegnato a un problema viene concesso automaticamente questo accesso al progetto. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Quando qualcuno invia una richiesta: Dare loro accesso</strong> </td> 
         <td> <p> Seleziona da <strong>Visualizza</strong>, <strong>Collaborare</strong>oppure <strong>Gestisci</strong> accesso alla richiesta. Quando presentano una richiesta al progetto, gli viene concesso l’accesso alla richiesta inviata. Per ulteriori informazioni, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Condividere un problema </a>.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Le persone della stessa società erediteranno le stesse autorizzazioni per tutte le richieste</strong> </td> 
         <td> <p>Seleziona questo campo se desideri che le persone della stessa azienda abbiano lo stesso accesso a tutte le richieste del progetto, sia che le abbiano inviate o meno.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Quando un utente ha accesso a questo progetto: Dare loro accesso a ...</strong> </td> 
         <td> <p>Seleziona le opzioni di accesso che vuoi che gli utenti dispongano del progetto se il progetto è condiviso con loro. Seleziona le opzioni specifiche per il loro accesso, se sono designate come <strong>Visualizzatori</strong>, <strong>Collaboratori</strong>oppure <strong>Manager</strong> quando condividi il progetto con loro. </p> </td> 
       </tr> 
       </tbody> 
      </table>

1. (Facoltativo) Continua a modificare le sezioni seguenti, a seconda delle informazioni che desideri modificare.

   Oppure

   Fai clic su **Salva**.

   Le modifiche verranno inviate per questo modello.

   Ora, quando utilizzi questo modello per creare un progetto, tutte queste impostazioni verranno trasferite al nuovo progetto.


## Modifica in serie di modelli

È possibile modificare i modelli in blocco e aggiornare tutte le relative informazioni contemporaneamente.

Per modificare in blocco i modelli:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Modelli**.
1. Seleziona diversi modelli nell’elenco.
1. Fai clic su **Modifica**.

   La **Modifica modelli** viene visualizzata la finestra di dialogo.

   ![](assets/edit-templates-in-bulk-box-nwe-350x327.png)

1. Fai clic sulle sezioni a sinistra per modificare tutti i modelli selezionati.

   Per ulteriori informazioni sulla modifica delle informazioni sui modelli, consulta la sezione [Modificare un modello](#edit-a-template) in questo articolo.

1. Fai clic su **Salva modifiche**.

   Tutte le modifiche apportate sono ora visibili su tutti i modelli selezionati.

## Aggiungere attività a un modello

Dopo aver creato il modello e aver modificato le informazioni sul modello, è possibile aggiungere attività al modello.

L&#39;aggiunta di attività a un modello è simile all&#39;aggiunta di attività a un progetto.

Per ulteriori informazioni sull’aggiunta di attività a un progetto, consulta [Creazione di attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Quando si aggiungono attività a un modello, la durata del modello e i giorni di inizio e completamento del modello cambiano di conseguenza. Per informazioni sui giorni di inizio e di completamento del modello e delle attività del modello, vedere [Panoramica dei giorni di inizio e di completamento in un modello](../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md).

## Aggiungere altri elementi a un modello

Dopo aver creato il modello e aver modificato le informazioni sul modello, puoi aggiungerne altri. Gli elementi aggiunti saranno disponibili per il progetto quando lo si crea dal modello.

L&#39;aggiunta dei seguenti elementi a un modello è identica all&#39;aggiunta a un progetto:

* Documenti
* Rischi

   Per ulteriori informazioni sulla creazione dei rischi, consulta la sezione [Creare e modificare i rischi relativi ai progetti](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md#create)  sezione dell&#39;articolo [Creare e modificare i rischi relativi ai progetti](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

* Processi di approvazione

   Per informazioni sull&#39;associazione dei processi di approvazione con il lavoro, vedere [Associa un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

* Tariffe di fatturazione

   Per ulteriori informazioni sull&#39;override delle tariffe di fatturazione per un progetto, consulta [Panoramica sulla priorità dei tassi di fatturazione dei ruoli di lavoro e sul calcolo dei ricavi per un progetto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Spese

   Per ulteriori informazioni sull&#39;aggiunta delle spese, consulta [Gestione delle spese di progetto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* Gruppi di argomenti e argomenti della coda

   Per ulteriori informazioni sull&#39;aggiunta di gruppi di argomenti e argomenti della coda a un progetto o a un modello, vedere [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

È possibile aggiungere i seguenti elementi alle attività nel modello:

* Documenti
* Spese

   Per ulteriori informazioni sull&#39;aggiunta delle spese, consulta [Gestione delle spese di progetto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* Approvazioni

   Per ulteriori informazioni sull&#39;associazione delle approvazioni al lavoro, vedere [Associa un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).


## Attivare o disattivare un modello

Puoi disattivare un modello se desideri che gli utenti non siano in grado di trovarlo e crearne di nuovi. Non è possibile allegare un modello disattivato ai progetti né utilizzarlo per creare un progetto.

I modelli disattivati non influiscono sui progetti esistenti creati utilizzando tali modelli.

Per disattivare un modello:

1. Passa a un modello attivo, quindi fai clic sul pulsante **Altro** ![](assets/qs-more-icon-on-an-object.png) accanto al nome del modello, quindi fai clic su **Disattiva**.

   ![](assets/deactivate-template-link-in-more-menu.png)

   Il modello non è più attivo e gli utenti non possono più trovarlo per creare progetti da esso.
1. (Facoltativo) Per attivare il modello, fai clic sul pulsante **Altro** ![](assets/qs-more-icon-on-an-object.png) accanto al nome del modello, quindi fai clic su **Attiva**.

   Il modello è ora attivo e può essere allegato a progetti o utilizzato per creare progetti.