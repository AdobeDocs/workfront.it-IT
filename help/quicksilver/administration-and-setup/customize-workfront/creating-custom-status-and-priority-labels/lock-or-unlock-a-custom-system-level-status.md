---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Stati bloccati e sbloccati a livello di sistema
description: Il blocco degli stati personalizzati consente di garantire che le persone di tutta l’organizzazione utilizzino gli stessi processi nel flusso di lavoro. Quando uno stato è bloccato, è disponibile a tutti gli utenti del sistema. Anche se è possibile modificarlo o eliminarlo, gli amministratori di gruppo non possono farlo per i loro gruppi. Al contrario, lo sblocco degli stati personalizzati consente agli amministratori di gruppo una maggiore flessibilità per gestire i flussi di lavoro univoci utilizzati nei loro gruppi. Possono modificare gli attributi di uno stato sbloccato o eliminarlo per i gruppi.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0e58a1d6-5e0c-4445-a5ac-400dfd4c4948
source-git-commit: c70a10a920d32ad00a2e833b331c92a598902d21
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Stati bloccati e sbloccati a livello di sistema

Il blocco degli stati personalizzati consente di garantire che le persone di tutta l’organizzazione utilizzino gli stessi processi nel flusso di lavoro. Quando uno stato è bloccato, è disponibile a tutti gli utenti del sistema. Anche se è possibile modificare o eliminare uno stato bloccato, gli amministratori dei gruppi non possono farlo per i loro gruppi; possono modificare solo l&#39;ordine di visualizzazione nell&#39;elenco Stato.

Al contrario, lo sblocco degli stati personalizzati consente agli amministratori di gruppo una maggiore flessibilità per gestire i flussi di lavoro univoci utilizzati nei loro gruppi. Quando uno stato viene sbloccato, gli amministratori di gruppo possono modificarne gli attributi o eliminarli per i gruppi.

>[!IMPORTANT]
>
>Se si blocca uno stato personalizzato dopo che è stato sbloccato per un qualsiasi periodo di tempo, le impostazioni a livello di sistema per lo stato sostituiscono quelle effettuate dagli amministratori di gruppo. Mentre lo stato è bloccato, gli amministratori del gruppo non possono modificare o eliminare lo stato dei gruppi.

Per istruzioni su come bloccare o sbloccare uno stato a livello di sistema, vedi [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Stati sbloccati nei processi di approvazione

È possibile utilizzare sia lo stato bloccato che quello sbloccato in un processo di approvazione del sistema. Se si crea un processo di approvazione del sistema con uno stato di sistema sbloccato, gli utenti di tutto il sistema possono allegare il processo di approvazione a qualsiasi progetto, attività o problema nel sistema.

I messaggi di avviso vengono visualizzati nei seguenti scenari per aiutarti a comprendere i risultati dei seguenti scenari:

* Un amministratore sblocca lo stato a livello di sistema utilizzato in un processo di approvazione. Un messaggio avverte che potrebbe eliminare lo stato sbloccato per i gruppi, impedendo ai membri del gruppo di utilizzare correttamente il processo di approvazione per gli oggetti assegnati al gruppo.

* Un utente inizia a modificare un processo di approvazione che utilizza uno stato sbloccato. Un messaggio avvisa l’utente dello stato sbloccato in modo che possa valutare se sia opportuno bloccarlo nuovamente o sostituirlo.

* Un processo di approvazione a livello di sistema con stato sbloccato viene allegato a un oggetto e lo stato viene eliminato per il gruppo assegnato all&#39;oggetto. Quando un membro del gruppo passa alla sezione Approvazioni per l&#39;oggetto, un messaggio spiega che il processo di approvazione non può essere avviato per l&#39;oggetto.

È possibile utilizzare sia lo stato bloccato che quello sbloccato in un processo di approvazione del gruppo. Se si crea un processo di approvazione del gruppo con uno stato di gruppo sbloccato, gli utenti possono allegare il processo di approvazione a qualsiasi progetto, attività o problema associato al gruppo.