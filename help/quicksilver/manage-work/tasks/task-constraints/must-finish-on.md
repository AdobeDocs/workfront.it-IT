---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Panoramica Vincolo Attività: Deve Finire Il'
description: È possibile utilizzare il vincolo attività Deve finire il (MFO) per pianificare la fine di un'attività in una data specifica.
author: Alina
feature: Work Management
exl-id: 9e546a0f-7f7a-4f1c-9d9d-aa3cea377fdf
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Panoramica sui vincoli attività: deve finire al

È possibile utilizzare il vincolo attività Deve finire il (MFO) per pianificare la fine di un&#39;attività in una data specifica.

Il vincolo Deve finire al pianifica il completamento di un&#39;attività esattamente alla data e all&#39;ora specificate nel campo **Data di completamento pianificata**.

>[!TIP]
>
>Quando si aggiorna manualmente la Data di completamento pianificata di un&#39;attività, il vincolo dell&#39;attività viene impostato su Deve finire al.

## Panoramica del vincolo Must Finish On Task

Quando si pianifica un&#39;attività con un vincolo Deve finire al, tenere presente quanto segue:

* Le relazioni con i predecessori non forzano la riprogrammazione dell&#39;attività. Adobe Workfront essenzialmente ignora le relazioni predecessore.
* L&#39;attività viene visualizzata come **A rischio** se i predecessori iniziano a essere in ritardo o sono in ritardo.

* Quando si sposta o si copia un&#39;attività con un vincolo MFO in un altro progetto, il vincolo dell&#39;attività o delle date del progetto può variare a seconda delle date del vincolo e delle date di inizio e di completamento del progetto. Esistono i seguenti scenari:

   * Quando il progetto di destinazione è programmato dall’inizio:

      * Quando la data di vincolo dell&#39;attività è precedente alla data di inizio pianificata del progetto, il vincolo dell&#39;attività viene impostato su Il più presto possibile.
      * Quando la data vincolo dell&#39;attività è successiva alla data completamento pianificato del progetto, la data completamento pianificato del progetto viene modificata in modo da corrispondere alla data vincolo completamento dell&#39;attività.

      * Quando il progetto di destinazione è programmato dal completamento:

         * Quando la data vincolo dell&#39;attività è successiva alla data di completamento del progetto, il vincolo attività diventa il più tardi possibile.
         * Quando la data vincolo dell&#39;attività è precedente alla data inizio pianificata del progetto, la data inizio pianificata del progetto viene modificata in modo da corrispondere alla data vincolo inizio dell&#39;attività.

      * Indipendentemente dalla programmazione del progetto, se la data vincolo dell&#39;attività è compresa tra le date di inizio e di completamento del progetto, non verranno apportate modifiche al vincolo attività o alle date del progetto.

  Per informazioni sullo spostamento delle attività, vedere [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md). Per informazioni sulla copia delle attività, vedere [Copia e duplica attività](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Per informazioni su come aggiornare il vincolo attività in un&#39;attività, vedere [Aggiornare il vincolo attività di un&#39;attività](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Must Finish On Task Constraint</h2>
<p>To update the Task Constraint to Must Finish On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Finish On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete by this date, and no later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
