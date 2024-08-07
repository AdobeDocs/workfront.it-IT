---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formattare numeri, valuta e valori percentuali nei report in modalità testo
description: I valori numerici, inclusa la valuta, possono essere configurati per la visualizzazione in diversi formati nei rapporti ed elenchi in Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 8de9c79f6c62b74a652482ec10bf38fada8c5fc8
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 7%

---

# Formattare numeri, valuta e valori percentuali nei report in modalità testo

<!-- Audited: 2/2024 -->

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
| 1234 | <pre>doubleAsString</pre> <br> o <br><pre>int</pre> |
| 1.234 | <pre>doubleAsInt</pre> |
| $1,234 | <pre>currencyStringCurrencyRounded</pre> |
| 1234,56 | <pre>doubleAsDouble</pre> |
| $1,234.56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounded</pre> |
| 12.34% | <pre>doubleAsPercent</pre> |
| (1,234.56) | <pre>doubleAsFinancial</pre> |
| (1,234) | <pre>doubleAsFinancialRounded</pre> |

