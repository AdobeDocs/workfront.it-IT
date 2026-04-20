---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Gestire le chiavi API
description: Per ridurre al minimo le vulnerabilità di sicurezza API, gli amministratori di Adobe Workfront possono gestire le chiavi API utilizzate per consentire alle applicazioni di accedere a Workfront per conto di un utente.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: aeb471fd63269d30a675e44fe1a47db6141eb9ed
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 17%

---

# Gestire le chiavi API

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->



>[!IMPORTANT]
>
>Workfront non consiglia più di utilizzare l’endpoint `/login` o le chiavi API. Utilizza invece uno dei seguenti metodi di autenticazione:
>
>* Autenticazione server con JWT
>* Autenticazione utente con OAuth2
>
>Per istruzioni sulla configurazione di questi metodi di autenticazione, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)
>
>Per istruzioni sull’utilizzo dell’autenticazione server in Workfront, consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso JWT](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md)
>
>Per istruzioni sull’utilizzo dell’autenticazione utente in Workfront, consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso del codice di autorizzazione](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md)

Per ridurre al minimo le vulnerabilità di sicurezza API, gli amministratori di Adobe Workfront possono gestire le chiavi API utilizzate per consentire alle applicazioni di accedere a Workfront per conto di un utente.

Puoi reimpostare o rimuovere la chiave API dell’amministratore corrente, configurare le chiavi API in scadenza e rimuovere le chiavi API per tutti gli utenti.

Esempi di applicazioni che sfruttano l’API di Workfront sono:

* Integrazioni di documenti come Dropbox, Google Drive e Workfront DAM
* Applicazioni mobili Workfront

>[!IMPORTANT]
>
>Quando si ripristina o si rimuove una chiave API, qualsiasi applicazione che sfrutta l’API Workfront e si autentica in Workfront tramite questa chiave API deve essere riconfigurata per poter riottenere l’accesso a Workfront.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td><p>Standard</p><p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Chiavi API Workfront

Ogni utente in Workfront ha una chiave API univoca. Questa chiave viene generata per singolo utente nel momento in cui l’utente accede a un’integrazione che sfrutta l’API di Workfront (ad esempio l’app mobile Workfront o un’integrazione con un documento).

>[!NOTE]
>
> Le chiavi API generate nell&#39;ambiente di produzione vengono copiate nell&#39;ambiente di anteprima durante l&#39;aggiornamento settimanale. Tutte le chiavi API generate nell’ambiente di anteprima verranno sovrascritte con le chiavi API di produzione durante l’aggiornamento settimanale.

Gli amministratori di Workfront dispongono inoltre di una chiave API univoca. Quando un’applicazione utilizza una chiave API amministratore per accedere a Workfront, ha accesso amministratore a Workfront.

## Gestire una chiave API di amministratore

Puoi generare, reimpostare o rimuovere la chiave API per l’account utente amministratore.

{{step-1-to-setup}}

1. Fai clic su **Sistema >** **Informazioni cliente.**
1. (Condizionale) Esegui una delle azioni seguenti:

   Per generare una chiave API: nella sezione **Impostazioni chiave API**, fai clic su **Genera chiave API**.

   Oppure\
   Per reimpostare una chiave API: nella sezione **Impostazioni chiave API**, fare clic su **Reimposta**, quindi su **Reimposta.**

   Oppure

   Per rimuovere la chiave API: nella sezione **Impostazioni chiave API**, fare clic su **Rimuovi**, quindi su **Rimuovi**.

<!--

   Remove me October 2026

## Generate an API Key for Non-Admin Users

You can generate and manage API Keys for users in roles other than Workfront administrator.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

1. (Conditional) If your organization uses Single Sign-On (SSO) access management, temporarily disable the option requiring SSO authentication.

   {{step-1-to-setup}} 
   
   1. Expand **System**, then click **Single Sign-on (SSO)**. 
   1. In the **Type** field, select the type of SSO your organization uses.
   1. With the type selected, scroll down and clear the **Enable** checkbox. 
      ![Enable SSO](assets/sysadmin-security-sso-disable-31620-350x320.png)  
   1. Click **Save**.


1. In the address bar of a browser, enter the following API call:

   `<domain>`.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&username=**username**&password=**password**&method=PUT

   Replace `<domain>` with your Workfront domain name, and username and password with the user's Workfront credentials.

1. (Conditional) Enable the option requiring SSO authentication if you disabled it in Step 1.

   {{step-1-to-setup}}
   
   1. Expand **System**, then click **Single Sign-on (SSO)**.
   
   1. Select your SSO method in the **Type** drop down menu.
   1. Check the checkbox requiring SSO authentication.

   -->

## Configurare quando scadono le chiavi API

