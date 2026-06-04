---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formattare numeri, valuta e valori percentuali nei rapporti in modalità testo
description: I valori numerici, inclusa la valuta, possono essere configurati per la visualizzazione in diversi formati nei rapporti ed elenchi in Adobe Workfront.
author: Courtney
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/z96Rvp54iQcZxVWJ4Evoe1Qasl-VrEZ-IrVy11n9cDc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 145
ht-degree: 20%

---

# Formattare numeri, valuta e valori percentuali nei rapporti in modalità testo

<!-- Audited: 1/2025 -->

I valori numerici, inclusa la valuta, possono essere configurati per la visualizzazione in diversi formati nei rapporti ed elenchi in Adobe Workfront.

Per modificare il formato di un valore numerico, è necessario modificare la riga **valueformat** della colonna.

Ad esempio, per visualizzare la colonna Budget come $1000, la riga del formato del valore sarà simile alla seguente:

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Per ulteriori informazioni sull&#39;applicazione della formattazione condizionale nei report e negli elenchi di Workfront utilizzando la modalità testo, vedere [Utilizzare la formattazione condizionale in modalità testo](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

È possibile formattare i numeri utilizzando i seguenti valori per la riga `valueformat` della colonna:

| Esempio | `valueformat=` |
|---|---|
| 1234 | `doubleAsString`<br>or<br>`int` |
| 1.234 | `doubleAsInt` |
| $1,234 | `currencyStringCurrencyRounded` |
| 1234,56 | `doubleAsDouble` |
| $1,234.56 | `currencyStringCurrency` |
| 12% | `doubleAsPercentRounded` |
| 12.34% | `doubleAsPercent` |
| (1,234.56) | `doubleAsFinancial` |
| (1,234) | `doubleAsFinancialRounded` |

