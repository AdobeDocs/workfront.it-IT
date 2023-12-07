---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Panoramica delle espressioni di dati calcolati
description: Puoi utilizzare le espressioni di dati per definire campi di dati personalizzati calcolati in Adobe Workfront. Le espressioni calcolate collegano i campi Workfront esistenti nelle istruzioni che generano un nuovo campo.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 26aa5a1f9b0fd88c83d9967245d2a8149d39b607
workflow-type: tm+mt
source-wordcount: '2166'
ht-degree: 0%

---

# Panoramica delle espressioni di dati calcolati

Puoi utilizzare le espressioni di dati per definire campi personalizzati calcolati in Adobe Workfront. Le espressioni calcolate collegano i campi Workfront esistenti nelle istruzioni che generano un nuovo campo.

Puoi utilizzare espressioni di dati calcolati in:

* Campo personalizzato calcolato in un modulo personalizzato

  Per ulteriori informazioni sulla creazione di campi personalizzati calcolati nei moduli personalizzati in Workfront, consulta [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* Colonna personalizzata calcolata in un report o in un elenco quando si utilizza la modalità testo

  Per ulteriori informazioni sull&#39;utilizzo della modalità testo nei report e nelle visualizzazioni, vedere [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Sintassi dei campi personalizzati calcolati rispetto alle colonne personalizzate calcolate

Sebbene le funzioni utilizzate siano le stesse, la sintassi per la creazione di un&#39;espressione in un campo personalizzato calcolato può essere diversa da quella per la creazione di una colonna personalizzata calcolata.

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
   <td>Non racchiudere i nomi dei campi tra parentesi quadre o parentesi quando li si utilizza in un <p><code>valuefield </code></p>linea. <p>Racchiudi i nomi dei campi tra parentesi graffe quando li utilizzi in una <p><code>valueexpression</code></p> linea.</p> </td> 
  </tr> 
  <tr> 
   <td>Separa i campi per periodi</td> 
   <td> <p>Separa i campi con due punti quando li utilizzi in una <p><code>valuefield </code></p>linea</p> <p>Separa i campi per punti quando li utilizzi in una <p><code>valueexpression </code></p>linea. </p> </td> 
  </tr> 
 </tbody> 
</table>

Ad esempio:

* In un campo personalizzato, in un modulo personalizzato per le attività, puoi utilizzare quanto segue per generare il nome del progetto principale dell’attività a cui è allegato il modulo personalizzato:

  ```
  {project}.{name}
  ```

* In una colonna personalizzata di un report, utilizzare quanto segue per aggiungere una colonna personalizzata Nome progetto a un report attività:

  ```
  valuefield=project:name
  ```

  Oppure

  ```
  valueexpression={project}.{name}
  ```

  >[!TIP]
  >
  >La stessa sintassi si applica a tutti gli elementi di reporting in modalità testo in cui vengono utilizzate espressioni calcolate: viste, filtri, raggruppamenti, prompt.

Per ulteriori informazioni sulla sintassi da utilizzare in una colonna personalizzata calcolata, consulta [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Espressioni dati utilizzabili

Gli elenchi seguenti definiscono le espressioni disponibili da utilizzare per la creazione di uno dei tre diversi tipi di campi personalizzati calcolati in Workfront:

* [Campi personalizzati calcolati per data e ora](#date-time-calculated-custom-fields)
* [Campi personalizzati matematici calcolati](#mathematical-calculated-custom-fields)
* [Testo dei campi personalizzati calcolati](#text-calculated-custom-fields)

Puoi utilizzare le espressioni elencate di seguito per creare colonne personalizzate calcolate. Tuttavia, devi utilizzare la sintassi corretta per una colonna personalizzata calcolata, come descritto nella sezione  [Sintassi dei campi personalizzati calcolati rispetto alle colonne personalizzate calcolate](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) in questo articolo.

### Campi personalizzati calcolati per data e ora {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Se crei un calcolo di data e ora che non include una porzione di ora o che utilizza i caratteri jolly $$TODAY o $$NOW, il sistema utilizza la data in base al fuso orario UTC (Coordinated Universal Time) e non al fuso orario locale. Questo può causare un risultato di data imprevisto.

Puoi creare un campo personalizzato calcolato per la data o l’ora utilizzando le seguenti espressioni:

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
   <td> <p>Aggiunge il numero di giorni alla data. Il valore numerico può includere giorni parziali. Ad esempio, 1.5 aggiunge un giorno e mezzo alla data.</p> <p>L’espressione viene formattata come segue:</p>

<p><code>ADDDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>Aggiunge il numero di giorni della settimana alla data. Questa espressione aggiunge alla data solo valori interi, con arrotondamento per difetto. </p> <p>L’espressione viene formattata come segue:</p>

<p><code>ADDWEEKDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Aggiunge il numero di mesi alla data e viene formattato come segue:

</p><p><code>ADDMONTHS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Aggiunge il numero di anni alla data e viene formattato come segue:</p>

<p><code>ADDYEARS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Cancella la porzione di ora di una data e viene formattata come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p>

<p><code>CLEARTIME({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATA</strong> </td> 
   <td> <p>Converte una stringa in una data e viene formattata come segue:</p>

<p><code>DATE(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Restituisce il numero di giorni tra le due date, tenendo conto dei giorni di inizio e di fine del periodo selezionato e delle marche temporali in tali giorni. Ad esempio, se l’ora di inizio della data di inizio è le 15, il giorno di inizio non viene conteggiato come giorno intero.</p> <p>L’espressione viene formattata come segue:</p>

<p><code>DATEDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Restituisce il giorno del mese per la data come numero, compreso tra 1 e 31.</p> <p>L’espressione viene formattata come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p>

<p><code>DAYOFMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Restituisce il giorno della settimana per la data come numero, compreso tra 1 (domenica) e 7 (sabato).</p> <p>L’espressione viene formattata come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p>

<p><code>DAYOFWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Restituisce il totale dei giorni del mese della data sotto forma di numero e viene formattato come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p>

<p><code>DAYSINMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Restituisce il numero totale di giorni della settimana compresi tra la data e la fine della settimana oppure la fine del mese, a seconda di quale dei due eventi si verifichi per primo. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p> <p>L’espressione viene formattata come segue:</p>

<p><code>DAYSINSPLITWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Restituisce il totale dei giorni dell’anno della data sotto forma di numero e viene formattato come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p>

<p><code>DAYSINYEAR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Restituisce la data più recente nell'elenco e viene formattato come segue:</p>

<p><code>DMAX(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Restituisce la prima data dell'elenco e viene formattata come segue:</p>

<p><code>DMIN(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ORA</strong> </td> 
   <td> <p>Restituisce l’ora della data come numero compreso tra 0 e 23.</p> <p>L’espressione viene formattata come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p>

<p><code>HOUR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTO</strong> </td> 
   <td> <p>Restituisce il minuto della data come numero compreso tra 0 e 60, formattato come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p>

<p><code>MINUTE({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MESE</strong> </td> 
   <td> <p>Restituisce il mese della data come numero compreso tra 1 e 12, formattato come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p>

<p><code>MONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>Restituisce il secondo della data come numero compreso tra 0 e 60, formattato come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p>

<p><code>SECOND({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>Restituisce il numero di giorni feriali tra due date, tenendo conto dei giorni di inizio e di fine del periodo selezionato e delle marche temporali in tali giorni. Ad esempio, se l’ora di inizio della data di inizio è le 15.00, il giorno di inizio non verrà conteggiato come giorno intero.</p> <p>L’espressione viene formattata come segue:</p>

<p><code>WEEKDAYDIFF(date2, date1)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Restituisce il numero di minuti programmati tra le date in base alla pianificazione predefinita.</p> <p>L’espressione viene formattata come segue:</p>

<p><code>WORKMINUTESDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ANNO</strong> </td> 
   <td> <p>Restituisce l'anno della data come numero a 4 cifre, formattato come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p>

<p><code>YEAR({entryDate})</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### Campi personalizzati matematici calcolati {#mathematical-calculated-custom-fields}

È possibile creare un campo personalizzato calcolato che utilizza alcune delle seguenti espressioni matematiche:

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
   <td>Restituisce il valore assoluto del numero ed è formattato come segue. In questo esempio viene utilizzato il numero di oggetti sotto l'oggetto a cui è allegato il modulo personalizzato.

<p><code>ABS({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MEDIA</strong> </td> 
   <td>Restituisce la media dei numeri ed è formattato come segue:

<p><code>AVERAGE(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Arrotonda un numero per eccesso al numero intero più vicino e viene formattato come segue. In questo esempio viene utilizzato il numero di oggetti sotto l'oggetto a cui è allegato il modulo personalizzato.

<p><code>CEIL({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Divide tutti i numeri nell’ordine indicato e viene formattato come segue:

<p><code>DIV(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>Arrotonda un numero per difetto al numero intero più vicino e viene formattato come segue. In questo esempio viene utilizzato il numero di oggetti sotto l'oggetto a cui è allegato il modulo personalizzato.

<p><code>FLOOR({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Restituisce il valore logaritmo naturale del numero ed è formattato come segue:

<p><code>LN({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Restituisce il valore logaritmico numero2 al numero base 1 ed è formattato come segue:

<p><code>LOG(number1, number2)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Restituisce l'elemento più grande dell'elenco e viene formattato come segue:

<p><code>MAX(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Restituisce l'elemento più piccolo dell'elenco e viene formattato come segue:

<p><code>MIN(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>NUMERO</strong> </td> 
   <td>Converte una stringa in un numero e viene formattato come segue:<p><code>NUMBER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>Restituisce un numero elevato a potenza e viene formattato come segue:

<p><code>POWER(number, power)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Moltiplica tutti i numeri e viene formattato come segue:

<p><code>PROD(number1, number2, ....)</code></p>
   <p><b>NOTA</b></p>

<p>Quando si moltiplicano i campi che contengono ore, verificare che il database salvi le ore nei campi selezionati in minuti, ore o secondi. Se le ore vengono salvate in minuti o secondi ma visualizzate in ore nell’interfaccia di Workfront, potrebbe essere necessario tenere conto della conversione da minuti o secondi a ore durante la scrittura di un’espressione utilizzando questo calcolo. </p>
   </td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>Arrotonda il numero per eccesso ai decimali di precisione specificati e viene formattato come segue:

<p><code>ROUND(number, precision)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Ordina i numeri in ordine crescente e viene formattato come segue:</p>

<p><code>SORTASCNUM(number1,number2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Ordina i numeri in ordine decrescente e viene formattato come segue:

<p><code>SORTDESCNUM(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Restituisce una radice quadrata di un numero ed è formattata come segue. In questo esempio viene utilizzato il numero di oggetti sotto l'oggetto a cui è allegato il modulo personalizzato.</p>

<p><code>SQRT({numberOfChildren})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Sottrae tutti i numeri nell'ordine specificato e viene formattato come segue:

<p><code>SUB(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SOMMA</strong> </td> 
   <td>Somma tutti i numeri e viene formattato come segue:

<p><code>SUM(number1, number2, ...)</code></p></td> 
  </tr> 
 </tbody> 
</table>

### Testo dei campi personalizzati calcolati {#text-calculated-custom-fields}

È possibile creare un campo personalizzato calcolato che visualizzi un valore in formato testo utilizzando le seguenti espressioni:

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
   <td><strong>CASE</strong> </td> 
   <td> <p>Viene utilizzato con altre espressioni per scegliere un valore da un elenco in base a un numero di indice. </p>
   <p>Un numero di indice è un campo o una funzione che restituisce un valore numerico (in genere in un intervallo noto).</p> 
   <p>L’espressione viene formattata come segue:</p>
   <p><code>CASE(indexNumber, value1, value2, ...)</code></p>

<p>Ad esempio, l'espressione seguente restituisce il nome del giorno della settimana, dove 1=domenica, 2=lunedì e così via, in una colonna calcolata:</p>

<p><code>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</code></p>

<p>Si adatta meglio ad altre espressioni che restituiscono un numero, come DAYOFWEEK, DAYOFMONTH e MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>Concatena la stringa e viene formattata come segue:</p><p><code>CONCAT(string1,"separator", string2)</code></p> <p>Di seguito sono riportati alcuni esempi di separatori che è possibile includere:</p> 
    <ul> 
     <li>uno spazio: ""</li> 
     <li>un trattino: "-"</li> 
     <li>una barra: "/"</li> 
     <li>una virgola: ","</li> 
     <li>una parola: "or", "and"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>CONTIENE</strong> </td> 
   <td>Restituisce true se la stringa findText si trova all'interno della stringa withinText e viene formattata come segue:

<p><code>CONTAINS(findText, withinText)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Evita qualsiasi carattere speciale nella stringa in modo che possa essere incluso in un argomento URL.<p>L’espressione viene formattata come segue:</p>

<p><code>ENCODEURL(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>Valuta una condizione specificata e restituisce il valore di trueExpression se è true oppure il valore di falseExpression se è false.</p>

<p>L’espressione viene formattata come segue:</p>

<p><code>IF(condition, trueExpression, falseExpression)</code></p>

<p>Ad esempio, è possibile confrontare due diversi campi data seguiti da un risultato Vero/Falso come stringa di dati:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</code></p>

<p>Nel discorso di tutti i giorni, questa istruzione significa: "SE la data di completamento prevista del mio oggetto è 'Maggiore di' la data di completamento pianificata del mio stesso oggetto, visualizza le parole 'Fuori pista' in questo campo; in caso contrario, visualizza le parole 'In pista'".</p>

<p>Se non si desidera etichettare le espressioni true o false, è necessario inserire un'etichetta vuota nell'istruzione, ad esempio:</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</code></p> 
   <p>Oppure</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</code></p>

<p>Per ulteriori informazioni sulla creazione di istruzioni "IF", vedere <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">Panoramica delle istruzioni "IF"</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Consente di cercare un valore specifico in una stringa di valori possibili. Se il valore che si sta cercando è uguale a uno dei valori specificati, l'espressione restituisce trueExpression; in caso contrario, restituisce falseExpression.</p> 
   <p>L’espressione viene formattata come segue:</p>

<p><code>IFIN(value, value1, value2,..., trueExpression, falseExpression)</code></p>

<p>Ad esempio, puoi trovare un proprietario del progetto specifico e contrassegnare i progetti con un tag specificato in una vista del progetto: <br><p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")
   </code></p>
    <p> Nel discorso di tutti i giorni, questa dichiarazione significa: "Se il proprietario del progetto è Jennifer Campbell o Rick Kuvec, contrassegna questo progetto con "Team di marketing"; altrimenti, contrassegnalo con "Altri team"."</p> 
    <p> Se non si desidera etichettare le espressioni true o false, è necessario inserire un'etichetta vuota nell'istruzione, ad esempio: </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> 
    <p>Oppure </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","")</code></p> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>Restituisce true se il valore è uguale a uno dei valori specificati; in caso contrario, l'espressione restituisce false.</p> <p>L’espressione viene formattata come segue:

</p><p><code>IN(value, value1[, value2...])</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Restituisce true se il valore è null o vuoto; in caso contrario, l'espressione restituisce false.</p> <p>L’espressione viene formattata come segue:

</p><p><code>ISBLANK(value)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEFT</strong> </td> 
   <td> <p>Restituisce un numero specificato di caratteri dal lato sinistro di una stringa e viene formattato come segue:</p>

<p><code>LEFT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Restituisce la lunghezza di una stringa e viene formattata come segue:</p>

<p><code>LEN(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>Restituisce la stringa in minuscolo ed è formattata come segue:

<p><code>LOWER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SOSTITUISCI</strong> </td> 
   <td> <p>Sostituisce tutte le occorrenze di stringa2 con stringa3 in stringa1.</p> <p>L’espressione viene formattata come segue:</p>

<p><code>REPLACE(string1, string2, string3)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>RIGHT</strong> </td> 
   <td> <p>Restituisce un numero specificato di caratteri dal lato destro di una stringa e viene formattato come segue:</p>

<p><code>RIGHT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>RICERCA</strong> </td> 
   <td> <p>Restituisce l'indice della prima occorrenza di findText nella stringa withinText, a partire dalla posizione iniziale specificata oppure -1 se il testo non viene trovato.</p> <p>L’espressione viene formattata come segue:</p>

<p><code>SEARCH(findText, withinText, start)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>STRINGA</strong> </td> 
   <td> <p>Converte un numero in una stringa e viene formattato come segue:</p>

<p><code>STRING(number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Ordina un elenco di stringhe in ordine crescente e viene formattato come segue:</p>

<p><code>SORTASCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Ordina un elenco di stringhe in ordine decrescente e viene formattato come segue:</p>

<p><code>SORTDESCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Restituisce i caratteri di una stringa in base all'indice iniziale e finale specificato e viene formattato come segue:</p>

<p><code>SUBSTR({string}, number of start position, number of end position)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>Rimuove lo spazio vuoto dall'inizio e dalla fine di una stringa e viene formattato come segue:</p>

<p><code>TRIM(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>Restituisce una stringa in maiuscolo ed è formattata come segue:</p>

<p><code>UPPER(string)</code></p> </td> 
  </tr> 
 </tbody> 
</table>
