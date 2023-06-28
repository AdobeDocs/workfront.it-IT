---
product-area: workfront-integrations
keywords: google,documento,documento,foglio,diapositiva
navigation-topic: workfront-for-g-suite
title: Gestisci [!DNL Adobe Workfront] dettagli delle notifiche da G Suite
description: In G Suite, quando apri un Adobe e-mail di notifica [!DNL Workfront] ha inviato, è possibile visualizzare i dettagli dell'elemento di lavoro associato e rispondere senza uscire dalla Posta in arrivo. Se sono disponibili azioni, ad esempio l'approvazione di una richiesta, è possibile eseguirle direttamente da Workfront for G Suite.
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 1%

---

# Gestisci [!DNL Adobe Workfront] dettagli notifica da [!DNL G Suite]

>[!NOTE]
>
>La versione più recente del plug-in Adobe Workfront per Google è stata rilasciata il 26 giugno 2023.

In entrata [!DNL G Suite], quando si apre un messaggio e-mail di notifica [!DNL Adobe Workfront] inviato, è possibile visualizzare i dettagli dell&#39;elemento di lavoro associato e rispondere senza uscire [!UICONTROL Casella in entrata]. Se sono disponibili azioni, ad esempio l&#39;approvazione di una richiesta, è possibile eseguirle direttamente da [!DNL Workfront for G Suite].

>[!NOTE]
>
> [!DNL Workfront for G Suite] supporta quasi tutti i tipi di notifiche e-mail che è possibile ricevere da [!DNL Workfront] circa 120 tipi diversi. [!UICONTROL Riepilogo giornaliero] e-mail inviate da [!DNL Workfront] non compaiono in [!DNL Workfront for G Suite]. Per informazioni su [!DNL Workfront] tipi di notifiche e-mail, vedi [Attiva o disattiva le notifiche degli eventi](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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

## Prerequisiti

Prima di poter gestire i dettagli delle notifiche da [!DNL G Suite], è necessario

* Installa [!DNL Workfront for G suite]\
   Per istruzioni, consulta [Installa [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Gestisci [!DNL Adobe Workfront] dettagli notifica da [!DNL G Suite]

1. Se il [!DNL Workfront for G Suite] non viene visualizzato, fare clic sul pulsante [!DNL Workfront] icona ![](assets/wf-lion-icon.png) nel [!DNL G Suite] barra laterale dei componenti aggiuntivi all’estrema destra della pagina.
1. In entrata [!DNL G Suite], apri un [!DNL Workfront] e-mail di notifica.
1. Clic **[!UICONTROL Visualizza tutti gli aggiornamenti]** se viene visualizzato nella parte superiore del pannello.
1. Clic **[!UICONTROL Dettagli]**.
1. Fai clic su una delle opzioni disponibili.

   Le opzioni che potrebbero essere visualizzate sono correlate al tipo di notifica e-mail aperta. Ad esempio, se si tratta di una notifica e-mail che richiede l’approvazione di un’attività, viene visualizzato **[!UICONTROL Approva]** e **[!UICONTROL Rifiuta]** invece di opzioni quali **[!UICONTROL Lavoraci]** o **[!UICONTROL Fine]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Tipo di notifica e-mail</th> 
      <th>Azione</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Attività o problema</td> 
      <td><strong>[!UICONTROL Approva]</strong> it, <strong>[!UICONTROL rifiuta]</strong> it, <strong>[!UICONTROL Grant]</strong> l'accesso, <strong>[!UICONTROL Ignora]</strong> una richiesta di accesso, <strong>[!UICONTROL Lavoraci]</strong>, oppure fai clic su un’opzione per indicare che <strong>[!UICONTROL completato]</strong> con esso</td> 
     </tr> 
     <tr> 
      <td>Progetto</td> 
      <td><strong>[!UICONTROL Approva]</strong> it, <strong>[!UICONTROL rifiuta]</strong> it, <strong>[!UICONTROL Grant]</strong> l'accesso ad essa, o <strong>[!UICONTROL Ignora]</strong> una richiesta di accesso</td> 
     </tr> 
     <tr> 
      <td>Documento</td> 
      <td><strong>[!UICONTROL Approva]</strong> it, <strong>[!UICONTROL rifiuta]</strong> it, <strong>[!UICONTROL Grant]</strong> l'accesso ad essa, o <strong>[!UICONTROL Ignora]</strong> una richiesta di accesso</td> 
     </tr> 
     <tr> 
      <td>Aggiorna </td> 
      <td> <p>Visualizzare una parte qualsiasi dell'intero elenco di aggiornamenti per l'elemento in modo da disporre del contesto necessario <strong>[!UICONTROL Post]</strong> un nuovo aggiornamento o un <strong>[!UICONTROL Reply]</strong>. Puoi fare clic su <strong>[!UICONTROL Notify]</strong> per avvisare determinati utenti della tua risposta. </p> <p>Per ulteriori informazioni, consulta <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Rispondi a [!DNL Adobe Workfront] notifica di aggiornamento da [!DNL G Suite]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Richiesta di approvazione</td> 
      <td><strong>[!UICONTROL Approva]</strong> o <strong>[!UICONTROL rifiuta]</strong> (puoi cambiare idea facendo clic sull’altra opzione), scaricala, visualizzane il proprietario o visualizzane il numero di riferimento</td> 
     </tr> 
     <tr> 
      <td>Modifica dello stato di un progetto</td> 
      <td> Visualizza tutte le informazioni correnti sul progetto, compresi eventuali moduli personalizzati. </td> 
     </tr> 
    </tbody> 
   </table>
