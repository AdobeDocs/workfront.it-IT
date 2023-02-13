---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '''Panoramica sul vincolo di attività: Inizia non oltre"'
description: Avvia non più tardi di (SNLT) è un Vincolo di attività che consente di programmare l'inizio di un'attività prima della data specificata.
author: Alina
feature: Work Management
exl-id: 86139ce6-c6b1-4ac4-a5cb-fd4aa899a025
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Panoramica sul vincolo di attività: Inizia non oltre

Avvia non più tardi di (SNLT) è un Vincolo di attività che consente di programmare l&#39;inizio di un&#39;attività prima della data specificata.

Quando si lavora con il vincolo SNLT, tenere presente quanto segue:

* È necessario utilizzare il vincolo Inizio non più tardi di quando il progetto è pianificato da data di completamento. In questo caso, è possibile fornire un vincolo morbido a un&#39;attività prima che altri task dipendenti vengano visualizzati come a rischio.
* Inizia non più tardi è il vincolo predefinito se un progetto utilizza una modalità di pianificazione di Pianificazione da Data completamento e l&#39;impostazione predefinita del sistema o del gruppo per la data di inizio di un&#39;attività è Oggi. Per informazioni su dove impostare il Vincolo predefinito per una nuova attività, fare riferimento a [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Quando si utilizza il vincolo SNLT con un progetto di pianificazione da data di inizio, Adobe Workfront pianifica l&#39;attività come se si trattasse di un&#39;attività il più presto possibile.
* Quando si sposta o si copia un&#39;attività con un vincolo SNLT in un altro progetto, il vincolo dell&#39;attività o delle date del progetto potrebbe variare a seconda delle date del vincolo e delle date di inizio e completamento del progetto. Esistono i seguenti scenari:

   * Quando il progetto di destinazione è programmato da inizio:

      * Quando la data di vincolo dell&#39;attività è precedente alla data di inizio pianificata del progetto, il vincolo dell&#39;attività diventa Non appena possibile.
      * Quando la data di vincolo dell&#39;attività è successiva alla data di completamento pianificata del progetto, la data di completamento pianificato del progetto viene modificata in modo da corrispondere alla data di vincolo di completamento dell&#39;attività.

      * Quando il progetto di destinazione è programmato da completamento:

         * Quando la data di vincolo dell&#39;attività è successiva alla data di completamento del progetto, il vincolo dell&#39;attività diventa il più tardi possibile.
         * Quando la data di vincolo dell&#39;attività è precedente alla data di inizio pianificata del progetto, la data di inizio pianificata del progetto viene modificata in modo da corrispondere alla data di vincolo iniziale dell&#39;attività.
      * Indipendentemente dalla pianificazione del progetto, quando la data del vincolo dell&#39;attività si trova entro le date di inizio e di completamento del progetto, non vi sono modifiche al Vincolo attività o alle date del progetto.

   Per informazioni sullo spostamento delle attività, consulta [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md).

   Per informazioni sulla copia delle attività, vedere [Copia e duplica le attività](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Per informazioni su come aggiornare il vincolo di attività su un&#39;attività, vedere [Aggiornare il vincolo di attività di un&#39;attività](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Start No Later Than Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Later Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>.<br></li>
</ol>
</div>
-->
