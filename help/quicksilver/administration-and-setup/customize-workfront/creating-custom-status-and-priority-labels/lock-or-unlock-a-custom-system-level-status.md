---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Stati bloccati e sbloccati a livello di sistema
description: Il blocco degli stati personalizzati è un modo per garantire che le persone in tutta l’organizzazione utilizzino gli stessi processi nel proprio flusso di lavoro. Quando uno stato è bloccato, è disponibile per tutti gli utenti del sistema. Sebbene sia possibile modificarlo o eliminarlo, gli amministratori di gruppi non possono farlo per i loro gruppi. Al contrario, lo sblocco degli stati personalizzati consente agli amministratori di gruppi una maggiore flessibilità per gestire i flussi di lavoro univoci utilizzati nei loro gruppi. Possono modificare gli attributi di uno stato sbloccato o eliminarlo per i loro gruppi.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0e58a1d6-5e0c-4445-a5ac-400dfd4c4948
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Stati bloccati e sbloccati a livello di sistema

Il blocco degli stati personalizzati è un modo per garantire che le persone in tutta l’organizzazione utilizzino gli stessi processi nel proprio flusso di lavoro. Quando uno stato è bloccato, è disponibile per tutti gli utenti del sistema. Sebbene sia possibile modificare o eliminare uno stato bloccato, gli amministratori dei gruppi non possono eseguire questa operazione per i propri gruppi, ma solo modificarne l&#39;ordine di visualizzazione nell&#39;elenco Stato.

Al contrario, lo sblocco degli stati personalizzati consente agli amministratori di gruppi una maggiore flessibilità per gestire i flussi di lavoro univoci utilizzati nei loro gruppi. Quando uno stato viene sbloccato, gli amministratori di gruppi possono modificarne gli attributi o eliminarlo dai rispettivi gruppi.

>[!IMPORTANT]
>
>Se si blocca uno stato personalizzato dopo che è stato sbloccato per un periodo di tempo qualsiasi, le impostazioni relative allo stato a livello di sistema sostituiscono quelle effettuate dagli amministratori di gruppo. Quando lo stato è bloccato, gli amministratori dei gruppi non possono modificare o eliminare lo stato dei loro gruppi.

Per istruzioni su come bloccare o sbloccare uno stato a livello di sistema, vedere [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Stati sbloccati nei processi di approvazione

In un processo di approvazione di sistema è possibile utilizzare sia gli stati bloccato che quello sbloccato. Se si crea un processo di approvazione del sistema con uno stato di sistema sbloccato, gli utenti di tutto il sistema possono allegare il processo di approvazione a qualsiasi progetto, attività o problema del sistema.

I messaggi di avviso vengono visualizzati nei seguenti scenari per aiutarti e fare in modo che gli utenti comprendano i risultati dei seguenti scenari:

* Un amministratore sblocca uno stato a livello di sistema utilizzato in un processo di approvazione. Viene visualizzato un messaggio di avviso che indica che lo stato sbloccato per i gruppi potrebbe essere eliminato, impedendo così ai membri del gruppo di utilizzare correttamente il processo di approvazione per gli oggetti assegnati al gruppo.

* Un utente inizia a modificare un processo di approvazione che utilizza uno stato sbloccato. Un messaggio avvisa l’utente dello stato sbloccato, in modo che possa valutare se è consigliabile bloccarlo di nuovo o sostituirlo.

* Un processo di approvazione a livello di sistema con uno stato sbloccato viene associato a un oggetto e lo stato è stato eliminato per il gruppo assegnato all&#39;oggetto. Quando un membro del gruppo accede alla sezione Approvazioni per l&#39;oggetto, un messaggio spiega che il processo di approvazione non può essere avviato per l&#39;oggetto.

In un processo di approvazione di gruppo è possibile utilizzare sia lo stato bloccato che quello sbloccato. Se si crea un processo di approvazione di gruppo con uno stato di gruppo sbloccato, gli utenti possono allegare il processo di approvazione a qualsiasi progetto, attività o problema associato al gruppo.
