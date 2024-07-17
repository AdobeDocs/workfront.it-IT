---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Calcolare il rischio per il valore netto in un portfolio
description: In Ottimizzatore Portfolio, l'indicatore [!UICONTROL Rischio sul valore netto] misura il rischio potenziale tenendo conto del valore netto fornito da tutti i progetti visualizzati in Ottimizzatore Portfolio.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

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
>L&#39;indicatore [!UICONTROL Rischio per valore netto] viene calcolato in base ai progetti visualizzati in [!UICONTROL Ottimizzatore Portfolio] e non a tutti i progetti associati al portfolio. 
