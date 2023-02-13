---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Panoramica dei tipi di dipendenza dell'attività
description: I tipi di dipendenza fanno riferimento alle relazioni predecessori tra le attività. Definiscono quando l'attività dipendente può iniziare o terminare in base all'inizio o alla fine del predecessore.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Panoramica dei tipi di dipendenza dell&#39;attività

I tipi di dipendenza fanno riferimento alle relazioni predecessori tra le attività. Definiscono quando l&#39;attività dipendente può iniziare o terminare in base all&#39;inizio o alla fine del predecessore.

>[!IMPORTANT]
>
>Adobe Workfront non limita l&#39;avvio o il completamento delle attività dipendenti in base ai tipi di dipendenza, a meno che le relazioni predecessori non vengano applicate. Per informazioni sull&#39;applicazione dei predecessori, consulta [Applica predecessori](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

È necessario specificare il tipo di dipendenza di una relazione predecessore quando si stabilisce questa relazione tra le attività.

Per ulteriori informazioni sui predecessori, consulta [Panoramica dei predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Di seguito sono riportati i tipi di dipendenza di Workfront:

* **Fine-Inizio (fs)**: L&#39;attività predecessore deve terminare prima che l&#39;attività dipendente possa essere avviata. Si tratta del tipo di dipendenza predefinito, utilizzato quando non viene specificato alcun altro tipo di dipendenza.
* **Fine-Fine (ff)**: L&#39;attività predecessore deve terminare prima del completamento dell&#39;attività dipendente.
* **Start-Start (ss)**: L&#39;attività predecessore deve essere avviata prima dell&#39;avvio dell&#39;attività dipendente. Non è possibile avviare l&#39;attività dipendente a meno che il predecessore non sia almeno iniziato.
* **Start-Finish (sf)**: L&#39;attività predecessore deve iniziare prima del completamento dell&#39;attività dipendente. È possibile avviare l&#39;attività dipendente prima dell&#39;avvio del predecessore, ma non è possibile completarla a meno che il predecessore non sia stato avviato.
* **Pianificazione-Start (sd)**: In questo modo si pianifica un&#39;attività come Fine-Inizio, ma il tipo di esecuzione effettivo è Fine-Fine. Quando si utilizza questa opzione, l&#39;attività dipendente viene pianificata per avviarsi dopo il completamento dell&#39;attività predecessore. Tuttavia, l&#39;applicazione lo rende in modo che l&#39;attività dipendente possa iniziare in qualsiasi momento, ma non possa terminare fino al termine dell&#39;attività predecessore.
