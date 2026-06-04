---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Credenziali utente di Adobe Workfront e credenziali utente SAML
description: Dopo la creazione dell’utente, puoi modificarlo e abilitare "Only Allow SAML 2.0 Authentication" (Consenti solo autenticazione SAML 2.0) in modo che l’utente e la password siano controllati dal sistema SAML. Se questa opzione è abilitata, l’utente può accedere solo tramite SAML.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
TQID: https://experienceleague.adobe.com/8paS2GIumamOltxTC8Gw2mBZ4bKB6TOgbly7IBPKhDw
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
source-wordcount: 235
ht-degree: 0%

---

# Credenziali utente Adobe Workfront e credenziali utente SAML

Questo articolo si concentra specificamente su [!DNL Adobe Workfront] e SAML e non copre altri metodi di autenticazione SSO.

In un database, [!DNL Workfront] memorizza l&#39;indirizzo e-mail di ogni utente come nome utente [!DNL Workfront], insieme alla password [!DNL Workfront]. Queste credenziali vengono replicate nelle Sandbox di anteprima e aggiornamento personalizzato.

Durante la creazione dell&#39;utente, se [!DNL Workfront] rileva che SAML 2.0 è configurato, per impostazione predefinita viene impostato su &quot;Consenti solo autenticazione SAML 2.0&quot; per l&#39;utente. Se la casella &quot;Send an invite email to this person&quot; (Invia un&#39;e-mail di invito a questa persona) è abilitata, [!DNL Workfront] disabilita &quot;Only Allow SAML 2.0 Authentication&quot; (Consenti solo autenticazione SAML 2.0) e nasconde questa opzione. Dopo aver abilitato &quot;Send an invite email to this person&quot; (Invia un&#39;e-mail di invito a questa persona), l&#39;utente diventa un utente [!DNL Workfront] non SAML.

Dopo la creazione dell&#39;utente, è possibile modificare l&#39;utente e abilitare **[!UICONTROL Consenti solo autenticazione SAML 2.0]** in modo che l&#39;utente e la password siano controllati dal sistema SAML.

Al termine, l’utente può accedere solo tramite SAML. Quando arrivano all&#39;URL [!DNL Workfront], vengono automaticamente reindirizzati al sistema SAML e viene richiesto di immettere il nome utente e la password SAML.

Le credenziali SAML vengono memorizzate in un sistema SAML esterno, ad esempio ADFS di Microsoft, non in Workfront.
