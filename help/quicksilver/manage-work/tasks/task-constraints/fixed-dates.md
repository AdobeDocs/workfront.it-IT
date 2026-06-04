---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Panoramica Vincoli Attività: Date Fisse'
description: È possibile utilizzare il vincolo dell'attività Date fisse per specificare la data di inizio e di fine esatte delle attività. Per ulteriori informazioni sui vincoli delle attività, vedere Cenni preliminari sui vincoli delle attività.
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
TQID: https://experienceleague.adobe.com/rVMjo1IgPBQpLatO8jufxGPYTn2W0qghce2v5O-zPRo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 437
ht-degree: 1%

---

# Panoramica sui vincoli attività: date fisse

È possibile utilizzare il vincolo dell&#39;attività Date fisse per specificare la data di inizio e di fine esatte delle attività. Per ulteriori informazioni sui vincoli delle attività, vedere [Panoramica sui vincoli delle attività](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

## Panoramica del vincolo Date fisse

Quando utilizzate il vincolo Date fisse, tenete presente quanto segue:

* Quando si seleziona il vincolo attività Date fisse, è necessario specificare la Data inizio pianificata e la Data completamento pianificata dell&#39;attività. In questo caso, la relazione predecessore dell&#39;attività viene ignorata.
* Il campo Durata dell&#39;attività non è modificabile quando si utilizza il vincolo FIXT. La durata viene calcolata come differenza tra le date di inizio pianificata e di completamento pianificata dell&#39;attività.
* Se il tipo di durata dell&#39;attività è Basato sull&#39;impegno, il numero di assegnatari influisce anche sulla durata dell&#39;attività.
* Quando si sposta o si copia un&#39;attività con un vincolo FIXT in un altro progetto, il vincolo dell&#39;attività o delle date del progetto può variare a seconda delle date del vincolo e delle date di inizio e di completamento del progetto. Esistono i seguenti scenari:

   * Quando il progetto di destinazione è programmato dall’inizio:

      * Quando le date di vincolo dell&#39;attività sono precedenti alla data di inizio del progetto, il vincolo dell&#39;attività viene impostato su Il più presto possibile.
      * Se una o entrambe le date vincolo dell&#39;attività sono successive alla Data completamento pianificata del progetto, la Data completamento pianificata del progetto viene modificata in modo da corrispondere alla data vincolo completamento dell&#39;attività.

   * Quando il progetto di destinazione è programmato dal completamento:

      * Quando le date di vincolo dell&#39;attività sono successive alla Data di completamento del progetto, il vincolo dell&#39;attività diventa Il più tardi possibile.
      * Se una o entrambe le date vincolo dell&#39;attività sono precedenti alla Data inizio pianificata del progetto, la Data inizio pianificata del progetto viene modificata in modo da corrispondere alla data vincolo inizio dell&#39;attività.

   * Indipendentemente dalla programmazione del progetto, se le date vincolo dell&#39;attività sono comprese tra le date di inizio e di completamento del progetto, non verranno apportate modifiche al vincolo attività o alle date del progetto.

  Per informazioni sullo spostamento delle attività, vedere [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md). Per informazioni sulla copia delle attività, vedere [Copia e duplica attività](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Per informazioni su come aggiornare il vincolo attività in un&#39;attività, vedere [Aggiornare il vincolo attività di un&#39;attività](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Fixed Dates Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
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
