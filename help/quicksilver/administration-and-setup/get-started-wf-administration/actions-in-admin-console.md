---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)
description: Se la tua organizzazione è stata integrata in Adobe Business Platform, gli utenti utilizzano Adobe Business Platform per accedere ad Adobe Workfront. Ciò significa che la gestione degli utenti viene in gran parte eseguita tramite Adobe Admin Console e che il Single Sign-On (SSO) viene gestito tramite Adobe Business Platform anziché tramite Workfront. In qualità di amministratore di Adobe Workfront, le responsabilità e le procedure di amministrazione variano a seconda che l’organizzazione sia stata integrata o meno in Adobe Business Platform. In questo articolo sono elencate le procedure che devono essere gestite in modo diverso e sono disponibili collegamenti alle istruzioni per Workfront e Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: b476c012f825afc4bc48b7172be26accc6bac0d1
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 1%

---

# Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)

Se la tua organizzazione è stata integrata in Adobe Business Platform, gli utenti utilizzano Adobe Business Platform per accedere ad Adobe Workfront. Ciò significa che:

* Gli amministratori di sistema vengono creati tramite Adobe Admin Console
* Il Single Sign-On (SSO) viene gestito tramite Adobe Business Platform anziché tramite Workfront

In qualità di amministratore di Adobe Workfront, le responsabilità e le procedure di amministrazione variano a seconda che l’organizzazione sia stata integrata o meno in Adobe Business Platform. In questo articolo sono elencate le procedure gestite in modo diverso e sono presenti collegamenti alle istruzioni per Workfront e Adobe Admin Console.

## Utenti



>[!NOTE]
>
>È consigliabile aggiungere utenti non amministratori di sistema direttamente in Workfront. È possibile aggiungere utenti in Adobe Admin Console, ma aggiungerli in Workfront consente di impostarne il livello di accesso durante la creazione, con un conseguente risparmio di tempo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Azione</th> 
   <th>Per istruzioni in Workfront, consulta</th> 
   <th>Per istruzioni in Admin Console di Adobe, consulta</th> 
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
   <td role="rowheader">Concedere a un amministratore utenti l’accesso</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sezione "Modifica dettagli utente" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gestire gli utenti singolarmente</a></p> </li> 
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
     <li> <p>La sezione "Aggiungere utenti" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gestire gli utenti singolarmente</a></p> </li> 
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
   <td role="rowheader">Disattivare un utente</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Disattivare o riattivare un utente</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sezione "Rimuovere gli utenti" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gestire gli utenti singolarmente</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Eliminare un utente</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Elimina utenti</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sezione "Eliminare definitivamente gli utenti" in <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">Gestire gli utenti della directory</a>
     </p><p>Nota: eliminazione di un utente da [!DNL Adobe Admin Console] disattiva l'utente in [!DNL Workfront], ma non li elimina da [!DNL Workfront].</p> </li> 
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
     <li> <p>La sezione "Modifica dettagli utente" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gestire gli utenti singolarmente</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Modifica in blocco dei profili utente</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Modificare i profili utente in blocco</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sezione "Modifica dettagli utente" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Caricamento CSV in blocco</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Importa utenti </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importa utenti</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sezione "Aggiungere utenti" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Caricamento CSV in blocco</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Accedere come un altro utente</td> 
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
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Rinnovare il certificato di metadati SAML 2.0 di Adobe Workfront</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La sezione "La firma digitale nella risposta SAML non è stata convalidata..." in <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">Federated ID di risoluzione dei problemi</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## SSO (Single Sign-On)

Poiché Adobe Business Platform controlla il Single Sign-On (SSO) per gli utenti, le azioni e le funzionalità seguenti vengono gestite automaticamente tramite Adobe Business Platform. Se la tua organizzazione non è ancora stata integrata in Adobe Business Platform, devi eseguire queste azioni in Workfront.


* [Configurare Adobe Workfront con SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [Configurare Adobe Workfront con SAML 2.0 utilizzando ADFS](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Disattivare il single sign-on in Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [Aggiornamento dei metadati SAML 2.0 nel provider di identità](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [Aggiornare gli utenti per il Single Sign-On](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [Configura criteri password per l&#39;autenticazione](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [Configurare le preferenze di sicurezza del sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
