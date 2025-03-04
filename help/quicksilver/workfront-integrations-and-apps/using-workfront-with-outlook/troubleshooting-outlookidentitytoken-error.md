---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Risoluzione dei problemi: errore outlookIdentityToken durante l’utilizzo di Workfront per Outlook'
description: Se si verifica un errore outlookIdentityToken quando si utilizza Workfront per Outlook, è necessario abilitare i token legacy di Microsoft 365 per l'organizzazione.
author: Becky
feature: Workfront Integrations and Apps
source-git-commit: 77cc1acde87b2ada96117daa06e98ba38e64fa8a
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Risoluzione dei problemi: errore outlookIdentityToken durante l’utilizzo di Workfront per Outlook

Quando si utilizza Workfront per Outlook, è possibile che venga visualizzato il seguente errore:

```
Unexpected error
Unable to get the outlookIdentityToken
```

Per risolvere questo errore, devi abilitare i token legacy di Microsoft 365 per la tua organizzazione. Poiché questo deve essere fatto in Microsoft 365, Workfront non può abilitare questi token per la tua organizzazione.

Per istruzioni sull&#39;abilitazione dei token legacy di Microsoft 365, consulta [Attivare o disattivare i token legacy di Exchange Online](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) nella documentazione di Microsoft.

Per ulteriori informazioni sui token di accesso, vedere [È possibile riattivare i token legacy di Exchange Online?](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) nella documentazione di Microsoft.
