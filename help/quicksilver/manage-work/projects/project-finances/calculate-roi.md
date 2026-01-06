---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcola il ritorno sull’investimento (ROI)
description: Il ROI (Return On Investment) è una metrica di Adobe Workfront che consente ai gestori del portfolio di visualizzare rapidamente le prestazioni del progetto rispetto al beneficio pianificato e al costo preventivato originali del progetto.
author: Lisa
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 1%

---

# Calcola il ritorno sull’investimento (ROI)

Il ROI (Return On Investment) è una metrica di Adobe Workfront che consente ai gestori del portfolio di visualizzare rapidamente le prestazioni del progetto rispetto al beneficio pianificato e al costo preventivato originali del progetto.

## Panoramica del ritorno sull’investimento (ROI) del progetto

Workfront calcola il ROI utilizzando la seguente formula:

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

I seguenti campi influiscono sul ROI di un progetto:

* **Beneficio pianificato progetto**: voce manuale specificata dal proprietario del progetto al completamento dell&#39;area Informazioni progetto del caso di business. In questo esempio viene illustrato ciò che si ritiene, in qualità di Proprietario del progetto, possa essere utile se si completa il progetto. Si tratta di un importo di valuta specifico che deve essere un valore positivo.\
  Per ulteriori informazioni sul beneficio pianificato di un progetto, vedere la sezione &quot;Informazioni sul progetto&quot; nell&#39;articolo [Creare un caso di business per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **Costo preventivato progetto**: questo è il costo totale associato al progetto come stimato al primo avvio del progetto.

  Il **Costo preventivato** utilizza il valore **Costo manodopera preventivato** calcolato nell&#39;area Budget risorse del caso di business e tiene conto delle ore preventivate per le mansioni in Programmazione risorse e della tariffa Costo per ora di ciascuna mansione.\
  Per ulteriori informazioni, vedere [Calcola costo preventivato](../../../manage-work/projects/project-finances/budgeted-cost.md).

## Individuazione del ritorno sull&#39;investimento (ROI) del progetto

Il valore del ROI di un progetto può essere visualizzato nelle seguenti aree in Workfront:

* In Portfolio Optimizer se il progetto è associato a un portfolio

  >[!NOTE]
  >
  >Il totale di tutti i valori di ROI del progetto è il ROI del portfolio.

  Per informazioni su Portfolio Optimizer, vedere l&#39;articolo [Panoramica di Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* Nel campo ROI progetto nei seguenti elenchi e rapporti:

   * Progetto
   * Attività
   * Problema
   * Progetto (dati finanziari)

  Per ulteriori informazioni sulla creazione di report in Workfront, vedere l&#39;articolo [Creazione di un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
