---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Panoramica delle istruzioni IF
description: È possibile utilizzare istruzioni "IF" nei linguaggi di programmazione generali. In Adobe Workfront, le istruzioni "IF" consentono di confrontare, formattare e stringere insieme campi di dati a scopo di reporting e di dati personalizzati. Inoltre, pensare matematicamente alle istruzioni "IF" porta a una migliore comprensione concettuale, dal momento che le variabili per le espressioni sono comunemente utilizzate.
author: Nolan
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 23b5ba9564b514e11c1ca9d5cca276238ef11066
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Panoramica delle istruzioni &quot;IF&quot;

<!-- Audited: 1/2024 -->

È possibile utilizzare istruzioni &quot;IF&quot; nei linguaggi di programmazione generali. In Adobe Workfront, le istruzioni &quot;IF&quot; consentono di confrontare, formattare e stringere insieme campi di dati a scopo di reporting e di dati personalizzati. Inoltre, pensare matematicamente alle istruzioni &quot;IF&quot; porta a una migliore comprensione concettuale, dal momento che le variabili per le espressioni sono comunemente utilizzate.

## Recommendations per istruzioni &quot;IF&quot;

Prima di creare un&#39;istruzione &quot;IF&quot;, considera quanto segue:

* Per questa guida si consiglia di conoscere tutti i linguaggi di programmazione generali, ma non è necessario conoscerli.
* È necessaria una comprensione avanzata della sintassi della modalità testo di Workfront. Questo aiuta a comprendere la terminologia dell’API di Workfront e la sintassi dei dati personalizzati in questi formati specifici.

  Per informazioni sull’API di Workfront, consulta [Nozioni di base sulle API](../../../wf-api/general/api-basics.md).

  Per informazioni sull&#39;utilizzo della modalità testo, vedere [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* Puoi creare istruzioni &quot;IF&quot; per i seguenti elementi di Workfront:

   * Viste
   * Raggruppamenti
   * Campi personalizzati calcolati

* Non è possibile creare istruzioni &quot;IF&quot; per i filtri. Questo genera un errore &quot;Ops&quot; in Workfront.
* Il team di supporto non è in grado di creare dati personalizzati. Dopo aver generato i campi o le colonne personalizzati, è possibile contattare il team di supporto e i risultati desiderati non vengono visualizzati. Per assistenza nella creazione di un’espressione, contatta il tuo Account Executive per informazioni sulle nostre opzioni di consulenza.
* È consigliabile innanzitutto scrivere queste espressioni in un editor di testo, ad esempio Sublime o Visual Studio Code, in quanto ciò consente di visualizzare i dati in modo più chiaro rispetto a quanto risulterebbe in Workfront.

## Componenti di un&#39;istruzione &quot;IF&quot;

Puoi creare istruzioni &quot;IF&quot; in Workfront utilizzando il seguente formato:
<pre>IF(Condizione,Espressione reale,Espressione falsa)</pre>I componenti di un'istruzione "IF" sono:

