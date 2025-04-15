---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Gestisci [!DNL Adobe Workfront] notifiche in [!DNL Microsoft] Team
description: Puoi ricevere notifiche da [!DNL Adobe Workfront] sugli elementi da approvare, sulle assegnazioni che ti sono state assegnate o sui commenti e le modifiche agli elementi a cui sei associato.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 69fdb5c23bb501fc81e4ef3c3ab7c94e78e69d29
workflow-type: tm+mt
source-wordcount: '1338'
ht-degree: 0%

---

# Gestisci notifiche [!DNL Adobe Workfront] in [!DNL Microsoft Teams]

<!--

>[!NOTE]
>
>As of July 1, 2025, Microsoft will remove support for the Classic Teams desktop app. As a result, the Workfront integration with Microsoft Teams will not be supported after the Classic Teams desktop app is no longer available.

-->

Puoi ricevere notifiche da [!DNL Adobe Workfront] sugli elementi da approvare, sulle assegnazioni che ti sono state assegnate o sui commenti e le modifiche agli elementi a cui sei associato.

Queste notifiche contengono [!DNL Workfront] azioni che è possibile eseguire in [!DNL Microsoft Teams] senza spostarsi da [!DNL Microsoft Teams] per eseguirle.

>[!NOTE]
>
>[!DNL Microsoft Teams] non supporta più [!DNL Internet Explorer]. Per utilizzare [!DNL Adobe Workfront for Microsoft Teams integration], è necessario utilizzare un browser diverso da [!DNL Internet Explorer].


## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Lavoro], [!UICONTROL Piano]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## Prerequisiti per ricevere [!DNL Workfront] notifiche in [!DNL Microsoft Teams]

Puoi ricevere [!DNL Workfront] notifiche in [!DNL Microsoft Teams] se sono soddisfatte le seguenti condizioni:

* Il proprietario del team ha installato e configurato [!DNL Workfront for Microsoft Teams] per il team.
* Sei connesso a [!DNL Workfront] da [!DNL Microsoft Teams].
* Hai abilitato le notifiche istantanee in [!DNL Workfront]. Per informazioni sull&#39;attivazione delle notifiche istantanee, vedere [Modificare le proprie notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Per informazioni sull&#39;installazione di [!DNL Workfront for Microsoft Teams] e sull&#39;accesso a [!DNL Workfront from Microsoft Teams], vedere [Installa [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Gestione di [!DNL Workfront] notifiche in [!DNL Microsoft Teams]

Quando l&#39;app [!DNL Workfront for Microsoft Teams] è installata, viene creato un canale di chat [!DNL Workfront] in [!DNL Microsoft Teams] per ogni membro del team. Quando viene eseguita una determinata azione in [!DNL Workfront], è possibile configurare le impostazioni per [!DNL Workfront for Microsoft Teams] per ricevere notifiche su tale azione nel canale di chat di [!DNL Microsoft Teams] di [!DNL Workfront].

Quando si lavora con [!DNL Workfront] notifiche da [!DNL Microsoft Teams], considera quanto segue:

* Non è possibile ricevere tutte le notifiche, ma solo un numero selezionato di [!DNL Workfront] notifiche in [!DNL Microsoft Teams].
* Tutte le notifiche ricevute da [!DNL Workfront] vengono visualizzate nel canale chat di bot [!DNL Workfront].

  Per informazioni sull&#39;installazione del canale bot [!DNL Workfront], vedere la sezione [Accesso a [!DNL Workfront] da [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) nell&#39;articolo [Installazione [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

* Può trascorrere un ritardo di 5 minuti tra il momento in cui viene effettuato un aggiornamento in [!DNL Workfront] e il momento in cui ricevi la relativa notifica in [!DNL Microsoft Teams].
* Per ogni notifica di [!DNL Microsoft Teams], si riceve anche una notifica e-mail.

Per gestire le notifiche [!DNL Workfront] che è possibile ricevere in [!DNL Microsoft Teams]:

1. Fai clic sull&#39;icona **[!UICONTROL Altre app aggiunte]** (tre punti) sulla barra di navigazione a sinistra in [!DNL Microsoft Teams].

1. Fare clic su [!DNL Workfront] nell&#39;elenco visualizzato.
1. Seleziona la scheda **[!UICONTROL Impostazioni]**.

   ![Scheda Impostazioni MS Teams](assets/ms-teams-settings-tab-350x552.png)

