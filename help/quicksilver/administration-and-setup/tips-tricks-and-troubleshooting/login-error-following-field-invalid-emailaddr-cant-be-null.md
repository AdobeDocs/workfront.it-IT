---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Errore di accesso: I campi seguenti non sono validi: emailAddr non può essere null'
description: Quando provo ad accedere [!DNL Adobe Workfront] l'URL del mio dominio, vengo reindirizzato al portale di accesso SAML e quindi reindirizzato nuovamente a [!DNL Workfront] errore che indica che il campo emailAddr non può essere null.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 2%

---

# Errore di accesso: I campi seguenti non sono validi: emailAddr non può essere null

## Problema

Quando provo ad accedere [!DNL Adobe Workfront] con il mio URL (https://customerdomain.my.workfront.com), vengo reindirizzato al portale di accesso SAML e quindi reindirizzato nuovamente a [!DNL Workfront] con il seguente errore:

“Riproviamo. I campi seguenti non sono validi: emailAddr non può essere null.&quot;

## Causa

Questo errore è causato da un elemento non corretto nell’area Attributi utente mappa della configurazione SAML 2.0. Per ulteriori informazioni sulla mappatura degli attributi utente per SAML 2.0, consulta [Configurare Adobe Workfront con SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Soluzione

Aggiorna la Mappatura attributi per l&#39;indirizzo e-mail e fai clic su **[!UICONTROL Salva]**.
