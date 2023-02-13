---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica dell'attività Data completamento pianificata
description: La data di completamento pianificata di un'attività corrisponde alla data in cui l'attività viene impostata per essere completata.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 1%

---

# Panoramica dell&#39;attività Data completamento pianificata

La data di completamento pianificata di un&#39;attività corrisponde alla data in cui l&#39;attività viene impostata per essere completata.

È possibile specificare la data di completamento pianificata di un&#39;attività oppure lasciare che sia possibile calcolarla in base a determinati criteri in Adobe Workfront. 

Le date di completamento pianificate delle attività di un progetto determinano la data di completamento pianificato di un progetto quando il progetto viene programmato dalla data di inizio. Per ulteriori informazioni sulla data di completamento pianificata del progetto, vedere [Imposta la data di completamento pianificato del progetto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>La data di completamento pianificata di un&#39;attività è diversa dalla data di commit dell&#39;attività o dalla data di completamento prevista dell&#39;attività nei seguenti modi:
>
>* La data di commit è la data in cui la persona assegnata all&#39;attività stima manualmente che avrà completato l&#39;attività. Per ulteriori informazioni, consulta i seguenti articoli:
   * [Panoramica sulla data del commit](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
   * [Interazioni tra la data di commit e la data di completamento pianificata](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
* La data di completamento prevista è una data calcolata da Workfront e tiene conto dei ritardi nell’attività, delle timeline dell’attività o dei relativi predecessori e di altri fattori per determinare una data di vita reale in cui l’attività può essere completata in modo realistico. Per ulteriori informazioni, consulta [Panoramica della data di completamento prevista per progetti, attività e problemi](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>


## Impostare manualmente la data di completamento pianificata di un&#39;attività

Per poter aggiornare la data di completamento pianificata dell&#39;attività, è necessario disporre dell&#39;accesso Modifica alle attività e delle autorizzazioni Gestione per l&#39;attività.

L&#39;impostazione della data di completamento pianificata di un&#39;attività dipende dal tipo di Vincolo attività assegnato all&#39;attività. 

È possibile impostare manualmente la data di completamento pianificata nelle seguenti aree di Workfront:

* Nella casella Modifica attività, durante la creazione o la modifica di un’attività. Per informazioni, consulta [Modifica delle attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* Nell’area Dettagli attività. Per informazioni, consulta [Gestire le informazioni sulle attività nell&#39;area Panoramica dettagli attività](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* Nell&#39;area Home se viene visualizzata la data di completamento pianificata durante la visualizzazione di un&#39;attività. Per informazioni, consulta [Aggiornare o modificare un elemento di lavoro nell&#39;area Home](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* Nell’intestazione dell’attività. Per informazioni, consulta [Nuove intestazioni oggetto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* In un elenco di attività o in un rapporto quando il campo Data completamento pianificato viene visualizzato nella visualizzazione.

   Per informazioni, consulta [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

È possibile specificare manualmente la data di completamento pianificata quando si seleziona uno dei seguenti vincoli task: 

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tipo di vincolo attività</strong> </p> </th> 
   <th> <p><strong>Effetto della modifica manuale della data di completamento pianificata</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Deve Finire al</p> <p>Finire non Dopo di</p> <p>Finire non Prima di</p> </td> 
   <td> <p><span class="s1">La data di inizio pianificata viene modificata in modo da mantenere uguale la durata.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dati Fissi</p> </td> 
   <td> <p>La durata viene modificata in modo da mantenere uguale la data di inizio pianificata.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modalità di calcolo automatico della data di completamento pianificata per un&#39;attività da parte di Workfront

Quando viene calcolato automaticamente dal sistema, quanto segue può influenzare la Data di completamento pianificata di un&#39;attività:

* Vincolo attività

   Per ulteriori informazioni sui vincoli di attività, consulta l’articolo [Panoramica sul vincolo di attività](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Relazione predecessore attività

   Per ulteriori informazioni sui predecessori delle attività, consulta l’articolo [Panoramica dei predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Data completamento progetto, quando il progetto è programmato da Data completamento.
* Tempo di programmazione dell&#39;assegnatario principale dell&#39;attività.

   Quando l&#39;Assegnatario principale ha un tempo di inattività programmato durante la durata dell&#39;attività, le date pianificate dell&#39;attività si adeguano di conseguenza quando il **Considerare il tempo di inattività dell&#39;utente nelle durate delle attività** è selezionata per **Ora di disattivazione utente** campo . I nuovi progetti ereditano questa impostazione dall’area Preferenze progetto , ma è possibile modificarla a livello di progetto.

   Ad esempio, se un&#39;attività con un Vincolo il più presto possibile viene pianificata per l&#39;inizio il 1° giugno e completa il 3 giugno e l&#39;Assegnatario principale ha contrassegnato il 2 giugno per il Time-off, l&#39;attività Data completamento pianificato diventa il 4 giugno.

   Per informazioni sulla **Ora di disattivazione utente** preferenza, vedere gli articoli [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) o [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

* Il tempo associato alle impostazioni di approvazione se l&#39;attività è associata a un&#39;approvazione. Per ulteriori informazioni, consulta [Configurare le impostazioni di approvazione globali](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

Se impostata automaticamente, la data di completamento pianificata viene determinata in base al seguente calcolo: 

```
Planned Completion Date = Planned Start Date + Duration
```

Ad esempio, se l’attività ha una data di inizio del 16 settembre e una durata di 10 giorni, la data di completamento pianificata è il 26 settembre.

>[!NOTE]
 Il tipo di aggiornamento per il progetto deve essere impostato su Automatico e Al momento della modifica o Automaticamente affinché le ore e la durata previste vengano regolate automaticamente.\
Per ulteriori informazioni sul tipo di aggiornamento, consulta l’articolo [Seleziona il tipo di aggiornamento del progetto](../../../manage-work/projects/manage-projects/select-project-update-type.md).
