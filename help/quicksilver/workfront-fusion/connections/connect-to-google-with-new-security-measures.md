---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connettore
navigation-topic: connections-annd-webhooks
title: Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] con misure di sicurezza aggiornate
description: Google ha recentemente introdotto restrizioni sulle modalità di utilizzo delle API da parte degli utenti. In questo articolo viene descritto come connettersi [!DNL Adobe Workfront Fusion] a Google tenendo conto di queste misure di protezione per gli aggiornamenti.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '649'
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
   <p>Requisiti di licenza correnti: nessun requisito di licenza [!DNL Workfront Fusion].</p>
   <p>Oppure</p>
   <p>Requisito licenza legacy: [!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>
   <p>Fabbisogno prodotto corrente: se si dispone del piano [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], l'organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo. [!DNL Workfront Fusion] è incluso nel piano [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>Oppure</p>
   <p>Requisiti del prodotto legacy: la tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore [!DNL Workfront].

Per informazioni sulle [!DNL Adobe Workfront Fusion] licenze, vedere [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] restrizioni

[!DNL Google] ha introdotto restrizioni su come gli utenti possono utilizzare le API a partire dal 1° giugno 2020. Queste misure di sicurezza proteggono [!DNL Google] utenti da perdite o uso improprio dei loro dati personali su [!DNL Google]. Le restrizioni sono correlate alle app [!DNL Gmail] e [!DNL Google Drive]. Per ulteriori informazioni su queste restrizioni, vedere &quot;Requisiti aggiuntivi per ambiti API specifici&quot; in [[!DNL Google] Criteri dei dati utente per i servizi API](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Per accedere agli ambiti con restrizioni, è necessario verificare il servizio connesso ([!DNL Adobe Workfront Fusion] o qualsiasi altro servizio che desideri accedere ai dati dell&#39;utente tramite l&#39;API) e disporre di una lettera di valutazione per verificare che il servizio sia sicuro e trasparente in merito all&#39;utilizzo dei dati. [!DNL Workfront Fusion] soddisfa tutti i requisiti di [!DNL Google] per l&#39;accesso agli ambiti con restrizioni. Tuttavia, la maggior parte dei servizi connessi di terze parti in [!DNL Workfront Fusion] non dispone della lettera di valutazione e pertanto non è conforme ai termini [!DNL Google]. Per questo motivo, a [!DNL Workfront Fusion] non è consentito inviare dati a questi servizi.

## Eccezioni alle restrizioni [!DNL Google Services]

Esistono alcune eccezioni che consentono di inviare dati a un servizio di terze parti non approvato che non dispone della lettera di valutazione senza violare alcuna delle nuove restrizioni. Differiscono in base a [!DNL Google Workspace] con il client OAuth [!DNL Workfront Fusion], [!DNL Google Workspace] con un altro client OAuth oppure [!DNL @gmail.com] e [!DNL @google.mail.com].

* [[!DNL Google Workspace] con  [!DNL Workfront Fusion] client OAuth](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL Google Workspace] con un altro client OAuth](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] e [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL Google Workspace] con [!DNL Workfront Fusion] client OAuth

[!DNL Workfront Fusion] utilizza l&#39;eccezione [!UICONTROL Installazione a livello di dominio]. L&#39;installazione a livello di dominio è adatta a [!DNL Google Workspace] utenti e consente agli utenti di integrare servizi non approvati senza alcuna limitazione. Se sei un utente di Google Workspace, non devi eseguire alcun passaggio aggiuntivo e puoi connetterti direttamente a servizi non approvati.

### [!DNL Google Workspace] con un altro client OAuth

[!DNL Google Workspace] utenti che preferiscono utilizzare il proprio client OAuth anziché il client OAuth [!DNL Workfront Fusion] possono connettersi a [!DNL Google Services] tramite l&#39;approccio [!UICONTROL Internal] Use. Questa opzione è destinata agli utenti avanzati. Per istruzioni, vedere [Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzando un client OAuth personalizzato](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] e [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

L&#39;utente che accede a [!DNL Google Services] tramite [!DNL @gmail.com] o [!DNL @googlemail.com] può connettersi a [!DNL Google Services] tramite l&#39;approccio Personal Use. Questa opzione è destinata agli utenti avanzati. Per istruzioni, vedere [Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzando un client OAuth personalizzato](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## Domande frequenti

* [Quali app in  [!DNL Adobe Workfront Fusion]  sono interessate?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Ho un account  [!DNL Google Workspace] ?](#do-i-have-a-g-suite-account)
* [Cosa devo fare se sono  [!DNL @gmail.com] o [!DNL @googlemail.com] utente?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [Cosa devo fare se sono un utente  [!DNL Google Workspace] ?](#what-should-i-do-if-im-a-g-suite-user)

### Quali app in [!DNL Adobe Workfront Fusion] sono interessate? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail] e e-mail (connesso all&#39;account [!DNL Gmail]).

### Ho un account [!DNL Google Workspace]? {#do-i-have-a-g-suite-account}

Se l&#39;indirizzo di posta elettronica termina con [!DNL @gmail.com] o [!DNL @googlemail.com], l&#39;account non è un account [!DNL Google Workspace]. Se l&#39;account [!DNL Google] termina con un dominio personalizzato come @my-company.com, si tratta di un account [!DNL Google Workspace].

### Cosa devo fare se sono utente [!DNL @gmail.com] o [!DNL @googlemail.com]? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Queste nuove restrizioni vengono applicate solo se si integra [!DNL Google Drive] o [!DNL Gmail]. Se desideri connetterti a [!DNL Google Drive] o [!DNL Gmail], puoi

* Passa a [!DNL Google Workspace]

  oppure

* Crea un client OAuth personalizzato. Questa opzione è destinata agli utenti avanzati.

  Per istruzioni, vedere [Connetti [!DNL Adobe Workfront Fusion] a [!DNL Google Services] utilizzando un client OAuth personalizzato](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Se si desidera integrare un servizio diverso da [!DNL Google Drive] o [!DNL Gmail], queste restrizioni non sono applicabili.

Per istruzioni sulla connessione di altri [!DNL Google Services] a [!DNL Workfront Fusion], vedere [Connettere l&#39;app o il servizio Web del modulo a  [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) nell&#39;articolo [Creare uno scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Cosa devo fare se sono un utente [!DNL Google Workspace]? {#what-should-i-do-if-im-a-g-suite-user}

Non è richiesta alcuna azione.
