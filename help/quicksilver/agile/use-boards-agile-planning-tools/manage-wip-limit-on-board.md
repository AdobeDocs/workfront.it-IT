---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Gestire il limite WIP (Work In Progress) su una bacheca
description: È possibile configurare un limite WIP per ogni colonna di una bacheca.
author: Courtney
feature: Agile
exl-id: 7901c6e7-75a4-41e4-b288-d527c4a6d031
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jOCQTCkNgEZfE8O4-KyKVjEluncwWx0vh5NdrKHC9vg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 242
ht-degree: 14%

---

# Gestisci il limite [!UICONTROL Work in Progress] (WIP) su una bacheca

È possibile configurare un limite di [!UICONTROL Work In Progress] (WIP) per ogni colonna di una bacheca.

Il limite WIP è semplicemente un&#39;avvertenza visiva e non impedisce di avere più elementi in ogni colonna rispetto al limite impostato.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o successiva</p> 
   <p>Richiedente o successiva</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
