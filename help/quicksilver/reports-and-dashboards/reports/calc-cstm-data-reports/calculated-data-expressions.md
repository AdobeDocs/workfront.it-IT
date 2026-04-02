---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Panoramica delle espressioni di dati calcolati
description: Puoi utilizzare le espressioni di dati per definire campi di dati personalizzati calcolati in Adobe Workfront. Le espressioni calcolate collegano i campi Workfront esistenti all’interno di istruzioni che generano un nuovo campo.
author: Courtney, Lisa
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '2551'
ht-degree: 100%

---

# Panoramica delle espressioni di dati calcolati

<!--Audited: 12/2023-->

Puoi utilizzare le espressioni di dati per definire campi personalizzati calcolati in Adobe Workfront. Le espressioni calcolate collegano i campi Workfront esistenti all’interno di istruzioni che generano un nuovo campo.

Puoi utilizzare le espressioni di dati calcolati in:

* Un campo personalizzato calcolato in un modulo personalizzato

  Per ulteriori informazioni sulla creazione di campi personalizzati calcolati nei moduli personalizzati in Workfront, consulta [Aggiungere campi calcolati a un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Una colonna personalizzata calcolata in un rapporto o in un elenco quando utilizzi la modalità testo

  Per ulteriori informazioni sull’utilizzo della modalità testo nei rapporti e nelle viste, consulta [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Sintassi dei campi personalizzati calcolati rispetto alle colonne personalizzate calcolate

Sebbene le funzioni utilizzate siano le stesse, la sintassi per la creazione di un’espressione in un campo personalizzato calcolato può essere diversa da quella per la creazione di una colonna personalizzata calcolata.

Le differenze tra le due sintassi sono:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Campo personalizzato calcolato</strong></td> 
   <td><strong>Elemento di reporting personalizzato calcolato</strong></td> 
  </tr> 
   <td>Racchiudi i nomi dei campi tra parentesi graffe</td> 
   <td>Non racchiudere i nomi dei campi tra parentesi quadre o tonde quando li utilizzi in una <p><code>valuefield </code></p>riga. <p>Racchiudi i nomi dei campi tra parentesi graffe quando li utilizzi in una <p><code>valueexpression</code></p> riga.</p> </td> 
  </tr> 
  <tr> 
   <td>Separa i campi con dei punti</td> 
   <td> <p>Separa i campi con i due punti quando li utilizzi in una <p><code>valuefield </code></p>riga</p> <p>Separa i campi per punti quando li utilizzi in una <p><code>valueexpression </code></p>riga. </p> </td> 
  </tr> 
 </tbody> 
</table>

Ad esempio:

* In un campo personalizzato, in un modulo personalizzato per le attività, dovresti utilizzare quanto segue per generare il nome del progetto principale dell’attività a cui è allegato il modulo personalizzato:


  `{project}.{name}`


* In una colonna personalizzata di un rapporto, utilizza quanto segue per aggiungere una colonna personalizzata Nome progetto a un rapporto di attività:


  `valuefield=project:name`


  Oppure

  `valueexpression={project}.{name}`


  >[!TIP]
  >
  >La stessa sintassi si applica a tutti gli elementi di reporting in modalità testo in cui vengono utilizzate le espressioni calcolate: viste, filtri, raggruppamenti, prompt.

Per ulteriori informazioni sulla sintassi da utilizzare in una colonna personalizzata calcolata, consulta [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Espressioni di dati utilizzabili

Gli elenchi seguenti definiscono le espressioni disponibili da utilizzare per la creazione di uno dei 3 diversi tipi di campi personalizzati calcolati in Workfront:

* [Campi personalizzati calcolati per data e ora](#date-time-calculated-custom-fields)
* [Campi personalizzati calcolati matematici](#mathematical-calculated-custom-fields)
* [Campi personalizzati calcolati di tipo testo](#text-calculated-custom-fields)

Puoi utilizzare le espressioni elencate di seguito per creare colonne personalizzate calcolate. Tuttavia, è necessario utilizzare la sintassi corretta per una colonna personalizzata calcolata, come descritto nella sezione [Sintassi dei campi personalizzati calcolati rispetto alle colonne personalizzate calcolate](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) in questo articolo.

### Campi personalizzati calcolati per data e ora {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Se crei un calcolo di data e ora che non include una parte oraria o che utilizza i caratteri jolly $$TODAY o $$NOW, il sistema utilizza la data in base al fuso orario UTC (Tempo coordinato universale) e non al fuso orario locale. Questo può causare un risultato di data imprevisto.

Puoi creare un campo personalizzato calcolato per data od ora utilizzando le seguenti espressioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Espressione</th> 
   <th>Spiegazione ed esempio</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ADDDAYS</strong> </td> 
   <td> <p>Aggiunge il numero di ore alla data. Il valore numerico può includere giorni parziali. Ad esempio, 1,5 aggiunge un giorno e mezzo alla data.</p> <p>L’espressione è formattata nel modo seguente:</p>

<p><code>ADDDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>Aggiunge il numero di giorni della settimana alla data. Questa espressione aggiunge alla data solo valori interi, con arrotondamento per difetto. </p> <p>L’espressione è formattata nel modo seguente:</p>

<p><code>ADDWEEKDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Aggiunge il numero di mesi alla data ed è formattata nel modo seguente:

</p><p><code>ADDMONTHS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Aggiunge il numero di anni alla data ed è formattata nel modo seguente:</p>

<p><code>ADDYEARS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDHOURS</strong> </td> 
   <td> <p>Aggiunge il numero di ore alla data ed è formattata nel modo seguente:</p>

<p><code>ADDHOUR(date, number)</code></p>
   <p>Nota: questa espressione non è supportata in Pianificazione di Workfront.</p></td> 
  </tr>
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Cancella la porzione di ora di una data ed è formattata nel modo seguente: In questo esempio, la data corrisponde alla data di inserimento di un oggetto di lavoro.</p>

<p><code>CLEARTIME({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATE</strong> </td> 
   <td> <p>Converte una stringa in una data ed è formattata nel modo seguente:</p>

<p><code>DATE(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Restituisce il numero di giorni tra le due date, tenendo conto sia dei giorni di inizio e di fine del periodo selezionato e sia delle marche temporali in tali giorni. Ad esempio, se l’ora di inizio della data di inizio corrisponde alle 15:00, il giorno di inizio non sarà conteggiato come giorno intero.</p> <p>L’espressione è formattata nel modo seguente:</p>

<p><code>DATEDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Restituisce il giorno del mese della data sotto forma di numero compreso tra 1 e 31.</p> <p>L’espressione è formattata nel modo seguente: In questo esempio, la data corrisponde alla data di inserimento di un oggetto di lavoro.</p>

<p><code>DAYOFMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Restituisce il giorno della settimana della data sotto forma di numero compreso tra 1 (domenica) e 7 (sabato).</p> <p>L’espressione è formattata nel modo seguente: In questo esempio, la data corrisponde alla data di inserimento di un oggetto di lavoro.</p>

<p><code>DAYOFWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Restituisce il totale dei giorni del mese della data sotto forma di numero ed è formattata nel modo seguente: In questo esempio, la data corrisponde alla data di inserimento di un oggetto di lavoro.</p>

<p><code>DAYSINMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Restituisce il totale di giorni della settimana tra la data e la fine della settimana o la fine del mese, a seconda di quale delle due si verifichi prima. In questo esempio, la data corrisponde alla data di inserimento di un oggetto di lavoro.</p> <p>L’espressione è formattata nel modo seguente:</p>

<p><code>DAYSINSPLITWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Restituisce il totale dei giorni dell’anno della data sotto forma di numero ed è formattata nel modo seguente. In questo esempio, la data corrisponde alla data di inserimento di un oggetto di lavoro.</p>

<p><code>DAYSINYEAR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Restituisce la data più recente nell’elenco ed è formattata nel modo seguente:</p>

<p><code>DMAX(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Restituisce la data meno recente dell’elenco ed è formattata nel modo seguente:</p>

<p><code>DMIN(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>HOUR</strong> </td> 
   <td> <p>Restituisce l’ora della data sotto forma di numero compreso tra 0 e 23.</p> <p>L’espressione è formattata nel modo seguente: In questo esempio, la data corrisponde alla data di inserimento di un oggetto di lavoro.</p>

<p><code>HOUR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>Restituisce il minuto della data sotto forma di numero compreso tra 0 e 60 ed è formattata nel modo seguente. In questo esempio, la data corrisponde alla data di inserimento di un oggetto di lavoro.</p>

<p><code>MINUTE({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MONTH</strong> </td> 
   <td> <p>Restituisce il mese della data sotto forma di numero compreso tra 1 e 12 ed è formattata nel modo seguente. In questo esempio, la data corrisponde alla data di inserimento di un oggetto di lavoro.</p>

<p><code>MONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>Restituisce il secondo della data sotto forma di numero compreso tra 0 e 60 ed è formattata nel modo seguente. In questo esempio, la data corrisponde alla data di inserimento di un oggetto di lavoro.</p>

<p><code>SECOND({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>Restituisce il numero di giorni della settimana tra le due date, tenendo conto sia dei giorni di inizio e di fine del periodo selezionato e sia delle marche temporali in tali giorni. Ad esempio, se l’ora di inizio della data di inizio corrisponde alle 15:00, il giorno di inizio non sarà conteggiato come giorno intero.</p> <p>L’espressione è formattata nel modo seguente:</p>

<p><code>WEEKDAYDIFF(date2, date1)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Restituisce il numero di minuti pianificati tra due date secondo la pianificazione predefinita.</p> <p>L’espressione è formattata nel modo seguente:</p>

<p><code>WORKMINUTESDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>YEAR</strong> </td> 
   <td> <p>Restituisce l’anno della data sotto forma di numero a 4 cifre ed è formattata nel modo seguente. In questo esempio, la data corrisponde alla data di inserimento di un oggetto di lavoro.</p>

<p><code>YEAR({entryDate})</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### Campi personalizzati matematici calcolati {#mathematical-calculated-custom-fields}

Puoi creare un campo personalizzato calcolato che utilizza alcune delle seguenti espressioni matematiche:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Espressione</th> 
   <th>Spiegazione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ABS</strong> </td> 
   <td>Restituisce il valore assoluto del numero ed è formattata nel modo seguente. In questo esempio viene utilizzato il numero di oggetti sotto l’oggetto a cui è associato il modulo personalizzato.

<p><code>ABS({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>Restituisce la media dei numeri ed è formattata nel modo seguente:

<p><code>AVERAGE(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Arrotonda un numero per eccesso al numero intero più vicino ed è formattata nel modo seguente. In questo esempio viene utilizzato il numero di oggetti sotto l’oggetto a cui è associato il modulo personalizzato.

<p><code>CEIL({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Divide tutti i numeri nell’ordine indicato ed è formattata nel modo seguente:

<p><code>DIV(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>Arrotonda un numero per difetto al numero intero più vicino ed è formattata nel modo seguente. In questo esempio viene utilizzato il numero di oggetti sotto l’oggetto a cui è associato il modulo personalizzato.

<p><code>FLOOR({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Restituisce il valore del logaritmo naturale del numero ed è formattata nel modo seguente:

<p><code>LN({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Restituisce il valore del logaritmo di number2 in base a number1 ed è formattata nel modo seguente:

<p><code>LOG(number1, number2)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Restituisce l’elemento più grande dell’elenco ed è formattata nel modo seguente:

<p><code>MAX(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Restituisce l’elemento più piccolo dell’elenco ed è formattata nel modo seguente:

<p><code>MIN(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>NUMBER</strong> </td> 
   <td>Converte una stringa in un numero ed è formattata nel modo seguente:<p><code>NUMBER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>Restituisce un numero elevato a potenza ed è formattata nel modo seguente:

<p><code>POWER(number, power)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Moltiplica tutti i numeri ed è formattata nel modo seguente:

<p><code>PROD(number1, number2, ....)</code></p>
   <p><b>NOTA</b></p>

<p>Quando moltiplichi i campi che contengono ore, verifica che il database salvi le ore nei campi selezionati in minuti, ore o secondi. Se le ore vengono salvate in minuti o secondi ma visualizzate in ore nell’interfaccia di Workfront, potrebbe essere necessario tenere conto della conversione da minuti o secondi a ore durante la scrittura di un’espressione utilizzando questo calcolo. </p>
   </td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>Arrotonda il numero per eccesso alla precisione di decimali specificata ed è formattata nel modo seguente:

<p><code>ROUND(number, precision)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Ordina i numeri in ordine crescente ed è formattata nel modo seguente:</p>

<p><code>SORTASCNUM(number1,number2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Ordina i numeri in ordine decrescente ed è formattata nel modo seguente:

<p><code>SORTDESCNUM(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Restituisce la radice quadrata di un numero ed è formattata nel modo seguente: In questo esempio viene utilizzato il numero di oggetti sotto l’oggetto a cui è associato il modulo personalizzato.</p>

<p><code>SQRT({numberOfChildren})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Sottrae tutti i numeri nell’ordine fornito ed è formattata nel modo seguente:

<p><code>SUB(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>Somma tutti i numeri ed è formattata nel modo seguente:

<p><code>SUM(number1, number2, ...)</code></p></td> 
  </tr> 
 </tbody> 
</table>

### Campi personalizzati calcolati di tipo testo {#text-calculated-custom-fields}

Puoi creare un campo personalizzato calcolato che mostri un valore in formato testo utilizzando le seguenti espressioni:

<table style="table-layout:auto:fixed"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Espressione</th> 
   <th>Spiegazione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ARRAY</strong> </td> 
   <td> <p>Converte una stringa in un array. Il delimitatore può essere una qualsiasi stringa.</p> 
   <p>L’espressione è formattata nel modo seguente:</p>
   <p><code>ARRAY(string1, "delimiter")</code></p> 
   </td> 
  </tr>

<tr> 
   <td><strong>ARRAYCONTAINS</strong> </td> 
   <td> <p>Cerca un valore specifico in un elenco o array. Se il valore viene trovato, la funzione restituisce True, altrimenti restituisce False. </p> 
   <p>L’espressione è formattata nel modo seguente:</p>
   <p><code>ARRAYCONTAINS(array, value)</code></p> 
   </td> 
  </tr>


<tr> 
   <td><strong>ARRAYLENGTH</strong> </td> 
   <td> <p>Restituisce il numero di elementi nell’array ed è formattata nel modo seguente:</p>
   <p><code>ARRAYLENGTH(array)</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>ARRAYELEMENT</strong> </td> 
   <td> <p>Restituisce l’elemento al numero specificato nell’array. Se l’indice è fuori dai limiti, lo restituisce vuoto.</p> 
   <p>L’espressione è formattata nel modo seguente:</p>
   <p><code>ARRAYELEMENT(array, number)</code></p> 
   </td> 
  </tr>

<tr>   
   <td><strong>CASE</strong> </td> 
   <td> <p>Viene utilizzato con altre espressioni per scegliere un valore da un elenco in base a un numero di indice. </p>
   <p>Un numero di indice è un campo o una funzione che restituisce un valore numerico (in genere in un intervallo noto).</p> 
   <p>L’espressione è formattata nel modo seguente:</p>
   <p><code>CASE(indexNumber, value1, value2, ...)</code></p>

<p>Ad esempio, l’espressione seguente restituisce il nome del giorno della settimana, dove 1=domenica, 2=lunedì e così via, in una colonna calcolata:</p>

<p><code>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</code></p>

<p>Funziona meglio con altre espressioni che restituiscono un numero, come DAYOFWEEK, DAYOFMONTH e MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>Concatena la stringa ed è formattata nel modo seguente:</p><p><code>CONCAT(string1,"separator", string2)</code></p> <p>Di seguito sono riportati alcuni esempi di separatori che puoi includere:</p> 
    <ul> 
     <li>uno spazio: “ ”</li> 
     <li>un trattino: “-”</li> 
     <li>una barra: “/”</li> 
     <li>una virgola: “,”</li> 
     <li>una parola: “or”, “and”</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>CONTAINS</strong> </td> 
   <td>Restituisce True se la stringa findText viene trovata all’interno della stringa withinText ed è formattata nel modo seguente:

<p><code>CONTAINS(findText, withinText)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Applica l’escape di tutti i caratteri speciali della stringa in modo che possano essere inclusi in un argomento URL.<p>L’espressione è formattata nel modo seguente:</p>

<p><code>ENCODEURL(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FORMAT</strong> </td> 
   <td><p>Restituisce il testo formattato. Con FORMAT sono consentite solo le opzioni dei parametri elencate qui.</p>
   <p>Le opzioni colore sono $$POSITIVE, $$INFORMATIVE, $$NEGATIVE, $$NOTICE e le altre opzioni di formattazione sono $$BOLD, $$ITALIC, $$UNDERLINE. È consentita una sola opzione colore, insieme a un massimo di tre altre opzioni di formattazione. Se non viene specificata alcuna opzione colore, viene applicato il colore predefinito del sistema.</p>
   <p>L’espressione è formattata nel modo seguente:</p>
   <p><code>FORMAT($$POSITIVE, $$BOLD, $$ITALIC)</code></p>
   <p>Nota: questa espressione non è supportata in Pianificazione di Workfront.</p></td> 
  </tr>   
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>Valuta una condizione specificata e restituisce il valore di trueExpression se è true oppure il valore di falseExpression se è false.</p>

<p>L’espressione è formattata nel modo seguente:</p>

<p><code>IF(condition, trueExpression, falseExpression)</code></p>

<p>Ad esempio, puoi confrontare due diversi campi data seguiti da un risultato True/False come stringa di dati:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</code></p>

<p>Nel linguaggio colloquiale, questa istruzione significa: “SE la data di completamento prevista del mio oggetto è ‘Successiva a’ la data di completamento pianificata del mio stesso oggetto, allora mostra le parole ‘In ritardo’ in questo campo; in caso contrario, mostra le parole ‘In linea con la pianificazione’”.</p>

<p>Se non desideri etichettare le espressioni true o false, è necessario inserire un’etichetta vuota nell’istruzione, ad esempio:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</code></p> 
   <p>Oppure</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</code></p>

<p>Per ulteriori informazioni sulla creazione delle istruzioni “IF”, consulta <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">Panoramica delle istruzioni “IF”</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Consente di cercare un valore specifico in una stringa di valori possibili. Se il valore che stai cercando è uguale a uno dei valori specificati, l’espressione restituisce trueExpression; in caso contrario, restituisce falseExpression.</p> 
   <p>L’espressione è formattata nel modo seguente:</p>

<p><code>IFIN(value, value1, value2,..., trueExpression, falseExpression)</code></p>

<p>Ad esempio, puoi trovare un proprietario del progetto specifico e contrassegnare tali progetti con un tag specificato in una vista di progetto: <br><p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")
   </code></p>
    <p> Nel linguaggio colloquiale, questa dichiarazione significa: “Se il proprietario del progetto è Jennifer Campbell o Rick Kuvec, contrassegna questo progetto con ‘Team di marketing’; altrimenti, contrassegnalo con ‘Altri team’”.</p> 
    <p> Se non desideri etichettare le espressioni true o false, è necessario inserire un’etichetta vuota nell’istruzione, ad esempio: </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> 
    <p>Oppure </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","")</code></p> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>Restituisce true se il valore è uguale a uno dei valori specificati; in caso contrario, l’espressione restituisce false.</p> <p>L’espressione è formattata nel modo seguente:

</p><p><code>IN(value, value1[, value2...])</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Restituisce true se il valore è null o vuoto; in caso contrario, l’espressione restituisce false.</p> <p>L’espressione è formattata nel modo seguente:

</p><p><code>ISBLANK(value)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEFT</strong> </td> 
   <td> <p>Restituisce un numero specificato di caratteri dalla parte sinistra di una stringa ed è formattata nel modo seguente:</p>

<p><code>LEFT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Restituisce la lunghezza di una stringa ed è formattata nel modo seguente:</p>

<p><code>LEN(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>Restituisce la stringa in minuscolo ed è formattata nel modo seguente:

<p><code>LOWER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PASCAL</strong> </td> 
   <td> <p>Converte la stringa di input in PascalCase trasformando in maiuscolo la prima lettera di ciascuna parola e rimuovendo tutti gli spazi. </p>
   <p>L’espressione è formattata nel modo seguente:</p>
   <p><code>PASCAL(string) </code></p>
   <p>Ad esempio, “hello world” diventa “HelloWorld”</p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>REMOVEACCENTS</strong> </td> 
   <td> <p>Rimuove i segni diacritici da tutti i caratteri accentati nella stringa di input. </p> 
   <p>L’espressione è formattata nel modo seguente:</p>
   <p><code>REMOVEACCENTS(string)</code></p> 
   <p>Ad esempio, “Héllo wörld con àccénti” diventa “Hello world con accenti”. </p>
   </td> 
  </tr>
  <tr> 
   <td><strong>REPLACE</strong> </td> 
   <td> <p>Sostituisce tutte le occorrenze di stringa2 con stringa3 nella stringa1.</p> <p>L’espressione è formattata nel modo seguente:</p>

<p><code>REPLACE(string1, string2, string3)</code></p> </td> 
  </tr>

<tr> 
   <td><strong>REPLACEPATTERN</strong> </td> 
   <td> <p>Sostituisce le corrispondenze del pattern specificato con la stringa di sostituzione. </p> 
   <p>L’espressione è formattata nel modo seguente:</p>
   <p><code>REPLACEPATTERN (string, pattern, replacement string)</code></p> 
   <p>Ad esempio, REPLACEPATTERN("foo123bar", "\d+", "_") genera la stringa “foo_bar”.
   </td> 
  </tr> 
  <tr> 
   <td><strong>RIGHT</strong> </td> 
   <td> <p>Restituisce un numero specificato di caratteri dalla parte destra di una stringa ed è formattata nel modo seguente:</p>

<p><code>RIGHT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>Restituisce l’indice della prima occorrenza di findText nella stringa withinText, a partire dalla posizione di avvio specificata o -1 se il testo non viene trovato.</p> <p>L’espressione è formattata nel modo seguente:</p>

<p><code>SEARCH(findText, withinText, start)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCARRAY</strong> </td> 
   <td> <p>Ordina gli elementi dell’array in ordine crescente e li converte nel tipo del primo elemento.</p>
   <p>L’espressione è formattata nel modo seguente:</p>
   <p><code>SORTASCARRAY(array)</code></p>
   <p>Ad esempio, [“-12,6”, -13,0] diventa [“-12,6”, “-13”].</p>
   <p>Nota: questa espressione non è supportata in Pianificazione di Workfront.</p></td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCARRAY</strong> </td> 
   <td> <p>Ordina gli elementi dell’array in ordine decrescente e li converte nel tipo del primo elemento.</p>
   <p>L’espressione è formattata nel modo seguente:</p>
   <p><code>SORTDESCARRAY(array)</code></p>
   <p>Ad esempio, [“-12,6”, -13,0] diventa [“-13”, “-12,6”].</p>
   <p>Nota: questa espressione non è supportata in Pianificazione di Workfront.</p></td> 
  </tr>
  <tr> 
   <td><strong>STRING</strong> </td> 
   <td> <p>Converte un numero in una stringa ed è formattata come segue:nel modo seguente:</p>

<p><code>STRING(number)</code></p> </td> 
  </tr>
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Ordina un elenco di stringhe in ordine crescente ed è formattata come segue:nel modo seguente:</p>
   <p><code>SORTASCSTRING(string1, string2, ...)</code></p> </td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Ordina un elenco di stringhe in ordine decrescente ed è formattata come segue:nel modo seguente:</p>
   <p><code>SORTDESCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Restituisce i caratteri di una stringa in base all’indice iniziale e finale specificato ed è formattata come segue:nel modo seguente:</p>

<p><code>SUBSTR({string}, number of start position, number of end position)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SWITCH</strong> </td> 
   <td> <p>Valuta l’espressione rispetto a un elenco di valori e restituisce il risultato che corrisponde al primo valore corrispondente.</p>
   <p>L’espressione è formattata nel modo sguente:</p>
   <p><code>SWITCH(expression, value1, result1, [value2, result2], ...)</code></p>
   <p>Questa espressione non è supportata in Pianificazione di Workfront.</p></td> 
  </tr>   
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>Rimuove lo spazio vuoto dall’inizio e dalla fine di una stringa ed è formattata nel modo seguente:</p>

<p><code>TRIM(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>Restituisce una stringa in maiuscolo ed è formattata nel modo seguente:</p>

<p><code>UPPER(string)</code></p> </td> 
  </tr> 
 </tbody> 
</table>

