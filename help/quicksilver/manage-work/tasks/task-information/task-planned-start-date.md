---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica della data di inizio pianificata dell'attività
description: La data di inizio pianificata di un'attività è la data in cui l'autore dell'attività decide che il lavoro sull'attività deve iniziare. Le date delle attività pianificate influiscono sulle date e sulla sequenza temporale del progetto. Per informazioni sulla data di inizio pianificata del progetto, vedere Panoramica della data di inizio pianificata del progetto.
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 2%

---

# Panoramica della data di inizio pianificata dell&#39;attività

<!-- Audited: 6/2025 -->

La data di inizio pianificata di un&#39;attività è la data in cui l&#39;autore dell&#39;attività decide che il lavoro sull&#39;attività deve iniziare. Le date delle attività pianificate influiscono sulle date e sulla sequenza temporale del progetto. Per informazioni sulla Data inizio pianificata del progetto, vedere [Panoramica della Data inizio pianificata del progetto](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## Data di inizio pianificata di un&#39;attività

È possibile specificare la data di inizio pianificata dell&#39;attività oppure lasciare che sia Adobe Workfront a calcolarla in base a determinati criteri.

* [Impostare manualmente la data di inizio pianificata di un&#39;attività](#manually-set-the-planned-start-date-of-a-task)
* [Calcolo della data di inizio pianificata per un&#39;attività](#how-the-planned-start-date-is-calculated-for-a-task)

### Impostare manualmente la data di inizio pianificata di un&#39;attività {#manually-set-the-planned-start-date-of-a-task}

L&#39;impostazione della data di inizio pianificata di un&#39;attività dipende dal tipo di vincolo attività assegnato all&#39;attività.

È possibile impostare manualmente la Data inizio pianificata durante la creazione di un&#39;attività. Per ulteriori informazioni, vedere [Creare attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

È possibile specificare manualmente la Data inizio pianificata quando si seleziona uno dei seguenti vincoli di task:

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
   <td> <p><span class="s1">La data di completamento pianificata viene modificata per mantenere la durata invariata.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dati Fissi</p> </td> 
   <td> <p>La Durata viene adeguata in modo da mantenere la stessa Data di completamento pianificata.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Calcolo della data di inizio pianificata per un&#39;attività {#how-the-planned-start-date-is-calculated-for-a-task}

Quando viene calcolato automaticamente dal sistema, le seguenti operazioni possono influenzare la Data inizio pianificata di un&#39;attività:

* Impostazione della preferenza Data di inizio nell&#39;area Attività e problemi in Configurazione

  L&#39;amministratore del Workfront o del gruppo può determinare se una nuova attività inizia nella stessa data della data di inizio pianificata del progetto o nel giorno in cui viene creata.

  Per informazioni sulle preferenze per attività e problemi, vedere [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Vincolo attività

  Per ulteriori informazioni sui vincoli attività, vedere [Panoramica sui vincoli attività](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Relazione predecessore attività

  Per ulteriori informazioni sui predecessori delle attività, vedere [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Data di inizio progetto, quando il progetto è programmato dalla Data di inizio.
* L&#39;indisponibilità programmata dell&#39;assegnatario principale dell&#39;attività.

  Quando l&#39;assegnatario principale ha un&#39;indisponibilità programmata durante la durata dell&#39;attività, le date pianificate dell&#39;attività vengono modificate di conseguenza quando per il campo Indisponibilità utente viene selezionata l&#39;impostazione Considera indisponibilità utente durante l&#39;attività. I nuovi progetti ereditano questa impostazione dall’area Preferenze progetto, ma è possibile modificarla a livello di progetto.

  Ad esempio, se un&#39;attività con un vincolo Il più presto possibile è programmata per iniziare il 1° giugno e completare il 3 giugno e l&#39;assegnatario principale ha il 1° giugno contrassegnato per l&#39;indisponibilità, la data di inizio pianificata dell&#39;attività diventa il 2 giugno.

  Per informazioni sulla preferenza Indisponibilità utente, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) o [Modificare i progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

Quando viene impostata automaticamente, la Data inizio pianificata viene determinata in base al seguente calcolo:

```
Planned Start Date = Planned Completion Date - Task Duration
```

Ad esempio, se l&#39;attività ha una data di completamento del 16 settembre e una durata di 10 giorni, la data di inizio pianificata è il 6 settembre.

>[!NOTE]
>
> Per poter regolare automaticamente le ore e la durata pianificate, il Tipo di aggiornamento per il progetto deve essere impostato anche su Automatico e su In modifica o Automaticamente.\
>Per ulteriori informazioni sul tipo di aggiornamento, vedere [Selezionare il tipo di aggiornamento del progetto](../../../manage-work/projects/manage-projects/select-project-update-type.md).
