---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Configurare l’accesso alle bozze di un utente
description: In qualità di amministratore Adobe Workfront o amministratore Workfront Proof, puoi configurare l’accesso di un utente per creare e visualizzare bozze in Workfront e Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
TQID: 'https://experienceleague.adobe.com/L-AMDvQYgtXJwxmtwekimbEA9OQQN72QHIcoQ2iKzGU'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4ea8bc003ce17978be5e5a6fd838012dfcfeae78
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 6%
---
# Configurare l’accesso alle bozze di un utente

In qualità di amministratore Adobe Workfront o amministratore Workfront Proof, puoi configurare l’accesso di un utente per creare e visualizzare bozze in Workfront e Workfront Proof.

Per informazioni sulle funzionalità di verifica disponibili per la verifica di base e integrata, vedere [Accesso alla funzionalità di verifica in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

Per eseguire i passaggi descritti in questo articolo, devi disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Devi essere un amministratore di Workfront o di Workfront Proof. Per informazioni sugli amministratori di Workfront, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

+++

<!--

## Configure a user's proof permission profile

The permission profile you select is granted to the users for each proof that exists within your organization.

{{step-1-to-users}}
 
1. Select one or more users, then click **Edit**.  

1. In the **Access** section, click one of the following Workfront Proof permission options in the **Proof Permission Profile** drop-down menu:

   >[!NOTE]
   >
   >If you are on a legacy Workfront plan, make sure the **User can generate proofs** option is enabled, as explained above in the section [Enable and disable proofing for a user (legacy plans only)](#enable-and-disable-proofing-for-a-user-legacy-plans-only). 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisor</strong> </td> 
      <td>Users can manage and view all proofs created on your organization's account. They can also edit reviewers added to these proofs. Users with this permission profile can't manage users or edit Workfront Proof settings.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Manager</strong> </td> 
      <td> <p> Users can manage and view proofs created or owned on your organization's account. They can view other users' proofs only when added as a reviewer. This is a default setting. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrator</strong> </td> 
      <td> Users are given Administrator permissions in Workfront Proof and can edit account settings. Users can manage and view all proofs created on your organization's account. This includes adding and removing reviewers, proofs, and comments.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Custom</strong> </td> 
      <td> <p>Available only if you have configured a custom permission profile within Workfront Proof.</p> <p><b>NOTE</b>:  <p>Ensure that the permission profile you grant here does not provide higher access than the user's Access Level setting in Workfront (see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>). If it does provide higher access, the user can access proofs within Workfront Proof that he or she cannot access within Workfront.</p> <p>This is especially important if you plan to allow all Workfront users to access Workfront Proof directly from the Workfront as described in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Access Workfront Proof from Adobe Workfront</a>.</p> <p>By default, only Workfront administrators have access to a direct link to the Workfront Proof site from the Workfront Global Navigation Bar.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   The permission profile you select is granted to the users for each proof that exists within your organization.

1. Click **Save Changes** to complete the update to the user settings.

   >[!NOTE]
   >
   >When you create or update a user in Workfront and the user's Workfront email address matches that of a licensed Workfront Proof user, the system enables proofing for the user within Workfront. For more information, see [User synchronization between Adobe Workfront and Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considerations

Consider the following information when setting permissions:

* If you change a user's permission profile to a profile with fewer permissions, the user might lose visibility to existing proofs within Workfront. This can occur when someone shares a task with a user within Workfront, but doesn't share the proof attached to the task (see [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* You can set Workfront Proof permissions from Workfront only if your Workfront environment is integrated with a Workfront Proof Premium account. If you cannot use proofing as discussed in this section, contact your Workfront administrator.
* At least one user in your Workfront environment must have Administrator permissions for proofing. An error message appears if you try to attempt to remove Administrator permissions for proofing from all users.
* When you change a user's Workfront Access level to any level other than System Administrator, the user's Workfront Proof permission profile defaults to Manager.   

* When you change the Workfront Access level to System Administrator, the Proof Permission profile changes to Administrator.

-->

## Configurare l’accesso a Workfront Proof tramite il menu principale di Workfront per tutti gli utenti {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

Per impostazione predefinita, solo gli utenti con diritti amministrativi in Workfront possono accedere a Workfront Proof come descritto [Accedere a Workfront Proof da Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

È possibile concedere a tutti gli utenti l&#39;accesso al pulsante Workfront Proof nel menu principale di Workfront contattando il supporto Workfront e inviando una richiesta.

>[!IMPORTANT]
>
> Se prevedi di consentire a tutti gli utenti di Workfront di accedere a Workfront Proof direttamente dalla barra di navigazione globale di Workfront, accertati che il profilo di autorizzazione per ogni utente non fornisca un accesso maggiore del livello di accesso dell’utente in Workfront. Questo impedisce agli utenti di accedere alle prove all’interno di Workfront Proof a cui non possono accedere in Workfront. Per ulteriori informazioni, vedere [Abilitare e disabilitare la verifica per un utente (solo piani legacy)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Configurare l&#39;accesso utente al Visualizzatore bozze desktop

Se gli utenti dell’organizzazione preferiscono utilizzare il Visualizzatore bozze desktop anziché il Visualizzatore bozze web per rivedere il contenuto interattivo, è possibile configurare il Visualizzatore bozze desktop in modo che venga avviato automaticamente quando gli utenti aprono le bozze dei contenuti interattivi. Per informazioni su questo visualizzatore di bozze per il desktop e sulle differenze rispetto al visualizzatore di bozze per il Web, vedere [Comprendere il visualizzatore di bozze per il desktop](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) e [Differenze tra il visualizzatore di bozze per il Web e la panoramica del visualizzatore di bozze per il desktop](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. Da Workfront, fai clic sull’icona Workfront Proof nella barra di navigazione globale per accedere a Workfront Proof.

   ![Icona bozza](assets/proof-access-proofhq-350x39.png)

1. Fai clic su **Impostazioni account** nell&#39;angolo superiore destro di Workfront Proof, quindi fai clic sulla scheda **Impostazioni**.

1. In **Proof Defaults**, alla fine della riga **Desktop Proofing Viewer for Interactive proofing**, fare clic su **Setup**.

1. Modificare le impostazioni del Visualizzatore bozze desktop, come descritto in [Visualizzatore bozze desktop](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) nell&#39;articolo [Configurare le impostazioni della bozza per l&#39;organizzazione](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Fai clic su **Salva**.

## Configurare dispositivi personalizzati per le bozze interattive

È possibile aggiungere qualsiasi dispositivo personalizzato al sistema, consentendo agli utenti di esaminare il contenuto interattivo e simulare la modalità di visualizzazione del contenuto su un dispositivo specifico quando utilizzano il Visualizzatore bozze desktop. Questa funzionalità non è disponibile nel visualizzatore bozze web, in cui gli utenti possono esaminare il contenuto interattivo, ma solo come viene visualizzato in varie risoluzioni, non su dispositivi diversi.

Per ulteriori informazioni, vedere [Modificare la risoluzione della bozza interattiva nel visualizzatore di bozze](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. Da Workfront, accedere all&#39;interfaccia di Workfront Proof, come descritto in [Accedere a Workfront Proof da Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. Modificare le impostazioni del Visualizzatore bozze desktop, come descritto in [Configurare dispositivi personalizzati per le bozze](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) nell&#39;articolo [Configurare le impostazioni della bozza per l&#39;organizzazione](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
