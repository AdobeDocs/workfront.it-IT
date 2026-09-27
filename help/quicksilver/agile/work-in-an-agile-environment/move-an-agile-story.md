---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Spostare una storia Agile
description: Puoi spostare una storia Agile in un’iterazione diversa (per i team Scrum) o nel backlog (per i team Kanban e Scrum).
author: Courtney
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/gVEWRh4iiYdy6CwzLubaY3GZ4EE5C5diJ-RvsYFFtE4'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
    internal-label: Agile
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 11%
---
# Spostare una storia Agile

Puoi spostare una storia Agile in un’iterazione diversa (per i team Scrum) o nel backlog (per i team Kanban e Scrum).

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
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td>Gestire l’accesso alla storia</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Spostare una storia da un&#39;iterazione o bacheca Kanban al backlog

1. Passare all&#39;iterazione o bacheca Kanban contenente il brano da spostare nel backlog.
1. Fai clic sull’intestazione dell’iterazione nella parte superiore della pagina.
1. Nella scheda **[!UICONTROL Storie]**, seleziona le storie che desideri spostare.
1. Fai clic su **[!UICONTROL Altro]** > **[!UICONTROL Sposta in]**. Viene visualizzata la finestra di dialogo **[!UICONTROL Sposta in]**.

   ![Finestra di dialogo Sposta storia](assets/iteration-story-move.png)

1. Seleziona il backlog di **team_name**. Nell&#39;esempio precedente, il nome del team è **Marketing**.

1. Fare clic su **[!UICONTROL Sposta]**.

## Spostare una storia in un&#39;iterazione diversa

Se siete un amministratore di sistema o un membro del team a cui è associata l&#39;iterazione, potete spostare una storia in un&#39;iterazione diversa per il team Scrum.

>[!NOTE]
>
> L&#39;opzione **[!UICONTROL Sposta in]** non è disponibile per i brani principali in un&#39;iterazione. È possibile spostare solo le sottoattività in un&#39;altra iterazione.


1. Passare all&#39;iterazione contenente il brano che si desidera spostare.
1. Fai clic sull’intestazione dell’iterazione nella parte superiore della pagina.
1. Nella scheda **[!UICONTROL Storie]**, seleziona le storie che desideri spostare.
1. Fai clic su **[!UICONTROL Altro]** > **[!UICONTROL Sposta in]**. Viene visualizzata la finestra di dialogo **[!UICONTROL Sposta in]**.

   ![Finestra di dialogo Sposta storia](assets/iteration-story-move.png)

1. Selezionare **[!UICONTROL Un&#39;altra iterazione]**.
1. Nel menu a discesa visualizzato, selezionate l&#39;iterazione in cui desiderate spostare il brano.

   >[!NOTE]
   >
   >L&#39;elemento di lavoro [!UICONTROL Data inizio pianificata] e [!UICONTROL Data completamento pianificata] è interessato da un&#39;impostazione nella pagina [!UICONTROL Modifica team]. Per informazioni, vedere la sezione [[!UICONTROL Configurare] come vengono applicate le date quando si aggiungono elementi di lavoro a un&#39;iterazione](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) nell&#39;articolo [Configurare Scrum](../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Fare clic su **[!UICONTROL Sposta]**.
