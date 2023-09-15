---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Ricezione [!DNL Adobe Workfront] notifiche in [!DNL Slack]
description: Ricezione [!DNL Adobe Workfront] notifiche in [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 6%

---

# Ricezione [!DNL Adobe Workfront] notifiche in [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

Dopo aver installato [!DNL Adobe Workfront for Slack], puoi ricevere [!DNL Workfront] notifiche in [!DNL Slack].\
Per informazioni sull&#39;installazione di [!DNL Workfront for Slack], vedi [Configura [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

È possibile abilitare un numero selezionato di [!UICONTROL notifiche] che compaiono nel fumetto delle notifiche nella [!DNL Workfront] , da distribuire anche in [!DNL Slack].

Le notifiche e-mail funzionano indipendentemente da [!DNL Workfront] notifiche di interfaccia. Tu o il tuo [!DNL Workfront] l’amministratore può disabilitare le notifiche e-mail, mentre le notifiche dell’interfaccia non possono essere disabilitate in [!DNL Workfront].\
Tuttavia, puoi disattivare [!DNL Workfront] notifiche che potresti ricevere in [!DNL Slack], se desideri concentrarti su tali notifiche solo all&#39;interno del [!DNL Workfront] di rete.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] piano]</a>*</td> 
   <td> <p>[!UICONTROL Pro] o versione successiva</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.\

## Prerequisiti

Prima di ricevere [!DNL Workfront] notifiche in [!DNL Slack], è necessario

* Configura [!DNL Workfront for Slack]\
   Per istruzioni sulla configurazione [!DNL Workfront for Slack], vedi [Configura [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Configura [!DNL Workfront] notifiche per [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (Condizionale) Dopo [!DNL Workfront] è stato aggiunto al tuo [!DNL Slack] istanza, accesso [!DNL Workfront] da [!DNL Slack].\
   Per informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], vedi [Accesso [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Da qualsiasi canale, inizia a digitare uno dei seguenti comandi nel campo del messaggio:

   `/workfront settings`

   Oppure

   `/wf settings`

1. Per impostazione predefinita, tutte le notifiche sono abilitate.\
   Disattiva una delle notifiche seguenti:

   * [!UICONTROL Quando si cambia l&#39;incaricato di un&#39;attività o un problema, invia una Email all&#39;incaricato]
   * [!UICONTROL Il mio team è assegnato a una nuova attività o problema]
   * [!UICONTROL Ricevo una nuova approvazione o richiesta di accesso]
   * [!UICONTROL Qualcuno mi include in un aggiornamento diretto]
   * [!UICONTROL Qualcuno ha commentato su un argomento che mi interessa]
   * [!UICONTROL Viene effettuato un aggiornamento a un&#39;attività, un problema o un progetto al quale sono iscritto]
   * [!UICONTROL Qualcuno ha commentato uno degli elementi del mio lavoro]
   * [!UICONTROL Qualcuno ha commentato la mia richiesta di aiuto]

   Le modifiche apportate al [!UICONTROL notifiche] le opzioni hanno effetto immediato.\
   Le notifiche abilitate vengono consegnate in [!DNL Workfront] [!DNL Slack] canale. Quando disattivi le notifiche qui, vengono disattivate solo per [!DNL Slack], e non per [!DNL Workfront] di rete. Continui a riceverli in [!DNL Workfront] bolla di notifica in alto a destra nell’interfaccia.

## Gestisci [!DNL Workfront] notifiche da [!DNL Slack]

Puoi ricevere e rispondere a [!DNL Workfront] notifiche da [!DNL Slack].

Puoi disattivare le notifiche e-mail per le notifiche abilitate in [!DNL Slack], per evitare di ricevere notifiche duplicate.\
Per informazioni sulla configurazione delle notifiche e-mail, consulta [Modifica le tue notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Attivazione o disattivazione [!DNL Workfront] notifiche in [!DNL Slack] non influisce sulle notifiche ricevute all&#39;interno del [!DNL Workfront] di rete.\
Notifiche all&#39;interno di [!DNL Workfront] l&#39;interfaccia non può essere disabilitata.

Per gestire [!DNL Workfront] notifiche per [!DNL Slack]:

1. Accedi a [!UICONTROL Slack].
1. Accedi a [!DNL Workfront] da [!DNL Slack].\
   Per informazioni sull&#39;accesso a [!DNL Workfront] da [!DNL Slack], consulta &quot;Accesso a [!DNL Workfront] da [!DNL Slack]&quot; sezione in [Accesso [!DNL Adobe Workfront] da [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Assicurati che il tuo [!DNL Workfront] notifiche per [!DNL Slack] sono attivati.\
   Per ulteriori informazioni su quali [!DNL Workfront] è possibile configurare le notifiche per l’invio anche a [!DNL Slack], vedi [Configura [!DNL Workfront] notifiche per [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. Vai a **[!DNL Workfront]** canale per trovare il tuo [!DNL Workfront] notifiche.
1. (Condizionale e facoltativo) Effettua una delle seguenti operazioni:

   * Clic **[!UICONTROL Lavoraci]** per accettare di lavorare su un&#39;attività.

   * (Condizionale e facoltativo) Fai clic su **[!UICONTROL Rispondi in[!DNL Workfront]]** per rispondere a un commento, digitare la risposta e fare clic su **[!UICONTROL Rispondi]**.

   * (Condizionale e facoltativo) Fai clic su **[!UICONTROL Approva]** o **[!UICONTROL Rifiuta]** per approvare o rifiutare un&#39;attività, un problema o un progetto in attesa di approvazione.

   * (Condizionale e facoltativo) Fai clic su **[!UICONTROL Approva]**, **[!UICONTROL Modifiche]**, o **[!UICONTROL Rifiuta]**, per approvare, approvare con modifiche o rifiutare un documento.

     È inoltre possibile passare il puntatore del mouse sulla miniatura del documento e fare clic sull&#39;icona della lente di ingrandimento per visualizzare un&#39;anteprima più grande del documento prima di approvarlo.\
      Solo lo Slack approvato [tipi di file](https://api.slack.com/types/file) possono essere visualizzate in anteprima.

   * (Condizionale e facoltativo) Fai clic su **[!UICONTROL Concedi]** o **[!UICONTROL Ignora]** per concedere o ignorare la richiesta di accesso aggiuntivo da parte di un altro utente.\

     Ricevi una conferma del completamento dell’azione in [!DNL Workfront], per ogni decisione presa all&#39;interno delle notifiche.
