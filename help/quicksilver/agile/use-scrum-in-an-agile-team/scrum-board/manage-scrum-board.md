---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Gestione di storie e problemi sulla bacheca Scrum
description: Puoi spostare una storia o un problema dalla bacheca Scrum a un’altra iterazione o nel backlog, oppure eliminarlo dalla bacheca Scrum. Quando elimini una storia o un problema, questa viene spostata nel Cestino per 30 giorni e può essere ripristinata solo dall'amministratore di sistema.
author: Lisa
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Gestisci storie e problemi sulla bacheca [!UICONTROL Scrum]

È possibile spostare una storia o un problema dalla bacheca [!UICONTROL Scrum] a un&#39;altra iterazione o nel backlog oppure eliminarlo dalla bacheca [!UICONTROL Scrum]. Quando elimini una storia o un problema, questa viene spostata nel Cestino per 30 giorni e può essere ripristinata solo dall&#39;amministratore di sistema.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Work] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o versione successiva</p> <p>Nota: se non disponi ancora dell'accesso, chiedi all'amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Accesso [!UICONTROL Gestisci] all'attività o al problema</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## Sposta storia o problema dalla bacheca [!UICONTROL Scrum]

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.
1. Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team](assets/switch-team-icon.png), quindi seleziona un team Scrum dal menu a discesa o cerca un team nella barra di ricerca.
1. Nel pannello a sinistra, seleziona **[!UICONTROL Iterazioni]** per scegliere un&#39;iterazione specifica oppure seleziona **[!UICONTROL Iterazione corrente]**.
1. Fai clic sull&#39;icona **[!UICONTROL Altro]** sulla storia o sul problema e seleziona **[!UICONTROL Sposta in]**.

   ![Elimina o sposta la storia dalla bacheca Scrum](assets/scrum-delete-move-story.png)

1. Nel messaggio di conferma, scegli:

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Another iteration]</strong></td>
        <td>Seleziona questa opzione per spostare l’elemento in un’altra iterazione, quindi scegli l’iterazione in cui verrà spostato il brano o il problema. Se non sono definite iterazioni future, non è possibile spostare l'elemento.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Backlog]</strong></td>
        <td>Seleziona questa opzione per spostare la storia o il problema nel backlog del team.</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >L&#39;elemento di lavoro [!UICONTROL Data inizio pianificata] e [!UICONTROL Data completamento pianificata] è interessato da un&#39;impostazione nella pagina [!UICONTROL Modifica team]. Per informazioni, vedere la sezione [[!UICONTROL Configurare] come vengono applicate le date quando si aggiungono elementi di lavoro a un&#39;iterazione](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) nell&#39;articolo [Configurare Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Fare clic su **[!UICONTROL Sposta]**.

## Elimina storia o problema dalla bacheca [!UICONTROL Scrum]

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.
1. Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team](assets/switch-team-icon.png), quindi seleziona un team Scrum dal menu a discesa o cerca un team nella barra di ricerca.
1. Nel pannello a sinistra, seleziona **[!UICONTROL Iterazioni]** per scegliere un&#39;iterazione specifica oppure seleziona **[!UICONTROL Iterazione corrente]**.
1. Fai clic sull&#39;icona **[!UICONTROL Altro]** sulla storia o sul problema e seleziona **[!UICONTROL Elimina storia]** o **[!UICONTROL Elimina problema]**.

   ![Elimina o sposta la storia dalla bacheca Scrum](assets/scrum-delete-move-story.png)

1. Nel messaggio di conferma, fare clic su **[!UICONTROL Sì, eliminarlo]**.
