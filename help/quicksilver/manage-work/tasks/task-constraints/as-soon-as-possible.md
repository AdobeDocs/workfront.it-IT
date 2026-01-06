---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Panoramica Vincoli Attività: Il Prima Possibile'
description: Il più presto possibile è un vincolo attività che posiziona l'ora di inizio dell'attività il più vicino possibile all'inizio del progetto.
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Panoramica sui vincoli delle attività: Il più presto possibile

Il più presto possibile è un vincolo attività che posiziona l&#39;ora di inizio dell&#39;attività il più vicino possibile all&#39;inizio del progetto.

## Considerazioni per l’utilizzo del vincolo Il più presto possibile

* Presto possibile è il vincolo predefinito se un progetto utilizza una modalità di programmazione a partire dalla data di inizio e se la data di inizio predefinita del sistema per una nuova attività è impostata su In base alla data pianificata del progetto.

* Se un progetto utilizza la modalità di programmazione Pianificazione dalla data di inizio e la data di inizio predefinita del sistema o del gruppo per una nuova attività è impostata su Oggi, il vincolo attività predefinito è Iniziare non prima di.

  Per informazioni su dove impostare il vincolo predefinito per una nuova attività, fare riferimento a [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Per informazioni su come aggiornare il vincolo attività in un&#39;attività, vedere [Aggiornare il vincolo attività di un&#39;attività](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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

## Differenza tra l&#39;orario disponibile più presto e il più presto possibile

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"]) </p>
-->

Il vincolo Primo tempo disponibile è diverso dal vincolo Il più presto possibile quando sono presenti tutti i seguenti criteri:

* Il progetto è pianificato dal completamento.
* Le attività del progetto hanno una relazione predecessore.
* L&#39;attività predecessore ha un vincolo di attività flessibile.

In questa situazione:

* **Primo orario disponibile:** L&#39;utilizzo del vincolo Primo orario disponibile sull&#39;attività successore dà priorità al vincolo flessibile del predecessore.

  Si supponga, ad esempio, che l&#39;attività A sia un predecessore dell&#39;attività B. L&#39;attività B ha il vincolo Primo tempo disponibile e l&#39;attività A ha il vincolo Il più tardi possibile. In questa situazione, l’attività è pianificata in prossimità del completamento del progetto.

* **Il più presto possibile:** In questo scenario, l&#39;utilizzo del vincolo Il più presto possibile sull&#39;attività successore conferisce la priorità all&#39;attività successore.

  Si supponga, ad esempio, che l&#39;attività A sia un predecessore dell&#39;attività B. L&#39;attività B ha il vincolo Il più presto possibile e l&#39;attività A ha il vincolo Il più tardi possibile. In questa situazione, l’attività viene pianificata il più vicino possibile all’inizio del progetto.
