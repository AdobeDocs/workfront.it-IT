---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Installa [!DNL Adobe Workfront] per [!DNL Salesforce]
description: Per installare l'app prima che diventi disponibile in AppExchange [!DNL Salesforce] , consulta Installazione di Salesforce [!DNL Workfront] prima che diventi disponibile in AppExchange Marketplace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: dc72ef4a3c5d55c418330af984f146f61f202d84
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 2%

---

# Installa [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>Per offrire integrazioni più stabili e scalabili, stiamo passando a un approccio di integrazione moderno e flessibile che utilizza l’automazione e l’integrazione di Workfront (Fusion). Come parte di questo processo di transizione, l&#39;integrazione di Workfront for Salesforce non sarà disponibile dopo il **28 febbraio 2026**.
>
>È consigliabile utilizzare l’automazione e l’integrazione di Workfront per le esigenze di integrazione della tua organizzazione con Salesforce.
>
>Per una panoramica dell&#39;automazione e dell&#39;integrazione di Workfront, vedere [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Per informazioni sulle funzionalità specifiche dei moduli di automazione e integrazione di Workfront per Salesforce, vedere [Moduli Salesforce](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

In qualità di amministratore di [!DNL Salesforce] e [!DNL Adobe Workfront], puoi installare [!DNL Workfront for Salesforce] per consentire agli utenti di [!DNL Salesforce] di inviare [!DNL Workfront] richieste e creare automaticamente progetti senza mai uscire da Salesforce.

