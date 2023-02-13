---
product-area: reporting
navigation-topic: text-mode-reporting
title: Panoramica della sintassi della modalità testo
description: È possibile utilizzare l’interfaccia in modalità testo per creare viste, filtri, raggruppamenti e prompt personalizzati più complessi negli elenchi e nei rapporti. Utilizzando la modalità testo, è possibile accedere ai campi e ai relativi attributi che non sono disponibili nell’interfaccia in modalità standard.
author: Nolan
feature: Reports and Dashboards
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1498'
ht-degree: 0%

---

# Panoramica della sintassi della modalità testo

È possibile utilizzare l’interfaccia in modalità testo per creare viste, filtri, raggruppamenti e prompt personalizzati più complessi negli elenchi e nei rapporti. Utilizzando la modalità testo, è possibile accedere ai campi e ai relativi attributi che non sono disponibili nell’interfaccia in modalità standard.

Per informazioni e considerazioni sulla modalità testo prima di iniziare, consulta [Panoramica della modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Per un elenco completo di tutti i campi da segnalare e dei relativi attributi, consulta [Esplora API](../../../wf-api/general/api-explorer.md).

## Considerazioni sulla sintassi della modalità testo

* È necessario comprendere la sintassi Adobe Workfront prima di poter iniziare a creare elementi di reporting in modalità testo. La sintassi Workfront per la modalità testo è univoca per questa applicazione e presenta caratteristiche uniche che devi conoscere bene.
* Prima di iniziare a utilizzare la modalità testo nei rapporti, ti consigliamo vivamente di seguire le nostre lezioni sul reporting avanzato, per comprendere meglio il nostro linguaggio in modalità testo. Per i materiali di formazione sul reporting vedi [Percorsi di apprendimento di Workfront Reports and Dashboards](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).
* Puoi personalizzare viste, filtri e raggruppamenti utilizzando l’interfaccia in modalità standard. Tuttavia, è possibile generare i prompt personalizzati solo utilizzando la modalità testo.

## Linee guida comuni per la creazione di elementi di reporting in modalità testo

Di seguito sono riportate le linee guida comuni per la creazione di rapporti o elementi di elenco in modalità testo:

* Utilizza sempre il cammello quando fai riferimento a oggetti o attributi nel database Workfront.
* Tenere presente la gerarchia degli oggetti in Workfront. Esistono le seguenti differenze tra viste, filtri e raggruppamenti:

   * In una visualizzazione è possibile visualizzare un oggetto distante tre oggetti dal rapporto o dall&#39;oggetto elenco.
   * Non è possibile fare riferimento a oggetti distanti più di 2 oggetti dall’oggetto principale in un prompt di raggruppamento, filtro o personalizzato.

   **Esempio:** È possibile visualizzare il nome o il GUID del proprietario del Portfolio in una visualizzazione attività:

   ```
   valuefield=project:portfolio:ownerID
   ```

   Non è possibile raggruppare, filtrare o richiedere il proprietario del Portfolio in una visualizzazione attività:

   ```
   project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa
   ```

   In questi esempi, l&#39;ID proprietario Portfolio si trova a tre oggetti dall&#39;oggetto dell&#39;elenco.

   Per informazioni sulla gerarchia degli oggetti in Workfront, vedere:

   * [Comprendere gli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [Esplora API](../../../wf-api/general/api-explorer.md)


* Utilizza i caratteri jolly ogni volta che è possibile per rendere i rapporti e gli elenchi più dinamici ed evita di duplicarli per utenti diversi e linee temporali simili.

## Panoramica della custodia del camcorder

Quando si fa riferimento a campi Workfront o ai relativi attributi in modalità testo, Workfront richiede di digitare i relativi nomi in caratteri maiuscoli e minuscoli. In questo caso, i campi per nome singolo sono scritti in lettere minuscole. I campi composti sono contrassegnati secondo il seguente pattern:

```
camelCaseSyntax
```

>[!IMPORTANT]
>
>Tutti gli elementi di reporting seguono questo pattern di casing.

Le caratteristiche del cammello sono:

* La prima parola inizia sempre con una lettera minuscola.
* Le parole seguenti iniziano sempre con una lettera maiuscola.
* Non ci sono spazi tra le parole.

**Esempio:** Per fare riferimento alla data di completamento effettivo di un progetto, il nome del campo da utilizzare per la creazione di elementi di reporting in modalità testo è

```
actualCompletionDate
```

.

## Sintassi della modalità testo per vari elementi di reporting

Esistono le seguenti somiglianze tra la sintassi dei set di elementi di reporting di seguito, quando vengono creati utilizzando la modalità testo:

* Le righe di codice e sintassi sono simili per visualizzazioni e raggruppamenti.

   Per informazioni sulle linee chiave dei codici per viste e raggruppamenti durante la loro creazione in modalità testo, consulta:

   * [Modificare una visualizzazione utilizzando la modalità testo](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [Modificare la modalità di testo in un raggruppamento](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* Le righe di codice e sintassi sono simili per i filtri e i prompt personalizzati.

   Per ulteriori informazioni, consulta:

   * [Modificare un filtro utilizzando la modalità testo](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### Sintassi per visualizzazioni e raggruppamenti

È possibile notare che le righe di codice durante la creazione di visualizzazioni e raggruppamenti sono simili.

Per informazioni sulla creazione di visualizzazioni e raggruppamenti, consulta i seguenti articoli:

* [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

La riga di codice più importante per una visualizzazione o un raggruppamento è la riga che identifica l&#39;oggetto a cui si fa riferimento nella colonna della visualizzazione o nel raggruppamento. A seconda che questo campo sia un riferimento diretto a un campo di database Workfront o un calcolo tra più campi, la riga di codice può iniziare con

```
valuefield
```

oppure

```
valueexpression
```

.

* [Panoramica della sintassi del campo di valore per visualizzazioni e raggruppamenti](#valuefield-syntax-overview-for-views-and-groupings)
* [Panoramica della sintassi della espressione di valore per visualizzazioni e raggruppamenti](#valueexpression-syntax-overview-for-views-and-groupings)

>[!TIP]
>
>* Anche se le righe di codice negli esempi seguenti sono simili tra visualizzazioni e raggruppamenti, ricorda sempre che ogni riga di codice per un raggruppamento inizia con il numero di raggruppamento.
>
>  Per raggruppare per nome progetto in un elenco o in un rapporto di progetto, utilizzare la riga seguente per il raggruppamento di primo livello:
>
>  
```>
>  group.0.valuefield=name
>  ```>
>* If you edit multiple columns in a view in the same column (as it is the case of shared columns), remember that every line of code for each column starts with the column number. 
>
>  
Use the following format to identify the first column of a view: 
>
>  
```>
>  column.0.valuefield=name
>  ```>
>  For information about sharing columns, see [View: merge information from multiple columns in one shared column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md). 
>



```
Valuefield
```

panoramica della sintassi per visualizzazioni e raggruppamenti {#valuefield-syntax-overview-for-views-and-groupings}

```
Valuefield=
```

è una riga chiave di codice in visualizzazioni e raggruppamenti che identifica l’oggetto a cui si fa riferimento direttamente.

La sintassi dei riferimenti diretti ai campi è identica per i raggruppamenti e le visualizzazioni.

Quando si fa riferimento a oggetti Workfront utilizzando un

```
valuefield
```

linea:

* Utilizza camel case per fare riferimento direttamente ai campi.

   **Esempio:** Per fare riferimento alla data di completamento effettivo attività in una visualizzazione attività, utilizzare la riga seguente:

   ```
   valuefield=actualCompletionDate
   ```

* Utilizzare maiuscole/minuscole e due punti per separare i campi correlati tra loro per lo stesso oggetto.

   **Esempio:** Per fare riferimento alla data di completamento pianificata del progetto in una visualizzazione attività, utilizzare la riga seguente:

   ```
   valuefield=project:plannedCompletionDate
   ```

   Per informazioni sul modo in cui gli oggetti fanno riferimento gli uni agli altri nel database Workfront, vedere la [Esplora API](../../../wf-api/general/api-explorer.md).

* Quando fai riferimento a un campo personalizzato, utilizza il nome del campo esattamente come appare nell’interfaccia.

   **Esempio:** Per fare riferimento a un campo personalizzato del progetto con l’etichetta Dettagli aggiuntivi in una visualizzazione attività, utilizzare la riga seguente:

   ```
   valuefield=project:Additional Details
   ```

 

```
Valueexpression
```

panoramica della sintassi per visualizzazioni e raggruppamenti {#valueexpression-syntax-overview-for-views-and-groupings}

È possibile sostituire

```
valuefield=
```

riga di codice con

```
valueexpression=
```

quando si creano viste e raggruppamenti in modalità testo quando si desidera fare riferimento a un calcolo tra 2 o più campi.

>[!TIP]
>
>Sebbene sia possibile creare campi calcolati che è possibile visualizzare nei rapporti, le viste calcolate e i raggruppamenti sono più dinamici. Le viste calcolate e i raggruppamenti vengono aggiornati con nuove informazioni ogni volta che si esegue il rapporto o si visualizza un elenco.
>
>Per informazioni sulla creazione di colonne calcolate in una visualizzazione, vedere [Campi personalizzati calcolati e colonne calcolate](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

La creazione di un raggruppamento calcolato è simile alla creazione di una colonna calcolata in una visualizzazione.

Quando si fa riferimento a oggetti Workfront utilizzando un

```
valueexpression
```

linea:

* Usa il cammello per fare riferimento direttamente ai campi e racchiudi ogni campo tra parentesi graffe.

   **Esempio:** Per visualizzare il campo Nome attività in una colonna attività utilizzando

   ```
   valueexpression
   ```

   , utilizza la seguente riga:

   ```
   valueexpression={name}
   ```

* Utilizza maiuscole/minuscole e i periodi per separare i campi correlati.

   **Esempio:** Per visualizzare il nome di un progetto concatenato con il nome dell’attività in un rapporto di attività, utilizzare le righe seguenti:

   * In questa visualizzazione:

      ```
      valueexpression=CONCAT({project}.{name},' - ',{name})
      ```

   * In un raggruppamento:

      ```
      group.0.valueexpression=CONCAT({project}.{name},' - ',{name})
      ```
   Per informazioni sul modo in cui gli oggetti fanno riferimento gli uni agli altri nel database Workfront, vedere la [Esplora API](../../../wf-api/general/api-explorer.md).

* Quando fai riferimento a un campo personalizzato, utilizza le seguenti regole:

   * Utilizza il nome del campo esattamente come appare nell’interfaccia.
   * Precede il nome del campo con &quot;DE:&quot;.
   * Racchiudi il campo tra parentesi graffe.
   * Separa i campi relativi all’oggetto per periodi.

   **Esempio:** Per visualizzare il campo personalizzato del progetto Dettagli aggiuntivi in una visualizzazione attività in una riga di espressione del valore, utilizzare la riga seguente:

   ```
   valueexpression={project}.{DE:Additional Details}
   ```

* È possibile utilizzare un carattere jolly in un

   ```
   valueexpression
   ```

   ma non in un

   ```
   valuefield
   ```

   linea.

   Per informazioni sui caratteri jolly, consulta [Variabili filtro caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

```
Valueformat
```

panoramica

La seconda riga di codice più importante in una visualizzazione o un raggruppamento è la

```
valueformat=
```

linea. Questo indica a Workfront in quale formato restituire il valore specificato nel

```
valuefield
```

o righe di espressione del valore. Anche se è possibile utilizzare vari formati per

```
valueformat
```

linee, è consigliabile utilizzare sempre il seguente valore quando si utilizza

```
valueexpression
```

:

```
valueformat=HTML
```

### Sintassi dei filtri e dei prompt personalizzati

La sintassi per la creazione di filtri è simile a quella per la creazione di prompt personalizzati.

>[!TIP]
>
>Puoi creare un prompt personalizzato creando prima un filtro per l’istruzione da includere nel prompt. Collega tutte le righe di codice in un filtro con &quot;&amp;&quot; senza spazi tra le righe e questo diventa il tuo prompt personalizzato.

Per informazioni sulla creazione di filtri e prompt personalizzati, consulta:

* [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Aggiungere un prompt a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

Per informazioni sulla creazione di filtri in modalità testo, consulta [Modificare un filtro utilizzando la modalità testo](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

È possibile utilizzare i seguenti elementi per creare filtri e prompt personalizzati in modalità testo:

* Riga di codice che fa riferimento all&#39;oggetto dell&#39;istruzione filter. Utilizzare la maiuscola/minuscola per l’oggetto filtro.
* Riga di codice che fa riferimento all&#39;oggetto filtro e al modificatore per il valore dell&#39;oggetto filtro. Utilizzare la maiuscola/minuscola per l&#39;oggetto filtro in questa riga.

   >[!TIP]
   >
   >Quando si fa riferimento a intervalli, sono necessarie 2 linee modificatrici.

* Un connettore di istruzioni che collega più istruzioni di filtro:

   * AND

      Questo è il connettore predefinito tra le istruzioni del filtro.

   * O

      >[!TIP]
      >
      >I connettori delle istruzioni sono sensibili all’uso di maiuscole e minuscole. &quot;AND&quot; può essere omesso in modalità testo.

* Caratteri jolly per rendere i filtri più dinamici e personalizzarli per l’ora corrente o per l’utente che ha effettuato l’accesso. Per informazioni sui caratteri jolly, consulta [Variabili filtro caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
