---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Abilitare Outlook per l'utilizzo con Workfront e SAML 2.0
description: Se si attiva l'autenticazione SAML 2.0 e si desidera consentire agli utenti di accedere a Workfront da Microsoft Outlook utilizzando le credenziali SAML 2.0, è necessario abilitare SAML 2.0 per l'autenticazione nei componenti aggiuntivi di Office.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 1%

---

# Abilitare Outlook per l&#39;utilizzo con Workfront e SAML 2.0

>[!IMPORTANT]
>
>Microsoft [È in corso la disabilitazione del supporto per i token online di Exchange legacy](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), attualmente utilizzati dal componente aggiuntivo di Workfront Outlook per l&#39;autenticazione. Questa modifica di Microsoft ha già iniziato a interessare i clienti e continuerà a essere implementata in più fasi fino a ottobre 2025.
>
>* **Dopo la completa disattivazione di questi token da parte di Microsoft, l&#39;integrazione di Workfront per Microsoft Outlook non funzionerà più.**
>
>Come parte di questa modifica, Microsoft ha deciso di cambiare il modo in cui i token vengono riabilitati. Dopo il **30 giugno 2025**, gli amministratori non saranno più in grado di riabilitare i token personalmente. Solo il supporto Microsoft può concedere eccezioni. **Il 1° ottobre 2025, i token legacy verranno disattivati per tutti i tenant. Le eccezioni non verranno concesse.**

Se si attiva l&#39;autenticazione SAML 2.0 e si desidera consentire agli utenti di accedere a Workfront da Microsoft Outlook utilizzando le credenziali SAML 2.0, è necessario abilitare SAML 2.0 per l&#39;autenticazione nei componenti aggiuntivi di Office.

>[!NOTE]
>
>Questa opzione non è disponibile se l’istanza Workfront dell’organizzazione utilizza un portale SSO personalizzato.>
>
>Per ulteriori informazioni, rivolgersi all&#39;amministratore di rete o IT.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Standard</p><p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Abilitare Outlook per l&#39;utilizzo con Workfront e SAML 2.0

{{step-1-to-setup}}

1. Fare clic su **Sistema** > **Preferenze**.

1. Nella sezione **Sicurezza**, verificare che **Consenti autenticazione SAML 2.0 nei componenti aggiuntivi di Office 365** sia abilitato.

   Questa opzione consente di incorporare Workfront in un Iframe solo per i componenti aggiuntivi di Office 365. Questa operazione non apre una violazione del click-jacking, in quanto non è presente alcun contenuto cliccabile.

   Questa opzione è attivata per impostazione predefinita.

   >[!NOTE]
   >
   >Se si abilita l&#39;opzione **Consenti incorporamento di Workfront in un iframe**, l&#39;opzione **Consenti autenticazione SAML 2.0 nei componenti aggiuntivi di Office 365** è disabilitata e abilitata.
   >
   >![Opzione Consenti incorporamento](assets/if-you-enable.png)
   >

1. Fai clic su **Salva**.

   Le modifiche salvate qui influiscono sull’esperienza di tutti gli utenti in Workfront.
