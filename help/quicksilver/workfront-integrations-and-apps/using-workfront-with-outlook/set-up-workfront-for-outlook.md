---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Configura [!DNL Adobe Workfront] per [!DNL Outlook]
description: Il componente aggiuntivo  [!DNL Adobe Workfront] [!DNL Outlook] consente di eseguire le attività chiave [!DNL Workfront]  direttamente da Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---

# Configura [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>Microsoft [È in corso la disabilitazione del supporto per i token online di Exchange legacy](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), attualmente utilizzati dal componente aggiuntivo di Workfront Outlook per l&#39;autenticazione. Questa modifica di Microsoft ha già iniziato a interessare i clienti e continuerà a essere implementata in più fasi fino a ottobre 2025.
>
>* **Dopo la completa disattivazione di questi token da parte di Microsoft, l&#39;integrazione di Workfront per Microsoft Outlook non funzionerà più.**
>
>Come parte di questa modifica, Microsoft ha deciso di cambiare il modo in cui i token vengono riabilitati. Dopo il **30 giugno 2025**, gli amministratori non saranno più in grado di riabilitare i token personalmente. Solo il supporto Microsoft può concedere eccezioni. **Il 1° ottobre 2025, i token legacy verranno disattivati per tutti i tenant. Le eccezioni non verranno concesse.**

Il componente aggiuntivo [!DNL Adobe Workfront] [!DNL Outlook] consente di eseguire le seguenti attività chiave [!DNL Workfront] direttamente da Outlook:

