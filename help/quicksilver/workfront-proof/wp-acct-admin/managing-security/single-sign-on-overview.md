---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Accesso singolo [!DNL Workfront Proof]
description: Single Sign-On (SSO) consente agli utenti di accedere [!DNL Workfront Proof] utilizzando il nome utente e la password esistenti della tua organizzazione.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Accesso singolo [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Un [!UICONTROL Enterprise] [!DNL Workfront] Per utilizzare questa funzione è necessario pianificare. Per ulteriori informazioni sui vari piani disponibili, vedi [Piani Workfront](https://www.workfront.com/plans).

Single Sign-On (SSO) consente agli utenti di accedere [!DNL Workfront Proof] utilizzando il nome utente e la password esistenti della tua organizzazione.

Per fornire questa funzionalità, utilizziamo [!DNL Security Assertion Markup Language] (SAML) 2.0, un protocollo basato su XML che consente di autorizzare i dati e scambiare l&#39;autenticazione tra un provider di identità e un servizio Web.

Ciò significa che ti autenticherai sul tuo sistema di accesso, non contro [!DNL Workfront Proof]Pagina di accesso di .

Devi avere un sottodominio personalizzato o un dominio configurato sul tuo [!DNL Workfront] Account di prova per abilitare SAML:

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* Per ulteriori informazioni sui domini completamente personalizzati in  [Marchio [!DNL Workfront Proof] sito - avanzato](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

Vedi [Configurare Single Sign-On per [!DNL Workfront Proof] utenti](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md) per informazioni sulla configurazione di SSO sul tuo account.
