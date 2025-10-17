---
title: Amministratori di gruppi
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: Gli amministratori di Adobe Workfront in un’organizzazione di grandi dimensioni con molti reparti potrebbero non voler gestire tutti i reparti e i gruppi dell’organizzazione all’interno di tali reparti. È invece possibile creare un gruppo per ogni reparto e sottogruppi all'interno del gruppo, ciascuno gestito da un amministratore di gruppo.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 1%

---

# Amministratori di gruppi

<!-- Audited: 12/2023 -->

Gli amministratori di Adobe Workfront in un’organizzazione di grandi dimensioni con molti reparti potrebbero non voler gestire tutti i reparti e i gruppi dell’organizzazione all’interno di tali reparti. È invece possibile creare un gruppo per ogni reparto e sottogruppi all&#39;interno del gruppo, ciascuno gestito da un amministratore di gruppo.

Un amministratore di gruppo può gestire le esigenze di un gruppo, ad esempio l’iscrizione degli utenti, i modelli di layout, i dati personalizzati, gli stati e le preferenze.

In un gruppo possono esistere fino a 14 livelli di sottogruppi.

>[!NOTE]
>
>Tutti gli amministratori di gruppi nella gerarchia sopra un sottogruppo dispongono di diritti amministrativi per gestire tale sottogruppo.

