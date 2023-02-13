---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '''Panoramica sul vincolo di attività: Il più tardi possibile"'
description: Il più tardi possibile (ALAP) è un vincolo di attività di Adobe Workfront che posiziona l’orario di completamento dell’attività il più vicino possibile alla fine del progetto.
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# Panoramica sul vincolo di attività: Il più tardi possibile

Il più tardi possibile (ALAP) è un vincolo di attività di Adobe Workfront che posiziona l’orario di completamento dell’attività il più vicino possibile alla fine del progetto.

L&#39;utilizzo di questo vincolo potrebbe causare la riprogrammazione di attività precedenti o dipendenti.

Per ulteriori informazioni sulle relazioni predecessori, vedi [Utilizzare i predecessori attività](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md).

Il vincolo predefinito è il più tardi possibile se un progetto utilizza una modalità di pianificazione di Pianificazione da Data completamento e il valore predefinito del sistema o del gruppo per la data di inizio di un&#39;attività si basa sulla data pianificata del progetto.

Per informazioni su dove impostare il Vincolo predefinito per una nuova attività, fare riferimento a [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Per informazioni su come aggiornare il vincolo di attività su un&#39;attività, vedere [Aggiornare il vincolo di attività di un&#39;attività](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible:&nbsp;</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click&nbsp;<strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the&nbsp;<strong>Overview</strong>&nbsp;section, expand the&nbsp;<strong>Task Constraint</strong>&nbsp;drop-down menu.</p> </li>
<li value="4"> <p>Select&nbsp;<strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.&nbsp;</li>
</ol>
</div>
-->

## Differenza tra l&#39;ultima ora disponibile e il più tardi possibile

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
-->

L&#39;ultimo vincolo Tempo disponibile differisce dal vincolo Più tardi possibile quando esistono i seguenti criteri:

* Il progetto è programmato dalla data di inizio
* Le attività del progetto hanno una relazione predecessore
* L&#39;attività successore ha un vincolo di attività flessibile

In questa situazione:

* **Ora disponibile più recente:** L&#39;utilizzo del vincolo Tempo disponibile più recente sull&#39;attività predecessore dà priorità al vincolo flessibile del successore.

   **Esempio:** Ad esempio, l&#39;attività A è un predecessore dell&#39;attività B. L&#39;attività A ha il vincolo Tempo disponibile più recente e l&#39;attività B ha il vincolo Il più presto possibile. In questa situazione, l’attività A è pianificata il più vicino possibile all’inizio del progetto.

   ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **Il Più Tardi Possibile:** In questo scenario, l&#39;utilizzo del vincolo Più tardi possibile sull&#39;attività predecessore dà la priorità all&#39;attività predecessore.

   **Esempio:** Ad esempio, l&#39;attività A è un predecessore dell&#39;attività B. L&#39;attività A ha il vincolo Più tardi possibile e l&#39;attività B ha il vincolo Il più presto possibile. In questa situazione, l’attività A è pianificata il più vicino possibile alla fine del progetto.

   ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

 

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest&nbsp;Available Time constraint differs from the As Late&nbsp;As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest&nbsp;Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest&nbsp;Available Time constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close&nbsp;to the start&nbsp;of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late&nbsp;As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late&nbsp;As Possible&nbsp;constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close to the end&nbsp;of the project as possible.</p> </li>
</ul>
</div>
-->
