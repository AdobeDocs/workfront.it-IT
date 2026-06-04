---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Panoramica Ciclo Dipendenza Attività
description: Quando si aggiungono relazioni predecessori ad attività, è possibile che si verifichino loop di dipendenza. Per informazioni sui predecessori, vedere Panoramica sui predecessori delle attività.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
TQID: https://experienceleague.adobe.com/cQbPOUES-tmSgZTpXrft8lQby-ubPmI-TZ1PjdGURMc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 263
ht-degree: 1%

---

# Panoramica del ciclo di dipendenza delle attività

Quando si aggiungono relazioni predecessori ad attività, è possibile che si verifichino loop di dipendenza. Per informazioni sui predecessori, vedere [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Panoramica del loop di dipendenza

I loop di dipendenza si verificano quando due o più attività dipendono l&#39;una dall&#39;altra vengono completate. Adobe Workfront non consente di creare una relazione predecessore tra attività se crea un loop di dipendenza.

**Esempio:** l&#39;attività 2 è un predecessore dell&#39;attività 1, pertanto è necessario completare l&#39;attività 2 prima di poter iniziare a lavorare sull&#39;attività 1.

Se si tenta di impostare l&#39;attività 1 come predecessore dell&#39;attività 2, viene visualizzato un errore di loop di dipendenza perché non è possibile avviare l&#39;attività 1 fino al completamento dell&#39;attività 2, ma l&#39;attività 2 non può essere avviata fino al completamento dell&#39;attività 1.

![Messaggio di errore del loop di dipendenza](assets/dependency-loop-error-message-350x209.png)

![Ciclo di dipendenza nell&#39;elenco attività](assets/dependency-loop-in-task-list-nwe-350x97.png)

## Considerazioni sui loop di dipendenza

* I loop di dipendenza possono coinvolgere più di due attività. A volte, un numero qualsiasi di padri delle attività che si stanno connettendo con una relazione predecessore è quello che crea il loop di dipendenza.
* Un ciclo di dipendenza può anche verificarsi se si tenta di rendere un padre predecessore di un figlio.
* Nel caso di un loop di dipendenza non è possibile salvare le attività o il progetto. Per correggere il loop di dipendenza, è necessario rivalutare la relazione predecessore tra le attività elencate nel messaggio di errore e rimuovere i conflitti prima di salvare le attività o il progetto.


