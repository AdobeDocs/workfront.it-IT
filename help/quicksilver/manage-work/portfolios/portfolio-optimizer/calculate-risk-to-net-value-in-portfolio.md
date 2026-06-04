---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Calcolare il rischio per il valore netto in un portfolio
description: In Portfolio Optimizer, l'indicatore [!UICONTROL Rischio sul valore netto] misura il rischio potenziale tenendo conto del valore netto fornito da tutti i progetti visualizzati in Portfolio Optimizer.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
TQID: https://experienceleague.adobe.com/mClkaUv0y-Y9wiqg4oJivWYtmJDuKG701nOr5TU5rCA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 178
ht-degree: 5%

---

# Calcola il [!UICONTROL Rischio per valore netto] in un portfolio

In [!UICONTROL Portfolio Optimizer], l&#39;indicatore [!UICONTROL Risk to Net Value] misura il rischio potenziale tenendo conto del [!UICONTROL Net Value] fornito da tutti i progetti visualizzati in [!UICONTROL Portfolio Optimizer].

Per ottenere la massima efficienza all&#39;interno del portfolio, è necessario che l&#39;indicatore [!UICONTROL Rischio] sia basso e che l&#39;indicatore [!UICONTROL Valore netto] sia alto.

Gli indicatori [!UICONTROL Rischio] e [!UICONTROL Valore Netto] sono rappresentati dal punto di vista della loro relazione reciproca.

[!DNL Adobe Workfront] calcola gli indicatori [!UICONTROL Rischio] e [!UICONTROL Valore Netto] utilizzando le formule seguenti:

* L&#39;indicatore [!UICONTROL Rischio] è calcolato dalla formula seguente:

  ```
  Risk indicator = Risk / (Risk + Net Value)
  ```

* L&#39;indicatore [!DNL Net Value] viene calcolato con le seguenti formule:

  ```
  Net Value indicator = 1 - Risk / (Risk + Net Value)
  ```

  Oppure

  ```
  Net Value indicator = Net Value / (Risk + Net Value)
  ```

>[!NOTE]
>
>L&#39;indicatore [!UICONTROL Rischio per valore netto] viene calcolato in base ai progetti visualizzati in [!UICONTROL Portfolio Optimizer] e non a tutti i progetti associati al portfolio.