Puoi configurare le chiavi API in modo che scadano per tutti gli utenti nel sistema. Quando la chiave API di un utente scade, l’utente deve autenticare nuovamente tutte le applicazioni che utilizzano l’API Workfront per accedere a Workfront. Puoi modificare la frequenza di scadenza delle chiavi API. Puoi anche configurare la scadenza delle chiavi API quando scade la password di un utente.

{{step-1-to-setup}}

1. Fai clic su **Sistema** > **Informazioni cliente**.
1. Nell&#39;area **Impostazioni chiave API**, nell&#39;elenco a discesa **Dopo la creazione**, **Le chiavi API scadono**, selezionare l&#39;intervallo di tempo in cui si desidera che scadano le chiavi API.

   Quando si modifica questa opzione, il nuovo intervallo temporale inizia dal momento in cui è stata apportata la modifica. Ad esempio, se modifichi questa opzione da *1 mese* a *6 mesi*, le chiavi API scadono dopo 6 mesi dal momento in cui effettui la modifica.

   Per impostazione predefinita, le chiavi API scadono ogni mese.

1. Per configurare le chiavi API in modo che scadano quando scadono le password degli utenti, abilitare **Rimuovi chiave API alla scadenza della password di un utente**.

   Per impostazione predefinita, questa opzione non è abilitata.

   Per informazioni su come configurare le password utente in modo che scadano, vedere [Configurare le preferenze di sicurezza del sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Fai clic su **Salva**.

## Rimuovi le chiavi API per tutti gli utenti

Se sei preoccupato di una particolare violazione di sicurezza relativa al tuo sistema Workfront, puoi rimuovere le chiavi API simultaneamente per tutti gli utenti.

>[!IMPORTANT]
>
>La rimozione delle chiavi API per tutti gli utenti invalida TUTTE le chiavi API per tutti gli utenti del sistema. Questa azione causerà un errore in tutte le integrazioni in Workfront fino a quando non genererai una nuova chiave API in Workfront e non aggiornerai tutte le integrazioni.

{{step-1-to-setup}}

1. Espandi **Sistema**, quindi fai clic su **Informazioni cliente**.

1. Nell&#39;area **Impostazioni chiave API**, fare clic su **Rimuovi tutte le chiavi API**, quindi su **Rimuovi** **Tutte**.

<!--

Remove me October 2026

## Restricting API logins with an X.509 certificate

>[!IMPORTANT]
>
>The procedure described in this section applies only to organizations that have not yet been onboarded to the Adobe Business Platform. Logging in to Workfront through the Workfront API is not available if your organization has been onboarded to the Adobe Business Platform.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

Third-party applications can communicate with Workfront through the API. To increase the security of your Workfront site, you can configure Workfront to restrict API login requests by uploading an X.509 certificate to Workfront. Once enabled, all login requests through the API must include a client certificate in addition to username and password.

* [Obtain the X.509 certificate](#obtain-the-x-509-certificate) 
* [Upload the certificate to Workfront](#upload-the-certificate-to-workfront) 
* [Verify API login calls are restricted](#verify-api-login-calls-are-restricted)

### Obtain the X.509 certificate {#obtain-the-x-509-certificate}

Obtain a valid X.509 certificate from a trusted Certificate Authority (such as Verisign), and save it to a temporary location on your workstation. 

### Upload the certificate to Workfront {#upload-the-certificate-to-workfront}

After you have obtained the X.509 certificate from your Certificate Authority, you need to upload it to Workfront.

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).  

1. Expand **System**, then click **Customer Info**.

1. In the **API Key Settings** area, select **Require X.509 Certificate for API logins**.
1. Click **Change Certificate**.
1. On your workstation, browse to and select the X.509 certificate that you previously downloaded.
1. (Optional) Click **View Details** next to the certificate name to view the following details about the certificate:

   * Subject Common Name
   * Subject Organization
   * Subject Organization Unit
   * Issuer Common Name
   * Issuer Organization
   * Issuer Organization Unit
   * Serial Number
   * Issue Date
   * Expiration Date

1. Click **Save**. 

### Verify API login calls are restricted {#verify-api-login-calls-are-restricted}

Prior to configuring your instance of Workfront to require an X.509 certificate, perform an API request to the `/login` endpoint using valid username and password parameters. You will receive a 200 response that contains a sessionID.

After making the X.509 certificate a requirement via the customer info page in your instance of Workfront, make another login attempt. This time you will receive a 500 error response with the following message: "Untrusted request. Please contact your system administrator and attach certificate."

After confirming that the X.509 certificate is required, perform the same login request with an additional parameter for apiCertificate set to the value of your certificate. If this operation was performed correctly you will receive a 200 response that contains a valid sessionID.

-->
