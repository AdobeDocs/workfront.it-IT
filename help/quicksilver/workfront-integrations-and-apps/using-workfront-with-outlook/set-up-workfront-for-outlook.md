---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Configurazione [!DNL Adobe Workfront] per [!DNL Outlook]
description: Adobe Workfront Fusion offre un'integrazione con Outlook. Questo articolo descrive come iniziare a utilizzare questa integrazione nei flussi di lavoro.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 16acba0f1981b75ca141a36d096fb6f5d37c40d1
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 0%

---

# Configurazione [!DNL Adobe Workfront for Outlook]

La [!DNL Adobe Workfront] [!DNL Outlook] add-in consente di eseguire la seguente chiave [!DNL Workfront] attività direttamente da Outlook:

* Aggiorna un progetto, un&#39;attività o un problema esistente con le informazioni di un&#39;e-mail. Per ulteriori informazioni, consulta [Aggiornare un oggetto esistente da un [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Crea un [!DNL Workfront] in base a un&#39;e-mail all&#39;interno di [!DNL Outlook]. Per ulteriori informazioni, consulta [Creare una richiesta Adobe Workfront da un [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Aggiungi un’e-mail come attività nel tuo [!UICONTROL Il mio lavoro] area. Per ulteriori informazioni, consulta [Aggiungi un [!DNL Outlook] invia un&#39;e-mail come attività all&#39;elenco di lavoro](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Risposta ai commenti tramite il [!DNL Workfront] add-in per [!DNL Outlook]. Per informazioni sulla risposta ai commenti di Workfront per [!DNL Outlook], vedi [Risposta a un commento da [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Crea attività e problemi da zero o creali da e-mail esistenti (utilizzando la funzionalità di trascinamento della selezione). Per ulteriori informazioni, consulta [Aggiungi un [!DNL Outlook] invia un’e-mail a un progetto come attività o come problema](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

È necessario aggiungere la [!DNL Workfront] componente aggiuntivo [!DNL Outlook] account prima di utilizzare [!DNL Workfront for Outlook].

Se non riesci a installare il [!DNL Workfront] componenti aggiuntivi con [!DNL Outlook] account, contatta il tuo [!DNL Workfront] amministratore per garantire che [!DNL Outlook] i componenti aggiuntivi sono abilitati per la tua organizzazione.

