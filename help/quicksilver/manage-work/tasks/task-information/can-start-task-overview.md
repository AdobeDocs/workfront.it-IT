---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica di '`Can Start` per le attività'
description: Quando un'attività è pronta per essere avviata, Adobe Workfront aggiunge all'attività un indicatore di avvio rapido per identificare facilmente che è sicuro iniziare a lavorare sull'attività. È possibile visualizzare questo indicatore nella visualizzazione di un elenco di attività o di un report.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Panoramica &quot;Can Start&quot; per le attività

Quando un&#39;attività è pronta per essere avviata, Adobe Workfront aggiunge all&#39;attività un indicatore di avvio rapido per identificare facilmente che è sicuro iniziare a lavorare sull&#39;attività. È possibile visualizzare questo indicatore nella visualizzazione di un elenco di attività o di un report.

Quando l&#39;attività è pronta, il campo Può iniziare sull&#39;attività è impostato su True.

## Come Workfront contrassegna un’attività come &quot;Può iniziare&quot;

Workfront verifica i seguenti elementi prima di contrassegnare un&#39;attività come True per il campo Can Start:

* Se l&#39;attività ha un elemento padre, controlla se il valore di Can Start per l&#39;elemento padre è impostato su True. Se il valore dell&#39;elemento padre è False, anche tutte le sottoattività avranno il valore di Can Start impostato su False. 
* Controlla anche se i predecessori del compito e i predecessori dei loro genitori sono completi. Se sono completi, il valore Can Start per l&#39;attività è impostato su True. Se uno dei predecessori dell&#39;attività o dei predecessori dei relativi genitori non è completo o se lo stato è Approvazione in attesa di completamento, il valore Can Start per l&#39;attività è impostato su False. 

   Per informazioni sui predecessori delle attività, consulta [Panoramica dei predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Considerazioni sull’identificazione delle attività pronte per essere avviate

* Se il Tipo di dipendenza tra un&#39;attività e i relativi predecessori è Start-Start, il predecessore deve iniziare prima che la relazione predecessore sia considerata risolta e le attività successive possono iniziare. Per informazioni sui tipi di dipendenza, consulta [Panoramica dei tipi di dipendenza dell&#39;attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* Se un&#39;attività ha un predecessore tra progetti diversi, il completamento del predecessore non attiva l&#39;indicatore Can Start da applicare automaticamente al successore. È necessario ricalcolare manualmente la timeline del progetto del successore oppure Workfront deve ricalcolarla automaticamente, prima che l&#39;attività successore venga visualizzata come attività Can Start. Per ulteriori informazioni sul ricalcolo delle timeline dei progetti, consulta [Ricalcolare le timeline dei progetti](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

   Per informazioni sui predecessori tra progetti, consulta [Creare predecessori tra progetti](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
