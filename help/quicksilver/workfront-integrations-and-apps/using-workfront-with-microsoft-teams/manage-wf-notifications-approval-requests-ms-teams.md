---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Gestisci [!DNL Adobe Workfront] notifiche in [!DNL Microsoft] Team
description: Puoi ricevere notifiche da [!DNL Adobe Workfront] informazioni sugli elementi da approvare, sulle assegnazioni assegnate o sui commenti e sulle modifiche apportate agli elementi associati.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '1279'
ht-degree: 0%

---

# Gestisci [!DNL Adobe Workfront] notifiche in [!DNL Microsoft Teams]

Puoi ricevere notifiche da [!DNL Adobe Workfront] informazioni sugli elementi da approvare, sulle assegnazioni assegnate o sui commenti e sulle modifiche apportate agli elementi associati.

Queste notifiche contengono [!DNL Workfront] azioni che puoi eseguire in [!DNL Microsoft Teams] senza allontanarsi [!DNL Microsoft Teams] per realizzarli.

>[!NOTE]
>
>[!DNL Microsoft Teams] non supporta più [!DNL Internet Explorer]. Per utilizzare [!DNL Adobe Workfront for Microsoft Teams integration], è necessario utilizzare un browser web diverso da [!DNL Internet Explorer].


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
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Prerequisiti per la ricezione [!DNL Workfront] Notifiche in [!DNL Microsoft Teams]

È possibile ricevere [!DNL Workfront] notifiche in [!DNL Microsoft Teams] se sono soddisfatte le seguenti condizioni:

* Installazione e configurazione di un proprietario del team [!DNL Workfront for Microsoft Teams] per la tua squadra.
* Accesso effettuato [!DNL Workfront] da [!DNL Microsoft Teams].
* Hai abilitato le notifiche istantanee in [!DNL Workfront]. Per informazioni sull&#39;abilitazione delle notifiche istantanee, vedi [Attivare o disattivare le notifiche degli eventi personali](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Per informazioni sull’installazione [!DNL Workfront for Microsoft Teams] e accedere a [!DNL Workfront from Microsoft Teams], vedi [Installa [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Gestione [!DNL Workfront] Notifiche in [!DNL Microsoft Teams]

Quando il [!DNL Workfront for Microsoft Teams] l&#39;app è installata, [!DNL Workfront] il canale chat viene creato in [!DNL Microsoft Teams] per ogni membro della squadra. Quando viene eseguita una determinata azione in [!DNL Workfront], puoi configurare le impostazioni per [!DNL Workfront for Microsoft Teams] per ricevere notifiche su tale azione nel [!DNL Workfront] canale di chat di [!DNL Microsoft Teams].

Quando si lavora con , considera quanto segue [!DNL Workfront] notifiche [!DNL Microsoft Teams]:

* Non è possibile ricevere tutti, ma solo un numero selezionato di [!DNL Workfront] notifiche in [!DNL Microsoft Teams].
* Tutte le notifiche ricevute da [!DNL Workfront] vengono visualizzate nel [!DNL Workfront] canale chat bot.

   Per informazioni sull&#39;installazione di [!DNL Workfront] canale bot, vedi [Accesso a [!DNL Workfront] da [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) sezione [Installazione [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) articolo.

* Tra il momento in cui viene effettuato un aggiornamento può trascorrere fino a 5 minuti [!DNL Workfront] e quando ricevi la notifica relativa a [!DNL Microsoft Teams].
* Per ogni [!DNL Microsoft Teams] , riceverai anche una notifica e-mail.

Per gestire [!DNL Workfront] notifiche che puoi ricevere in [!DNL Microsoft Teams]:

1. Fai clic sul pulsante **[!UICONTROL Altri]** icona delle app nella barra di navigazione a sinistra in [!DNL Microsoft Teams].

   ![](assets/ms-teams-more-added-apps-icon.png)

1. Fai clic su [!DNL Workfront] nell&#39;elenco visualizzato.
1. Seleziona la **[!UICONTROL Impostazioni]** scheda .

   ![](assets/ms-teams-settings-tab-350x552.png)

