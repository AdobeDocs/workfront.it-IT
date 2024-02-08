---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica sulla percentuale di completamento del progetto
description: Il valore percentuale di completamento di un progetto viene calcolato in base alla durata pianificata o alle ore pianificate delle attività del progetto. L’amministratore di Adobe Workfront o un amministratore di gruppo definisce quale valore viene preso in considerazione per calcolare la percentuale di completamento nel sistema quando configura le informazioni nell’area Preferenze progetto. Per informazioni sulla configurazione delle preferenze di progetto, consulta Configurare le preferenze di progetto a livello di sistema.
author: Alina
feature: Work Management
exl-id: d2395569-9fe5-42e7-a392-cff49eb519d9
source-git-commit: 816fd70642ffb7b24095602ce160421aa947e2a6
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 0%

---

# Panoramica sulla percentuale di completamento del progetto

<!-- Audited 01/2024 -->

Il valore Percentuale completamento di un progetto viene calcolato in base alla Durata o alle Ore pianificate delle attività del progetto. L’amministratore di Adobe Workfront o un amministratore di gruppo definisce quale valore viene preso in considerazione per calcolare la percentuale di completamento nel sistema quando configura le informazioni nell’area Preferenze progetto.

Per informazioni sulla configurazione delle preferenze del progetto, consulta [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

La percentuale di completamento di un&#39;attività padre si basa sulla durata o sulle ore pianificate di ciascuna delle relative sottoattività.

Analogamente, la percentuale di completamento di un progetto si basa sulle durate o sulle ore pianificate di ogni attività principale del progetto.

Le attività principali sono le attività padre e le attività autonome che non hanno elementi figlio.

>[!TIP]
>
>Le attività principali non sono rientrate in un piano di progetto.

## Come Workfront calcola la percentuale di completamento

### Aggiornare la percentuale di completamento di un&#39;attività {#update-the-percent-complete-on-a-task}

È possibile modificare manualmente la percentuale di completamento di un&#39;attività. Questo non è un calcolo.

Workfront utilizza la percentuale di completamento di una singola attività per calcolare la percentuale di completamento della relativa attività padre o la percentuale di completamento del progetto.

Per informazioni sull&#39;aggiornamento della percentuale di completamento di un&#39;attività, vedere [Visualizza e aggiorna la percentuale di completamento per le attività](../../../manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

### Come Workfront calcola la percentuale di completamento di un&#39;attività padre {#how-workfront-calculates-percent-complete-on-a-parent-task}

A seconda dell&#39;opzione selezionata dall&#39;amministratore del Workfront o del gruppo nelle Preferenze progetto a livello di sistema o di gruppo, la percentuale di completamento per un&#39;attività padre viene calcolata in base alla Durata o alle Ore pianificate delle attività.

Considera i seguenti scenari:

* Se il sistema calcola la percentuale di completamento in base alle ore pianificate, la percentuale di completamento dell&#39;attività padre viene calcolata utilizzando la formula seguente:

  `Parent Task Percent Complete = (((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of Parent)*100`

  Le ore pianificate totali del padre rappresentano la somma di tutte le ore pianificate di ciascuno dei figli.

  ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

* Se il sistema calcola la percentuale di completamento in base alla durata, la percentuale di completamento dell&#39;attività padre viene calcolata utilizzando la formula seguente:

  `Parent Task Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/ Total Duration of Parent)*100`

  ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

  >[!IMPORTANT]
  >
  >La durata totale dell&#39;attività padre è il totale di tutte le durate delle attività figlio. Ad esempio, un&#39;attività padre con due figli con una rispettiva durata di 1 giorno e 2 giorni ha una durata totale di 3 giorni, anche quando i due figli possono iniziare nello stesso giorno.


### Come Workfront calcola la percentuale di completamento di un progetto {#how-workfront-calculates-percent-complete-on-a-project}

A seconda di ciò che il Workfront o l&#39;amministratore di gruppo hanno selezionato nelle Preferenze del progetto a livello di sistema o di gruppo, la percentuale di completamento per un progetto viene calcolata in base alla Durata o alle Ore pianificate delle attività principali del progetto.

* Se il sistema calcola la percentuale di completamento in base alle ore pianificate, la percentuale di completamento del progetto viene calcolata utilizzando la seguente formula:

  `Project Percent Complete =(((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of the Project)*100`

  Le ore pianificate totali del progetto corrispondono alla somma delle ore pianificate di tutte le attività principali del progetto.

  ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

  >[!NOTE]
  >
  >Il task 1 o il task 2 può essere solo padre o autonomo. Le ore pianificate e la percentuale di completamento delle attività figlio non vengono utilizzate in questo calcolo.

* Se il sistema calcola la percentuale di completamento in base alla durata, la percentuale di completamento del progetto viene calcolata utilizzando la formula seguente:

  `Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

  >[!IMPORTANT]
  >
  >La durata del progetto è il totale di tutte le durate delle attività principali che presentano una percentuale di completamento. Ad esempio, un progetto con un&#39;attività autonoma con una durata di 2 giorni e un&#39;attività padre con una durata di 5 giorni per cui è stato completato il lavoro avrà una durata totale di 7 giorni, anche se le due attività possono iniziare nello stesso giorno.

  ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

  >[!NOTE]
  >
  >Il task 1 o il task 2 può essere solo padre o autonomo. Le attività Durata e Percentuale completamento delle attività figlio non vengono utilizzate in questo calcolo.

## Esempio di percentuale di completamento di un progetto utilizzando la durata

Quando utilizzi la Durata delle attività per calcolare la percentuale di completamento di un progetto, considera l’esempio seguente:

![](assets/project-with-tasks-percent-complete-duration-calculation.png)

Le seguenti informazioni vengono utilizzate per calcolare la percentuale di completamento del progetto

* Percentuale di completamento dell&#39;attività autonoma (Attività 1 - 20%)
* La percentuale di completamento dell&#39;attività padre (Attività 2 - 25%)
* Durata dell&#39;attività 1 (5 giorni)
* Durata dell&#39;attività 2 (2 giorni)
* Durata del progetto (7 giorni)


Per calcolare la percentuale di completamento del progetto utilizzando la durata:

`Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

Oppure

`(((5*0.2)+(2*0.25))/7)*100= 21.43%`


<!--drafted, this was the old example:

When using the Planned Duration of the tasks to calculate the percent complete of a project, consider the following example:

percent_complete_on_project_example.png

Only the parent task (Task 1) and the standalone task (Task 8) are used to calculate the percent complete of the project.

The secondary parents of Task 1 are used to calculate the percent complete of the main parent (Task 1).

To calculate the percent complete of the main parent (Task 1), first calculate the percent complete of its secondary parents:

Task 5 Percent Complete = ((14 * 0.75 + 12 * 0.25)/(12 + 14))*100 = 51.92%

Task 2 Percent Complete = ((5 * 0.7 + 2 * 0.5)/(5 + 2))*100 = 64.29 %

Then, to calculate the percent complete of the main parent (Task 1), use the following formula:

Task 1 Percent Complete =((56 * 0.5192 + 7 * 0.6429)/63)*100 = 53.29%

To calculate the percent complete of the project, you will need to have the following numbers ready:

Task 1 Duration (63 hours) and Percent Complete (53.29%)
Task 8 Duration (100 hours) and Percent Complete (4%)
Now, to calculate the percent complete of the project, use the following formula:

Project Percent Complete =((100 * 0.04 + 63 * 0.5329))/163)*100 = 23.05%
-->