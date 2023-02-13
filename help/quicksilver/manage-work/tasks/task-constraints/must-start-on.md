---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '''Panoramica sul vincolo di attività: Deve iniziare'
description: Utilizzare il Vincolo di task deve iniziare su (MSO) per pianificare l'inizio esatto di un'attività in una data specifica.
author: Alina
feature: Work Management
exl-id: 09062d46-2b80-4758-946e-d6dec0f7a7c0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Panoramica sul vincolo di attività: Deve iniziare

Utilizzare il Vincolo di task deve iniziare su (MSO) per pianificare l&#39;inizio esatto di un&#39;attività in una data specifica.

Il vincolo Deve iniziare su pianifica un&#39;attività in modo che inizi esattamente all&#39;ora e alla data specificate nella **Data di inizio prevista** campo .

>[!TIP]
>
>L&#39;aggiornamento manuale della Data inizio pianificata di un&#39;attività modifica il vincolo dell&#39;attività su Deve iniziare su.

## Panoramica del vincolo deve iniziare su attività

Quando si pianifica un&#39;attività con un vincolo Must Start On, tenere presente quanto segue:

* Le relazioni predecessori non forzano la riprogrammazione dell&#39;attività. Workfront ignora sostanzialmente le relazioni precedenti dell&#39;attività con questo vincolo.
* L’attività viene visualizzata **A rischio** se i predecessori iniziano a correre indietro o in ritardo.

* Quando si sposta o si copia un&#39;attività con un vincolo MSO in un altro progetto, il vincolo dell&#39;attività o delle date del progetto potrebbe variare a seconda delle date del vincolo e delle date di inizio e completamento del progetto. Esistono i seguenti scenari:

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
<h2>Use the Must Start On Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Must Start On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Start On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start by this date, and no later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
