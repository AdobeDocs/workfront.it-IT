---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: "Panoramica sui vincoli dell’attività: ultimo orario disponibile"
description: Ultimo orario disponibile (LAT, Latest Available Time) è un tipo di vincolo attività in Adobe Workfront.
author: Alina
feature: Work Management
exl-id: acf55004-9424-4e24-9ff5-90f6fd7f72a6
source-git-commit: c3abb5dce14c0b19ab2e5b82f159cd29f80f79e4
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Panoramica sui vincoli delle attività: ora più recente disponibile

Ultimo orario disponibile (LAT, Latest Available Time) è un tipo di vincolo attività in Adobe Workfront.

## Usa il vincolo attività tempo disponibile più recente

È possibile utilizzare il vincolo LAT quando si desidera pianificare l&#39;inizio di un&#39;attività al più tardi dopo aver considerato le relazioni predecessore-successore nel progetto.

Questo vincolo differisce dal Più presto possibile in quanto non forzerà la riprogrammazione di predecessori o successori. Ha effetto solo sulla pianificazione dell&#39;attività a cui è associata, impostandola sull&#39;ultimo tempo disponibile in base alla relazione con altre attività.

Per informazioni su come aggiornare il vincolo attività in un&#39;attività, vedere [Aggiornare il vincolo attività di un&#39;attività](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To update the Task Constraint to Latest Available Time:</p>
<p>(NOTE: replaced with new article linked above) </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Latest Available Time</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## Differenza tra l&#39;ultimo orario disponibile e il più tardi possibile

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "As Late As Possible"] - inserted snippet in both (Alina)) </p>
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
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