Per informazioni sulla creazione e la gestione dei gruppi, vedere [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) e [Gestire un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). Vedi anche [Panoramica sui sottogruppi](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Designazione degli amministratori di gruppi

Ogni gruppo di primo livello deve disporre di almeno un amministratore di gruppo. Un amministratore di Workfront o un amministratore di un gruppo può assegnare amministratori di gruppi ai sottogruppi del gruppo, ma questo non è obbligatorio. Per ulteriori informazioni, vedere [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Se sei un amministratore di Workfront, ti consigliamo di effettuare le seguenti operazioni prima di designare gli utenti come amministratori di gruppi:

* Prendere nota del numero corrente di amministratori di Workfront nel sistema.
* Prendi nota del numero di gruppi che hai nel sistema.
* Determina se è possibile modificare il livello di accesso di alcuni amministratori di Workfront e designarli come amministratori di gruppi.

  Per ulteriori informazioni sulle funzionalità degli amministratori di gruppi, vedere [Attività eseguite dagli amministratori di gruppi](#tasks-done-by-group-administrators) in questo articolo.

* Determinare se si desidera che gli amministratori di gruppi possano accedere come altri utenti o reimpostare le password per gli utenti dei gruppi amministrati. Per eseguire queste attività è necessario un accesso aggiuntivo, come spiegato di seguito in [Accesso necessario per gli amministratori di gruppi](#access-needed-for-group-administrators).
* Per una migliore gestione degli utenti, è consigliabile assegnare gruppi o sottogruppi anziché utenti ai seguenti oggetti:

   * Modelli di layout
   * Schedule
   * Profili schede orario

## Accesso necessario per gli amministratori di gruppi {#access-needed-for-group-administrators}

Ogni amministratore di gruppo deve disporre di

* Una licenza Pianificazione nel modello di determinazione prezzi e imballaggio corrente
* Una licenza Standard nel nuovo modello di prezzo e imballaggio

È consigliabile che gli amministratori dei gruppi abbiano accesso in Modifica per gli utenti in modo che possano eseguire le seguenti attività:

* Accedere come altri utenti nei gruppi e nei sottogruppi che gestiscono.
* Reimpostare la password di un altro utente nei gruppi da esso gestiti.

>[!IMPORTANT]
>
>Gli amministratori dei gruppi devono disporre di un accesso più elevato rispetto a quelli che gestiscono; in caso contrario, non potranno visualizzare o modificare livelli di accesso inferiori.
>>Per istruzioni sulla concessione dell&#39;accesso, vedere [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Per un amministratore di gruppo che deve assegnare profili della scheda orario agli utenti nei loro gruppi e sottogruppi, consigliamo anche l’accesso Amministrativo alle schede orario e alle ore. Per istruzioni sulla concessione di questo accesso, vedere [Concedere agli utenti l&#39;accesso amministrativo ad alcune aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Attività eseguite dagli amministratori di gruppi {#tasks-done-by-group-administrators}

In qualità di amministratore di gruppo, puoi eseguire le attività descritte di seguito per gestire i gruppi di cui hai la supervisione. Alcune di queste sono le stesse funzionalità offerte a un amministratore Workfront.

>[!NOTE]
>
>Nel nuovo modello di determinazione prezzi e imballaggio è necessario disporre di un piano Prime o superiore per eseguire le operazioni seguenti:
>
> * Creare notifiche di eventi di gruppo
> * Configurare le preferenze di progetto del gruppo
> * Configurare le preferenze per attività e problemi del gruppo
> * Sblocca configurazione preferenze sottogruppo
> * Raggruppa le preferenze di orario e scheda orario
> * Sblocca le preferenze di ora e scheda orario

### Gestisci membri del gruppo {#manage-group-members}

* Creare, modificare ed eliminare i sottogruppi all’interno dei gruppi e dei sottogruppi gestiti. Per istruzioni, vedere [Creare un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* Aggiungere ai gruppi e ai sottogruppi tutti gli utenti per i quali si dispone dell&#39;accesso di modifica. In alternativa, puoi aggiungere utenti a gruppi e sottogruppi modificandone i profili.

  È inoltre possibile aggiornare i campi nel profilo di un membro del gruppo se nel proprio livello di accesso è abilitata l’autorizzazione Amministratore utenti (Utenti gruppo).

  Per ulteriori informazioni, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >Gli amministratori di Workfront possono ignorare le modifiche alle appartenenze ai gruppi apportate da un amministratore.

* Reimpostare le password per gli utenti membri dei gruppi gestiti. Per ulteriori informazioni, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* Accedi come utenti membri dei gruppi che gestisci. Per ulteriori informazioni, vedere [Accedere come altro utente](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* Visualizzare il numero di licenze disponibili per il gruppo e i sottogruppi sottostanti. Per ulteriori informazioni, consulta [Gestire le licenze disponibili nel sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### Gestisci oggetti gruppo {#manage-group-objects}

* Creare modelli di layout a livello di gruppo e associarli ai gruppi e ai sottogruppi gestiti. Per ulteriori informazioni, vedere [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* Crea profili di schede orario a livello di gruppo, associali a utenti e gruppi gestiti e genera manualmente le schede orario. Per ulteriori informazioni, vedere [Creare, modificare e assegnare profili scheda orario](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* Senza l&#39;accesso amministrativo ai processi di approvazione, creare e modificare i processi di approvazione per i gruppi e i sottogruppi gestiti. Per ulteriori informazioni, vedere [Creare un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Per informazioni sull&#39;accesso amministrativo ai processi di approvazione, vedere [Concedere agli utenti l&#39;accesso amministrativo ad alcune aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Creare pianificazioni e associarle a un gruppo gestito dall&#39;utente. Per ulteriori informazioni, vedere [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* Gestisci un team assegnato a un gruppo che gestisci, senza essere membro del team. Creare inoltre un report del team basato sul campo Gruppo per identificare il gruppo a cui è assegnato un determinato team. Per ulteriori informazioni, vedere [Creare un team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* Ripristina un progetto associato a un gruppo che gestisci, insieme a tutte le attività, i problemi o i documenti associati al progetto. Per ulteriori informazioni, vedere [Ripristinare gli elementi eliminati](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### Gestire le preferenze e gli strumenti del gruppo {#manage-group-preferences-and-tools}

* Quando una preferenza di progetto, una preferenza di attività o problema oppure una preferenza di schede orario e ore viene sbloccata per i gruppi in tutto il sistema, modificare tale preferenza per i gruppi gestiti. Queste preferenze influiscono sul comportamento di un progetto, di un’attività e di un problema. Per ulteriori informazioni vedi quanto segue:

   * [Configurare le preferenze del progetto per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* Creare e modificare gli stati dei gruppi per i gruppi gestiti. Per ulteriori informazioni, vedere [Creare o modificare lo stato di un gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Configurare una notifica di evento per i gruppi gestiti. È possibile eseguire questa operazione solo dopo che un amministratore di Workfront ha sbloccato la possibilità di configurare le notifiche degli eventi per i gruppi attraverso il sistema. Per ulteriori informazioni, vedere [Visualizzare e configurare le notifiche degli eventi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