1. Disattiva le notifiche che non desideri ricevere. Puoi abilitare o disabilitare gruppi di notifiche, ad esempio informazioni o notifiche di approvazione, oppure puoi gestire le notifiche singolarmente.

   Tutte le notifiche sono abilitate per impostazione predefinita.

   Le impostazioni di notifica per [!DNL Workfront for Microsoft] I team vengono salvati automaticamente.

   >[!NOTE]
   >
   >Non puoi aggiungere altre notifiche a quelle disponibili per impostazione predefinita.

## Risposta a [!DNL Workfront] Notifiche e richieste di approvazione in [!DNL Microsoft Teams]

1. Accedi a [!DNL Workfront] da [!DNL Microsoft Teams].\
   Per informazioni sull&#39;accesso a [!DNL Workfront], vedi [Installa [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Vai a **[!UICONTROL Chat]** e fai clic su **[!DNL Workfront]** canale bot.\
   Questo canale è per la tua chat personale con [!DNL Workfront] bot. Tutto [!DNL Workfront] le notifiche vengono visualizzate qui.
1. A seconda del tipo di notifica ricevuto, procedi alla sezione pertinente:

   * [Notifiche di approvazione](#approval-notifications-approval-notifications)
   * [Notifiche di assegnazione](#assignment-notifications-assignment-notifications)
   * [Notifiche di commento](#comment-notifications-comment-notifications)
   * [Notifiche di aggiornamento](#update-notifications-update-notifications)
   * [Notifiche di modifica della data](#date-change-notifications-date-change-notifications)

### Notifiche di approvazione {#approval-notifications}

Si ricevono notifiche di approvazione quando viene richiesto di approvare un oggetto, ad esempio un&#39;attività, una scheda attività o una bozza. È comunque possibile commentare la notifica.Dalla notifica di approvazione, è possibile eseguire le seguenti azioni:

* **[!UICONTROL Approva]**: Fai clic su per approvare l’elemento.
* **[!UICONTROL Modifica]**: Fai clic su per approvare l’elemento con le modifiche.
* **[!UICONTROL Rifiuta]**: Fare clic per rifiutare l&#39;elemento.
* **[!UICONTROL Commento]**: Fai clic su per aggiungere un commento. Il commento viene visualizzato anche in [!DNL Workfront] come aggiornamento dell&#39;oggetto di cui si occupa la notifica.
* **[!UICONTROL Vai a prova]**: Fai clic su per aprire la bozza. Puoi quindi prendere una decisione direttamente nella bozza. Per ulteriori informazioni, consulta [Prendere una decisione su una bozza nel visualizzatore di correzione](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

>[!NOTE]
>
>Una volta presa una decisione di approvazione, non puoi modificarla dalla notifica.

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
   <th>[!UICONTROL Approve]</th> 
   <th>[!UICONTROL Rifiuta]</th> 
   <th> <p>[!UICONTROL Change]</p> </th> 
   <th> <p>[!UICONTROL Vai a prova] </p> </th> 
   <th>[!UICONTROL Commento]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Devi approvare un progetto</td> 
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
   <td role="rowheader">Devi approvare un problema</td> 
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
   <td role="rowheader">È necessario approvare una scheda attività</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Qualcuno vuole che lei approvi questa prova</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Scheda attività rifiutata</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">La scheda attività viene riaperta</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">È stata approvata una richiesta di approvazione del documento richiesta</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Una richiesta di approvazione del documento richiesta viene approvata con modifiche</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Richiesta di approvazione del documento rifiutata</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Scheda attività approvata</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Notifiche di assegnazione {#assignment-notifications}

Ricevi notifiche di assegnazione quando, o un team in cui ti trovi, sei assegnato a un&#39;attività o a un problema in Workfront. Dalla notifica di assegnazione è possibile eseguire le azioni seguenti:

* **[!UICONTROL Lavorare]**: Selezionare per eseguire il commit per lavorare sull&#39;elemento. Viene visualizzata brevemente una notifica per confermare l’aggiunta di un nuovo elemento all’elenco di lavoro.
* **[!UICONTROL Visualizza in[!DNL Workfront]]**: Selezionare questa opzione per visualizzare il problema o l&#39;attività assegnata in Workfront, che apre una nuova scheda.
* **[!UICONTROL Inizio]**: Fai clic su per iniziare a lavorare sull&#39;elemento. Viene visualizzata brevemente una notifica per confermare l’aggiunta di un nuovo elemento all’elenco di lavoro.
* **[!UICONTROL Commento]**: Fare clic per aggiungere un commento all&#39;elemento. Il commento viene visualizzato anche nel flusso di aggiornamento dell&#39;elemento in Workfront.
* **[!UICONTROL Stato]**: Fare clic su, quindi selezionare il nuovo stato per l&#39;elemento di lavoro dal menu a discesa.

#### Azioni disponibili per notifiche di assegnazione specifiche:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notifica</th> 
   <th>[!UICONTROL Start]</th> 
   <th>[!UICONTROL Commento]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">È assegnato a un'attività</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sei assegnato a un problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un team a cui si è assegnati riceve una richiesta di lavoro per un'attività</td> 
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

### Notifiche di commento {#comment-notifications}

Ricevi una notifica di comunicazione quando qualcuno commenta un elemento a cui sei associato o ti include in un aggiornamento. Dalla notifica di comunicazione, puoi eseguire le azioni seguenti:

* **Reply**: Fai clic per rispondere al commento o [!UICONTROL update]. La risposta viene visualizzata anche nel flusso di aggiornamento in cui il commento viene visualizzato in Workfront.
* **[!UICONTROL Visualizza in Workfront]**: Selezionare per visualizzare il commento e l&#39;elemento in Workfront, che viene aperto in una nuova scheda.
* **[!UICONTROL Stato]**: Fare clic su, quindi selezionare un nuovo stato per l&#39;elemento di lavoro di cui si occupa il commento o l&#39;aggiornamento.

#### Azioni disponibili su notifiche di comunicazione specifiche:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notifica</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Un commento è pubblicato sulla tua richiesta</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Una risposta è pubblicata sulla tua richiesta di lavoro</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Qualcuno commenta un thread in cui ti trovi</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Qualcuno commenta uno dei tuoi oggetti di lavoro</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un utente commenta una scheda attività approvata</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un commento viene aggiunto nella pagina del profilo utente o tramite modifica collettiva di più utenti</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">È stato aggiunto un commento a uno degli aggiornamenti</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nella scheda attività viene aggiunto un commento</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Notifiche di aggiornamento {#update-notifications}

Ricevi una notifica di informazioni quando si verifica un aggiornamento di un elemento a cui sei associato, ma non devi eseguire alcuna azione sull’elemento. Dalla notifica di informazioni, puoi eseguire le azioni seguenti:

* **[!UICONTROL Rispondi]**: Fai clic per rispondere al [!UICONTROL update]. La risposta viene visualizzata anche nel flusso di aggiornamento dell&#39;elemento in Workfront.
* **Visualizza in Workfront**: Selezionare per visualizzare il commento e l&#39;elemento in Workfront, che viene aperto in una nuova scheda.
* **[!UICONTROL Stato]**: Fai clic su , quindi seleziona il nuovo stato dell’elemento dal menu a discesa.

#### Azioni disponibili su notifiche di informazioni specifiche:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notifica</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Viene eseguito un aggiornamento a un'attività, un problema o un progetto a cui si è abbonati</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Qualcuno ti include in un aggiornamento diretto</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Qualcuno include il tuo team in un [!UICONTROL aggiornamento diretto]</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Notifiche di modifica della data {#date-change-notifications}

Viene visualizzata una notifica di modifica della data quando la data cambia in un elemento di lavoro a cui si è assegnati. Dalla notifica della modifica della data, puoi eseguire le seguenti azioni.

* **[!UICONTROL Commento]**: Fare clic per aggiungere un commento all&#39;elemento. Il commento viene visualizzato anche nel flusso di aggiornamento dell&#39;elemento in Workfront.
* **[!UICONTROL Stato]**: Fare clic su, quindi selezionare il nuovo stato per l&#39;elemento di lavoro dal menu a discesa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notifica</th> 
   <th> <p>[!UICONTROL Commento]</p> </th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">La data di scadenza cambia in un'attività a cui si è assegnati</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
