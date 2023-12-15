---
product-area: reporting
navigation-topic: text-mode-reporting
title: Panoramica sulla sintassi della modalità testo
description: È possibile utilizzare l’interfaccia in modalità testo per creare visualizzazioni, filtri, raggruppamenti e prompt personalizzati più complessi in elenchi e rapporti. La modalità testo consente di accedere ai campi e ai relativi attributi non disponibili nell'interfaccia della modalità standard.
author: Nolan
feature: Reports and Dashboards
role: User
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 6d2144732e5f47b670c2281d042a2dc950a2928f
workflow-type: tm+mt
source-wordcount: '1865'
ht-degree: 0%

---

# Panoramica sulla sintassi della modalità testo

<!--Audited: 12/2023-->

È possibile utilizzare l’interfaccia in modalità testo per creare visualizzazioni, filtri, raggruppamenti e prompt personalizzati più complessi in elenchi e rapporti. La modalità testo consente di accedere ai campi e ai relativi attributi non disponibili nell&#39;interfaccia della modalità standard.

Per informazioni e considerazioni sulla modalità testo prima di iniziare, consulta [Panoramica sulla modalità testo](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Per un elenco completo di tutti i campi da segnalare e dei relativi attributi, vedere [API Explorer](../../../wf-api/general/api-explorer.md).

Per ulteriori informazioni sulla creazione di rapporti utilizzando la modalità testo, inclusi classi, video e tutorial, visita la sezione Informazioni sul sito Adobe Experience League.

## Considerazioni sulla sintassi della modalità testo

* Devi comprendere la sintassi di Adobe Workfront prima di iniziare a creare elementi di reporting in modalità testo. La sintassi Workfront per la modalità testo è univoca per questa applicazione e presenta caratteristiche univoche che è necessario conoscere.
* Prima di iniziare a utilizzare la modalità testo nei rapporti, consigliamo vivamente di seguire le nostre lezioni sui rapporti avanzati per comprendere meglio il linguaggio della modalità testo. <!--outdated link: For training materials on reporting see [Workfront Reports and Dashboards Learning Paths](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).-->
* Puoi personalizzare viste, filtri e raggruppamenti utilizzando l’interfaccia in modalità standard. Tuttavia, è possibile creare prompt personalizzati solo utilizzando la modalità testo.

## Linee guida comuni per la creazione di elementi di reporting in modalità testo

Di seguito sono riportate le linee guida comuni per la creazione di elementi di reporting o di elenco in modalità testo:

* Utilizza sempre Camel Case quando si fa riferimento a oggetti o attributi nel database di Workfront.
* Tieni presente la gerarchia di oggetti in Workfront. Esistono le seguenti differenze tra viste, filtri e raggruppamenti:

   * È possibile visualizzare in una visualizzazione un oggetto che si trova a tre oggetti distanti dall&#39;oggetto report o elenco.
   * Non è possibile fare riferimento a oggetti che si trovano a più di 2 oggetti lontani dall&#39;oggetto principale in un raggruppamento, un filtro o un prompt personalizzato.

  **Esempio:** È possibile visualizzare il nome o il GUID del proprietario del Portfolio in una visualizzazione delle attività:


  `valuefield=project:portfolio:ownerID`

  Non è possibile raggruppare, filtrare o richiedere il proprietario del Portfolio in una visualizzazione delle attività:

  `project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa`


  In questi esempi, l&#39;ID proprietario Portfolio è a tre oggetti dall&#39;oggetto dell&#39;elenco.

  Per informazioni sulla gerarchia degli oggetti in Workfront, vedi:

   * [Comprendere gli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API Explorer](../../../wf-api/general/api-explorer.md)

* Se possibile, utilizza i caratteri jolly per rendere più dinamici i rapporti e gli elenchi ed evitare di duplicarli per utenti diversi e con timeline simili.

## Panoramica del caso Camel

Quando si fa riferimento ai campi Workfront o ai relativi attributi in modalità testo, Workfront richiede di digitarne i nomi in Camel Case. In questo caso, i campi single-name vengono scritti in minuscolo. I campi composti vengono digitati in base al seguente schema:

`camelCaseSyntax`

>[!IMPORTANT]
>
>Tutti gli elementi di reporting seguono questo pattern di maiuscole/minuscole.

Le caratteristiche del corpo del cammello sono:

* La prima parola inizia sempre con una lettera minuscola.
* Le parole seguenti iniziano sempre con una lettera maiuscola.
* Non ci sono spazi tra le parole.

**Esempio:** Per fare riferimento alla Data di completamento effettiva di un progetto, il nome del campo che si utilizzerebbe durante la creazione di elementi di reporting in modalità testo è

`actualCompletionDate`

## Sintassi della modalità testo per vari elementi di reporting

Esistono le seguenti somiglianze tra la sintassi dei set di elementi di reporting riportati di seguito, quando vengono creati utilizzando la modalità testo:

* Le righe di codice e la sintassi sono simili per le visualizzazioni e i raggruppamenti.

  Per informazioni sulle righe chiave dei codici per le visualizzazioni e i raggruppamenti durante la creazione in modalità testo, vedere:

   * [Modificare una vista utilizzando la modalità testo](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [Modifica modalità testo in un raggruppamento](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* Le righe di codice e la sintassi sono simili per i filtri e i prompt personalizzati.

  Per ulteriori informazioni, consulta:

   * [Modificare un filtro utilizzando la modalità testo](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [Aggiungere una richiesta a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### Sintassi per visualizzazioni e raggruppamenti

Le righe di codice per la creazione di visualizzazioni e raggruppamenti sono simili.

Per informazioni sulla creazione di viste e raggruppamenti, vedere gli articoli seguenti:

* [Panoramica delle visualizzazioni in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

La riga di codice più importante per una visualizzazione o un raggruppamento è la riga che identifica l&#39;oggetto a cui si fa riferimento nella colonna della visualizzazione o nel raggruppamento. Questa riga di codice può iniziare con `valuefield` o `valueexpression` a seconda che si tratti di un riferimento diretto a un campo di un database Workfront o di un calcolo tra più campi.

Nella tabella seguente sono elencate le righe di codice più comuni in una visualizzazione o in un raggruppamento:

| Riga di codice | Descrizione |
|-----------------|------------------------------------------------------------------------------------------------------------------------------|
| `valuefield` | Identifica l&#39;oggetto a cui si fa riferimento nella colonna della visualizzazione o nel raggruppamento. Riferimento diretto all&#39;oggetto a cui si fa riferimento. |
| `valueexpression` | Identifica l&#39;oggetto a cui si fa riferimento nella colonna della visualizzazione o nel raggruppamento. Si tratta di un calcolo tra diversi campi. |
| `valueformat` | Identifica il formato in cui Workfront restituisce il valore specificato nelle righe valuefield o valueexpression. |
| `width` | Identifica la larghezza di una colonna in pixel. |
| `stretch` | Identifica le colonne che occupano spazio aggiuntivo non necessario per la visualizzazione. |

>[!TIP]
>
>* Anche se le righe di codice negli esempi seguenti sono simili tra le viste e i raggruppamenti, ricorda sempre che ogni riga di codice per un raggruppamento inizia con il numero del raggruppamento.
>
>  Per raggruppare in base al nome del progetto in un elenco o in un report di progetti, utilizzare la riga seguente per il raggruppamento di primo livello:
>
>  `group.0.valuefield=name`
>  
>* Se si modificano più colonne in una visualizzazione nella stessa colonna (come nel caso delle colonne condivise), tenere presente che ogni riga di codice per ogni colonna inizia con il numero di colonna.
>
>  Utilizza il formato seguente per identificare la prima colonna di una vista:
>
>  `column.0.valuefield=name`
>  
>  Per informazioni sulla condivisione delle colonne, vedere [Vista: unire le informazioni provenienti da più colonne in una colonna condivisa](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).
>

#### `Valuefield` panoramica della sintassi per visualizzazioni e raggruppamenti

`Valuefield=` è una riga di codice chiave nelle visualizzazioni e nei raggruppamenti che identifica l&#39;oggetto a cui si fa direttamente riferimento.

La sintassi per i campi che fanno direttamente riferimento a è identica per raggruppamenti e viste.

Le seguenti regole si applicano quando si fa riferimento a oggetti Workfront utilizzando un `valuefield` riga:

* Utilizza Camel Case per fare riferimento direttamente ai campi.

  **Esempio:** Per fare riferimento alla data di completamento effettiva dell&#39;attività in una visualizzazione dell&#39;attività, utilizzare la riga seguente:

  `valuefield=actualCompletionDate`

* Utilizza maiuscole/minuscole e due punti per separare i campi correlati tra loro per lo stesso oggetto.

  **Esempio:** Per fare riferimento alla data di completamento pianificata del progetto in una visualizzazione delle attività, utilizzare la riga seguente:

  `valuefield=project:plannedCompletionDate`

  Per informazioni sul modo in cui gli oggetti fanno riferimento l&#39;uno all&#39;altro nel database di Workfront, vedere [API Explorer](../../../wf-api/general/api-explorer.md).

* Quando fai riferimento a un campo personalizzato, utilizza il nome del campo esattamente come viene visualizzato nell’interfaccia.

  **Esempio:** Per fare riferimento a un campo personalizzato del progetto con l&#39;etichetta Dettagli aggiuntivi in una visualizzazione delle attività, utilizzare la riga seguente:

  `valuefield=project:Additional Details`

#### `Valueexpression` panoramica della sintassi per visualizzazioni e raggruppamenti

È possibile sostituire il `valuefield=` riga di codice con `valueexpression=` quando si creano visualizzazioni e raggruppamenti in modalità testo quando si desidera fare riferimento a un calcolo tra 2 o più campi.

>[!TIP]
>
>Sebbene sia possibile creare campi calcolati che è possibile visualizzare nei rapporti, le visualizzazioni e i raggruppamenti calcolati sono più dinamici. Le visualizzazioni e i raggruppamenti calcolati vengono aggiornati con nuove informazioni ogni volta che si esegue il report o si visualizza un elenco.
>
>Per informazioni sulla creazione di colonne calcolate in una visualizzazione, vedere [Campi personalizzati calcolati e colonne calcolate](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

La creazione di un raggruppamento calcolato è simile alla creazione di una colonna calcolata in una visualizzazione.

Le seguenti regole si applicano quando si fa riferimento a oggetti Workfront utilizzando un `valueexpression` riga:

* Utilizza Camel Case per fare riferimento direttamente ai campi e racchiudere ogni campo tra parentesi graffe.

  **Esempio:** Per visualizzare il campo Nome attività in una colonna di attività tramite `valueexpression`, utilizza la riga seguente:

  `valueexpression={name}`


* Utilizza il caso camel e i periodi per separare i campi correlati gli uni agli altri.

  **Esempio:** Per visualizzare il nome di un progetto concatenato con il nome dell&#39;attività in un report attività, utilizzare le righe seguenti:

   * In una visualizzazione:

     `valueexpression=CONCAT({project}.{name},' - ',{name})`

   * In un raggruppamento:

     `group.0.valueexpression=CONCAT({project}.{name},' - ',{name})`

  Per informazioni sul modo in cui gli oggetti fanno riferimento l&#39;uno all&#39;altro nel database di Workfront, vedere [API Explorer](../../../wf-api/general/api-explorer.md).

* Quando si fa riferimento a un campo personalizzato, utilizza le regole seguenti:

   * Utilizza il nome del campo esattamente come viene visualizzato nell’interfaccia.
   * Anteponi al nome del campo &quot;DE:&quot;.
   * Racchiudere il campo tra parentesi graffe.
   * Separare i campi correlati all&#39;oggetto in base ai punti.

  **Esempio:** Per visualizzare il campo personalizzato del progetto Dettagli aggiuntivi in una visualizzazione delle attività in una riga di espressione del valore, utilizzare la riga seguente:

  `valueexpression={project}.{DE:Additional Details}`

* È possibile utilizzare un carattere jolly in un `valueexpression` ma non in un `valuefield` linea.

  Per informazioni sui caratteri jolly, vedere [Panoramica delle variabili filtro con caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).


#### `Valueformat` panoramica su visualizzazioni e raggruppamenti

La seconda riga di codice più importante in una visualizzazione o in un raggruppamento è `valueformat=` linea. Questo indica a Workfront in quale formato restituire il valore specificato nel `valuefield` o `valueexpression` linee. Anche se è possibile utilizzare vari formati per `valueformat` linee, si consiglia di utilizzare sempre il seguente valore quando si utilizza `valueexpression`:

`valueformat=HTML`

Per ulteriori `valueformat` , vedi anche i seguenti articoli:

* [Formattare le date nei report in modalità testo](../../reports/text-mode/format-dates-in-text-mode-reports.md)
* [Formattare numeri, valuta e valori percentuali nei report in modalità testo](../../reports/text-mode/format-numbers-in-text-mode-reports.md)

#### `width` panoramica sulle visualizzazioni

`width=` è la riga di codice in cui è possibile specificare la larghezza di ogni colonna in pixel. Workfront fornisce una larghezza consigliata per ogni campo, anche se a seconda del tipo di campo e del formato, potrebbe essere necessario apportare delle modifiche.

È necessario utilizzare il pulsante aggiuntivo `usewidths=true` riga di codice per applicare la larghezza specificata per la colonna.

**Esempio:** Per visualizzare una colonna con una larghezza di 80 pixel, utilizzare le seguenti righe:

`width=80`

`usewidths=true`

#### `stretch` panoramica sulle visualizzazioni

Il `stretch` viene utilizzato per identificare le colonne che occupano spazio aggiuntivo non necessario per la visualizzazione. La larghezza dell’interfaccia utente dell’area di lavoro per un utente tipico è di circa 850 pixel. Ciò significa che se disponi di una vista con quattro colonne (150 pixel ciascuna), la vista occupa 600 di 850 pixel. Nell’interfaccia utente sono presenti 250 pixel aggiuntivi che verranno aggiunti alle colonne per le quali è fornita una percentuale di estensione.

L&#39;estensione di una colonna viene applicata quando si utilizza la riga di codice aggiuntiva: `usewidths=true` per almeno una delle colonne della visualizzazione.

**Esempio:** Per indicare che una colonna può utilizzare il 70% dello spazio vuoto in una visualizzazione, utilizzare le righe seguenti:

`stretch=70`

`usewidths=true`

### Sintassi dei filtri e dei prompt personalizzati

La sintassi per la creazione di filtri è simile a quella per la creazione di prompt personalizzati.

>[!TIP]
>
>È possibile creare un prompt personalizzato creando prima un filtro per l&#39;istruzione da includere nel prompt. Connetti tutte le righe di codice in un filtro con &quot;&amp;&quot; senza spazi tra le righe e che diventa il prompt personalizzato.

Per informazioni sulla creazione di filtri e prompt personalizzati, consulta:

* [Panoramica sui filtri in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Aggiungere una richiesta a un report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

Per informazioni sulla creazione di filtri in modalità testo, consulta [Modificare un filtro utilizzando la modalità testo](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

Per creare filtri e prompt personalizzati in modalità testo, puoi utilizzare i seguenti elementi:

* Riga di codice che fa riferimento all’oggetto dell’istruzione di filtro. Utilizza Camel Case per l’oggetto filtro.
* Riga di codice che fa riferimento all&#39;oggetto filtro e al modificatore per il valore dell&#39;oggetto filtro. Usa Camel Case per l&#39;oggetto filtro in questa riga.

  >[!TIP]
  >
  >Quando si fa riferimento a intervalli, sono necessarie 2 linee di modificatore.

* Connettore di istruzioni che connette più istruzioni di filtro:

   * E

     Questo è il connettore predefinito tra le istruzioni di filtro.

   * OPPURE

     >[!TIP]
     >
     >I connettori delle istruzioni fanno distinzione tra maiuscole e minuscole e sono sempre maiuscoli. &quot;AND&quot; può essere omesso in modalità testo.

* Caratteri jolly per rendere i filtri più dinamici e personalizzarli per l&#39;ora corrente o per l&#39;utente che ha eseguito l&#39;accesso. Per informazioni sui caratteri jolly, vedere [Panoramica delle variabili filtro con caratteri jolly](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
