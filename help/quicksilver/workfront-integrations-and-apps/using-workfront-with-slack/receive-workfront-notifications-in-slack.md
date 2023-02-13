---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Ricezione [!DNL Adobe Workfront] notifiche in [!DNL Slack]
description: Ricezione [!DNL Adobe Workfront] notifiche in [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 6%

---

# Ricezione [!DNL Adobe Workfront] notifiche in [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

Dopo aver installato [!DNL Adobe Workfront for Slack], è possibile ricevere [!DNL Workfront] notifiche in [!DNL Slack].\
Per informazioni sull’installazione [!DNL Workfront for Slack], vedi [Configura [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

È possibile abilitare un numero selezionato di [!UICONTROL Notifiche] che compaiono nella bolla delle notifiche nel [!DNL Workfront] interfaccia, disponibile anche in [!DNL Slack].

Le notifiche e-mail funzionano in modo indipendente [!DNL Workfront] notifiche dell’interfaccia. Tu o il tuo [!DNL Workfront] l’amministratore può disabilitare le notifiche e-mail, mentre le notifiche dell’interfaccia non possono essere disabilitate in [!DNL Workfront].\
È tuttavia possibile disabilitare [!DNL Workfront] notifiche che potresti ricevere in [!DNL Slack], se desideri concentrarti su tali notifiche solo all’interno della [!DNL Workfront] interfaccia.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] piano]</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.\

## Prerequisiti

Prima di ricevere [!DNL Workfront] notifiche in [!DNL Slack], devi

* Configura [!DNL Workfront for Slack]\
   Per istruzioni sulla configurazione [!DNL Workfront for Slack], vedi [Configura [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Configura [!DNL Workfront] notifiche [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (Condizionale) Dopo [!DNL Workfront] è stato aggiunto al [!DNL Slack] istanza, accedere [!DNL Workfront] da [!DNL Slack].\
   Per informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], vedi [Accesso [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Da qualsiasi canale, inizia a digitare uno dei seguenti comandi nel campo messaggio:

   `/workfront settings`

   Oppure

   `/wf settings`

   <img src="assets/slack-configuring-settings-350x302.png" style="width: 350;height: 302;">

1. Per impostazione predefinita, tutte le notifiche sono abilitate.\
   Disattiva una delle seguenti notifiche:

   * [!UICONTROL Sono assegnato a un nuovo compito o problema]
   * [!UICONTROL Il team viene assegnato a una nuova attività o problema]
   * [!UICONTROL Ricevo una nuova approvazione o una nuova richiesta di accesso]
   * [!UICONTROL Qualcuno mi include in un aggiornamento diretto]
   * [!UICONTROL Qualcuno ha commentato su un argomento che mi interessa]
   * [!UICONTROL Viene effettuato un aggiornamento a un&#39;attività, un problema o un progetto al quale sono iscritto]
   * [!UICONTROL Qualcuno ha commentato uno degli elementi del mio lavoro]
   * [!UICONTROL Qualcuno commenta la mia richiesta di aiuto]

   Le modifiche apportate al [!UICONTROL Notifiche] le opzioni hanno effetto immediato.\
   Le notifiche abilitate vengono consegnate nella [!DNL Workfront] [!DNL Slack] canale. Quando disattivi le notifiche qui, vengono disabilitate solo per [!DNL Slack]e non per [!DNL Workfront] interfaccia. Continui a riceverli nel [!DNL Workfront] le notifiche si propagano in alto a destra nell&#39;interfaccia.

## Gestisci [!DNL Workfront] notifiche [!DNL Slack]

Puoi ricevere e rispondere a [!DNL Workfront] notifiche [!DNL Slack].

Puoi disabilitare le notifiche e-mail per le notifiche attivate in [!DNL Slack], per evitare di ricevere notifiche duplicate.\
Per informazioni sulla configurazione delle notifiche e-mail, consulta [Attivare o disattivare le notifiche degli eventi personali](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Abilitazione o disabilitazione [!DNL Workfront] notifiche in [!DNL Slack] non influisce sulle notifiche ricevute all’interno della [!DNL Workfront] interfaccia.\
Notifiche all’interno della [!DNL Workfront] Impossibile disabilitare l&#39;interfaccia.

Per gestire le [!DNL Workfront] notifiche [!DNL Slack]:

1. Accedi a [!UICONTROL Slack].
1. Accedi a [!DNL Workfront] da [!DNL Slack].\
   Per informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], consulta &quot;Accesso a [!DNL Workfront] da [!DNL Slack]&quot; sezione in [Accesso [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Assicurati che il tuo [!DNL Workfront] notifiche [!DNL Slack] sono abilitati.\
   Per ulteriori informazioni su quali [!DNL Workfront] le notifiche possono essere configurate in modo che vengano inviate anche a [!DNL Slack], vedi [Configura [!DNL Workfront] notifiche [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. Vai a **[!DNL Workfront]** canale per trovare il tuo [!DNL Workfront] notifiche.
1. (Condizionale e facoltativo) Effettuare una delle seguenti operazioni:

   * Fai clic su **[!UICONTROL Lavorare]** accettare di lavorare su un&#39;attività.

      <!--   
     <img src="assets/slack-assigned-to-a-task-notification-350x198.png" alt="slack_assigned_to_a_task_notification.png" style="width: 350;height: 198;" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

   * (Condizionale e facoltativo) Fai clic su **[!UICONTROL Rispondi in[!DNL Workfront]]** per rispondere a un commento, digitare la risposta e fare clic su **[!UICONTROL Rispondi]**.\

      ![slack_tagged_in_a_comment_notification.png](assets/slack-tagged-in-a-comment-notification.png)

   * (Condizionale e facoltativo) Fai clic su **[!UICONTROL Approva]** o **[!UICONTROL Rifiuta]** per approvare o rifiutare un&#39;attività, un problema o un progetto in attesa di approvazione.\

      ![slack_authorization_task_notification.png](assets/slack-approve-task-notification-350x105.png)

   * (Condizionale e facoltativo) Fai clic su **[!UICONTROL Approva]**, **[!UICONTROL Modifiche]** oppure **[!UICONTROL Rifiuta]**, per approvare, approvare con le modifiche o rifiutare un documento.\

      ![slack_authorization_a_document.png](assets/slack-approve-a-document-350x362.png)\
      È inoltre possibile passare il mouse sulla miniatura del documento e fare clic sull&#39;icona della lente di ingrandimento per visualizzare un&#39;anteprima più ampia del documento prima di approvarlo.\
      Solo lo Slack approvato [tipi di file](https://api.slack.com/types/file) può essere visualizzato in anteprima.

   * (Condizionale e facoltativo) Fai clic su **[!UICONTROL Concessione]** o **[!UICONTROL Ignora]** per concedere o ignorare la richiesta di più accesso da un altro utente.\

      ![](assets/slack-access-approvals-list-350x213.png)\
      Ricevi una conferma del completamento dell’azione in [!DNL Workfront], per ogni decisione presa nelle notifiche.
