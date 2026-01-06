---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Panoramica della durata del progetto
description: Adobe Workfront calcola la durata di un progetto tenendo conto della data di inizio della prima attività e della data di completamento dell'attività più recente e conta il numero di giorni tra le due date.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Panoramica della durata del progetto

Adobe Workfront calcola la durata di un progetto tenendo conto della data di inizio della prima attività e della data di completamento dell&#39;attività più recente e conta il numero di giorni tra le due date.

## Durata progetto

La durata del progetto è calcolata con la seguente formula:

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>La durata dei problemi sul progetto non influisce sulla durata del progetto.

La durata del progetto conta il numero di giorni tra le due date dell&#39;attività in base alla pianificazione associata al progetto o agli utenti assegnati alle attività. Per informazioni sulla pianificazione utilizzata da Workfront per calcolare la durata, vedere [Panoramica pianificazioni](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).

## Tipi di durata del progetto

Esistono due tipi di Durata del progetto e le formule in base alle quali Workfront li calcola:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **Durata Pianificata**:

  ```
  Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
  ```

* **Durata effettiva**:

  ```
  Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
  ```

## Individua la durata del progetto

Puoi individuare le durate pianificate e effettive del progetto nelle seguenti aree di Workfront:

* . Nell’area Dettagli progetto, nella sezione Panoramica.

  Per ulteriori informazioni sulla scheda secondaria Panoramica di un progetto, vedere l&#39;articolo [Gestire le informazioni nell&#39;area Panoramica del progetto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* In un report di progetto, includendo i campi Durata o Durata effettiva nel report.

  Per ulteriori informazioni sulla creazione di report, vedere l&#39;articolo [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
