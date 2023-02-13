---
product-area: projects
navigation-topic: task-information
title: Aggiorna ritardo livellamento attività
description: In alcuni casi, potrebbero verificarsi conflitti tra le pianificazioni delle attività di un progetto. È possibile livellare le risorse o risolvere i conflitti tra risorse ripianificando le risorse e le attività in modo che tutte le attività possano essere completate entro una pianificazione realistica. Per informazioni sul livellamento delle attività, vedere Risorse di livello nel Diagramma di Gantt .
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 3%

---

# Aggiorna ritardo livellamento attività

In alcuni casi, potrebbero verificarsi conflitti tra le pianificazioni delle attività di un progetto. È possibile livellare le risorse o risolvere i conflitti tra risorse ripianificando le risorse e le attività in modo che tutte le attività possano essere completate entro una pianificazione realistica. Per informazioni sulle attività di livellamento, vedi [Risorse di livello nel diagramma di Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

In qualità di project manager o di assegnatario dell&#39;attività, è inoltre possibile aggiungere un ritardo di livellamento per le singole attività per tenere conto di eventuali conflitti di risorse o di pianificazione. In altre parole, un&#39;attività potrebbe essere pianificata con un ritardo per garantire che, quando Adobe Workfront livella le attività, una pianificazione più realistica superi i conflitti di risorse.

L&#39;aggiunta di un ritardo di livellamento a un&#39;attività regola la data di completamento prevista dell&#39;attività. Per informazioni sulla data di completamento prevista, vedere [Panoramica della data di completamento prevista per progetti, attività e problemi](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

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
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l’accesso a Attività e Progetti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestione delle autorizzazioni per le attività </p> <p>Autorizzazioni di Contribute o superiori per i progetti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Aggiungere un ritardo di livellamento a un&#39;attività

1. Passare a un&#39;attività per la quale si desidera aggiungere un ritardo di livellamento.
1. Fai clic sul pulsante **Icona Altro** a destra del nome dell&#39;attività, quindi fai clic su **Modifica**.

   ![](assets/qs-task-edit-icon-highlighted-350x154.png)

1. Fai clic su **Impostazioni**.

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. Specifica la **Ritardo di livellamento**, in ore, quindi scegli un’unità di tempo.\
   È il momento in cui la risorsa verrà ritardata all’avvio dell’attività a causa di conflitti tra risorse.

   Selezionare tra le seguenti opzioni per unità di tempo:

   * Minuti
   * Ore. Questa è l’impostazione predefinita.
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
   >Il tempo trascorso è un&#39;unità di tempo per la durata di un&#39;attività. È l&#39;intervallo tra la data di inizio pianificata e la data di completamento pianificata di un&#39;attività che include le festività, i fine settimana e l&#39;ora di inattività. In altre parole, il tempo trascorso è il passaggio dei giorni di calendario.

1. Fai clic su **Salva**. 

 
