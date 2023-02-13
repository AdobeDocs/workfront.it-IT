---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''Errore: Gli utenti SSO non possono accedere a [!DNL Adobe Workfront] A causa di vari errori"'
description: Quando ricevi un errore di accesso su single sign-on federato, la combinazione nome utente/password o l'accesso a [!DNL Workfront], the problem might be that your [!DNL Workfront] L'istanza utilizza SSO e stai tentando di accedere utilizzando un URL errato. Assicurati di accedere utilizzando l'URL corretto senza alcun elemento dopo ".com".
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 13%

---

# Errore: Gli utenti SSO non possono accedere a [!DNL Adobe Workfront] A causa di vari errori

## Problema

Non riesco ad accedere a [!DNL Workfront] e ha ricevuto uno dei seguenti errori:

* Non puoi accedere [!DNL Workfront] tramite questa schermata di accesso. [!DNL Workfront] è configurato per Federated Single Sign-On con SAML 2.0. Contatta il tuo [!DNL Workfront] amministratore.
* Combinazione Non Valido di username/password
* Spiacenti, non si dispone dell&#39;accesso a [!DNL Workfront]. Contatta il tuo [!DNL Workfront] amministratore per ottenere un nome utente e una password.

## Soluzione

Le [!DNL Workfront] L&#39;istanza utilizza SSO e stai tentando di accedere tramite un URL errato. Assicurati di accedere utilizzando l&#39;URL corretto senza alcun elemento dopo &quot;.com&quot;

>[!TIP]
>
>Rimuovi eventuali segnalibri esistenti con URL non validi.
