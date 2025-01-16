---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Panoramica delle assegnazioni intelligenti
description: Quando gestisci le assegnazioni di attività e problemi, puoi utilizzare le assegnazioni intelligenti per identificare l’utente migliore per completare il lavoro. Le assegnazioni intelligenti sono suggerimenti che Adobe Workfront presenta quando si assegnano elementi di lavoro alle risorse in base a un algoritmo che determina la risorsa più appropriata per il processo.
author: Alina
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# Panoramica delle assegnazioni intelligenti

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">Le informazioni evidenziate in questa pagina fanno riferimento alle funzionalità disponibili solo nell&#39;ambiente di anteprima.</span>

<!--<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview"> This functionality will be removed from the Production environment for customers who enabled fast release with the 25.1 release in January 2025. For information about the 25.1 release, see [First Quarter 2025 release overview](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md). -->

Quando gestisci le assegnazioni di attività e problemi, puoi utilizzare le assegnazioni intelligenti per identificare la risorsa migliore per completare il lavoro.

Le assegnazioni intelligenti sono suggerimenti che Adobe Workfront presenta quando si assegnano elementi di lavoro alle risorse in base a un algoritmo che determina la risorsa più appropriata per il processo. Le assegnazioni intelligenti possono essere utenti, mansioni o team.

>[!NOTE]
>
>Quando si suggeriscono gli utenti, le assegnazioni intelligenti non tengono conto della disponibilità dell’utente. Tuttavia, la loro disponibilità in base alle loro pianificazioni influisce sulle Date pianificate e previste delle attività e dei problemi quando vengono assegnate. Per informazioni sulle pianificazioni, vedere l&#39;articolo [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Questo articolo contiene informazioni generali sulle assegnazioni avanzate. Per informazioni sull&#39;utilizzo delle assegnazioni avanzate per assegnare attività e problemi agli utenti, vedere [Assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md).

## Panoramica delle assegnazioni intelligenti

Quando si lavora con le assegnazioni intelligenti, considera quanto segue:

<!--* <span class="preview">The algorithm works independently for tasks and issues. This means that the list of suggested users for issues might differ from the list of suggested users for a task because Workfront builds the lists according to criteria pertaining to issues and tasks separately. </span>-->
<!--not sure this is accurate: * Smart assignments do not recommend job roles or teams. Instead, they are suggestions of users who are best fit to complete a task or an issue. -->
* Le assegnazioni suggerite sono sempre utenti attivi, mansioni o team.
* La risorsa elencata per prima deve corrispondere al meglio per l&#39;attività.

## Individuazione suggerimenti assegnazione avanzata

Puoi visualizzare le assegnazioni intelligenti nelle seguenti aree, dove puoi assegnare attività o problemi:

* Un elenco di problemi o un report nella colonna Assegnazioni

  ![](assets/smart-assignments-issue-list.png)

* Un elenco di attività o un report nella colonna Assegnazioni

  ![](assets/smart-assignments-task-list.png)

* Un&#39;intestazione di attività nel campo Assegnazioni

  ![](assets/smart-assignments-task-header-nwe-350x302.png)

* Intestazione di un problema nel campo Assegnazioni

  ![](assets/smart-assignments-issue-header.png)

* Pannello Riepilogo attività o problemi nell’area Assegnazioni

  ![](assets/issue-assignments-summary-panel.png)

<!--* The Assignments field in the New Task box, when adding a task to a project

  ![](assets/smart-assignments-new-task-modal.png)-->

<!--this is not possible in the new home  - we have Summary there: 
* The Assignments field for an item listed in the Home area, when you open a task or issue

  ![](assets/smart-assignments-in-home-nwe-350x216.png)
-->

* Bilanciatore dei carichi di lavoro nell’area Assegnato a quando si assegna un’attività o un problema

  ![](assets/smart-assignments-workload-balancer-bulk-assignments.png)


## Criteri di assegnazione intelligenti

<!--Smart assignments work differently for tasks than for issues.  -->

<!--### Smart assignments criteria for tasks

The task smart assignments calculation works in <span class="preview">two phases which use two different algorithms.</span>

