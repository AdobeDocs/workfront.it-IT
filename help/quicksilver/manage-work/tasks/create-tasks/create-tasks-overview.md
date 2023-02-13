---
product-area: projects
navigation-topic: create-tasks
title: Panoramica sulla creazione di attività
description: È possibile creare attività in un progetto solo dopo la creazione del progetto.
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# Panoramica sulla creazione di attività

È possibile creare attività in un progetto solo dopo la creazione del progetto.

Ad esempio, dopo aver creato un progetto, è possibile aggiungere attività e modificarle per organizzare il piano di progetto. Per ulteriori informazioni sulla creazione di un progetto, consulta [Creare un progetto](../../../manage-work/projects/create-projects/create-project.md). Per informazioni sulla creazione delle attività, consulta [Creazione di attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Questo articolo descrive considerazioni, limitazioni e impostazioni predefinite applicabili durante la creazione di attività.

## Modalità di creazione delle attività in un progetto

È possibile creare attività su un progetto nei modi seguenti:

* Da zero, come descritto in [Creazione di attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).
* Copiare le attività nello stesso progetto o in un nuovo progetto o attività duplicate nello stesso progetto, come descritto in [Copia e duplica le attività](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Spostare le attività da un progetto a un altro, come descritto in [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Limitazioni nella creazione di attività

Se disponi dell&#39;accesso e delle autorizzazioni corrette, puoi creare attività su un progetto. Tuttavia, i seguenti casi non consentono la creazione di attività:

* L’amministratore di Adobe Workfront o un amministratore di gruppo deve abilitare l’aggiunta di attività a un progetto con stato Completa o Morto nell’area Preferenze progetto. Per informazioni sull&#39;impostazione delle preferenze del progetto, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Impossibile aggiungere attività a un progetto in sospeso.

## Numero massimo di attività consentite per un progetto

Un progetto può contenere fino a 5.000 attività. Nel progetto viene visualizzato un messaggio di avviso quando si sta avvicinando il limite, quando si è raggiunto il limite e se si tenta di superarlo.

A seconda del numero di attività nei progetti al momento dell’imposizione di questa limitazione, l’istanza Workfront potrebbe consentire più di 5.000 attività in un singolo progetto.

Se puoi includere più di 5.000 attività in un singolo progetto, tieni presente quanto segue:

* Il limite di attività per l’ambiente Workfront è impostato sul numero corrente di attività nel progetto più grande, più un ulteriore 10%.

   Ad esempio, se un progetto nell’istanza di Workfront contiene 10.000 attività, il limite per ogni progetto nell’istanza di Workfront è di 11.000 attività.

* I progetti più piccoli migliorano le prestazioni e riducono al minimo le sfide di gestione che accompagnano i grandi progetti.

## Valori predefiniti delle attività quando si aggiungono attività a un progetto

Esistono due tipi di informazioni predefinite che Workfront aggiorna automaticamente per le attività quando le crei:

* Informazioni predefinite a livello di sistema

   L’amministratore di Workfront o un amministratore di gruppo stabilisce le impostazioni predefinite a livello di sistema per le attività nell’area Attività e problemi di Preferenze progetto. Per informazioni sulle preferenze relative a attività e problemi, consulta [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) o [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

* Informazioni predefinite a livello di progetto

   Il resto di questa sezione descrive le impostazioni predefinite a livello di progetto che, in qualità di project manager, puoi definire per tutte le nuove attività aggiunte a un progetto

Quando si aggiunge un&#39;attività a un progetto, a seconda della configurazione del progetto, Workfront potrebbe allegare automaticamente all&#39;attività un processo di approvazione o moduli personalizzati.

Per informazioni sulla configurazione di un progetto per aggiungerli per impostazione predefinita, consulta la sezione &quot;Attività&quot; nella sezione [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md) articolo.

Quando definisci le informazioni predefinite da associare alle attività aggiunte a un progetto a livello di progetto, considera quanto segue:

* Per definire le impostazioni predefinite per il processo di approvazione delle attività e i moduli personalizzati, è necessario disporre delle autorizzazioni di gestione per il progetto.
* Tutte le nuove attività vengono create con il processo di approvazione e i moduli personalizzati definiti durante la modifica del progetto.
* È possibile modificare queste impostazioni predefinite quando si aggiungono attività utilizzando la casella Modifica attività, ma non quando si aggiungono attività in modifica in linea.
* È possibile definire il processo di approvazione e i moduli personalizzati per le attività in un modello.

   * Quando un progetto viene creato a partire da questo modello, il processo di approvazione e i moduli personalizzati vengono applicati automaticamente al progetto.
   * Quando un modello viene allegato a un progetto esistente, il progetto conserva il processo di approvazione dell’attività originale e le impostazioni dei moduli personalizzati, se definiti. Se non sono definite, le impostazioni del modello diventano le impostazioni del progetto.
   * Quando un modello viene allegato a un progetto esistente, le attività aggiunte al progetto dal modello conservano il processo di approvazione e le impostazioni dei moduli personalizzati presenti nel modello, indipendentemente dalle impostazioni delle attività del progetto.

   Per informazioni sull&#39;associazione di un modello a un progetto, consulta [Allegare un modello a un progetto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Quando copi il progetto, le impostazioni predefinite dell’attività vengono trasferite al nuovo progetto.

   Per informazioni sulla copia di un progetto, consulta [Copiare un progetto](../../../manage-work/projects/manage-projects/copy-project.md).

* Quando si copiano le attività da un progetto all&#39;altro e il progetto di destinazione dispone di impostazioni predefinite diverse per le attività, le attività copiate conservano le impostazioni predefinite del progetto originale, a meno che non vengano cancellate nel processo di copia.
* Quando si duplica un&#39;attività sullo stesso progetto, i moduli personalizzati e il processo di approvazione vengono trasferiti all&#39;attività duplicata.

   Per informazioni sulla copia e la duplicazione delle attività, consulta [ [Copia e duplica le attività](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

* Quando si sposta l&#39;attività in un altro progetto, le impostazioni predefinite vengono salvate sulle attività del progetto originale, indipendentemente dalle impostazioni predefinite dell&#39;attività del nuovo progetto.

   Per informazioni sullo spostamento delle attività, consulta [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md).
