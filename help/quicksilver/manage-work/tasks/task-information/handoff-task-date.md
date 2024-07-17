---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica sulla data di handoff dell’attività
description: La data di handoff è la data in cui un'attività diventa disponibile per il lavoro. In genere, ciò significa che i suoi predecessori si sono risolti e che l’assegnatario dell’attività può iniziare a lavorarci.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 2%

---

# Panoramica sulla data di handoff dell’attività

La data di handoff è la data in cui un&#39;attività diventa disponibile per il lavoro. In genere, ciò significa che i suoi predecessori si sono risolti e che l’assegnatario dell’attività può iniziare a lavorarci.

>[!TIP]
>
>Le date di handoff non esistono per problemi e progetti.

## Calcolo della data di handoff in Adobe Workfront

>[!NOTE]
>
>La data di handoff viene calcolata solo se lo stato del progetto è uguale ai seguenti stati:
>
>* In sospeso
>* Attuali
>* Completato
>* Morto
>

Workfront utilizza le seguenti regole per calcolare la Data handoff di un’attività:

* **Quando l&#39;attività ha un predecessore incompleto**: la data di handoff per l&#39;attività è nulla.
* **Quando l&#39;attività ha un predecessore completo**: la data di handoff è uguale alla data di completamento effettiva dell&#39;attività predecessore. Se il predecessore presenta un ritardo, Workfront calcola la Data handoff dell&#39;attività successore utilizzando la formula seguente:

  `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

  Per informazioni sul tempo di ritardo, vedere [Panoramica sui tipi di ritardo](../use-prdcssrs/lag-types.md).

  Se l&#39;attività successore ha più di un predecessore, la data di handoff viene calcolata in base alla data di completamento effettiva più recente dei predecessori. Ad esempio, se le date di completamento effettive dei due predecessori sono l’8 novembre 2022 e il 20 novembre 2022, la data di handoff del successore è il 20 novembre 2022.

  >[!NOTE]
  >
  >   Il calcolo della data di handoff di un&#39;attività successore in base alla data di completamento effettiva o a un&#39;attività predecessore è lo stesso indipendentemente dal fatto che il predecessore sia applicato o meno. Per ulteriori informazioni sui predecessori imposti, vedere [Imponi predecessori](../use-prdcssrs/enforced-predecessors.md).


* **Quando l&#39;attività non ha predecessori e**:

   * **La data di inizio pianificata è nel passato**: la data di handoff corrisponde alla data di inizio pianificata del progetto se per l&#39;attività non è impostato alcun vincolo forzato. Per i casi in cui le attività hanno vincoli forzati, vedere la sezione seguente &quot;Quando l&#39;attività ha un vincolo forzato per le date pianificate&quot;.
   * **La data di inizio pianificata è nel futuro (qualsiasi data successiva alla data corrente)**: la data di handoff è uguale alla data di inizio pianificata dell&#39;attività se l&#39;attività non ha vincoli forzati impostati. Per i casi in cui le attività hanno vincoli forzati, vedere la sezione seguente &quot;Quando l&#39;attività ha un vincolo forzato per le date pianificate&quot;.

>[!NOTE]
>
>Quando l&#39;attività ha un predecessore per più progetti, la data di handoff del successore viene ricalcolata solo quando si verifica una delle seguenti situazioni:
>
>* La timeline del progetto del successore viene ricalcolata manualmente. Per ricalcolare la sequenza temporale è necessario disporre delle autorizzazioni di gestione per il progetto.
>* La sequenza temporale del progetto del successore viene ricalcolata automaticamente di notte.
>
>Per informazioni sul ricalcolo della sequenza temporale del progetto, vedere [Ricalcolare le sequenze temporali del progetto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **Quando l&#39;attività ha un vincolo forzato per le date pianificate**: la data di handoff varia a seconda del tipo di vincolo e del fatto che l&#39;attività abbia o meno una data di inizio effettiva.\
  Di seguito sono riportati i vincoli obbligatori per le attività:

   * Deve ininziare al
   * Deve Finire al
   * Iniziare non Prima di
   * Iniziare non Dopo di
   * Data Fissa

  Esistono i seguenti scenari:

   * **Quando l&#39;attività ha un vincolo Deve iniziare il o Non iniziare prima del**: se la data del vincolo dell&#39;attività è nel passato e non è presente una data di inizio effettiva per l&#39;attività (l&#39;attività non è ancora iniziata), la data di handoff è la data più vicina alla quale l&#39;attività può iniziare a essere elaborata. Se l&#39;attività è iniziata, la data di handoff corrisponde alla data di inizio del progetto.
   * **Quando l&#39;attività ha un vincolo Deve finire il o Deve iniziare non oltre il**: se la data del vincolo dell&#39;attività è nel futuro e non è presente una data di inizio effettiva sull&#39;attività (l&#39;attività non è ancora iniziata), la data di handoff è la data di inizio pianificata dell&#39;attività. Se sull&#39;attività è presente la data di inizio effettiva, la data di handoff sarà la data di inizio del progetto.
   * **Quando l&#39;attività ha un vincolo di Date Fisse**: La Data di handoff è la Data di inizio pianificata dell&#39;attività, indipendentemente dal fatto che abbia o meno un predecessore e dal fatto che il predecessore sia stato completato o meno.

<!--these are old descriptions, edited by Anna As. on August 25, 2023 in this issue - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/64c0032500018fabd4fc484167eb10dc/updates
   * When the task has a constraint of Must Start On or Start No Earlier Than, the Handoff Date is the Constraint date, unless there is an Actual Start Date on the task. If there is an Actual Start Date on the task, the Handoff Date is the Actual Completion Date of the predecessor.
   * When the task has a constraint of Must Finish On or Start No Later Than, the Handoff Date is always the Actual Completion Date of the predecessor, regardless of whether there is an Actual Start Date on the task or not. 
   * When the task has a constraint of Fixed Dates, the Handoff Date is the Planned Start Date of the task, regardless of whether it has a predecessor or not and regardless of whether the predecessor is completed or not.

-->

## Individuare la data di handoff

È possibile visualizzare la Data handoff di un&#39;attività in un report di attività o la visualizzazione di un elenco di attività.\
Per ulteriori informazioni sulla creazione di un report, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
