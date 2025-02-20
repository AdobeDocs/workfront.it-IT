---
title: Gestire gli utenti in Adobe Admin Console
description: In qualità di amministratore di Adobe, puoi creare utenti e amministratori di sistema di Adobe Workfront utilizzando Adobe Admin Console.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: ae657964-d4a5-4c3b-afc6-8dde7695955d
source-git-commit: f9dea6c80c0d681e3638c9baf36e6e511693b59c
workflow-type: tm+mt
source-wordcount: '1322'
ht-degree: 0%

---

# Gestione degli utenti in Adobe Admin Console

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

>[!IMPORTANT]
>
>La funzionalità di questo articolo è disponibile solo se l’istanza di Workfront della tua organizzazione è stata integrata in Adobe Business Platform.
>
>Per un elenco delle procedure che differiscono a seconda che l&#39;organizzazione sia stata integrata o meno in Adobe Business Platform, consulta [Differenze di amministrazione basate su Platform (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

In qualità di amministratore di Adobe, puoi creare amministratori di sistema di Adobe Workfront utilizzando Adobe Admin Console. La console è una posizione centrale per la gestione delle adesioni Adobe in tutta l’organizzazione. Per ulteriori informazioni, vedere [Panoramica di Admin Console](https://helpx.adobe.com/it/enterprise/using/admin-console.html).

>[!NOTE]
>
>È consigliabile aggiungere utenti non amministratori di sistema direttamente in Workfront. È possibile aggiungere utenti in Adobe Admin Console, ma aggiungerli in Workfront consente di impostarne il livello di accesso durante la creazione, con un conseguente risparmio di tempo.

<span class="preview">Quando si apportano modifiche ai profili degli utenti da Admin Console, viene aggiunto un aggiornamento alla scheda Attività di sistema dell&#39;utente in Workfront. L’aggiornamento viene visualizzato come effettuato dal &quot;Sistema&quot;. Si riferisce all&#39;amministratore di Adobe Admin Console e non all&#39;amministratore principale di Workfront.</span>

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td> <p>Devi essere amministratore della configurazione del prodotto dei prodotti Adobe per la tua organizzazione</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di utilizzare Admin Console per Workfront, dovresti ricevere un’e-mail di invito alla console.

1. Se hai poca esperienza con Adobe e hai ricevuto un’e-mail che ti diceva che ora disponi dei diritti di amministrazione per gestire il software e i servizi Adobe per la tua organizzazione, fai clic sul pulsante nell’e-mail per creare un account Adobe e aprire Admin Console.

   Oppure

   Se disponi già di un account Adobe, passa alla [pagina Adobe Admin Console](https://adminconsole.adobe.com/).

## Dettagli aggiuntivi su Adobe Admin Console

* Gli amministratori di sistema di Workfront possono disattivare un utente Workfront da Workfront, ma questo non disattiva l’utente in Admin Console.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about deactivating a user in Workfront, see </p>
  -->

* L&#39;utente **Gruppo predefinito** è determinato in base all&#39;utente che li ha creati. Questo non è personalizzabile dall’interno di Admin Console.
* Il livello di accesso Amministratore di sistema di Workfront può essere modificato solo dall&#39;interno di Adobe Admin Console.

  <!--
  DRAFTED IN FLARE:
  How is this done?
  
  -->

* Il passaggio dell’accesso di un utente da Amministratore di sistema a qualsiasi altro livello di accesso deve essere eseguito innanzitutto tramite Admin Console.

  <!--
   This is not clear
  -->

* Per rimuovere l’accesso come amministratore di sistema da un utente in Workfront, è necessario utilizzare Adobe Admin Console per rimuovere l’utente come amministratore del profilo di prodotto. In questo modo il livello di accesso Workfront dell&#39;utente cambia da Amministratore di sistema a Richiedente.

  >[!IMPORTANT]
  >
  >Non apportare modifiche al profilo di prodotto stesso.

* Gli amministratori di Adobe Admin Console possono impostare regole di assegnazione automatica per automatizzare il processo di assegnazione dei prodotti Adobe agli utenti della propria organizzazione. Per ulteriori informazioni e istruzioni, consulta [Gestire le regole di assegnazione automatica](https://helpx.adobe.com/enterprise/using/automatic-assignment-rules.html) nella documentazione di Adobe.

## Accedi all’area utente e amministrazione per l’istanza Production di Workfront {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}

1. Dalla [pagina Adobe Admin Console](https://adminconsole.adobe.com/), seleziona la scheda **Prodotti** nella barra di navigazione superiore, quindi seleziona **Workfront**.

   <!--![Admin Console product](assets/admin-product-1.png)-->

1. Nell’elenco visualizzato, seleziona il collegamento in alto.

   Questa è l’istanza di produzione in cui lavorano gli utenti.

   <!--![Admin Console instances](assets/instances-1.png)-->

   >[!TIP]
   >
   >Il secondo collegamento nell’elenco, l’istanza Anteprima, è un ambiente di test che replica l’ambiente di produzione live. Per ulteriori informazioni, consulta [Ambiente Sandbox di anteprima di Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).
   >
   >
   >Nell’elenco potrebbero essere visualizzati anche i collegamenti agli ambienti sandbox. Per ulteriori informazioni, consulta [Ambiente Sandbox di anteprima di Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

1. Nell&#39;elenco visualizzato, con la scheda **Profili di prodotto** selezionata, fare clic sul collegamento Profilo di prodotto Workfront.

   ![Profili di prodotto](assets/prod-profile-1.png)

   Questo elenco include tutti gli utenti già assegnati all’istanza Production di Workfront.

   >[!IMPORTANT]
   >
   >Non apportare modifiche al profilo di prodotto stesso.

1. Passare a una delle sezioni seguenti in questo articolo:

   * [Creare utenti in Workfront con Adobe Admin Console](#create-users-in-workfront-with-the-adobe-admin-console)
   * [Creazione di amministratori di sistema in Workfront con Adobe Admin Console](#create-system-administrators-in-workfront-with-the-adobe-admin-console)

## Creazione di amministratori di sistema in Workfront con Adobe Admin Console {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

<!--Audited: 12/2023-->

Il livello di accesso Amministratore di sistema è concesso solo su Adobe Admin Console. Non puoi concedere o rimuovere l’accesso come amministratore da Workfront.

È necessario aggiungere un utente all&#39;istanza Production di Workfront prima di poter impostare l&#39;utente come amministratore di sistema di Workfront.

1. Vai all&#39;area utenti e amministratori in Admin Console, come descritto nella sezione [Accedi all&#39;area utenti e amministratori per l&#39;istanza di produzione di Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) in questo articolo.
1. Seleziona la scheda **Amministratori** sopra l&#39;elenco degli utenti.
1. Selezionare **Aggiungi amministratore**.
1. Nella casella **Aggiungi amministratori profilo prodotto**, inserisci gli indirizzi e-mail o i nomi degli amministratori che desideri aggiungere, quindi seleziona **Salva**.

   ![Aggiungi un amministratore](assets/add-admin-1.png)

   Gli amministratori di sistema vengono creati in Workfront.

   >[!IMPORTANT]
   >
   >Non apportare modifiche al profilo di prodotto stesso.


## Creare utenti in Workfront con Adobe Admin Console {#create-users-in-workfront-with-the-adobe-admin-console}

>[!NOTE]
>
>È consigliabile aggiungere utenti non amministratori di sistema direttamente in Workfront. È possibile aggiungere utenti in Adobe Admin Console, ma aggiungerli in Workfront consente di impostarne il livello di accesso durante la creazione, con un conseguente risparmio di tempo.

* [Creazione di utenti in Workfront direttamente in Adobe Admin Console](#create-users-in-workfront-directly-in-the-adobe-admin-console)
* [Creare utenti in Workfront e approvarli per Adobe Admin Console](#create-users-in-workfront-and-approve-them-for-the-adobe-admin-console)

### Creazione di utenti in Workfront direttamente in Adobe Admin Console

1. Vai all&#39;area utenti e amministratori in Admin Console, come descritto nella sezione [Accedi all&#39;area utenti e amministratori per l&#39;istanza di produzione di Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) in questo articolo.
1. Con la scheda **Utenti** selezionata sopra l&#39;elenco, selezionare **Aggiungi utente**.
1. Nella casella **Aggiungi utenti a questo profilo di prodotto**, inserisci l&#39;indirizzo e-mail o il nome di un utente che desideri aggiungere, quindi seleziona **Salva**.

   L’utente viene creato in Workfront con il livello di accesso Richiedente.

   >[!IMPORTANT]
   >
   >Non apportare modifiche al profilo di prodotto stesso.

1. In Workfront, modifica il livello di accesso dell’utente.

   Per istruzioni su come un amministratore di Workfront può modificare il livello di accesso dell&#39;utente, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Ripeti i passaggi 3 e 4 per aggiungere altri utenti.

   >[!NOTE]
   >
   >Per i nuovi utenti di Adobe, l’Admin Console fornisce un’e-mail per invitarli a completare il processo di registrazione. Tutti gli utenti devono completare il processo di registrazione per accedere a qualsiasi applicazione Adobe.
   >
   >Per gli utenti esistenti di Adobe, l’utente può ricevere o meno un’e-mail sulla disponibilità di Workfront. Questa è una preferenza controllata dall’amministratore di Adobe per il prodotto. L’amministratore Adobe potrebbe essere una persona diversa dall’amministratore Workfront.

### Creare utenti in Workfront e approvarli per Adobe Admin Console

Questo flusso di lavoro consente agli amministratori di gruppi che non hanno accesso a Adobe Admin Console di creare utenti.

Innanzitutto, l’amministratore del gruppo crea l’utente in Workfront. L’utente viene quindi impostato sullo stato Disattivato e In attesa di approvazione.

Quindi, un amministratore Workfront approva l’utente. In questo modo l’utente viene attivato in Workfront e aggiunto al Adobe Admin Console.

#### Creare l’utente in Workfront (amministratore gruppo)

Per istruzioni sulla creazione di un utente in Workfront, vedi [Aggiungere utenti](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/add-users.md).

#### Approva l&#39;utente (amministratore Workfront)

Per approvare un utente:

{{step-1-to-users}}

1. Seleziona l&#39;utente, quindi fai clic sull&#39;icona **Altro** ![Altro](assets/more-icon.png).

1. Per approvare l&#39;utente, fare clic su **Approva**, quindi su **Invia**.

   Oppure

   Per rifiutare l&#39;utente ed eliminarlo da Workfront, fare clic su **Rifiuta**, quindi su **Invia**.

   Gli utenti approvati vengono aggiunti automaticamente al Adobe Admin Console.

   Gli utenti rifiutati vengono eliminati automaticamente da Workfront.






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
