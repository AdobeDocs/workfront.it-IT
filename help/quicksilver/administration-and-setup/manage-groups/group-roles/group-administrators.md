---
title: Amministratori di gruppo
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: Gli amministratori di Adobe Workfront in una grande organizzazione con molti dipartimenti potrebbero non voler gestire tutti i dipartimenti e i gruppi dell'organizzazione all'interno di tali dipartimenti. Al contrario, possono creare un gruppo per ogni reparto e sottogruppi all'interno del gruppo, ciascuno gestito da un amministratore del gruppo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: 03667fbdd1b0d68b9ad2d2db4a1ed85b8136062b
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 0%

---

# Amministratori di gruppo

Gli amministratori di Adobe Workfront in una grande organizzazione con molti dipartimenti potrebbero non voler gestire tutti i dipartimenti e i gruppi dell&#39;organizzazione all&#39;interno di tali dipartimenti. Al contrario, possono creare un gruppo per ogni reparto e sottogruppi all&#39;interno del gruppo, ciascuno gestito da un amministratore del gruppo.

Un amministratore di gruppo può gestire le esigenze di un gruppo, ad esempio l’appartenenza utente, i modelli di layout, i dati personalizzati, gli stati e le preferenze.

In un gruppo possono esistere fino a 14 livelli di sottogruppi.

>[!NOTE]
>
>Tutti gli amministratori di gruppo nella gerarchia sopra un sottogruppo dispongono dei diritti amministrativi per gestire tale sottogruppo.

