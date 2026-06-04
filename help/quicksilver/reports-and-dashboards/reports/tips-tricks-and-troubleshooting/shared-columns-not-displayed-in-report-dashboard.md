---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: I dati delle colonne condivise non vengono mostrati nei rapporti della dashboard
description: I dati delle colonne condivise non vengono visualizzati quando il rapporto viene inserito in un layout con dashboard a più colonne, ma in un layout a colonna singola. Vengono inoltre sostituite le interruzioni di riga.
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OEFlwkdPf98g4-rC1tzaTmmEwb5-BXHx-j8XGrRR8sE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 162
ht-degree: 12%

---

# I dati delle colonne condivise non vengono mostrati nei rapporti della dashboard

## Problema

I dati delle colonne condivise non vengono visualizzati quando il rapporto viene inserito in un layout con dashboard a più colonne, ma in un layout a colonna singola. Vengono inoltre sostituite le interruzioni di riga.

## Causa

Solo le colonne contrassegnate come

```
shortview=true
```

sono incluse nella vista del dashboard del report quando il layout del dashboard ha la suddivisione sinistra/destra o la suddivisione sinistra/centro/destra impostata.

## Soluzione

Accedi alla visualizzazione utilizzata nel report e apri la modalità testo. Per ulteriori informazioni, vedere [Modificare una visualizzazione utilizzando la modalità testo](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md). Etichettare tutte le colonne del report, incluse quelle utilizzate in una colonna condivisa/unita, con

```
shortview=true
```

. Le colonne del rapporto vengono quindi visualizzate correttamente nel dashboard.
