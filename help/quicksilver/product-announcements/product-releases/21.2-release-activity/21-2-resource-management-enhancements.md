---
content-type: release-notes
keywords: note, trimestrale, aggiornamento, versione
navigation-topic: 2021-2-release-activity
title: 21.2 Miglioramenti alla gestione delle risorse
description: Questa pagina descrive tutti i miglioramenti apportati alla gestione delle risorse con la versione 21.2 nell’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell'ambiente di produzione la settimana del 10 maggio 2021. Per un elenco di tutte le modifiche disponibili con la versione 21.2, consulta Panoramica sulla versione 21.2.
author: Luke
feature: Product Announcements
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# 21.2 Miglioramenti alla gestione delle risorse

Questa pagina descrive tutti i miglioramenti apportati alla gestione delle risorse con la versione 21.2 nell’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione la settimana del 10 maggio 2021. Per un elenco di tutte le modifiche disponibili con la versione 21.2, vedi [Panoramica sulla versione 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Visualizzazione a livello di mese nel bilanciamento del carico di lavoro

Per aiutarti a gestire l’allocazione delle risorse per periodi di tempo più lunghi, ora abbiamo implementato una visualizzazione a livello di mese per il servizio di bilanciamento del carico di lavoro. È possibile visualizzare fino a tre mesi alla volta e aggiornare le allocazioni di risorse mensili. Prima di questa modifica, era possibile visualizzare il servizio di bilanciamento del carico di lavoro solo per giorno o settimana.

Per informazioni, consulta [Naviga nel bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Connessione tra il Planner scenario, il bilanciamento del carico di lavoro e l&#39;elenco delle attività

>[!NOTE]
>
>Disponibile solo nella nuova esperienza Adobe Workfront.

Per facilitare la pianificazione strategica dei progetti e garantire che siano allineati alle iniziative con un quadro più ampio del Planner scenario, abbiamo creato una nuova area sul progetto che mostra i requisiti del ruolo di lavoro dalle iniziative e le ore pianificate stimate sugli elementi di lavoro del progetto. Quest’area è disponibile per il servizio di bilanciamento del carico di lavoro a livello di progetto e per l’elenco delle attività nella nuova esperienza Workfront. Nell’esperienza classica, questa opzione è disponibile solo per il servizio di bilanciamento del carico di lavoro del progetto.

Per informazioni, vedi i seguenti articoli:

* [Panoramica sulla riconciliazione delle assegnazioni di risorse tra progetti e iniziative](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [Naviga nel bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Questa nuova funzionalità è visibile a tutti gli utenti, sia nella nuova che nell’esperienza classica di Workfront. Questo è visibile anche ai clienti che non hanno acquistato una licenza Workfront Scenario Planner .

## Utilizzare le ore pianificate per calcolare i valori netti nel planner risorse

Una nuova impostazione nel Planner risorse consente di utilizzare Orari pianificati per il calcolo dei valori netti.

Prima di questo miglioramento, i valori netti calcolati da Workfront si basano solo su ore a budget. I valori netti mostrano la differenza tra le ore disponibili e in budget o pianificate, FTE o costo. L&#39;impostazione predefinita per il calcolo dei valori netti rimane l&#39;ora a budget.

Per informazioni, consulta [Panoramica delle informazioni su ore, FTE e costi nelle visualizzazioni Progetto e Ruolo del Planner risorse](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Visualizzazione di 12 settimane nel servizio di bilanciamento del carico di lavoro

Ora puoi visualizzare fino a 12 settimane di informazioni nel servizio di bilanciamento del carico di lavoro. Prima di questo miglioramento, era possibile visualizzare 2,4 e 6 settimane di informazioni.

Per informazioni sulla visualizzazione del servizio di bilanciamento del carico di lavoro, vedi [Naviga nel bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)Naviga nel servizio di bilanciamento del carico di lavoro.

## Modifica del modo in cui il filtro Ruolo lavoro funziona nell&#39;area Non assegnata del bilanciamento del carico di lavoro

Per migliorare il modo in cui il filtro Ruolo lavoro funziona nel bilanciamento del carico di lavoro e per soddisfare le aspettative degli utenti, abbiamo modificato la funzionalità del filtro nell’area Non assegnato. È ora possibile visualizzare solo le ore assegnate ai ruoli di lavoro specificati nel filtro.

Prima di questo miglioramento, quando si applica il filtro Ruolo lavoro all&#39;area Non assegnata, il servizio di bilanciamento del carico di lavoro visualizzava tutte le ore associate agli elementi di lavoro assegnati ai ruoli del lavoro .

Per informazioni sul filtro delle informazioni nel servizio di bilanciamento del carico di lavoro, consulta [Gestire i filtri nel servizio di bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
