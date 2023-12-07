---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Panoramica dei tipi di relazione tra attività
description: I tipi di dipendenza si riferiscono alle relazioni precedenti tra le attività. Definiscono quando l'attività dipendente può iniziare o finire in base all'inizio o alla fine del predecessore.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: 45c82f659d02dca69d2a2c390b084330773d4252
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Panoramica dei tipi di relazione tra attività

I tipi di dipendenza si riferiscono alle relazioni precedenti tra le attività. Definiscono quando l&#39;attività dipendente può iniziare o finire in base all&#39;inizio o alla fine del predecessore.

>[!IMPORTANT]
>
>Adobe Workfront non limita l&#39;avvio o la conclusione delle attività dipendenti in base ai tipi di relazione, a meno che non vengano applicate le relazioni predecessori. Per informazioni sull&#39;applicazione dei predecessori, vedere [Imponi predecessori](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

Quando si stabilisce questa relazione tra le attività, è necessario specificare il tipo di dipendenza di una relazione predecessore.

Per ulteriori informazioni sui predecessori, vedere [Panoramica dei predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Di seguito sono riportati i tipi di dipendenza di Workfront:

* **Fine-Inizio (fs)**: l&#39;attività predecessore deve terminare prima che l&#39;attività dipendente possa iniziare. Si tratta del tipo di dipendenza predefinito, utilizzato quando non è specificato alcun altro tipo di dipendenza.
* **Fine-Fine (ff)**: l&#39;attività predecessore deve terminare prima che l&#39;attività dipendente possa terminare.
* **Inizio-Inizio (ss)**: l&#39;attività predecessore deve iniziare prima che l&#39;attività dipendente possa iniziare. Non è possibile avviare l&#39;attività dipendente a meno che il predecessore non abbia almeno iniziato.
* **Inizio-Fine (sf)**: l&#39;attività predecessore deve iniziare prima che l&#39;attività dipendente possa terminare. È possibile avviare l&#39;attività dipendente prima dell&#39;inizio del predecessore, ma non è possibile terminarla se il predecessore non è stato avviato.
* **Avvio programmato (sd)**: in questo modo un&#39;attività viene pianificata come Fine-Inizio, ma il tipo di applicazione effettivo è Fine-Fine. In questo caso, l&#39;attività dipendente viene programmata per iniziare dopo il completamento dell&#39;attività predecessore. Tuttavia, l&#39;imposizione consente di avviare l&#39;attività dipendente in qualsiasi momento, ma non può terminare fino al completamento dell&#39;attività predecessore.

>[!NOTE]
>
>Le abbreviazioni per i tipi di dipendenza vengono utilizzate negli elenchi di task per definire le relazioni dei predecessori. Per ulteriori informazioni, consulta [Esempi di valori predecessori in un elenco attività](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list) in [Panoramica dei predecessori delle attività](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md).

