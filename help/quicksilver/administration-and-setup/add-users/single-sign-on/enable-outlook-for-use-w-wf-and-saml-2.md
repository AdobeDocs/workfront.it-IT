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
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Abilitare Outlook per l&#39;utilizzo con Workfront e SAML 2.0

Se si attiva l&#39;autenticazione SAML 2.0 e si desidera consentire agli utenti di accedere a Workfront da Microsoft Outlook utilizzando le credenziali SAML 2.0, è necessario abilitare SAML 2.0 per l&#39;autenticazione nei componenti aggiuntivi di Office.

>[!NOTE]
>
>Questa opzione non è disponibile se l’istanza Workfront dell’organizzazione utilizza un portale SSO personalizzato.>
><!--
>or is enabled with Adobe IMS>
>-->
>Per ulteriori informazioni, rivolgersi all&#39;amministratore di rete o IT.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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
