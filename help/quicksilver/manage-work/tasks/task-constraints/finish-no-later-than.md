---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '''Panoramica sul vincolo di attività: Fine non oltre"'
description: Fine Non più tardi di (FNLT) è un Vincolo di attività che consente di programmare il completamento di un'attività prima della data specificata.
author: Alina
feature: Work Management
exl-id: ea0e74fb-45a0-4466-b57d-294a9babb340
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Panoramica sul vincolo di attività: Fine entro

Fine Non più tardi di (FNLT) è un Vincolo di attività che consente di programmare il completamento di un&#39;attività prima della data specificata.

## Panoramica del vincolo Fine non oltre

Quando si utilizza il vincolo Fine non più tardi di (FNLT) per un&#39;attività, tenere presente quanto segue:

* Utilizzare questo vincolo quando il progetto è programmato dalla data di inizio. In questo caso, è possibile fornire un vincolo morbido a un&#39;attività prima che altri task dipendenti vengano visualizzati come a rischio.
* Quando si utilizza il vincolo FNLT con un progetto di data di completamento da programma, questo vincolo consente di programmare l&#39;attività come se si trattasse di un&#39;attività il più tardi possibile.
* Quando si sposta o si copia un&#39;attività con un vincolo FNET in un altro progetto, il vincolo dell&#39;attività o delle date del progetto potrebbe variare a seconda delle date del vincolo e delle date di inizio e completamento del progetto. Esistono i seguenti scenari:

   * Quando il progetto di destinazione è programmato da inizio:

      * Quando la data di vincolo dell&#39;attività è precedente alla data di inizio pianificata del progetto, il vincolo dell&#39;attività diventa Non appena possibile.
      * Quando la data di vincolo dell&#39;attività è successiva alla data di completamento pianificata del progetto, la data di completamento pianificato del progetto viene modificata in modo da corrispondere alla data di vincolo di completamento dell&#39;attività.

      * Quando il progetto di destinazione è programmato da completamento:

         * Quando la data di vincolo dell&#39;attività è successiva alla data di completamento del progetto, il vincolo dell&#39;attività diventa il più tardi possibile.
         * Quando la data di vincolo dell&#39;attività è precedente alla data di inizio pianificata del progetto, la data di inizio pianificata del progetto viene modificata in modo da corrispondere alla data di vincolo iniziale dell&#39;attività.
      * Indipendentemente dalla pianificazione del progetto, quando la data del vincolo dell&#39;attività si trova entro le date di inizio e di completamento del progetto, non vi sono modifiche al Vincolo attività o alle date del progetto.

   Per informazioni sullo spostamento delle attività, consulta [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md). Per informazioni sulla copia delle attività, vedere [Copia e duplica le attività](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Per informazioni su come aggiornare il vincolo di attività su un&#39;attività, vedere [Aggiornare il vincolo di attività di un&#39;attività](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Finish No Later Than constraint</h2>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Finish No Later Than</strong>.</p> <p> <img src="assets/fnlt-350x266.png" alt="FNLT.png" style="width: 350;height: 266;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>You must complete the task on and not later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
