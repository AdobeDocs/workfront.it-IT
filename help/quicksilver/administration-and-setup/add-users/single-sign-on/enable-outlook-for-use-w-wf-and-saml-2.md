---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Abilita Outlook per l'uso con Workfront e SAML 2.0
description: Se si abilita l'autenticazione SAML 2.0 e si desidera che gli utenti siano in grado di accedere a Workfront da Microsoft Outlook utilizzando le proprie credenziali SAML 2.0, è necessario abilitare SAML 2.0 per l'autenticazione nei componenti aggiuntivi di Office.
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%

---

# Abilita Outlook per l&#39;uso con Workfront e SAML 2.0

Se si abilita l&#39;autenticazione SAML 2.0 e si desidera che gli utenti siano in grado di accedere a Workfront da Microsoft Outlook utilizzando le proprie credenziali SAML 2.0, è necessario abilitare SAML 2.0 per l&#39;autenticazione nei componenti aggiuntivi di Office.

>[!NOTE]
>
>Questa opzione non è disponibile se l&#39;istanza Workfront della tua organizzazione utilizza un portale SSO personalizzato.>
><!--
>or is enabled with Adobe IMS>
>-->
>Per ulteriori informazioni, rivolgiti al tuo amministratore di rete o IT.

## Requisiti di accesso

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Abilita Outlook per l&#39;uso con Workfront e SAML 2.0

1. Fai clic su **Configurazione** nell’angolo in alto a destra di Adobe Workfront sulla barra di navigazione globale.
1. Fai clic su **Sistema** > **Preferenze**.

1. In **Sicurezza** sezione , assicurati che **Consenti autenticazione SAML 2.0 nei componenti aggiuntivi di Office 365**&#x200B;è abilitato.

   Questa opzione consente di incorporare Workfront in un Iframe solo per i componenti aggiuntivi di Office 365. Questo non apre una violazione di click-jacking in quanto non è coinvolto alcun contenuto cliccabile.

   Questa opzione è attivata per impostazione predefinita.

   >[!NOTE]
   >
   >Se abiliti l’opzione **Consenti incorporazione di Workfront in un iframe**, l’opzione **Consenti autenticazione SAML 2.0 nei componenti aggiuntivi di Office 365** è oscurato e abilitato.
   >
   >![](assets/if-you-enable.png)

1. Fai clic su **Salva**.

   Le modifiche salvate qui influiscono sull’esperienza di tutti gli utenti in Workfront.
