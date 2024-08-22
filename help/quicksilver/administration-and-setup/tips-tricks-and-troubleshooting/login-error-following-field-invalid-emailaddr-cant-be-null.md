---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Errore di accesso: i campi seguenti non sono validi: emailAddr non può essere null"
description: Quando si tenta di accedere all'URL  [!DNL Adobe Workfront]  del dominio, l'utente viene reindirizzato al portale di accesso SAML e quindi reindirizzato a  [!DNL Workfront]  con un errore che indica che il campo emailAddr non può essere nullo.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 2%

---

# Errore di accesso: i campi seguenti non sono validi: emailAddr non può essere null

## Problema

Quando si tenta di accedere a [!DNL Adobe Workfront] con il proprio URL (https://customerdomain.my.workfront.com), viene reindirizzato al portale di accesso SAML e quindi viene reindirizzato a [!DNL Workfront] con il seguente errore:

“Riproviamo. I campi seguenti non sono validi: emailAddr non può essere null.&quot;

## Causa

Questo errore è causato da un elemento non corretto nell’area Mappa attributi utente della configurazione SAML 2.0. Per ulteriori informazioni sul mapping degli attributi utente per SAML 2.0, vedere [Configurare Adobe Workfront con SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Soluzione

Aggiorna il mapping degli attributi per l&#39;indirizzo e-mail e fai clic su **[!UICONTROL Salva]**.
