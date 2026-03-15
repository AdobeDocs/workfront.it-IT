---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: I dati delle colonne condivise non vengono mostrati nei rapporti della dashboard
description: I dati delle colonne condivise non vengono visualizzati quando il rapporto viene inserito in un layout con dashboard a più colonne, ma in un layout a colonna singola. Vengono inoltre sostituite le interruzioni di riga.
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '162'
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
