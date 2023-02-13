---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Panoramica della durata del progetto
description: Adobe Workfront calcola la durata di un progetto tenendo conto della data di inizio del primo task e della data di completamento dell'ultimo task e del numero di giorni tra le due date.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 2%

---

# Panoramica della durata del progetto

Adobe Workfront calcola la durata di un progetto tenendo conto della data di inizio del primo task e della data di completamento dell&#39;ultimo task e del numero di giorni tra le due date.

## Durata progetto

La durata del progetto è calcolata con la seguente formula:

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>La durata dei problemi relativi al progetto non influisce sulla durata del progetto.

La durata del progetto conta il numero di giorni tra le due date delle attività in base alla pianificazione associata al progetto o agli utenti assegnati alle attività. Per informazioni sulla pianificazione utilizzata da Workfront per calcolare la durata, consulta [Panoramica sulle pianificazioni](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).

## Tipi di durata del progetto

Esistono due tipi di Durata del progetto e le formule in base alle quali Workfront le calcola:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **Durata Pianificata**: 

   ```
   Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
   ```

* **Durata Reale**: 

   ```
   Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
   ```

## Individua la durata del progetto

È possibile individuare le durate pianificate e effettive del progetto nelle seguenti aree di Workfront:

* . Nell’area Dettagli progetto, nella sezione Panoramica .

   Per ulteriori informazioni sulla sottoscheda Panoramica di un progetto, consulta l’articolo [Gestire le informazioni nell’area Panoramica del progetto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* In un rapporto Progetto, includendo i campi Durata o Durata effettiva nel rapporto.

   Per ulteriori informazioni sulla creazione di rapporti, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
