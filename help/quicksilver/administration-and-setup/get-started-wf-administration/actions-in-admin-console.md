---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Differenze di amministrazione basate sulla piattaforma (Adobe Workfront/Adobe Business Platform)
description: Se la tua organizzazione è stata integrata in Adobe Business Platform, gli utenti utilizzano Adobe Business Platform per accedere ad Adobe Workfront. Ciò significa che la gestione degli utenti viene in gran parte eseguita tramite Adobe Admin Console e che il Single Sign-On (SSO) viene gestito tramite la piattaforma aziendale Adobe anziché tramite Workfront. In qualità di amministratore di Adobe Workfront, le responsabilità e le procedure di amministrazione variano a seconda che l’organizzazione sia stata integrata o meno in Adobe Business Platform. In questo articolo sono elencate le procedure che devono essere gestite in modo diverso e sono disponibili collegamenti alle istruzioni per Workfront e Adobe Admin Console.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: c71c5c4a545f9256ecce123ae3513d01a7251ad7
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)

<!--DELETE ME MARCH 2026-->

>[!IMPORTANT]
>
>Tutte le organizzazioni Workfront ora sono state integrate in Adobe Admin Console.
>
>Questo articolo verrà rimosso a breve.

In qualità di amministratore di Adobe Workfront, le responsabilità e le procedure di amministrazione possono variare a seconda che l’organizzazione sia stata integrata o meno in Adobe Business Platform. In questo articolo sono elencate le procedure gestite in modo diverso e sono presenti collegamenti alle istruzioni per Workfront e Adobe Admin Console.

Se la tua organizzazione è stata integrata in Adobe Business Platform, gli utenti utilizzano Adobe Business Platform per accedere ad Adobe Workfront. Ciò significa che:

* Gli amministratori di sistema vengono creati tramite Adobe Admin Console
* Il rinnovo di un certificato SAML viene gestito tramite Adobe Admin Console.
* Il Single Sign-On (SSO) viene gestito tramite Adobe Business Platform anziché tramite Workfront

## Creazione di amministratori di sistema Workfront in Adobe Admin Console

>[!NOTE]
>
>È consigliabile aggiungere utenti non amministratori di sistema direttamente in Workfront. È possibile aggiungere utenti in Adobe Admin Console, ma aggiungerli in Workfront consente di impostarne il livello di accesso durante la creazione, con un conseguente risparmio di tempo.

Per istruzioni sulla creazione degli amministratori di sistema di Workfront, vedere [Gestione degli utenti in Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Action</th> 
   <th>For instructions in Workfront, see</th> 
   <th>For instructions in the Adobe Admin console, see</th> 
  </tr> 
 </thead> 
 <tbody> 
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">View information about access levels and licenses for your users</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md" class="MCXref xref">List your users' access levels and licenses</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p>The section "View user list" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Grant a user admin access</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Add a user to Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
     <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Add a user to Adobe Workfront Fusion</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../workfront-fusion/organizations/add-user-to-an-organization.md" class="MCXref xref">Add a user to an organization in Adobe Workfront Fusion</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
      <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Deactivate a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Remove users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Delete a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Delete users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Permanently delete users" in <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">Manage directory users</a>
     </p><p>Note: Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Edit a user profile</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bulk edit user profiles</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Edit user profiles in bulk</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Import users </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Import users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Add users" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Log in as another user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">Log in as another user</a> </p> </li> 
    </ul> </td> 
   <td>Not available</td> 
  </tr> 
  <tr> 
    -->

## Rinnovare il certificato SAML

Per istruzioni sul rinnovo del certificato SAML sul Adobe Admin Console, vedere la sezione &quot;La firma digitale nella risposta SAML non è stata convalidata...&quot; in [Risoluzione dei problemi di Federated ID](https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html)

<!--

   <td role="rowheader">Renew SAML certificate</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Renew the Adobe Workfront SAML 2.0 metadata certificate</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "The digital signature in the SAML response did not validate..." in <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">Troubleshooting Federated ID</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

-->

## SSO (Single Sign-On)

Poiché Adobe Business Platform controlla il Single Sign-On (SSO) per gli utenti, le azioni e le funzionalità seguenti vengono gestite automaticamente tramite Adobe Business Platform. Se la tua organizzazione non è ancora stata integrata in Adobe Business Platform, devi eseguire queste azioni in Workfront.


* [Configura Adobe Workfront con SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [Configurazione di Adobe Workfront con SAML 2.0 tramite ADFS](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Disattivare il Single Sign-On in Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [Aggiorna metadati SAML 2.0 nel provider di identità](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [Aggiorna utenti per Single Sign-On](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [Configura criteri password per l&#39;autenticazione](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [Configurare le preferenze di sicurezza del sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