* **IF** = Espressione dei dati calcolati di Workfront per &quot;function&quot;. Simile alle espressioni SUM e PROD, questa prima istruzione indica al sistema di comprendere la funzione come un&#39;istruzione &quot;IF&quot;. Utilizzare sempre lettere maiuscole per &quot;IF&quot; in questa istruzione.\
  Per un elenco di tutte le espressioni di dati calcolati, vedi [Panoramica delle espressioni di dati calcolati](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **Condizione** = Questa è la condizione che la variabile Workfront deve soddisfare ed è la base per questa equazione. Tutto ciò che può essere successivamente specificato nell&#39;equazione dipende dalla condizione. È possibile utilizzare una serie di riferimenti, confronti o espressioni matematiche per avviare un&#39;equazione. Alcuni esempi di condizioni sono:

   * Una data è successiva a un&#39;altra data su un oggetto specificato.
   * Uno stato è uguale a uno degli stati disponibili su un oggetto specificato.
   * La percentuale di completamento di un&#39;attività è minore o maggiore di una determinata percentuale.

* **Operatore condizione** = questo è l’operatore che ti aiuta a creare la condizione dell’istruzione &quot;IF&quot;. Ad esempio, &quot;è uguale a&quot; o &quot;è maggiore di&quot; sono operatori di condizione. Per un elenco degli operatori di condizione che è possibile utilizzare nelle istruzioni, vedere [Operatori condizione nelle espressioni personalizzate calcolate](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* **Espressione ****** = Questa è la variabile &quot;True&quot;, che indica all&#39;equazione quale indicatore visualizzare una volta soddisfatti i criteri della condizione (indicatori true).

* **Espressione False** = Variabile &quot;False&quot; che indica all&#39;equazione quale indicatore visualizzare quando i criteri della condizione non sono soddisfatti (indicatori falsi).

Nell&#39;esempio seguente viene utilizzato il formato di istruzione originale per scrivere un&#39;espressione dati semplice per un&#39;istruzione &quot;IF&quot;. L’espressione confronta due diversi campi data in Workfront seguiti da un risultato Vero/Falso come stringa di dati:

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

Nel discorso di tutti i giorni, questa affermazione significherebbe: se la data di completamento prevista del mio oggetto è &quot;maggiore di&quot; la data di completamento pianificata del mio stesso oggetto, visualizza le parole &quot;Fuori pista&quot; in questo campo. In caso contrario, visualizzare le parole &quot;In esecuzione&quot;.

## Creare campi calcolati in moduli personalizzati o colonne personalizzate utilizzando istruzioni &quot;IF&quot;

È possibile creare istruzioni &quot;IF&quot; in un campo calcolato in un modulo personalizzato o in una colonna personalizzata.

La sintassi utilizzata in un modulo personalizzato calcolato è diversa da quella di una colonna personalizzata calcolata. Consulta i seguenti esempi:

* [Istruzioni singole &quot;IF&quot;](#single-if-statements)
* [Più istruzioni &quot;IF&quot;](#multiple-if-statements)

### Istruzioni singole &quot;IF&quot; {#single-if-statements}

Di seguito sono riportati alcuni esempi di campi personalizzati calcolati e della colonna corrispondente che utilizzano un’istruzione &quot;IF&quot;:

* Campo personalizzato calcolato:

Quando crei un campo personalizzato, utilizza la sintassi seguente per un’istruzione &quot;IF&quot;:

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* Colonna personalizzata calcolata:

Durante la creazione di una colonna personalizzata, è necessario utilizzare la sintassi seguente per l&#39;istruzione &quot;IF&quot; nella riga dell&#39;espressione di valore:

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### Più istruzioni &quot;IF&quot; {#multiple-if-statements}

Per creare un’espressione più complessa e dinamica, puoi creare più istruzioni &quot;IF&quot; con la seguente istruzione:

<pre>IF(Condizione1,Espressione True,IF(Condizione2,Espressione True,Espressione False))</pre>Si noti che ora non è presente alcuna istruzione false per la prima "IF". Invece, l'abbiamo sostituito con l'inizio di un secondo "IF".

Di seguito sono riportati alcuni esempi di campi personalizzati calcolati e della corrispondente colonna personalizzata che utilizzano più istruzioni &quot;IF&quot;:

* Campo personalizzato calcolato:

  ```
  IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
  ```

* Colonna personalizzata calcolata:

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

In questo esempio, lo stesso risultato è stato ottenuto mettendo insieme due variabili di criteri diverse.\
Puoi esplorare ulteriormente queste opzioni ricostruendo questi esempi nel tuo ambiente.

Il modo migliore per imparare questo è sperimentare con vari campi e scenari. Acquisisci inoltre familiarità con API Explorer, che rivela i nomi dei campi che possono essere utilizzati. Per informazioni su API Explorer, consulta [API Explorer](../../../wf-api/general/api-explorer.md).

Per ulteriori informazioni sulla sintassi Workfront delle espressioni di dati calcolati, vedi [Panoramica delle espressioni di dati calcolati](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
