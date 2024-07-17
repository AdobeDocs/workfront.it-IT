---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Panoramica del ciclo di dipendenza delle attività
description: Quando si aggiungono relazioni predecessori ad attività, è possibile che si verifichino loop di dipendenza. Per informazioni sui predecessori, vedere Panoramica sui predecessori delle attività.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Panoramica del ciclo di dipendenza delle attività

Quando si aggiungono relazioni predecessori ad attività, è possibile che si verifichino loop di dipendenza. Per informazioni sui predecessori, vedere [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Panoramica del loop di dipendenza

I loop di dipendenza si verificano quando due o più attività dipendono l&#39;una dall&#39;altra vengono completate. Adobe Workfront non consente di creare una relazione predecessore tra attività se crea un loop di dipendenza.

**Esempio:** l&#39;attività 2 è un predecessore dell&#39;attività 1, pertanto è necessario completare l&#39;attività 2 prima di poter iniziare a lavorare sull&#39;attività 1.

Se si tenta di impostare l&#39;attività 1 come predecessore dell&#39;attività 2, viene visualizzato un errore di loop di dipendenza perché non è possibile avviare l&#39;attività 1 fino al completamento dell&#39;attività 2, ma l&#39;attività 2 non può essere avviata fino al completamento dell&#39;attività 1.

![](assets/dependency-loop-error-message-350x209.png)

![](assets/dependency-loop-in-task-list-nwe-350x97.png)

## Considerazioni sui loop di dipendenza

* I loop di dipendenza possono coinvolgere più di due attività. A volte, un numero qualsiasi di padri delle attività che si stanno connettendo con una relazione predecessore è quello che crea il loop di dipendenza.
* Un ciclo di dipendenza può anche verificarsi se si tenta di rendere un padre predecessore di un figlio.
* Nel caso di un loop di dipendenza non è possibile salvare le attività o il progetto. Per correggere il loop di dipendenza, è necessario rivalutare la relazione predecessore tra le attività elencate nel messaggio di errore e rimuovere i conflitti prima di salvare le attività o il progetto.

 
