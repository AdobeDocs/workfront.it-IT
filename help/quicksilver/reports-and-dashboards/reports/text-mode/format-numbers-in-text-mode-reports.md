---
product-area: reporting
navigation-topic: text-mode-reporting
title: Valori di formato, valuta e percentuale nei report in modalità testo
description: I valori numerici, compresa la valuta, possono essere configurati per essere visualizzati in diversi formati nei rapporti e negli elenchi in Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 7%

---

# Valori di formato, valuta e percentuale nei report in modalità testo

I valori numerici, compresa la valuta, possono essere configurati per essere visualizzati in diversi formati nei rapporti e negli elenchi in Adobe Workfront.

Per modificare il formato di un valore numerico, è necessario modificare il **valueformat** linea della colonna.

Ad esempio, se desideri visualizzare la colonna Budget come $1000, la riga del formato del valore sarà simile alla seguente:

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Per ulteriori informazioni sull&#39;applicazione della formattazione condizionale nei rapporti e negli elenchi di Workfront utilizzando la modalità testo, consulta [Utilizzare la formattazione condizionale nella modalità Testo](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

È possibile formattare i numeri utilizzando i seguenti valori per `valueformat` riga della colonna:

| Esempio | `valueformat=` |
|---|---|
| 1234 | <pre>doubleAsString</pre> <br>oppure <br><pre>int</pre> |
| 1.234 | <pre>doubleAsInt</pre> |
| $1,234 | <pre>currencyStringCurrencyRounded</pre> |
| 1234.56 | <pre>doubleAsDouble</pre> |
| $1,234.56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounded</pre> |
| 12.34% | <pre>doubleAsPercent</pre> |
| (1,234.56) | <pre>doubleAsFinancial</pre> |
| (1,234) | <pre>doubleAsFinancialRounded</pre> |
