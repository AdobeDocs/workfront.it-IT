---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: "Panoramica sul tipo di durata: semplice"
description: Il Tipo di Durata Semplice è un Tipo di Durata che puoi impostare per un’attività in Adobe Workfront. Per informazioni generali sui tipi di durata in Workfront, vedere Panoramica sulla durata e sul tipo di durata dell'attività.
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
source-git-commit: 1efd7c0270fe1396345cfa6e5499e8f998297d61
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Panoramica sul tipo di durata: semplice

Il Tipo di Durata Semplice è un Tipo di Durata che puoi impostare per un’attività in Adobe Workfront. Per informazioni generali sui tipi di durata in Workfront, vedi [Panoramica sulla durata e sul tipo di durata dell&#39;attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Panoramica del tipo di durata semplice

Il Workfront o un amministratore di gruppo può impostare il Tipo di durata predefinito del sistema o del gruppo come Semplice. In questo caso, tutte le nuove attività verranno create con questo Tipo di durata. Per informazioni sulla modifica delle preferenze di attività e problemi come parte delle preferenze di progetto a livello di sistema o di gruppo, consulta [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Quando un’attività ha un Tipo di durata semplice, si verificano gli eventi seguenti:

* I project manager possono modificare sia la durata che le ore pianificate di un&#39;attività quando modificano la modalità di distribuzione di tali ore tra gli assegnatari.

  Per informazioni, consulta [Aggiornare le ore e la durata pianificate di un&#39;attività con un tipo di durata semplice](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md).

  >[!IMPORTANT]
  >
  >Quando si crea un&#39;attività, vi si assegna il tipo di durata semplice e non si specifica una durata, Workfront calcola la durata dell&#39;attività in base alla quantità di ore pianificate specificate per l&#39;attività. Se si modifica manualmente la Durata di un&#39;attività di Durata semplice, Workfront non corrisponde più alla Durata in quanto presuppone che si desideri definirle manualmente.
  >
  >Workfront calcola la durata delle attività la cui durata non è stata modificata manualmente utilizzando la formula seguente:
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >L&#39;amministratore di Workfront definisce `Typical hours per work day` nell’area Preferenze progetto della Configurazione dell’istanza.

* La percentuale di allocazione è nascosta e le ore di allocazione sono disponibili per la modifica.
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
