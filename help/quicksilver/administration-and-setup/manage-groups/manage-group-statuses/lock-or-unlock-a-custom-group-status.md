---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Stati dei gruppi bloccati e sbloccati
description: Il blocco degli stati personalizzati di un gruppo consente di garantire che gli utenti del gruppo e dei relativi sottogruppi utilizzino gli stessi processi nel flusso di lavoro. Quando lo stato di un gruppo è bloccato, è disponibile per tutti gli utenti del gruppo e dei gruppi inferiori.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3463e4cb-7336-49b7-b81a-c2acef72f61d
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Stati dei gruppi bloccati e sbloccati

Il blocco degli stati personalizzati di un gruppo consente di garantire che gli utenti del gruppo e dei relativi sottogruppi utilizzino gli stessi processi nel flusso di lavoro. Quando lo stato di un gruppo è bloccato, è disponibile per tutti gli utenti del gruppo e dei gruppi inferiori. Anche se l&#39;utente o un amministratore di Workfront può modificare o eliminare uno stato bloccato, gli amministratori dei sottogruppi di seguito non possono eseguire questa operazione per tali gruppi, ma solo modificarne l&#39;ordine di visualizzazione nell&#39;elenco Stato.

Al contrario, sbloccare gli stati personalizzati di un gruppo consente agli amministratori dei sottogruppi più bassi di gestire in modo più flessibile i flussi di lavoro univoci utilizzati nei loro gruppi. Quando lo stato di un gruppo viene sbloccato, gli amministratori dei sottogruppi inferiori possono modificarne gli attributi o eliminarlo per tali sottogruppi.

>[!IMPORTANT]
>
>Se si blocca uno stato personalizzato dopo che è stato sbloccato per un periodo di tempo qualsiasi, le impostazioni dello stato sostituiscono quelle effettuate dagli amministratori di gruppi nei sottogruppi inferiori. Quando lo stato è bloccato, gli amministratori non possono modificare o eliminare lo stato dei loro gruppi.

Per istruzioni su come bloccare o sbloccare uno stato di gruppo, vedere [Creare o modificare uno stato di gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

In un processo di approvazione di gruppo è possibile utilizzare sia lo stato bloccato che quello sbloccato. Se si crea un processo di approvazione di gruppo con uno stato di gruppo sbloccato, gli utenti possono allegare il processo di approvazione a qualsiasi progetto, attività o problema associato al gruppo.

