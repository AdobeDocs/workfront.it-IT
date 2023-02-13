---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '''Panoramica sul vincolo di attività: Non Appena Possibile"'
description: Il più presto possibile è un vincolo di attività che posiziona l'ora di inizio dell'attività il più vicino possibile all'inizio del progetto.
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Panoramica sul vincolo di attività: Il più presto possibile

Il più presto possibile è un vincolo di attività che posiziona l&#39;ora di inizio dell&#39;attività il più vicino possibile all&#39;inizio del progetto.

## Considerazioni sull&#39;utilizzo del vincolo Il prima possibile

* Non appena possibile è il vincolo predefinito se un progetto utilizza una modalità di pianificazione da Data inizio e se la data di inizio predefinita del sistema per una nuova attività è impostata su Basato sulla data pianificata del progetto.

* Se un progetto utilizza una modalità di programmazione di Pianificazione dalla data di inizio e se la data di inizio predefinita del sistema o del gruppo per una nuova attività è impostata su Oggi, il Vincolo attività predefinito è Inizio non prima di.

   Per informazioni su dove impostare il Vincolo predefinito per una nuova attività, fare riferimento a [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Per informazioni su come aggiornare il vincolo di attività su un&#39;attività, vedere [Aggiornare il vincolo di attività di un&#39;attività](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Soon As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Soon As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## La differenza tra il tempo disponibile più presto e il più presto possibile

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])&nbsp;</p>
-->

Il vincolo Tempo disponibile più breve è diverso dal vincolo Il più presto possibile quando esistono tutti i seguenti criteri:

* Il progetto è Pianificato dal completamento.
* Le attività del progetto hanno una relazione predecessore.
* L&#39;attività predecessore ha un vincolo di attività flessibile.

In questa situazione:

* **Prima ora disponibile:** L&#39;utilizzo del vincolo Tempo disponibile più breve sull&#39;attività successore dà priorità al vincolo flessibile del predecessore.

   Si supponga, ad esempio, che l&#39;attività A sia un predecessore dell&#39;attività B. L&#39;attività B presenta il vincolo Tempo disponibile più breve e che l&#39;attività A abbia il vincolo Più tardi possibile. In questa situazione, il compito è programmato il più vicino possibile al completamento del progetto.

* **Non Appena Possibile:** In questo scenario, l&#39;utilizzo del vincolo Il prima possibile sull&#39;attività successore dà la priorità all&#39;attività successore.

   Ad esempio, supponiamo che l&#39;attività A sia un predecessore dell&#39;attività B. L&#39;attività B ha il vincolo Il più presto possibile e l&#39;attività A ha il vincolo Il più tardi possibile. In questa situazione, l&#39;attività è pianificata il più vicino possibile all&#39;inizio del progetto.
