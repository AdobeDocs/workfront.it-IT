---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Panoramica Vincoli Attività: Primo Orario Disponibile'
description: Primo orario disponibile è un vincolo dell'attività che pianifica l'inizio di un'attività il più presto possibile dopo aver preso in considerazione le relazioni precedenti.
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
TQID: https://experienceleague.adobe.com/htQAqPWSYcdft3g3RDQuRu3VdmxmvVQt2EFrvFJsRU4
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
source-wordcount: 299
ht-degree: 2%

---

# Panoramica sui vincoli attività: primo orario disponibile

Primo orario disponibile è un vincolo dell&#39;attività che pianifica l&#39;inizio di un&#39;attività il più presto possibile dopo aver preso in considerazione le relazioni precedenti.

Per informazioni su come aggiornare il vincolo attività in un&#39;attività, vedere [Aggiornare il vincolo attività di un&#39;attività](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above) </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To update the Task Constraint to Earliest Available Time:</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to a task whose constraint you want to modify. </li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit Task</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Earliest Available Time</strong>.</p>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save Changes</strong>.</li>
   -->

## Differenza tra l&#39;orario disponibile più presto e il più presto possibile

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

Il vincolo Primo tempo disponibile è diverso dal vincolo Il più presto possibile quando sono presenti tutti i seguenti criteri:

* Il progetto è programmato dal completamento
* Le attività del progetto hanno una relazione predecessore
* L&#39;attività predecessore ha un vincolo di attività flessibile

In questa situazione:

* **Primo orario disponibile:** L&#39;utilizzo del vincolo Primo orario disponibile sull&#39;attività successore dà priorità al vincolo flessibile del predecessore.

  **ESEMPIO**

  L&#39;attività A è un predecessore dell&#39;attività B. L&#39;attività B ha il vincolo Primo tempo disponibile e l&#39;attività A ha il vincolo Il più tardi possibile. In questa situazione, l&#39;Attività B è programmata il più vicino possibile al completamento del progetto.

  ![Primo vincolo di tempo disponibile quando le date dell&#39;attività sono vicine alla data di completamento del progetto](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **Il più presto possibile:** In questo scenario, l&#39;utilizzo del vincolo Il più presto possibile sull&#39;attività successore conferisce la priorità all&#39;attività successore.

  **ESEMPIO**

  L&#39;attività A è un predecessore dell&#39;attività B. L&#39;attività B ha il vincolo Il più presto possibile e l&#39;attività A ha il vincolo Il più tardi possibile. In questa situazione, l&#39;Attività B è programmata il più vicino possibile all&#39;inizio del progetto.

  ![Vincolo Il più presto possibile quando le date dell&#39;attività sono vicine alla data di inizio del progetto](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
