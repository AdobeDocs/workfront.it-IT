---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Panoramica dei predecessori delle attività
description: Un predecessore è l'attività da cui dipende un'altra attività (chiamata successore o attività dipendente). Adobe Workfront supporta cinque tipi di dipendenze predecessori.
author: Alina
feature: Work Management
exl-id: b2020a50-0921-4ed2-8a34-1a0411992b99
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '1112'
ht-degree: 0%

---

# Panoramica dei predecessori delle attività

<!-- 

CONTEXT SENSITIVE HELP article. DO NOT CHANGE THE NAME OF THE ARTICLE/ DO NOT MOVE OR DELETE! -->

Un predecessore è l&#39;attività da cui dipende un&#39;altra attività (chiamata successore o attività dipendente). Adobe Workfront supporta cinque tipi di dipendenze predecessori. Per comprendere le dipendenze dei predecessori, vedi [Panoramica dei tipi di dipendenza dell&#39;attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Panoramica sui predecessori

La comprensione della funzionalità predecessore è importante per comprendere le timeline nei progetti.

I rapporti predecessori tra le attività esistono sia all’interno di un singolo progetto che tra più progetti.

Nel caso di una dipendenza da più progetti, puoi stabilire predecessori tra progetti diversi.

Se le attività predecessore e successive appartengono allo stesso progetto o a due progetti diversi, le dipendenze e le tempistiche vengono calcolate allo stesso modo.

Per quanto riguarda i predecessori, la timeline del progetto è interessata dai seguenti elementi:

