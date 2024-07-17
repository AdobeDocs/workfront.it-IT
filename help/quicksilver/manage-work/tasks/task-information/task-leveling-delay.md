---
product-area: projects
navigation-topic: task-information
title: Ritardo livellamento attività di aggiornamento
description: Talvolta possono verificarsi conflitti tra le pianificazioni delle attività di un progetto. È possibile livellare le risorse o risolvere i conflitti tra risorse riprogrammando le risorse e le attività in modo che tutte le attività possano essere completate entro una pianificazione realistica. Per informazioni sul livellamento delle attività, vedere Livellare le risorse nel Diagramma di Gantt.
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 3%

---

# Ritardo livellamento attività di aggiornamento

Talvolta possono verificarsi conflitti tra le pianificazioni delle attività di un progetto. È possibile livellare le risorse o risolvere i conflitti tra risorse riprogrammando le risorse e le attività in modo che tutte le attività possano essere completate entro una pianificazione realistica. Per informazioni sul livellamento delle attività, vedere [Livellare le risorse nel Diagramma di Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

Il project manager o l&#39;assegnatario dell&#39;attività può inoltre aggiungere un ritardo di livellamento alle singole attività per tenere conto di eventuali conflitti di risorse o di programmazione. In altre parole, un’attività potrebbe essere pianificata con un ritardo per garantire che, quando Adobe Workfront livella le attività, una pianificazione più realistica superi i conflitti di risorse.

Se si aggiunge un ritardo di livellamento a un&#39;attività, la data di completamento prevista dell&#39;attività viene modificata. Per informazioni sulla data di completamento prevista, vedere [Panoramica della data di completamento prevista per progetti, attività e problemi](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

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
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per le attività </p> <p>Autorizzazioni Contribute o superiori per i progetti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Aggiungere un ritardo di livellamento a un&#39;attività

1. Passare a un&#39;attività per la quale si desidera aggiungere un ritardo di livellamento.
1. Fai clic sull&#39;icona **Altro** a destra del nome dell&#39;attività, quindi fai clic su **Modifica**.

1. Fare clic su **Impostazioni**.

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. Specifica il **ritardo livellamento**, in ore, quindi scegli un&#39;unità di tempo.\
   Tempo di ritardo della risorsa per l&#39;avvio dell&#39;attività a causa di conflitti di risorse.

   Selezionare una delle seguenti opzioni per le unità di tempo:

   * Minuti
   * Ore. Questa è l&#39;impostazione predefinita.
   * Giorni
   * Settimane
   * Mesi
   * Minuti trascorsi
   * Ore trascorse
   * Giorni trascorsi
   * Settimane trascorse
   * Mesi trascorsi

   >[!TIP]
   >
   >Il tempo trascorso è un&#39;unità di tempo per la durata di un&#39;attività. Si tratta del tempo che intercorre tra la Data inizio pianificata e la Data completamento pianificata di un&#39;attività e che include ferie, fine settimana e ferie. In altre parole, il tempo trascorso è il trascorrere dei giorni di calendario.

1. Fai clic su **Salva**. 

 
