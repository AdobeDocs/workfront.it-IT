---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Aggiungere o rimuovere membri da una bacheca
description: Le persone devono essere aggiunte alla bacheca come membri prima che possano visualizzare la bacheca e essere assegnate alle schede.
author: Lisa
feature: Agile
exl-id: 8a46846c-f9b8-45cb-9923-e7596854557b
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Aggiungere o rimuovere membri da una bacheca

Persone e team devono essere aggiunti alla bacheca come membri prima che possano visualizzarla.

Per impostazione predefinita, il proprietario è il creatore di una bacheca. Il proprietario della bacheca è l’unica persona che può eliminarla o aggiornarne i filtri nel pannello Configura. Solo un amministratore di sistema o il proprietario corrente della bacheca può modificare il proprietario della bacheca.

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
   <td> 
   <p>Collaboratore o versione successiva</p> 
   <p>Richiedi o superiore</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungere membri a una bacheca

{{step1-to-boards}}

1. Crea una nuova bacheca o modificane una esistente. Per informazioni, consulta [Creare o modificare una bacheca](../../agile/get-started-with-boards/create-edit-board.md).
1. Fare clic sull&#39;icona **[!UICONTROL Aggiungi membro]** ![Aggiungi membri](assets/boards-addmember-spectrum-25x25.png).
1. Nella casella **[!UICONTROL Aggiungi membri]**, inizia a digitare un nome, quindi selezionalo quando viene visualizzato nell&#39;elenco.

   È possibile selezionare un singolo membro o un team. Se scegli un team, il team stesso viene aggiunto alla bacheca.

   >[!NOTE]
   >
   >Un singolo utente deve avere l&#39;opzione **[!UICONTROL Visualizza]** o **[!UICONTROL Modifica]** impostata nel proprio livello di accesso per i team, altrimenti non potrà visualizzare la bacheca.


   ![Aggiungi membri alla bacheca](assets/boards-add-members.png)

## Rimuovere membri da una bacheca

{{step1-to-boards}}

1. Crea una nuova bacheca o modificane una esistente. Per informazioni, consulta [Creare o modificare una bacheca](../../agile/get-started-with-boards/create-edit-board.md).
1. Fare clic sull&#39;icona **[!UICONTROL Aggiungi membro]** ![Aggiungi membri](assets/boards-addmember-spectrum-25x25.png).
1. Nella casella **[!UICONTROL Aggiungi membri]** fare clic sulla X accanto al nome di una persona o di un team per rimuoverli dalla bacheca.

   ![Rimuovi membro dalla bacheca](assets/boards-remove-member-from-board-350x367.png)

   Quando rimuovi un membro da una bacheca, non viene rimosso dalle schede a cui è assegnato. Per le schede connesse, le assegnazioni vengono aggiornate anche sull&#39;attività o sul problema [!DNL Workfront].

   I membri vengono rimossi solo da questa bacheca. Non vengono rimosse dalle altre bacheche a cui appartengono.

   >[!NOTE]
   >
   >Non puoi rimuovere il proprietario della bacheca.

## Cambia il proprietario della bacheca

>[!NOTE]
>
>Solo un amministratore di sistema o il proprietario corrente della bacheca può modificare il proprietario della bacheca. Una bacheca può avere un solo proprietario.
>
>La possibilità di cambiare il proprietario della bacheca è disponibile su bacheche di base, retrospettive e Kanban, ma non su bacheche dinamiche.

1. Accedi alla bacheca.
1. Fai clic sul menu **[!UICONTROL Altro]** ![Altro menu](assets/more-icon-spectrum.png) accanto al nome della bacheca, quindi scegli **[!UICONTROL Cambia proprietario della bacheca]**.
1. Nella finestra di dialogo Cambia proprietario della bacheca cercare e selezionare l&#39;utente che si desidera impostare come proprietario.

   Non puoi cercare utenti che sono già membri della bacheca. Per rendere proprietario un membro esistente, devi prima rimuoverlo dalla bacheca. Facendo in modo che un utente sia il proprietario della bacheca, lo aggiunge alla bacheca.

   Solo un utente può essere il proprietario della bacheca. Una squadra non può essere un proprietario.

1. Fai clic su [!UICONTROL **Aggiorna**].
