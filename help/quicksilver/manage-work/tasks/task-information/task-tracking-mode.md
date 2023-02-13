---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica sulla modalità di tracciamento delle attività
description: È possibile regolare l'impostazione della modalità di tracciamento di un'attività durante la creazione o la modifica di un'attività per controllare come e quando vengono visualizzati gli indicatori di stato di avanzamento di un'attività. Adobe Workfront visualizza i flag Stato di avanzamento quando si configurano alcune impostazioni per tenere traccia dell'avanzamento delle attività.
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 3%

---

# Panoramica sulla modalità di tracciamento delle attività

È possibile regolare l&#39;impostazione della modalità di tracciamento di un&#39;attività durante la creazione o la modifica di un&#39;attività per controllare come e quando vengono visualizzati gli indicatori di stato di avanzamento di un&#39;attività. Adobe Workfront visualizza i flag Stato di avanzamento quando si configurano alcune impostazioni per tenere traccia dell&#39;avanzamento delle attività.

Per ulteriori informazioni sullo stato di avanzamento delle attività, vedere [Panoramica sullo stato dell&#39;avanzamento dell&#39;attività](../../../manage-work/tasks/task-information/task-progress-status.md).

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

In qualità di proprietario di un&#39;attività o di project manager, è possibile selezionare il modo in cui Workfront indica lo stato di avanzamento di ogni attività. Per informazioni su come impostare la modalità di tracciamento delle attività, consulta [Impostare la modalità di tracciamento per le attività](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

Puoi scegliere tra le seguenti opzioni:

* [Utente deve Aggiornare](#user-must-update)
* [presume nei tempi](#assume-on-time)
* [Ignora Avvertimenti di Ritardo](#ignore-late-warnings)
* [Auto completamento](#auto-complete)
* [Predecessore](#predecessor)

### Utente deve Aggiornare {#user-must-update}

Quando questa opzione è selezionata, Workfront utilizza la percentuale di completamento e le ore effettive dell&#39;attività registrate per determinare lo stato di avanzamento dell&#39;attività. Questa è l’opzione predefinita.

### presume nei tempi {#assume-on-time}

Workfront presuppone che un&#39;attività venga completata in tempo, indipendentemente dallo stato di completamento corrente. In caso contrario, Workfront assume automaticamente una data di completamento pianificata del giorno lavorativo successivo. È comunque necessario indicare quando l&#39;attività viene completata. Utilizza questa opzione quando gli utenti non aggiornano regolarmente le attività.

### Ignora Avvertimenti di Ritardo {#ignore-late-warnings}

Lo stato di avanzamento di un&#39;attività sarà attivato in tempo finché non diventa in ritardo. Ad esempio, se si pianifica un&#39;attività per 10 giorni e il giorno in cui deve essere completata, l&#39;attività mostra una percentuale di completamento del 60%, Workfront aggiorna la data di completamento prevista aggiungendo quattro giorni e lo stato di avanzamento dell&#39;attività diventa in ritardo.

### Auto completamento {#auto-complete}

Workfront presuppone che le attività vengano completate come pianificato e le contrassegna come completate in base alle rispettive date di completamento previste o previste. Fino ad allora, Workfront utilizza Percentuale di completamento e Ore effettive registrate per determinare lo stato di avanzamento. Tuttavia, indipendentemente dallo stato di avanzamento prima della data di completamento pianificata, Workfront contrassegna ancora l’attività completata.

Esistono le seguenti eccezioni:

* Se l&#39;attività ha predecessori incompleti, non verrà completata automaticamente fino al completamento di tutti i predecessori.
* Se l&#39;attività presenta un vincolo di data fissa, l&#39;attività viene sempre completata alla data di completamento pianificata, indipendentemente dal completamento dei predecessori.

>[!IMPORTANT]
>
>Quando si seleziona questa opzione per completare automaticamente le attività, l&#39;attività viene completata quando viene ricalcolata l&#39;ora del progetto. Se Tipo di aggiornamento del progetto è impostato su Automatico o Automatico e su Modifica, la timeline del progetto viene calcolata quotidianamente. Per informazioni sul ricalcolo temporale dei progetti, consulta [Ricalcolare le timeline dei progetti](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).
>
>L&#39;ora della Data di completamento effettiva è la mezzanotte del giorno in cui la timeline viene calcolata automaticamente. L&#39;ora utilizzata per generare questa marca temporale è il fuso orario del sistema, come definito dall&#39;amministratore Workfront nella sezione Informazioni cliente di Configurazione. Per informazioni sull&#39;impostazione del fuso orario del sistema, vedi [Configurare le informazioni di base per il sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Predecessore {#predecessor}

Workfront stima la data di completamento prevista di un&#39;attività in base alla relazione precedente. Lo stato di avanzamento di un&#39;attività viene determinato in base a questa stima. Ad esempio, l’attività B ha una durata di 1 giorno e deve essere completata due giorni dopo il suo predecessore, l’attività A, che dovrebbe richiedere cinque giorni. Un utente aggiorna quindi l’attività B al 50% completata, ma il predecessore, l’attività A, non è ancora iniziato. Workfront determina il completamento dell&#39;attività dipendente B sei giorni dopo la data di inizio dell&#39;attività predecessore, consentendo 5 giorni per l&#39;attività A e 1 giorno per l&#39;attività B.
