---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Credenziali utente di Adobe Workfront vs. [!DNL SAML] credenziali utente
description: Dopo la creazione dell'utente, è possibile modificare l'utente e abilitare "Consenti solo autenticazione SAML 2.0" in modo che l'utente e la password siano controllati dal sistema SAML. Con questa opzione abilitata, l’utente può accedere solo tramite SAML. Quando passano al [!DNL Workfront] URL, vengono automaticamente reindirizzati al sistema SAML e viene richiesto il nome utente e la password SAML.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Credenziali utente di Adobe Workfront e credenziali utente SAML

Questo articolo si concentra in particolare sui seguenti argomenti: [!DNL Adobe Workfront] e SAML e non coprono altri metodi di autenticazione SSO.

In un database, [!DNL Workfront] memorizza l&#39;indirizzo e-mail di ogni utente come proprio [!DNL Workfront] nome utente e [!DNL Workfront] password. Queste credenziali vengono replicate nelle Sandbox di anteprima e aggiornamento personalizzato.

Durante la creazione dell&#39;utente, se [!DNL Workfront] rileva che SAML 2.0 è configurato, per impostazione predefinita l&#39;utente utilizza &quot;Consenti solo autenticazione SAML 2.0&quot;. Se la casella &quot;Invia un invito a questa persona&quot; è abilitata, [!DNL Workfront] disabilita &quot;Consenti solo autenticazione SAML 2.0&quot; e nasconde questa opzione. Una volta che &quot;Invia un invito a questa persona&quot; è abilitato, l&#39;utente diventa un non SAML [!DNL Workfront] utente.

Dopo la creazione dell’utente, puoi modificare l’utente e abilitare **[!UICONTROL Consenti solo autenticazione SAML 2.0]** in modo che l&#39;utente e la password siano controllati dal sistema SAML.

A questo scopo, l’utente può accedere solo tramite SAML. Quando passano al [!DNL Workfront] URL, vengono automaticamente reindirizzati al sistema SAML e viene richiesto il nome utente e la password SAML.

Le credenziali SAML sono memorizzate in un sistema SAML esterno, ad esempio ADFS Microsoft, non in Workfront.
