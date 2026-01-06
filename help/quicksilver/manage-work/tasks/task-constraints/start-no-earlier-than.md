---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Panoramica Vincoli Attività: Iniziare Non Prima Di'
description: Utilizzare il vincolo di attività Inizia non prima del (SNET) per pianificare l'inizio di un'attività dopo la data specificata.
author: Alina
feature: Work Management
exl-id: 857859fb-87ee-4397-b292-239ed9dc8281
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Panoramica sui vincoli attività: Iniziare non prima di

Utilizzare il vincolo di attività Inizia non prima del (SNET) per pianificare l&#39;inizio di un&#39;attività dopo la data specificata.

## Panoramica del vincolo Inizia non prima del task

Quando si utilizza il vincolo Iniziare non prima del task, tenere presente quanto segue:

* Utilizzare il vincolo Iniziare non prima di quando il progetto è programmato dalla data di inizio. In questo caso, è possibile fornire un vincolo morbido a un&#39;attività prima che quest&#39;ultima obblighi altre attività dipendenti a essere visualizzate come A rischio.
* Iniziare non prima di è il vincolo predefinito se un progetto è programmato Dalla data di inizio e se la data di inizio predefinita del sistema o del gruppo per una nuova attività è impostata su Oggi. Per informazioni sulla configurazione delle impostazioni predefinite per le attività, vedere [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Se si pianifica il progetto Dalla data di inizio e la data di inizio predefinita del sistema per una nuova attività è impostata su In base alla data pianificata del progetto, il vincolo predefinito per una nuova attività è Il più presto possibile.
* Se si pianifica il progetto Da data di completamento e la data di inizio predefinita del sistema per una nuova attività è impostata su Oggi, il vincolo Iniziare non prima di pianifica l&#39;attività come se fosse un&#39;attività Il più tardi possibile.
* Quando si sposta o si copia un&#39;attività con un vincolo SNET in un altro progetto, il vincolo dell&#39;attività o delle date del progetto può variare a seconda delle date del vincolo e delle date di inizio e di completamento del progetto. Esistono i seguenti scenari:

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
<h2>Use the Start No Earlier Than Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
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
