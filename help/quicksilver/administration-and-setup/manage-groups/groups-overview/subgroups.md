---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: Panoramica sui sottogruppi
description: È possibile creare fino a 14 livelli di sottogruppi in un unico gruppo. Su uno qualsiasi di questi livelli, puoi creare un numero illimitato di sottogruppi paralleli.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# Panoramica sui sottogruppi

È possibile creare fino a 14 livelli di sottogruppi in un unico gruppo. Su uno qualsiasi di questi livelli, puoi creare un numero illimitato di sottogruppi paralleli. Per istruzioni, consulta [Creare un sottogruppo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

Per informazioni sui gruppi, consulta [Panoramica sui gruppi](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Cosa ereditano i sottogruppi?

I sottogruppi ereditano l’appartenenza del gruppo padre. Pertanto, gli utenti e i gruppi di un sottogruppo hanno la stessa visibilità, le stesse autorizzazioni e l&#39;accesso a tutti gli oggetti degli utenti e dei gruppi che appartengono al gruppo padre che condividono.

Inoltre, un sottogruppo eredita automaticamente gli amministratori del gruppo di primo livello, ma è anche possibile assegnare i membri di un sottogruppo in modo che agiscano come amministratori del gruppo.

>[!TIP]
>
>A volte può essere utile utilizzare sottogruppi per aggiungere più utenti a un gruppo esistente per consentire loro di accedere a un oggetto di cui hanno bisogno.
>
>Ad esempio, supponiamo di avere un gruppo di tecnici dell&#39;help desk e un gruppo separato di amministratori IT. Il gruppo help desk dispone delle autorizzazioni per una determinata coda di richiesta. Si desidera aggiungere i director IT al gruppo help desk in modo che dispongano anche delle autorizzazioni per la coda richieste. Senza la funzionalità dei sottogruppi, è necessario aggiungere manualmente i director IT al gruppo help desk, che potrebbe essere inefficiente e difficile da gestire. Se aggiungi il gruppo di amministratori IT al gruppo help desk come sottogruppo, esegui questo compito più velocemente con una sola modifica.

>[!NOTE]
>
>Se un utente è stato aggiunto separatamente a un sottogruppo e al relativo gruppo padre, la rimozione dell&#39;utente da un altro non comporta la rimozione dell&#39;utente dall&#39;altro. Se non si desidera che l&#39;utente disponga dell&#39;accesso consentito per il gruppo padre, è necessario rimuovere l&#39;utente sia dal sottogruppo che dal gruppo padre.

## Sottogruppi pubblici e privati

Per un gruppo pubblico, qualsiasi utente (all&#39;interno o all&#39;esterno del gruppo) con accesso per l&#39;utente con modifica può aggiungere il gruppo al profilo di altri utenti. Non possono farlo per un gruppo privato.

È possibile modificare questa opzione solo nel gruppo principale superiore in una gerarchia di gruppi con più di un livello. Tutti i sottogruppi del gruppo padre ereditano le relative impostazioni.

Se crei un sottogruppo sotto un gruppo pubblico, anche il sottogruppo è pubblico, per impostazione predefinita. Per ulteriori informazioni sulla creazione e la pubblicazione di un gruppo, consulta [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). Per ulteriori informazioni sull&#39;accesso necessario per modificare gli utenti, vedi [Concedere l’accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Qualsiasi gruppo aggiunto a un gruppo esistente diventa automaticamente un sottogruppo e non è più un gruppo principale. Tuttavia, il sottogruppo mantiene i propri utenti esistenti, nonché le associazioni con progetti, problemi e attività, oltre a tutti gli stati di progetto, attività e problemi che appartengono al nuovo gruppo padre.

## Amministratori di gruppo per sottogruppi

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

È possibile assegnare i membri del sottogruppo come amministratori di gruppo al sottogruppo quando lo si crea o lo si modifica. Per istruzioni, consulta [](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) nell&#39;articolo [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

In alternativa, puoi lasciare l’amministrazione del sottogruppo agli amministratori del gruppo assegnati ai gruppi sopra di esso. Quando crei un sottogruppo, gli amministratori del gruppo posizionati sui gruppi sopra hanno accesso automatico per gestire il sottogruppo.

>[!NOTE]
>
>Se si aggiunge un utente a un sottogruppo e tale utente è un amministratore di gruppo per un gruppo in un punto qualsiasi del sottogruppo, tale utente dispone dei diritti amministrativi per gestire il sottogruppo, anche senza essere assegnato come amministratore di gruppo.

Per informazioni sulle azioni disponibili per un amministratore Adobe Workfront che gestisce il sistema Workfront, un amministratore di gruppo che gestisce un gruppo di livello principale e un amministratore di gruppo che gestisce un sottogruppo, consulta [Azioni consentite per diversi tipi di amministratori](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md).
