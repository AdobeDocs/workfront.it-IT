---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: connections-annd-webhooks
title: Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] con misure di sicurezza aggiornate
description: Google ha recentemente introdotto restrizioni sulle modalità di utilizzo delle API da parte degli utenti. Questo articolo descrive come connettersi [!DNL Adobe Workfront Fusion] a Google, tenendo conto di queste misure di sicurezza dell’aggiornamento.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '669'
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
   <td> <p>[!UICONTROL Pro] o versione successiva</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td>
   <p>Fabbisogno di licenza corrente: No [!DNL Workfront Fusion] requisito di licenza.</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per l'automazione e l'integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone di [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Pianifica, la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo. [!DNL Workfront Fusion] è incluso in [!UICONTROL Ultimate] [!DNL Workfront] piano.</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare la funzionalità descritta in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, consulta [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] restrizioni

[!DNL Google] A partire dal 1° giugno 2020 sono state introdotte restrizioni sulle modalità di utilizzo delle API da parte degli utenti. Queste misure di sicurezza proteggono [!DNL Google] utenti dalla perdita o dall&#39;uso improprio dei loro dati personali su [!DNL Google]. Le restrizioni sono correlate al [!DNL Gmail] e [!DNL Google Drive] app. Per ulteriori informazioni su queste restrizioni, consulta &quot;Requisiti aggiuntivi per ambiti API specifici&quot; in [[!DNL Google] Criterio dati utente servizi API](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Per accedere agli ambiti con restrizioni, il servizio connesso ([!DNL Adobe Workfront Fusion] o qualsiasi altro servizio che desideri accedere ai dati dell’utente tramite l’API deve essere verificato e disporre di una lettera di valutazione per dimostrare che il servizio è sicuro e trasparente sul modo in cui utilizzano i dati. [!DNL Workfront Fusion] è conforme a tutte le [!DNL Google]requisiti di per l&#39;accesso agli ambiti con restrizioni. Tuttavia, la maggior parte dei servizi connessi di terze parti in [!DNL Workfront Fusion] non dispongono della lettera di valutazione e pertanto non rispettano [!DNL Google] termini. Per questo motivo, [!DNL Workfront Fusion] non è autorizzato a inviare dati a questi servizi.

## Eccezioni a [!DNL Google Services] restrizioni

Esistono alcune eccezioni che consentono di inviare dati a un servizio di terze parti non approvato che non dispone della lettera di valutazione senza violare alcuna delle nuove restrizioni. Differiscono in base a [!DNL G Suite] con [!DNL Workfront Fusion] client OAuth, [!DNL G Suite] con un altro client OAuth, oppure [!DNL @gmail.com] e [!DNL @google.mail.com].

* [[!DNL G suite] con [!DNL Workfront Fusion] Client OAuth](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL G suite] con un altro client OAuth](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] e [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] con [!DNL Workfront Fusion] Client OAuth

[!DNL Workfront Fusion] utilizza [!UICONTROL Installazione a livello di dominio] eccezione. L&#39;installazione a livello di dominio è ideale per [!DNL G Suite] e consente agli utenti di integrare servizi non approvati senza alcuna limitazione. Se sei un utente di G Suite, non devi eseguire alcun passaggio aggiuntivo e puoi connetterti direttamente a servizi non approvati.

### [!DNL G suite] con un altro client OAuth

[!DNL G Suite] utenti che preferiscono utilizzare il proprio client OAuth invece di utilizzare [!DNL Workfront Fusion] Il client OAuth può connettersi a [!DNL Google Services] tramite [!UICONTROL Interno] Utilizza l’approccio. Questa opzione è destinata agli utenti avanzati. Per istruzioni, consulta [Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzo di un client OAuth personalizzato](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] e [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

Utente che accede a [!DNL Google Services] da a [!DNL @gmail.com] o [!DNL @googlemail.com] può connettersi a [!DNL Google Services] mediante l’approccio Personal Use (Uso personale). Questa opzione è destinata agli utenti avanzati. Per istruzioni, consulta [Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzo di un client OAuth personalizzato](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## Domande frequenti

* [Quali app in [!DNL Adobe Workfront Fusion] sono interessati?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Ho un account [!DNL G Suite]?](#do-i-have-a-g-suite-account)
* [Cosa devo fare se sono [!DNL @gmail.com] o [!DNL @googlemail.com] utente?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [Cosa devo fare se sono un utente di [!DNL G Suite]?](#what-should-i-do-if-im-a-g-suite-user)

### Quali app in [!DNL Adobe Workfront Fusion] sono interessati? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail], e-mail (connesso a [!DNL Gmail] account).

### Ho un [!DNL G Suite] account? {#do-i-have-a-g-suite-account}

Se l’indirizzo e-mail termina con [!DNL @gmail.com] o [!DNL @googlemail.com] il tuo account non è un [!DNL G Suite] account. Se il [!DNL Google] l’account termina con un dominio personalizzato come @my-company.com, è un [!DNL G Suite] account.

### Cosa devo fare se sono [!DNL @gmail.com] o [!DNL @googlemail.com] utente? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Queste nuove restrizioni si applicano solo se si integra [!DNL Google Drive] o [!DNL Gmail]. Se desideri connetterti a [!DNL Google Drive] o [!DNL Gmail], è possibile

* Passa a [!DNL G Suite]

  oppure

* Crea un client OAuth personalizzato. Questa opzione è destinata agli utenti avanzati.

  Per istruzioni, consulta [Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzo di un client OAuth personalizzato](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Se desideri integrare un servizio diverso da [!DNL Google Drive] o [!DNL Gmail], queste restrizioni non si applicano.

Per istruzioni sulla connessione ad altri [!DNL Google Services] a [!DNL Workfront Fusion], vedi [Connetti l’app o il servizio web del modulo a [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) nell’articolo [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Cosa devo fare se sono un [!DNL G Suite] utente? {#what-should-i-do-if-im-a-g-suite-user}

Non è richiesta alcuna azione.
