---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '''Panoramica sul vincolo di attività: Tempo disponibile anticipato"'
description: Tempo disponibile più breve è un vincolo di task che consente di programmare l'inizio di un'attività al più presto disponibile dopo aver considerato le relazioni predecessori.
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Panoramica sul vincolo di attività: Tempo disponibile

Tempo disponibile più breve è un vincolo di task che consente di programmare l&#39;inizio di un&#39;attività al più presto disponibile dopo aver considerato le relazioni predecessori.

Per informazioni su come aggiornare il vincolo di attività su un&#39;attività, vedere [Aggiornare il vincolo di attività di un&#39;attività](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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

## La differenza tra il tempo disponibile più presto e il più presto possibile

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

Il vincolo Tempo disponibile più breve è diverso dal vincolo Il più presto possibile quando esistono tutti i seguenti criteri:

* Il progetto è programmato da completamento
* Le attività del progetto hanno una relazione predecessore
* L&#39;attività predecessore ha un vincolo di attività flessibile

In questa situazione:

* **Prima ora disponibile:** L&#39;utilizzo del vincolo Tempo disponibile più breve sull&#39;attività successore dà priorità al vincolo flessibile del predecessore.

   **Esempio:** L&#39;attività A è un predecessore dell&#39;attività B. L&#39;attività B ha il vincolo Tempo disponibile più presto e l&#39;attività A ha il vincolo Più tardi possibile. In questa situazione, il compito B è programmato il più vicino possibile al completamento del progetto.

   ![Vincolo di tempo disponibile più presto quando l&#39;attività ha le date prossime alla data di completamento del progetto](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **Non Appena Possibile:** In questo scenario, l&#39;utilizzo del vincolo Il prima possibile sull&#39;attività successore dà la priorità all&#39;attività successore.

   **Esempio:**  L&#39;attività A è un predecessore dell&#39;attività B. L&#39;attività B ha il vincolo Il più presto possibile e l&#39;attività A ha il vincolo Il più tardi possibile. In questa situazione, l&#39;attività B è pianificata il più vicino possibile all&#39;inizio del progetto.

   ![Vincolo quanto prima possibile quando l&#39;attività ha le date prossime alla data di inizio del progetto](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
