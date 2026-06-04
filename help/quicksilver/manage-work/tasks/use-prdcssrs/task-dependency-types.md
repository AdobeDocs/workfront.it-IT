---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Panoramica dei tipi di relazione attività
description: I tipi di dipendenza si riferiscono alle relazioni precedenti tra le attività. Definiscono quando l'attività dipendente può iniziare o finire in base all'inizio o alla fine del predecessore.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
TQID: https://experienceleague.adobe.com/AioKERGt0FLv1eBE5-evwa2d35fItwknWI-ZouBECSo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 322
ht-degree: 1%

---

# Panoramica dei tipi di dipendenza delle attività

<!-- Audited: 12/2023 -->

I tipi di dipendenza si riferiscono alle relazioni precedenti tra le attività. Definiscono quando l&#39;attività dipendente può iniziare o finire in base all&#39;inizio o alla fine del predecessore.

>[!IMPORTANT]
>
>Adobe Workfront non limita l&#39;avvio o la conclusione delle attività dipendenti in base ai tipi di relazione, a meno che non vengano applicate le relazioni predecessori. Per informazioni sull&#39;applicazione dei predecessori, vedere [Applicazione dei predecessori](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

Quando si stabilisce questa relazione tra le attività, è necessario specificare il tipo di dipendenza di una relazione predecessore.

Per ulteriori informazioni sui predecessori, vedere [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Di seguito sono riportati i tipi di dipendenza di Workfront:

* **Fine-Inizio (fs)**: l&#39;attività predecessore deve essere completata prima dell&#39;inizio dell&#39;attività dipendente. Si tratta del tipo di dipendenza predefinito, utilizzato quando non è specificato alcun altro tipo di dipendenza.
* **Fine-Fine (ff)**: l&#39;attività predecessore deve terminare prima che l&#39;attività dipendente possa terminare.
* **Inizio-Inizio (ss)**: l&#39;attività predecessore deve iniziare prima che l&#39;attività dipendente possa iniziare. Non è possibile avviare l&#39;attività dipendente a meno che il predecessore non abbia almeno iniziato.
* **Inizio-Fine (sf)**: l&#39;attività predecessore deve iniziare prima che l&#39;attività dipendente possa terminare. È possibile avviare l&#39;attività dipendente prima dell&#39;inizio del predecessore, ma non è possibile terminarla se il predecessore non è stato avviato.
* **Inizio pianificato (sd)**: pianifica un&#39;attività come Fine-Inizio, ma il tipo di imposizione effettivo è Fine-Fine. In questo caso, l&#39;attività dipendente viene programmata per iniziare dopo il completamento dell&#39;attività predecessore. Tuttavia, l&#39;imposizione consente di avviare l&#39;attività dipendente in qualsiasi momento, ma non può terminare fino al completamento dell&#39;attività predecessore.

>[!NOTE]
>
>Le abbreviazioni per i tipi di dipendenza vengono utilizzate negli elenchi di task per definire le relazioni dei predecessori. Per ulteriori informazioni, vedere [Esempi di valori dei predecessori in un elenco attività](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list) in [Panoramica sui predecessori attività](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md).

