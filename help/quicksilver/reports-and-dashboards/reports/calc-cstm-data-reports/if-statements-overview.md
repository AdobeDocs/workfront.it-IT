---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Panoramica delle istruzioni IF
description: È possibile utilizzare le istruzioni "IF" nei linguaggi di programmazione generali. In Adobe Workfront, le istruzioni "IF" consentono di confrontare, formattare e stringa insieme i campi di dati a scopo di reporting e di dati personalizzati. Inoltre, il pensiero matematico delle istruzioni "IF" porta a una migliore comprensione concettuale, in quanto le variabili per le espressioni sono comunemente utilizzate.
author: Nolan
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# Panoramica delle istruzioni &quot;IF&quot;

È possibile utilizzare le istruzioni &quot;IF&quot; nei linguaggi di programmazione generali. In Adobe Workfront, le istruzioni &quot;IF&quot; consentono di confrontare, formattare e stringa insieme i campi di dati a scopo di reporting e di dati personalizzati. Inoltre, il pensiero matematico delle istruzioni &quot;IF&quot; porta a una migliore comprensione concettuale, in quanto le variabili per le espressioni sono comunemente utilizzate.

## Istruzioni Recommendations per &quot;IF&quot;

Considera quanto segue prima di creare un&#39;istruzione &quot;IF&quot;:

* Si consiglia di comprendere tutti i linguaggi di programmazione generale, ma non è necessario per questa guida.
* È necessaria una comprensione avanzata della sintassi della modalità testo di Workfront. Questo aiuta a comprendere la terminologia dell’API Workfront e la sintassi dei dati personalizzati in questi formati specifici.

   Per informazioni sull’API di Workfront, consulta [Nozioni di base sulle API](../../../wf-api/general/api-basics.md).

   Per informazioni sull’utilizzo della modalità testo, consulta [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* Puoi generare istruzioni &quot;IF&quot; per i seguenti elementi Workfront:

   * Viste
   * Raggruppamenti
   * Campi personalizzati calcolati

* Non è possibile generare istruzioni &quot;IF&quot; per i filtri. Questo si traduce in un errore &quot;Whoops&quot; in Workfront.
* Il team di supporto non aiuta a creare dati personalizzati. È possibile contattare il team di supporto dopo aver creato i campi o le colonne personalizzati e non si visualizzano i risultati desiderati. Per informazioni sulle opzioni di consulenza, contatta il tuo Account Executive.
* È consigliabile scrivere queste espressioni prima in un editor di testo, ad esempio in Sublime o in Visual Studio Code, in quanto ciò consente di visualizzare i dati in modo più chiaro rispetto a quelli visualizzati in Workfront.

## Componenti di un’istruzione &quot;IF&quot;

È possibile creare istruzioni &quot;IF&quot; in Workfront utilizzando il seguente formato:
<pre>IF(Condizione,Espressione True,Espressione False)</pre>I componenti di un'istruzione "IF" sono:

* **IF**= Espressione di dati calcolata Workfront per &quot;function&quot;. Simile alle espressioni SUM e PROD, questo indica al sistema di comprendere la funzione come istruzione &quot;IF&quot;. Utilizzare sempre lettere maiuscole per &quot;IF&quot; in questa dichiarazione.\
   Per un elenco di tutte le espressioni dati calcolate, vedi [Espressioni dati calcolate](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **Condizione**= Questa è la condizione che la variabile Workfront deve soddisfare ed è la base di questa equazione. Tutto ciò che può essere successivamente specificato nell&#39;equazione dipende dalla condizione. È possibile utilizzare un numero di riferimenti, confronti o espressioni matematiche per avviare un&#39;equazione. Alcuni esempi di condizioni sono:

   * Una data è maggiore di un&#39;altra data in un oggetto specificato.
   * Uno stato è uguale a uno degli stati disponibili per un oggetto specificato.
   * La percentuale di completamento di un&#39;attività è minore o maggiore di una determinata percentuale.

* **Operatore condizione** = questo è l&#39;operatore che consente di creare la condizione dell&#39;istruzione &quot;IF&quot;. Ad esempio, &quot;è uguale a&quot; o &quot;è maggiore di&quot; sono operatori di condizioni. Per un elenco degli operatori di condizioni utilizzabili nelle istruzioni, consulta [Operatori di condizione nelle espressioni personalizzate calcolate](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* **True****Expression**= Questa è la variabile &quot;True&quot;, che indica all&#39;equazione quale indicatore visualizzare una volta soddisfatti i criteri della condizione (indicatori true).

* **Espressione False**= Questa è la variabile &quot;False&quot;, che indica all&#39;equazione quale indicatore visualizzare quando i criteri della condizione non sono soddisfatti (indicatori falsi).

Nell&#39;esempio seguente, il formato dell&#39;istruzione originale viene utilizzato per scrivere un&#39;espressione di dati semplice per un&#39;istruzione &quot;IF&quot;. L&#39;espressione confronta due campi data diversi in Workfront, seguiti da un risultato True/False come stringa dati:

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

Nel discorso quotidiano, questa affermazione significherebbe: Se la data di completamento prevista dell&#39;oggetto è &quot;Maggiore di&quot; la data di completamento pianificata dello stesso oggetto, in questo campo vengono visualizzate le parole &quot;Disattivato brano&quot;. In caso contrario, visualizzare le parole &quot;Sulla traccia&quot;.

## Creare campi calcolati in moduli personalizzati o colonne personalizzate utilizzando istruzioni &quot;IF&quot;

È possibile creare istruzioni &quot;IF&quot; in un campo calcolato in un modulo personalizzato o in una colonna personalizzata.

C&#39;è una differenza nella sintassi utilizzata in un modulo personalizzato calcolato rispetto a una colonna personalizzata calcolata. Fai riferimento ai seguenti esempi:

* [Dichiarazioni singole &quot;IF&quot;](#single-if-statements)
* [Istruzioni &quot;IF&quot; multiple](#multiple-if-statements)

### Dichiarazioni singole &quot;IF&quot; {#single-if-statements}

Di seguito sono riportati alcuni esempi di un campo personalizzato calcolato e la colonna corrispondente utilizzando un&#39;istruzione &quot;IF&quot;:

* Campo personalizzato calcolato:

Quando si crea un campo personalizzato, utilizzare la sintassi seguente per un&#39;istruzione &quot;IF&quot;:

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* Colonna personalizzata calcolata:

Quando si crea una colonna personalizzata, è necessario utilizzare la sintassi seguente per l&#39;istruzione &quot;IF&quot; nella riga di espressione del valore:

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### Istruzioni &quot;IF&quot; multiple {#multiple-if-statements}

Per creare un’espressione più complessa e dinamica, è possibile combinare più istruzioni &quot;IF&quot; con la seguente istruzione:

<pre>IF(Condition1,Espressione True,IF(Condition2,Espressione True,Espressione False)</pre>Nota che non esiste più alcuna istruzione falsa per il primo "IF". Invece, l'abbiamo sostituito con l'inizio di un secondo "IF".

Di seguito sono riportati alcuni esempi di un campo personalizzato calcolato e la relativa colonna personalizzata utilizzando più istruzioni &quot;IF&quot;:

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

Il modo migliore per imparare questo è sperimentare vari campi e scenari. Inoltre, acquisisci familiarità con API Explorer, che rivela i nomi di campo che possono essere utilizzati. Per informazioni su API Explorer, consulta [Esplora API](../../../wf-api/general/api-explorer.md).

Per ulteriori informazioni sulla sintassi Workfront delle espressioni dati calcolate, consulta [Espressioni dati calcolate](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
