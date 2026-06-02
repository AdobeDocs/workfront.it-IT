---
product-area: projects
navigation-topic: create-tasks
title: Panoramica sulla creazione di attività
description: È possibile creare le attività di un progetto solo dopo averlo creato.
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
TQID: https://experienceleague.adobe.com/-xOLBxAGitQAXXRxHSr6R9mv-2hfuLOq0VZKB2TzuqI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 9053a824ecec4feb35a612b26aebb91904ef2546
workflow-type: tm+mt
source-wordcount: 926
ht-degree: 0%

---

# Panoramica sulla creazione di attività

È possibile creare le attività di un progetto solo dopo averlo creato.

Ad esempio, dopo aver creato un progetto, è possibile aggiungere attività e modificarle per organizzare il piano del progetto. Per ulteriori informazioni sulla creazione di un progetto, vedere [Creare un progetto](../../../manage-work/projects/create-projects/create-project.md). Per informazioni sulla creazione di attività, vedere [Creare attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

In questo articolo vengono descritte considerazioni, limitazioni e valori predefiniti che vengono applicati durante la creazione di attività.

## Modalità di creazione delle attività in un progetto

È possibile creare attività in un progetto nei modi seguenti:

* Da zero, come descritto in [Creare attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).
* Copiare le attività nello stesso progetto o in un nuovo progetto o duplicare le attività nello stesso progetto, come descritto in [Copiare e duplicare le attività](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Spostare le attività da un progetto a un altro, come descritto in [Spostare le attività](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Limitazioni nella creazione di attività

Quando si dispone dell&#39;accesso e delle autorizzazioni corretti è possibile creare attività in un progetto. Tuttavia, di seguito sono riportati alcuni casi in cui potrebbe non essere possibile creare attività:

* L’amministratore di Adobe Workfront o un amministratore gruppo deve abilitare l’aggiunta di attività a un progetto che si trova nello stato Complete (Completato) o Dead (Inattivo) nell’area Project Preferences (Preferenze del progetto). Per informazioni sull&#39;impostazione delle preferenze di progetto, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Impossibile aggiungere attività a un progetto in attesa di approvazione.

## Il numero massimo di attività consentite in un progetto

Un progetto può contenere fino a 5.000 attività. Viene visualizzato un messaggio di avvertenza sul progetto quando ti avvicini al limite, quando hai raggiunto il limite e se tenti di superarlo.

A seconda del numero di attività nei progetti in cui è stato imposto questo limite, l’istanza di Workfront potrebbe consentire più di 5.000 attività in un singolo progetto.

Se si è in grado di includere più di 5.000 attività in un singolo progetto, tenere presente quanto segue:

* Il limite di attività per l’ambiente Workfront è impostato sul numero corrente di attività nel progetto più grande, più un ulteriore 10%.

  Ad esempio, se un progetto nell’istanza Workfront contiene 10.000 attività, il limite per ciascun progetto nell’istanza Workfront è di 11.000 attività.

* I progetti più piccoli migliorano le prestazioni e riducono al minimo le sfide di gestione che accompagnano i progetti di grandi dimensioni.

## Valori predefiniti attività quando si aggiungono attività a un progetto

Esistono due tipi di informazioni predefinite che Workfront aggiorna automaticamente per le attività quando le crei:

* Informazioni predefinite a livello di sistema

  L&#39;amministratore di Workfront o un amministratore di gruppo stabilisce le impostazioni predefinite a livello di sistema per le attività nell&#39;area Attività e problemi di Preferenze progetto. Per informazioni sulle preferenze per attività e problemi, vedere [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) o [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

* Informazioni predefinite a livello di progetto

  Il resto di questa sezione descrive le impostazioni predefinite a livello di progetto che il project manager può definire per tutte le nuove attività aggiunte a un progetto

Quando si aggiunge un&#39;attività a un progetto, a seconda della configurazione del progetto, Workfront potrebbe allegare automaticamente un processo di approvazione o moduli personalizzati all&#39;attività.

Per informazioni sulla configurazione di un progetto per aggiungerli per impostazione predefinita, consulta la sezione &quot;Attività&quot; nell&#39;articolo [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

Quando definisci le informazioni predefinite da associare alle attività aggiunte a un progetto a livello di progetto, considera quanto segue:

* Per definire le impostazioni predefinite per il processo di approvazione delle attività e i moduli personalizzati è necessario disporre delle autorizzazioni Gestione per il progetto.
* Tutte le nuove attività vengono create con il processo di approvazione e i moduli personalizzati definiti durante la modifica del progetto.
* È possibile modificare queste impostazioni predefinite quando si aggiungono attività utilizzando la casella Modifica attività, ma non quando si aggiungono attività nella modifica in linea.
* È possibile definire il processo di approvazione e i moduli personalizzati per le attività in un modello.

   * Quando un progetto viene creato da questo modello, il processo di approvazione e i moduli personalizzati vengono applicati automaticamente al progetto.
   * Quando un modello viene allegato a un progetto esistente, il progetto mantiene il processo di approvazione dell’attività originale e le impostazioni dei moduli personalizzati, se definiti. Se non sono definite, le impostazioni del modello diventano le impostazioni del progetto.
   * Quando un modello viene allegato a un progetto esistente, le attività aggiunte al progetto dal modello mantengono le impostazioni del processo di approvazione e dei moduli personalizzati disponibili nel modello, indipendentemente dalle impostazioni delle attività nel progetto.

  Per informazioni su come allegare un modello a un progetto, vedere [Allegare un modello a un progetto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Quando si copia il progetto, le impostazioni predefinite dell&#39;attività vengono trasferite al nuovo progetto.

  Per informazioni sulla copia di un progetto, vedere [Copiare un progetto](../../../manage-work/projects/manage-projects/copy-project.md).

* Quando si copiano attività da un progetto a un altro e il progetto di destinazione ha impostazioni predefinite diverse per le attività, le attività copiate mantengono le impostazioni predefinite del progetto originale, a meno che non vengano cancellate durante la copia.
* Quando si duplica un&#39;attività sullo stesso progetto, i moduli personalizzati e il processo di approvazione vengono trasferiti all&#39;attività duplicata.

  Per informazioni sulla copia e la duplicazione delle attività, vedere [Copiare e duplicare le attività](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

* Quando si sposta l&#39;attività in un altro progetto, le impostazioni predefinite dell&#39;attività vengono salvate nelle attività del progetto originale, indipendentemente dalle impostazioni predefinite dell&#39;attività nel nuovo progetto.

  Per informazioni sullo spostamento delle attività, vedere [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md).

* Quando l’organizzazione utilizza sia l’archiviazione cloud legacy di Workfront che Adobe, non è possibile spostare o copiare attività tra progetti che utilizzano tipi di archiviazione diversi.

  Per informazioni, consulta [Panoramica sulla gestione dei documenti per progetti e oggetti correlati](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).
