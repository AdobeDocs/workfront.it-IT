---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Errore di accesso: i campi seguenti non sono validi: emailAddr non può essere null'
description: Quando si tenta di accedere all'URL  [!DNL Adobe Workfront]  del dominio, l'utente viene reindirizzato al portale di accesso SAML e quindi reindirizzato a  [!DNL Workfront]  con un errore che indica che il campo emailAddr non può essere nullo.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
TQID: https://experienceleague.adobe.com/MfWVOYcQAVjlbxwiqVaPwipyq5ulv0toajH-2tX7c9k
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 146
ht-degree: 4%

---

# Errore di accesso: i campi seguenti non sono validi: emailAddr non può essere null

## Problema

Quando si tenta di accedere a [!DNL Adobe Workfront] con il proprio URL (https://customerdomain.my.workfront.com), viene reindirizzato al portale di accesso SAML e quindi viene reindirizzato a [!DNL Workfront] con il seguente errore:

“Riproviamo. I campi seguenti non sono validi: emailAddr non può essere null.&quot;

## Causa

Questo errore è causato da un elemento non corretto nell’area Mappa attributi utente della configurazione SAML 2.0. Per ulteriori informazioni sul mapping degli attributi utente per SAML 2.0, vedere [Configurare Adobe Workfront con SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Soluzione

Aggiorna il mapping degli attributi per l&#39;indirizzo e-mail e fai clic su **[!UICONTROL Salva]**.
