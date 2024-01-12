---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Configurazione [!DNL Adobe Workfront] per [!DNL Outlook]
description: Il [!DNL Adobe Workfront] [!DNL Outlook] componente aggiuntivo che consente di eseguire la chiave [!DNL Workfront] attività direttamente da Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 8382b69e6a55af69397dd8f566395143f3c1dcd3
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Configurazione [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

Il [!DNL Adobe Workfront] [!DNL Outlook] componente aggiuntivo consente di eseguire la chiave seguente [!DNL Workfront] attività direttamente da Outlook:

* Aggiornare un progetto, un’attività o un problema esistente con le informazioni contenute in un messaggio e-mail. Per ulteriori informazioni, consulta [Aggiornare un oggetto esistente da un [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Creare un [!DNL Workfront] richiesta basata su un messaggio e-mail entro [!DNL Outlook]. Per ulteriori informazioni, consulta [Creare una richiesta Adobe Workfront da un [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Aggiungi un messaggio e-mail come attività nel tuo [!UICONTROL Il mio lavoro] area. Per ulteriori informazioni, consulta [Aggiungi un [!DNL Outlook] invia un messaggio e-mail come attività al tuo elenco lavori](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Risposta ai commenti tramite [!DNL Workfront] componente aggiuntivo per [!DNL Outlook]. Per informazioni sulla risposta ai commenti di Workfront per [!DNL Outlook], vedi [Rispondi a un commento da [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Crea attività e problemi da zero o dalle e-mail esistenti (tramite la funzionalità di trascinamento della selezione). Per ulteriori informazioni, consulta [Aggiungi un [!DNL Outlook] inviare un messaggio e-mail a un progetto come attività o problema](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

È necessario aggiungere [!DNL Workfront] componente aggiuntivo per [!DNL Outlook] account prima di poter utilizzare [!DNL Workfront for Outlook].

Se non è possibile installare [!DNL Workfront] componente aggiuntivo con [!DNL Outlook] account, contatta il [!DNL Workfront] l&#39;amministratore per garantire che [!DNL Outlook] i componenti aggiuntivi sono abilitati per la tua organizzazione.

Per informazioni su come abilitare [!DNL Outlook] per la tua organizzazione, consulta [Abilita [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> 
   <p>Nuovo piano: [!UICONTROL Standard]</p> 
   <p>Piano corrente: [!UICONTROL Lavoro], [!UICONTROL Piano]</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisiti

Il tuo [!DNL Workfront] l&#39;amministratore deve abilitare [!DNL Outlook for Office] con [!DNL Workfront] prima di poter utilizzare questa integrazione.

## Requisiti di sistema

Sono disponibili le seguenti applicazioni:

* **[!DNL Outlook]sul Web:** Il [!DNL Workfront] il componente aggiuntivo è disponibile quando si utilizza [!DNL Outlook] da un browser web su un dispositivo desktop o mobile. Questa funzionalità è disponibile anche quando si utilizza [!DNL Outlook] App web.
* **[!DNL Outlook]Applicazione desktop:** Il [!DNL Workfront] il componente aggiuntivo è disponibile quando si utilizza [!DNL Windows] e [!DNL Mac] versioni desktop di [!DNL Outlook] in dotazione con [!DNL Office] pacchetto.

Il [!DNL Workfront] componente aggiuntivo per [!DNL Outlook] è supportato in ambienti che soddisfano i seguenti requisiti:

* [Requisiti del client](#client-requirements-client-requirements)
* [Requisiti del server di posta](#mail-server-requirements-mail-server-requirements)

### Requisiti del client {#client-requirements}

Workfront supporta le seguenti versioni di [!DNL Outlook]:

* [!DNL Outlook 2013] o più tardi [!DNL Windows]
*[!DNL  Outlook 2016] o più tardi [!DNL Windows]
* [!DNL Outlook] il [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] il [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] sul web

È necessario essere connessi a un [!DNL Exchange Server] o [!DNL Office 365] mediante una connessione diretta.

Durante la configurazione del client, l’utente deve selezionare uno dei seguenti tipi di account:

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]&#x200B;**&#x200B;**&#x200B;Se il client è configurato per la connessione con POP3 o IMAP, [!DNL Workfront] il componente aggiuntivo non si carica.

### Requisiti del server di posta {#mail-server-requirements}

I requisiti del server di posta sono soddisfatti per impostazione predefinita quando ci si connette a [!DNL Office 365] o [!DNL Outlook.com]. Tuttavia, se sei connesso a un’installazione on-premise di [!DNL Exchange Server], si applicano i seguenti requisiti:

* Workfront supporta tutti [!DNL Exchange On-Premise] server
* [!DNL Exchange Web Services] (EWS) deve essere abilitato e esposto a Internet.
* Il server deve disporre di un certificato di autenticazione valido affinché possa rilasciare token di identità validi. Nuove installazioni di [!DNL Exchange Server] includere un certificato di autenticazione predefinito.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* Per accedere al [!DNL Workfront] componente aggiuntivo da [[!DNL Office] Archivia](https://store.office.com/), i server di accesso client devono essere in grado di comunicare con  [https://store.office.com](https://store.office.com/).

Per informazioni più dettagliate sugli ambienti supportati, vedi [[!DNL Microsoft Office 365] home page](https://products.office.com/en-us/office-365-home).

## Installare il componente aggiuntivo

È possibile ottenere il componente aggiuntivo di Workfront per Outlook dal [Microsoft store](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview).

### [!DNL Workfront] per [!DNL Outlook 365] {#workfront-for-outlook-365}

1. In entrata [!DNL Outlook 365], fare clic su **[!UICONTROL Sfoglia componenti aggiuntivi]** icona ![](assets/outlook-add-in-26x26.png)nella parte superiore dell&#39;interfaccia di Office 365, quindi fare clic su **[!UICONTROL Gestione componenti aggiuntivi]**.

1. In **[!UICONTROL Cerca componenti aggiuntivi]** casella, cerca **[!DNL Workfront]** quindi premere [!UICONTROL Invio].

1. Clic **[!UICONTROL Aggiungi]**.

### [!DNL Workfront] per [!DNL Outlook] sul Web {#workfront-for-outlook-on-the-web}

1. Apri [!DNL Microsoft Outlook] in un browser web.
1. Fai clic su **[!UICONTROL Sfoglia] componenti aggiuntivi** icona ![](assets/outlook-add-in-web-version-20x20.png).

   Per individuare l’icona, consulta [Utilizzo dei componenti aggiuntivi in [!DNL Outlook] sul web](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) nella documentazione di Microsoft.

1. Cerca **[!DNL Workfront]** nel **[!UICONTROL Cerca componenti aggiuntivi]** , quindi premere **[!UICONTROL Invio]**.

1. Quando viene visualizzato nell&#39;elenco, fare clic su **Aggiungi**.

### [!DNL Workfront for Outlook] il [!UICONTROL Windows] o [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Clic **[!UICONTROL Home]** > **[!UICONTROL Archivia]** sul nastro.

1. Cerca **[!DNL Workfront]** nel **[!UICONTROL Ricerca]** , quindi premere **[!UICONTROL Invio]**.

1. Fai clic sull’interruttore per abilitare **[!UICONTROL [!DNL Workfront]componente aggiuntivo]**.

## Accedi a [!DNL Workfront] da [!DNL Outlook]

1. In entrata [!DNL Outlook], seleziona un messaggio e-mail, quindi fai clic su **[!DNL Workfront]** nell’intestazione e-mail.
1. Segui le istruzioni per accedere a [!DNL Workfront] utilizzando l’URL Enhanced Authentication, OAuth 2.0 o SAML (Security Assertion Markup Language).

   Prima che gli utenti possano accedere a [!DNL Workfront] componente aggiuntivo tramite SAML, un [!DNL Workfront] l&#39;amministratore deve prima abilitare [!DNL Office 365] componenti aggiuntivi per l’autenticazione mediante una soluzione SAML 2.0. Per ulteriori informazioni, consulta la sezione [Configura [!DNL Adobe Workfront] con SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) nell’articolo [Configura [!DNL Adobe Workfront] con SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* Quando viene richiesto di immettere il dominio del [!DNL Workfront] account, digitalo utilizzando questo formato: *yourCompany&#39;sDomain.my.workfront.com*. Il dominio della tua azienda è in genere il nome della tua azienda.
   >* L’autenticazione avanzata non è disponibile fino a quando non viene [!DNL Workfront] l&#39;amministratore consente questa integrazione.

