---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Panoramica dei predecessori delle attività
description: Un predecessore è l'attività da cui dipende un'altra attività, denominata attività successore o dipendente. Adobe Workfront supporta cinque tipi di dipendenze dei predecessori.
author: Alina
feature: Work Management
exl-id: b2020a50-0921-4ed2-8a34-1a0411992b99
source-git-commit: d5f4e83badd4d011816551f06b056ffe886d3b17
workflow-type: tm+mt
source-wordcount: '1189'
ht-degree: 0%

---

# Panoramica dei predecessori delle attività

<!--Audited: 12/2023-->

<!-- 

CONTEXT SENSITIVE HELP article. DO NOT CHANGE THE NAME OF THE ARTICLE/ DO NOT MOVE OR DELETE! -->

Un predecessore è l&#39;attività da cui dipende un&#39;altra attività, denominata attività successore o dipendente. Adobe Workfront supporta cinque tipi di dipendenze dei predecessori. Per informazioni sulle dipendenze dei predecessori, vedere [Panoramica sui tipi di relazione tra attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Panoramica sui predecessori

Comprendere la funzionalità dei predecessori è importante per comprendere le tempistiche dei progetti.

Esistono relazioni predecessore di attività sia tra attività all’interno di un singolo progetto sia tra attività di progetti diversi.

Nel caso di una relazione tra più progetti, è possibile stabilire predecessori tra progetti diversi per attività appartenenti a due progetti diversi.

Se le attività predecessore e successore appartengono allo stesso progetto o a due progetti diversi, le dipendenze e le tempistiche di ciascun progetto vengono calcolate nello stesso modo.

Per quanto riguarda i predecessori, la sequenza temporale del progetto è influenzata dai seguenti fattori:

