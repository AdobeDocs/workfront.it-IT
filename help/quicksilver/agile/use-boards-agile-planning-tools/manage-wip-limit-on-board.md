---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Gestire il limite WIP (Work In Progress) su una bacheca
description: È possibile configurare un limite WIP per ogni colonna di una bacheca.
author: Jenny
feature: Agile
exl-id: 7901c6e7-75a4-41e4-b288-d527c4a6d031
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Gestisci il limite [!UICONTROL Work in Progress] (WIP) su una bacheca

È possibile configurare un limite di [!UICONTROL Work In Progress] (WIP) per ogni colonna di una bacheca.

Il limite WIP è semplicemente un&#39;avvertenza visiva e non impedisce di avere più elementi in ogni colonna rispetto al limite impostato.

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

## Impostare il limite WIP per una colonna

{{step1-to-boards}}

1. Accedi a una bacheca. Per informazioni, consulta [Creare o modificare una bacheca](../../agile/get-started-with-boards/create-edit-board.md).
1. Individuare la colonna a cui si desidera aggiungere il limite WIP.

   Per aggiungere una nuova colonna, vedi [Gestisci colonne bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

1. Fai clic sul menu **[!UICONTROL Altro]** nella colonna e seleziona **[!UICONTROL Modifica]** per aprire l&#39;area Impostazioni.
1. In [!UICONTROL Criteri colonna], abilita il criterio **[!UICONTROL Work in progress] limit** per limitare il numero di schede che possono essere aggiunte alla colonna.
1. Digitare il numero di limite nel campo **[!UICONTROL Imposta limite]**.

   ![Limite WIP per colonna](assets/boards-wip-limit-in-column.png)

   Il numero di schede e il limite vengono visualizzati nella parte superiore della colonna. Se la colonna contiene più schede del limite, il contatore diventa rosso.

   ![Contatore limite WIP](assets/boards-wip-limit-counter.png)

1. Fai clic su **[!UICONTROL Chiudi]** per uscire dall&#39;area [!UICONTROL Impostazioni] e visualizzare la colonna e le relative schede.
