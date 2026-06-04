---
product-area: templates
navigation-topic: templates-navigation-topic
title: Panoramica sui modelli di progetto
description: È possibile utilizzare i modelli di progetto per acquisire la maggior parte dei processi, delle informazioni e delle impostazioni ripetibili associati ai progetti dell'organizzazione.
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
TQID: https://experienceleague.adobe.com/9RlRNqkZYIcLjI5-he3f2BMtoXj3R--8MQbVUFmRHqI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 702
ht-degree: 5%

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
   * Moduli personalizzati
   * Informazioni sulla società e sul gruppo

## Best practice per la creazione di modelli

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

Durante la creazione dei modelli, considera quanto segue:

* Non assegnare utenti ad attività modello. Anche se è possibile non assegnare le attività, si consiglia di assegnare mansioni alle attività. Questo ti darà un&#39;idea di quali utenti potrebbero essere in grado di essere assegnati alle attività quando crei il progetto utilizzando il modello.
* Assegna sempre alle attività modello un valore Durata e Ore pianificate. Ogni attività del progetto deve essere associata a una durata che indica il tempo di apertura dell&#39;attività e a un valore Ora pianificata che indica il tempo effettivamente necessario per il completamento dell&#39;attività. Le attività senza queste informazioni non possono essere preventivate correttamente per le risorse quando si utilizzano strumenti di gestione delle risorse in Workfront.

  Per informazioni sulla durata, vedere i seguenti articoli:

   * [Panoramica della durata e del tipo di durata dell&#39;attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Panoramica sulla durata del progetto](../../../manage-work/projects/planning-a-project/project-duration.md)

  Per informazioni sulle ore pianificate, consulta [Panoramica sulle ore pianificate](../../../manage-work/tasks/task-information/planned-hours.md).

* Aggiungere le relazioni precedenti tra le attività alla fine, quando si ha una chiara comprensione dell&#39;intero piano di progetto futuro. L’aggiunta di predecessori alle attività modello è simile all’aggiunta di predecessori alle attività di un progetto.

  Per informazioni sull&#39;aggiunta di predecessori alle attività, vedere [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Indica con chi deve essere condiviso il modello per utilizzi futuri e con chi devono essere condivisi i progetti che verranno creati dal modello. Per informazioni sulla condivisione dei modelli, vedere [Condividere modelli di progetto](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Se possibile, utilizza i processi di approvazione globali e aggiungili ai modelli e alle attività modello. Questo consente di risparmiare tempo quando le attività o il progetto futuro dovranno passare attraverso le stesse approvazioni.

  Per informazioni sulla creazione di approvazioni, vedere [Creare un processo di approvazione per gli elementi di lavoro](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Per informazioni sull&#39;associazione di un processo di approvazione a un elemento di lavoro, vedere [Associare un processo di approvazione nuovo o esistente a un lavoro](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

* Decidere quale archivio documenti utilizzare per i progetti futuri. Alcune organizzazioni hanno accesso ai seguenti tipi di archiviazione dei documenti:

   * Storage Workfront legacy
   * Archiviazione cloud Adobe

  L&#39;aggiunta di documenti varia a seconda del tipo di archiviazione scelto. Il tipo di archiviazione scelto per i modelli influirà sul tipo di archiviazione che erediteranno i progetti futuri.

  L’aggiunta di modelli ai progetti esistenti non influisce sul tipo di archiviazione del progetto.

  Per ulteriori informazioni, consulta anche:

   * [Creare un modello di progetto](/help/quicksilver/manage-work/projects/create-and-manage-templates/create-template.md)
   * [Panoramica sulla gestione dei documenti per progetti e oggetti correlati](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md)

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
