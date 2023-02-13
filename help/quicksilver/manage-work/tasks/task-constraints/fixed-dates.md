---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '''Panoramica sul vincolo di attività: Date fisse"'
description: È possibile utilizzare il vincolo di attività Date fisse quando si desidera specificare la data di inizio e la data di fine esatte delle attività. Per ulteriori informazioni sui vincoli dell'attività, vedere Panoramica sui vincoli dell'attività.
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Panoramica sul vincolo di attività: Date fisse

È possibile utilizzare il vincolo di attività Date fisse quando si desidera specificare la data di inizio e la data di fine esatte delle attività. Per ulteriori informazioni sui vincoli delle attività, vedere [Panoramica sul vincolo di attività](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

## Panoramica del vincolo Date fisse

Quando si utilizza il vincolo Date fisse, tenere presente quanto segue:

* Quando si seleziona il vincolo di attività Date fisse (FIXT), è necessario specificare la data di inizio pianificata e la data di completamento pianificata dell&#39;attività. In questo caso, la relazione predecessore dell&#39;attività viene ignorata.
* Il campo Durata dell&#39;attività non è modificabile quando si utilizza il vincolo FIXT. La durata viene calcolata come differenza tra le date di inizio pianificata e di completamento pianificato dell&#39;attività.
* Se il tipo di durata dell&#39;attività è Guidata da sforzo, il numero di assegnatari dell&#39;attività influisce anche sulla durata dell&#39;attività.
* Quando si sposta o si copia un&#39;attività con un vincolo FIXT in un altro progetto, il vincolo dell&#39;attività o delle date del progetto potrebbe variare a seconda delle date del vincolo e delle date di inizio e completamento del progetto. Esistono i seguenti scenari:

   * Quando il progetto di destinazione è programmato da inizio:

      * Quando le date dei vincoli dell&#39;attività sono precedenti alla data di inizio del progetto, il vincolo dell&#39;attività diventa Il più presto possibile.
      * Quando una o entrambe le date dei vincoli dell&#39;attività sono successive alla data di completamento pianificata del progetto, la data di completamento pianificato del progetto viene modificata in modo da corrispondere alla data del vincolo di completamento dell&#39;attività.
   * Quando il progetto di destinazione è programmato da completamento:

      * Quando le date dei vincoli dell&#39;attività sono successive alla data di completamento del progetto, il vincolo dell&#39;attività diventa il più tardi possibile.
      * Quando una o entrambe le date dei vincoli dell&#39;attività sono precedenti alla data di inizio pianificata del progetto, la data di inizio pianificata del progetto viene modificata in modo da corrispondere alla data del vincolo iniziale dell&#39;attività.
   * Indipendentemente dalla pianificazione del progetto, quando le date dei vincoli dell&#39;attività si trovano entro le date di inizio e di completamento del progetto, non vi sono modifiche al Vincolo attività o alle date del progetto.

   Per informazioni sullo spostamento delle attività, consulta [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md). Per informazioni sulla copia delle attività, vedere [Copia e duplica le attività](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Per informazioni su come aggiornare il vincolo di attività su un&#39;attività, vedere [Aggiornare il vincolo di attività di un&#39;attività](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Fixed Dates Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above) </p>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Fixed Dates</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start on this date. </p> </li>
<li value="6"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete on this date. </p> </li>
<li value="7">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
