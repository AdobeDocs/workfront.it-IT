---
product-area: projects
navigation-topic: use-predecessors
title: Creare una relazione predecessore utilizzando l'area Predecessori
description: È possibile utilizzare le attività predecessori (o solo i predecessori) per collegare le attività che dipendono da altre attività da avviare o completare. Ad esempio, non si desidera ospitare una parte (attività dipendente) prima di inviare gli inviti (attività predecessore).
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Creare una relazione predecessore utilizzando l&#39;area Predecessori

È possibile utilizzare le attività predecessori (o solo i predecessori) per collegare le attività che dipendono da altre attività da avviare o completare. Ad esempio, non si desidera ospitare una parte (attività dipendente) prima di inviare gli inviti (attività predecessore).

Questo articolo mostra come impostare i predecessori utilizzando la scheda Predecessori all&#39;interno di un&#39;attività.

Per informazioni sull&#39;impostazione dei predecessori in un elenco delle attività, vedere [Creare una relazione predecessore nell&#39;elenco delle attività](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

È possibile visualizzare i predecessori delle attività nelle seguenti aree di Adobe Workfront:

* Nella sezione Predecessori delle attività dipendenti
* Nel diagramma di Gantt
* Nell&#39;elenco delle attività della colonna Predecessori

Per informazioni sui predecessori, consulta [Panoramica dei predecessori delle attività](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l’accesso a Attività e Progetti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci le autorizzazioni per le attività e il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare un predecessore per un&#39;attività

1. Passa a un&#39;attività da designare come attività dipendente, quindi fai clic su **Predecessori** nel pannello a sinistra.

   Potrebbe essere necessario fare clic su **Mostra altro**, quindi **Predecessori**.

1. Fai clic su **+Aggiungi predecessore**.
1. (Facoltativo) Per aggiungere un predecessore tra progetti, sostituisci il nome del progetto nel **Progetto padre** campo con un altro progetto, quindi digitare il nome dell&#39;attività o delle attività desiderate come predecessori.

   Per informazioni sull’aggiunta di predecessori tra progetti, consulta [Creare predecessori tra progetti](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. Digitare il nome dell&#39;attività o delle attività da designare come predecessori.

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. Seleziona una **Tipo di dipendenza**.

   Per informazioni sui tipi di dipendenza dell&#39;attività, vedere una [Panoramica dei tipi di dipendenza dell&#39;attività](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Specifica una **Ritardo** in giorni.

   Per informazioni sui tipi di tag, consulta &#x200B; [Panoramica dei tipi di ritardo](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

1. Seleziona **Impiegato** se si desidera applicare la relazione predecessore tra le due attività.

   Per informazioni sull&#39;applicazione dei predecessori, consulta [Applica predecessori](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Fai clic su **Salva**.