* Dipendenza predecessore
* Valore e tipo Lag\
  Per ulteriori informazioni sulla dipendenza e sui ritardi, vedere [Esempi di valori predecessori in un elenco attività](#examples-of-predecessor-values-in-a-task-list).

  Se, ad esempio, l&#39;attività A è un predecessore dell&#39;attività B in una relazione di fine-inizio e l&#39;attività B ha un vincolo attività Il più presto possibile, Workfront assegna all&#39;attività B una data di inizio pianificata immediatamente successiva alla data di completamento pianificata dell&#39;attività A, indipendentemente dal fatto che il predecessore sia applicato o meno.

Per comprendere le relazioni dei predecessori, è necessario comprendere:

* **Tipi di dipendenza:** I predecessori sono collegati da vari tipi di dipendenza. Per ulteriori informazioni sui tipi di relazione, vedere [Panoramica sui tipi di relazione tra attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

* **Applicazione di un predecessore:** Quando si applica un predecessore, l&#39;attività successore non può assolutamente iniziare fino al completamento del predecessore. L&#39;attività successore viene visualizzata come inizio immediatamente dopo il completamento del predecessore.

  Quando il predecessore non è completato (o iniziato) e non è applicato, l&#39;attività successore può iniziare ma la timeline del progetto è ancora influenzata dalle date sia dell&#39;attività predecessore che di quella successore.

  Con un predecessore imposto, Workfront non consente che l&#39;attività successore venga contrassegnata come In corso o Completata fino al completamento del predecessore.

  Workfront, tuttavia, consente la generazione di rapporti sulle ore dell’attività.\
  Per ulteriori informazioni sull&#39;applicazione dei predecessori, vedere [Applicazione dei predecessori](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

* **Flag:** Nelle dipendenze è possibile creare dei flag che creano un ritardo che deve verificarsi dopo il completamento di un&#39;attività predecessore e prima che l&#39;attività successore possa iniziare. I ritardi influiscono sulla timeline del progetto.

  Per informazioni sui tipi di ritardo, vedere [Panoramica sui tipi di ritardo](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

## Creare relazioni predecessore

Per creare predecessori, vedere uno dei seguenti articoli:

* Per stabilire i predecessori utilizzando la scheda Predecessori dell&#39;attività, vedere [Creare una relazione predecessore utilizzando l&#39;area Predecessori](../../../manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
* Per stabilire i predecessori in un elenco attività, vedere [Creare una relazione predecessore nell&#39;elenco attività](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).
* Per stabilire relazioni predecessore concatenando attività, vedere [Creare relazioni predecessore concatenando attività](../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md).
* Per stabilire predecessori tra progetti, vedi [Creare predecessori tra progetti](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

## Individuare i predecessori di un&#39;attività {#locate-the-predecessors-of-a-task}

Per trovare i predecessori di un&#39;attività, effettuare una delle seguenti operazioni:

* Vai al progetto su cui stai lavorando ed effettua le seguenti operazioni:

   1. Individuare l&#39;attività per la quale si desidera trovare i predecessori e fare clic sull&#39;attività.
   1. Fai clic su **Predecessori** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro**, quindi su **Predecessori**.
   1. Il nome del progetto in cui si trova il predecessore viene visualizzato nella colonna **Progetto**.

      Il numero nella colonna **#** mostra il numero dell&#39;attività predecessore. Ad esempio, &quot;6&quot; indica la sesta attività del progetto.

      ![Sezione Predecessori dell&#39;attività](assets/predecessors-area-with-task-header.png)

* Vai al progetto su cui stai lavorando ed effettua le seguenti operazioni:

   1. Fare clic sulla scheda **Attività**.
   1. Scegli la **Visualizzazione standard** in alto nell&#39;elenco delle attività.
   1. La colonna **Predecessori** mostra i numeri delle attività predecessori.

      Per un predecessore con più progetti, la colonna Predecessori mostra il numero di riferimento del progetto a cui appartiene il predecessore e il numero dell’attività, separati da due punti.

      L&#39;icona del predecessore diventa verde quando l&#39;attività predecessore è contrassegnata come completata. Questo indica che l&#39;attività dipendente è pronta per il lavoro.

      Passa il cursore del mouse su questo valore per ottenere ulteriori informazioni sul predecessore, sul progetto e sulle date.

      ![Dettagli predecessore](assets/predecessor-details-in-task-list.png)

## Esempi di valori predecessori in un elenco attività {#examples-of-predecessor-values-in-a-task-list}

Quando si visualizzano i predecessori in un elenco di attività, è possibile che vengano visualizzati i seguenti tipi di predecessori con i rispettivi tipi di dipendenza e gli importi di ritardo:

* **1fs -** Il numero dell&#39;attività predecessore è 1. Il tipo di dipendenza è Fine-Inizio. Nella sequenza temporale del progetto, l&#39;attività è programmata per iniziare immediatamente dopo il completamento dell&#39;attività 1. Ciononostante, può ancora essere contrassegnato come In corso o Completato.
* **1 -** Il numero dell&#39;attività predecessore è 1. È uguale a **1fs**, poiché **fs** è la relazione predefinita predecessore in Workfront.

* **1fse -** Il numero dell&#39;attività predecessore è 1. Il tipo di dipendenza è Finish-Start-Enforced. Nella sequenza temporale del progetto, questa attività viene visualizzata come se fosse in fase di avvio subito dopo il completamento dell&#39;attività 1. Workfront non consente di contrassegnarlo come In corso o Completato fino al completamento dell&#39;attività 1. Workfront, tuttavia, consente la generazione di rapporti sulle ore dell’attività.
* **1fs+3d -** Il numero dell&#39;attività predecessore è 1. Il tipo di dipendenza è Fine-Inizio con un ritardo di 3 giorni. Nella sequenza temporale del progetto, questa attività viene visualizzata come a partire da 3 giorni lavorativi dopo il completamento dell&#39;attività 1.
* **1fs-3d -** Il numero dell&#39;attività predecessore è 1. Il tipo di dipendenza è Fine-Inizio con un ritardo di 3 giorni. Nella sequenza temporale del progetto, questa attività viene visualizzata come se iniziasse 3 giorni lavorativi prima del completamento dell&#39;attività predecessore.
* **1fs+3de** - Il numero dell&#39;attività predecessore è 1. Il tipo di dipendenza è Finish-Start-Enforced con un ritardo di 3 giorni. Nella sequenza temporale del progetto, questa attività viene visualizzata come a partire da 3 giorni lavorativi dopo il completamento dell&#39;attività 1. Workfront non consente di contrassegnarlo come In corso o Completato fino al completamento dell&#39;attività 1. Workfront, tuttavia, consente la generazione di rapporti sulle ore dell’attività.

  >[!NOTE]
  >
  >È necessario aggiungere il valore imposto (**e**) al Lag e non al predecessore.

* **4515:2** Il numero dell&#39;attività predecessore è 2. - Si tratta di una dipendenza Fine-Inizio non imposta con il predecessore nel progetto con numero di riferimento **4515**.

## Visualizza informazioni predecessore

Puoi visualizzare le informazioni sui predecessori nelle seguenti aree di Workfront. Ciò include informazioni sui predecessori tra progetti:

* A livello di attività, nella sezione Predecessori.

  Per informazioni sulla visualizzazione delle informazioni sui predecessori nella sezione Predecessori, vedere la sezione [Individuare i predecessori di un&#39;attività](#locate-the-predecessors-of-a-task) in questo articolo.

* Nel diagramma di Gantt.

  Per informazioni sulla visualizzazione dei predecessori nel diagramma di Gantt, vedere [Configurare la visualizzazione delle informazioni nel diagramma di Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

* In un elenco di attività.

  Per visualizzare le informazioni sui predecessori delle attività in un elenco di attività, è possibile effettuare una delle seguenti operazioni:

   * Applicare la visualizzazione standard incorporata in un elenco di attività.

     Per informazioni sulla visualizzazione delle informazioni sui predecessori nella visualizzazione Standard, vedere la sezione [Individuare i predecessori di un&#39;attività](#locate-the-predecessors-of-a-task) in questo articolo.

   * Creare una visualizzazione attività o un report e aggiungere la colonna Predecessori a tale visualizzazione.

     Per ulteriori informazioni sulla creazione di una visualizzazione personalizzata per le attività con informazioni sui predecessori, vedere [Visualizzazione: dettagli predecessori](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-predecessor-details.md).

* Nell’intestazione dell’attività quando si accede all’attività.

  ![](assets/qs-predecessor-info-in-task-header-350x141.png)
