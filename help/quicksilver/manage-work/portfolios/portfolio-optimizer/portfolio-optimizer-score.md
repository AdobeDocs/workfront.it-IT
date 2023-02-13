---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Panoramica del punteggio di Portfoli Optimizer
description: Puoi trovare il punteggio di Portfolio Optimizer in Portfoli Optimizer. Viene visualizzato nel [!UICONTROL Punteggio] per ogni progetto. Rappresenta un punteggio per ogni progetto del portfolio.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 4451b1a3-57ae-4c66-a6a1-a85bd51a1648
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 1%

---

# Panoramica [!UICONTROL Ottimizzatore Portfolio] Punteggio

È possibile trovare le [!UICONTROL Ottimizzatore Portfolio] punteggio nel [!UICONTROL Ottimizzatore Portfolio]. Viene visualizzato nel **[!UICONTROL Punteggio]** per ogni progetto. Rappresenta un punteggio per ogni progetto del portfolio.

Per informazioni su come individuare il [!UICONTROL Ottimizzatore Portfolio], vedi l&#39;articolo [[!UICONTROL Ottimizzatore Portfolio] panoramica](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

Per informazioni su come [!DNL Adobe Workfront] utilizza il punteggio del progetto e altre informazioni sul progetto per ottimizzare i progetti nel [!UICONTROL Ottimizzatore Portfolio], vedi [Ottimizzare i progetti in Portfoli Optimizer](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

## Differenza tra [!UICONTROL Punteggio di allineamento] e [!UICONTROL Punteggio di Portfoli Optimizer]

C&#39;è una differenza tra il punteggio di allineamento e il punteggio di ottimizzazione del portfolio di un progetto.

Il punteggio di allineamento di un progetto viene calcolato in base ai punti ottenuti dopo il completamento della scorecard. Questo punteggio viene quindi utilizzato per determinare il punteggio di allineamento del portfolio. Il punteggio di allineamento viene visualizzato come percentuale.\
Il punteggio di allineamento di un progetto viene visualizzato nel **[!UICONTROL Allineamento]** della colonna [!UICONTROL Ottimizzatore Portfolio] o [!UICONTROL Allineamento] campo [!UICONTROL Riepilogo del caso aziendale].

![](assets/business-case-summary-aligned-field-highlighted.png)

![](assets/project-alignment-score-portfolio-optimizer-highlighted-350x174.png)

Per ulteriori informazioni sulla generazione del punteggio di allineamento di un progetto, consulta l’articolo [Applicare una scorecard a un progetto e generare un punteggio di allineamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

La [!UICONTROL ottimizzatore di portafoglio] il punteggio è una classificazione calcolata automaticamente nel [!UICONTROL Ottimizzatore Portfolio] in base a quali progetti è possibile dare la priorità. Il punteggio dell&#39;ottimizzatore portfolio viene visualizzato come un&#39;icona indicatore accompagnata da un numero e viene visualizzato nella **[!UICONTROL Punteggio]** della colonna [!UICONTROL Ottimizzatore Portfolio].

>[!NOTE]
>
>Puoi assegnare un punteggio a un progetto nel [!UICONTROL Ottimizzatore Portfolio] solo se il relativo Business Case è stato completato. Per ulteriori informazioni sul completamento di un Business Case, consulta l’articolo [[!UICONTROL Creare un caso aziendale] per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

![](assets/portfolio-optimizer-project-score-highlighted-350x132.png)

Il punteggio per ciascun progetto viene calcolato in base all’importanza delle seguenti categorie:

* [!UICONTROL Costo]
* [!UICONTROL Allineamento]
* [!UICONTROL Valore Netto]
* [!UICONTROL Rischio di benefici]
* [!UICONTROL ROI]

## Calcola il [!UICONTROL Ottimizzatore Portfolio] Punteggio

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This was edited based on this issue, per Anna: https://hub.workfront.com/issue/603d0c58000095ea0bc00ce5e2110693/overview)</p>
-->

[!DNL Workfront] produce un punteggio utilizzando [!UICONTROL Ottimizzatore Portfolio] che è una graduatoria per contribuire alla definizione delle priorità dei progetti. I valori nel portfolio si basano sui valori inseriti nei business case dei progetti e vengono utilizzati per calcolare un punteggio per il progetto. I progetti con un punteggio più elevato potrebbero essere considerati di maggiore importanza e potrebbero essere prioritari per essere completati per primi.

Per conoscere la classificazione di un progetto, procedi come segue:

1. Vai a [!UICONTROL Ottimizzatore Portfolio].
1. Passa il cursore del mouse sull’icona della classificazione per visualizzare il punteggio dell’ottimizzatore di portfolio per un progetto.

![ranking_icon_in_portfolio_optimizer_new.png](assets/ranking-icon-in-portfolio-optimizer-new-350x160.png)

L&#39;algoritmo per il calcolo dei punteggi prende in considerazione i valori descritti nei Casi aziendali dei progetti e i pesi che essi comportano. Dà a ogni progetto nell&#39;ottimizzatore un punteggio e normalizza quel punteggio in modo che ci sia sempre un progetto con un punteggio di 100. Questo dà un punteggio alto al progetto migliore.

**Esempio:** Ad esempio, se [!UICONTROL allineamento superiore] l’unico fattore da considerare è che il progetto con l’allineamento più alto ottiene il punteggio di 100.

Di seguito sono riportati i criteri per la valutazione di un progetto:

* [!UICONTROL Costo]
* [!UICONTROL Allineamento]
* [!UICONTROL Valore]
* [!UICONTROL Rischio di benefici]
* [!UICONTROL ROI]

![](assets/optimizer-sliding-value-options-350x77.png)

Per informazioni su come ottimizzare i progetti nel portfolio, vedi [Ottimizzare i progetti nelle [!UICONTROL Ottimizzatore Portfolio]](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

Ogni criterio nel pannello di configurazione ([!UICONTROL Costo], [!UICONTROL Allineamento], [!UICONTROL ROI], [!UICONTROL Valore netto], [!UICONTROL Rischio di benefici]) viene assegnato il peso compreso tra 0 e 100 in base a quello selezionato.

Per ogni progetto con un business case completo, viene generato un punteggio per criterio con la seguente formula:

```
Score Per Criteria = (Project Value For The Criteria - AVG(all the project values for this criteria)) / Standard Deviation of that value for that project
```

**Esempio:** Per [!UICONTROL Punteggio di allineamento] per il progetto A, avrai i seguenti elementi:

```
Alignment Score = (Project A Alignment Score - AVG (of all the project Alignments)) / Standard Deviation of alignment score for that project
```

Una volta che hai tutti [!UICONTROL Punteggio per criterio] calcolati, puoi aggiungerli tenendo conto dei loro pesi per ottenere il punteggio completo per progetto. Il punteggio del progetto viene calcolato con la seguente formula:

```
Score = Cost Score * Cost Weight + Alignment Score * Alignment Weight + ROI Score * ROI Weight + Net Value Score * Net Value Weight + Risk Score * Risk Weight
```

Per il costo del progetto e [!UICONTROL rischio] la logica funziona al contrario del funzionamento degli altri criteri: se vuoi [!UICONTROL Basso costo] per essere importante, non aumenterà ma diminuirà il punteggio complessivo del progetto per `Cost Score * Cost Weight`.

Dopo aver calcolato i punteggi per ciascun progetto, la [!UICONTROL Punteggio di ottimizzazione] è definito per i progetti nel modo seguente:

1. [!UICONTROL Minimo] e [!UICONTROL Massimo] i punteggi sono definiti.
1. Viene calcolato l’intervallo tra tali valori.
1. Per ogni progetto, [!UICONTROL Punteggio di ottimizzazione] viene calcolato con la seguente formula:

   ```
   Optimization Score = Rounded ((Score - Minimum / Range)*100)
   ```
