---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formattare numeri, valuta e valori percentuali nei report in modalità testo
description: I valori numerici, inclusa la valuta, possono essere configurati per la visualizzazione in diversi formati nei rapporti ed elenchi in Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 6%

---

# Formattare numeri, valuta e valori percentuali nei report in modalità testo

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

