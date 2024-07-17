---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 altri miglioramenti
description: Questa pagina descrive tutti gli altri miglioramenti apportati con la versione 2020.2 all’ambiente di produzione. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana dell’11 maggio 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 46ed705e-b966-4ae9-a602-a5a73a3de3aa
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 2020.2 altri miglioramenti

Questa pagina descrive tutti gli altri miglioramenti apportati con la versione 2020.2 all’ambiente di produzione. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana dell’11 maggio 2020.

Per un elenco di tutte le modifiche disponibili con la versione 2020.2, consulta [Panoramica sulla versione 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Per gli amministratori di Workfront: i nuovi modelli di layout creati in Workfront Classic sono ora disponibili nella nuova esperienza Workfront

I modelli di layout creati in Workfront Classic dopo l’autunno 2019 sono ora disponibili nella nuova esperienza Workfront. È consigliabile aggiornare questi modelli di layout nella nuova esperienza Workfront per sfruttare le nuove funzionalità e renderli il più utili possibile per gli utenti in tale ambiente.

Per ulteriori informazioni, vedere [Modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

**Disponibile in questi ambienti:**

* La nuova esperienza Adobe Workfront

## I processi di approvazione specifici del gruppo sono disponibili per tutti gli oggetti

Per utilizzare completamente i processi di approvazione specifici del gruppo, è ora possibile aggiungerli ad attività, problemi e progetti quando si modificano questi oggetti.

Quando si configurano code di richieste o Argomenti coda in un progetto, è inoltre possibile associare automaticamente un processo di approvazione specifico per gruppo a un&#39;attività nell&#39;area Attività della casella Modifica progetto, nonché ai problemi.

Per informazioni sull’aggiunta di processi di approvazione a progetti, attività e problemi, consulta i seguenti articoli:

* [Modificare progetti](../../../manage-work/projects/manage-projects/edit-projects.md)
* [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Modifica problemi](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
* [Crea argomenti coda](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)

## Creare processi di approvazione per gruppi utilizzando stati personalizzati

Per facilitare la gestione dei propri flussi di lavoro univoci da parte dei gruppi, è ora possibile utilizzare gli stati personalizzati specifici dei gruppi nei processi di approvazione.

In precedenza, un gruppo non poteva utilizzare i propri stati personalizzati con i propri processi di approvazione specifici per gruppo. Erano disponibili solo gli stati a livello di sistema, che non sempre rientravano nei processi di approvazione di gruppo.

Gli stati personalizzati possono essere utilizzati ora nei processi di approvazione a uso singolo e a livello di sistema:

* Crea un processo di approvazione a utente singolo per un oggetto (progetto, attività o problema) e basalo sugli stati associati al gruppo che lavora su tale oggetto. Questo include eventuali stati personalizzati associati al gruppo.
* Crea un processo di approvazione globale e rendilo disponibile solo per il gruppo o per tutti gli utenti del sistema.

Per gli utenti con accesso amministrativo ai processi di approvazione, le informazioni sulla configurazione dei processi di approvazione sono disponibili in [Creare un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (o se si utilizza Adobe Workfront Classic, vedere [Creazione di processi di approvazione](https://one.workfront.com/s/article/Creating-Approval-Processes-1001577410)).

Per gli utenti, le informazioni sull&#39;associazione dei processi di approvazione agli elementi di lavoro sono disponibili in [Associa un processo di approvazione nuovo o esistente al lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (oppure se si utilizza Adobe Workfront Classic, vedere [Associazione di un processo di approvazione nuovo o esistente al lavoro](https://one.workfront.com/s/article/Associating-a-New-or-Existing-Approval-Process-with-Work-708455630)).

**Disponibile in questi ambienti:**

* Adobe Workfront Classic
* La nuova esperienza Adobe Workfront

## Nuove pagine di sovrapposizione per la ricerca

Per consentire agli utenti di spostarsi più facilmente avanti e indietro tra le pagine di ricerca e le pagine precedenti nella nuova esperienza Workfront, è stata aggiunta una pagina di sovrapposizione della ricerca che copre parzialmente lo schermo.

Ora, quando si fa clic su Ricerca avanzata nel menu Ricerca o si esegue una ricerca di base, una pagina si apre dal lato destro dello schermo.

Per ulteriori informazioni, vedere [Cerca in Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

**Disponibile in questi ambienti:**

* La nuova esperienza Adobe Workfront

## Aggiornamenti a Sottoscrizioni eventi

Per consentire agli utenti di valutare, risolvere e risolvere meglio i problemi, abbiamo modificato il comportamento e aggiunto più dati all’API Sottoscrizioni eventi. Sono state apportate anche le seguenti modifiche:

* Migrazione delle tecnologie di messaggistica sottostanti
* Il servizio è stato ricostruito per avere dipendenze meno complesse e quindi scalare in modo più efficiente
* Miglioramenti apportati al monitoraggio e all&#39;avviso

Per ulteriori informazioni, consulta [Domande frequenti - Sottoscrizioni eventi](../../../wf-api/general/event-subs-faq.md) e [Best practice sottoscrizioni eventi](../../../wf-api/general/event-sub-best-practice.md).
