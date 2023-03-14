---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica sulla data di handoff dell’attività
description: La data di handoff è la data in cui un'attività diventa disponibile per il lavoro. In genere, ciò significa che i suoi predecessori si sono risolti e che l’assegnatario dell’attività può iniziare a lavorarci.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: b2859f3d268bd947fba5bb0280677465b3039d93
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 3%

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

* **Quando l’attività ha un predecessore incompleto**: la data di handoff per l’attività è nulla.
* **Quando l’attività ha un predecessore completo**: la data di handoff corrisponde alla data di completamento effettiva dell&#39;attività predecessore. Se il predecessore presenta un ritardo, Workfront calcola la Data handoff dell&#39;attività successore utilizzando la formula seguente:

   `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

   Per informazioni sul tempo di ritardo, consulta [Panoramica sui tipi di ritardo](../use-prdcssrs/lag-types.md).

   Se l&#39;attività successore ha più di un predecessore, la data di handoff viene calcolata in base alla data di completamento effettiva più recente dei predecessori. Ad esempio, se le date di completamento effettive dei due predecessori sono l’8 novembre 2022 e il 20 novembre 2022, la data di handoff del successore è il 20 novembre 2022.

   >[!NOTE]
   >
   >   Il calcolo della data di handoff di un&#39;attività successore in base alla data di completamento effettiva o a un&#39;attività predecessore è lo stesso indipendentemente dal fatto che il predecessore sia applicato o meno. Per ulteriori informazioni sui predecessori imposti, consulta [Imponi predecessori](../use-prdcssrs/enforced-predecessors.md).


* **Quando l’attività non ha un predecessore e**:

   * **La data di inizio pianificata è nel passato**: la data di handoff corrisponde alla data di inizio pianificata del progetto.
   * **La data di inizio pianificata è nel futuro (qualsiasi data successiva alla data corrente)**: la data di handoff corrisponde alla data di inizio pianificata del progetto.

>[!NOTE]
>
>Quando l&#39;attività ha un predecessore per più progetti, la data di handoff del successore viene ricalcolata solo quando si verifica una delle seguenti situazioni:
>
>* La timeline del progetto del successore viene ricalcolata manualmente. Per ricalcolare la sequenza temporale è necessario disporre delle autorizzazioni di gestione per il progetto.
>* La sequenza temporale del progetto del successore viene ricalcolata automaticamente di notte.
>
>Per informazioni sul ricalcolo della sequenza temporale del progetto, consulta [Ricalcolare i timeline dei progetti](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **Quando l&#39;attività ha un vincolo forzato per le Date Pianificate**: la data di handoff varia a seconda del tipo di vincolo e del fatto che l&#39;attività abbia o meno una data di inizio effettiva.\
   Di seguito sono riportati i vincoli obbligatori per le attività:

   * Deve ininziare al
   * Deve Finire al
   * Iniziare non Prima di
   * Iniziare non Dopo di
   * Data Fissa

   Esistono i seguenti scenari:

   * Quando per l&#39;attività è impostato il vincolo Deve iniziare il o Non iniziare prima di, la Data handoff corrisponde alla Data vincolo, a meno che non sia presente una Data inizio effettiva per l&#39;attività. Se sull&#39;attività è presente una data di inizio effettiva, la data di handoff è la data di completamento effettiva del predecessore.
   * Quando per l&#39;attività è impostato il vincolo Deve finire il o Inizia non dopo il, la Data handoff è sempre la Data di completamento effettiva del predecessore, indipendentemente dal fatto che l&#39;attività abbia o meno una Data di inizio effettiva.
   * Quando l&#39;attività ha un vincolo di Date fisse, la Data handoff è la Data inizio pianificata dell&#39;attività, indipendentemente dal fatto che abbia o meno un predecessore e dal fatto che il predecessore sia stato completato o meno.


## Individuare la data di handoff

È possibile visualizzare la Data handoff di un&#39;attività in un report di attività o la visualizzazione di un elenco di attività.\
Per ulteriori informazioni sulla creazione di un rapporto, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
