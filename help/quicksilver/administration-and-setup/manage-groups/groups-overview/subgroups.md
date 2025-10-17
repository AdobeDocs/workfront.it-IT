---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: Panoramica dei sottogruppi
description: È possibile creare fino a 14 livelli di sottogruppi in un unico gruppo. Su uno qualsiasi di questi livelli, puoi creare un numero illimitato di sottogruppi paralleli.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Panoramica sui sottogruppi

È possibile creare fino a 14 livelli di sottogruppi in un unico gruppo. Su uno qualsiasi di questi livelli, puoi creare un numero illimitato di sottogruppi paralleli. Per istruzioni, vedere [Creare un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

Per informazioni sui gruppi, vedere [Panoramica sui gruppi](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Cosa ereditano i sottogruppi?

I sottogruppi ereditano l’appartenenza del gruppo principale. Gli utenti e i gruppi di un sottogruppo hanno quindi la stessa visibilità, le stesse autorizzazioni e lo stesso accesso a tutti gli oggetti degli utenti e dei gruppi appartenenti al gruppo principale che condividono.

Inoltre, un sottogruppo eredita automaticamente gli amministratori di gruppo del suo gruppo principale, ma puoi anche assegnare i membri di un sottogruppo affinché agiscano come amministratori di gruppo.

>[!TIP]
>
>Talvolta, potrebbe essere utile utilizzare i sottogruppi per aggiungere più utenti a un gruppo esistente in modo da consentire loro di accedere a un oggetto di cui hanno bisogno.
>
>Si supponga, ad esempio, di disporre di un gruppo di tecnici dell&#39;help desk e di un gruppo separato di responsabili IT. Il gruppo dell&#39;helpdesk dispone delle autorizzazioni per una determinata coda di richieste. Si desidera aggiungere i responsabili IT al gruppo dell&#39;helpdesk in modo che dispongano anche delle autorizzazioni per la coda richieste. Senza la funzionalità di sottogruppo, sarebbe necessario aggiungere manualmente i responsabili IT al gruppo dell&#39;help desk, il che potrebbe essere inefficiente e difficile da gestire. Se si aggiunge il gruppo dei responsabili IT al gruppo dell&#39;help desk come sottogruppo, questa operazione viene eseguita più rapidamente con una sola modifica.

>[!NOTE]
>
>Se un utente è stato aggiunto a un sottogruppo e al relativo gruppo padre separatamente, la rimozione dell’utente da uno non comporta la rimozione dell’utente dall’altro. Se non si desidera che l&#39;utente disponga dell&#39;accesso consentito per il gruppo padre, è necessario rimuovere l&#39;utente sia dal sottogruppo che dal gruppo padre.

## Sottogruppi pubblici e privati

Per un gruppo pubblico, qualsiasi utente (interno o esterno al gruppo) con accesso di modifica utente può aggiungere il gruppo al profilo di altri utenti. Non possono farlo per un gruppo privato.

È possibile modificare questa opzione solo sul gruppo padre superiore in una gerarchia di gruppi con più livelli. Tutti i sottogruppi del gruppo padre ereditano l&#39;impostazione.

Se si crea un sottogruppo in un gruppo pubblico, anche il sottogruppo è pubblico per impostazione predefinita. Per ulteriori informazioni sulla creazione e la pubblicazione di un gruppo, vedere [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). Per ulteriori informazioni sull&#39;accesso necessario per modificare gli utenti, vedere [Concedere l&#39;accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Qualsiasi gruppo aggiunto a un gruppo esistente diventa automaticamente un sottogruppo e non è più un gruppo principale. Tuttavia, il sottogruppo mantiene gli utenti esistenti, nonché le associazioni con progetti, problemi e attività, oltre a tutti gli stati di progetto, attività e problema che appartengono al nuovo gruppo principale.

## Amministratori di gruppi per sottogruppi

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

È possibile assegnare i membri del sottogruppo come amministratori di gruppo al sottogruppo quando lo si crea o lo si modifica. Per istruzioni, vedere [&#128279;](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) nell&#39;articolo [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

In alternativa, puoi lasciare l’amministrazione del sottogruppo agli amministratori di gruppi assegnati ai gruppi al di sopra di esso. Quando si crea un sottogruppo, gli amministratori dei gruppi sopra i gruppi dispongono dell&#39;accesso automatico per gestire il sottogruppo.

>[!NOTE]
>
>Se si aggiunge un utente a un sottogruppo e tale utente è amministratore di gruppo per un gruppo in un punto qualsiasi al di sopra del sottogruppo, tale utente dispone dei diritti di amministratore per gestire il sottogruppo, anche senza essere assegnato come amministratore di gruppo.

Per informazioni sulle azioni disponibili per un amministratore di Adobe Workfront che gestisce il sistema Workfront, un amministratore di gruppo che gestisce un gruppo di livello superiore e un amministratore di gruppo che gestisce un sottogruppo, vedere [Azioni consentite per diversi tipi di amministratori](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md).