<span class="preview">Depending on which algorithm finds the smart assignment, the assignments are listed under two separate sections in the Assignments field.</span> For information, see [Make smart assignments](/help/quicksilver/manage-work/tasks/assign-tasks/make-smart-assignments.md). 

![](assets/smart-assignments-task-list.png)

<div class="preview">

#### First phase of smart assignment calculation for tasks 

In the first phase of calculating smart assignments, Workfront calculates a similarity score for every assignment. 

>[!NOTE]
>
>The first phase of the smart assignments calculation does not apply to the following task areas:
>
>* Bulk Assignments in the Workload Balancer.
>* Connected cards on boards.


The calculation for the similarity score and the order in which the assignments are listed take into account the following:  

* A score of 100% is given to an existing assignment where the task, project, and portfolio names are identical to the task you're trying to assign. The project and portfolio names of the task of an existing assignment must also match the project and portfolio of the task you are trying to assign.   

* If only some of this information from other assignments matches on the existing tasks, the score might be lower than 100%.  

  For example, if you are assigning a task called "My second task" on a project called "My project" in a portfolio called "My portfolio" and you have an existing task called "My task" in another project called "My project" in a portfolio called "My portfolio", the user assigned to "My task" might get a score of 95% because the name of the existing task and the task you're trying to assign now are similar, but not identical.  
 
    >[!TIP]
    >
    >  Workfront looks for matches only in the Name fields of tasks, projects, and portfolios and not in any other fields. 

* An assignment could get a higher score when they are assigned to a lot of tasks in the system that have similar names. For example, if a team called "Development" is assigned to 50% of the tasks in the system containing "AI" in the name and you are now assigning another task with "AI" in the name, the score of the "Development" team is higher. In this case, the names of  projects and portfolios are not as important.  

* Taking into account this scoring system, the first 7 suggestions are listed as smart assignments, in the descending order of their scores. Assignments with scores lower than 40% do not display.  

* If several assignments have identical scores, they display in order of the date on which the assignments were made, starting from the most recent date.  

  For example, if Rick was assigned to a similar task earlier today and Jennifer was assigned to a similar task two days ago, Rick displays first.  

* Assignments identified in this phase are listed in the    **Suggested assignments**  section of the Assignments field for tasks. 

* If there are no matches using this calculation, the second phase of smart assignments starts which is calculated using a different algorithm.  

</div>

#### Second phase of smart assignment calculation for tasks-->

<!--If the first step of task smart assignments has found no matches,-->

Workfront calcola le assegnazioni intelligenti per le attività nello stesso modo in cui le calcola per i problemi.

