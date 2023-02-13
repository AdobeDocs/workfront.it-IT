---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica dell'attività Data inizio prevista
description: La data di inizio pianificata di un'attività è la data in cui, in qualità di creatore dell'attività, si decide che il lavoro sull'attività deve iniziare. Le date delle attività pianificate influenzano le date e la cronologia del progetto. Per informazioni sul progetto Data inizio pianificata, vedere Panoramica della data di inizio prevista del progetto.
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 2%

---

# Panoramica dell&#39;attività Data inizio prevista

La data di inizio pianificata di un&#39;attività è la data in cui, in qualità di creatore dell&#39;attività, si decide che il lavoro sull&#39;attività deve iniziare. Le date delle attività pianificate influenzano le date e la cronologia del progetto. Per informazioni sulla data di inizio prevista del progetto, consulta [Panoramica del progetto Data di inizio prevista](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## Data di inizio pianificata di un&#39;attività

È possibile specificare la data di inizio pianificata di un&#39;attività oppure lasciare ad Adobe Workfront il compito di calcolarla in base a determinati criteri. 

* [Impostare manualmente la data di inizio pianificata di un&#39;attività](#manually-set-the-planned-start-date-of-a-task)
* [Calcolo della data di inizio prevista per un&#39;attività](#how-the-planned-start-date-is-calculated-for-a-task)

### Impostare manualmente la data di inizio pianificata di un&#39;attività {#manually-set-the-planned-start-date-of-a-task}

L&#39;impostazione della data di inizio pianificata di un&#39;attività dipende dal tipo di Vincolo attività assegnato all&#39;attività. 

È possibile impostare manualmente la data di inizio pianificata durante la creazione di un&#39;attività, come descritto nell&#39;articolo [Creazione di attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

È possibile specificare manualmente la data di inizio pianificata quando si seleziona uno dei seguenti vincoli di attività: 

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
   <td> <p>Deve ininziare al</p> <p>Iniziare non Prima di</p> <p>Iniziare non Dopo di</p> </td> 
   <td> <p><span class="s1">La data di completamento pianificata viene modificata in modo da mantenere uguale la durata.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dati Fissi</p> </td> 
   <td> <p>La durata viene modificata in modo da mantenere uguale la data di completamento pianificata.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Calcolo della data di inizio prevista per un&#39;attività {#how-the-planned-start-date-is-calculated-for-a-task}

Quando viene calcolato automaticamente dal sistema, quanto segue può influenzare la Data di inizio pianificata di un&#39;attività:

* Impostazione della preferenza Data inizio nell&#39;area Attività e problemi in Configurazione

   L’amministratore di Workfront o di gruppo può determinare se una nuova attività viene avviata nella stessa data della data di inizio pianificata del progetto o nel giorno in cui viene creata l’attività.

   Per informazioni sulle preferenze Attività e problemi, consulta [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Vincolo attività

   Per ulteriori informazioni sui vincoli di attività, consulta l’articolo [Panoramica sul vincolo di attività](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)

* Relazione predecessore attività

   Per ulteriori informazioni sui predecessori delle attività, consulta l’articolo [Panoramica dei predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Data inizio progetto, quando il progetto è programmato dalla data di inizio.
* Tempo di programmazione dell&#39;assegnatario principale dell&#39;attività.

   Quando l&#39;Assegnatario principale ha un tempo di inattività programmato durante la durata dell&#39;attività, le date pianificate dell&#39;attività si adeguano di conseguenza quando il **Considerare il tempo di inattività dell&#39;utente nelle durate delle attività** è selezionata per **Ora di disattivazione utente** campo . I nuovi progetti ereditano questa impostazione dall’area Preferenze progetto , ma è possibile modificarla a livello di progetto.

   Ad esempio, se è previsto che un&#39;attività con un vincolo il più presto possibile inizi il 1° giugno e venga completata il 3 giugno, e il primo assegnatario principale contrassegni il 1° giugno per il timeout, l&#39;attività Data inizio pianificata diventerà il 2 giugno.

   Per informazioni sulla **Ora di disattivazione utente** preferenza, vedere gli articoli  [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) o [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

Quando viene impostata automaticamente, la data di inizio pianificata viene determinata in base al seguente calcolo: 

```
Planned Start Date = Planned Completion Date - Task Duration
```

Ad esempio, se l’attività ha una data di completamento del 16 settembre e una durata di 10 giorni, la data di inizio prevista è il 6 settembre.

>[!NOTE]
>
> Il tipo di aggiornamento del progetto deve essere impostato anche su &quot;Automatico e al momento della modifica&quot; o su &quot;Automatico&quot; affinché le ore e la durata previste vengano regolate automaticamente.\
Per ulteriori informazioni sul tipo di aggiornamento, consulta l’articolo [Seleziona il tipo di aggiornamento del progetto](../../../manage-work/projects/manage-projects/select-project-update-type.md).
