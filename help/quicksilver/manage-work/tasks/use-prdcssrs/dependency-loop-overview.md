---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Panoramica del ciclo di dipendenza attività
description: Quando si aggiungono relazioni predecessori alle attività, è possibile che si verifichino cicli di dipendenza. Per informazioni sui predecessori, vedere Panoramica dei predecessori delle attività.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Panoramica del ciclo di dipendenza attività

Quando si aggiungono relazioni predecessori alle attività, è possibile che si verifichino cicli di dipendenza. Per informazioni sui predecessori, consulta [Panoramica dei predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Panoramica del ciclo di dipendenza

I cicli di dipendenza si verificano quando due o più attività dipendono l’una dall’altra da completare. Adobe Workfront non consente di creare una relazione predecessore tra attività se crea un ciclo di dipendenza.

**Esempio:** L&#39;attività 2 è un predecessore dell&#39;attività 1, il che significa che è necessario completare l&#39;attività 2 prima di poter iniziare a lavorare sull&#39;attività 1.

Se si tenta di rendere l&#39;attività 1 un predecessore dell&#39;attività 2, si ottiene un errore di ciclo di dipendenza perché non è possibile avviare l&#39;attività 1 fino al completamento dell&#39;attività 2, ma l&#39;attività 2 non può essere avviata fino al completamento dell&#39;attività 1.

![](assets/dependency-loop-error-message-350x209.png)

![](assets/dependency-loop-in-task-list-nwe-350x97.png)

## Considerazioni sui cicli di dipendenza

* I cicli di dipendenza possono includere più di due attività. A volte qualsiasi numero di elementi padre delle attività che si collegano a una relazione predecessore sono quelli che creano il ciclo di dipendenza.
* Un ciclo di dipendenza può anche verificarsi se si tenta di rendere un padre il predecessore di un figlio.
* Nel caso di un ciclo di dipendenza non è possibile salvare le attività o il progetto. Per correggere il ciclo di dipendenza, è necessario rivalutare la relazione predecessore tra le attività elencate nel messaggio di errore e rimuovere i conflitti prima di salvare le attività o il progetto.

 
