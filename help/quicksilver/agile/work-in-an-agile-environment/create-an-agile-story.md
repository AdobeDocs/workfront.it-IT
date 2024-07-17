---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Creare una storia agile
description: Potete creare una storia agile su un'iterazione in vari modi. Dopo aver creato una storia agile, potete aggiungere sottoattività alla storia.
author: Lisa
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 0%

---

# Creare una storia agile

Potete creare una storia agile su un&#39;iterazione in vari modi. Dopo aver creato una storia agile, potete aggiungere sottoattività alla storia.

Quando aggiungi una storia o un&#39;attività secondaria in un&#39;iterazione, il Tipo di durata è impostato su [!UICONTROL Semplice] e il Vincolo attività è impostato su Date fisse, con le date bloccate all&#39;interno dell&#39;iterazione. Non è possibile modificare il Tipo di durata o il Vincolo attività in un&#39;iterazione. Inoltre, la durata dell&#39;attività deve essere maggiore di 0 minuti.

Per informazioni su come gestire il brano dopo che è stato aggiunto all&#39;iterazione, vedere [Iterazioni](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td> <p>[!UICONTROL Worker] o versione successiva</p> <p>Nota: se non disponi ancora dell'accesso, chiedi all'amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Accesso [!UICONTROL Gestisci] al progetto in cui si trova il brano</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## Creare una storia agile in un’iterazione

1. Passare all&#39;iterazione agile in cui si desidera creare la storia:

   1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.

   1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.

   1. Nel pannello a sinistra, seleziona **[!UICONTROL Iterazioni]** per scegliere un&#39;iterazione specifica oppure seleziona **[!UICONTROL Iterazione corrente]**.
   1. Fare clic sul nome dell&#39;iterazione specifica in cui si desidera creare un brano.

   ![Aggiungi nuova storia all&#39;iterazione](assets/iteration-add-story.png)

1. Fai clic su **[!UICONTROL Nuova storia].**
1. Specifica le seguenti informazioni:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nome brano]</strong></td>
      <td>Digitate un nome per il brano.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Descrizione]</strong></td>
      <td>Digitate una descrizione per il brano.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Pronto]</strong></td>
      <td>Selezionate questa opzione se il brano è pronto per essere aggiunto a un'iterazione. Quando questa opzione è selezionata, indica agli utenti quali brani nel backlog sono pronti per essere aggiunti a un’iterazione.<br>È possibile aggiungere una storia a un'iterazione indipendentemente dal fatto che sia contrassegnata o meno <strong>[!UICONTROL Ready].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Stima] (punti)</strong></td>
      <td>Specificate la stima per il brano. Se il team agile è configurato per stimare le storie in punti, per impostazione predefinita 1 punto equivale a 8 ore. Le stime vengono aggiunte come [!UICONTROL Lavoro Necessario] alla storia.<br>Ad esempio, se si stima una storia come 3 punti, il comportamento predefinito consiste nell'aggiungere 24 [!UICONTROL Planned Hours] alla storia.<br>Se un brano contiene sottoattività, tenere presente che le stime combinate di tutte le sottoattività determinano la stima del brano principale. Per ulteriori informazioni, vedere <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">Aggiungere brani a un'iterazione esistente</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Progetto padre [!UICONTROL]</strong></td>
      <td>Inizia a digitare il nome del progetto a cui sarà associata questa storia.<br>Per impostazione predefinita, il colore del brano viene visualizzato con lo stesso colore degli altri brani di questo progetto.<br>Lo stato del progetto deve essere impostato su [!UICONTROL Current]. Se lo stato del progetto è diverso da [!UICONTROL Current], non viene visualizzato nel menu a discesa.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Attività Padre]</strong></td>
      <td>Dopo aver scelto un progetto padre, è possibile scegliere un'attività padre. Quando si seleziona un'attività padre, il brano viene creato come sottoattività dell'attività padre nel progetto selezionato.<br>Iniziare a digitare il nome dell'attività padre per il brano, quindi fare clic su di esso quando viene visualizzato nell'elenco a discesa.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>Seleziona i moduli personalizzati da aggiungere alla storia.</td>
     </tr>
    </tbody>
   </table>

1. Fai clic su **[!UICONTROL Salva storia]**.

## Creare una storia agile nel backlog

Puoi creare una storia agile dal backlog agile, come descritto nella sezione [Creare nuove storie nel backlog](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) nell&#39;articolo [[!UICONTROL Gestire] il backlog agile](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Aggiungere un’attività o un problema come storia agile

È possibile aggiungere un’attività o un problema esistente come storia a un’iterazione. Per ulteriori informazioni, consulta [Aggiungere brani a un&#39;iterazione esistente](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) o [Aggiungere brani e problemi dalla bacheca [!UICONTROL Scrum]](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Creare sottoattività in una storia agile

È possibile creare un&#39;attività secondaria in un brano agile utilizzando uno dei metodi seguenti:

* Utilizzando la scheda **[!UICONTROL Sottoattività]**, come descritto in [Crea sottoattività](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) in [Crea sottoattività](../../manage-work/tasks/create-tasks/create-subtasks.md).

* Direttamente dallo storyboard, come descritto in [Creare un&#39;iterazione](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
