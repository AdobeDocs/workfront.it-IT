---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Gestisci [!DNL Adobe Workfront] notifiche in [!DNL Microsoft] Team
description: Puoi ricevere notifiche da [!DNL Adobe Workfront] informazioni sugli elementi da approvare, sulle assegnazioni assegnate o sui commenti e le modifiche agli elementi associati.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 0%

---

# Gestisci [!DNL Adobe Workfront] notifiche in [!DNL Microsoft Teams]

Puoi ricevere notifiche da [!DNL Adobe Workfront] informazioni sugli elementi da approvare, sulle assegnazioni assegnate o sui commenti e le modifiche agli elementi associati.

Queste notifiche contengono [!DNL Workfront] azioni che è possibile eseguire in [!DNL Microsoft Teams] senza allontanarsi da [!DNL Microsoft Teams] per raggiungerli.

>[!NOTE]
>
>[!DNL Microsoft Teams] non supporta più [!DNL Internet Explorer]. Per utilizzare [!DNL Adobe Workfront for Microsoft Teams integration], è necessario utilizzare un browser Web diverso da [!DNL Internet Explorer].


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

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Prerequisiti per la ricezione [!DNL Workfront] Notifiche in [!DNL Microsoft Teams]

Puoi ricevere [!DNL Workfront] notifiche in [!DNL Microsoft Teams] se sono soddisfatte le seguenti condizioni:

