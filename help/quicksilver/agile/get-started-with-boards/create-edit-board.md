---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Creazione o modifica di una bacheca
description: Dal dashboard [!UICONTROL bacheche], puoi creare una nuova bacheca o modificarne una esistente.
author: Courtney
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 6%

---

# Creare o modificare una bacheca

<!-- Audited: 12/2023 -->

Dal dashboard [!UICONTROL bacheche], puoi creare una nuova bacheca o modificarne una esistente.

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

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crea una nuova bacheca

{{step1-to-boards}}

1. Fai clic su **[!UICONTROL Aggiungi bacheca]**.

1. Seleziona un modello per la bacheca.

   | Modello | Descrizione |
   |---------|----------|
   | Bacheca base | Nella bacheca sono disponibili tre colonne predefinite. Potete aggiungere nuove colonne e rinominare o eliminare le colonne predefinite. <p>Nella bacheca sono disponibili tre colonne predefinite. Potete aggiungere nuove colonne e rinominare o eliminare le colonne predefinite. |
   | Bacheca Kanban | Nella bacheca sono disponibili le seguenti colonne: Backlog, Nuovo, In corso, Completo e Bloccato. Potete aggiungere nuove colonne e rinominare o eliminare le colonne predefinite.<p>Per utilizzare il backlog, è necessario impostare i filtri per la colonna di input. Per informazioni, vedere [Aggiungere una colonna di aspirazione a una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Per verificare i criteri predefiniti per ogni colonna, fare clic sul menu [!UICONTROL **Altro**] in una colonna e selezionare [!UICONTROL **Modifica**]. Puoi modificare una di queste policy predefinite. Per informazioni, consulta [Gestire le colonne delle bacheche](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Bacheca retrospettiva | Le seguenti colonne sono fornite sulla bacheca: Che cosa è andato bene? Cosa potrebbe essere migliorato? Chi dovremmo celebrare? Cosa possiamo fare per muoverci più velocemente? Potete aggiungere nuove colonne e rinominare o eliminare le colonne predefinite. <p>Nessun criterio colonna applicato. |
   | Bacheca dinamica | Nella bacheca sono disponibili le seguenti colonne: Non selezionato, Nuovo, In corso, In sospeso e Completo. Potete aggiungere nuove colonne e rinominare o eliminare le colonne predefinite. La colonna Non selezionato può essere rinominata ma non eliminata. Questa colonna contiene tutte le schede con uno stato che non corrisponde a nessuno degli altri stati della colonna.) <p>I criteri di colonna predefiniti assegnano le schede alle colonne in base al loro stato. Per informazioni, consulta [Gestire le colonne della bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. Solo per una scheda dinamica, segui i passaggi della procedura guidata di configurazione:

   1. Digita un nome per la bacheca e fai clic su [!UICONTROL **Avanti**].
   1. Cerca e seleziona [!DNL Workfront] [!UICONTROL **Progetti**] per inserire attività e problemi nella bacheca.
   1. Cerca e seleziona [!UICONTROL **Assegnazioni**] per inserire attività e problemi nella bacheca.

      Tutti gli oggetti vengono visualizzati sulla scheda come schede collegate.

      Il contatore [!UICONTROL **Schede da aggiungere**] indica quante schede saranno presenti sulla bacheca. Se ad esempio si seleziona un progetto con 100 attività e problemi, il contatore indica 100. Se si aggiunge un&#39;assegnazione utente e la persona viene assegnata a 5 attività del progetto, il contatore indica 5.

      >[!NOTE]
      >
      >Il limite di schede dinamiche è di 700 operazioni e 700 problemi, per un totale di 1.400 schede. Un numero elevato di schede può influire sulle prestazioni della scheda. Tutte le schede archiviate, sia nascoste che visibili, vengono conteggiate ai fini del raggiungimento di questo limite.

   1. (Facoltativo) Selezionare [!UICONTROL **Non archiviare le schede completate**] per inserire le attività completate e i problemi nella scheda come schede visibili nella colonna Completato. Quando questa opzione non è selezionata, le schede completate al momento della creazione della scheda vengono inserite nella scheda come schede archiviate.

      >[!NOTE]
      >
      >Per impostazione predefinita, le schede archiviate non vengono visualizzate sulla bacheca. Per visualizzare le schede archiviate, è necessario attivare un&#39;impostazione di configurazione e quindi filtrare la scheda per visualizzare le schede archiviate. Per ulteriori informazioni, consulta [Personalizzare i campi visualizzati in una scheda](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) e [Filtrare e cercare in una bacheca](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   1. (Facoltativo) Fai clic su [!UICONTROL **Usa filtri avanzati**] per visualizzare altre opzioni di filtro.

      È lo stesso processo della creazione di un filtro per una colonna di acquisizione. Per ulteriori informazioni, vedere [Aggiungere una colonna di acquisizione a una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

      Se aggiorni i filtri su una bacheca dinamica dopo la sua creazione, le impostazioni della scheda che non fanno parte dell’attività o del problema di Workfront (come i tag) vengono reimpostate.

   1. Dopo aver aggiunto i filtri, fai clic su [!UICONTROL **Crea bacheca**].

1. Digita un nome per la bacheca nel campo **[!UICONTROL Bacheca]** e premi Invio.
1. Configura la bacheca in base alle esigenze.

   Per ulteriori informazioni, consulta [Aggiungere o rimuovere membri da una bacheca](../../agile/get-started-with-boards/add-members-to-board.md), [Gestire le colonne delle bacheche](../../agile/get-started-with-boards/manage-board-columns.md), [Aggiungere una scheda ad hoc a una bacheca](../../agile/get-started-with-boards/add-card-to-board.md) e [Utilizzare schede collegate sulle bacheche](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. Fai clic su **[!UICONTROL Tutte le bacheche]** per tornare al dashboard delle bacheche.

   Puoi anche individuare il menu a discesa con il nome della bacheca corrente e fare clic su di essa per passare a un’altra bacheca.

   ![Elenco delle bacheche](assets/boards-button-list-of-boards-350x188.png)

## Modificare una bacheca esistente

{{step1-to-boards}}

1. Nel dashboard, seleziona la bacheca da aprire.
1. Modifica la bacheca in base alle esigenze. Puoi fare clic sul nome della bacheca per rinominarla.

   Per sincronizzare le schede collegate con Workfront e inserire nuove attività e problemi nella scheda o nella colonna di immissione, fare clic sul menu **[!UICONTROL Altro]** ![[!UICONTROL Altro menu]](assets/more-icon-spectrum.png) accanto al nome della scheda e selezionare **[!UICONTROL Sincronizza elementi connessi]**.

   Per ulteriori informazioni, consulta [Aggiungere o rimuovere membri da una bacheca](../../agile/get-started-with-boards/add-members-to-board.md), [Gestire le colonne delle bacheche](../../agile/get-started-with-boards/manage-board-columns.md) e [Aggiungere una scheda a una bacheca](../../agile/get-started-with-boards/add-card-to-board.md).

1. Fai clic su **[!UICONTROL Tutte le bacheche]** per tornare al dashboard delle bacheche.

   Puoi anche individuare il menu a discesa con il nome della bacheca corrente e fare clic su di essa per passare a un’altra bacheca.

