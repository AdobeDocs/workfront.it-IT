---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Panoramica della durata del progetto
description: Adobe Workfront calcola la durata di un progetto tenendo conto della data di inizio della prima attività e della data di completamento dell'attività più recente e conta il numero di giorni tra le due date.
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
TQID: https://experienceleague.adobe.com/1j0nj2W5f7FtgIk46G3ePFA-zwt7VAyV9fQWKm2kZJ4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 254
ht-degree: 2%

---

# Panoramica sulla durata del progetto

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
