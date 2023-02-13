---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: Panoramica della scheda di scorrimento
description: Viene visualizzata la tabella dei racconti Scrum agile insieme allo stato di completamento e al grafico a discesa.
author: Lisa
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 0%

---

# [!UICONTROL Scratto] panoramica della bacheca

La [!UICONTROL Scratto] viene visualizzata una bacheca a storie agile con stato di completamento e grafico a discesa. Questi componenti agili sono disponibili nelle seguenti situazioni in [!UICONTROL Adobe Workfront]:

* Sulle iterazioni agili. Per ulteriori dettagli sull&#39;utilizzo della bacheca di storie agili, del grafico a discesa e dello stato di completamento in un ambiente agile puro (con backlog e iterazione), consulta [Lavorare in un ambiente agile](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).
* Quando visualizzi un progetto in una visualizzazione agile. Per informazioni su come utilizzare la storyboard agile, il grafico a discesa e lo stato di completamento all&#39;interno di un progetto esistente, consulta [Gestire un progetto nella vista Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

![Iterazione Agile](assets/agile-iteration-with-callouts.png)

## Layout e funzioni del pannello Story

![Tavola di storie Agile](assets/agile-storyboard-callouts.png)

Il racconto è costituito dai seguenti elementi:

* **[!UICONTROL Storia principale] Colonna:** A differenza delle altre colonne sulla bacheca delle storie, il  [!UICONTROL Storia principale]  la colonna non è uno stato dell&#39;attività, ma esiste per ospitare i brani contenenti sottoattività nell&#39;iterazione o nel progetto. In questa colonna possono risiedere solo le storie principali che hanno almeno una sottoattività sulla bacheca del racconto. Le storie dei genitori non si spostano da stato a stato in tutto il tramonto.

   In un&#39;iterazione, questa colonna viene visualizzata sulla lavagna del racconto solo quando uno o più brani della bacheca del racconto contengono almeno una sottoattività che soddisfa i seguenti requisiti:

   * Assegnato allo stesso team agile dell&#39;attività padre
   * Appartiene all&#39;iterazione

      In un progetto, questa colonna viene visualizzata ogni volta che un’attività ha almeno una sottoattività.

      ![Colonna storia padre](assets/agile-parentstory-swimlane.png)

* **Stati attività:** Indica il progresso di un brano nell&#39;iterazione o nel progetto in base alla colonna di stato in cui si trova il brano.

   Gli stati delle attività possono essere personalizzati per il progetto modificando la visualizzazione agile, come descritto in [Creare o personalizzare una visualizzazione Agile](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [Panoramica delle visualizzazioni in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* **Corsia di nuoto:** Quando una storia principale e le sue sottoattività compaiono sulla tavola dei racconti, viene creata una corsia da bagno specifica per la storia e le sue sottoattività. Questo fornisce una distinzione visiva per vedere meglio come le attività secondarie di un brano progrediscono all&#39;interno della trama.

   In un&#39;iterazione, le piste da bagno appaiono sulla tavola dei racconti solo quando una storia sulla tavola dei racconti contiene almeno una sottoattività che soddisfa i seguenti requisiti:

   * Assegnato allo stesso team agile dell&#39;attività padre
   * Appartiene all&#39;iterazione

   In un progetto, le corsie di nuoto vengono visualizzate ogni volta che un&#39;attività ha almeno una sottoattività o un&#39;attività principale.

* **Storie individuali:** Le storie e i problemi individuali sono visualizzati sotto le piste di nuoto sulla tavola dei racconti. Questo fornisce una distinzione visiva dalle storie che fanno parte di una corsia di nuoto.

## Relazione tra sottoattività e storie

Se una storia contiene attività secondarie, non è possibile aggiornare informazioni sulla storia padre stessa (ad esempio punti/ore o percentuale di completamento). Inoltre, non è possibile spostare la storia all&#39;interno della trama per aggiornarne lo stato. Piuttosto, qualsiasi modifica apportata alle attività secondarie della storia si riflette sulla storia. I punti o le ore del brano combinato per tutte le sottoattività determinano i punti o le ore del racconto principale.

Ad esempio, se una storia ha una sola sottoattività valutata a 4 punti, anche la storia stessa ha 4 punti. Se si modifica il valore del punto della sottoattività a 3, il valore del punto del brano principale viene modificato in 3. Se si crea un&#39;altra sottoattività sullo stesso brano e si imposta il valore del punto per la sottoattività su 4, il valore del punto del brano viene modificato in 7 per riflettere il valore combinato del punto per entrambe le sottoattività.

Questa stessa logica si applica alle sottoattività di secondo livello (sottoattività delle sottoattività). Se una sottoattività ha una o più sottoattività di secondo livello, la sottoattività viene calcolata in base alle sottoattività di secondo livello.

## Relazione tra la bacheca della storia e il backlog

>[!NOTE]
>
>Le informazioni contenute in questa sezione si applicano solo alle visualizzazioni agili su un&#39;iterazione; le visualizzazioni agili su un progetto non utilizzano un backlog. Per ulteriori informazioni sulle differenze tra le visualizzazioni agili di un’iterazione e di un progetto, consulta &quot;Differenze quando si utilizza il [!UICONTROL Agile] Visualizza i versi di un progetto su un&#39;iterazione&quot; in [Gestire un progetto nella vista Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).)

Il backlog di iterazione mostra solo storie o sottoattività in cui è possibile impostare una stima. Se un brano padre presenta attività secondarie visualizzate sulla bacheca del racconto (poiché sono assegnate allo stesso team agile e appartengono all&#39;iterazione), l&#39;attività principale non viene visualizzata nel backlog. In questa situazione, solo le sottoattività vengono visualizzate nel backlog, mentre le sottoattività e il brano principale vengono visualizzati nel storyboard.

Ad esempio, supponiamo che la storia A contenga la sottoattività 1 e la sottoattività 2 (e che entrambe le sottoattività siano assegnate allo stesso team agile). In questa situazione, la storia A viene visualizzata sulla tavola dei racconti in una corsia da nuoto con sottoattività 1 e sottoattività 2. Tuttavia, nel backlog vengono visualizzati solo i campi Sottoattività 1 e Sottoattività 2.

Questa stessa logica si applica alle sottoattività di secondo livello (sottoattività delle sottoattività). Se una sottoattività ha una o più sottoattività di secondo livello assegnate allo stesso team agile e appartengono all’iterazione, nel backlog viene visualizzata solo la sottoattività di secondo livello.

Per ulteriori informazioni sul backlog, vedi [Gestire il backlog agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).
