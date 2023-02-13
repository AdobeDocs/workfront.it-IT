---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcola valore netto
description: Il valore netto di un progetto è il valore totale previsto del progetto dopo il calcolo del vantaggio e la rimozione dei costi.
author: Alina
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# Calcola valore netto

Il valore netto di un progetto è il valore totale previsto del progetto dopo il calcolo del vantaggio e la rimozione dei costi. 

## Panoramica del progetto Valore netto

Adobe Workfront calcola il valore netto di un progetto utilizzando la formula seguente: 

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

I campi seguenti possono influenzare il valore netto di un progetto:

* **Vantaggio pianificato**: Si tratta di una voce manuale specificata dal proprietario del progetto al completamento del **Informazioni progetto** area del Business Case.\
   Per ulteriori informazioni sul beneficio pianificato di un progetto, consulta la sezione [Informazioni progetto](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) sezione dell&#39;articolo [Panoramica delle aree del Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* **Costo preventivato**: è il costo totale associato al progetto stimato al primo avvio del progetto.

   La **Costo preventivato** utilizza **Costo manodopera a budget** Valore calcolato nell&#39;area Resource Budgeting del Business Case e che tiene conto delle ore previste per i ruoli di lavoro nel Resource Planner e del tasso Costo per ora di ciascun ruolo di lavoro.\
   Il costo preventivato influisce sul **Valore netto** del progetto. Per ulteriori informazioni sul calcolo del costo preventivato, vedere [Calcola costo preventivato](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **Costo potenziale del rischio**: Questo è il costo associato a eventuali rischi sul progetto, come definiti nel Business Case o nella scheda Rischi del progetto.\
   Per ulteriori informazioni sul calcolo del costo potenziale di un progetto, consulta l’articolo [Calcolare il costo potenziale del rischio](../../../manage-work/projects/project-finances/potential-risk-cost.md).

    

## Individua il valore netto del progetto

Puoi trovare il Valore netto di un progetto nelle seguenti aree in Workfront:

* Nell&#39;area Riepilogo del caso aziendale \
   Per ulteriori informazioni sull&#39;area Riepilogo del caso aziendale, vedere la sezione &quot;Informazioni sul sintetico del caso aziendale&quot; nell&#39;articolo [Creare un business case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md) [Creare un business case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

   ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* In Portfoli Optimizer se il progetto è associato a un portfolio

   >[!TIP]
   >
   >Il totale di tutti i valori netti del progetto è il valore netto del portafoglio.

   Per ulteriori informazioni su Portfoli Optimizer, vedi [Panoramica di Portfoli Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* Nel campo Valore netto progetto degli elenchi e dei rapporti seguenti:

   * Progetto
   * Attività
   * Problema
   * Progetto (dati finanziari)
   Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
