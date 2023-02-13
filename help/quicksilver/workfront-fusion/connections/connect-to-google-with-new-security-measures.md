---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: connections-annd-webhooks
title: Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] con misure di sicurezza aggiornate
description: Google ha recentemente introdotto restrizioni su come gli utenti possono utilizzare le loro API. Questo articolo descrive come connettersi [!DNL Adobe Workfront Fusion] a Google, tenendo conto di queste misure di sicurezza di aggiornamento.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] con misure di sicurezza aggiornate

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] restrizioni

[!DNL Google] a partire dal 1° giugno 2020, sono state introdotte restrizioni sulle modalità di utilizzo delle API da parte degli utenti. Queste misure di sicurezza proteggono [!DNL Google] gli utenti da perdite o uso improprio dei loro dati personali su [!DNL Google]. Le restrizioni sono legate al [!DNL Gmail] e [!DNL Google Drive] app. Per ulteriori informazioni su queste restrizioni, consulta &quot;Requisiti aggiuntivi per ambiti API specifici&quot; in [[!DNL Google] Criteri utente dei servizi API](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Per accedere agli ambiti limitati, il servizio connesso ([!DNL Adobe Workfront Fusion] o qualsiasi altro servizio che desideri accedere ai dati dell’utente tramite l’API) deve essere verificato e deve disporre di una lettera di valutazione per dimostrare che il servizio è sicuro e trasparente sul modo in cui utilizzano i dati. [!DNL Workfront Fusion] è conforme a tutte le [!DNL Google]Requisiti di accesso agli ambiti ristretti. Tuttavia, la maggior parte dei servizi collegati di terze parti in [!DNL Workfront Fusion] non hanno la lettera di valutazione e quindi non si conformano [!DNL Google] termini. Per questo motivo, [!DNL Workfront Fusion] non è consentito inviare dati a tali servizi.

## Eccezioni a [!DNL Google Services] restrizioni

Ci sono alcune eccezioni che permettono di inviare dati a un servizio di terze parti non autorizzato che non ha la lettera di valutazione senza violare nessuna delle nuove restrizioni. Si differenziano in base a [!DNL G Suite] con [!DNL Workfront Fusion] client OAuth, [!DNL G Suite] con un altro client OAuth, oppure [!DNL @gmail.com] e [!DNL @google.mail.com].

* [[!DNL G suite] con [!DNL Workfront Fusion] Client OAuth](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL G suite] con un altro client OAuth](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] e [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] con [!DNL Workfront Fusion] Client OAuth

[!DNL Workfront Fusion] utilizza [!UICONTROL Installazione a livello di dominio] eccezione. Installazione a livello di dominio [!DNL G Suite] e consente agli utenti di integrare servizi non approvati senza alcuna limitazione. Se sei un utente di G Suite, non devi eseguire altri passaggi e puoi connetterti direttamente a servizi non approvati.

### [!DNL G suite] con un altro client OAuth

[!DNL G Suite] utenti che preferiscono utilizzare il proprio client OAuth invece di utilizzare il [!DNL Workfront Fusion] Il client OAuth può connettersi a [!DNL Google Services] attraverso [!UICONTROL Interno] Utilizza l’approccio . Questa opzione è destinata agli utenti avanzati. Per istruzioni, consulta [Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzo di un client OAuth personalizzato](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] e [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

Utente con accesso [!DNL Google Services] attraverso [!DNL @gmail.com] o [!DNL @googlemail.com] può connettersi a [!DNL Google Services] mediante l’approccio Uso personale. Questa opzione è destinata agli utenti avanzati. Per istruzioni, consulta [Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzo di un client OAuth personalizzato](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## Domande frequenti

* [Quali app in [!DNL Adobe Workfront Fusion] sono interessati?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Ho un account [!DNL G Suite]?](#do-i-have-a-g-suite-account)
* [Cosa dovrei fare se sono [!DNL @gmail.com] o [!DNL @googlemail.com] utente?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [Cosa devo fare se sono un utente di [!DNL G Suite]?](#what-should-i-do-if-im-a-g-suite-user)

### Quali app in [!DNL Adobe Workfront Fusion] sono interessati? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail], e-mail (connesso a [!DNL Gmail] account).

### Ho un [!DNL G Suite] account? {#do-i-have-a-g-suite-account}

Se il tuo indirizzo e-mail termina con [!DNL @gmail.com] o [!DNL @googlemail.com] il tuo account non è un [!DNL G Suite] conto. Se [!DNL Google] l&#39;account termina con un dominio personalizzato come @my-company.com e quindi è un [!DNL G Suite] conto.

### Cosa dovrei fare se sono [!DNL @gmail.com] o [!DNL @googlemail.com] utente? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Queste nuove restrizioni si applicano solo se si esegue l&#39;integrazione [!DNL Google Drive] o [!DNL Gmail]. Se desideri connetterti a [!DNL Google Drive] o [!DNL Gmail], puoi

* Passa a [!DNL G Suite]

   oppure

* Crea un client OAuth personalizzato. Questa opzione è destinata agli utenti avanzati.

   Per istruzioni, consulta [Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzo di un client OAuth personalizzato](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Se desideri integrare un servizio diverso da [!DNL Google Drive] o [!DNL Gmail], queste restrizioni non si applicano.

Per istruzioni su come collegare altri [!DNL Google Services] a [!DNL Workfront Fusion], vedi [Collega l’app o il servizio Web del modulo a [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) nell&#39;articolo [Crea uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Cosa devo fare se sono un [!DNL G Suite] utente? {#what-should-i-do-if-im-a-g-suite-user}

Non è necessaria alcuna azione.
