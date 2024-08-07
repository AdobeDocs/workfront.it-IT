---
content-type: release-notes
navigation-topic: product-releases-archive
title: Attività sulla versione 2018.2 di Beta 2
description: Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.2 di Beta 2. La funzionalità è stata resa disponibile nell’ambiente di anteprima il 5 aprile 2018. Sarà disponibile nell’ambiente di produzione a giugno 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: c8ef68f5-53db-4c3c-af0f-e1c98521ec27
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Attività sulla versione 2018.2 di Beta 2

Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.2 di Beta 2. La funzionalità è stata resa disponibile nell’ambiente di anteprima il 5 aprile 2018. Sarà disponibile nell’ambiente di produzione a giugno 2018.

>[!IMPORTANT]
>
> La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate in 2018.2, consulta  Panoramica dell&#39;attività di [versione 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La versione 2018.2 di Beta 2 contiene i seguenti miglioramenti:

* [Modifica campi direttamente dall&#39;area Home](#edit-fields-directly-from-the-home-area)
* [Tempo di connessione in giorni](#log-time-in-days)
* [Visualizzare le relazioni tra i predecessori di progetti nel diagramma di Gantt in un elenco di progetti](#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects)
* [Utilizzare il costo preventivato in Ottimizzatore Portfolio per calcolare le finanze del Portfolio](#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances)
* [Rapporto utilizzo: popola le ore preventivate dalla nuova area budget risorse](#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area) (solo anteprima)

* [Rapporto utilizzo: visualizzazione ore preventivate per utente in un progetto](#utilization-report-view-budgeted-hours-by-user-on-a-project) (solo anteprima)

* [Avanzamento bozza dall&#39;elenco dei documenti disponibile per gli utenti che non eseguono bozze](#proof-progress-from-the-document-list-available-to-non-proofing-users)
* [Miglioramenti per dispositivi mobili](#mobile-improvements)

## Modifica campi direttamente dall&#39;area Home {#edit-fields-directly-from-the-home-area}

Ora, quando si seleziona un oggetto nell’area Home, è possibile modificare i campi associati a tale oggetto direttamente dal pannello di destra dell’area Home. 

Prima di questa modifica, le informazioni potevano essere visualizzate solo nell’area Home, non modificate.

Per ulteriori informazioni, vedere [Aggiornare o modificare un elemento di lavoro nell&#39;area Home](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md) nell&#39;articolo  [Aggiornare o modificare un elemento di lavoro nell&#39;area Home](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).

## Tempo di connessione in giorni {#log-time-in-days}

Gli amministratori di Workfront ora possono configurare il tempo di accesso degli utenti nella propria organizzazione in giorni o ore. Gli utenti con una licenza Planner possono configurare questa impostazione autonomamente.

Prima di questa modifica, gli utenti potevano registrare il tempo solo in ore.

Puoi configurare questa impostazione modificando il profilo utente. Per ulteriori informazioni, vedere [Configurare l&#39;ora registrata in ore o giorni](../../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

Per informazioni su come gli utenti possono registrare il tempo nei giorni successivi all&#39;aggiornamento di questa impostazione, vedere [Tempo di registrazione](../../../../timesheets/create-and-manage-timesheets/log-time.md).

## Visualizzare le relazioni tra i predecessori di progetti nel diagramma di Gantt in un elenco di progetti {#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects}

È ora possibile visualizzare le relazioni dei predecessori tra progetti nel diagramma di Gantt nei seguenti elenchi di progetti:

* Scheda Progetti all’interno di un portfolio o programma
* In un report di progetto

Prima di questa modifica, era possibile visualizzare le relazioni predecessore tra progetti diversi solo per singole attività a livello di progetto.

Per ulteriori informazioni, vedere [Configurare la visualizzazione delle informazioni nel Diagramma di Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## Utilizzare Costo preventivato in Ottimizzatore Portfolio per calcolare le finanze del Portfolio {#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances}

Il nuovo Ottimizzatore Portfolio ora utilizza il Costo preventivato della nuova area Budget risorse del Business Case o del Pianificatore risorse per calcolare i campi riportati di seguito.

* Valore Netto
* Ritorno sull&#39;investimento (ROI)
* Costo

In precedenza, sia il nuovo che il precedente Ottimizzatore Portfolio utilizzavano il costo preventivato legacy. Legacy Portfolio Optimizer utilizza ancora il costo preventivato legacy per calcolare il valore netto, il ritorno sull’investimento e il costo.

Sono stati inoltre aggiunti due nuovi campi ai campi finanziari del Portfolio: ROI legacy e Valore netto legacy per acquisire i nuovi valori dai nuovi strumenti di gestione delle risorse.

Per ulteriori informazioni, vedere [Panoramica di Portfolio Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md) nell&#39;articolo  [Panoramica di Portfolio Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Rapporto Utilizzo: popola le ore preventivate dalla nuova area di budget risorse {#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area}

>[!NOTE]
>
>Questa funzionalità non verrà inclusa nella versione ufficiale dell’ambiente di anteprima con la versione 2018.2. Verrà reintrodotto durante il periodo beta per la versione 2018.3 e rilasciato nell’ambiente di produzione con la versione 2018.3. 

Le ore preventivate nel rapporto Utilizzo ora sono compilate dalle informazioni disponibili nella nuova area Budget risorse del Business Case.

Prima di questa modifica, venivano utilizzate le informazioni provenienti dall’area Stime risorse legacy.

Per ulteriori informazioni, vedere [Panoramica del report sull&#39;utilizzo delle risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) nell&#39;articolo  [Panoramica del report Utilizzo risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Rapporto Utilizzo: visualizzazione delle ore preventivate per utente in un progetto {#utilization-report-view-budgeted-hours-by-user-on-a-project}

>[!NOTE]
>
>Questa funzionalità non verrà inclusa nella versione ufficiale dell’ambiente di anteprima con la versione 2018.2. Verrà reintrodotto durante il periodo beta per la versione 2018.3 e rilasciato nell’ambiente di produzione con la versione 2018.3. 

Il rapporto Utilizzo di un progetto ora visualizza Ore preventivate per utente.

Prima di questa modifica, il rapporto Utilizzo mostrava Ore preventivate solo per mansione. 

Per ulteriori informazioni, vedere [Panoramica del report sull&#39;utilizzo delle risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) nell&#39;articolo [Panoramica del report sull&#39;utilizzo delle risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Avanzamento bozza dall’elenco dei documenti disponibile per gli utenti non bozza {#proof-progress-from-the-document-list-available-to-non-proofing-users}

Ora gli indicatori di avanzamento della bozza (Inviato, Aperto, Commenti aggiunti e Decisione) vengono visualizzati per tutti gli utenti quando si visualizza l’elenco dei documenti. Sono inclusi gli utenti che non sono in grado di generare bozze (per ulteriori informazioni su come consentire agli utenti di generare bozze, consulta la sezione .

Prima di questa modifica, gli indicatori di avanzamento della bozza erano disponibili solo per gli utenti che potevano generare bozze.

Per ulteriori informazioni, vedere [Panoramica sull&#39;avanzamento e sullo stato della bozza](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

## Miglioramenti per dispositivi mobili {#mobile-improvements}

L’app mobile contiene i seguenti miglioramenti:

* I collegamenti condivisi con te in altre app mobili ora vengono aperti nell’app mobile di Workfront.

  Per ulteriori informazioni sulla condivisione di collegamenti, vedere .

  Questo aggiornamento è ora disponibile su iOS e Android.

* Abbiamo aggiornato i requisiti di supporto per la piattaforma iOS per supportare iPhone X.

  Per ulteriori informazioni sui dispositivi mobili e i sistemi operativi supportati, consulta la . 
