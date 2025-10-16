---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Panoramica del tipo di durata: semplice'
description: Il Tipo di Durata Semplice è un Tipo di Durata che puoi impostare per un’attività in Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Panoramica sul tipo di durata: semplice

<!-- Audited: 5/2025 -->

Il tipo di durata semplice è un tipo di durata che è possibile impostare per un&#39;attività in Adobe Workfront. Per ulteriori informazioni sui tipi di durata in Workfront, vedere [Panoramica sulla durata dell&#39;attività e sul tipo di durata](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Panoramica del tipo di durata semplice

L&#39;amministratore del Workfront o del gruppo può impostare come Semplice il tipo di durata predefinito del sistema o del gruppo. In questo caso, tutte le nuove attività verranno create con questo tipo di durata.

Per informazioni sulla modifica delle preferenze di attività e problemi come parte delle preferenze di progetto a livello di sistema o di gruppo, consulta [Configurare le preferenze di problema e attività a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Quando un&#39;attività ha un tipo di durata semplice si verificano gli eventi seguenti:

* I project manager possono modificare sia la durata che le ore pianificate di un&#39;attività quando modificano la modalità di distribuzione di tali ore tra gli assegnatari.

  Per informazioni, vedere [Aggiornare le ore e la durata pianificate di un&#39;attività con un tipo di durata semplice](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md).

  >[!IMPORTANT]
  >
  >Quando si crea un&#39;attività assegnandole il tipo di durata Semplice ma non si specifica una Durata, Workfront calcola la durata dell&#39;attività in base alla quantità di ore pianificate specificate per l&#39;attività. Se si modifica manualmente la durata di un&#39;attività di durata semplice, Workfront non corrisponde più alla durata delle ore pianificate, poiché si presuppone che si desideri definirle manualmente.
  >
  >Workfront calcola la durata delle attività la cui durata non è stata modificata manualmente utilizzando la formula seguente:
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >L&#39;amministratore di Workfront definisce `Typical hours per work day` nell&#39;area Preferenze progetto della Configurazione dell&#39;istanza.

* La percentuale di allocazione è nascosta, ma è possibile modificare le ore di allocazione.
* Per tutti i nuovi clienti, il Tipo di durata a livello di sistema è impostato su Semplice.

## Impostare il tipo di durata di un&#39;attività su Semplice

Per informazioni sulla modifica del tipo di durata di un&#39;attività, vedere [Aggiornare il tipo di durata di un&#39;attività](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Simple</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong><strong>.</strong></li>
</ol>
-->
