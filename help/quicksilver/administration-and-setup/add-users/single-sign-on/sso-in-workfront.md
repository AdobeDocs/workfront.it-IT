---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Panoramica del single sign-on in Adobe Workfront
description: Workfront fornisce una configurazione SSO (Single Sign-On) gestita a livello centrale che integra facilmente Workfront con la soluzione SSO aziendale esistente. Questa configurazione è facile da configurare e gestire ed è disponibile per i clienti OnDemand e OnPremise Enterprise.
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Panoramica del single sign-on in Adobe Workfront

{{important-admin-console-onboard}}


Workfront fornisce una configurazione SSO (Single Sign-On) gestita a livello centrale che integra facilmente Workfront con la soluzione SSO aziendale esistente. Questa configurazione è facile da configurare e gestire ed è disponibile per i clienti OnDemand e OnPremise Enterprise.

Per utilizzare la funzionalità SSO in Workfront, l&#39;organizzazione deve configurare un&#39;applicazione SSO. Puoi quindi configurare Workfront in modo che possa comunicare con la tua soluzione SSO.

Le soluzioni federate consentono agli utenti di accedere a tutte le applicazioni immettendo il proprio nome utente e password in un portale di accesso centralizzato.

![](assets/overview-sso-wf.png)


## Configurare il firewall

Quando si utilizza una soluzione SSO, Workfront avvia una connessione al server sulla porta specificata.

Se ti abboni a Workfront on-demand e se hai configurato il firewall o il server di posta elettronica per consentire l’accesso solo a fornitori specifici, devi aggiungere alcuni indirizzi IP Workfront al tuo inserire nell&#39;elenco Consentiti firewall. Per ulteriori informazioni, consulta [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configurare Single Sign-On

Workfront si integra con le seguenti soluzioni SSO:

* Soluzioni federate che supportano SAML 2.0

   Per informazioni sull&#39;integrazione di Workfront con SAML 2.0, vedi [Configurare Adobe Workfront con SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

* Soluzioni federate che supportano SAML 2.0 utilizzando ADFS

   Per informazioni sull&#39;integrazione di Workfront con SAML 2.0 utilizzando ADFS, vedi [Configurare Adobe Workfront con SAML 2.0 utilizzando ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
