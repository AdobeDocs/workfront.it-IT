---
content-type: release-notes
navigation-topic: product-releases-archive
title: Attività sulla versione finale 2018.1 di Beta
description: Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione finale di Beta 2018.1. La funzionalità è stata resa disponibile nell’ambiente di anteprima il 31 gennaio 2018. Sarà disponibile nell’ambiente di produzione a marzo 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 35bd3604-5452-4b46-afb1-78bc2fbb48ec
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# Attività sulla versione finale 2018.1 di Beta

Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione finale di Beta 2018.1. La funzionalità è stata resa disponibile nell’ambiente di anteprima il 31 gennaio 2018. Sarà disponibile nell’ambiente di produzione a marzo 2018.

>[!IMPORTANT]
>
> La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate in 2018.1, consulta  Panoramica dell&#39;attività della versione di [2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La versione finale 2018.1 di Beta contiene miglioramenti sia per gli amministratori di Workfront che per altri utenti:

**Per Amministratori**

* [Configura la disponibilità delle risorse e le allocazioni utente da calcolare in base alla pianificazione utente](#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule)

**Per Tutti Gli Utenti**

* [Miglioramenti per dispositivi mobili](#mobile-enhancements)
* [Integrazione Jira](#jira-integration)
* [Aggiornamento dei nomi dei visualizzatori di verifica](#update-to-proofing-viewer-names)
* [Modifica della cadenza di sincronizzazione durante la sincronizzazione dall&#39;ambiente di produzione della bozza all&#39;anteprima](#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview)
* [Messaggio di avvertenza visualizzato quando viene raggiunto il limite di 2.000 elementi nella programmazione delle risorse](#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner)

## Miglioramenti per dispositivi mobili {#mobile-enhancements}

Le seguenti funzionalità saranno disponibili negli app store per dispositivi mobili all’inizio di marzo 2018:

* Nuova navigazione: la home page delle nostre app mobili è stata riprogettata.
* Home on Mobile: la nuova funzionalità Home è stata aggiornata anche sulle app mobili.

La nuova funzionalità è supportata sia per le piattaforme iOS che per Android.

## Integrazione Jira {#jira-integration}

Ora puoi collegare i problemi Jira ad attività o problemi Workfront installando e configurando il componente aggiuntivo Workfront per Jira. Con questa integrazione, i project manager possono continuare a lavorare in Workfront, mentre i tecnici dello sviluppo possono continuare a lavorare in Jira, mentre i singoli elementi vengono collegati tramite l’integrazione di Workfront con Jira.

Puoi configurare quanto segue tramite questa integrazione:

* Stabilisci i trigger per le assegnazioni Workfront per creare automaticamente problemi Jira quando si verificano.
* Collega manualmente i problemi Jira ad attività o problemi Workfront creati in precedenza.
* Specificare i campi da sincronizzare sugli elementi collegati non appena uno degli elementi viene aggiornato in una delle applicazioni.

Il componente aggiuntivo Workfront sarà disponibile per le versioni On-Premise e On-Demand di Jira. Il componente aggiuntivo è gratuito e sarà disponibile per il download nel Marketplace Atlassian all’inizio di marzo 2018.

Per ulteriori informazioni sul componente aggiuntivo Workfront per Jira, incluso un collegamento per scaricarlo, vedere [Utilizzo di Workfront con Jira.](https://support.workfront.com/hc/en-us/sections/115001130053)

## Aggiornamento dei nomi dei visualizzatori di verifica {#update-to-proofing-viewer-names}

I nomi del visualizzatore di bozze basato su HTML5 e dei visualizzatori di bozze basati sul Flash sono stati rinominati in tutto il sistema Workfront. I nomi precedenti e aggiornati sono i seguenti: 

| **Nome precedente** | **Nome aggiornato** |
|---|---|
| Visualizzatore di bozze di HTML5 | Nuovo visualizzatore di bozze |
| Visualizzatore bozze Flash | Visualizzatore di bozze legacy |

{style="table-layout:auto"}

 Per ulteriori informazioni sull&#39;utilizzo del nuovo visualizzatore di bozze, vedere [Esame delle bozze nel visualizzatore di bozze.](https://support.workfront.com/hc/en-us/sections/115000275214)

## Configura la disponibilità delle risorse e le allocazioni utente da calcolare in base alla pianificazione utente {#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule}

>[!NOTE]
>
>Gli strumenti di pianificazione delle risorse sono stati dichiarati obsoleti e rimossi da Workfront con la versione 23.1. Per informazioni sulla pianificazione delle risorse tramite il Bilanciatore dei carichi di lavoro, vedere [Panoramica del Bilanciatore dei carichi di lavoro](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

L’amministratore di Workfront può ora determinare il modo in cui Workfront calcola la disponibilità delle risorse e l’allocazione degli utenti a livello di sistema (considerando le ore e la disponibilità FTE). L&#39;amministratore di Workfront può configurare la disponibilità delle risorse e l&#39;allocazione degli utenti da calcolare utilizzando la pianificazione predefinita o quella dell&#39;utente.

Questa impostazione influisce sulla disponibilità dell&#39;utente nelle seguenti circostanze durante la pianificazione delle risorse:

* Quando si consente a Workfront di assegnare automaticamente le risorse, come descritto in &quot;Assegnare manualmente le attività e i problemi non assegnati nelle aree Pianificazione&quot;.

* Quando vengono visualizzati gli indicatori di allocazione, come descritto in &quot;Gestire le allocazioni utente nelle aree Pianificazione&quot;.

Per ulteriori informazioni, vedere &quot;Configurare il modo in cui Workfront calcola la disponibilità delle ore risorsa e FTE per l&#39;area Pianificazione&quot;.

>[!NOTE]
>
>Gli strumenti di pianificazione delle risorse sono stati dichiarati obsoleti e rimossi da Workfront con la versione 23.1. Per informazioni sulla pianificazione delle risorse tramite il Bilanciatore dei carichi di lavoro, vedere [Panoramica del Bilanciatore dei carichi di lavoro](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).


## Modifica della cadenza di sincronizzazione durante la sincronizzazione dall’ambiente di produzione della bozza all’ambiente di anteprima {#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview}

>[!NOTE]
>
>Questa modifica entrerà in vigore l’11 febbraio 2018.

I dati dell’ambiente di produzione di Workfront Proof vengono ora sincronizzati con l’ambiente di anteprima di Workfront Proof ogni settimana.

Prima di questa modifica, i dati venivano sincronizzati dall’ambiente di produzione Workfront Proof all’ambiente di anteprima su base mensile, mentre i dati dall’ambiente di produzione Workfront venivano sincronizzati all’ambiente di anteprima Workfront su base settimanale. Questa discrepanza ha causato alcuni errori di sincronizzazione durante l’utilizzo della funzionalità Bozza nell’ambiente di anteprima di Workfront. 

Per ulteriori informazioni, vedere [Anteprima ambiente di test sandbox: Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md). 

## Messaggio di avvertenza visualizzato quando viene raggiunto il limite di 2.000 elementi nella programmazione delle risorse {#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner}

Poiché stiamo attualmente lavorando a una soluzione più permanente per migliorare le prestazioni nella Programmazione delle risorse, è stato introdotto un limite di 2.000 elementi per ogni visualizzazione applicabile alla Programmazione delle risorse:

* Nella Vista utente vengono visualizzate solo 2.000 assegnazioni
* Nella visualizzazione Progetto sono visualizzati solo 2.000 progetti
* Nella vista Ruolo vengono visualizzati solo 2.000 ruoli

Quando la Programmazione delle risorse tenta di caricare più di 2.000 elementi, viene visualizzata una notifica che avvisa che è possibile visualizzare solo 2.000 elementi.

Per ulteriori informazioni su questi limiti e su come influiscono sulla pianificazione delle risorse, vedere [Limitazioni di visualizzazione della pianificazione delle risorse](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our beta program for the Resource Planner performance, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a>.</p>
-->
