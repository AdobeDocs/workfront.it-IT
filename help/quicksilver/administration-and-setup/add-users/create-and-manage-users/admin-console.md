---
title: Gestione degli utenti in Adobe Admin Console
description: In qualità di amministratore di Adobe, puoi creare utenti e amministratori di sistema Adobe Workfront utilizzando Adobe Admin Console.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: ae657964-d4a5-4c3b-afc6-8dde7695955d
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# Gestione degli utenti in Adobe Admin Console

>[!IMPORTANT]
>
>La funzionalità di questo articolo è disponibile solo se l’istanza di Workfront della tua organizzazione è stata caricata su Adobe Business Platform.
>
>Per un elenco delle procedure che differiscono a seconda che l’organizzazione sia stata imbarcata in Adobe Business Platform, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

In qualità di amministratore di Adobe, puoi creare utenti e amministratori di sistema Adobe Workfront utilizzando Adobe Admin Console. La console è una posizione centrale per la gestione delle adesioni Adobe in tutta l’organizzazione. Per ulteriori informazioni, consulta la sezione [Panoramica dell’Admin Console](https://helpx.adobe.com/it/enterprise/using/admin-console.html).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Diritti di amministratore di Adobe</td> 
   <td> <p>Devi essere un amministratore di configurazione del prodotto per i prodotti Adobe per la tua organizzazione</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisiti

Prima di utilizzare l’Admin Console per Workfront, riceverai una e-mail di invito alla console.

1. Se hai ricevuto un&#39;e-mail che ti informa che ora disponi dei diritti di amministratore per gestire il software e i servizi Adobe per la tua organizzazione, fai clic sul pulsante nell&#39;e-mail per creare un account Adobe e aprire l&#39;Admin Console.

   Oppure

   Se disponi già di un account di Adobe, passa alla pagina [Pagina Adobe Admin Console](https://adminconsole.adobe.com/).

## Accedi all’area utente e amministratore per la tua istanza Production di Workfront {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}

1. Da [Pagina Adobe Admin Console](https://adminconsole.adobe.com/), seleziona **Prodotti** nella barra di navigazione superiore, quindi seleziona la **Workfront** riquadro del prodotto.

   ![](assets/admin-product-1.png)

1. Nell’elenco visualizzato, seleziona il collegamento in alto.

   Questa è l’istanza Production in cui lavorano gli utenti.

   ![](assets/instances-1.png)

   >[!TIP]
   >
   >L’istanza Preview, il secondo collegamento nell’elenco, è un ambiente di test che replica l’ambiente di produzione live. Per ulteriori informazioni, consulta [Ambiente Sandbox di anteprima di Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).
   >
   >
   >Nell’elenco potrebbero inoltre essere presenti collegamenti agli ambienti sandbox. Per ulteriori informazioni, consulta [Ambiente Sandbox di anteprima di Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

1. Nell’elenco visualizzato, con la **Profili di prodotto** , fai clic sul nome del collegamento Profilo di prodotto Workfront .

   ![](assets/prod-profile-1.png)

   Questo elenco include tutti gli utenti che sono già assegnati alla tua istanza Production di Workfront.

   >[!IMPORTANT]
   >
   >Non apportare alcuna modifica al profilo di prodotto stesso.

1. Procedi a una delle seguenti sezioni del presente articolo:

   * [Creare utenti in Workfront con Adobe Admin Console](#create-users-in-workfront-with-the-adobe-admin-console)
   * [Creare amministratori di sistema in Workfront con Adobe Admin Console](#create-system-administrators-in-workfront-with-the-adobe-admin-console)

## Creare utenti in Workfront con Adobe Admin Console {#create-users-in-workfront-with-the-adobe-admin-console}

1. Vai all’area utente e amministratore nell’Admin Console, come descritto in [Accedi all’area utente e amministratore per la tua istanza Production di Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) in questo articolo.
1. Con la **Utenti** scheda selezionata sopra l’elenco, seleziona **Aggiungi utente**.
1. In **Aggiungi utenti a questo profilo di prodotto** immettere l&#39;indirizzo e-mail o il nome dell&#39;utente che si desidera aggiungere, quindi selezionare **Salva**.

   L’utente viene creato in Workfront con il livello di accesso Richiedente.

   >[!IMPORTANT]
   >
   >Non apportare alcuna modifica al profilo di prodotto stesso.

1. In Workfront, modifica il livello di accesso dell’utente.

   Per istruzioni su come un amministratore di Workfront può modificare il livello di accesso dell’utente, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Ripetere i passaggi 3 e 4 per aggiungere altri utenti.

   >[!NOTE]
   >
   >Per i nuovi utenti di Adobe, l’Admin Console invia un messaggio e-mail per invitarli a completare il processo di registrazione. Tutti gli utenti devono completare il processo di registrazione per accedere a qualsiasi sistema di Adobe.
   >
   >Per gli utenti esistenti di Adobe, l’utente potrebbe ricevere o meno un’e-mail sulla disponibilità di Workfront. Si tratta di una preferenza controllata dall’amministratore di Adobe per il prodotto.

## Creare amministratori di sistema in Workfront con Adobe Admin Console {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

Il livello di accesso amministratore di sistema viene concesso solo su Adobe Admin Console. Non puoi concedere o rimuovere l&#39;accesso amministratore da Workfront.

È necessario aggiungere un utente all&#39;istanza Production di Workfront prima di rendere l&#39;utente un amministratore di sistema di Workfront. Per istruzioni, consulta [Creare utenti in Workfront con Adobe Admin Console](#create-users-in-workfront-with-the-adobe-admin-console) in questo articolo.

1. Vai all’area utente e amministratore nell’Admin Console, come descritto in [Accedi all’area utente e amministratore per la tua istanza Production di Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) in questo articolo.
1. Seleziona la **Amministratori** sopra l’elenco degli utenti.
1. Seleziona **Aggiungi amministratore**.
1. In **Aggiungi amministratori del profilo di prodotto** immettere gli indirizzi e-mail o i nomi degli amministratori che si desidera aggiungere, quindi selezionare **Salva**.

   ![](assets/add-admin-1.png)

   Gli amministratori di sistema vengono creati in Workfront.

   >[!IMPORTANT]
   >
   >Non apportare alcuna modifica al profilo di prodotto stesso.

## Ulteriori dettagli su Adobe Admin Console:

* Gli amministratori di sistema di Workfront possono disattivare un utente Workfront dall’interno di Workfront, ma questo non disattiva l’utente nell’Admin Console.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about deactivating a user in Workfront, see </p>
  -->

* Utente **Gruppo Home** viene determinato in base all’utente che li ha creati. Al momento non è personalizzabile dall’interno dell’Admin Console.
* È possibile modificare il livello di accesso dell’amministratore di sistema di Workfront solo da Adobe Admin Console.

   <!--
  DRAFTED IN FLARE:
  How is this done?
  
  -->

* La modifica di un utente che è amministratore di sistema a qualsiasi altro livello di accesso deve essere eseguita prima tramite l’Admin Console .

   <!--
   This is not clear
  -->

* Per rimuovere l’accesso amministratore di sistema da un utente in Workfront, è necessario utilizzare Adobe Admin Console per rimuovere l’utente come amministratore del profilo di prodotto. Questo cambia il livello di accesso Workfront dell&#39;utente da Amministratore di sistema a Richiedente.

   >[!IMPORTANT]
   >
   >Non apportare alcuna modifica al profilo di prodotto stesso.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>You can create Adobe Workfront users and system administrators with the <a href="https://adminconsole.adobe.com/" alt="Admin Console link">Adobe Admin Console</a>. The console is a central location for managing the Adobe entitlements across your organization. For more information, see the <a href="https://helpx.adobe.com/enterprise/using/admin-console.html" alt="Admin Console Overview">Admin Console Overview</a>.</p>
<p>Before using the Admin Console for Workfront, you should receive a receive an email inviting you to the console. Click in the invitation to accept it and create an account. You can also use an existing account, if already available.</p>
<h2>Create users</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Create users in WF with the Adobe admin console</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">May need to add something about oging throug WF -- check with Jonah</p>

<p>To create users in Workfront with the Admin Console:</p>
<ol>
<li value="1"> <p>From the <a href="https://adminconsole.adobe.com/">Admin Console page</a>, select the <b>Products</b> tab and then select the <b>Workfront</b> product tile.</p> </li>
<li value="2"> <p>Select the link to the Workfront instance you want to change.</p> </li>
<li value="3"> <p>Select the Product profile link. This shows a list of the currently-assigned users. If the list is very long, you can also search for users in the search field above the list.</p> </li>
<li value="4"> <p>Select the <b>Add User</b> button.</p> </li>
<li value="5"> <p>In the <b>Add users</b> box, enter the email address or name of the user you want to add. Select <b>Save</b>. The administrator is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Create system administrators</h2>
<p>To create system administrators:</p>
<ol>
<li value="1"> <p>Make product profile assignments first. To be a Workfront System Administrator, the user must be assigned the Workfront product profile and be an admin for that product profile.</p> </li>
<li value="2"> <p>From the console, select the <b>Products</b> tab and then select the <b>Admins</b> tab. </p> </li>
<li value="3"> <p>Select <b>Add Admin</b>.</p> </li>
<li value="4"> <p>In the <b>Add product profile administrators</b> box, enter the email address or name of the administrator you want to add. Select <b>Save</b>. The user is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Additional details for the Admin Console</h2>
<ul>
<li> <p>System Administrator access level is granted only on the Admin Console. You cannot grant or remove admin access from within Workfront.</p> </li>
</ul>
<ul>
<li> <p>Creating and deleting users inside Workfront is only possible through the Admin Console.</p> </li>
<li> <p>Workfront System Administrators can deactivate Workfront users from within Workfront, but this does not deactivate the user in the Admin Console.</p> </li>
<li> <p>All new users are are assigned <b>Requestor</b> access level upon creation. Also, the user <b>Home Group</b> is determined based on the user who created them. This is currently not customizable from within the Admin Console.</p> </li>
<li> <p>The Workfront System Administrator access level can only be edited from within the Adobe Admin Console.</p> </li>
<li> <p>Editing a user who is a system admin to any other access level must be done through the Admin Console first.</p> </li>
<li> <p>To remove Workfront system admin access, remove users as Product Profile Administrators. This action changes the user access level in Workfront from a system admin to a <b>Requestor</b>.</p> </li>
</ul>
</div>
-->
