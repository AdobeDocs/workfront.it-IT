---
product-area: templates
navigation-topic: templates-navigation-topic
title: Panoramica sui modelli di progetto
description: È possibile utilizzare i modelli di progetto per acquisire la maggior parte dei processi, delle informazioni e delle impostazioni ripetibili associati ai progetti dell'organizzazione.
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: ca4da5302198d8fffc8b706baa3b3aeaa1f738e3
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 1%

---

# Panoramica sui modelli di progetto

<!-- Audited: 12/2023 -->

È possibile utilizzare i modelli di progetto per acquisire la maggior parte dei processi, delle informazioni e delle impostazioni ripetibili associati ai progetti dell&#39;organizzazione.

È possibile definire operazioni, argomenti della coda, moduli personalizzati e allegare documenti nel modello.

Dopo aver creato i modelli, puoi allegarli ai progetti esistenti o utilizzarli per creare nuovi progetti. Tutte le informazioni contenute nel modello vengono trasferite ai progetti creati utilizzando tale modello.

## Vantaggi dell’utilizzo dei modelli in Adobe Workfront

Di seguito sono riportati alcuni dei vantaggi dell’utilizzo di modelli per la creazione di progetti:

* Consente di risparmiare tempo e fatica quando si creano nuovi progetti ripetitivi.
* Disponi di informazioni coerenti tra i progetti con ambito simile.
* È utile quando si riferiscono ai progetti. Ad esempio, puoi generare rapporti sui progetti che condividono lo stesso modello, per confrontarne l’avanzamento e trovare miglioramenti nelle modalità di completamento.
* Oltre a definire le impostazioni del progetto futuro, è possibile aggiungere a un modello le seguenti informazioni per il progetto futuro:

   * Attività
   * Documenti
   * Approvazioni
   * Dettagli coda
   * Argomenti Coda
   * Gruppi di argomenti
   * Regole di instradamento
   * Forms personalizzato
   * Informazioni sulla società e sul gruppo

## Best practice per la creazione di modelli

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

Durante la creazione dei modelli, considera quanto segue:

* Non assegnare utenti ad attività modello. Anche se è possibile non assegnare le attività, si consiglia di assegnare mansioni alle attività. Questo ti darà un&#39;idea di quali utenti potrebbero essere in grado di essere assegnati alle attività quando crei il progetto utilizzando il modello.
* Assegna sempre alle attività modello un valore Durata e Ore pianificate. Ogni attività del progetto deve essere associata a una durata che indica il tempo di apertura dell&#39;attività e a un valore Ora pianificata che indica il tempo effettivamente necessario per il completamento dell&#39;attività. Le attività senza queste informazioni non possono essere preventivate correttamente per le risorse quando si utilizzano strumenti di gestione delle risorse in Workfront.

  Per informazioni sulla durata, vedere i seguenti articoli:

   * [Panoramica della durata e del tipo di durata dell&#39;attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Panoramica della durata del progetto](../../../manage-work/projects/planning-a-project/project-duration.md)

  Per informazioni sulle ore pianificate, vedi [Panoramica sulle ore pianificate](../../../manage-work/tasks/task-information/planned-hours.md).

* Aggiungere le relazioni precedenti tra le attività alla fine, quando si ha una chiara comprensione dell&#39;intero piano di progetto futuro. L’aggiunta di predecessori alle attività modello è simile all’aggiunta di predecessori alle attività di un progetto.

  Per informazioni sull&#39;aggiunta di predecessori alle attività, vedere [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Indica con chi deve essere condiviso il modello per utilizzi futuri e con chi devono essere condivisi i progetti che verranno creati dal modello. Per informazioni sulla condivisione dei modelli, vedere [Condividere modelli di progetto](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Se possibile, utilizza i processi di approvazione globali e aggiungili ai modelli e alle attività modello. Questo consente di risparmiare tempo quando le attività o il progetto futuro dovranno passare attraverso le stesse approvazioni.

  Per informazioni sulla creazione di approvazioni, vedere [Creare un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Per informazioni sull&#39;associazione di un processo di approvazione a un elemento di lavoro, vedere [Associare un processo di approvazione nuovo o esistente a un lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Modi per creare i modelli

È possibile creare un nuovo modello nei modi seguenti:

* Da zero.\
  Per ulteriori informazioni sulla creazione di un nuovo modello, vedere [Creare un modello di progetto](../../../manage-work/projects/create-and-manage-templates/create-template.md).

* Da progetti esistenti, salvando un progetto come modello.\
  Per ulteriori informazioni sulla creazione di modelli da progetti esistenti, vedere [Creare un modello dal progetto](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).

* Copiandolo da un altro modello.\
  Per ulteriori informazioni sulla copia di un modello esistente, vedere [Copiare un modello di progetto](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Utilizzando i nostri modelli di esempio.\
  Per ulteriori informazioni sulla creazione dei modelli utilizzando i modelli di esempio, vedere [Creare modelli di progetto da esempi](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md).
