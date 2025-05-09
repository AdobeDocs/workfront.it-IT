---
product-area: projects
navigation-topic: use-predecessors
title: Imponi predecessori
description: I predecessori sono attività da cui dipendono altre attività per il completamento. Le relazioni con i predecessori influiscono sulle date di inizio e di completamento delle attività e in ultima analisi sulla sequenza temporale del progetto.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Imponi predecessori

<!-- Audited: 2/2024 -->

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

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
      <p>Nuovo: Standard</p> 
      <p>OPPURE</p>
      <p>Corrente: Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td><p>Gestire le autorizzazioni per le attività e il progetto</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

   ![predecor_enforced_in_list.png](assets/predecessor-enforced-in-list-350x308.png)
