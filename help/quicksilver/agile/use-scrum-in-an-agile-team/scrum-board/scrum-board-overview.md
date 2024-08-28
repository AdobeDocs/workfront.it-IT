---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: Panoramica della bacheca Scrum
description: Lo storyboard agile Scrum viene visualizzato insieme allo stato di completamento e al grafico a burn-down.
author: Lisa
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# Panoramica della bacheca [!UICONTROL Scrum]

Lo storyboard Agile [!UICONTROL Scrum] viene visualizzato insieme allo stato di completamento e al grafico di burn-down. Questi componenti Agile sono disponibili nelle seguenti situazioni in [!UICONTROL Adobe Workfront]:

* Sulle iterazioni agili. Per ulteriori dettagli sull&#39;utilizzo dello storyboard agile, del grafico a burn-down e dello stato di completamento in un ambiente agile puro (con backlog e iterazione), vedere [Operazioni in un ambiente agile](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).
* Quando visualizzi un progetto in una visualizzazione agile. Per informazioni su come sfruttare lo storyboard agile, il grafico Burndown e lo stato di completamento all&#39;interno di un progetto esistente, vedi [Gestire un progetto in Agile View](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

![Iterazione Agile](assets/agile-iteration-with-callouts.png)

## Funzioni e layout storyboard

![Storyboard Agile](assets/agile-storyboard-callouts.png)

Lo storyboard è costituito dai seguenti elementi:

* **[!UICONTROL Storia principale] Colonna:** A differenza delle altre colonne della bacheca delle storie, la colonna [!UICONTROL Storia principale] non è uno stato di attività, ma esiste per ospitare le storie che contengono sottoattività nell&#39;iterazione o nel progetto. In questa colonna possono risiedere solo i brani principali con almeno un&#39;attività secondaria nella bacheca delle storie. Le storie principali non passano dallo stato allo stato lungo tutta la bacheca delle storie.

  In un&#39;iterazione, questa colonna viene visualizzata nella bacheca delle storie solo quando uno o più brani della bacheca delle storie contengono almeno una sottoattività che soddisfa i seguenti requisiti:

   * Assegnato allo stesso team agile dell’attività principale
   * Appartiene all&#39;iterazione

     In un progetto questa colonna viene visualizzata ogni volta che un&#39;attività include almeno una sottoattività.

     ![Colonna storia principale](assets/agile-parentstory-swimlane.png)

* **Stati attività:** indicare l&#39;avanzamento di un brano nell&#39;iterazione o nel progetto in base alla colonna di stato in cui si trova il brano.

  Gli stati delle attività possono essere personalizzati per il progetto modificando la visualizzazione agile, come descritto in [Creare o personalizzare una visualizzazione agile](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [Panoramica delle visualizzazioni in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* **Corsia di nuoto:** Quando una storia principale e le relative sottoattività vengono visualizzate nella bacheca delle storie, viene creata una corsia di nuoto specifica per la storia e le relative sottoattività. Ciò fornisce una distinzione visiva per visualizzare meglio come le sottoattività di un brano progrediscono lungo la bacheca del brano.

  In un&#39;iterazione, le corsie per il nuoto vengono visualizzate sullo storyboard solo quando un brano sullo storyboard contiene almeno un&#39;attività secondaria che soddisfa i seguenti requisiti:

   * Assegnato allo stesso team agile dell’attività principale
   * Appartiene all&#39;iterazione

  In un progetto le corsie preferenziali vengono visualizzate ogni volta che un&#39;attività ha almeno una sottoattività o un&#39;attività padre.

* **Singole storie:** le singole storie e i singoli problemi sono visualizzati sotto qualsiasi corsia di nuoto sulla bacheca delle storie. Questo fornisce una distinzione visiva dalle storie che fanno parte di una corsia di nuoto.

## Relazione tra le sottoattività e i brani

Se un brano contiene sottoattività, non è possibile aggiornare alcuna informazione sul brano principale stesso, ad esempio punti/ore o percentuale di completamento. Inoltre, non è possibile spostare la storia in un&#39;altra pagina per aggiornarne lo stato. Piuttosto, qualsiasi modifica apportata alle sottoattività del brano viene riflessa sul brano. I punti o le ore del brano combinato per tutte le sottoattività determinano i punti o le ore del brano principale.

Ad esempio, se una storia ha una sola sottoattività valutata in 4 punti, anche la storia stessa ha 4 punti. Se modificate il valore del punto della sottoattività in 3, il valore del punto del brano padre viene modificato in 3. Se create un&#39;altra sottoattività sullo stesso brano e impostate il valore del punto per tale sottoattività su 4, il valore del punto del brano viene modificato su 7 in modo da riflettere il valore del punto combinato per entrambe le sottoattività.

La stessa logica si applica alle sottoattività di secondo livello (sottoattività delle sottoattività). Se una sottoattività include una o più sottoattività di secondo livello, la sottoattività viene calcolata in base alle sottoattività di secondo livello.

## Relazione tra storyboard e backlog

>[!NOTE]
>
>Le informazioni contenute in questa sezione si applicano solo alle visualizzazioni Agile in un’iterazione; le visualizzazioni Agile in un progetto non utilizzano un backlog. (Per ulteriori informazioni sulle differenze tra le visualizzazioni Agile in un&#39;iterazione e un progetto, vedi &quot;Differenze quando si utilizza la visualizzazione [!UICONTROL Agile] per i versi di un progetto in un&#39;iterazione&quot; in [Gestire un progetto nella visualizzazione Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).)

Il backlog dell&#39;iterazione mostra solo brani o sottoattività in cui è possibile impostare una stima. Se un brano principale include sottoattività visualizzate sullo storyboard (perché sono assegnate allo stesso team agile e appartengono all&#39;iterazione), l&#39;attività principale non viene visualizzata nel backlog. In questa situazione, nel backlog vengono visualizzate solo le sottoattività, mentre le sottoattività e il brano padre vengono visualizzati sullo storyboard.

Si supponga, ad esempio, che la storia A contenga la sottoattività 1 e la sottoattività 2 e che entrambe le sottoattività siano assegnate allo stesso team agile. In questa situazione, la storia A viene visualizzata sulla bacheca delle storie in una corsia di nuoto con le sottoattività 1 e 2. Tuttavia, nel backlog vengono visualizzate solo la sottoattività 1 e la sottoattività 2.

La stessa logica si applica alle sottoattività di secondo livello (sottoattività delle sottoattività). Se a una sottoattività sono assegnate una o più sottoattività di secondo livello allo stesso team Agile e appartengono all&#39;iterazione, nel backlog viene visualizzata solo la sottoattività di secondo livello.

Per ulteriori informazioni sul backlog, vedere [Gestione del backlog Agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).
