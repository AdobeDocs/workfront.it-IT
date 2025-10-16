---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Panoramica Vincoli Attività: Il Più Tardi Possibile'
description: Il più tardi possibile (ALAP) è un vincolo attività di Adobe Workfront che colloca il tempo di completamento dell’attività il più vicino possibile alla fine del progetto.
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Panoramica sui vincoli delle attività: Il più tardi possibile

Il più tardi possibile (ALAP) è un vincolo attività di Adobe Workfront che colloca il tempo di completamento dell’attività il più vicino possibile alla fine del progetto.

L&#39;utilizzo di questo vincolo può causare la riprogrammazione delle attività precedenti o dipendenti.

Per ulteriori informazioni sulle relazioni dei predecessori, vedere [Utilizzare i predecessori delle attività: articolo indice](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md).

Ritardo il più possibile è il vincolo predefinito se un progetto utilizza la modalità di programmazione Pianificazione dalla data di completamento e se la data di inizio di un&#39;attività è Basata sulla data pianificata del progetto.

Per informazioni su dove impostare il vincolo predefinito per una nuova attività, fare riferimento a [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Per informazioni su come aggiornare il vincolo attività in un&#39;attività, vedere [Aggiornare il vincolo attività di un&#39;attività](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Differenza tra l&#39;ultimo orario disponibile e il più tardi possibile

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
-->

Il vincolo Ultimo tempo disponibile è diverso dal vincolo Il più tardi possibile quando sono presenti i seguenti criteri:

* Il progetto è programmato dalla data di inizio
* Le attività del progetto hanno una relazione predecessore
* L&#39;attività successore ha un vincolo di attività flessibile

In questa situazione:

* **Ultimo tempo disponibile:** L&#39;utilizzo del vincolo Ultimo tempo disponibile nell&#39;attività predecessore dà priorità al vincolo flessibile del successore.

  **Esempio:** Ad esempio, l&#39;attività A è un predecessore dell&#39;attività B. L&#39;attività A ha l&#39;ultimo vincolo di tempo disponibile e l&#39;attività B ha il vincolo Il più presto possibile. In questa situazione, l&#39;Attività A è programmata il più vicino possibile all&#39;inizio del progetto.

  ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **Il più tardi possibile:** In questo scenario, l&#39;utilizzo del vincolo Il più tardi possibile sull&#39;attività predecessore dà la priorità all&#39;attività predecessore.

  **Esempio:** Ad esempio, l&#39;attività A è un predecessore dell&#39;attività B. L&#39;attività A ha il vincolo Il più tardi possibile e l&#39;attività B ha il vincolo Il più presto possibile. In questa situazione, l&#39;Attività A è programmata il più vicino possibile alla fine del progetto.

  ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)



<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest Available Time constraint differs from the As Late As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, the task is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, the task is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
