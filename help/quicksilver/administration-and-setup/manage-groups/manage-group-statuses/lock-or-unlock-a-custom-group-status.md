---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Stati del gruppo bloccati e sbloccati
description: Il blocco degli stati personalizzati di un gruppo è un modo per garantire che le persone del gruppo e dei suoi sottogruppi utilizzino gli stessi processi nel loro flusso di lavoro. Quando lo stato di un gruppo è bloccato, è disponibile per tutti gli utenti del gruppo e dei gruppi inferiori. Anche se l’utente (o un amministratore di Workfront) può modificare o eliminare uno stato bloccato, gli amministratori dei sottogruppi di seguito non possono farlo per tali gruppi. Al contrario, lo sblocco degli stati personalizzati di un gruppo consente agli amministratori dei sottogruppi più bassi di gestire in modo più flessibile i loro flussi di lavoro. Possono modificare gli attributi di uno stato sbloccato o eliminarlo per i gruppi.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3463e4cb-7336-49b7-b81a-c2acef72f61d
source-git-commit: d67de32fcbe4706cf8a1fc6f5bb8ec9d08b07119
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Stati del gruppo bloccati e sbloccati

Il blocco degli stati personalizzati di un gruppo è un modo per garantire che le persone del gruppo e dei suoi sottogruppi utilizzino gli stessi processi nel loro flusso di lavoro. Quando lo stato di un gruppo è bloccato, è disponibile per tutti gli utenti del gruppo e dei gruppi inferiori. Anche se l’utente (o un amministratore di Workfront) può modificare o eliminare uno stato bloccato, gli amministratori dei sottogruppi sottostanti non possono farlo per tali gruppi; possono modificare solo l&#39;ordine di visualizzazione nell&#39;elenco Stato.

Al contrario, lo sblocco degli stati personalizzati di un gruppo consente agli amministratori dei sottogruppi più bassi una maggiore flessibilità per gestire i flussi di lavoro univoci utilizzati nei loro gruppi. Quando uno stato di gruppo viene sbloccato, gli amministratori dei sottogruppi inferiori possono modificarne gli attributi o eliminarli per tali sottogruppi.

>[!IMPORTANT]
>
>Se si blocca uno stato personalizzato dopo che è stato sbloccato per un qualsiasi periodo di tempo, le impostazioni per lo stato sostituiscono quelle effettuate dagli amministratori di gruppo nei sottogruppi inferiori. Mentre lo stato è bloccato, questi amministratori non possono modificare o eliminare lo stato dei loro gruppi.

Per istruzioni su come bloccare o sbloccare lo stato di un gruppo, consulta [Creare o modificare uno stato di gruppo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

È possibile utilizzare sia lo stato bloccato che quello sbloccato in un processo di approvazione del gruppo. Se si crea un processo di approvazione del gruppo con uno stato di gruppo sbloccato, gli utenti possono allegare il processo di approvazione a qualsiasi progetto, attività o problema associato al gruppo.

