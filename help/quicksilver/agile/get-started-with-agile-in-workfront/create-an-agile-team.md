---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Creare un team agile
description: Adobe Workfront consente ai team Agile di completare il lavoro in modo incrementale e organizzato.
author: Jenny
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 2%

---

# Creare un team Agile

<!--Audited: 01/2024-->

[!DNL Adobe Workfront] consente ai team Agile di completare il lavoro in modo incrementale e organizzato.

Qualsiasi utente dell’organizzazione può vedere il team Agile e visualizzare tutti i componenti Agile del team, inclusi il backlog, le iterazioni, la bacheca delle storie e le singole storie. Tuttavia, solo i membri del team con accesso [!UICONTROL Modifica] al lavoro possono apportare modifiche al lavoro assegnato al team.

[!DNL Workfront] supporta le seguenti metodologie Agile:

* **[!UICONTROL Scrum]**: i team hanno un backlog di lavoro che deve essere completato. Quando il team è pronto a lavorare su un pezzo specifico di lavoro, il lavoro viene spostato dal backlog a un’iterazione. Per informazioni più dettagliate sulla gestione di un team Scrum, vedi [Scrum in un team Agile](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** I team spostano il lavoro nella visualizzazione Kanban in stati predeterminati. Gli stati predefiniti sono: backlog, in-process e done. Per informazioni più dettagliate sulla gestione di un team Kanban, vedi [Kanban in un team Agile](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Pianifica la creazione di un nuovo team Agile</p>
  <p>Lavora o più per convertire un team in un team agile</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Decidere su una metodologia Agile

Puoi utilizzare una metodologia Scrum o Kanban Agile per il tuo team Agile. Ogni metodologia offre diversi vantaggi. Il modo in cui lavora il team Agile determina la metodologia Agile che scegli di utilizzare.

Entrambe le metodologie Scrum e Kanban Agile in [!DNL Workfront] consentono di spostare le storie in una bacheca delle storie per indicare una modifica dello stato e l&#39;avanzamento della storia.

Le metodologie Scrum e Kanban Agile in [!DNL Workfront] differiscono nei seguenti modi:

### Vantaggi dell&#39;utilizzo di Kanban in [!DNL Workfront]

La metodologia Agile [!DNL Kanban] in [!DNL Workfront] consente di spostare più facilmente le storie in una bacheca delle storie Agile, limitando al contempo la quantità di lavoro in corso. Nessuna data di inizio e fine quando si utilizza la metodologia Agile [!DNL Kanban].

Le funzionalità seguenti supportano questa metodologia:

* Visualizza il backlog nella bacheca delle storie di Agile [!DNL Kanban].
Per ulteriori informazioni, vedere [Aggiungere il backlog alla bacheca [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Configura gli elementi nel backlog da aggiungere automaticamente allo storyboard Agile [!UICONTROL Kanban] quando gli altri elementi vengono spostati in uno stato che equivale a Complete.
Per ulteriori informazioni, vedere la sezione [Configurare i brani da aggiungere automaticamente dal backlog](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) nell&#39;articolo [Configurare Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configura un limite WIP (Work In Progress) da visualizzare sullo storyboard Agile [!UICONTROL Kanban].
Per ulteriori informazioni, vedere [Gestire il limite WIP (Work In Progress) sulla bacheca Kanban](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Vantaggi dell&#39;utilizzo di Scrum in [!DNL Workfront]

La metodologia Scrum Agile in [!DNL Workfront] consente di aggiungere un set di storie a un&#39;iterazione Agile e di creare una bacheca delle storie per tale iterazione. L&#39;iterazione si basa sulle date di inizio e di fine definite.

Le funzionalità seguenti supportano questa metodologia:

* Includi problemi nello storyboard [!UICONTROL Scrum]
* Includi problemi nel backlog di un team Agile
* Le sottoattività possono essere visualizzate sullo storyboard [!UICONTROL Scrum]
* Visualizza un grafico a burn-down per visualizzare i progressi rispetto alle storie durante l’iterazione
Per ulteriori informazioni, vedere [Panoramica del grafico a burn-down Agile](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Creare un team Agile

{{step1-to-team}}

1. Fai clic sull&#39;icona **[!UICONTROL Switch Teams]** ![Switch team icon](assets/switch-team-icon.png), quindi fai clic su **[!UICONTROL Create new team]**.

   ![Seleziona Crea nuovo team](assets/create-new-team.png)

   Viene visualizzata la casella Nuovo team.

1. Specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Nome team]</strong> </td> 
      <td>Digita un nome per il nuovo team Agile.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Questo è un Team Agile]</strong> </td> 
      <td>Seleziona questa opzione per configurare il nuovo team come Team agile.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>[!UICONTROL Attivo]</strong> </td> 
      <td>Selezionare questa opzione per attivare il team. I team inattivi non sono visibili agli altri utenti per l’assegnazione al lavoro. </td> 
     </tr>


   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Group]</strong> </td> 
      <td> <p>Inizia a digitare il nome di un gruppo da aggiungere al team, quindi selezionalo quando viene visualizzato nell’elenco a discesa.</p> <p><b>NOTA</b></p> <p> Quando un team viene assegnato a un gruppo o a un sottogruppo, qualsiasi amministratore di gruppo di tale gruppo o sottogruppo può gestire il team senza esserne membro. Gli amministratori dei gruppi possono passare all'area [!UICONTROL Team] dal menu principale  e fare clic sulla freccia [!UICONTROL Switch Teams] <img src="assets/switch-team-icon.png" alt="Icona Cambia team"> per elencare tutti i team assegnati ai gruppi che gestiscono.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Membri Team]</strong> </td> 
      <td>Inizia a digitare il nome di un utente che deve far parte del team, quindi selezionalo quando viene visualizzato nell’elenco a discesa.<br>Ripetere questo processo per aggiungere più utenti al team.<br>Poiché gli utenti possono far parte di più team, possono far parte sia dei team Agile che di quelli non Agile.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Descrizione]</strong> </td> 
      <td><p>Digitare una descrizione per il team.</p> <p>La descrizione viene visualizzata in alto a destra nell'area [!UICONTROL Teams] quando il team è selezionato.</p>
      <p>Se la descrizione è lunga, è possibile fare clic su di essa per visualizzare la descrizione completa in un pop-up. Se si dispone dell'accesso per modificare le impostazioni del team di , è anche possibile modificare la descrizione direttamente nel pop-up.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Crea]**.

   Per informazioni sulla configurazione di un team Agile, consulta i seguenti articoli:

   * [Configura [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configura [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Convertire un team esistente in un team Agile

Puoi convertire un team esistente in un team agile:

{{step1-to-team}}

1. Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team icona](assets/switch-team-icon.png), quindi seleziona un nuovo team dal menu a discesa o cerca un team nella barra di ricerca.

1. Seleziona il team da convertire in team Agile.
1. Fai clic sul menu **[!UICONTROL Altro]**, quindi seleziona **[!UICONTROL Modifica]**.

   Solo i membri del team con una licenza [!UICONTROL Standard], [!UICONTROL Piano] o [!UICONTROL Lavoro] possono vedere questa opzione.
   ![Seleziona Modifica](assets/edit-team-settings.png)

1. Nella sezione **[!UICONTROL Agile]**, seleziona **[!UICONTROL Questo è un team Agile]**.

1. Nella sezione **[!UICONTROL Metodologia]**, seleziona se il team utilizzerà una metodologia Agile **[!UICONTROL Scrum]** o **[!UICONTROL Kanban]**.

1. Fai clic su **Salva modifiche**.

   Il team viene salvato come team Agile. È possibile configurare il nuovo team come Scrum o Kanban quando si modifica il team.

   Per ulteriori informazioni, consulta i seguenti articoli:

   * [Configura [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configura [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
