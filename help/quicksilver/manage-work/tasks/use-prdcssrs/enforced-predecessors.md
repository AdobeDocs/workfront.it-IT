---
product-area: projects
navigation-topic: use-predecessors
title: Imponi predecessori
description: I predecessori sono attività da cui dipendono altre attività per il completamento. Le relazioni con i predecessori influiscono sulle date di inizio e di completamento delle attività e in ultima analisi sulla sequenza temporale del progetto.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: 4897f165a7316a52b968601b45f95f7045f63840
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# Imponi predecessori

<!-- Audited: 11/2025 -->

I predecessori sono attività da cui dipendono altre attività per il completamento. Le relazioni con i predecessori influiscono sulle date di inizio e di completamento delle attività e in ultima analisi sulla sequenza temporale del progetto.

Per informazioni sui predecessori, vedere [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Se si impostano relazioni di predecessori tra attività, si definisce in che modo l&#39;inizio o la fine di un&#39;attività dipendente dipende dall&#39;inizio o dalla fine delle attività predecessori. Questa operazione viene eseguita utilizzando tipi di dipendenza diversi.

Per informazioni sui tipi di dipendenza, vedere [Panoramica sui tipi di relazione tra attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Panoramica dei predecessori forzati

>[!IMPORTANT]
>
>È necessario imporre ai predecessori di richiedere il rispetto delle relazioni con i predecessori. Senza applicare i predecessori, le attività dipendenti possono iniziare e finire indipendentemente dall&#39;inizio e dalla fine dei predecessori, indipendentemente dai tipi di dipendenza.

Puoi applicare la relazione di predecessore quando imposti predecessori su un progetto.

Se viene applicato un predecessore, l&#39;attività successore non può iniziare prima del completamento del predecessore. Ad esempio, se si applica una relazione Fine-Inizio tra l&#39;Attività A e l&#39;Attività B, l&#39;Attività B non può iniziare (lo Stato deve rimanere Nuovo e la Percentuale di completamento deve rimanere 0%) finché l&#39;Attività A non viene contrassegnata come completata. L’applicazione delle relazioni si applica a tutti i tipi di predecessori.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Standard</p> 
   <p>Piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per le attività e il progetto</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
      <p>New: Standard</p> 
      <p>OR</p>
      <p>Current: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td><p>Manage permissions to the tasks and the project</p></td> 
  </tr> 
 </tbody> 
</table>-->

## Imponi un predecessore a livello di attività

1. Passare all&#39;attività successore di cui si desidera applicare il predecessore.
1. Fai clic su **Predecessori** nel pannello a sinistra, quindi fai clic su **Aggiungi predecessore**.
1. (Condizionale) Se desideri aggiungere un predecessore per più progetti, rimuovi il nome del progetto nel campo **Progetto principale** e sostituiscilo con un altro progetto.
1. Specifica il nome dell&#39;attività predecessore o delle attività nel campo **Attività**.
1. Specificare il **Tipo di dipendenza** tra queste due attività.

   Il tipo di dipendenza **predefinito** è **Fine-Inizio**.

1. Seleziona il campo **Imposto** per applicare il predecessore.
1. Fai clic su **Salva**.

## Imporre un predecessore in un elenco di attività

1. Consente di passare a un elenco di attività in un progetto.
1. Dal menu a discesa **Visualizza**, selezionare la **Visualizzazione standard**.

1. Prendi nota del numero di attività che intendi designare come predecessore.
1. Individuare l&#39;attività successore di cui si desidera applicare il predecessore.
1. Nella colonna **Predecessori**, inizia a immettere il numero dell&#39;attività predecessore seguito da &quot;e&quot;. Digitare ad esempio &quot;1e&quot; per aggiungere l&#39;attività numero 1 come predecessore dell&#39;attività selezionata.
1. Fare clic su Invio per salvare le informazioni sul predecessore per l&#39;attività.

   ![Elenco dei predecessori applicati](assets/predecessor-enforced-in-list-350x308.png)

   Le informazioni sul predecessore che viene applicato vengono salvate immediatamente.
