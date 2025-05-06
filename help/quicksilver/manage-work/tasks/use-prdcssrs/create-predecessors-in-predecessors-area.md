---
product-area: projects
navigation-topic: use-predecessors
title: Creare una relazione predecessore utilizzando l'area Predecessori
description: È possibile utilizzare le attività predecessore (o solo i predecessori) per collegare attività che dipendono da altre attività per iniziare o completare.
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Creare una relazione predecessore utilizzando l&#39;area Predecessori

<!-- Audited: 5/2025 -->

È possibile utilizzare le attività predecessore (o solo i predecessori) per collegare attività che dipendono da altre attività per iniziare o completare. Ad esempio, non si desidera ospitare una parte (attività dipendente) prima di inviare gli inviti (attività predecessore).

Questo articolo mostra come impostare i predecessori utilizzando la scheda Predecessori all’interno di un’attività.

Per informazioni sull&#39;impostazione dei predecessori in un elenco di attività, vedere [Creare una relazione predecessore nell&#39;elenco attività](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

Puoi visualizzare i predecessori delle attività nelle seguenti aree di Adobe Workfront:

* Nella sezione Predecessori delle attività dipendenti
* Nel diagramma di Gantt
* Nell&#39;elenco delle attività nella colonna Predecessori

Per informazioni sui predecessori, vedere [Panoramica sui predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <p>Nuovo: Standard </p>
   <p>Oppure </p>
   <p>Corrente: Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per le attività e il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare un predecessore per un&#39;attività

1. Passare all&#39;attività che si desidera designare come attività dipendente.

1. Nel pannello a sinistra, fai clic su **Predecessori**.

1. Nella sezione **Predecessori**, fai clic su **+Aggiungi predecessore**. Viene visualizzata la finestra di dialogo **Aggiungi predecessore**.

1. (Facoltativo) Per aggiungere un predecessore per più progetti, sostituisci il nome del progetto nel campo **Progetto principale** con un altro progetto.

   Per informazioni, consulta [Creare predecessori per più progetti](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. Nel campo **Attività** digitare il nome dell&#39;attività o delle attività che si desidera designare come predecessori, quindi selezionarle quando vengono visualizzate nel menu a discesa.

1. Selezionare un **tipo di dipendenza**.

   Per informazioni, vedere [Panoramica dei tipi di relazione tra attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Immetti un valore di **Lag**.

   Per informazioni, vedere &#x200B;[Panoramica sui tipi di Lag](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   ![Finestra di dialogo Aggiungi predecessore](assets/add-predecessor-dialog-box.png)

1. Selezionare la casella di controllo **Imposto** se si desidera applicare la relazione predecessore tra le due attività.

   Per informazioni, vedere [Imponi predecessori](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Fai clic su **Salva**.
