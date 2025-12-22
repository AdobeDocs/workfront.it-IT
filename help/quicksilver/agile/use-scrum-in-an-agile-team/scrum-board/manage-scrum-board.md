---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: Gestione di storie e problemi sulla bacheca Scrum
description: Puoi spostare una storia o un problema dalla bacheca Scrum a un’altra iterazione o nel backlog, oppure eliminarlo dalla bacheca Scrum. Quando elimini una storia o un problema, questa viene spostata nel Cestino per 30 giorni e può essere ripristinata solo dall'amministratore di sistema.
author: Jenny
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 3%

---

# Gestisci storie e problemi sulla bacheca [!UICONTROL Scrum]

È possibile spostare una storia o un problema dalla bacheca [!UICONTROL Scrum] a un&#39;altra iterazione o nel backlog oppure eliminarlo dalla bacheca [!UICONTROL Scrum]. Quando elimini una storia o un problema, questa viene spostata nel Cestino per 30 giorni e può essere ripristinata solo dall&#39;amministratore di sistema.

Per rimuovere un’attività o un problema dall’iterazione senza eliminarlo o inviarlo al backlog, vai al progetto e rimuovi il team Agile dalla colonna delle assegnazioni. In questo modo l’attività o il problema viene rimosso dalla bacheca Scrum, ma rimane nel progetto.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Accesso [!UICONTROL Gestisci] all'attività o al problema </td> 
  </tr>
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Sposta una storia o un problema dalla bacheca [!UICONTROL Scrum]

{{step1-to-team}}

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

## Elimina una storia o un problema dalla bacheca [!UICONTROL Scrum]

{{step1-to-team}}

1. Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team](assets/switch-team-icon.png), quindi seleziona un team Scrum dal menu a discesa o cerca un team nella barra di ricerca.
1. Nel pannello a sinistra, seleziona **[!UICONTROL Iterazioni]** per scegliere un&#39;iterazione specifica oppure seleziona **[!UICONTROL Iterazione corrente]**.
1. Fai clic sull&#39;icona **[!UICONTROL Altro]** sulla storia o sul problema e seleziona **[!UICONTROL Elimina storia]** o **[!UICONTROL Elimina problema]**.

   ![Elimina o sposta la storia dalla bacheca Scrum](assets/scrum-delete-move-story.png)

1. Nel messaggio di conferma, fare clic su **[!UICONTROL Sì, eliminarlo]**.
