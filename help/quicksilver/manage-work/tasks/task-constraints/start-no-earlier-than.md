---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '''Panoramica sul vincolo di attività: Inizia non prima di"'
description: Utilizzare il Vincolo di attività Inizio non precedente a (SNET) per pianificare l'inizio di un'attività dopo la data specificata.
author: Alina
feature: Work Management
exl-id: 857859fb-87ee-4397-b292-239ed9dc8281
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Panoramica sul vincolo di attività: Inizia non prima di

Utilizzare il Vincolo di attività Inizio non precedente a (SNET) per pianificare l&#39;inizio di un&#39;attività dopo la data specificata.

## Panoramica dell&#39;avvio non precedente al vincolo di attività

Quando si utilizza il vincolo Inizio non precedente a Attività, tenere presente quanto segue:

* È necessario utilizzare il vincolo Inizio non prima di quando il progetto è programmato dalla data di inizio. In questo caso, è possibile fornire un vincolo morbido a un&#39;attività prima che altri task dipendenti vengano visualizzati come a rischio.
* Inizia non prima di è il vincolo predefinito se un progetto è programmato dalla data di inizio e se la data di inizio predefinita del sistema o del gruppo per una nuova attività è impostata su Oggi. Per informazioni sulla configurazione delle impostazioni predefinite per le attività, vedere [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Se si pianifica il progetto dalla data di inizio e la data di inizio predefinita del sistema per una nuova attività è impostata su In base alla data pianificata del progetto, il vincolo predefinito per una nuova attività è Il più presto possibile.
* Se si pianifica il progetto Da data di completamento e la data di inizio predefinita del sistema per un nuovo task è impostata su Oggi, il vincolo Start No early Than consente di programmare l&#39;attività come se si trattasse di un&#39;attività il più tardi possibile.
* Quando si sposta o si copia un&#39;attività con un vincolo SNET in un altro progetto, il vincolo dell&#39;attività o delle date del progetto potrebbe variare a seconda delle date del vincolo e delle date di inizio e completamento del progetto. Esistono i seguenti scenari:

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
<h2>Use the Start No Earlier Than Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above)&nbsp;</p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Earlier Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
