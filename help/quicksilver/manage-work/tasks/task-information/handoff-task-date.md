---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica sulla data di sospensione attività
description: La data di consegna è la data in cui un'attività diventa disponibile per il lavoro. Ciò significa tipicamente che i suoi predecessori hanno risolto e che l'assegnatario dell'attività può iniziare a lavorarci.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: 39efbf1d678cf85e9b6b61744fb046664992370c
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 3%

---

# Panoramica sulla data di sospensione attività

La data di consegna è la data in cui un&#39;attività diventa disponibile per il lavoro. Ciò significa tipicamente che i suoi predecessori hanno risolto e che l&#39;assegnatario dell&#39;attività può iniziare a lavorarci.

>[!TIP]
>
>Le date di consegna non esistono per problemi e progetti.

## Modalità di calcolo della data di consegna da parte di Adobe Workfront

>[!NOTE]
>
>La data di consegna viene calcolata solo se lo stato del progetto corrisponde ai seguenti stati:
>
>* In sospeso
>* Attuali
>* Completato
>* Morto
>


Workfront utilizza le regole seguenti per calcolare la data di consegna di un&#39;attività:

* **Quando l&#39;attività ha un predecessore incompleto**: La data di consegna per l&#39;attività è null.
* **Quando l&#39;attività ha un predecessore completo**: La data di consegna corrisponde alla data di completamento effettivo dell&#39;attività predecessore. Se il predecessore ha un ritardo, Workfront calcola la data di consegna dell&#39;attività successiva utilizzando la seguente formula:

   `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

   Per informazioni sul tempo di ritardo, vedi [Panoramica dei tipi di ritardo](../use-prdcssrs/lag-types.md).

   Se l&#39;attività successore ha più di un predecessore, la data di consegna viene calcolata in base alla data di completamento effettivo più recente dei predecessori. Ad esempio, se le date di completamento effettivo dei due predecessori sono l’8 novembre 2022 e il 20 novembre 2022, la data di consegna del successore sarà il 20 novembre 2022.

   >[!NOTE]
   >
   >   Il calcolo della data di consegna di un&#39;attività successore in base alla data di completamento effettivo o a un&#39;attività predecessore è lo stesso, indipendentemente dal fatto che il predecessore sia applicato o meno. Per ulteriori informazioni sui predecessori applicati, consulta [Applica predecessori](../use-prdcssrs/enforced-predecessors.md).


* **Quando l’attività non ha predecessori e**:

   * **La data di inizio prevista è passata**: La data di consegna è la stessa della data di inizio prevista del progetto.
   * **La data di inizio prevista è futura (qualsiasi data successiva alla data corrente)**: La data di consegna è la stessa della data di inizio prevista del progetto.

>[!NOTE]
>
>Quando l’attività ha un predecessore tra progetti diversi, la data di abbandono del successore ricalcola solo quando si verifica uno dei seguenti casi:
>
>* È possibile ricalcolare manualmente la timeline del progetto del successore. Per ricalcolare la timeline, è necessario disporre delle autorizzazioni Gestisci per il progetto.
>* La tempistica del progetto del successore viene automaticamente ricalcolata di notte.
>
>Per informazioni sul ricalcolo della timeline del progetto, consulta [Ricalcolare le timeline dei progetti](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **Quando l&#39;attività presenta un vincolo forzato per le date previste**: La data di consegna è sempre la stessa della data impostata dal vincolo, indipendentemente da qualsiasi altra condizione.\
   Di seguito sono riportati i vincoli imposti alle attività:

   * Deve ininziare al
   * Deve Finire al
   * Iniziare non Prima di
   * Iniziare non Dopo di
   * Data fissa

## Individua la data di consegna

È possibile visualizzare la data di consegna di un&#39;attività in un rapporto di attività o nella visualizzazione di un elenco di attività.\
Per ulteriori informazioni sulla creazione di un rapporto, vedi [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
