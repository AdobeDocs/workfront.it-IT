---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Gestire storie e problemi sulla scheda Scrum
description: È possibile spostare una storia o un problema dalla bacheca Scrum a un'altra iterazione o al backlog, oppure eliminarla dalla bacheca Scrum. Quando si elimina un brano o un problema, questo viene spostato nel Cestino per 30 giorni e può essere recuperato solo dall'amministratore di sistema.
author: Lisa
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# Gestire storie e problemi relativi [!UICONTROL Scratto] bacheca

È possibile spostare una storia o un problema dal [!UICONTROL Scratto] bacheca a un&#39;altra iterazione o al backlog, o eliminalo dal [!UICONTROL Scratto] consiglio di amministrazione. Quando si elimina un brano o un problema, questo viene spostato nel Cestino per 30 giorni e può essere recuperato solo dall&#39;amministratore di sistema.

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
   <td> <p>[!UICONTROL Work] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o superiore</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>[!UICONTROL Gestisci] accesso all'attività o al problema</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Sposta storia o problema da [!UICONTROL Scratto] bacheca

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.
1. Fai clic sul pulsante **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi seleziona un team Scrum dal menu a discesa o cerca un team nella barra di ricerca.
1. Nel pannello a sinistra, seleziona **[!UICONTROL Iterazioni]** per scegliere un&#39;iterazione specifica o selezionare **[!UICONTROL Iterazione corrente]**.
1. Fai clic sul pulsante **[!UICONTROL Altro]** icona sulla storia o sul problema, e selezionare **[!UICONTROL Sposta a]**.

   ![Elimina o sposta la storia dalla scheda Scrum](assets/scrum-delete-move-story.png)

1. Nel messaggio di conferma, scegli:

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Un'altra iterazione]</strong></td>
        <td>Selezionare per spostare l'elemento in un'altra iterazione, quindi scegliere l'iterazione in cui si sposterà il brano o il problema. Se non sono definite iterazioni future, non è possibile spostare l’elemento.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Backlog]</strong></td>
        <td>Selezionare questa opzione per spostare la storia o il problema nel backlog del team.</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >Elemento di lavoro [!UICONTROL Data di inizio prevista] e [!UICONTROL Data completamento pianificata] sono influenzati da un&#39;impostazione [!UICONTROL Modifica team] pagina. Per informazioni, consulta la sezione . [[!UICONTROL Configura] modalità di applicazione delle date quando si aggiungono elementi di lavoro a un&#39;iterazione](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) nell&#39;articolo [Configura punteggio](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Fai clic su **[!UICONTROL Sposta]**.

## Elimina la storia o il problema dal [!UICONTROL Scratto] bacheca

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.
1. Fai clic sul pulsante **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi seleziona un team Scrum dal menu a discesa o cerca un team nella barra di ricerca.
1. Nel pannello a sinistra, seleziona **[!UICONTROL Iterazioni]** per scegliere un&#39;iterazione specifica o selezionare **[!UICONTROL Iterazione corrente]**.
1. Fai clic sul pulsante **[!UICONTROL Altro]** icona sulla storia o sul problema, e selezionare **[!UICONTROL Elimina storia]** o **[!UICONTROL Elimina problema]**.

   ![Elimina o sposta la storia dalla scheda Scrum](assets/scrum-delete-move-story.png)

1. Nel messaggio di conferma, fai clic su **[!UICONTROL Sì, eliminalo]**.
