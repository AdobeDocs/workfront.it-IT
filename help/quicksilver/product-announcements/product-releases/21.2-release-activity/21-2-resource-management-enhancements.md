---
content-type: release-notes
keywords: note,trimestrale,aggiornamento,rilascio
navigation-topic: 2021-2-release-activity
title: 21.2 Miglioramenti alla gestione delle risorse
description: Questa pagina descrive tutti i miglioramenti alla gestione delle risorse apportati con la versione 21.2 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione la settimana del 10 maggio 2021. Per un elenco di tutte le modifiche disponibili con la versione 21.2, consulta Panoramica sulla versione 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# 21.2 Miglioramenti alla gestione delle risorse

Questa pagina descrive tutti i miglioramenti alla gestione delle risorse apportati con la versione 21.2 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione la settimana del 10 maggio 2021. Per un elenco di tutte le modifiche disponibili con la versione 21.2, consulta la [panoramica sulla versione 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Vista a livello di mese nel Bilanciatore dei carichi di lavoro

Per aiutarti a gestire l’allocazione delle risorse per periodi di tempo più lunghi, ora abbiamo implementato una visualizzazione a livello di mese per il Bilanciatore dei carichi di lavoro. Puoi visualizzare fino a tre mesi alla volta e aggiornare le allocazioni di risorse mensili. Prima di questa modifica, era possibile visualizzare il Bilanciatore dei carichi di lavoro solo per giorno o per settimana.

Per informazioni, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Connessione tra la Pianificazione scenario, il Bilanciatore dei carichi di lavoro e l&#39;elenco delle attività

>[!NOTE]
>
>Disponibile solo nella nuova esperienza Adobe Workfront.

Per aiutarti nella pianificazione strategica dei tuoi progetti e garantirne l&#39;allineamento con le iniziative di più ampio respiro di Scenario Planner, abbiamo creato una nuova area sul progetto che mostra i requisiti del ruolo dalle iniziative così come le ore pianificate stimate sugli elementi di lavoro del progetto. Quest’area è disponibile per il Bilanciatore dei carichi di lavoro a livello di progetto e per l’elenco delle attività nella nuova esperienza Workfront. Nell’esperienza classica, questo è disponibile solo per il progetto Bilanciatore dei carichi di lavoro.

Per informazioni, vedere i seguenti articoli:

* [Panoramica sulla riconciliazione delle allocazioni di risorse tra progetti e iniziative](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Questa nuova funzionalità è visibile a tutti gli utenti, sia nella nuova che nella classica esperienza Workfront. Questo è visibile anche ai clienti che non hanno acquistato una licenza Workfront Scenario Planner.

## Usa ore pianificate per il calcolo dei valori netti nella pianificazione risorse

Una nuova impostazione nella pianificazione risorse consente di utilizzare le ore pianificate per il calcolo dei valori netti.

Prima di questo miglioramento, Workfront calcolava i valori netti utilizzando solo le ore preventivate. I valori netti visualizzano la differenza tra ore disponibili e ore preventivate o pianificate, FTE o costo. Ore preventivate è ancora l&#39;impostazione predefinita durante il calcolo dei valori netti.

Per informazioni, vedere [Panoramica su ore, FTE e informazioni sui costi nelle visualizzazioni Progetto e Ruolo della Programmazione delle risorse](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Visualizzazione di 12 settimane nel Bilanciatore dei carichi di lavoro

Ora è possibile visualizzare fino a 12 settimane di informazioni nel Bilanciatore dei carichi di lavoro. Prima di questo miglioramento, era possibile visualizzare 2, 4 e 6 settimane di informazioni.

Per informazioni sulla visualizzazione del Bilanciatore dei carichi di lavoro, vedere [Navigare nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)Navigare nel Bilanciatore dei carichi di lavoro.

## Modifica del funzionamento del filtro Mansione nell’area Non assegnato del Bilanciatore dei carichi di lavoro

Per migliorare il funzionamento del filtro Mansione nel Bilanciatore dei carichi di lavoro e per soddisfare le aspettative degli utenti, abbiamo modificato la funzionalità del filtro nell’area Non assegnato. Ora puoi visualizzare solo le ore assegnate alle mansioni specificate nel filtro.

Prima di questo miglioramento, quando si applicava il filtro Mansione all’area Non assegnato, il Bilanciatore dei carichi di lavoro mostrava tutte le ore associate agli elementi di lavoro assegnati alle mansioni.

Per informazioni sul filtro delle informazioni nel Bilanciatore dei carichi di lavoro, vedere [Gestione dei filtri nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
