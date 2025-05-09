---
content-type: release-notes
navigation-topic: product-releases-archive
title: Attività sulla versione 2017.3 di Beta 4
description: Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2017.3 di Beta 4. La funzionalità in questa pagina è stata resa disponibile nell’ambiente di anteprima la settimana del 25 settembre 2017. Sarà disponibile nell’ambiente di produzione all’inizio di novembre 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d6bb889c-a057-453f-8f80-761cfb1ad4a1
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '1676'
ht-degree: 0%

---

# Attività sulla versione 2017.3 di Beta 4

Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2017.3 di Beta 4. La funzionalità in questa pagina è stata resa disponibile nell’ambiente di anteprima la settimana del 25 settembre 2017. Sarà disponibile nell’ambiente di produzione all’inizio di novembre 2017.

>[!IMPORTANT]
>
> La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate nel 2017.3, consulta  Panoramica sull&#39;attività della versione [2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

La versione 2017.3 di Beta 4 contiene miglioramenti sia per gli amministratori di Workfront che per altri utenti:

**Per Amministratori**

* [Nuova area delle preferenze di gestione delle risorse nell&#39;area di configurazione](#new-resource-management-preferences-area-in-the-setup-area)

**Per Tutti Gli Utenti**

* [Attività duplicate](#duplicate-tasks)
* [Automatizzare Le Assegnazioni Durante La Pianificazione Delle Risorse](#automate-assignments-when-scheduling-resources)
* [Modifica assegnazioni per più attività durante la pianificazione delle risorse](#modify-assignments-for-multiple-tasks-when-scheduling-resources)
* [Applica distribuzione FTE alla programmazione delle risorse](#apply-fte-distribution-to-the-resource-planner)
* [La sezione Ruolo per le impostazioni utente include la percentuale di disponibilità FTE](#job-role-section-for-user-settings-includes-percentage-of-fte-availability)
* [Salva e gestisci filtri nel report utilizzo in un progetto](#save-and-manage-filters-in-the-utilization-report-on-a-project)
* [Opzioni di filtro aggiuntive nel report utilizzo](#additional-filtering-options-in-the-utilization-report)
* [Visualizza il report utilizzo per programma o Portfolio](#view-the-utilization-report-by-program-or-portfolio)
* [Mostra le informazioni originali sul problema nei report di progetto e attività](#show-original-issue-information-in-project-and-task-reports)
* [Filtra aggiornamenti di sistema nel flusso di aggiornamento ora è persistente tra gli oggetti](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Rapporto sugli stadi di bozza attivi in Workfront](#report-on-active-proof-stages-within-workfront)
* [Assegna profili di autorizzazione Workfront Proof personalizzati agli utenti in Workfront](#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront)
* [Risorsa oraria aggiunta agli abbonamenti agli eventi](#hour-resource-added-to-event-subscriptions)

## Duplica attività {#duplicate-tasks}

È ora possibile duplicare rapidamente un’attività o un set di attività all’interno di un progetto. Questa azione crea un&#39;attività identica a quella originale. Durante il processo di duplicazione non sono disponibili opzioni aggiuntive che consentirebbero di apportare modifiche all&#39;attività appena creata.  

Prima di questa modifica, è possibile copiare un&#39;attività in un nuovo progetto o nel progetto esistente e modificare alcune informazioni copiate.

Per  per ulteriori informazioni sulla duplicazione delle attività, vedere [Copia e duplica attività](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Automatizzare Le Assegnazioni Durante La Programmazione Delle Risorse {#automate-assignments-when-scheduling-resources}

>[!NOTE]
>
>Gli strumenti di pianificazione delle risorse sono stati dichiarati obsoleti e rimossi da Workfront con la versione 23.1. Per informazioni sulla pianificazione delle risorse tramite il Bilanciatore dei carichi di lavoro, vedere [Panoramica del Bilanciatore dei carichi di lavoro](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

È ora possibile consentire a Workfront di proporre automaticamente assegnazioni per attività e problemi non assegnati durante la programmazione di risorse per più progetti (dalla scheda Pianificazione) o durante la programmazione di risorse per un singolo progetto (dalla scheda Gestione del personale).

Workfront analizza le assegnazioni di lavoro correnti tra gli utenti disponibili e propone assegnazioni intelligenti e logiche per le attività o i problemi non ancora assegnati. È possibile modificare qualsiasi assegnazione proposta o esistente prima di finalizzare le assegnazioni.

Per ulteriori informazioni, vedere &quot;Assegnazione manuale di attività e problemi non assegnati nelle aree Pianificazione&quot;.

## Modifica assegnazioni per più attività durante la programmazione delle risorse {#modify-assignments-for-multiple-tasks-when-scheduling-resources}

Quando si assegnano, si scambiano o si annullano in blocco assegnazioni di utenti durante la programmazione delle risorse (dalla scheda Pianificazione o dalla scheda Assegnazione personale), è ora possibile modificare le assegnazioni per attività specifiche designate (incluse tutte le sottoattività e i problemi associati) in uno o più progetti.

Prima di questa modifica, era possibile modificare le assegnazioni alle attività e ai problemi solo per interi progetti (non era possibile designare attività specifiche all’interno di un progetto).

Per ulteriori informazioni, vedere &quot;Assegnazione manuale di attività e problemi non assegnati nelle aree Pianificazione&quot;.

## Applica distribuzione FTE alla programmazione delle risorse {#apply-fte-distribution-to-the-resource-planner}

>[!NOTE]
>
>Questa funzionalità non è attualmente disponibile in Anteprima su tutti i cluster.

È ora possibile visualizzare la quantità corretta di ore disponibili per ciascun ruolo dell&#39;utente in base alla percentuale di disponibilità FTE per ciascun ruolo, quando gli utenti hanno più di un ruolo.

Ad esempio, se la pianificazione di un utente indica che è disponibile a lavorare 100 ore in un mese e la sua Percentuale di disponibilità FTE per il Ruolo principale è del 75% e la Percentuale di disponibilità FTE del suo Altro Ruolo è del 25%, la Programmazione delle risorse elencherà l’utente con 75 ore disponibili nel Ruolo principale e con 25 ore disponibili nel suo Altro Ruolo.

Prima di questa modifica, il nome dell&#39;utente visualizzato nella Programmazione delle risorse solo per il Ruolo principale e la disponibilità completa dell&#39;utente in base alla programmazione (100 ore) era associata solo al Ruolo principale. L&#39;altro ruolo dell&#39;utente viene visualizzato nella Programmazione delle risorse solo se l&#39;utente è stato assegnato a un&#39;attività con quel ruolo e le ore disponibili per l&#39;utente con l&#39;altro ruolo sono pari a zero.

Per ulteriori informazioni sul calcolo delle ore disponibili e degli FTE disponibili per gli utenti e i ruoli nella Programmazione delle risorse, vedere [Panoramica sul calcolo delle ore e degli FTE per gli utenti e i ruoli nella Programmazione delle risorse](../../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## La sezione Ruolo per le impostazioni utente include la percentuale di disponibilità FTE {#job-role-section-for-user-settings-includes-percentage-of-fte-availability}

>[!NOTE]
>
>Questa funzionalità non è attualmente disponibile in Anteprima su tutti i cluster.

Ora, quando si aggiorna un profilo utente, è possibile aggiungere ulteriori ruoli a un utente e definire la percentuale di FTE allocata a ciascun ruolo.

Prima di questa modifica, non era possibile allocare una quantità specifica di FTE a nessuna delle mansioni a cui era associato l’utente.

Per ulteriori informazioni sull&#39;aggiornamento della percentuale di disponibilità FTE per le mansioni dell&#39;utente, vedere [Modificare il profilo di un utente](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) o [Configurare le impostazioni personali](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

## Nuova area delle preferenze di gestione delle risorse nell&#39;area di configurazione {#new-resource-management-preferences-area-in-the-setup-area}

Nella configurazione è ora disponibile una nuova area denominata Gestione risorse. In quest’area è stata introdotta un’impostazione che consente di specificare come calcolare la disponibilità dell’utente nella Programmazione delle risorse. Puoi calcolarlo utilizzando i seguenti metodi:

* Manualmente: la pianificazione predefinita del sistema, oltre al singolo FTE dell’utente, viene utilizzata per determinare la disponibilità dell’ora dell’utente nella Programmazione delle risorse. La pianificazione dell’utente viene ignorata.
* Automaticamente: la pianificazione dell&#39;utente viene utilizzata per determinare la disponibilità dell&#39;ora dell&#39;utente nella programmazione delle risorse. La disponibilità FTE viene calcolata in base alla pianificazione dell&#39;utente e alla pianificazione predefinita. Il valore dell&#39;FTE utente viene ignorato. 

Per ulteriori informazioni sulla configurazione delle preferenze di Gestione risorse per il sistema, vedere [Configurare le preferenze di Gestione risorse](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Salvataggio e gestione dei filtri nel report Utilizzo di un progetto {#save-and-manage-filters-in-the-utilization-report-on-a-project}

Ora puoi salvare i filtri creati nel rapporto Utilizzo. Inoltre, puoi rinominare un filtro salvato, duplicarne uno salvato, eliminarne uno salvato o modificarne uno salvato.

In precedenza, era necessario specificare singole opzioni di filtro ogni volta che si filtrava il rapporto Utilizzo.

Per ulteriori informazioni sul salvataggio e la gestione dei filtri nel report Utilizzo, vedere [Panoramica del report Utilizzo risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Panoramica del report Utilizzo risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Opzioni di filtro aggiuntive nel rapporto Utilizzo {#additional-filtering-options-in-the-utilization-report}

Ora, quando si esegue il rapporto Utilizzo, sono disponibili nuovi campi di filtro per Portfoli, Programmi e Progetti al momento della creazione del filtro, oltre ai campi Attività, Problemi e Ruoli precedentemente disponibili.

Prima di questa modifica, era possibile filtrare per portfolio, programma e progetto solo aggiungendo una nuova regola di filtro.

Per ulteriori informazioni, vedere [Panoramica del report sull&#39;utilizzo delle risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Panoramica del report sull&#39;utilizzo delle risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Visualizza il rapporto Utilizzo per programma o Portfolio {#view-the-utilization-report-by-program-or-portfolio}

È ora possibile visualizzare un rapporto Utilizzo per programma o portfolio. In questo modo è possibile visualizzare le informazioni provenienti da più progetti all&#39;interno di un unico rapporto Utilizzo.

Per facilitare questa modifica, la scheda Utilizzo è ora disponibile sia nell’area Reporting (Reporting) di Workfront, sia all’interno di un singolo progetto.

Prima di questa modifica, era possibile accedere ai rapporti sull’utilizzo solo all’interno di un progetto.

Per ulteriori informazioni, consulta  [Panoramica del report Utilizzo risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md). 

## Mostra le informazioni originali sulla Issue nei Report di Progetto e Attività {#show-original-issue-information-in-project-and-task-reports}

>[!NOTE]
>
>Questa funzionalità non è attualmente disponibile in Anteprima su tutti i cluster.

Ora è possibile trovare le seguenti informazioni sul problema originale in un progetto o in un rapporto di attività, per i progetti e le attività creati dalla conversione di un problema:

* Data voce problema originale
* Nome problema originale
* ID del mittente del problema originale

Queste informazioni possono essere visualizzate in un report o in un elenco di attività o progetti creando una visualizzazione personalizzata in modalità testo.

Prima di questa modifica non era possibile generare rapporti su queste informazioni.

Per ulteriori informazioni sulla creazione della visualizzazione in modalità testo personalizzata che acquisisce le informazioni dal problema originale, vedere [Visualizzazione: visualizzazione delle informazioni sul problema originale negli elenchi di attività o progetti](../../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

## Filtra aggiornamenti di sistema nel flusso di aggiornamento ora è persistente tra gli oggetti {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

>[!NOTE]
>
>Questa funzionalità non è stata rilasciata nell’ambiente di anteprima con Beta 4. Sarà disponibile in anteprima nella prima metà di ottobre.

L’opzione Filtra aggiornamenti sistema è ora persistente tra gli oggetti in tutto il sito Workfront. Questo consente di nascondere gli aggiornamenti di sistema e visualizzare solo i commenti degli utenti nel flusso di aggiornamento su un oggetto e di mantenere tale impostazione mentre si passa ad altri oggetti.

Prima di questa modifica, era necessario scegliere di filtrare gli aggiornamenti di sistema per ogni oggetto durante l&#39;esplorazione del sito Workfront.

Per ulteriori informazioni, vedere [Aggiorna lavoro](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Rapporto sugli stadi di bozza attivi in Workfront {#report-on-active-proof-stages-within-workfront}

Durante la creazione di un rapporto sulla versione del documento in Workfront, è ora disponibile una colonna denominata &quot;Fasi di bozza attive&quot;. Questa colonna consente di visualizzare la fase della bozza attualmente attiva su ogni versione del documento nel report. Il nome dell’area di visualizzazione viene visualizzato nella colonna &quot;Fasi di bozza attive&quot;. Se nella versione del documento non è attiva alcuna fase, la colonna è vuota.

Per ulteriori informazioni sui campi disponibili nelle visualizzazioni e nei report, consulta [Glossario della terminologia di Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Assegnare profili di autorizzazione Workfront Proof personalizzati agli utenti in Workfront {#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront}

Ora, quando si abilitano le funzionalità di verifica per un utente in Workfront, è possibile assegnare un profilo di autorizzazione Workfront Proof personalizzato. 

Prima di questa modifica, erano disponibili solo i seguenti profili di autorizzazione: supervisore, manager, amministratore.

## Risorsa oraria aggiunta agli abbonamenti agli eventi {#hour-resource-added-to-event-subscriptions}

Utilizzando la nuova risorsa Ora, ora puoi creare un abbonamento a un evento per mantenere l’applicazione di fatturazione sincronizzata con Workfront.

Per ulteriori informazioni sulle sottoscrizioni di eventi, vedere [API sottoscrizione eventi](../../../../wf-api/general/event-subs-api.md).