Per informazioni sulla creazione e la gestione dei gruppi, consulta [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) e [Gestire un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). Vedi anche [Panoramica sui sottogruppi](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Designazione degli amministratori dei gruppi

Per ogni gruppo di livello superiore deve essere presente almeno un amministratore di gruppo. Un amministratore Workfront o un amministratore di un gruppo può assegnare amministratori di gruppo ai sottogruppi del gruppo, ma questo non è necessario. Per ulteriori informazioni, consulta [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Gli amministratori di Workfront possono effettuare le seguenti operazioni prima di designare gli utenti come amministratori di gruppo:

* Prendi nota del numero corrente di amministratori Workfront nel tuo sistema.
* Prendi nota del numero di gruppi presenti nel sistema.
* Determina se puoi modificare il livello di accesso di alcuni degli amministratori di Workfront e designarli come amministratori di gruppo.

   Per ulteriori informazioni sulle funzionalità degli amministratori dei gruppi, consulta [Attività eseguite dagli amministratori del gruppo](#tasks-done-by-group-administrators).

* Stabilisci se desideri che gli amministratori dei gruppi siano in grado di accedere come altri utenti o di reimpostare le password per gli utenti nei gruppi che amministri. È necessario un accesso aggiuntivo per eseguire queste attività, come spiegato in [Accesso necessario per gli amministratori dei gruppi](#access-needed-for-group-administrators).
* Per una migliore gestione degli utenti, è consigliabile assegnare gruppi o sottogruppi invece che utenti ai seguenti oggetti:

   * Modelli di layout
   * Schedule
   * Profili schede orario

## Accesso necessario per gli amministratori dei gruppi {#access-needed-for-group-administrators}

Ogni amministratore del gruppo deve disporre di una licenza Plan.

È consigliabile che gli amministratori di gruppo abbiano accesso in Modifica agli utenti in modo che possano eseguire le seguenti attività:

* Accedi come altri utenti nei gruppi e sottogruppi che gestiscono.
* Reimposta la password di un altro utente nei gruppi gestiti.

>[!IMPORTANT]
>
>Gli amministratori dei gruppi devono avere un accesso più elevato rispetto a quelli che gestiscono; in caso contrario, non potranno visualizzare o modificare livelli di accesso inferiori.
>Per istruzioni su come concedere questo accesso, vedi [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Per un amministratore del gruppo che deve assegnare profili della scheda attività agli utenti dei propri gruppi e sottogruppi, si consiglia inoltre l&#39;accesso amministrativo alle schede attività e alle ore. Per istruzioni su come concedere questo accesso, vedi [Consentire agli utenti l&#39;accesso amministrativo a determinate aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Attività eseguite dagli amministratori del gruppo {#tasks-done-by-group-administrators}

In qualità di amministratore di gruppo, puoi eseguire le attività riportate di seguito per gestire i gruppi che sovrascrivi. Alcune di queste sono le stesse capacità offerte a un amministratore Workfront.

* [Gestire i membri del gruppo](#manage-group-members)
* [Gestire gli oggetti gruppo](#manage-group-objects)
* [Gestione delle preferenze e degli strumenti del gruppo](#manage-group-preferences-and-tools)

### Gestire i membri del gruppo {#manage-group-members}

* Crea, modifica ed elimina sottogruppi all’interno dei gruppi e sottogruppi gestiti. Per istruzioni, consulta [Creare un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* Aggiungi tutti gli utenti per i quali hai accesso a Modifica ai tuoi gruppi e sottogruppi. Oppure puoi aggiungere utenti a gruppi e sottogruppi modificando i loro profili.

   Puoi anche aggiornare i campi nel profilo di un membro del gruppo se disponi dell’autorizzazione Amministratore utente (Utenti del gruppo) abilitata nel livello di accesso.

   Per ulteriori informazioni, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   >[!NOTE]
   >
   >Gli amministratori di Workfront possono ignorare le modifiche apportate alle appartenenze di gruppo da un amministratore di gruppo.

* Reimpostare le password per gli utenti membri dei gruppi gestiti. Per ulteriori informazioni, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* Accedi come utenti membri dei gruppi gestiti. Per ulteriori informazioni, consulta [Accedi come altro utente](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* Visualizzare il numero di licenze disponibili per il gruppo e i sottogruppi sottostanti. Per ulteriori informazioni, consulta [Gestione delle licenze disponibili nel sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### Gestire gli oggetti gruppo {#manage-group-objects}

* Creare modelli di layout a livello di gruppo e associarli ai gruppi e ai sottogruppi gestiti. Per ulteriori informazioni, consulta [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* Creare profili a livello di gruppo, associarli a utenti e gruppi gestiti e generare manualmente fogli presenze. Per ulteriori informazioni, consulta [Creare, modificare e assegnare profili della scheda attività](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* Senza l&#39;accesso amministrativo ai processi di approvazione, crea e modifica i processi di approvazione per i gruppi e i sottogruppi gestiti. Per ulteriori informazioni, consulta [Creazione di un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   Per informazioni sull&#39;accesso amministrativo ai processi di approvazione, vedi [Consentire agli utenti l&#39;accesso amministrativo a determinate aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Crea pianificazioni e associale a un gruppo gestito. Per ulteriori informazioni, consulta [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* Gestisci un team assegnato a un gruppo gestito senza essere membro del team. Inoltre, crea un rapporto del team basato sul campo Gruppo per identificare a quale gruppo è assegnato un determinato team. Per ulteriori informazioni, consulta [Creare un team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* Ripristinare un progetto associato a un gruppo gestito, insieme a tutte le attività, i problemi o i documenti associati al progetto. Per ulteriori informazioni, consulta [Ripristina elementi eliminati](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### Gestione delle preferenze e degli strumenti del gruppo {#manage-group-preferences-and-tools}

* Quando si sblocca la preferenza di un progetto, di un&#39;attività o di un problema, oppure la preferenza relativa a fogli presenze e ore per i gruppi in tutto il sistema, modificare tale preferenza per i gruppi gestiti. Queste preferenze influiscono sul comportamento del progetto, delle attività e dei problemi. Per ulteriori informazioni, consulta quanto segue:

   * [Configurare le preferenze di progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* Creare e modificare gli stati dei gruppi gestiti. Per ulteriori informazioni, consulta [Creare o modificare uno stato di gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Configura una notifica evento per i gruppi gestiti. Puoi eseguire questa operazione solo dopo che un amministratore di Workfront sblocca la possibilità di configurare le notifiche degli eventi per i gruppi all’esterno del sistema. Per ulteriori informazioni, consulta [Visualizzare e configurare le notifiche evento per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
