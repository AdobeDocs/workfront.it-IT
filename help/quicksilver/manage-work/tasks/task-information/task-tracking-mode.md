---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica sulla modalità di monitoraggio attività
description: È possibile regolare l'impostazione della modalità Tracciamento di un'attività durante la creazione o la modifica di un'attività per controllare come e quando vengono visualizzati gli indicatori di stato di avanzamento di un'attività. Adobe Workfront mostra i flag di stato di avanzamento quando configuri alcune impostazioni per il tracciamento dell’avanzamento delle attività.
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: d2836549ee3c615201ce5f3454258e9af31efa42
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 2%

---

# Panoramica sulla modalità di monitoraggio attività

<!-- Audited: 01/2024 -->

È possibile regolare l&#39;impostazione della modalità Tracciamento di un&#39;attività durante la creazione o la modifica di un&#39;attività per controllare come e quando vengono visualizzati gli indicatori di stato di avanzamento di un&#39;attività. Adobe Workfront mostra i flag di stato di avanzamento quando configuri alcune impostazioni per il tracciamento dell’avanzamento delle attività.

Per ulteriori informazioni sullo stato di avanzamento delle attività, vedere [Panoramica sullo stato di avanzamento delle attività](../../../manage-work/tasks/task-information/task-progress-status.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set Tracking Mode for tasks</h2>
<p>(NOTE: drafted, because we created a new article and linked it below. Left this article as a "Overview" article only.) </p>
<p>To set the tracking mode:</p>
<ol>
<li value="1">Go to the task you want to set the tracking mode for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png">next to the name of the task, then click&nbsp;<strong>Edit</strong>.</p> <p>The Edit Task dialog box opens. </p> </li>
<li value="3"> <p>In the&nbsp;<strong>Settings</strong> section, use the&nbsp;<strong>Tracking Mode</strong> drop-down menu to select the Tracking Mode for the task.</p> <p>For more information about the tracking mode options, see the <a href="#tracking-mode-options" class="MCXref xref" xrefformat="{para}">Tracking Mode options</a> section in this article. </p> </li>
<li value="4">Click&nbsp;<strong>Save Changes.</strong></li>
</ol>
</div>
-->

## Opzioni della modalità di tracciamento {#tracking-mode-options}

In qualità di proprietario di un&#39;attività o di project manager, è possibile selezionare il modo in cui Workfront indica lo stato di avanzamento di ogni attività. Per informazioni su come impostare la modalità di verifica per le attività, vedere [Impostare la modalità di verifica per le attività](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

Puoi scegliere tra le seguenti opzioni:

* [L&#39;Utente Deve Aggiornare](#user-must-update)
* [Presupponi puntuale](#assume-on-time)
* [Ignora avvisi di ritardo](#ignore-late-warnings)
* [Completamento automatico](#auto-complete)
* [Predecessore](#predecessor)

### Utente deve Aggiornare {#user-must-update}

Quando questa opzione è selezionata, Workfront utilizza la percentuale di completamento e le ore effettive registrate dell&#39;attività per determinare lo stato di avanzamento dell&#39;attività. Questa è l&#39;opzione predefinita.

### presume nei tempi {#assume-on-time}

Workfront presuppone che un&#39;attività verrà completata in tempo, indipendentemente dallo stato di completamento corrente. Se l&#39;attività non viene completata in tempo (alla data di completamento pianificata), Workfront presuppone automaticamente una data di completamento pianificata del giorno lavorativo successivo. È comunque necessario indicare quando l&#39;attività viene completata. Utilizza questa opzione quando gli utenti non aggiorneranno regolarmente le loro attività.

### Ignora Avvertimenti di Ritardo {#ignore-late-warnings}

Lo stato di avanzamento di un&#39;attività è Attivo fino a quando non è in ritardo. Se ad esempio si pianifica un&#39;attività che richiede 10 giorni e il giorno in cui deve essere completata, l&#39;attività mostra una percentuale di completamento del 60%, Workfront aggiorna la data di completamento prevista aggiungendo quattro giorni e lo stato di avanzamento dell&#39;attività diventa in ritardo.

### Auto completamento {#auto-complete}

Workfront presuppone che le attività saranno completate come programmato e le contrassegna come completate alle rispettive Date di completamento previste o in scadenza. Fino ad allora, Workfront utilizza la percentuale di completamento e le ore effettive registrate per determinare lo stato di avanzamento. Tuttavia, indipendentemente dallo stato di avanzamento prima della data di completamento pianificata, Workfront contrassegna comunque l’attività come completata.

Esistono le seguenti eccezioni:

* Se l&#39;attività ha predecessori incompleti, non verrà completata automaticamente fino al completamento di tutti i predecessori. I Predecessori devono essere fatti rispettare.
* Se l&#39;attività ha un vincolo Data fissa, l&#39;attività viene sempre completata alla Data di completamento pianificata, indipendentemente dal fatto che i predecessori siano stati completati.

>[!IMPORTANT]
>
>Se si seleziona l&#39;opzione per il completamento automatico delle attività, l&#39;attività viene contrassegnata come completata quando viene ricalcolata l&#39;ora del progetto. Se il tipo di aggiornamento del progetto è impostato su Automatico o Automatico e su Modifica, la sequenza temporale del progetto viene calcolata quotidianamente. Per informazioni sui ricalcoli della sequenza temporale nei progetti, vedere [Ricalcolare le sequenze temporali dei progetti](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).
>
>L&#39;ora della data di completamento effettiva è la mezzanotte del giorno in cui la sequenza temporale viene calcolata automaticamente. L’ora utilizzata per generare questa marca temporale è il fuso orario del sistema definito dall’amministratore di Workfront nella sezione Informazioni cliente di Configurazione. Per informazioni sull&#39;impostazione del fuso orario del sistema, vedere [Configurare le informazioni di base per il sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Predecessore {#predecessor}

Workfront stima la data di completamento prevista di un&#39;attività in base alla relazione predecessore. Lo stato di avanzamento di un&#39;attività viene determinato in base a questa stima. Ad esempio, l&#39;attività B ha una durata di 1 giorno ed è programmata per essere completata due giorni dopo il predecessore, l&#39;attività A, che dovrebbe richiedere cinque giorni. Un utente aggiorna quindi l’Attività B al 50% completato, ma il predecessore, l’Attività A, non è ancora iniziato. Workfront pianifica il completamento dell&#39;attività B dipendente sei giorni dopo la data di inizio dell&#39;attività predecessore, consentendo 5 giorni per l&#39;attività A e 1 giorno per l&#39;attività B.
