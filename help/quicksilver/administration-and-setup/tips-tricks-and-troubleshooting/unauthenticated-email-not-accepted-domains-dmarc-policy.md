---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Quando un'e-mail autenticata non viene accettata a causa dei criteri DMARC del dominio
description: Se un’e-mail è stata inviata da [!DNL Workfront] sistema non accettato a causa dei criteri DMARC del dominio, l'amministratore di posta elettronica può risolvere il problema configurando il sistema di posta elettronica per consentire tutte le e-mail da workfront.com.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Le e-mail non autenticate non sono accettate a causa dei criteri DMARC del dominio

## Problema

[Test] Ho ricevuto il seguente messaggio e-mail non recapitato:

550-5.7.1 L&#39;e-mail non autenticata da &quot;customer domain.com&quot; non è accettata a causa di\
Criteri DMARC del dominio 550-5.7.1. Contattare l&#39;amministratore di &quot;customer domain.com&quot;\
Dominio 550-5.7.1 se questa era una posta legittima. Visita\
550-5,7,1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) per informazioni sul DMARC\
550 5.7.1.

## Soluzione

Il DMARC è configurato nel sistema e-mail della tua azienda e non fa parte del [!DNL Adobe Workfront]. Se ricevi questa e-mail, contatta l’amministratore e-mail.

L’amministratore dell’e-mail deve configurare il sistema e-mail per consentire/fidare l’e-mail da noreply@workfront.com o preferibilmente tutte le e-mail da workfront.com.

Per ulteriori informazioni sul DMARC, vedi [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)
