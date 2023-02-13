---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcola il ritorno sull'investimento (ROI)
description: Il Return On Investment (ROI) è una metrica Adobe Workfront che consente ai responsabili del portafoglio di vedere rapidamente le prestazioni del progetto rispetto al costo originale pianificato del benefit e a budget del progetto.
author: Alina
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Calcola il ritorno sull&#39;investimento (ROI)

Il Return On Investment (ROI) è una metrica Adobe Workfront che consente ai responsabili del portafoglio di vedere rapidamente le prestazioni del progetto rispetto al costo originale pianificato del benefit e a budget del progetto.

## Panoramica del progetto Return on Investment (ROI)

Workfront calcola il ROI utilizzando la seguente formula:

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

I campi seguenti influiscono sul ROI di un progetto:

* **Vantaggio pianificato progetto**: Si tratta di una voce manuale specificata dal proprietario del progetto durante il completamento dell&#39;area Informazioni progetto del Business Case. Si tratta di una stima di ciò che, in qualità di proprietario del progetto, ritieni che il beneficio del progetto possa derivare dal completamento del progetto. Si tratta di un importo specifico di valuta e deve essere un valore positivo.\
   Per ulteriori informazioni sul beneficio pianificato di un progetto, consulta la sezione &quot;Informazioni sul progetto&quot; nell’articolo [Creare un business case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **Costo preventivato progetto**: è il costo totale associato al progetto stimato al primo avvio del progetto.

   La **Costo preventivato** utilizza **Costo manodopera a budget** Valore calcolato nell&#39;area Resource Budgeting del Business Case e che tiene conto delle ore previste per i ruoli di lavoro nel Resource Planner e del tasso Costo per ora di ciascun ruolo di lavoro.\
   Per ulteriori informazioni, consulta [Calcola costo preventivato](../../../manage-work/projects/project-finances/budgeted-cost.md).

## Individua il ritorno sull&#39;investimento (ROI) del progetto

Puoi visualizzare il valore del ROI di un progetto nelle seguenti aree in Workfront:

* In Portfoli Optimizer se il progetto è associato a un portfolio

   >[!NOTE]
   >
   >Il totale di tutti i valori del ROI del progetto è il ROI del portafoglio.

   Per informazioni su Portfoli Optimizer, consulta l&#39;articolo [Panoramica di Portfoli Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* Nel campo ROI del progetto , puoi trovare gli elenchi e i rapporti seguenti: 

   * Progetto
   * Attività
   * Problema
   * Progetto (dati finanziari)
   Per ulteriori informazioni sulla creazione di rapporti in Workfront, consulta l’articolo [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
