---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcolare il costo del rischio potenziale
description: Il costo potenziale del rischio di un progetto tiene conto dei costi potenziali dei rischi del progetto e della loro probabilità di verificarsi.
author: Lisa
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
TQID: https://experienceleague.adobe.com/32kwPUhdtWhFeqQ34oReoU8xl2JlaWQeZlq7MI1jqtc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 302
ht-degree: 2%

---

# Calcolare il costo del rischio potenziale

Il costo potenziale del rischio di un progetto tiene conto dei costi potenziali dei rischi del progetto e della loro probabilità di verificarsi.

## Panoramica sul costo potenziale del rischio di un progetto

Adobe Workfront calcola il costo rischio potenziale di un progetto utilizzando la formula seguente:

```
Potential Risk Cost =SUM(Potential Risk Costs * Risk Probability)
```

Quando si esamina il costo del rischio potenziale di un progetto, tenere presente quanto segue:

* Il costo del rischio pianificato di un progetto è identico al costo del rischio potenziale.
* Il Costo Rischio Potenziale non viene incorporato nel Costo Pianificato di un progetto. Viene invece utilizzato per determinarne il valore netto.

## Individuazione del costo rischio potenziale di un progetto

Puoi trovare i Rischi per un progetto e il loro Costo Potenziale nelle seguenti aree in Workfront:

* Nella scheda Rischi del progetto.
* Nel Business Case Summary.\
  Per ulteriori informazioni sul Business Case di un progetto, vedere l&#39;articolo [Creare un Business Case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).
* In un report di progetto quando si aggiunge il campo Costo rischio pianificato alle colonne del report.\
  Per ulteriori informazioni sulla creazione di report in Workfront, vedere l&#39;articolo [Creazione di un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* In Portfolio Optimizer, quando il progetto è associato a un Portfolio, nella colonna Rischio.\
  La somma di tutti i costi di rischio potenziale di tutti i progetti del portfolio corrisponde al rischio di Portfolio.\
  Per ulteriori informazioni su Portfolio Optimizer, vedere l&#39;articolo [Panoramica di Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

Per ulteriori informazioni sulla creazione di Rischi in un progetto, vedere l&#39;articolo [Creare e modificare i rischi nei progetti](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)

Per ulteriori informazioni sul Business Case di un progetto, vedere l&#39;articolo [Creare un Business Case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).
