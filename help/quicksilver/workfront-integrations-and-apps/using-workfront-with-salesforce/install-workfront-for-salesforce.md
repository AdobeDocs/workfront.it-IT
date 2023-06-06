---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Installa [!DNL Adobe Workfront] per [!DNL Salesforce]
description: Per installare l’app prima che diventi disponibile nella [!DNL Salesforce] AppExchange, vedere Installazione [!DNL Workfront] per Salesforce prima che diventi disponibile nel marketplace di AppExchange.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: 0c49ab99653f390d592bba39bcb92145b8bedd0c
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 1%

---

# Installa [!DNL Adobe Workfront for Salesforce]

Per installare l’app prima che diventi disponibile nella [!DNL Salesforce AppExchange], vedi [Installazione [!DNL Workfront for Salesforce] prima che diventi disponibile in [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

As a [!DNL Salesforce] e [!DNL Adobe Workfront] amministratore, è possibile installare [!DNL Workfront for Salesforce] per consentire [!DNL Salesforce] utenti da inviare [!DNL Workfront] richiede e crea automaticamente progetti senza mai uscire da Salesforce.

Per informazioni generali su ciò che è possibile aspettarsi installando [!DNL Workfront for Salesforce], vedi [[!DNL Adobe Workfront for Salesforce] panoramica](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Prerequisiti per l’installazione e l’utilizzo di [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce-prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Installazione [!DNL Workfront for Salesforce]](#install-adobe-workfront-for-salesforce)

## Requisiti di accesso

Per utilizzare le funzionalità descritte in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr>  </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Prerequisiti per l’installazione e l’utilizzo di [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* È necessario disporre di [!DNL Salesforce] con accesso a un account amministratore di sistema per installare l’app.
* È necessario disporre di [!DNL Workfront] con accesso a un account amministratore di sistema per configurare l’integrazione.
* [!UICONTROL Salesforce] gli utenti devono avere [!DNL Workfront] per essere in grado di

   * Crea [!DNL Workfront] richieste da [!DNL Salesforce] o
   * Visualizza [!DNL Workfront] richieste o progetti in Salesforce.

## Installazione [!DNL Workfrontfor Salesforce] {#installing-workfront-for-salesforce}

Devi essere un [!DNL Salesforce] e un [!DNL Workfront] l&#39;amministratore di sistema per installare e configurare [!DNL Workfront for Salesforce].

Nelle sottosezioni seguenti viene descritto come installare [!DNL Workfront] per [!DNL Salesforce] Ambiente di produzione. Puoi seguire gli stessi passaggi per installare [!DNL Workfront] per [!DNL Salesforce] Ambiente sandbox.

* [Installazione [!DNL Workfront for Salesforce] prima che diventi disponibile in [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Installazione [!DNL Workfront for Salesforce] nel [!DNL Salesforce Classic] Framework](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Installazione [!DNL Workfront for Salesforce] nel [!DNL Salesforce Lightning Experience] Framework](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### Installazione [!DNL Workfront for Salesforce] prima che diventi disponibile in [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] sarà disponibile nel [!DNL Salesforce AppExchange] presto.

Per installare l’app prima che sia disponibile:

1. Nell’ambiente di produzione, vai a

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

   Nell’ambiente Sandbox, vai a

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

1. Controlla la **[!UICONTROL Sì, consenti l’accesso a questi siti web di terze parti]** casella.

   Viene visualizzata una schermata di caricamento e l’installazione potrebbe richiedere del tempo.

1. Clic **[!UICONTROL Fine]** al termine dell’installazione.

1. Accedi a **[!UICONTROL Configurazione>Controlli di protezione>Impostazioni sito remoto]**.
1. (Condizionale) Se non vedi il [!DNL Workfront] URL elencato in **[!UICONTROL Tutti i siti remoti]** , fare clic su **[!UICONTROL Nuovo sito remoto]**.

1. Specifica la **[!UICONTROL Nome sito remoto]**.

   Ad esempio, *[!DNL Workfront]*.

1. Specifica la **[!UICONTROL URL sito remoto]**.

   Ad esempio: *yourDomain.my.workfront.com*.

1. Fai clic su **[!UICONTROL Salva]**.

   Il [!DNL Workfront] l&#39;app è ora installata sul tuo [!DNL Salesforce] e **[!UICONTROL Opportunità Workfront]** e **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] Le pagine sono state create nell’ambiente.

   [!DNL Salesforce] Gli utenti possono utilizzare l’app dopo che hai aggiunto [!DNL Workfront] sezione alla loro [!UICONTROL opportunità] o [!UICONTROL Account] layout di pagina.\
   Per informazioni sulla configurazione della sezione Workfront per gli utenti, consulta [Configurare la sezione Adobe Workfront per gli utenti Salesforce](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installazione [!DNL Workfront] per [!DNL Salesforce] nel [!DNL Salesforce Classic] Framework

1. Accedi a [!DNL Salesforce] come amministratore di sistema.
1. Vai a **Configurazione.**
1. In **Genera** , fare clic su **AppExchange Marketplace**.

1. In **Cerca app di AppExchange** casella, digitare **Workfront**.

1. Fai clic sull’app quando la trovi, quindi fai clic su **Ottieni subito**.
1. Clic **[!UICONTROL Installazione in produzione]** per installare [!DNL Workfront] app nel tuo [!DNL Salesforce] Ambiente di produzione. (consigliato)
1. Seleziona la **[!UICONTROL Ho letto e accetto i termini e le condizioni]** dopo aver letto e accettato i termini e le condizioni.
1. Clic **[!UICONTROL Conferma e installa]**.
1. Seleziona **[!UICONTROL Installa per tutti gli utenti]** (scelta consigliata), quindi fai clic su **[!UICONTROL Installa]**.

1. (Condizionale) Se viene richiesto se desideri approvare l’accesso di terze parti, seleziona **[!UICONTROL Sì, consenti l’accesso a questi siti web di terze parti]**, quindi fai clic su **[!UICONTROL Continua]**.

1. Clic **[!UICONTROL Fine]** al termine dell’installazione.

   Il [!DNL Workfront] l&#39;app è elencata in **[!UICONTROL Pacchetti installati]**.


1. Accedi a **[!UICONTROL Configurazione>Controlli di protezione>Impostazioni sito remoto]**.
1. (Condizionale) Se non vedi il [!DNL Workfront] URL elencato in **[!UICONTROL Tutti i siti remoti]** , fare clic su **[!UICONTROL Nuovo sito remoto]**.\

1. Specifica la **[!UICONTROL Nome sito remoto]**.\
   Ad esempio, *[!DNL Workfront]*.

1. Specifica la **[!UICONTROL URL sito remoto]**.\
   Ad esempio: *yourDomain.my.workfront.com*.

1. Fai clic su **[!UICONTROL Salva]**.\
   Il [!DNL Workfront] l&#39;app è ora installata sul tuo [!DNL Salesforce] e **[!UICONTROL Opportunità Workfront]** e **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] Le pagine sono state create nell’ambiente.\
   [!DNL Salesforce] Gli utenti non possono ancora utilizzare l&#39;app finché non aggiungi il [!DNL Workfront] sezione alla loro [!UICONTROL opportunità] o [!UICONTROL Account] layout di pagina.\
   Per informazioni sulla configurazione di [!DNL Workfront] sezione per gli utenti, consulta [Configurare [!DNL Adobe Workfront] sezione per [!DNL Salesforce] utenti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installazione [!DNL Workfront for Salesforce] nel [!DNL Salesforce Lightning Experience] Framework

1. Accedi a [!DNL Salesforce] come amministratore di sistema.
1. Fai clic su **[!UICONTROL Configurazione] icona**, quindi fai clic su **[!UICONTROL Configurazione]**.

1. In **[!UICONTROL STRUMENTI DELLA PIATTAFORMA]** , espandere **[!UICONTROL App].**

1. Clic **[!DNL AppExchange Marketplace]**.
1. In **[!UICONTROL Ricerca [!DNL AppExchange] App]** casella, digitare **[!DNL Workfront]**.

1. Fai clic sull’app quando la trovi, quindi fai clic su **[!UICONTROL Ottieni subito]**.
1. Clic **[!UICONTROL Apri schermata di accesso]**.\
   Devi accedere con il tuo [!DNL Workfront] account amministratore per [!DNL Salesforce].

1. Clic **[!UICONTROL Consenti]**.
1. In **[!UICONTROL Installa in questa organizzazione]** , fare clic su **[!UICONTROL Installa qui]** per installare [!DNL Workfront] nel tuo [!DNL Salesforce] Ambiente di produzione. (consigliato)

1. Seleziona la **[!UICONTROL Ho letto e accetto i termini e le condizioni]** dopo aver letto e accettato i termini e le condizioni.
1. Clic **[!UICONTROL Conferma e installa]**.
1. Seleziona **[!UICONTROL Installa per tutti gli utenti]** (scelta consigliata), quindi fai clic su **[!UICONTROL Installa]**.

1. (Condizionale) Se viene richiesto se desideri approvare l’accesso di terze parti, seleziona **[!UICONTROL Sì, consenti l’accesso a questi siti web di terze parti]**, quindi fai clic su **[!UICONTROL Continua]**.

1. Clic **[!UICONTROL Fine]** al termine dell’installazione.

   Il [!DNL Workfront] l&#39;app è elencata in **[!UICONTROL Pacchetti installati]**.

1. Accedi a **[!UICONTROL Configurazione].**
1. In **[!UICONTROL IMPOSTAZIONI]** , espandere&#x200B;**[!UICONTROL Sicurezza].**

1. Clic **[!UICONTROL Impostazioni sito remoto]**.
1. (Condizionale) Se non vedi il [!DNL Workfront] URL elencato in **[!UICONTROL Tutti i siti remoti]** , fare clic su **[!UICONTROL Nuovo sito remoto]**.

1. Specifica la **[!UICONTROL Nome sito remoto]**.

   Ad esempio, *[!DNL Workfront]*.

1. Specifica la **[!UICONTROL URL sito remoto]**.

   Ad esempio: *yourDomain.my.workfront.com*.

1. Fai clic su **[!UICONTROL Salva]**.

   Il [!DNL Workfront] l&#39;app è ora installata sul tuo [!DNL Salesforce] e **[!DNL Workfront]** Il componente viene ora aggiunto all&#39;ambiente.

   [!UICONTROL Salesforce] Gli utenti possono utilizzare [!DNL Workfront] una volta aggiunto il [!DNL Workfront] sezione alla loro [!UICONTROL opportunità] o [!UICONTROL Account] layout di pagina.\
   Per informazioni sulla configurazione di [!DNL Workfront] sezione per gli utenti, consulta [Configurare [!DNL Adobe Workfront] sezione per [!DNL Salesforce] utenti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