1. Disattiva le notifiche che non desideri ricevere. Puoi abilitare o disabilitare gruppi di notifiche, ad esempio notifiche di informazione o di approvazione, oppure gestire le notifiche singolarmente.

   Tutte le notifiche sono abilitate per impostazione predefinita.

   Le impostazioni delle notifiche per [!DNL Workfront for Microsoft] team vengono salvate automaticamente.

   >[!NOTE]
   >
   >Non è possibile aggiungere altre notifiche a quelle disponibili per impostazione predefinita.

## Risposta a [!DNL Workfront] notifiche e richieste di approvazione in [!DNL Microsoft Teams]

1. Accedere a [!DNL Workfront] da [!DNL Microsoft Teams].\
   Per informazioni sull&#39;accesso a [!DNL Workfront], vedere [Installa [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Vai all&#39;area **[!UICONTROL Chat]** e fai clic sul canale bot **[!DNL Workfront]**.\
   Questo canale è destinato alla tua chat personale con il bot [!DNL Workfront]. Tutte le notifiche [!DNL Workfront] vengono visualizzate qui.
1. A seconda del tipo di notifica che ricevi, procedi alla sezione pertinente:

   * [Notifiche di approvazione](#approval-notifications-approval-notifications)
   * [Notifiche di assegnazione](#assignment-notifications-assignment-notifications)
   * [Notifiche di commenti](#comment-notifications-comment-notifications)
   * [Aggiorna notifiche](#update-notifications-update-notifications)
   * [Notifiche di modifica data](#date-change-notifications-date-change-notifications)

### Notifiche di approvazione {#approval-notifications}

Si ricevono notifiche di approvazione quando viene richiesto di approvare un oggetto, ad esempio un&#39;attività, una scheda orario o una bozza. È comunque possibile aggiungere un commento alla notifica.Dalla notifica di approvazione, è possibile eseguire le azioni seguenti:

* **[!UICONTROL Approva]**: fare clic per approvare l&#39;elemento.
* **[!UICONTROL Modifica]**: fare clic per approvare l&#39;elemento con le modifiche.
* **[!UICONTROL Rifiuta]**: fare clic per rifiutare l&#39;elemento.
* **[!UICONTROL Commento]**: fare clic per aggiungere un commento. Il commento viene visualizzato anche in [!DNL Workfront] come aggiornamento dell&#39;oggetto che la notifica riguarda.
* **[!UICONTROL Vai alla bozza]**: fai clic per aprire la bozza. Puoi quindi prendere una decisione direttamente nella bozza. Per ulteriori informazioni, vedere [Decidere su una bozza nel visualizzatore di bozze](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

>[!NOTE]
>
>Dopo aver preso una decisione di approvazione, non puoi modificarla dalla notifica.

#### Azioni disponibili su notifiche di approvazione specifiche:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notifica</th> 
   <th>[!UICONTROL Approva]</th> 
   <th>[!UICONTROL rifiuta]</th> 
   <th> <p>[!UICONTROL Change]</p> </th> 
   <th> <p>[!UICONTROL Vai alla bozza] </p> </th> 
   <th>[!UICONTROL Comment]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">È necessario approvare un progetto</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">È necessario approvare un'attività</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">È necessario approvare un problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">È necessario approvare un documento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">È necessario approvare l’accesso a un oggetto</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">È necessario approvare una scheda orario</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Qualcuno vuole che tu approvi questa bozza</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Scheda orario rifiutata</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">La scheda orario è stata riaperta</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Una richiesta di approvazione documento richiesta viene approvata</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Una richiesta di approvazione documento richiesta viene approvata con modifiche</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Richiesta di approvazione documento rifiutata</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">La scheda orario è stata approvata</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Notifiche di assegnazione {#assignment-notifications}

Ricevi notifiche di assegnazione quando tu o un team a cui lavori siete assegnati a un&#39;attività o a un problema in Workfront. Dalla notifica di assegnazione è possibile eseguire le azioni seguenti:

* **[!UICONTROL Lavoraci]**: seleziona per eseguire il commit per lavorare sull&#39;elemento. Viene visualizzata brevemente una notifica per confermare che un nuovo elemento è stato aggiunto all’elenco di lavoro.
* **[!UICONTROL Visualizza in[!DNL Workfront]]**: selezionare questa opzione per visualizzare il problema o l&#39;attività assegnata in Workfront, che apre una nuova scheda.
* **[!UICONTROL Inizio]**: fare clic per avviare il lavoro sull&#39;elemento. Viene visualizzata brevemente una notifica per confermare che un nuovo elemento è stato aggiunto all’elenco di lavoro.
* **[!UICONTROL Commento]**: fare clic per aggiungere un commento all&#39;elemento. Il commento viene visualizzato anche nel flusso di aggiornamento dell&#39;elemento in Workfront.
* **[!UICONTROL Stato]**: fare clic su, quindi selezionare il nuovo stato per l&#39;elemento di lavoro dal menu a discesa.

#### Azioni disponibili su notifiche di assegnazione specifiche:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notifica</th> 
   <th>[!UICONTROL Start]</th> 
   <th>[!UICONTROL Comment]</th> 
   <th> <p>[!UICONTROL Stato]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ti è stata assegnata un’attività</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ti è stato assegnato un problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un team al quale si è assegnati riceve una richiesta di lavoro per un'attività</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un team a cui sei assegnato riceve una richiesta di lavoro per un problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Notifiche di commenti {#comment-notifications}

Ricevi una notifica di comunicazione quando qualcuno commenta un elemento a cui sei associato o ti include in un aggiornamento. Dalla notifica di comunicazione, puoi eseguire le seguenti azioni:

* **Rapprly**: fai clic per rispondere al commento o [!UICONTROL aggiorna]. La risposta viene visualizzata anche nel flusso di aggiornamento in cui il commento viene visualizzato in Workfront.
* **[!UICONTROL Visualizza in Workfront]**: selezionare questa opzione per visualizzare il commento e l&#39;elemento in Workfront, che viene aperto in una nuova scheda.
* **[!UICONTROL Stato]**: fare clic su, quindi selezionare un nuovo stato per l&#39;elemento di lavoro su cui verte il commento o l&#39;aggiornamento.

#### Azioni disponibili su notifiche di comunicazione specifiche:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notifica</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL Stato]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">È stato pubblicato un commento alla tua richiesta</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">È stata pubblicata una risposta alla tua richiesta di lavoro</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Qualcuno ha commentato su un argomento in cui sei presente</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Qualcuno ha commentato uno dei tuoi elementi di lavoro</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Qualcuno ha commentato una scheda orario che hai approvato</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un commento viene aggiunto alla pagina del profilo utente o modificando in blocco più utenti</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">È stato aggiunto un commento a uno degli aggiornamenti</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">È stato aggiunto un commento alla tua scheda orario</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Aggiorna notifiche {#update-notifications}

Ricevi una notifica di informazione quando viene aggiornato un elemento a cui sei associato, ma non è necessario eseguire alcuna azione sull’elemento. Dalla notifica delle informazioni, puoi eseguire le azioni seguenti:

* **[!UICONTROL Risposta]**: fare clic per rispondere all&#39;[!UICONTROL aggiornamento]. La risposta viene visualizzata anche nel flusso di aggiornamento dell&#39;elemento in Workfront.
* **Visualizza in Workfront**: selezionare questa opzione per visualizzare il commento e l&#39;elemento in Workfront, che viene aperto in una nuova scheda.
* **[!UICONTROL Stato]**: fare clic su, quindi selezionare il nuovo stato per l&#39;elemento dal menu a discesa.

#### Azioni disponibili sulle notifiche di informazioni specifiche:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notifica</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL Stato]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Viene effettuato un aggiornamento a un’attività, un problema o un progetto a cui sei abbonato</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Qualcuno ti include in un aggiornamento diretto</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Qualcuno include il tuo team in un aggiornamento diretto di [!UICONTROL]</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Notifiche di modifica data {#date-change-notifications}

Riceverai una notifica di modifica della data quando cambia la data su un elemento di lavoro a cui sei assegnato. Dalla notifica di modifica della data, puoi eseguire le azioni seguenti.

* **[!UICONTROL Commento]**: fare clic per aggiungere un commento all&#39;elemento. Il commento viene visualizzato anche nel flusso di aggiornamento dell&#39;elemento in Workfront.
* **[!UICONTROL Stato]**: fare clic su, quindi selezionare il nuovo stato per l&#39;elemento di lavoro dal menu a discesa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notifica</th> 
   <th> <p>[!UICONTROL Comment]</p> </th> 
   <th> <p>[!UICONTROL Stato]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Le modifiche della data di scadenza su un'attività a cui sei assegnato</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