Per informazioni su come abilitare il [!DNL Outlook] integrazione per la tua organizzazione, consulta [Abilita [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

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

## Prerequisiti

Le [!DNL Workfront] l&#39;amministratore deve abilitare [!DNL Outlook for Office] con [!DNL Workfront] prima di poter utilizzare questa integrazione.

## Requisiti di sistema

Sono disponibili le seguenti applicazioni:

* **[!DNL Outlook]sul Web:** La [!DNL Workfront] add-in è disponibile quando si utilizza [!DNL Outlook] da un browser web su un desktop o su un dispositivo mobile. Questa funzionalità è disponibile anche quando si utilizza la funzione [!DNL Outlook] App web.
* **[!DNL Outlook]Applicazione desktop:** La [!DNL Workfront] il componente aggiuntivo è disponibile quando si utilizza il [!DNL Windows] e [!DNL Mac] versioni desktop di [!DNL Outlook] incluso con [!DNL Office] pacchetto.

La [!DNL Workfront] add-in per [!DNL Outlook] è supportato in ambienti che soddisfano i seguenti requisiti:

* [Requisiti del cliente](#client-requirements-client-requirements)
* [Requisiti del server di posta](#mail-server-requirements-mail-server-requirements)

### Requisiti del cliente {#client-requirements}

Supportiamo le seguenti versioni di [!DNL Outlook]:

* [!DNL Outlook 2013] o successivamente [!DNL Windows]
*[!DNL  Outlook 2016] o successivamente [!DNL Windows]
* [!DNL Outlook] su [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] su [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] sul web

È necessario essere connessi a un [!DNL Exchange Server] o [!DNL Office 365] mediante una connessione diretta.

Durante la configurazione del client, l&#39;utente deve selezionare uno dei seguenti tipi di account:

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]&#x200B;**&#x200B;**&#x200B; Se il client è configurato per la connessione con POP3 o IMAP, la [!DNL Workfront] add-in non viene caricato.

### Requisiti del server di posta {#mail-server-requirements}

I requisiti del server di posta vengono soddisfatti per impostazione predefinita quando ci si connette a [!DNL Office 365] o [!DNL Outlook.com]. Tuttavia, se sei connesso a un’installazione on-premise di [!DNL Exchange Server], si applicano i seguenti requisiti:

* Noi sosteniamo [!DNL Exchange 2016 On-Premise]
* [!DNL Exchange Web Services] (EWS) deve essere abilitato e deve essere esposto a Internet.
* Affinché il server possa emettere token di identità validi, è necessario che il server disponga di un certificato di autenticazione valido. Nuovi impianti di [!DNL Exchange Server] includere un certificato di autenticazione predefinito.

   Per ulteriori informazioni, consulta [Certificati digitali e cifratura in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) e [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).

* Per accedere al [!DNL Workfront] componente aggiuntivo da [[!DNL Office] Store](https://store.office.com/), i server di accesso client devono essere in grado di comunicare con  [https://store.office.com](https://store.office.com/).

Per informazioni più dettagliate sugli ambienti supportati, consulta la sezione [[!DNL Microsoft Office 365] home page](https://products.office.com/en-us/office-365-home).

## Installare il componente aggiuntivo

Per ulteriori informazioni sulla configurazione della [!DNL Workfront] add-in per [!DNL Outlook], vedi [[!DNL Workfront] - Gestione collaborativa del lavoro.](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview)

* [[!DNL Workfront] per [!DNL Outlook 365]](#workfront-for-outlook-365-workfront-for-outlook-365)
* [[!DNL Workfront] per [!DNL Outlook] sul Web](#workfront-for-outlook-on-the-web-workfront-for-outlook-on-the-web)
* [[!DNL Workfront] per [!DNL Outlook] su [!DNL Windows] o [!DNL Mac]](#workfront-for-outlook-on-windows-or-mac-workfront-for-outlook-on-windows-or-mac)

### [!DNL Workfront] per [!DNL Outlook 365] {#workfront-for-outlook-365}

1. In [!DNL Outlook 365], fai clic su **[!UICONTROL Sfoglia componenti aggiuntivi]** icona ![](assets/outlook-add-in-26x26.png)nella parte superiore dell&#39;interfaccia di Office 365, quindi fai clic su **[!UICONTROL Gestire i componenti aggiuntivi]**.

1. In **[!UICONTROL Ricerca di componenti aggiuntivi]** casella, cerca **[!DNL Workfront]** quindi premere [!UICONTROL Invio].

1. Fai clic su **[!UICONTROL Aggiungi]**.

### [!DNL Workfront] per [!DNL Outlook] sul Web {#workfront-for-outlook-on-the-web}

1. Apri [!DNL Microsoft Outlook] in un browser web.
1. Fai clic sul pulsante **[!UICONTROL Sfoglia] componenti aggiuntivi** icona ![](assets/outlook-add-in-web-version-20x20.png).

   Per individuare l’icona, vedi [Utilizzo dei componenti aggiuntivi in [!DNL Outlook] sul web](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) nella documentazione di Microsoft.

1. Cerca **[!DNL Workfront]** in **[!UICONTROL Ricerca di componenti aggiuntivi]** campo, quindi premere **[!UICONTROL Invio]**.

1. Quando viene visualizzato nell’elenco, fai clic su **Aggiungi**.

### [!DNL Workfront for Outlook] su [!UICONTROL Windows] o [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Fai clic su **[!UICONTROL Pagina principale]** > **[!UICONTROL Store]** sul nastro.

1. Cerca **[!DNL Workfront]** in **[!UICONTROL Ricerca]** campo, quindi premere **[!UICONTROL Invio]**.

1. Fai clic sull’interruttore per abilitare il **[!UICONTROL [!DNL Workfront]add-in]**.

## Accedi a [!DNL Workfront] da [!DNL Outlook]

1. In [!DNL Outlook], seleziona un messaggio e-mail, quindi fai clic sul pulsante **[!DNL Workfront]** nell’intestazione e-mail.
1. Segui le istruzioni per accedere a [!DNL Workfront] utilizzando l’URL SAML (Enhanced Authentication, OAuth 2.0 o Security Assertion Markup Language).

   Prima che gli utenti possano accedere al [!DNL Workfront] add-in utilizzando SAML, un [!DNL Workfront] l&#39;amministratore deve prima abilitare [!DNL Office 365] componenti aggiuntivi per l&#39;autenticazione tramite una soluzione SAML 2.0. Per ulteriori informazioni, consulta la sezione . [Configura [!DNL Adobe Workfront] con SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) nell&#39;articolo [Configura [!DNL Adobe Workfront] con SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* Quando viene richiesto di accedere al dominio del [!DNL Workfront] account, digitare il formato: *la tua azienda&#39;sDomain.my.workfront.com*. Il dominio della tua azienda è in genere il nome della tua azienda.
   >* L’autenticazione avanzata non è disponibile finché non viene [!DNL Workfront] l&#39;amministratore lo abilita per questa integrazione.


