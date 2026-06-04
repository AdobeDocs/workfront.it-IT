---
product-area: projects
navigation-topic: issue-information
title: Panoramica della data di completamento del problema pianificata
description: La Data di completamento pianificata di un problema è la data entro la quale si prevede che il problema venga completato.
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
TQID: https://experienceleague.adobe.com/WodCHwmu7JYCZKdoqoJ6W88AP0xzlZ-Jglj5zxD8-6g
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 595
ht-degree: 1%

---

# Panoramica della data di completamento pianificata del problema

<!--Audited: 08/2025-->

La Data di completamento pianificata di un problema è la data entro la quale si prevede che il problema venga completato.

Puoi specificare la Data di completamento pianificata di un problema oppure lasciare che sia Adobe Workfront a calcolarla in base a determinati criteri.

Le Date di completamento pianificate dei problemi non influiscono sulla Data di completamento pianificata del progetto. Solo le date di completamento pianificate delle attività influiscono sulla data di completamento pianificata del progetto. Per ulteriori informazioni sulla data di completamento pianificata del progetto, vedere [Impostare la data di completamento pianificata del progetto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>La Data di completamento pianificata di un problema differisce dalla Data di impegno del problema o dalla Data di completamento prevista del problema nei seguenti modi:
>
>* La Data impegno è la data entro la quale la persona assegnata all’emissione stima manualmente che avrà completato l’emissione. Per ulteriori informazioni, consulta i seguenti articoli:
>
>   * [Panoramica sulla data di conferma](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [Interazioni tra la data di conferma e la data di completamento pianificata](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* La data di completamento prevista è una data calcolata da Workfront che prende in considerazione fattori esterni per determinare una data reale per il completamento realistico del problema. Per ulteriori informazioni, vedere [Panoramica della data di completamento prevista per progetti, attività e problemi](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## Impostare manualmente la Data di completamento pianificata di un problema

Per poter aggiornare la Data di completamento pianificata del problema, è necessario disporre dell’accesso in Modifica ai problemi e delle autorizzazioni di Gestione sul problema.

Puoi impostare manualmente la Data di completamento pianificata di un problema nelle seguenti aree di Workfront:

* Nella casella Modifica problema o nell’area Dettagli problema durante la creazione o la modifica di un problema. Per informazioni, vedere [Modifica problemi](../../../manage-work/issues/manage-issues/edit-issues.md).
* Nell’area Home se la Data di completamento pianificata viene visualizzata nel pannello Riepilogo di un problema. Per informazioni, vedere [Aggiornare o modificare un elemento di lavoro nell&#39;area Home](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* Nell’intestazione del problema. Per informazioni, vedere [Nuove intestazioni oggetto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* In un elenco o in un rapporto di problemi quando il campo Data di completamento pianificata viene visualizzato nella vista.

  Per informazioni, vedere [Modifica problemi in un elenco](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Come Workfront calcola automaticamente la Data di completamento pianificata per un problema

Quando Workfront calcola automaticamente la Data di completamento pianificata di un problema, i seguenti elementi possono influenzare la data:

* Data di inizio pianificata

  La Data di ingresso e la Data di inizio pianificata devono corrispondere su un problema quando crei il problema per la prima volta.

* La durata predefinita configurata nella sezione Dettagli coda del progetto. Per informazioni, vedere [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

  Se la durata predefinita è 0 giorni, la data di completamento pianificata corrisponde alla data di inizio pianificata del problema.

* Pianificazione progetto

Quando viene impostata automaticamente, la Data di completamento pianificata viene determinata in base al seguente calcolo:

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**Esempio:** Ad esempio, se l&#39;attività ha una data di inizio venerdì 14 gennaio e la durata predefinita è di 5 giorni, la data di completamento pianificata è venerdì 21 gennaio, se la pianificazione del progetto è lunedì-venerdì per 8 ore al giorno.

Esistono le seguenti situazioni:

* Se il progetto non dispone di una pianificazione, viene presa in considerazione la pianificazione predefinita del sistema Workfront. Per informazioni, vedere [Panoramica sugli Schedules](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).
* Se la pianificazione è da lunedì a venerdì dalle 9 alle 13 (4 ore al giorno) e l&#39;orario di lavoro tipico del sistema Workfront è di 8 ore, la data di completamento pianificata è il 27 gennaio.

>[!TIP]
>
>Workfront prende in considerazione le eccezioni alla pianificazione come festività e fine settimana nel calcolo delle date di completamento pianificate.


