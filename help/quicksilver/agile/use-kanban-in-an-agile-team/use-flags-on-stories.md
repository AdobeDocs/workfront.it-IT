---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Utilizzare i flag sulle storie sul Kanban Board
description: Sulla bacheca  [!DNL Kanban] , i flag forniscono un'indicazione visiva di quando una storia è pronta per passare allo stato successivo. Questo consente ai team Kanban di utilizzare un approccio "pull" anziché un approccio "push" per spostare le storie da uno stato all’altro.
author: Courtney
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/zyfrbteuJy-xfPZL75ElkfotVrJWLHF78hDsIwkouko
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 457
ht-degree: 7%

---

# Utilizza i flag sulle storie nella bacheca [!UICONTROL Kanban]

Sulla bacheca [!DNL Kanban], i flag forniscono un&#39;indicazione visiva di quando una storia è pronta per passare allo stato successivo. Questo consente ai team di [!UICONTROL Kanban] di utilizzare un approccio &quot;pull&quot; anziché un approccio &quot;push&quot; per spostare le storie da uno stato all&#39;altro.

**Esempio:** Considera il seguente esempio di team che utilizza un approccio &quot;pull&quot;: Olivia, la designer grafica del team, completa il lavoro e imposta il contrassegno della storia come &quot;[!UICONTROL Pronta per il richiamo]&quot;. Questo flag fornisce un&#39;indicazione visiva a Tony, il copywriter del team, che la storia è pronta per il passaggio allo stato successivo. Tony passa quindi la storia allo stato successivo quando è pronto a iniziare a lavorarci.

Quando si utilizzano i flag sui brani, considera quanto segue:

* I flag non sono uno stato, ma piuttosto un’indicazione visiva del fatto che la storia è pronta per essere spostata nello stato successivo da un altro membro del team.
* I contrassegni non vengono visualizzati nelle schede delle storie presenti nella colonna [!UICONTROL Backlog] o nella colonna [!UICONTROL Complete] (o in qualsiasi colonna in cui lo stato della colonna equivale a [!UICONTROL Complete]).

  Per ulteriori informazioni sugli stati delle storie, vedere [Utilizzare i flag sulle storie sulla bacheca Kanban](#updating-the-status-of-stories-and-subtasks)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Work o successiva</p> </td> 
  </tr>
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Utilizza i flag sulle storie nella bacheca [!UICONTROL Kanban]

Per modificare un contrassegno su una storia:

{{step1-to-team}}

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team di [!UICONTROL Kanban] dal menu a discesa o cerca un team nella barra di ricerca.

1. Vai alla bacheca [!UICONTROL Kanban] in cui desideri modificare un flag su una storia.
1. Espandi il riquadro del brano per visualizzare il contrassegno.
Per impostazione predefinita, il contrassegno è impostato su **[!UICONTROL On Track]** per ogni brano.
   ![Scheda Kanban](assets/agile-storycard-kanban-2021-350x308.png)

1. Fai clic sul flag corrente, quindi seleziona una delle seguenti opzioni di flag:

   * **[!UICONTROL Sul binario]:** Lo stato della storia è appropriato e al momento non è necessario eseguire alcuna azione.

     Questo è il flag predefinito per ogni storia sul Kanban Board.
     ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL È bloccato]:** Impossibile passare allo stato successivo. Quando questo flag viene impostato su una storia, la storia non viene conteggiata nel limite WIP. (Per ulteriori informazioni sui limiti WIP, vedere l&#39;articolo [Configurare Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).)

     ![kanban_flag_locked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Pronto per il richiamo]:** La storia è pronta per essere spostata allo stato successivo da un altro membro del team.

     ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