<!--For more information, see the section [Smart assignments criteria for tasks and issues](#smart-assignments-criteria-for-tasks-and-issues) in this article. -->

Le assegnazioni identificate sono elencate nelle sezioni **Utenti e team**, **Assegnazioni mansioni** e <span class="preview">**Ruoli scheda valutazione**</span> del campo Assegnazioni. <span class="preview">Per ulteriori informazioni sulle schede delle tariffe, vedi [Gestire le schede delle tariffe](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)</span>. <!--keep the rate cards roles in yellow after the release of assignments to Prod-->

<!--
### Smart assignments criteria for tasks and issues 

>[!NOTE]
>
>The following criteria applies for tasks only when the first phase of the task smart assignment calculation did not find any matches. For information, see the section [First phase of smart assignment calculation for tasks](#first-phase-of-smart-assignment-calculation-for-tasks) in this article. The following criteria always applies for issues, by default. -->

![](assets/smart-assignments-issue-header.png)

Gli utenti sono consigliati nell’elenco a discesa delle assegnazioni intelligenti in base a una combinazione dei seguenti criteri (elencati in ordine crescente e decrescente):

1. Utenti assegnati ad altri elementi di lavoro negli ultimi 30 giorni dall&#39;utente che ha effettuato l&#39;assegnazione. Vengono visualizzati i primi 50 utenti che soddisfano questo criterio. Viene visualizzato per primo l’utente assegnato più di frequente.

2. Se l’elemento di lavoro è assegnato a un team o a un ruolo, l’elenco degli utenti suggeriti viene filtrato ulteriormente tenendo conto delle assegnazioni esistenti di seguito. In questo caso, nell’elenco dei suggerimenti vengono visualizzati solo i seguenti utenti:

   * Utenti il cui Team predefinito è il team assegnato all&#39;elemento di lavoro.
   * Utenti il cui ruolo principale è il ruolo assegnato all&#39;elemento di lavoro.

>[!TIP]
>
>* Se all’attività o al problema non è assegnato alcun ruolo o team, in Workfront vengono visualizzati tutti gli utenti assegnati per gli ultimi 30 giorni, fino a 50 utenti.
>
>* Se non sono state effettuate assegnazioni negli ultimi 30 giorni, nell&#39;elenco assegnazioni avanzate verranno visualizzati solo gli utenti che appartengono al team assegnato o a cui è stato assegnato il ruolo all&#39;elemento di lavoro.



<!--the commented out piece in the tip above was live before but I am not totally sure that smart assignments look at your team. I think they look JUST at the team/ role assigned to the work item; see this help site request for more info: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/62fd222200037eb87572c5b6ad6bf53e/overview -->
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h3>Smart assignments criteria for the Production environment</h3>
<p>(NOTE: drafted,this was the case BEFORE we updated the logic in the WB - with the 21.4 release)</p>
</div>
<p>Smart assignments display on tasks and issues when the following conditions are met:</p>
<ul>
<li>The task or issue is subordinate to a parent task or issue that has a user, team, or job role currently assigned. </li>
</ul>
<p>Smart assignments display the top twenty recommendations based on a proprietary algorithm that uses your own team information.</p>
<p>Users are recommended in the smart assignments drop-down list based on a combination of the following criteria (listed in order from most important to least important):</p>
<ul>
<li>The user has the team assigned to the task or issue designated as their Home Team</li>
<li>The user is also assigned to the parent task</li>
<li>The user has the same primary job role as is currently assigned to the task or issue</li>
<li>The user has the team assigned to the parent task or issue designated as their Home Team</li>
<li>The user is associated with the same primary job role currently assigned to the parent task</li>
<li>The user is a member of the same team as the user who assigned the task or issue and the team is designated as their Home Team</li>
<li>The user is a member of the same Home Group as the user who is assigning the task or issue</li>
<li>The user has the same primary job role as the user who is assigning the task or issue.</li>
</ul>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Make smart assignments</h2>
<p>(NOTE:&nbsp;this was moved to its own article: make-smart-assignments.) </p>
<p>Smart assignments are available in most locations where you can make assignments in Workfront.</p>
<p>You can use smart assignments on tasks and issues that have previously been assigned to a job role or a team.</p> <note type="note">
You must have a Plan or a Work license and have at least Contribute permissions to a task or an issue to be able to make assignments to the task or the issue. You must have the Make Assignments option enabled in your permission level to make assignments.
</note>
<p>To use smart assignments:</p>
<ol>
<li value="1">Navigate to an issue or a task and click one of the following fields to edit them: <br>
<ul>
<li><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The <strong>Assignments</strong> field in the task or issue header</p></li>
<li>The <strong>Assignments</strong> field of a task or issue list using in-line editing in a task or issue list. </li>
<li>The <strong>Assignee</strong> field after you have clicked <strong>Advanced</strong> from a task or an issue. </li>
</ul></li>
<li value="2"> <p>Place your cursor in the assignment field, and wait for two seconds, then the <strong>Suggestions</strong> list is displayed.</p> <p>Users displayed in this list are the smart assignment suggestions for the task or the issue.<br></p> <p> <img src="assets/nwe-smart-assignment-suggestions-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p>Select the user in the recommendations list by clicking their name. </p> <p>If there are no suggestions, the suggestion list does not open.</p> </li>
<li value="4">(Optional) If you do not want to use one of the recommended users from the smart assignments list, start typing the name of the desired user and select the name when it appears in the list.</li>
<li value="5">Click <strong>Enter</strong> to make the assignment. </li>
</ol>
</div>
-->
