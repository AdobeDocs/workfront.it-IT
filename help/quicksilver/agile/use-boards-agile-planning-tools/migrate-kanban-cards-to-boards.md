---
content-type: reference
navigation-topic: boards
title: Migrazione delle schede Kanban del team Agile alle schede madri Workfront
description: È possibile migrare gli elementi di lavoro da una bacheca Kanban del team Agile a una bacheca Workfront nuova o esistente.
author: Lisa
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Migrare le schede Kanban del team agile alle schede madri Workfront

È possibile migrare gli elementi di lavoro da una bacheca Kanban del team Agile a una bacheca Workfront nuova o esistente. Quando esegui la migrazione, tutte le schede sulla bacheca Kanban vengono copiate nella bacheca Workfront. Non è consentito scegliere schede specifiche.

Il posizionamento delle schede sulla bacheca Workfront si basa su criteri colonna. Ad esempio, una policy potrebbe spostare tutte le carte con lo stato &quot;In corso&quot; in una colonna specifica. Per ulteriori informazioni sui criteri di colonna, consulta [Gestisci colonne bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) Se non sono presenti criteri o le schede non corrispondono ai criteri, le schede vengono posizionate nella colonna più a sinistra della bacheca. Al momento, le schede nella colonna Backlog nella bacheca legacy non vengono aggiunte alla bacheca Workfront.

Le schede non vengono rimosse dalla bacheca Kanban del team Agile e le modifiche di stato delle schede verranno sincronizzate con entrambe le bacheche. È possibile mantenere entrambe le schede attive fino a quando non si è pronti a passare alle schede Workfront.

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
