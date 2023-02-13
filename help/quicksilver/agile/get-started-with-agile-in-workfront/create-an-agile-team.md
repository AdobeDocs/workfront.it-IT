---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Creare un team agile
description: Adobe Workfront consente ai team agili di completare il lavoro in modo incrementale e organizzato.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 0%

---

# Creare un team agile

[!DNL Adobe Workfront] consente ai team agili di completare il lavoro in modo incrementale e organizzato.

Qualsiasi utente dell’organizzazione può vedere il team agile e visualizzare tutti i componenti agili per il team, compresi il backlog, le iterazioni, la storiella e i singoli racconti. Tuttavia, solo i membri del team con [!UICONTROL Modifica] l&#39;accesso al lavoro può apportare modifiche al lavoro assegnato al team.

[!DNL Workfront] supporta le seguenti metodologie agili:

* **[!UICONTROL Scratto]**: Le squadre hanno un ritardo di lavoro che deve essere fatto. Quando il team è pronto per lavorare su un blocco di lavoro specifico, il lavoro viene spostato dal backlog a un&#39;iterazione. Per informazioni più dettagliate sulla gestione di un team Scrum, vedi [Rum in una squadra agile](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** I team spostano il lavoro nella vista Kanban tra gli stati predeterminati. Gli stati predefiniti sono: backlog, in-process e done. Per informazioni più dettagliate sulla gestione di un team Kanban, vedi [Kanban in un team agile](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

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
   <td> <p>[!UICONTROL Plan] per creare un nuovo team agile; Lavoro [!UICONTROL] o superiore per convertire un team in un team agile</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo [!DNL Workfront] amministratore.

## Decidere su una metodologia agile

Puoi utilizzare una metodologia agile Scrum o Kanban per il tuo team agile. Ogni metodologia offre diversi vantaggi. Il modo in cui il tuo team agile funziona determina la metodologia agile che scegli di utilizzare.

Metodologie sia di Scrum che di Kanban agile [!DNL Workfront] consente di spostare i racconti in un&#39;area della storia per indicare un cambiamento di stato e l&#39;avanzamento della storia.

Metodologie agili di Scrum e Kanban in [!DNL Workfront] sono diversi nei seguenti modi:

### Vantaggi dell’utilizzo di Kanban in [!DNL Workfront]

La [!DNL Kanban] metodo agile [!DNL Workfront] consente di spostare più facilmente le storie in una bacheca di storie agili limitando al contempo la quantità di lavoro in corso. Non ci sono date di inizio e di fine quando si utilizza il [!DNL Kanban] metodo agile.

La seguente funzionalità supporta questa metodologia:

* Visualizza il backlog sul [!DNL Kanban] tabellone di storia agile.\
   Per ulteriori informazioni, consulta [Aggiungi il backlog al [!UICONTROL Kanban] bacheca](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Configura gli elementi del backlog da aggiungere automaticamente al [!UICONTROL Kanban] tabellone della storia agile quando altri elementi vengono spostati in uno stato che equivale a Complete.\
   Per ulteriori informazioni, consulta la sezione . [Configurare le storie da aggiungere automaticamente dal backlog](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) nell&#39;articolo [Configurare Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configura un limite WIP da visualizzare sul [!UICONTROL Kanban] tabellone di storia agile.\
   Per ulteriori informazioni, consulta [Gestire il limite WIP sulla bacheca kanban](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Vantaggi dell&#39;utilizzo di Scrum in [!DNL Workfront]

La metodologia Scrum agile in [!DNL Workfront] consente di aggiungere un insieme di storie a un&#39;iterazione agile e di creare una tabella di storie per tale iterazione. L’iterazione si basa sulle date di inizio e di fine definite dall’utente.

La seguente funzionalità supporta questa metodologia:

* Includi i problemi nel [!UICONTROL Scratto] tabellone
* Includi problemi nel backlog di un team agile
* Le sottoattività possono essere visualizzate sul [!UICONTROL Scratto] tabellone
* Visualizza un grafico a discesa per visualizzare l&#39;avanzamento rispetto ai brani durante l&#39;iterazione\
   Per ulteriori informazioni, consulta [Panoramica del grafico a discesa Agile](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Crea un nuovo team agile

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.
1. Fai clic sul pulsante **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi fai clic su **[!UICONTROL Crea nuovo team]**.

   ![Selezionare Crea nuovo team.](assets/create-new-team-350x198.png)

1. Specifica le seguenti informazioni sul [!UICONTROL Nuovo team] finestra di dialogo:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Name]</strong> </td> 
      <td>Digita un nome per il nuovo team agile.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Questo è un team Agile]</strong> </td> 
      <td>Seleziona questa opzione per configurare questo nuovo team come team agile.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Group]</strong> </td> 
      <td> <p>Inizia a digitare il nome di un gruppo da aggiungere al team, quindi seleziona il nome quando viene visualizzato nell’elenco a discesa.</p> <p>Nota: Quando un team viene assegnato a un gruppo o a un sottogruppo, gli amministratori del gruppo o sottogruppo possono gestire il team senza esserne membri. Gli amministratori del gruppo possono passare all'area [!UICONTROL Teams] dal menu principale e fare clic sulla freccia [!UICONTROL Switch Teams] <img src="assets/switch-team-icon.png" alt="Icona Cambia team"> per elencare tutti i team assegnati ai gruppi gestiti.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Members]</strong> </td> 
      <td>Inizia a digitare il nome di un utente che deve far parte del team, quindi seleziona il nome quando viene visualizzato nell’elenco a discesa.<br>Ripeti questo processo per aggiungere più utenti al team.<br>Poiché gli utenti possono far parte di più di un team, possono essere sia su team agili che non agili.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Descrizione]</strong> </td> 
      <td><p>Digita una descrizione per il team.</p> <p>La descrizione viene visualizzata in alto a destra nell’area dei team quando il team è selezionato.</p>
      <p>Se la descrizione è lunga, puoi fare clic su di essa per visualizzarne la descrizione completa in un pop-up. Se hai accesso per modificare le [!UICONTROL impostazioni del team], puoi anche modificare la descrizione direttamente nella finestra a comparsa.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Crea]**.

   Per informazioni sulla configurazione di un team Agile, vedi i seguenti articoli:

   * [Configura [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configura [!UICONTROL Scratto]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Convertire un team esistente in un team agile

Puoi convertire un team esistente in un team agile:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.
1. Fai clic sul pulsante **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.

1. Seleziona il team da convertire in un team agile.
1. Fai clic sul pulsante **[!UICONTROL Altro]** quindi seleziona **[!UICONTROL Modifica]**.\
   Solo i membri del team con una [!UICONTROL Pianificare] o [!UICONTROL Lavoro] licenza vedere questa opzione.\
   ![](assets/edit-team-settings-350x205.png)

1. In **[!UICONTROL Agile]** sezione , seleziona **[!UICONTROL Questo è un team Agile]**.

1. In **[!UICONTROL Metodologia]** seleziona se il team utilizzerà un **[!UICONTROL Scratto]** o **[!UICONTROL Kanban]** metodo agile.

1. Fai clic su **Salva le modifiche.**

   Per informazioni sulla configurazione di un team Agile, vedi i seguenti articoli:

   * [Configura [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configura [!UICONTROL Scratto]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
