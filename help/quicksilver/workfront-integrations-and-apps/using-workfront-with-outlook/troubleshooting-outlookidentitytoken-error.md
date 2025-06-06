---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Risoluzione dei problemi: errore outlookIdentityToken durante l’utilizzo di Workfront per Outlook'
description: Se si verifica un errore outlookIdentityToken quando si utilizza Workfront per Outlook, è necessario abilitare i token legacy di Microsoft 365 per l'organizzazione.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 31%

---

# Risoluzione dei problemi: errore outlookIdentityToken durante l’utilizzo di Workfront per Outlook

>[!IMPORTANT]
>
>Microsoft [È in corso la disabilitazione del supporto per i token online di Exchange legacy](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), attualmente utilizzati dal componente aggiuntivo di Workfront Outlook per l&#39;autenticazione. Questa modifica di Microsoft ha già iniziato a interessare i clienti e continuerà a essere implementata in più fasi fino a ottobre 2025.
>
>* **Dopo la completa disattivazione di questi token da parte di Microsoft, l&#39;integrazione di Workfront per Microsoft Outlook non funzionerà più.**
>
>Come parte di questa modifica, Microsoft ha deciso di cambiare il modo in cui i token vengono riabilitati. Dopo il **30 giugno 2025**, gli amministratori non saranno più in grado di riabilitare i token personalmente. Solo il supporto Microsoft può concedere eccezioni. **Il 1° ottobre 2025, i token legacy verranno disattivati per tutti i tenant. Le eccezioni non verranno concesse.**


Quando si utilizza Workfront per Outlook, è possibile che venga visualizzato il seguente errore:

```
Unexpected error
Unable to get the outlookIdentityToken
```

Per risolvere questo errore, è necessario abilitare i token legacy di Microsoft 365 per l’organizzazione. Poiché questo deve essere fatto in Microsoft 365, Workfront non può abilitare questi token per l’organizzazione.

Per istruzioni sull’abilitazione dei token legacy di Microsoft 365, consulta [Attivare o disattivare i token legacy di Exchange Online](https://learn.microsoft.com/it-it/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) nella documentazione di Microsoft.

Per ulteriori informazioni sui token legacy, consulta [È possibile riattivare i token legacy di Exchange Online?](https://learn.microsoft.com/it-it/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) nella documentazione di Microsoft.