* Dipendenza predecessore
* Valore e tipo di ritardo\
   Per ulteriori informazioni sia sulla dipendenza che sui tag, consulta [Esempi di valori precedenti in un elenco di attività](#examples-of-predecessor-values-in-a-task-list).

Ad esempio, se l&#39;attività A è un predecessore dell&#39;attività B in una relazione di fine inizio e l&#39;attività B ha un vincolo di attività Il più presto possibile, Workfront assegna all&#39;attività B una data di inizio pianificata immediatamente dopo la data di completamento pianificata dell&#39;attività A, indipendentemente dal fatto che il predecessore sia applicato o meno.

Per comprendere le relazioni predecessori, è necessario comprendere:

* **Tipi di dipendenza:** I predecessori sono collegati da vari tipi di dipendenza. Per ulteriori informazioni sui tipi di dipendenza, consulta [Panoramica dei tipi di dipendenza dell&#39;attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

* **Applicazione di un predecessore:** Quando si applica un predecessore, l&#39;attività successore non può essere avviata fino al completamento del predecessore. L&#39;attività successore viene visualizzata come avviata immediatamente dopo il completamento del predecessore.

   Workfront non consente di contrassegnarlo come In corso o Completato fino al completamento del predecessore. Workfront, tuttavia, consente la generazione di rapporti sulle ore relative all’attività.\
   Per ulteriori informazioni sull&#39;applicazione dei predecessori, vedi [Applica predecessori](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

* **Ritardi:** È possibile creare dei ritardi nelle dipendenze che creano un ritardo che deve verificarsi dopo il completamento di un&#39;attività predecessore e prima che l&#39;attività successore possa iniziare. I ritardi influiscono sulla timeline del progetto.

   Per comprendere i tipi di ritardo, vedi [Panoramica dei tipi di ritardo](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

## Creare relazioni predecessori

Per creare i predecessori, vedi uno dei seguenti articoli:

* Per stabilire i predecessori utilizzando la scheda Predecessori dell&#39;attività, vedere [Creare una relazione predecessore utilizzando l&#39;area Predecessori](../../../manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
* Per stabilire i predecessori in un elenco di attività, vedere [Creare una relazione predecessore nell&#39;elenco delle attività](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).
* Per stabilire relazioni predecessori mediante attività di concatenamento, vedere [Creare relazioni predecessori tramite la combinazione di attività](../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md).
* Per stabilire predecessori tra progetti, consulta [Creare predecessori tra progetti](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

## Individuare i predecessori di un&#39;attività {#locate-the-predecessors-of-a-task}

Per trovare i predecessori di un&#39;attività eseguire una delle operazioni seguenti:

* Vai al progetto su cui stai lavorando ed effettua le seguenti operazioni:

   1. Individuare l&#39;attività per la quale si desidera trovare i predecessori e fare clic sull&#39;attività.
   1. Fai clic su **Predecessori** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro**, quindi **Predecessori**.
   1. Il nome del progetto su cui si trova il predecessore viene visualizzato nella **Progetto** colonna.

      Il numero nel **#** mostra il numero dell&#39;attività predecessore. Ad esempio, &quot;6&quot; indica la sesta attività del progetto.

      ![Sezione Predecessori dell&#39;attività](assets/predecessors-area-with-task-header.png)

* Vai al progetto su cui stai lavorando ed effettua le seguenti operazioni:

   1. Fai clic sul pulsante **Attività** scheda .
   1. Scegli la **Vista standard** nella parte superiore dell’elenco delle attività.
   1. La **Predecessori** mostra i numeri delle attività predecessori.

      Per un predecessore tra progetti, la colonna Predecessori mostra il numero di riferimento del progetto a cui appartiene il predecessore e il numero dell’attività, separati da due punti.

      L&#39;icona predecessore diventa verde quando l&#39;attività predecessore è contrassegnata come completata. Questo indica che l&#39;attività dipendente è pronta per il lavoro.

      Passa il puntatore del mouse su questo valore per ottenere ulteriori informazioni sul predecessore, sul progetto e sulle date.

      ![Dettagli predecessore](assets/predecessor-details-in-task-list.png)

## Esempi di valori precedenti in un elenco di attività {#examples-of-predecessor-values-in-a-task-list}

Quando si visualizzano i predecessori in un elenco di attività, è possibile che vengano visualizzati i seguenti tipi di predecessori con i rispettivi tipi di dipendenza e gli importi di ritardo:

* **1fs -** Il numero dell&#39;attività predecessore è 1. Il tipo di dipendenza è Finish-Start. Nella timeline del progetto, l’attività verrà avviata subito dopo il completamento dell’attività 1. Nonostante ciò, può essere ancora contrassegnato come In corso o Completato.
* **1 -** Il numero dell&#39;attività predecessore è 1. È lo stesso di **1fs** perché **fs** è la relazione predecessore predefinita in Workfront.

* **1fse -** Il numero dell&#39;attività predecessore è 1. Il tipo di dipendenza è Finish-Start-Enforced. Nella timeline del progetto, questa attività viene visualizzata come avviata subito dopo il completamento dell’attività 1. Workfront non consente di contrassegnarlo come In corso o Completo fino al completamento dell&#39;attività 1. Workfront, tuttavia, consente la generazione di rapporti sulle ore relative all’attività.
* **1fs+3d -** Il numero dell&#39;attività predecessore è 1. Il tipo di dipendenza è Finish-Start con un ritardo di 3 giorni. Nella timeline del progetto, questa attività viene visualizzata come a partire da 3 giorni lavorativi dopo il completamento dell’attività 1.
* **1fs-3d -** Il numero dell&#39;attività predecessore è 1. Il tipo di dipendenza è Finish-Start con un ritardo di 3 giorni. Nella timeline del progetto, questa attività viene visualizzata come a partire da 3 giorni lavorativi prima del completamento dell’attività predecessore.
* **1fs+3d** - Il numero dell&#39;attività predecessore è 1. Il tipo di dipendenza è Fine-Inizio-Imposto con un ritardo di 3 giorni. Nella timeline del progetto, questa attività viene visualizzata come a partire da 3 giorni lavorativi dopo il completamento dell’attività 1. Workfront non consente di contrassegnarlo come In corso o Completo fino al completamento dell&#39;attività 1. Workfront, tuttavia, consente la generazione di rapporti sulle ore relative all’attività.

   >[!NOTE]
   >
   >Valore imposto (**e**) deve essere aggiunto al carrello, non al predecessore.

* **4515:2** Il numero dell&#39;attività predecessore è 2. - È una dipendenza da Fine a Inizio, non forzata con il predecessore del progetto con il numero di riferimento **4515**; il numero dell&#39;attività predecessore è **2**.

## Visualizza informazioni predecessore

È possibile visualizzare le informazioni sui predecessori nelle seguenti aree di Workfront. Sono incluse informazioni sui predecessori tra progetti diversi:

* A livello di attività, nella sezione Predecessori.

   Per informazioni sulla visualizzazione delle informazioni sui predecessori nella sezione Predecessori , consulta la sezione . [Individuare i predecessori di un&#39;attività](#locate-the-predecessors-of-a-task) in questo articolo.

* Nel diagramma di Gantt.

   Per informazioni sulla visualizzazione dei predecessori nel diagramma di Gantt, vedere [Configurare la visualizzazione delle informazioni nel Diagramma di Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

* In un elenco di attività.

   Per visualizzare le informazioni sui predecessori delle attività in un elenco di attività, eseguire una delle operazioni seguenti:

   * Applicare la visualizzazione Standard integrata in un elenco di attività.

      Per informazioni sulla visualizzazione delle informazioni sui predecessori nella visualizzazione Standard, consulta la sezione [Individuare i predecessori di un&#39;attività](#locate-the-predecessors-of-a-task) in questo articolo.

   * Creare una visualizzazione o un report attività e aggiungere la colonna Predecessori a tale visualizzazione.

      Per ulteriori informazioni sulla creazione di una visualizzazione personalizzata per le attività con informazioni sui predecessori, vedere [Visualizza: dettagli predecessore](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-predecessor-details.md).

* Nell&#39;intestazione dell&#39;attività quando si accede all&#39;attività.

   ![](assets/qs-predecessor-info-in-task-header-350x141.png)
