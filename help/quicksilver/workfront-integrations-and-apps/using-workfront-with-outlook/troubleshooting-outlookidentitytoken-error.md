---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Risoluzione dei problemi: errore outlookIdentityToken durante l’utilizzo di Workfront per Outlook'
description: Se si verifica un errore outlookIdentityToken quando si utilizza Workfront per Outlook, è necessario abilitare i token legacy di Microsoft 365 per l'organizzazione.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 43%

---

# Risoluzione dei problemi: errore outlookIdentityToken durante l’utilizzo di Workfront per Outlook

>[!IMPORTANT]
>
>[Microsoft ha disabilitato il supporto per i token online di Exchange legacy](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), utilizzati dal componente aggiuntivo di Workfront Outlook per l&#39;autenticazione. Questa modifica apportata da Microsoft è stata implementata in più fasi ed è stata completata il 1° ottobre 2025.
>
>**Poiché Microsoft ha disabilitato questi token, l&#39;integrazione di Workfront per Microsoft Outlook non funziona più.**

Quando si utilizza Workfront per Outlook, è possibile che venga visualizzato il seguente errore:

```
Unexpected error
Unable to get the outlookIdentityToken
```

Per risolvere questo errore, è necessario abilitare i token legacy di Microsoft 365 per l’organizzazione. Poiché questo deve essere fatto in Microsoft 365, Workfront non può abilitare questi token per l’organizzazione.

Per istruzioni sull’abilitazione dei token legacy di Microsoft 365, consulta [Attivare o disattivare i token legacy di Exchange Online](https://learn.microsoft.com/it-it/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) nella documentazione di Microsoft.

Per ulteriori informazioni sui token legacy, consulta [È possibile riattivare i token legacy di Exchange Online?](https://learn.microsoft.com/it-it/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) nella documentazione di Microsoft.
