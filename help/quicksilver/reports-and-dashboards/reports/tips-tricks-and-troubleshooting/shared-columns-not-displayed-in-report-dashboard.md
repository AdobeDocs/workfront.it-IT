---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: I dati provenienti da colonne condivise non vengono visualizzati nei rapporti del dashboard
description: I dati provenienti da colonne condivise non vengono visualizzati quando il rapporto viene posizionato in un layout di dashboard a più colonne, ma in un layout a una singola colonna. Vengono ignorate anche le interruzioni di riga.
author: Nolan
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# I dati provenienti da colonne condivise non vengono visualizzati nei rapporti del dashboard

## Problema

I dati provenienti da colonne condivise non vengono visualizzati quando il rapporto viene posizionato in un layout di dashboard a più colonne, ma in un layout a una singola colonna. Vengono ignorate anche le interruzioni di riga.

## Causa

Solo le colonne contrassegnate come

```
shortview=true
```

sono inclusi nella vista dashboard del rapporto quando il layout del dashboard presenta la suddivisione sinistra/destra o la suddivisione sinistra/centrale/destra.

## Soluzione

Accedi alla visualizzazione utilizzata nel rapporto e alla modalità di testo aperto. (Per ulteriori informazioni, consulta [Modificare una visualizzazione utilizzando la modalità testo](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Etichettare tutte le colonne del rapporto, comprese quelle utilizzate in una colonna condivisa/unita, con

```
shortview=true
```

. Le colonne del rapporto vengono quindi visualizzate correttamente nel dashboard.
