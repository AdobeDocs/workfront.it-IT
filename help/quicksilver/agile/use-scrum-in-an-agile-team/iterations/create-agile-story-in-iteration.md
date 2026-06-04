---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Creare una storia Agile in un’iterazione
description: Questo articolo descrive come creare una nuova storia Agile quando si è già nell’iterazione.
author: Courtney
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/-6cBWltTBk0t64BiNadClfh-y9a0Qj2eee2BSUb11OI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 503
ht-degree: 11%

---

# Creare una storia Agile in un’iterazione

Questo articolo descrive come creare una nuova storia Agile quando si è già nell’iterazione. Per informazioni sulla creazione di una storia Agile da un&#39;attività, un problema o un&#39;altra area di [!DNL Adobe Workfront], consulta [Aggiungere storie a un&#39;iterazione esistente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
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
   <td>Gestire l'accesso al progetto a cui appartiene il brano </td> 
  </tr>
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare una storia Agile in un’iterazione

1. Passa all’iterazione Agile in cui desideri creare il brano:

   {{step1-to-team}}

   1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.

   1. Nel pannello a sinistra, seleziona **[!UICONTROL Iterazioni]**.
   1. Fare clic sul nome dell&#39;iterazione specifica in cui si desidera creare un brano.
   1. Nel pannello a sinistra, seleziona **[!UICONTROL Storie]**.

1.  Fai clic su **[!UICONTROL Nuova storia]**.
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
      <td>Selezionate questa opzione se il brano è pronto per essere aggiunto a un'iterazione. Quando questa opzione è selezionata, indica agli utenti quali brani nel backlog sono pronti per essere aggiunti a un'iterazione.<br>È possibile aggiungere un brano a un'iterazione indipendentemente dal fatto che sia contrassegnato <strong>[!UICONTROL Ready].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Stima] (punti)</strong></td>
      <td>Specificate la stima per il brano. Se il team agile è configurato per stimare le storie in punti, per impostazione predefinita 1 punto equivale a 8 ore. Le stime vengono aggiunte come [!UICONTROL Lavoro Necessario] alla storia.<br>Ad esempio, se si stima una storia in 3 punti, il comportamento predefinito consiste nell'aggiungere 24 ore pianificate alla storia.<br>Se un brano contiene sottoattività, tenere presente che le stime combinate di tutte le sottoattività determinano la stima del brano principale. Per ulteriori informazioni, vedere <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">Aggiungere un'attività secondaria a un brano esistente nella bacheca [!UICONTROL Scrum]</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Progetto padre </strong></td>
      <td>Inizia a digitare il nome del progetto a cui sarà associata questa storia.<br>Per impostazione predefinita, il colore del brano viene visualizzato con lo stesso colore degli altri brani di questo progetto.<br>Lo stato del progetto deve essere impostato su [!UICONTROL Current]. Se lo stato del progetto è diverso da [!UICONTROL Current], non viene visualizzato nel menu a discesa.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Attività padre]</strong></td>
      <td>Dopo aver scelto un progetto padre, è possibile scegliere un'attività padre. Quando si seleziona un'attività padre, il brano viene creato come sottoattività dell'attività padre nel progetto selezionato.<br>Iniziare a digitare il nome dell'attività padre per il brano, quindi fare clic su di esso quando viene visualizzato nell'elenco a discesa.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Campi personalizzati]</strong></td>
      <td>Seleziona i moduli personalizzati da aggiungere alla storia.</td>
     </tr>
    </tbody>
   </table>

1. Fai clic su **[!UICONTROL Salva storia]**.