* Aggiornare un progetto, un’attività o un problema esistente con le informazioni contenute in un messaggio e-mail. Per ulteriori informazioni, vedere [Aggiornare un oggetto esistente da un [!DNL Outlook] messaggio e-mail](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Crea una richiesta [!DNL Workfront] in base a un&#39;e-mail entro [!DNL Outlook]. Per ulteriori informazioni, consulta [Creare una richiesta Adobe Workfront da un [!DNL Outlook] messaggio e-mail](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Aggiungi un&#39;e-mail come attività nell&#39;area [!UICONTROL Il mio lavoro]. Per ulteriori informazioni, consulta [Aggiungere un&#39;e-mail [!DNL Outlook] come attività al tuo elenco di lavoro](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Rispondere ai commenti tramite il componente aggiuntivo [!DNL Workfront] per [!DNL Outlook]. Per informazioni sulla risposta ai commenti di Workfront per [!DNL Outlook], vedere [Risposta a un commento di [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Crea attività e problemi da zero o dalle e-mail esistenti (tramite la funzionalità di trascinamento della selezione). Per ulteriori informazioni, consulta [Aggiungere un&#39;e-mail [!DNL Outlook] a un progetto come attività o problema](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

Aggiungere il componente aggiuntivo [!DNL Workfront] all&#39;account [!DNL Outlook] prima di poter utilizzare [!DNL Workfront for Outlook].

Se non riesci a installare il componente aggiuntivo [!DNL Workfront] con il tuo account [!DNL Outlook], contatta l&#39;amministratore [!DNL Workfront] per assicurarti che [!DNL Outlook] componenti aggiuntivi siano abilitati per la tua organizzazione.

Per informazioni su come abilitare l&#39;integrazione di [!DNL Outlook] per l&#39;organizzazione, vedere [Abilita [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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

+++

## Prerequisiti

L&#39;amministratore di [!DNL Workfront] deve abilitare [!DNL Outlook for Office] con [!DNL Workfront] prima di poter utilizzare questa integrazione.

## Requisiti di sistema

Sono disponibili le seguenti applicazioni:

* **[!DNL Outlook]sul Web:** Il componente aggiuntivo [!DNL Workfront] è disponibile quando si utilizza [!DNL Outlook] da un browser Web su un dispositivo desktop o mobile. Questa funzionalità è disponibile anche quando si utilizza l&#39;app Web [!DNL Outlook].
* Applicazione desktop **[!DNL Outlook]:** Il componente aggiuntivo [!DNL Workfront] è disponibile quando si utilizzano le versioni desktop [!DNL Windows] e [!DNL Mac] di [!DNL Outlook] incluse nel pacchetto [!DNL Office].

Il componente aggiuntivo [!DNL Workfront] per [!DNL Outlook] è supportato in ambienti che soddisfano i seguenti requisiti:

* [Requisiti del client](#client-requirements-client-requirements)
* [Requisiti del server di posta](#mail-server-requirements-mail-server-requirements)

### Requisiti del client {#client-requirements}

Workfront supporta le seguenti versioni di [!DNL Outlook]:

* [!DNL Outlook 2013] o versione successiva il [!DNL Windows]
* [!DNL Outlook 2016] o versione successiva il [!DNL Windows]
* [!DNL Outlook] il [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] il [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] sul Web

È necessario essere connessi a [!DNL Exchange Server] o [!DNL Office 365] tramite una connessione diretta.

Durante la configurazione del client, l’utente deve selezionare uno dei seguenti tipi di account:

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com] Se il client è configurato per la connessione con POP3 o IMAP, il componente aggiuntivo [!DNL Workfront] non si carica.

### Requisiti del server di posta {#mail-server-requirements}

I requisiti del server di posta sono soddisfatti per impostazione predefinita quando ci si connette a [!DNL Office 365] o [!DNL Outlook.com]. Tuttavia, se si è connessi a un&#39;installazione locale di [!DNL Exchange Server], si applicano i seguenti requisiti:

* Workfront supporta tutti i server [!DNL Exchange On-Premise]
* [!DNL Exchange Web Services] (EWS) deve essere abilitato e esposto a Internet.
* Il server deve disporre di un certificato di autenticazione valido affinché possa rilasciare token di identità validi. Le nuove installazioni di [!DNL Exchange Server] includono un certificato di autenticazione predefinito.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* Per accedere al componente aggiuntivo [!DNL Workfront] da [[!DNL Office] Store](https://store.office.com/), i server di accesso client devono essere in grado di comunicare con [https://store.office.com](https://store.office.com/).

Per informazioni più dettagliate sugli ambienti supportati, consulta la [[!DNL Microsoft Office 365] home page](https://products.office.com/en-us/office-365-home).

## Installare il componente aggiuntivo

È possibile ottenere il componente aggiuntivo di Workfront per Outlook da [Microsoft store](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview).

### [!DNL Workfront] per [!DNL Outlook 365] {#workfront-for-outlook-365}

1. In [!DNL Outlook 365], fai clic sull&#39;icona **[!UICONTROL Sfoglia componenti aggiuntivi]** ![Sfoglia componenti aggiuntivi](assets/outlook-add-in-26x26.png)nella parte superiore dell&#39;interfaccia di Office 365, quindi fai clic su **[!UICONTROL Gestisci componenti aggiuntivi]**.

1. Nella casella **[!UICONTROL Cerca componenti aggiuntivi]**, cerca **[!DNL Workfront]**, quindi premi [!UICONTROL Invio].

1. Fare clic su **[!UICONTROL Aggiungi]**.

### [!DNL Workfront] per [!DNL Outlook] sul Web {#workfront-for-outlook-on-the-web}

1. Apri [!DNL Microsoft Outlook] in un browser Web.
1. Fai clic sull&#39;icona **[!UICONTROL Sfoglia] componenti aggiuntivi** ![Sfoglia componenti aggiuntivi](assets/outlook-add-in-web-version-20x20.png).

   Per individuare l&#39;icona, vedere [Utilizzo di componenti aggiuntivi in [!DNL Outlook] sul Web](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) nella documentazione di Microsoft.

1. Cerca **[!DNL Workfront]** nel campo **[!UICONTROL Cerca componenti aggiuntivi]**, quindi premi **[!UICONTROL Invio]**.

1. Quando viene visualizzato nell&#39;elenco, fare clic su **Aggiungi**.

### [!DNL Workfront for Outlook] su [!UICONTROL Windows] o [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Fai clic su **[!UICONTROL Home]** > **[!UICONTROL Store]** sulla barra multifunzione.

1. Cerca **[!DNL Workfront]** nel campo **[!UICONTROL Cerca]**, quindi premi **[!UICONTROL Invio]**.

1. Fare clic sull&#39;interruttore per abilitare il componente aggiuntivo **[!UICONTROL [!DNL Workfront]]**.

## Accedi a [!DNL Workfront] da [!DNL Outlook]

1. In [!DNL Outlook], selezionare un messaggio di posta elettronica, quindi fare clic sull&#39;icona **[!DNL Workfront]** nell&#39;intestazione dell&#39;e-mail.
1. Nella pagina di accesso, fare clic su **Accedi a Workfront**.
1. Segui le istruzioni per accedere a [!DNL Workfront] utilizzando OAuth 2.0. <!--Enhanced Authentication or your Security Assertion Markup Language (SAML) URL.-->

   <!--Before users can log in to the [!DNL Workfront] add-in using SAML, a [!DNL Workfront] administrator must first enable [!DNL Office 365] add-ins to authenticate using a SAML 2.0 solution. For more information, see the section [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) in the article [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).-->

   >[!NOTE]
   >
   >* Se viene richiesto di immettere il dominio dell&#39;account [!DNL Workfront], digitarlo in questo formato: *yourCompany&#39;sDomain.my.workfront.com*. Il dominio della tua azienda è in genere il nome della tua azienda.

<!--ADDITIONAL BULLET REMOVED FROM NOTE BOX: Enhanced Authentication is not available until a Workfront administrator enables it for this integration.-->
