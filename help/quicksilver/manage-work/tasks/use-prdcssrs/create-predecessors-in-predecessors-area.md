---
product-area: projects
navigation-topic: use-predecessors
title: Creare una relazione predecessore utilizzando l'area Predecessori
description: È possibile utilizzare le attività predecessore (o solo i predecessori) per collegare attività che dipendono da altre attività per iniziare o completare. Ad esempio, non si desidera ospitare una parte (attività dipendente) prima di inviare gli inviti (attività predecessore).
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: d5f4e83badd4d011816551f06b056ffe886d3b17
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Creare una relazione predecessore utilizzando l&#39;area Predecessori

È possibile utilizzare le attività predecessore (o solo i predecessori) per collegare attività che dipendono da altre attività per iniziare o completare. Ad esempio, non si desidera ospitare una parte (attività dipendente) prima di inviare gli inviti (attività predecessore).

Questo articolo mostra come impostare i predecessori utilizzando la scheda Predecessori all’interno di un’attività.

Per informazioni sull&#39;impostazione dei predecessori in un elenco di attività, vedere [Creare una relazione predecessore nell&#39;elenco delle attività](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

Puoi visualizzare i predecessori delle attività nelle seguenti aree di Adobe Workfront:

* Nella sezione Predecessori delle attività dipendenti
* Nel diagramma di Gantt
* Nell&#39;elenco delle attività nella colonna Predecessori

Per informazioni sui predecessori, vedere [Panoramica dei predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per le attività e il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Creare un predecessore per un&#39;attività

1. Passare a un&#39;attività da designare come attività dipendente, quindi fare clic su **Predecessori** nel pannello a sinistra.

   Potrebbe essere necessario fare clic su **Mostra altro**, quindi **Predecessori**.

1. Clic **+Aggiungi predecessore**.
1. (Facoltativo) Per aggiungere un predecessore per più progetti, sostituisci il nome del progetto in **Progetto principale** in un altro progetto, quindi digitare il nome dell&#39;attività o delle attività che si desidera come predecessori.

   Per informazioni sull’aggiunta di predecessori per più progetti, consulta [Creare predecessori per più progetti](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. Digitare il nome dell&#39;attività o delle attività da designare come predecessori.

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. Seleziona un **Tipo di dipendenza**.

   Per informazioni sui tipi di relazione tra attività, vedere [Panoramica dei tipi di relazione tra attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Specifica un **Lag** importo in giorni.

   Per informazioni sui tipi di Lag, vedi &#x200B; [Panoramica sui tipi di ritardo](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

1. Seleziona **Enforced** se si desidera applicare la relazione predecessore tra le due attività.

   Per informazioni sull&#39;applicazione dei predecessori, vedere [Imponi predecessori](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Fai clic su **Salva**.
