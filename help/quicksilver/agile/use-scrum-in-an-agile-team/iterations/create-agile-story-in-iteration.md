---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Creare una storia agile in un'iterazione
description: Questo articolo descrive come creare una nuova storia agile quando sei già nell'iterazione.
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# Creare una storia agile in un&#39;iterazione

Questo articolo descrive come creare una nuova storia agile quando sei già nell&#39;iterazione. Per informazioni sulla creazione di una storia agile da un&#39;attività, un problema o un&#39;altra area di [!DNL Adobe Workfront], vedi [Aggiungere storie a un&#39;iterazione esistente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

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
   <td> <p>[!UICONTROL Work] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o superiore</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Accesso a [!UICONTROL Gestire] il progetto su cui si trova la storia</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Creare una storia agile in un&#39;iterazione

1. Vai all&#39;iterazione agile in cui desideri creare la storia:

   1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe] Workfront, quindi fai clic su **[!UICONTROL Team]**.

   1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.

   1. Nel pannello a sinistra, seleziona **[!UICONTROL Iterazioni]**.
   1. Fare clic sul nome dell&#39;iterazione specifica in cui si desidera creare un brano.
   1. Nel pannello a sinistra, seleziona **[!UICONTROL Storie]**.

1.  Fai clic su **[!UICONTROL Nuova storia].**
1. Specifica le seguenti informazioni:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nome Story]</strong></td>
      <td>Digitate un nome per la storia.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Descrizione]</strong></td>
      <td>Digita una descrizione della storia.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td>Seleziona questa opzione se il brano è pronto per essere aggiunto a un’iterazione. Quando questa opzione è selezionata, indica agli utenti quali storie nel backlog sono pronte per essere aggiunte a un'iterazione.<br>Un brano può essere aggiunto a un'iterazione indipendentemente dal fatto che sia contrassegnato o meno <strong>[!UICONTROL Ready].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Stima [!UICONTROL] (punti)</strong></td>
      <td>Specifica la stima per la storia. Se il team agile è configurato per stimare le storie in punti, per impostazione predefinita 1 punto è uguale a 8 ore. Le stime vengono aggiunte come [!UICONTROL Pianifica ore] sulla storia.<br>Ad esempio, se stimate una storia come 3 punti, il comportamento predefinito consiste nell’aggiungere 24 ore pianificate alla storia.<br>Se un brano contiene sottoattività, ricordare che le stime combinate per tutte le sottoattività determinano la stima del brano padre. Per ulteriori informazioni, consulta <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">Aggiungi una sottoattività a una storia esistente sulla scheda [!UICONTROL Scrum]</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Progetto padre]</strong></td>
      <td>Inizia a digitare il nome del progetto a cui verrà associato il brano.<br>Per impostazione predefinita, il colore della storia viene visualizzato con lo stesso colore degli altri brani di questo progetto.<br>Lo stato del progetto deve essere impostato su [!UICONTROL Current]. Se lo stato del progetto è diverso da [!UICONTROL Current], non viene visualizzato nel menu a discesa.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Attività padre]</strong></td>
      <td>Dopo aver scelto un progetto padre, è possibile scegliere un'attività padre. Quando si seleziona un'attività padre, il brano viene creato come sottoattività dell'attività padre sul progetto selezionato.<br>Inizia a digitare il nome dell'attività principale per il brano, quindi fai clic su di esso quando viene visualizzato nell'elenco a discesa.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>Seleziona i moduli personalizzati da aggiungere al brano.</td>
     </tr>
    </tbody>
   </table>

1. Fai clic su **[!UICONTROL Salva storia]**.
