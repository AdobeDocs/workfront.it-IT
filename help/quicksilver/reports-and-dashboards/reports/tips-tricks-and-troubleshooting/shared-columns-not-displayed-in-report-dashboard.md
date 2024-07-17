---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: I dati delle colonne condivise non vengono visualizzati nei rapporti del dashboard
description: I dati delle colonne condivise non vengono visualizzati quando il rapporto viene inserito in un layout con dashboard a più colonne, ma in un layout a colonna singola. Vengono inoltre sostituite le interruzioni di riga.
author: Nolan
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# I dati delle colonne condivise non vengono visualizzati nei rapporti del dashboard

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
