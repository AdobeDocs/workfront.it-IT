---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: E-mail non autenticata non accettata a causa dei criteri DMARC del dominio
description: Se un messaggio di posta elettronica inviato dal sistema [!DNL Workfront] non viene accettato a causa dei criteri DMARC del dominio, l'amministratore della posta elettronica può risolvere il problema configurando il sistema di posta elettronica per consentire tutti i messaggi di posta elettronica da workfront.com.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
TQID: 'https://experienceleague.adobe.com/f44Wkid-gwfXgHKmSKa6oevhN5jA6720JTlOcH8kJKY'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 1%
---
# L’e-mail non autenticata non è accettata a causa dei criteri DMARC del dominio

## Problema

[Test] Ho ricevuto il seguente messaggio di mancato recapito:

550-5.7.1 L’e-mail non autenticata da &quot;customer domain.com&quot; non è accettata a causa di\
550-5.7.1 del dominio DMARC. Contatta l’amministratore di &quot;customer domain.com&quot;\
550-5.7.1 se si trattava di una posta legittima. Visita\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) per informazioni su DMARC\
550 5.7.1 iniziativa.

## Soluzione

DMARC è configurato nel sistema di posta elettronica della tua azienda e non fa parte di [!DNL Adobe Workfront]. Se ricevi questa e-mail, devi contattare l’amministratore della posta elettronica.

L’amministratore della posta elettronica deve configurare il sistema di posta elettronica in modo da consentire/considerare attendibili i messaggi di posta elettronica provenienti da noreply@workfront.com o, preferibilmente, tutti i messaggi di posta elettronica provenienti da workfront.com.

Per ulteriori informazioni su DMARC, vedere [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)
