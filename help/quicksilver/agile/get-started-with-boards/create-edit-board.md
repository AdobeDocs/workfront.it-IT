---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Creare o modificare una bacheca
description: Dalla sezione [!UICONTROL schede madri] dashboard, puoi creare una nuova bacheca o modificare una bacheca esistente.
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: d593d288546abb4a674646519c6245563673b938
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Creare o modificare una bacheca

<!-- Audited: 12/2023 -->

Dalla sezione [!UICONTROL schede madri] dashboard, puoi creare una nuova bacheca o modificare una bacheca esistente.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> <p>Nuovo: Collaboratore o versione successiva </p>
 <p>oppure</p> 
<p>Corrente: [!UICONTROL Request] o versione successiva </p> 
</td> 
  </tr>
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Crea una nuova bacheca

{{step1-to-boards}}

1. Clic **[!UICONTROL Aggiungi bacheca]**.

1. Seleziona un modello per la bacheca.

   | Modello | Descrizione |
   |---------|----------|
   | Bacheca base | Sulla bacheca sono disponibili tre colonne predefinite. È possibile aggiungere nuove colonne e rinominare o eliminare le colonne predefinite. <p>Sulla bacheca sono disponibili tre colonne predefinite. È possibile aggiungere nuove colonne e rinominare o eliminare le colonne predefinite. |
   | Bacheca Kanban | Nella bacheca sono disponibili le seguenti colonne: Backlog, Nuovo, In corso, Completo e In sospeso. È possibile aggiungere nuove colonne e rinominare o eliminare le colonne predefinite.<p>Per utilizzare il backlog, è necessario impostare i filtri per la colonna Acquisizione. Per informazioni, consulta [Aggiungere una colonna Acquisizione a una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Per rivedere i criteri predefiniti per ogni colonna, fare clic sul pulsante [!UICONTROL **Altro** menu] in una colonna e seleziona [!UICONTROL **Modifica**]. Puoi modificare uno qualsiasi di questi criteri predefiniti. Per informazioni, consulta [Gestisci colonne bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Bacheca retrospettiva | Sulla bacheca sono fornite le seguenti colonne: Cosa è andato bene? Cosa si può migliorare? Chi dovremmo festeggiare? Cosa possiamo fare per muoverci più velocemente? È possibile aggiungere nuove colonne e rinominare o eliminare le colonne predefinite. <p>Nessun criterio colonna applicato. |
   | Bacheca dinamica | Nella bacheca sono disponibili le seguenti colonne: Non selezionato, Nuovo, In corso, In sospeso e Completo. È possibile aggiungere nuove colonne e rinominare o eliminare le colonne predefinite. La colonna Non selezionato può essere rinominata ma non eliminata. Questa colonna contiene tutte le schede con uno stato che non corrisponde a nessuno degli altri stati della colonna.) <p>I criteri di colonna predefiniti assegnano le schede alle colonne in base al loro stato. Per informazioni, consulta [Gestisci colonne bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. Solo per una scheda dinamica, segui i passaggi della procedura guidata di configurazione:

   1. Digita un nome per la bacheca e fai clic su [!UICONTROL **Successivo**].
   1. Cerca e seleziona [!DNL Workfront] [!UICONTROL **Progetti**] per inserire attività e problemi nella bacheca.
   1. Cerca e seleziona [!UICONTROL **Assegnazioni**] per inserire attività e problemi nella bacheca.

      Tutti gli oggetti vengono visualizzati sulla bacheca come schede collegate.

      Il [!UICONTROL **Schede aggiunte**] Il contatore mostra il numero di schede che saranno presenti sulla bacheca. Ad esempio, se selezioni un progetto con 100 attività e problemi, il contatore mostra 100. Se aggiungi un’assegnazione utente e tale persona è assegnata a 5 attività sul progetto, il contatore mostra 5.

      >[!NOTE]
      >
      >Il limite di schede per le bacheche dinamiche è di 700 attività e 700 problemi, per un totale di 1.400 schede. Un numero elevato di schede sulla scheda può influire sulle prestazioni della scheda.

   1. (Facoltativo) Seleziona [!UICONTROL **Non archiviare le schede completate**] per inserire le attività e i problemi completati nella bacheca come schede visibili nella colonna Completati. Se questa opzione non è selezionata, le schede completate al momento della creazione della bacheca vengono inserite nella bacheca come schede archiviate.

      >[!NOTE]
      >
      >Per impostazione predefinita, le schede archiviate non vengono visualizzate sulla bacheca. Per visualizzare le schede archiviate, devi attivare un’impostazione di configurazione e filtrare la bacheca per visualizzarle. Per ulteriori informazioni, consulta [Personalizzare i campi visualizzati su una scheda](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) e [Filtrare ed eseguire ricerche in una bacheca](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   1. (Facoltativo) Fai clic su [!UICONTROL **Utilizzare filtri avanzati**] per visualizzare opzioni di filtro aggiuntive.

      È lo stesso processo della creazione di un filtro per una colonna di acquisizione. Per ulteriori informazioni, consulta [Aggiungere una colonna Acquisizione a una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

      Se aggiorni i filtri su una bacheca dinamica dopo la sua creazione, le impostazioni della scheda che non fanno parte dell’attività o del problema di Workfront (come i tag) vengono reimpostate.

   1. Dopo aver aggiunto i filtri, fai clic su [!UICONTROL **Crea bacheca**].

1. Digita un nome per la bacheca nella **[!UICONTROL Scheda madre]** e premere Invio.
1. Configura la bacheca come necessario.

   Per informazioni, consulta [Aggiungere o rimuovere membri da una bacheca](../../agile/get-started-with-boards/add-members-to-board.md), [Gestisci colonne bacheca](../../agile/get-started-with-boards/manage-board-columns.md), [Aggiungere una scheda ad hoc a una bacheca](../../agile/get-started-with-boards/add-card-to-board.md), e [Utilizzare le schede collegate sulle bacheche](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. Clic **[!UICONTROL Tutte le bacheche]** per tornare alla dashboard delle bacheche.

   Puoi anche individuare il menu a discesa con il nome della bacheca corrente e fare clic su di esso per passare a un’altra bacheca.

   ![Elenco dei board](assets/boards-button-list-of-boards-350x188.png)

## Modificare una bacheca esistente

{{step1-to-boards}}

1. Nel dashboard, seleziona la bacheca da aprire.
1. Modifica la bacheca in base alle esigenze. Puoi fare clic sul nome della bacheca per rinominarla.

   Per informazioni, consulta [Aggiungere o rimuovere membri da una bacheca](../../agile/get-started-with-boards/add-members-to-board.md), [Gestisci colonne bacheca](../../agile/get-started-with-boards/manage-board-columns.md), e [Aggiungere una scheda a una bacheca](../../agile/get-started-with-boards/add-card-to-board.md).

1. Clic **[!UICONTROL Tutte le bacheche]** per tornare alla dashboard delle bacheche.

   Puoi anche individuare il menu a discesa con il nome della bacheca corrente e fare clic su di esso per passare a un’altra bacheca.
