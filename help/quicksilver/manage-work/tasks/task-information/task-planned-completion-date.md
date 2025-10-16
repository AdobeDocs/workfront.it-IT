---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica della data di completamento pianificata dell’attività
description: La data di completamento pianificata di un'attività è la data entro la quale l'attività è impostata per il completamento.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 1%

---

# Panoramica della data di completamento pianificata dell&#39;attività

La data di completamento pianificata di un&#39;attività è la data entro la quale l&#39;attività è impostata per il completamento.

È possibile specificare la data di completamento pianificata di un&#39;attività oppure lasciare che sia Adobe Workfront a calcolarla in base a determinati criteri.

Le date di completamento pianificate delle attività di un progetto determinano la data di completamento pianificata di un progetto quando il progetto è programmato dalla data di inizio. Per ulteriori informazioni sulla data di completamento pianificata del progetto, vedere [Impostare la data di completamento pianificata del progetto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>La data di completamento pianificata di un&#39;attività differisce dalla data di commit dell&#39;attività o dalla data di completamento prevista dell&#39;attività nei modi seguenti:
>
>* La Data conferma è la data entro la quale la persona assegnata all&#39;attività calcola manualmente che avrà completato l&#39;attività. Per ulteriori informazioni, consulta i seguenti articoli:
>
>   * [Panoramica sulla data di conferma](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [Interazioni tra la data di conferma e la data di completamento pianificata](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* La data di completamento prevista è una data calcolata da Workfront e tiene conto dei ritardi dell&#39;attività, delle tempistiche dell&#39;attività o dei suoi predecessori e di altri fattori per determinare una data reale in cui l&#39;attività può essere completata in modo realistico. Per ulteriori informazioni, vedere [Panoramica della data di completamento prevista per progetti, attività e problemi](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## Impostare manualmente la data di completamento pianificata di un&#39;attività

Per poter aggiornare la data di completamento pianificata dell&#39;attività, è necessario disporre dell&#39;accesso di modifica alle attività e delle autorizzazioni di gestione per l&#39;attività.

L&#39;impostazione della Data di completamento pianificata di un&#39;attività dipende dal tipo di Vincolo attività assegnato all&#39;attività.

Puoi impostare manualmente la Data di completamento pianificata nelle seguenti aree di Workfront:

* Nella casella Modifica attività, durante la creazione o la modifica di un&#39;attività. Per informazioni, vedere [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* Nell&#39;area Dettagli attività. Per informazioni, vedere [Informazioni sulla gestione delle attività nell&#39;area Panoramica dettagli attività](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* Nell&#39;area Home, se la Data di completamento pianificata viene visualizzata quando si visualizza un&#39;attività nel pannello Riepilogo. Per informazioni, vedere [Aggiornare o modificare un elemento di lavoro nell&#39;area Home](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* Nell&#39;intestazione dell&#39;attività. Per informazioni, vedere [Nuove intestazioni oggetto](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* In un elenco di attività o in un report quando nella visualizzazione viene visualizzato il campo Data di completamento pianificata.

  Per informazioni, vedere [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

È possibile specificare manualmente la Data di completamento pianificata quando si seleziona uno dei seguenti Vincoli attività:

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
   <td> <p>Deve essere completato il</p> <p>Completa entro e non oltre</p> <p>Completa non prima di</p> </td> 
   <td> <p><span class="s1">La data di inizio pianificata viene modificata per mantenere la durata invariata.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dati Fissi</p> </td> 
   <td> <p>La Durata viene modificata in modo da mantenere la stessa Data di Inizio Pianificata.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Calcolo automatico della data di completamento pianificata per un&#39;attività in Workfront

Quando viene calcolato automaticamente dal sistema, i seguenti elementi possono influenzare la Data di completamento pianificata di un&#39;attività:

* Vincolo attività

  Per ulteriori informazioni sui vincoli attività, vedere l&#39;articolo [Panoramica sui vincoli attività](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Relazione predecessore attività

  Per ulteriori informazioni sui predecessori delle attività, vedere l&#39;articolo [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Data di completamento progetto, quando il progetto è programmato dalla Data di completamento.
* L&#39;indisponibilità della programmazione dell&#39;assegnatario principale dell&#39;attività.

  Quando l&#39;assegnatario principale ha un&#39;indisponibilità programmata durante la durata dell&#39;attività, le date pianificate dell&#39;attività vengono modificate di conseguenza quando per il campo **Indisponibilità utente** è selezionata l&#39;impostazione **Considera indisponibilità utente nelle durate dell&#39;attività**. I nuovi progetti ereditano questa impostazione dall’area Preferenze progetto, ma è possibile modificarla a livello di progetto.

  Ad esempio, se un&#39;attività con un vincolo Il più presto possibile è programmata per iniziare il 1° giugno e completare il 3 giugno e l&#39;assegnatario principale ha il 2 giugno contrassegnato per l&#39;indisponibilità, la data di completamento pianificata dell&#39;attività diventa il 4 giugno.

  Per informazioni sulla preferenza **Indisponibilità utente**, consulta gli articoli [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) o [Modificare i progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

* Quantità di tempo associata alle impostazioni di approvazione se l&#39;attività è associata a un&#39;approvazione. Per ulteriori informazioni, vedere [Configurare le impostazioni di approvazione globali](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

Quando viene impostata automaticamente, la Data di completamento pianificata viene determinata in base al seguente calcolo:

```
Planned Completion Date = Planned Start Date + Duration
```

Ad esempio, se l&#39;attività ha una data di inizio il 16 settembre e una durata di 10 giorni, la data di completamento pianificata è il 26 settembre.

>[!NOTE]
>
> Per poter regolare automaticamente le ore e la durata pianificate, il Tipo di aggiornamento per il progetto deve essere impostato su Automatico e su In modifica o Automaticamente.\
>Per ulteriori informazioni sul tipo di aggiornamento, vedere l&#39;articolo [Selezionare il tipo di aggiornamento del progetto](../../../manage-work/projects/manage-projects/select-project-update-type.md).
