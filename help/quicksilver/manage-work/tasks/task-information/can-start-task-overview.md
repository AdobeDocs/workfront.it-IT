---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica di "Can Start" per le attività
description: Quando un’attività è pronta per iniziare, Adobe Workfront aggiunge un indicatore Can Start all’attività per identificare facilmente che è sicuro per te iniziare a lavorare sull’attività. È possibile visualizzare questo indicatore nella visualizzazione di un elenco di attività o di un report.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Panoramica di &quot;Può iniziare&quot; per le attività

Quando un’attività è pronta per iniziare, Adobe Workfront aggiunge un indicatore Can Start all’attività per identificare facilmente che è sicuro per te iniziare a lavorare sull’attività. È possibile visualizzare questo indicatore nella visualizzazione di un elenco di attività o di un report.

Quando l&#39;attività è pronta per essere elaborata, il campo Può iniziare dell&#39;attività è impostato su True.

## Come Workfront contrassegna un’attività come &quot;Può iniziare&quot;

Workfront verifica quanto segue prima di contrassegnare un&#39;attività come True per il campo Può iniziare:

* Indica se il valore di Può iniziare per l&#39;elemento padre è impostato su True, se l&#39;attività ha un elemento padre. Se il valore dell&#39;elemento padre è False, anche il valore di Can Start per tutte le sottoattività sarà impostato su False.
* Indica se i predecessori dell&#39;attività e i predecessori dei genitori sono completi. Se sono state completate, il valore Può iniziare dell&#39;attività è impostato su True. Se uno dei predecessori delle attività o dei predecessori dei relativi padri non è completo o ha lo stato Completo - In attesa di approvazione, il valore Può iniziare per l&#39;attività è impostato su False.
* Indica se il tipo di relazione tra attività è Start-Start o Start-Finish. Se il tipo di relazione è Inizio-Inizio o Inizio-Fine, per l&#39;attività dipendente il flag &quot;Può iniziare&quot; sarà impostato su True dopo che l&#39;attività predecessore è in corso o dopo che la percentuale di completamento dell&#39;attività predecessore è superiore all&#39;1%.

  Per informazioni sui predecessori delle attività, vedere [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Considerazioni sull&#39;identificazione delle attività pronte per l&#39;avvio

* Se il tipo di dipendenza tra un&#39;attività e i suoi predecessori è Inizio-Inizio, il predecessore deve iniziare prima che la relazione predecessore sia considerata risolta e che le attività successori possano iniziare. Per informazioni sui tipi di relazione, vedere [Panoramica sui tipi di relazione tra attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* Se un&#39;attività ha un predecessore per più progetti, il completamento del predecessore non attiva l&#39;indicatore Può iniziare per applicarlo automaticamente al successore. È necessario ricalcolare manualmente la sequenza temporale del progetto del successore oppure è necessario che Workfront ricalcoli automaticamente la sequenza temporale prima che l&#39;attività successore venga visualizzata come attività Può iniziare. Per ulteriori informazioni sul ricalcolo delle sequenze temporali del progetto, vedere [Ricalcolare le sequenze temporali del progetto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

  Per informazioni sui predecessori di progetti incrociati, vedi [Creare predecessori di progetti incrociati](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