* Un proprietario del team ha installato e configurato [!DNL Workfront for Microsoft Teams] per il tuo team.
* Hai effettuato l’accesso a [!DNL Workfront] da [!DNL Microsoft Teams].
* Hai abilitato le notifiche istantanee in [!DNL Workfront]. Per informazioni sull’abilitazione delle notifiche istantanee, consulta [Modifica le tue notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Per informazioni sull&#39;installazione di [!DNL Workfront for Microsoft Teams] e accesso a [!DNL Workfront from Microsoft Teams], vedi [Installa [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Gestione [!DNL Workfront] Notifiche in [!DNL Microsoft Teams]

Quando [!DNL Workfront for Microsoft Teams] l&#39;app è installata, un [!DNL Workfront] canale di chat creato in [!DNL Microsoft Teams] per ogni membro di quel team. Quando viene eseguita una determinata azione in [!DNL Workfront], è possibile configurare le impostazioni per [!DNL Workfront for Microsoft Teams] per ricevere notifiche su tale azione nella [!DNL Workfront] canale di chat di [!DNL Microsoft Teams].

Quando si lavora con, considera quanto segue [!DNL Workfront] notifiche da [!DNL Microsoft Teams]:

* Non puoi ricevere tutti, ma solo un numero selezionato di [!DNL Workfront] notifiche in [!DNL Microsoft Teams].
* Tutte le notifiche ricevute da [!DNL Workfront] vengono visualizzati nel [!DNL Workfront] canale di chat bot.

  Per informazioni sull&#39;installazione di [!DNL Workfront] canale bot, consulta la [Accesso a [!DNL Workfront] da [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) sezione in [Installazione [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) articolo.

* Può trascorrere un ritardo fino a 5 minuti tra il momento in cui viene effettuato un aggiornamento in [!DNL Workfront] e quando ricevi la notifica su di esso in [!DNL Microsoft Teams].
* Per ogni [!DNL Microsoft Teams] notifica, ricevi anche una notifica e-mail.

Per gestire [!DNL Workfront] notifiche che puoi ricevere in [!DNL Microsoft Teams]:

1. Fai clic su **[!UICONTROL Altro aggiunto]** (tre punti) nella barra di navigazione a sinistra di [!DNL Microsoft Teams].

1. Clic [!DNL Workfront] nell&#39;elenco visualizzato.
1. Seleziona la **[!UICONTROL Impostazioni]** scheda.

   ![](assets/ms-teams-settings-tab-350x552.png)

1. Disattiva le notifiche che non desideri ricevere. Puoi abilitare o disabilitare gruppi di notifiche, ad esempio notifiche di informazione o di approvazione, oppure gestire le notifiche singolarmente.

   Tutte le notifiche sono abilitate per impostazione predefinita.

   Impostazioni delle notifiche per [!DNL Workfront for Microsoft] I team vengono salvati automaticamente.

   >[!NOTE]
   >
   >Non è possibile aggiungere altre notifiche a quelle disponibili per impostazione predefinita.

## Risposta a [!DNL Workfront] Notifiche e richieste di approvazione in [!DNL Microsoft Teams]

1. Accedi a [!DNL Workfront] da [!DNL Microsoft Teams].\
   Per informazioni sull&#39;accesso a [!DNL Workfront], vedi [Installa [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Vai a **[!UICONTROL Chat]** e fare clic sul pulsante **[!DNL Workfront]** canale bot.\
   Questo canale è per la tua chat personale con [!DNL Workfront] bot. Tutti [!DNL Workfront] le notifiche vengono visualizzate qui.
1. A seconda del tipo di notifica che ricevi, procedi alla sezione pertinente:

   * [Notifiche di approvazione](#approval-notifications-approval-notifications)
   * [Notifiche di assegnazione](#assignment-notifications-assignment-notifications)
   * [Notifiche di commenti](#comment-notifications-comment-notifications)
   * [Aggiorna notifiche](#update-notifications-update-notifications)
   * [Notifiche di modifica data](#date-change-notifications-date-change-notifications)

### Notifiche di approvazione {#approval-notifications}

Si ricevono notifiche di approvazione quando viene richiesto di approvare un oggetto, ad esempio un&#39;attività, una scheda orario o una bozza. È comunque possibile aggiungere un commento alla notifica.Dalla notifica di approvazione, è possibile eseguire le azioni seguenti:

* **[!UICONTROL Approva]**: Fare clic per approvare l&#39;elemento.
* **[!UICONTROL Cambia]**: fare clic per approvare l&#39;elemento con le modifiche.
* **[!UICONTROL Rifiuta]**: Fare clic per rifiutare l&#39;elemento.
* **[!UICONTROL Commento]**: fai clic su per aggiungere un commento. Il commento viene visualizzato anche in [!DNL Workfront] come aggiornamento dell’oggetto che sta alla base della notifica.
* **[!UICONTROL Vai alla bozza]**: fai clic su per aprire la bozza. Puoi quindi prendere una decisione direttamente nella bozza. Per ulteriori informazioni, consulta [Decidi su una bozza nel visualizzatore di bozze](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

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

* **[!UICONTROL Lavoraci]**: seleziona per confermare il lavoro sull’elemento. Viene visualizzata brevemente una notifica per confermare che un nuovo elemento è stato aggiunto all’elenco di lavoro.
* **[!UICONTROL Visualizza in[!DNL Workfront]]**: seleziona per visualizzare il problema o l’attività assegnati in Workfront, aprendo una nuova scheda.
* **[!UICONTROL Inizio]**: consente di iniziare a lavorare sull&#39;elemento. Viene visualizzata brevemente una notifica per confermare che un nuovo elemento è stato aggiunto all’elenco di lavoro.
* **[!UICONTROL Commento]**: consente di aggiungere un commento all&#39;elemento. Il commento viene visualizzato anche nel flusso di aggiornamento dell&#39;elemento in Workfront.
* **[!UICONTROL Stato]**: fai clic su, quindi seleziona il nuovo stato dell’elemento di lavoro dal menu a discesa.

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

* **Reply**: fai clic per rispondere al commento o [!UICONTROL aggiorna]. La risposta viene visualizzata anche nel flusso di aggiornamento in cui il commento viene visualizzato in Workfront.
* **[!UICONTROL Visualizza in Workfront]**: seleziona per visualizzare il commento e l’elemento in Workfront, che viene aperto in una nuova scheda.
* **[!UICONTROL Stato]**: fai clic su, quindi seleziona un nuovo stato per l’elemento di lavoro oggetto del commento o dell’aggiornamento.

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

* **[!UICONTROL Rispondi]**: fai clic per rispondere al [!UICONTROL aggiorna]. La risposta viene visualizzata anche nel flusso di aggiornamento dell&#39;elemento in Workfront.
* **Visualizza in Workfront**: seleziona per visualizzare il commento e l’elemento in Workfront, che viene aperto in una nuova scheda.
* **[!UICONTROL Stato]**: fai clic su, quindi seleziona il nuovo stato dell’elemento dal menu a discesa.

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

* **[!UICONTROL Commento]**: consente di aggiungere un commento all&#39;elemento. Il commento viene visualizzato anche nel flusso di aggiornamento dell&#39;elemento in Workfront.
* **[!UICONTROL Stato]**: fai clic su, quindi seleziona il nuovo stato dell’elemento di lavoro dal menu a discesa.

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
