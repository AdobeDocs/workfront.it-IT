---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcola valore netto
description: Il valore netto di un progetto è il valore totale previsto del progetto dopo il calcolo del vantaggio e l'eliminazione dei costi.
author: Lisa
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 1%

---

# Calcola valore netto

Il valore netto di un progetto è il valore totale previsto del progetto dopo il calcolo del vantaggio e l&#39;eliminazione dei costi.

## Panoramica del progetto Valore netto

Adobe Workfront calcola il valore netto di un progetto utilizzando la formula seguente:

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

I campi seguenti possono influire sul valore netto di un progetto:

* **Vantaggio pianificato**: voce manuale specificata dal proprietario del progetto al completamento dell&#39;area **Informazioni progetto** del caso di business.\
  Per ulteriori informazioni sul beneficio pianificato di un progetto, vedere la sezione [Informazioni sul progetto](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) nell&#39;articolo [Panoramica delle aree del caso aziendale](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* **Costo preventivato**: questo è il costo totale associato al progetto come stimato al primo avvio del progetto.

  Il **Costo preventivato** utilizza il valore **Costo manodopera preventivato** calcolato nell&#39;area Budget risorse del caso di business e tiene conto delle ore preventivate per le mansioni in Programmazione risorse e della tariffa Costo per ora di ciascuna mansione.\
  Il costo preventivato influisce sul **valore netto** del progetto. Per ulteriori informazioni sul calcolo del costo preventivato, vedere [Calcolare il costo preventivato](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **Costo rischio potenziale**: si tratta del costo associato a qualsiasi rischio nel progetto, come definito nel Business Case o nella scheda Rischi del progetto.\
  Per ulteriori informazioni sul calcolo del costo del rischio potenziale di un progetto, vedere l&#39;articolo [Calcolare il costo del rischio potenziale](../../../manage-work/projects/project-finances/potential-risk-cost.md).



## Individuazione del valore netto del progetto

Il valore netto di un progetto si trova nelle seguenti aree in Workfront:

* Area Riepilogo del caso di business\
  Per ulteriori informazioni sull&#39;area Riepilogo caso di business, vedere la sezione &quot;Informazioni sul riepilogo del caso di business&quot; nell&#39;articolo [Creare un caso di business per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md) [Creare un caso di business per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

  ![Valore netto nel caso di business](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* In Portfolio Optimizer se il progetto è associato a un portfolio

  >[!TIP]
  >
  >Il totale di tutti i valori netti del progetto è il valore netto del portfolio.

  Per ulteriori informazioni su Portfolio Optimizer, vedere [Panoramica di Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* Nel campo Valore netto progetto dei seguenti elenchi e rapporti:

   * Progetto
   * Attività
   * Problema
   * Progetto (dati finanziari)

  Per ulteriori informazioni sulla creazione di un report, vedere l&#39;articolo [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
