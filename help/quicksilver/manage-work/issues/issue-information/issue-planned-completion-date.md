---
product-area: projects
navigation-topic: issue-information
title: Panoramica del problema Data di completamento pianificata
description: La data di completamento pianificata di un problema è la data in cui il problema deve essere completato.
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Panoramica del problema Data di completamento pianificata

La data di completamento pianificata di un problema è la data in cui il problema deve essere completato.

È possibile specificare la data di completamento pianificata di un problema oppure lasciare che sia Adobe Workfront a calcolarlo in base a determinati criteri. 

Le date di completamento pianificate dei problemi non influiscono sulla data di completamento pianificata del progetto. Solo le date di completamento pianificate delle attività influiscono sulla data di completamento pianificata del progetto. Per ulteriori informazioni sulla data di completamento pianificata del progetto, vedere [Imposta la data di completamento pianificato del progetto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>La data di completamento pianificata di un problema è diversa dalla data di commit del problema o dalla data di completamento prevista del problema nei seguenti modi:
>
>* La data di commit è la data in cui la persona assegnata al problema stima manualmente che avrà completato il problema. Per ulteriori informazioni, consulta i seguenti articoli:
   * [Panoramica sulla data del commit](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
   * [Interazioni tra la data di commit e la data di completamento pianificata](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
* La data di completamento prevista è una data calcolata da Workfront che tiene conto di fattori esterni per determinare una data di completamento realistico del problema. Per ulteriori informazioni, consulta [Panoramica della data di completamento prevista per progetti, attività e problemi](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>


## Impostare manualmente la data di completamento pianificata di un problema

Per poter aggiornare la data di completamento pianificata del problema, è necessario disporre dell&#39;accesso Modifica ai problemi e delle autorizzazioni Gestione.

Puoi impostare manualmente la data di completamento pianificata di un problema nelle seguenti aree di Workfront:

* Nella casella Modifica problema o nell&#39;area Dettagli problema durante la creazione o la modifica di un problema. Per informazioni, consulta [Modifica dei problemi](../../../manage-work/issues/manage-issues/edit-issues.md).
* Nell&#39;area Home se viene visualizzata la data di completamento pianificata durante la visualizzazione di un problema. Per informazioni, consulta [Aggiornare o modificare un elemento di lavoro nell&#39;area Home](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* Nell’intestazione del problema. Per informazioni, consulta [Nuove intestazioni oggetto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* In un elenco di problemi o in un rapporto quando il campo Data completamento pianificata viene visualizzato nella visualizzazione.

   Per informazioni, consulta [Modificare i problemi in un elenco](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## In che modo Workfront calcola automaticamente la data di completamento pianificata per un problema

Quando Workfront calcola automaticamente la data di completamento pianificata di un problema, la data può essere influenzata da quanto segue:

* Data di inizio prevista

   La data di ingresso e la data di inizio pianificata devono corrispondere a un problema alla prima creazione del problema.

* La durata predefinita configurata nella sezione Dettagli coda del progetto. Per informazioni, consulta [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Se la durata predefinita è pari a 0 giorni, la data di completamento pianificata corrisponde alla data di inizio pianificata del problema.

* Pianificazione del progetto

Se impostata automaticamente, la data di completamento pianificata viene determinata in base al seguente calcolo: 

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**Esempio:** Ad esempio, se l’attività ha una data di inizio di venerdì, 14 gennaio e la durata predefinita è di 5 giorni, la data di completamento pianificata è venerdì 21 gennaio se la pianificazione del progetto è dal lunedì al venerdì per 8 ore al giorno.

Esistono le seguenti situazioni:

* Se il progetto non dispone di una pianificazione, viene presa in considerazione la pianificazione predefinita del sistema Workfront. Per informazioni, consulta [Panoramica sulle pianificazioni](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).
* Se l&#39;orario è dal lunedì al venerdì dalle 9 alle 13 (4 ore al giorno) e il numero di ore tipiche del sistema Workfront per giorno lavorativo è di 8 ore, la data di completamento pianificata è il 27 gennaio.

>[!TIP]
Workfront tiene conto delle eccezioni di pianificazione, come le festività e i fine settimana, durante il calcolo delle date di completamento pianificate.

 
