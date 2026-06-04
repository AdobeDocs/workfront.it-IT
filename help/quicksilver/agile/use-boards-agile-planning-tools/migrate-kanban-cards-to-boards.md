---
content-type: reference
navigation-topic: boards
title: Migrazione delle schede Kanban del team Agile alle schede madri Workfront
description: Puoi migrare gli elementi di lavoro da una bacheca Kanban del team Agile a una bacheca Workfront nuova o esistente.
author: Courtney
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/RXk7PYF6JsdF71pRVwEA-Wk23h-UqbgLPXSyNR7VX5Y
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 360
ht-degree: 11%

---

# Migrazione delle schede Kanban del team Agile alle bacheche Workfront

Puoi migrare gli elementi di lavoro da una bacheca Kanban del team Agile a una bacheca Workfront nuova o esistente. Quando esegui la migrazione, tutte le schede sulla bacheca Kanban vengono copiate nella bacheca Workfront. Non è consentito scegliere schede specifiche.

Il posizionamento delle schede sulla bacheca Workfront si basa su criteri colonna. Ad esempio, una policy potrebbe spostare tutte le carte con lo stato &quot;In corso&quot; in una colonna specifica. Per ulteriori informazioni sui criteri delle colonne, vedere [Gestisci colonne bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) Se non ci sono criteri o le schede non corrispondono ai criteri, le schede vengono posizionate nella colonna più a sinistra sulla bacheca. Al momento, le schede nella colonna Backlog nella bacheca legacy non vengono aggiunte alla bacheca Workfront.

Le schede non vengono rimosse dalla bacheca Kanban del team Agile e le modifiche di stato delle schede verranno sincronizzate con entrambe le bacheche. È possibile mantenere entrambe le schede attive fino a quando non si è pronti a passare alle schede Workfront.

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

## Migrare schede Kanban a una nuova bacheca

{{step1-to-team}}

1. Accedi a un Kanban Board.
1. Fai clic su [!UICONTROL **Aggiungi alle bacheche**] e seleziona [!UICONTROL **Nuova bacheca**].
1. Nella finestra di dialogo [!UICONTROL Aggiungi a nuova bacheca], digita un nome per la nuova bacheca (viene visualizzato automaticamente il nome della bacheca [!UICONTROL Kanban] corrente) e fai clic su [!UICONTROL **Aggiungi**].

   ![Aggiungi schede Kanban a una nuova bacheca](assets/add-kanban-cards-to-new-board-dialog.png)

1. (Facoltativo) Nel messaggio di successo visualizzato, fai clic sul collegamento per aprire la nuova bacheca.

## Migrare schede Kanban a una bacheca esistente

{{step1-to-team}}

1. Accedi a un Kanban Board.
1. Fai clic su [!UICONTROL **Aggiungi alle bacheche**] e seleziona [!UICONTROL **Bacheca esistente**].
1. Nella finestra di dialogo [!UICONTROL Aggiungi alla bacheca esistente], cerca e seleziona la bacheca in cui migrare le schede. Quindi fare clic su [!UICONTROL **Aggiungi**].

   ![Aggiungi schede Kanban alla bacheca esistente](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (Facoltativo) Nel messaggio di successo visualizzato, fai clic sul collegamento per aprire la bacheca.
