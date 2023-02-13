---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)
description: Se l’organizzazione è stata integrata in Adobe Business Platform, gli utenti utilizzano Adobe Business Platform per accedere ad Adobe Workfront. Ciò significa che la gestione degli utenti avviene in gran parte tramite Adobe Admin Console e che l’accesso Single Sign-On (SSO) viene gestito tramite Adobe Business Platform anziché tramite Workfront. In qualità di amministratore di Adobe Workfront, le responsabilità e le procedure di amministrazione variano a seconda che l’organizzazione sia stata integrata in Adobe Business Platform. Questo articolo elenca le procedure che devono essere gestite in modo diverso e fornisce collegamenti alle istruzioni sia per Workfront che per Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: 137165deb0c0e9172224e810c82bc651bb0adfc0
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 1%

---

# Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)

Se l’organizzazione è stata integrata in Adobe Business Platform, gli utenti utilizzano Adobe Business Platform per accedere ad Adobe Workfront. Ciò significa che:

* La gestione degli utenti avviene in gran parte tramite Adobe Admin Console
* L’accesso Single Sign-On (SSO) viene gestito tramite Adobe Business Platform anziché tramite Workfront.

In qualità di amministratore di Adobe Workfront, le responsabilità e le procedure di amministrazione variano a seconda che l’organizzazione sia stata integrata in Adobe Business Platform. Questo articolo elenca le procedure che devono essere gestite in modo diverso e fornisce collegamenti alle istruzioni sia per Workfront che per Adobe Admin Console.

## Utenti

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Azione</th> 
   <th>Per istruzioni in Workfront, consulta</th> 
   <th>Per istruzioni su come utilizzare Adobe Admin Console, consulta</th> 
  </tr> 
 </thead> 
 <tbody> <!--
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
  --> 
  <tr> 
   <td role="rowheader">Concedere un accesso amministratore utente</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sezione "Modifica dettagli utente" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gestire gli utenti individualmente</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aggiungere un utente ad Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Aggiungi utenti</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Gestione degli utenti in Adobe Admin Console</a> </p> </li> 
     <li> <p>La sezione "Aggiungi utenti" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gestire gli utenti individualmente</a></p> </li> 
    </ul> </td> 
  </tr> <!--
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
  --> 
  <tr> 
   <td role="rowheader">Disattiva un utente</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Disattivare o riattivare un utente</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sezione "Rimuovi utenti" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gestire gli utenti individualmente</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Eliminare un utente</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Eliminare gli utenti</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sezione "Eliminare definitivamente gli utenti" in <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">Gestire gli utenti delle directory</a>
     </p><p>Nota: Eliminazione di un utente dal [!DNL Adobe Admin Console] disattiva l'utente in [!DNL Workfront], ma non eliminarli [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Modificare un profilo utente</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sezione "Modifica i dettagli utente" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gestire gli utenti individualmente</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Modifica in serie dei profili utente</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Modificare in blocco i profili utente</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sezione "Modifica dettagli utente" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Caricamento CSV in blocco</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Importare utenti </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importare utenti</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sezione "Aggiungi utenti" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Caricamento CSV in blocco</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Accedi come altro utente</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">Accedi come altro utente</a> </p> </li> 
    </ul> </td> 
   <td>Non disponibile</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rinnova certificato SAML</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Rinnovare il certificato metadati Adobe Workfront SAML 2.0</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sezione "La firma digitale nella risposta SAML non è stata convalidata..." in <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">Federated ID di risoluzione dei problemi</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## SSO (Single Sign-On)

Poiché Adobe Business Platform controlla l’accesso Single Sign-On (SSO) per gli utenti, le azioni e le funzionalità seguenti vengono gestite automaticamente tramite Adobe Business Platform. Se la tua organizzazione non è ancora stata caricata su Adobe Business Platform, devi eseguire queste azioni in Workfront.


* [Configurare Adobe Workfront con SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [Configurare Adobe Workfront con SAML 2.0 utilizzando ADFS](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Disattivazione del single sign-on in Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [Aggiornare i metadati SAML 2.0 nel provider di identità](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [Aggiornare gli utenti per il single sign-on](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [Configurare i criteri password per l&#39;autenticazione](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [Configurare le preferenze di sicurezza del sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