Per informazioni generali su ciò che è possibile aspettarsi installando [!DNL Workfront for Salesforce], vedere [[!DNL Adobe Workfront for Salesforce] panoramica](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Prerequisiti per l&#39;installazione e l&#39;utilizzo di  [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Installazione di  [!DNL Workfront for Salesforce] in corso](#installing-workfrontfor-salesforce)

>[!NOTE]
>
>La versione più recente di questa integrazione è stata rilasciata il 30 ottobre 2025.

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
   <td> <p>Standard</p>
   <p>Piano</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti per l&#39;installazione e l&#39;utilizzo di [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* Per installare l&#39;app, è necessario disporre di un&#39;istanza [!DNL Salesforce] con accesso a un account amministratore di sistema.
* Per configurare l&#39;integrazione è necessario disporre di un&#39;istanza [!DNL Workfront] con accesso a un account amministratore di sistema.
* [!UICONTROL Gli utenti di Salesforce] devono avere un account [!DNL Workfront] per poter:

   * Crea [!DNL Workfront] richieste da [!DNL Salesforce]
   * Visualizza [!DNL Workfront] richieste o progetti in Salesforce

## Installazione di [!DNL Workfront for Salesforce] in corso  {#installing-workfront-for-salesforce}

Per installare e configurare [!DNL Salesforce] è necessario essere un [!DNL Workfront] e un amministratore di sistema [!DNL Workfront for Salesforce].

Nelle sottosezioni seguenti viene descritto come installare [!DNL Workfront] per l&#39;ambiente di produzione [!DNL Salesforce]. Puoi seguire gli stessi passaggi per installare [!DNL Workfront] per l&#39;ambiente sandbox [!DNL Salesforce].

* [Installazione di  [!DNL Workfront for Salesforce] prima che diventi disponibile nel [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Installazione di  [!DNL Workfront for Salesforce]  in  [!DNL Salesforce Classic] Framework](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Installazione di  [!DNL Workfront for Salesforce]  in  [!DNL Salesforce Lightning Experience] Framework](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### Installazione di [!DNL Workfront for Salesforce] prima che diventi disponibile nel marketplace [!DNL AppExchange] {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] sarà presto disponibile in [!DNL Salesforce AppExchange].

Per installare l’app prima che sia disponibile:

1. Nell’ambiente di produzione, vai a

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqp](https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqp)

   Nell’ambiente Sandbox, vai a

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqp](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqp)

   >[!NOTE]
   >
   >Devi aver effettuato l’accesso a Salesforce per accedere a queste pagine.

1. Selezionare la casella **[!UICONTROL Sì, concedere l&#39;accesso a questi siti Web di terze parti]**.

   Viene visualizzata una schermata di caricamento. L&#39;installazione potrebbe richiedere del tempo.

1. Al termine dell&#39;installazione, fare clic su **[!UICONTROL Fine]**.

1. Passa a **[!UICONTROL Configurazione]** > **[!UICONTROL Sicurezza] Controlli** > **[!UICONTROL Impostazioni sito remoto]**.
1. (Condizionale) Seleziona Workfront dall’elenco.

   Oppure

   Se l&#39;URL di [!DNL Workfront] non viene visualizzato nell&#39;elenco **[!UICONTROL Tutti i siti remoti]**, fare clic su **[!UICONTROL Nuovo sito remoto]**.

1. (Condizionale) Se si aggiunge il sito, specificare **[!UICONTROL Nome sito remoto]**.

   Ad esempio, *[!DNL Workfront]*.

1. (Condizionale) Se si aggiunge il sito, specificare l&#39;**[!UICONTROL URL sito remoto]**.

   Ad esempio, *yourDomain.my.workfront.com*.

1. Fai clic su **[!UICONTROL Salva]**.

   L&#39;app [!DNL Workfront] è ora installata nell&#39;istanza [!DNL Salesforce] e le pagine **[!UICONTROL WorkfrontOpportunities]** e **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] sono state create nell&#39;ambiente.

   [!DNL Salesforce] utenti possono utilizzare l&#39;app dopo aver aggiunto la sezione [!DNL Workfront] ai layout di pagina [!UICONTROL Opportunity] o [!UICONTROL Account].\
   Per informazioni sulla configurazione della sezione Workfront per gli utenti, vedere [Configurare la sezione Adobe Workfront per gli utenti di Salesforce](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installazione di [!DNL Workfront] per [!DNL Salesforce] nel framework [!DNL Salesforce Classic]

1. Accedere a [!DNL Salesforce] come amministratore di sistema.
1. Vai a **Configurazione.**
1. Nella sezione **Build**, fai clic su **AppExchange Marketplace**.

1. Nella casella **Cerca app AppExchange** digitare **Workfront**.

1. Fai clic sull&#39;app Workfront quando la trovi, quindi fai clic su **Scarica ora**.
1. Fai clic su **[!UICONTROL Installa in produzione]** per installare l&#39;app [!DNL Workfront] nell&#39;ambiente di produzione [!DNL Salesforce]. (operazione consigliata)
1. Dopo aver letto e accettato i termini e le condizioni, abilita il campo **[!UICONTROL Ho letto e accetto i termini e le condizioni]**.
1. Fare clic su **[!UICONTROL Conferma e installa]**.
1. Seleziona **[!UICONTROL Installa per tutti gli utenti]** (scelta consigliata), quindi fai clic su **[!UICONTROL Installa]**.

1. (Condizionale) Se viene richiesto se si desidera approvare l&#39;accesso di terze parti, selezionare **[!UICONTROL Sì, concedere l&#39;accesso a questi siti Web di terze parti]**, quindi fare clic su **[!UICONTROL Continua]**.

1. Al termine dell&#39;installazione, fare clic su **[!UICONTROL Fine]**.

   L&#39;app [!DNL Workfront] è elencata in **[!UICONTROL Pacchetti installati]**.


1. Passare a **[!UICONTROL Configurazione>Controlli di protezione>Impostazioni sito remoto]**.
1. (Condizionale) Se l&#39;URL [!DNL Workfront] non viene visualizzato nell&#39;elenco **[!UICONTROL Tutti i siti remoti]**, fare clic su **[!UICONTROL Nuovo sito remoto]**.

1. (Condizionale) Se si aggiunge il sito, specificare **[!UICONTROL Nome sito remoto]**.
Ad esempio, *[!DNL Workfront]*.

1. (Condizionale) Se si aggiunge il sito, specificare l&#39;**[!UICONTROL URL sito remoto]**.
Ad esempio, *yourDomain.my.workfront.com*.

1. Fai clic su **[!UICONTROL Salva]**.\
   L&#39;app [!DNL Workfront] è ora installata nell&#39;istanza [!DNL Salesforce]. Le pagine **[!UICONTROL WorkfrontOpportunities]** e **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] sono state create nel tuo ambiente.\
   [!DNL Salesforce] utenti non possono ancora utilizzare l&#39;app finché non aggiungi la sezione [!DNL Workfront] ai layout di pagina [!UICONTROL Opportunity] o [!UICONTROL Account].\
   Per informazioni sulla configurazione della sezione [!DNL Workfront] per gli utenti, vedere [Configurare la sezione  [!DNL Adobe Workfront] per [!DNL Salesforce] utenti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installazione di [!DNL Workfront for Salesforce] nel framework [!DNL Salesforce Lightning Experience]

1. Accedere a [!DNL Salesforce] come amministratore di sistema.
1. Fai clic sull&#39;icona **[!UICONTROL Setup]**, quindi fai clic su **[!UICONTROL Setup]**.

1. Nella sezione **[!UICONTROL STRUMENTI PLATFORM]**, espandi **[!UICONTROL App].**

1. Fai clic su **[!DNL AppExchange Marketplace]**.
1. Nella casella **[!UICONTROL Cerca [!DNL AppExchange] app]** digitare **[!DNL Workfront]**.

1. Fai clic sull&#39;app Workfront quando la trovi, quindi fai clic su **Scarica ora**.
1. Fare clic su **[!UICONTROL Apri schermata di accesso]**.\
   Devi accedere con il tuo account amministratore [!DNL Workfront] per [!DNL Salesforce].

1. Fare clic su **[!UICONTROL Consenti]**.
1. Nella casella **[!UICONTROL Installa in questa organizzazione]**, fare clic su **[!UICONTROL Installa qui]** per installare [!DNL Workfront] nell&#39;ambiente di produzione [!DNL Salesforce]. (operazione consigliata)

1. Dopo aver letto e accettato i termini e le condizioni, abilita il campo **[!UICONTROL Ho letto e accetto i termini e le condizioni]**.
1. Fare clic su **[!UICONTROL Conferma e installa]**.
1. Seleziona **[!UICONTROL Installa per tutti gli utenti]** (scelta consigliata), quindi fai clic su **[!UICONTROL Installa]**.

1. (Condizionale) Se viene richiesto se si desidera approvare l&#39;accesso di terze parti, selezionare **[!UICONTROL Sì, concedere l&#39;accesso a questi siti Web di terze parti]**, quindi fare clic su **[!UICONTROL Continua]**.

1. Al termine dell&#39;installazione, fare clic su **[!UICONTROL Fine]**.

   L&#39;app [!DNL Workfront] è elencata in **[!UICONTROL Pacchetti installati]**.

1. Passa a **[!UICONTROL Configurazione].**
1. Nella sezione **[!UICONTROL SETTINGS]** espandere **[!UICONTROL Security].**

1. Fare clic su **[!UICONTROL Impostazioni sito remoto]**.
1. (Condizionale) Se l&#39;URL [!DNL Workfront] non viene visualizzato nell&#39;elenco **[!UICONTROL Tutti i siti remoti]**, fare clic su **[!UICONTROL Nuovo sito remoto]**.

1. (Condizionale) Se si aggiunge il sito, specificare **[!UICONTROL Nome sito remoto]**.
Ad esempio, *[!DNL Workfront]*.

1. (Condizionale) Se si aggiunge il sito, specificare l&#39;**[!UICONTROL URL sito remoto]**.
Ad esempio, *yourDomain.my.workfront.com*.

1. Fai clic su **[!UICONTROL Salva]**.

   L&#39;app [!DNL Workfront] è ora installata nell&#39;istanza [!DNL Salesforce] e il componente **[!DNL Workfront]** è stato aggiunto all&#39;ambiente.

   Gli utenti di [!UICONTROL Salesforce] possono utilizzare l&#39;app [!DNL Workfront] dopo aver aggiunto la sezione [!DNL Workfront] ai layout di pagina [!UICONTROL Opportunity] o [!UICONTROL Account].\
   Per informazioni sulla configurazione della sezione [!DNL Workfront] per gli utenti, vedere [Configurare la sezione  [!DNL Adobe Workfront] per [!DNL Salesforce] utenti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## Configurare le autorizzazioni per l’integrazione di Workfront for Salesforce

### Autorizzazioni per `workfront_business`

1. Passa a **Configurazione** > **Sicurezza** > **URL attendibili**.
1. Seleziona `workfront_business` dall&#39;elenco.
1. Fai clic su **Modifica**.
1. In Direttive CSP, seleziona le seguenti opzioni:

   * connect-src (script)
   * font-src (font)
   * frame-src (contenuto iframe)
   * img-src (immagini)
   * media-src (audio e video)
   * style-src (fogli di stile)

1. Fai clic su **Salva**.


### Autorizzazioni per workfront_session

1. Passa a **Configurazione** > **Sicurezza** > **URL attendibili**.
1. Seleziona `workfront_session` dall&#39;elenco.
1. Fai clic su **Modifica**.
1. In Direttive CSP, seleziona le seguenti opzioni:

   * connect-src (script)
   * font-src (font)
   * frame-src (contenuto iframe)
   * img-src (immagini)
   * media-src (audio e video)
   * style-src (fogli di stile)

1. Fai clic su **Salva**.

