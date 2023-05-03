---
content-type: reference
navigation-topic: boards
title: Migrazione di schede Kanban del team agile alle schede Workfront
description: È possibile migrare gli elementi di lavoro da una bacheca Kanban di un team agile a una bacheca Workfront nuova o esistente.
author: Lisa
exl-id: c40b6453-5869-437b-a1e0-f20dd833d2b8
source-git-commit: c990b897a4e6722515c6b065ee2a5832fdc31231
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Migrazione di schede Kanban del team agile alle schede Workfront

{{highlighted-preview-article-level}}

È possibile migrare gli elementi di lavoro da una bacheca Kanban di un team agile a una bacheca Workfront nuova o esistente. Quando esegui la migrazione, tutte le schede sulla bacheca Kanban vengono copiate nella bacheca di Workfront. Non è consentito scegliere schede specifiche.

Il posizionamento delle schede sulla bacheca di Workfront si basa sui criteri delle colonne. Ad esempio, un criterio potrebbe spostare tutte le schede con lo stato &quot;In corso&quot; in una colonna specifica. Per ulteriori informazioni sui criteri delle colonne, consulta [Gestire le colonne della bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) Se non sono presenti criteri o le schede non corrispondono ai criteri, le schede vengono posizionate nella colonna più a sinistra della bacheca. Al momento, le schede nella colonna Backlog della bacheca legacy non vengono aggiunte alla bacheca Workfront.

Le schede non vengono rimosse dalla bacheca Kanban del team agile e le modifiche allo stato delle schede si sincronizzano con entrambe le bacheche. Potete mantenere attive entrambe le bacheche finché non siete pronti per passare alle bacheche Workfront.

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
   <td> <p>[!UICONTROL Request] o superiore</p> </td>
  </tr>
 </tbody>
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Migrazione di schede Kanban a una nuova bacheca

{{step1-to-team}}

1. Accedi a una bacheca Kanban.
1. Fai clic su [!UICONTROL **Aggiungi alle bacheche**] e seleziona [!UICONTROL **Nuova bacheca**].
1. Sulla [!UICONTROL Aggiungi a nuova bacheca] digitate un nome per la nuova bacheca (il nome della scheda corrente) [!UICONTROL Kanban] appare automaticamente la bacheca) e fate clic su [!UICONTROL **Aggiungi**].

   ![Aggiungi schede Kanban a una nuova bacheca](assets/add-kanban-cards-to-new-board-dialog.png)

1. (Facoltativo) Nel messaggio di successo visualizzato, fate clic sul collegamento per aprire la nuova bacheca.

## Migrazione di schede Kanban a una scheda esistente

{{step1-to-team}}

1. Accedi a una bacheca Kanban.
1. Fai clic su [!UICONTROL **Aggiungi alle bacheche**] e seleziona [!UICONTROL **Scheda esistente**].
1. Sulla [!UICONTROL Aggiungi a bacheca esistente] finestra di dialogo, cerca e seleziona la bacheca in cui eseguire la migrazione delle schede. Quindi, fai clic su [!UICONTROL **Aggiungi**].

   ![Aggiungi schede Kanban alla bacheca esistente](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (Facoltativo) Nel messaggio di successo visualizzato, fate clic sul collegamento per aprire la bacheca.
