---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Manage Stories and Issues on the Scrum Board
description: You can move a story or issue from the Scrum board to another iteration or to the backlog, or delete it from the Scrum board. When you delete a story or issue, it is moved to the Recycle Bin for 30 days and can be recovered only by the system administrator.
author: Courtney
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 10%

---

# Manage stories and issues on the [!UICONTROL Scrum] board

You can move a story or issue from the [!UICONTROL Scrum] board to another iteration or to the backlog, or delete it from the [!UICONTROL Scrum] board. Quando elimini una storia o un problema, questa viene spostata nel Cestino per 30 giorni e può essere ripristinata solo dall&#39;amministratore di sistema.

To remove a task or issue from the iteration without deleting it or sending it to the backlog, go to the project and remove the Agile team from the assignment column. This removes the task or issue from the Scrum board, but it remains on the project.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

Per eseguire i passaggi descritti in questo articolo, devi disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> <p>Nuovo: [!UICONTROL Standard]</p> 
   oppure
   <p>Corrente: [!UICONTROL Work] o versione successiva</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td>[!UICONTROL Manage] access to the task or issue </td> 
  </tr>
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Move a story or issue from the [!UICONTROL Scrum] board

{{step1-to-team}}

1. Click the **[!UICONTROL Switch team]** icon ![Switch team icon](assets/switch-team-icon.png), then either select a Scrum team from the drop-down menu or search for a team in the search bar.
1. Nel pannello a sinistra, seleziona **[!UICONTROL Iterazioni]** per scegliere un&#39;iterazione specifica oppure seleziona **[!UICONTROL Iterazione corrente]**.
1. Click the **[!UICONTROL More]** icon on the story or issue, and select **[!UICONTROL Move to]**.

   ![Delete or move story from Scrum board](assets/scrum-delete-move-story.png)

1. On the confirmation message, choose either:

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Another iteration]</strong></td>
        <td>Seleziona questa opzione per spostare l’elemento in un’altra iterazione, quindi scegli l’iterazione in cui verrà spostato il brano o il problema. Se non sono definite iterazioni future, non è possibile spostare l'elemento.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Backlog]</strong></td>
        <td>Select to move the story or issue to the team's backlog.</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >The work item [!UICONTROL Planned Start Date] and [!UICONTROL Planned Completion Date] are affected by a setting on the [!UICONTROL Edit Team] page. For information, see the section [[!UICONTROL Configure] how dates are applied when adding work items to an iteration](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) in the article [Configure Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Fare clic su **[!UICONTROL Sposta]**.

## Delete a story or issue from the [!UICONTROL Scrum] board

{{step1-to-team}}

1. Click the **[!UICONTROL Switch team]** icon ![Switch team icon](assets/switch-team-icon.png), then either select a Scrum team from the drop-down menu or search for a team in the search bar.
1. Nel pannello a sinistra, seleziona **[!UICONTROL Iterazioni]** per scegliere un&#39;iterazione specifica oppure seleziona **[!UICONTROL Iterazione corrente]**.
1. Click the **[!UICONTROL More]** icon on the story or issue, and select **[!UICONTROL Delete Story]** or **[!UICONTROL Delete Issue]**.

   ![Elimina o sposta la storia dalla bacheca Scrum](assets/scrum-delete-move-story.png)

1. Nel messaggio di conferma, fare clic su **[!UICONTROL Sì, eliminarlo]**.
