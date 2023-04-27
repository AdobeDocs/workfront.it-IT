---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Espressioni dati calcolate
description: Puoi utilizzare le espressioni dati per definire campi dati personalizzati calcolati in Adobe Workfront. Connettono i campi Workfront esistenti nelle istruzioni che generano un nuovo campo.
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 1e91514f86a307ffa71cde650b35a2e3b8f0fa88
workflow-type: tm+mt
source-wordcount: '2302'
ht-degree: 7%

---

# Espressioni dati calcolate

Puoi utilizzare le espressioni dati per definire campi dati personalizzati calcolati in Adobe Workfront. Connettono i campi Workfront esistenti nelle istruzioni che generano un nuovo campo.

Puoi utilizzare espressioni dati calcolate in:

* Un modulo personalizzato

   Per ulteriori informazioni sulla creazione di campi di dati personalizzati calcolati nei moduli personalizzati in Workfront, vedere [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* Colonna personalizzata calcolata in un rapporto o in un elenco quando si utilizza la modalità testo

   Per ulteriori informazioni sull’utilizzo della modalità testo nei rapporti e nelle viste, consulta [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Sintassi dei campi personalizzati calcolati rispetto alle colonne personalizzate calcolate

Anche se le funzioni utilizzate sono le stesse, la sintassi per la creazione di un&#39;espressione in un campo personalizzato calcolato può essere diversa da quella per la creazione di una colonna personalizzata calcolata.

Ad esempio:

* In un campo personalizzato, in un modulo personalizzato per le attività, è possibile utilizzare quanto segue per generare il nome del progetto principale dell’attività a cui è allegato il modulo personalizzato:

   ```
   {project}.{name}
   ```

* In una colonna personalizzata di un rapporto, puoi utilizzare quanto segue per aggiungere una colonna personalizzata Nome progetto in un rapporto di attività:

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

Le differenze tra le due sintassi sono:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Campo personalizzato calcolato</strong></td> 
   <td><strong>Elemento di reporting personalizzato calcolato</strong></td> 
  </tr> 
   <td>Racchiudere i nomi dei campi tra parentesi graffe.</td> 
   <td>Non racchiudere i nomi dei campi tra parentesi o parentesi quando vengono utilizzati in una <code>valuefield </code>linea. <p>Racchiudi i nomi dei campi tra parentesi graffe quando vengono utilizzati in una <code>valueexpression</code> linea.</p> </td> 
  </tr> 
  <tr> 
   <td>Separa i campi per periodi.</td> 
   <td> <p>Separa i campi con due punti quando vengono utilizzati in una <code>valuefield </code>line</p> <p>Separa i campi per periodi quando vengono utilizzati in una <code>valueexpression </code>linea. </p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni sulla sintassi da utilizzare in una colonna personalizzata calcolata, consulta [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Espressioni dati utilizzabili

Gli elenchi seguenti definiscono le espressioni disponibili utilizzabili per la creazione di uno dei 3 diversi tipi di campi personalizzati calcolati in Workfront:

* [Campi personalizzati calcolati in base alla data e all’ora](#date-time-calculated-custom-fields)
* [Campi personalizzati calcolati matematicamente](#mathematical-calculated-custom-fields)
* [Campi personalizzati calcolati in testo](#text-calculated-custom-fields)

### Campi personalizzati calcolati in base alla data e all’ora {#date-time-calculated-custom-fields}

>[!NOTE]
>
>Se si crea un calcolo di data e ora che non include una porzione di ora o che utilizza i caratteri jolly della data $$TODAY o $$NOW, il sistema utilizza la data in base al fuso orario UTC (Coordinated Universal Time), non in base al fuso orario locale. Questo può causare un risultato della data imprevisto.

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
   <td> <p>Questa espressione aggiunge il numero di giorni alla data. Il valore numerico può includere giorni parziali (ad esempio, 1,5 aggiungerà un giorno e mezzo alla data).</p> <p>L'espressione viene formattata come segue:</p><pre>ADDDAYS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>Questa espressione aggiunge il numero di giorni feriali alla data. Questa espressione aggiunge alla data solo valori interi interi, con arrotondamento verso il basso. </p> <p>L'espressione viene formattata come segue:</p><pre>ADDWEEKDAYS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>Questa espressione aggiunge il numero di mesi alla data ed è formattata come segue:</p><pre>ADDMONTHS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>Questa espressione aggiunge il numero di anni alla data ed è formattata come segue:</p><pre>ADDYEARS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>Questa espressione cancella la parte temporale di una data e viene formattata come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p><pre>CLEARTIME({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATE</strong> </td> 
   <td> <p>Questa espressione converte una stringa in una data e viene formattata come segue:</p><pre>DATE(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>Questa espressione restituisce il numero di giorni tra le due date, tenendo conto dei giorni di inizio e di fine del periodo selezionato e delle marche temporali di tali giorni. Ad esempio, se l’ora di inizio della data di inizio è 3 PM, il giorno di inizio non sarà conteggiato come giorno intero.</p> <p>L'espressione viene formattata come segue:</p><pre>DATEDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>Questa espressione restituisce il giorno del mese per la data sotto forma di numero, compreso tra 1 e 31.</p> <p>L'espressione viene formattata come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p><pre>DAYOFMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>Questa espressione restituisce come numero il giorno della settimana della data, tra 1 (domenica) e 7 (sabato).</p> <p>L'espressione viene formattata come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p><pre>DAYOFWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>Questa espressione restituisce come numero i giorni totali del mese della data ed è formattata come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p><pre>DAYSINMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>Questa espressione restituisce il totale dei giorni feriali tra la data e la fine della settimana, o la fine del mese, a seconda di quale dei due eventi si verifica per primi. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p> <p>L'espressione viene formattata come segue:</p><pre>DAYSINSPLITWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>Questa espressione restituisce come numero i giorni totali nell'anno della data ed è formattata come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p><pre>DAYSINYEAR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>Questa espressione restituisce la data più recente nell’elenco ed è formattata come segue:</p><pre>DMAX(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>Questa espressione restituisce la prima data dell’elenco e viene formattata come segue:</p><pre>DMIN(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>HOUR</strong> </td> 
   <td> <p>Questa espressione restituisce l'ora della data come numero compreso tra 0 e 23.</p> <p>L'espressione viene formattata come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p><pre>HOUR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>Questa espressione restituisce il minuto della data come numero compreso tra 0 e 60, formattato come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p><pre>MINUTE({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MESE</strong> </td> 
   <td> <p>Questa espressione restituisce il mese della data sotto forma di numero compreso tra 1 e 12, formattato come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p><pre>MONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>Questa espressione restituisce il secondo della data come numero compreso tra 0 e 60, formattato come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p><pre>SECOND({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>Questa espressione restituisce il numero di giorni feriali tra due date, tenendo conto dei giorni di inizio e di fine del periodo selezionato e delle marche temporali di tali giorni. Ad esempio, se l’ora di inizio della data di inizio è 3 PM, il giorno di inizio non sarà conteggiato come giorno intero.</p> <p>L'espressione viene formattata come segue:</p><pre>WEEKDAYDIFF(date2, date1)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>Questa espressione restituisce il numero di minuti pianificati tra le date in base alla pianificazione predefinita.</p> <p>L'espressione viene formattata come segue:</p><pre>WORKMINUTESDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ANNO</strong> </td> 
   <td> <p>Questa espressione restituisce l'anno della data sotto forma di numero a 4 cifre, formattato come segue. In questo esempio, la data corrisponde alla data di immissione di un oggetto di lavoro.</p><pre>YEAR({entryDate})</pre> </td> 
  </tr> 
 </tbody> 
</table>

### Campi personalizzati calcolati matematicamente {#mathematical-calculated-custom-fields}

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
   <td>Questa espressione restituisce il valore assoluto del numero ed è formattata come segue. In questo esempio viene utilizzato il numero di oggetti sotto l'oggetto a cui è associato il modulo personalizzato.<pre>ABS({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>Questa espressione restituisce la media dei numeri ed è formattata come segue:<pre>AVERAGE(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>Questa espressione arrotonda un numero al numero intero più vicino e viene formattata come segue. In questo esempio viene utilizzato il numero di oggetti sotto l'oggetto a cui è associato il modulo personalizzato.<pre>CEIL({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>Questa espressione divide tutti i numeri nell'ordine specificato ed è formattata come segue:<pre>DIV(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>Questa espressione arrotonda un numero al numero intero più vicino e viene formattata come segue. In questo esempio viene utilizzato il numero di oggetti sotto l'oggetto a cui è associato il modulo personalizzato.<pre>FLOOR({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>Questa espressione restituisce il valore del logaritmo naturale del numero ed è formattata come segue:<pre>LN({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>Questa espressione restituisce il valore logaritmo di num2 al numero base1 ed è formattata come segue:<pre>LOG(number1, number2)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>Questa espressione restituisce l'elemento più grande dell'elenco ed è formattata come segue:<pre>MAX(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>Questa espressione restituisce l'elemento più piccolo dell'elenco ed è formattata come segue:<pre>MIN(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>NUMBER</strong> </td> 
   <td>Questa espressione converte una stringa in un numero e viene formattata come segue:<pre>NUMBER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>Questa espressione restituisce un numero elevato a una potenza e viene formattata come segue:<pre>POWER(number, power)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>Questa espressione moltiplica tutti i numeri ed è formattata come segue:<pre>PROD(number1, number2, ....)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>Questa espressione arrotonda il numero a decimali specifici di precisione e viene formattata come segue:<p>ROUND(numero, precisione)</p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> Questa espressione ordina i numeri in ordine crescente ed è formattata come segue:</p><pre>SORTASCNUM(number1, number2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>Questa espressione ordina i numeri in ordine decrescente ed è formattata come segue:<pre>SORTDESCNUM(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>Questa espressione restituisce una radice quadrata di un numero ed è formattata come segue. In questo esempio viene utilizzato il numero di oggetti sotto l'oggetto a cui è associato il modulo personalizzato.</p><pre>SQRT({numberOfChildren})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>Questa espressione sottrae tutti i numeri nell'ordine specificato e viene formattata come segue:<pre>SUB(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>Questa espressione aggiunge tutti i numeri ed è formattata come segue:<pre>SUM(number1, number2, ...)</pre></td> 
  </tr> 
 </tbody> 
</table>

### Campi personalizzati calcolati in testo {#text-calculated-custom-fields}

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
   <td> <p>Questa espressione viene utilizzata con altre espressioni per scegliere un valore da un elenco, in base a un numero di indice. Un numero di indice è un campo o una funzione che restituisce un valore numerico (in genere in un intervallo noto).</p> <p>L'espressione viene formattata come segue:</p><pre>CASE(indexNumber, value1, value2, ...)</pre> <p>Ad esempio, l'espressione seguente restituisce il nome del giorno della settimana, dove 1=domenica, 2=lunedì e così via, in una colonna calcolata:</p><pre>CASE(DAYOFWEEK({entryDate}),"domenica","lunedì","martedì","mercoledì","giovedì","venerdì","sabato")</pre> <p>Questa espressione funziona meglio con altre espressioni che restituiscono un numero, ad esempio DAYOFWEEK, DAYOFMONTH e MONTH.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>Questa espressione concatena la stringa ed è formattata come segue:</p><pre>CONCAT(string1,"separator", string2)</pre> <p>Di seguito sono riportati alcuni esempi di separatori che è possibile includere:</p> 
    <ul> 
     <li>uno spazio: "</li> 
     <li>un trattino: "-"</li> 
     <li>una barra: "/"</li> 
     <li>una virgola: ","</li> 
     <li>una parola: "or", "and"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>CONTAINS</strong> </td> 
   <td>Questa espressione restituisce true se la stringa findText si trova all'interno della stringa withinText e viene formattata come segue:<pre>CONTAINS(findText, withinText)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>Questa espressione evita qualsiasi carattere speciale nella stringa in modo che possano essere inclusi in un argomento URL.<p>L'espressione viene formattata come segue:</p><pre>ENCODEURL(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>Questa espressione valuta una condizione specificata e restituisce il valore di trueExpression se è true oppure il valore di falseExpression se è false.</p> <p>L'espressione viene formattata come segue:</p><pre>IF(condition, trueExpression, falseExpression)</pre> <p>Ad esempio, è possibile confrontare due campi data diversi seguiti da un risultato True/False come stringa dati:</p><pre>IF({projectsCompletionDate}&gt;{scheduledCompletionDate},"Off Track","On Track")</pre> <p>Nel discorso quotidiano, questa dichiarazione significa: "SE la data di completamento prevista dell'oggetto è 'Maggiore di' la data di completamento pianificata dello stesso oggetto, visualizzare le parole 'Disattivato brano' in questo campo; in caso contrario, visualizzare le parole "Su traccia".</p> <p>Se non si desidera etichettare le espressioni true o false, è necessario inserire un'etichetta vuota nell'istruzione, ad esempio:</p><pre>IF({projectsCompletionDate}&gt;{scheduledCompletionDate},"","On Track")</pre> <p>Oppure</p><pre>IF({projectionCompletionDate}&gt;{scheduledCompletionDate},"Off Track","")</pre> <p>Per ulteriori informazioni sulla creazione di istruzioni "IF", vedi <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">Panoramica delle istruzioni "IF"</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>Questa espressione ti consente di cercare un valore specifico in una stringa di possibili valori. Se il valore ricercato è uguale a uno dei valori forniti, l'espressione restituisce trueExpression; in caso contrario restituisce falseExpression.</p> <p>L'espressione viene formattata come segue:</p><pre>IFIN(valore, valore1, valore2,.., trueExpression, falseExpression)</pre> <p>Ad esempio, puoi trovare un proprietario progetto specifico e contrassegnare i progetti con un tag specificato in una visualizzazione di progetto: <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> Nel discorso quotidiano, questa dichiarazione significa: "Se il proprietario del progetto è Jennifer Campbell o Rick Kuvec, contrassegna il progetto con "Marketing Team"; altrimenti, contrassegnalo con "Altri team"."</p> <p> Se non si desidera etichettare le espressioni true o false, è necessario inserire un'etichetta vuota nell'istruzione, ad esempio: </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> <p>Oppure </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>TRA</strong> </td> 
   <td> <p>Questa espressione restituisce true se il valore è uguale a uno dei valori specificati; in caso contrario, l'espressione restituisce false.</p> <p>L'espressione viene formattata come segue:</p><pre>IN(value, value1[, value2...])</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>Questa espressione restituisce true se il valore è null o empty; in caso contrario, l'espressione restituisce false.</p> <p>L'espressione viene formattata come segue:</p><pre>ISBLANK(value)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SINISTRA</strong> </td> 
   <td> <p>Questa espressione restituisce un numero specificato di caratteri dal lato sinistro di una stringa e viene formattata come segue:</p><pre>LEFT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>Questa espressione restituisce la lunghezza di una stringa e viene formattata come segue:</p><pre>LEN(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>Questa espressione restituisce la stringa in minuscolo e viene formattata come segue:<pre>LOWER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SOSTITUISCI</strong> </td> 
   <td> <p>Questa espressione sostituisce tutte le occorrenze di string2 con string3 in string1.</p> <p>L'espressione viene formattata come segue:</p><pre>REPLACE(string1, string2, string3)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DESTRA</strong> </td> 
   <td> <p>Questa espressione restituisce un numero specificato di caratteri dal lato destro di una stringa e viene formattata come segue:</p><pre>RIGHT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>RICERCA</strong> </td> 
   <td> <p>Questa espressione restituisce l'indice della prima occorrenza di findText nella stringa withinText, a partire dalla posizione iniziale specificata, oppure -1 se il testo non viene trovato.</p> <p>L'espressione viene formattata come segue:</p><pre>SEARCH(findText, withinText, start)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>STRING</strong> </td> 
   <td> <p>Questa espressione converte un numero in una stringa e viene formattata come segue:</p><pre>STRING(numero)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>Questa espressione ordina un elenco di stringhe in ordine crescente e viene formattata come segue:</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> Questa espressione ordina un elenco di stringhe in ordine decrescente e viene formattata come segue:</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>Questa espressione restituisce i caratteri di una stringa in base all'indice iniziale e finale specificato ed è formattata come segue:</p><pre>SUBSTR({stringa}, numero di posizioni iniziali, numero di posizioni finali)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>Questa espressione rimuove gli spazi bianchi dall'inizio e dalla fine di una stringa e viene formattata come segue:</p><pre>TRIM(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>Questa espressione restituisce una stringa in maiuscolo e viene formattata come segue:</p><pre>UPPER(string)</pre> </td> 
  </tr> 
 </tbody> 
</table>
