---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Calcolare il rischio del valore netto in un portafoglio
description: In Portfoli Optimizer, la variabile [!UICONTROL Rischio di valore netto] L'indicatore misura il rischio potenziale tenendo conto del valore netto fornito da tutti i progetti visualizzati in Portfoli Optimizer.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Calcola il [!UICONTROL Rischio di valore netto] in un portafoglio

In [!UICONTROL Ottimizzatore Portfolio], [!UICONTROL Rischio di valore netto] L&#39;indicatore misura il rischio potenziale tenendo conto [!UICONTROL Valore netto] forniti da tutti i progetti visualizzati nel [!UICONTROL Ottimizzatore Portfolio]. 

Per ottenere la massima efficienza all’interno del portfolio, desideri che la [!UICONTROL Rischio] l&#39;indicatore è basso e [!UICONTROL Valore netto] l&#39;indicatore è alto. 

La [!UICONTROL Rischio] e [!UICONTROL Valore netto] Gli indicatori sono rappresentati dal punto di vista del loro rapporto reciproco.

[!DNL Adobe Workfront] calcola il [!UICONTROL Rischio] e [!UICONTROL Valore netto] utilizzando le seguenti formule:

* La [!UICONTROL Rischio] l&#39;indicatore è calcolato con la seguente formula:

   ```
   Risk indicator = Risk / (Risk + Net Value)
   ```

* La [!DNL Net Value] Questo indicatore è calcolato dalle seguenti formule:

   ```
   Net Value indicator = 1 - Risk / (Risk + Net Value)
   ```

   Oppure

   ```
   Net Value indicator = Net Value / (Risk + Net Value)
   ```

>[!NOTE]
>
>La [!UICONTROL Rischio di valore netto] in base ai progetti visualizzati nella [!UICONTROL Ottimizzatore Portfolio]e non su tutti i progetti associati al portafoglio. 
