---
product-area: projects
navigation-topic: task-information
title: Ritardo livellamento attività di aggiornamento
description: Talvolta possono verificarsi conflitti tra le pianificazioni delle attività di un progetto. È possibile livellare le risorse o risolvere i conflitti tra risorse riprogrammando le risorse e le attività in modo che tutte le attività possano essere completate entro una pianificazione realistica. Per informazioni sul livellamento delle attività, vedere Livellare le risorse nel Diagramma di Gantt.
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 3%

---

# Ritardo livellamento attività di aggiornamento

Talvolta possono verificarsi conflitti tra le pianificazioni delle attività di un progetto. È possibile livellare le risorse o risolvere i conflitti tra risorse riprogrammando le risorse e le attività in modo che tutte le attività possano essere completate entro una pianificazione realistica. Per informazioni sul livellamento delle attività, vedere [Livellare le risorse nel Diagramma di Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

Il project manager o l&#39;assegnatario dell&#39;attività può inoltre aggiungere un ritardo di livellamento alle singole attività per tenere conto di eventuali conflitti di risorse o di programmazione. In altre parole, un’attività potrebbe essere pianificata con un ritardo per garantire che, quando Adobe Workfront livella le attività, una pianificazione più realistica superi i conflitti di risorse.

Se si aggiunge un ritardo di livellamento a un&#39;attività, la data di completamento prevista dell&#39;attività viene modificata. Per informazioni sulla data di completamento prevista, vedere [Panoramica della data di completamento prevista per progetti, attività e problemi](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

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
   <td> <p>Standard</p>
   <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ad attività e progetti</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per le attività </p> <p>Autorizzazioni Contribute o superiori per i progetti</p> </td> 
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
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to Tasks </p> <p>Contribute or higher permissions to Projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Aggiungere un ritardo di livellamento a un&#39;attività

1. Passare a un&#39;attività per la quale si desidera aggiungere un ritardo di livellamento.
1. Fai clic sull&#39;icona **Altro** a destra del nome dell&#39;attività, quindi fai clic su **Modifica**.

1. Fare clic su **Impostazioni**.

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. Specifica il **ritardo livellamento**, in ore, quindi scegli un&#39;unità di tempo.\
   Tempo di ritardo della risorsa per l&#39;avvio dell&#39;attività a causa di conflitti di risorse.

   Selezionare una delle seguenti opzioni per le unità di tempo:

   * Minutes
   * Ore. Questa è l&#39;impostazione predefinita.
   * Days
   * Weeks
   * Months
   * Minuti trascorsi
   * Ore trascorse
   * Giorni trascorsi
   * Settimane trascorse
   * Mesi trascorsi

   >[!TIP]
   >
   >Il tempo trascorso è un&#39;unità di tempo per la durata di un&#39;attività. Si tratta del tempo che intercorre tra la Data inizio pianificata e la Data completamento pianificata di un&#39;attività e che include ferie, fine settimana e ferie. In altre parole, il tempo trascorso è il trascorrere dei giorni di calendario.

1. Fai clic su **Salva**. 

 
