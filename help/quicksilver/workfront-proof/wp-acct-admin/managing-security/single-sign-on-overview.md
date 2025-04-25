---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Single Sign-On in [!DNL Workfront Proof]
description: Single Sign-On (SSO) consente agli utenti di accedere a [!DNL Workfront Proof] utilizzando il nome utente e la password esistenti dell'organizzazione.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Accesso singolo in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

Per utilizzare questa funzionalità è necessario un piano [!UICONTROL Enterprise] [!DNL Workfront]. Per ulteriori informazioni sui vari piani disponibili, vedere [Piani Workfront](https://business.adobe.com/products/workfront/pricing.html).

Single Sign-On (SSO) consente agli utenti di accedere a [!DNL Workfront Proof] utilizzando il nome utente e la password esistenti dell&#39;organizzazione.

Per fornire questa funzionalità, viene utilizzato [!DNL Security Assertion Markup Language] (SAML) 2.0, un protocollo basato su XML che consente di autorizzare i dati e di scambiare l&#39;autenticazione tra un provider di identità e un servizio Web.

Ciò significa che effettuerai l&#39;autenticazione in base al tuo sistema di accesso e non in base alla pagina di accesso di [!DNL Workfront Proof].

Per abilitare SAML, è necessario che nel proprio account di verifica [!DNL Workfront] siano impostati sottodomini o domini personalizzati:

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* Puoi trovare ulteriori informazioni sui domini completamente personalizzati in [Personalizza il  [!DNL Workfront Proof] sito - avanzato](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

Consulta [Configurare Single Sign-On per [!DNL Workfront Proof] utenti](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md) per informazioni sulla configurazione di SSO nel tuo account.
