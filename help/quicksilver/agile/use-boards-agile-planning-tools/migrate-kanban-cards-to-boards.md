---
content-type: reference
navigation-topic: boards
title: Migrare le schede Kanban del team agile alle schede madri Workfront
description: È possibile migrare gli elementi di lavoro da una bacheca Kanban del team Agile a una bacheca Workfront nuova o esistente.
author: Lisa
feature: Agile
exl-id: c40b6453-5869-437b-a1e0-f20dd833d2b8
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Migrare le schede Kanban del team agile alle schede madri Workfront

È possibile migrare gli elementi di lavoro da una bacheca Kanban del team Agile a una bacheca Workfront nuova o esistente. Quando esegui la migrazione, tutte le schede sulla bacheca Kanban vengono copiate nella bacheca Workfront. Non è consentito scegliere schede specifiche.

Il posizionamento delle schede sulla bacheca Workfront si basa su criteri colonna. Ad esempio, una policy potrebbe spostare tutte le carte con lo stato &quot;In corso&quot; in una colonna specifica. Per ulteriori informazioni sui criteri delle colonne, consulta [Gestisci colonne bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) Se non ci sono criteri o le schede non corrispondono ai criteri, le schede vengono posizionate nella colonna più a sinistra sulla bacheca. Al momento, le schede nella colonna Backlog nella bacheca legacy non vengono aggiunte alla bacheca Workfront.

Le schede non vengono rimosse dalla bacheca Kanban del team Agile e le modifiche di stato delle schede verranno sincronizzate con entrambe le bacheche. È possibile mantenere entrambe le schede attive fino a quando non si è pronti a passare alle schede Workfront.

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
   <td> <p>[!UICONTROL Request] o versione successiva</p> </td>
  </tr>
 </tbody>
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Migrare schede Kanban a una nuova bacheca

{{step1-to-team}}

1. Accedi a un Kanban Board.
1. Clic [!UICONTROL **Aggiungi a bacheche**] e seleziona [!UICONTROL **Nuova bacheca**].
1. Il giorno [!UICONTROL Aggiungi a nuova bacheca] , digitare un nome per la nuova bacheca (il nome della bacheca [!UICONTROL Kanban] viene visualizzata automaticamente) e fare clic su [!UICONTROL **Aggiungi**].

   ![Aggiungi schede Kanban a nuova bacheca](assets/add-kanban-cards-to-new-board-dialog.png)

1. (Facoltativo) Nel messaggio di successo visualizzato, fai clic sul collegamento per aprire la nuova bacheca.

## Migrare schede Kanban a una bacheca esistente

{{step1-to-team}}

1. Accedi a un Kanban Board.
1. Clic [!UICONTROL **Aggiungi a bacheche**] e seleziona [!UICONTROL **Bacheca esistente**].
1. Il giorno [!UICONTROL Aggiungi a bacheca esistente] , cerca e seleziona la bacheca in cui migrare le schede. Quindi, fai clic su [!UICONTROL **Aggiungi**].

   ![Aggiungi schede Kanban a bacheca esistente](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (Facoltativo) Nel messaggio di successo visualizzato, fai clic sul collegamento per aprire la bacheca.
