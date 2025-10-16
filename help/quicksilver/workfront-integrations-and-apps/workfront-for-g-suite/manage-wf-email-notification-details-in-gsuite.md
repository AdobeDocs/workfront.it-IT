---
product-area: workfront-integrations
keywords: google,documento,documento,foglio,diapositiva
navigation-topic: workfront-for-g-suite
title: Gestisci [!DNL Adobe Workfront] dettagli notifica da Google Workspace
description: In Google Workspace, quando apri un messaggio e-mail di notifica inviato da Adobe [!DNL Workfront] puoi visualizzare i dettagli dell'elemento di lavoro associato e rispondere senza uscire dalla Posta in arrivo. Se sono disponibili azioni, ad esempio l’approvazione di una richiesta, è possibile eseguirle direttamente da Workfront per Google Workspace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 1%

---

# Gestisci dettagli notifica [!DNL Adobe Workfront] da [!DNL Google Workspace]

>[!IMPORTANT]
>
>Per offrire integrazioni più stabili e scalabili, stiamo passando a un approccio di integrazione moderno e flessibile che utilizza l’automazione e l’integrazione di Workfront (Fusion). Nell&#39;ambito di questo processo di transizione, le seguenti funzionalità di Workfront per Google Workspace non saranno disponibili dopo il **28 febbraio 2026**:
>
>* Accesso alle funzionalità di Google Workspace da Workfront
>
>* Visualizzazione e gestione delle attività di Workfront da Gmail o dal pannello del sito Calendario di Google
>
>È consigliabile utilizzare l&#39;automazione e l&#39;integrazione di Workfront per le esigenze di integrazione dell&#39;organizzazione con Google Workspace.
>
>Per una panoramica dell&#39;automazione e dell&#39;integrazione di Workfront, vedere [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Per informazioni sulle funzionalità specifiche dei moduli di automazione e integrazione di Workfront per Google Workspace, vedere [Moduli Gmail](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) e [Moduli calendario Google](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

In [!DNL Google Workspace], quando apri un&#39;e-mail di notifica [!DNL Adobe Workfront] inviata, puoi visualizzare i dettagli dell&#39;elemento di lavoro associato e rispondere senza uscire dalla [!UICONTROL casella in entrata]. Se sono disponibili azioni, ad esempio l&#39;approvazione di una richiesta, è possibile eseguire tali azioni direttamente da [!DNL Workfront for Google Workspace].

>[!NOTE]
>
> [!DNL Workfront for Google Workspace] supporta quasi tutti i tipi di notifiche e-mail che è possibile ricevere da [!DNL Workfront] (circa 120 tipi diversi). Le e-mail di [!UICONTROL Riepilogo giornaliero] inviate da [!DNL Workfront] non vengono visualizzate in [!DNL Workfront for Google Workspace]. Per informazioni sui tipi di notifiche e-mail [!DNL Workfront], vedere [Modificare le proprie notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p><p>Lavoro o superiore</p>
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di poter gestire i dettagli delle notifiche da [!DNL Google Workspace], è necessario

* Installa [!DNL Workfront for Google Workspace]\
   Per istruzioni, vedere [Installa [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Gestisci dettagli notifica [!DNL Adobe Workfront] da [!DNL Google Workspace]

1. Se il pannello [!DNL Workfront for Google Workspace] non è visualizzato, fai clic sull&#39;icona [!DNL Workfront] ![icona Workfront](assets/wf-lion-icon.png) nella barra laterale dei componenti aggiuntivi di [!DNL Google Workspace] all&#39;estrema destra della pagina.
1. In [!DNL Google Workspace], apri un messaggio e-mail di notifica [!DNL Workfront].
1. Fai clic su **[!UICONTROL Visualizza tutti gli aggiornamenti]** se è visualizzato nella parte superiore del pannello.
1. Fare clic su **[!UICONTROL Dettagli]**.
1. Fai clic su una delle opzioni disponibili.

   Le opzioni che potrebbero essere visualizzate sono correlate al tipo di notifica e-mail aperta. Ad esempio, se si tratta di una notifica e-mail che richiede l&#39;approvazione di un&#39;attività, verranno visualizzati **[!UICONTROL Approva]** e **[!UICONTROL Rifiuta]** anziché opzioni quali **[!UICONTROL Lavoraci]** o **[!UICONTROL Fine]**:

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
      <td><strong>[!UICONTROL Approva]</strong>, <strong>[!UICONTROL Rifiuta]</strong>, <strong>[!UICONTROL Concedi]</strong> l'accesso, <strong>[!UICONTROL Ignora]</strong> una richiesta di accesso, <strong>[!UICONTROL Lavoraci]</strong>, oppure fare clic su un'opzione per indicare che è <strong>[!UICONTROL Completato]</strong></td> 
     </tr> 
     <tr> 
      <td>Progetto</td> 
      <td><strong>[!UICONTROL Approva]</strong>, <strong>[!UICONTROL Rifiuta]</strong>, <strong>[!UICONTROL Concedi]</strong> l'accesso o <strong>[!UICONTROL Ignora]</strong> una richiesta per l'accesso</td> 
     </tr> 
     <tr> 
      <td>Documento</td> 
      <td><strong>[!UICONTROL Approva]</strong>, <strong>[!UICONTROL Rifiuta]</strong>, <strong>[!UICONTROL Concedi]</strong> l'accesso o <strong>[!UICONTROL Ignora]</strong> una richiesta per l'accesso</td> 
     </tr> 
     <tr> 
      <td>Aggiornamento </td> 
      <td> <p>Visualizzare una parte dell'intero elenco di aggiornamenti per l'elemento in modo da disporre del contesto necessario per <strong>[!UICONTROL Post]</strong> un nuovo aggiornamento o una <strong>[!UICONTROL Reply]</strong>. Puoi fare clic su <strong>[!UICONTROL Notify]</strong> per avvisare determinati utenti della tua risposta. </p> <p>Per ulteriori informazioni, vedere <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Risposta a una notifica di aggiornamento di [!DNL Adobe Workfront] da [!DNL Google Workspace]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Richiesta di approvazione</td> 
      <td><strong>[!UICONTROL Approva]</strong> o <strong>[!UICONTROL Rifiuta]</strong> (puoi cambiare idea facendo clic sull'altra opzione), scaricarla, visualizzarne il proprietario o visualizzarne il numero di riferimento</td> 
     </tr> 
     <tr> 
      <td>Modifica dello stato di un progetto</td> 
      <td> Visualizza tutte le informazioni correnti sul progetto, compresi eventuali moduli personalizzati. </td> 
     </tr> 
    </tbody> 
   </table>
