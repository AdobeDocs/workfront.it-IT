---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Errore: gli utenti SSO non possono accedere a  [!DNL Adobe Workfront] a causa di vari errori'
description: Quando ricevi un errore di accesso relativo al Single Sign-On federato, alla combinazione nome utente/password o all'accesso all'istanza  [!DNL Workfront], the problem might be that your [!DNL Workfront]  utilizza l'SSO e stai tentando di accedere con un URL errato.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
TQID: https://experienceleague.adobe.com/8L78zoOjC2KgtVKTorhvWDd8MvaficRL2pZKOfrlGSs
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
source-wordcount: 166
ht-degree: 4%

---

# Errore: gli utenti SSO non possono accedere a [!DNL Adobe Workfront] a causa di vari errori

## Problema

Non è possibile accedere a [!DNL Workfront] e si è verificato uno dei seguenti errori:

* Spiacenti, impossibile accedere a [!DNL Workfront] tramite questa schermata di accesso. [!DNL Workfront] è configurato per il Single Sign-On federato con SAML 2.0. Contattare l&#39;amministratore [!DNL Workfront].
* La combinazione nome utente/password non è corretta. Verifica che il blocco maiuscole non sia attivato e riprova.
* Non si dispone dell&#39;accesso a [!DNL Workfront]. Contattare l&#39;amministratore [!DNL Workfront] per ottenere un nome utente e una password.

## Soluzione

L&#39;istanza [!DNL Workfront] utilizza l&#39;SSO e si sta tentando di accedere con un URL errato. Assicurati di effettuare l’accesso con l’URL corretto senza utilizzare nulla dopo &quot;.com&quot;

>[!TIP]
>
>Rimuovi eventuali segnalibri esistenti con URL non validi.
