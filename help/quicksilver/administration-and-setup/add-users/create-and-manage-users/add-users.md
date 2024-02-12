---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Aggiungi utenti
description: In qualità di amministratore di Workfront o di utente con accesso amministrativo completo, puoi aggiungere utenti in Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: b476c012f825afc4bc48b7172be26accc6bac0d1
workflow-type: tm+mt
source-wordcount: '1229'
ht-degree: 1%

---

# Aggiungi utenti

>[!IMPORTANT]
>
>Se la tua organizzazione è stata integrata in Adobe Admin Console, devi creare gli amministratori di sistema tramite Adobe Admin Console.
>
>Per istruzioni sulla creazione di amministratori di sistema in Adobe Admin Console, consulta [Gestione degli utenti in Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>Gli amministratori di gruppi nelle organizzazioni che hanno effettuato l’onboarding in Adobe Admin Console possono utilizzare questa procedura per creare utenti e inviare l’utente per l’approvazione dell’amministratore.
>
>Per un elenco delle procedure che differiscono in base al fatto che la tua organizzazione sia stata onboarding in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Puoi aggiungere utenti in Adobe Workfront creando singoli utenti da zero o copiando quelli esistenti.

Per informazioni su come importare più utenti contemporaneamente, consulta [Importa utenti](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

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
   <td> <p>È necessario disporre di uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Livello di accesso Amministratore di sistema. Per informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>. </p> </li> 
     <li> <p><b>Utenti</b> impostazione nel livello di accesso configurato su <b>Modifica</b> accesso, con <b>Crea</b> e almeno uno dei due <b>Amministratore utenti</b> opzioni abilitate in <b>Metti a punto le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se Utente <b>Amministratore (utenti gruppo)</b> è abilitato, è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> <p>Per ulteriori informazioni su <b>Utenti</b> impostazione in un livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisiti

Prima di aggiungere un utente, raccogliere le informazioni sull&#39;utente elencate di seguito e determinare quali informazioni si desidera associare all&#39;utente:

* Quali sono le informazioni personali dell&#39;utente? Come minimo sono necessari i seguenti elementi:

   * Nome e cognome
   * Un nome utente
   * Password predefinita
   * Indirizzo e-mail

  >[!NOTE]
  >
  >È possibile determinare se gli utenti possono visualizzare le informazioni di contatto di altri utenti regolando l&#39;impostazione Visualizzazione utenti quando si specificano i livelli di accesso per gli oggetti Workfront. Per ulteriori informazioni, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Qual è la posizione del nuovo utente all’interno dell’azienda? Questa persona ha dei referenti diretti? A chi si riferisce questa persona?
* Quale ruolo occupa la persona? Questo ruolo esiste in Workfront? Esiste un limite al numero di persone che possono ricoprire questo ruolo? Per informazioni sulla creazione di ruoli, consulta [Creare e gestire le mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* Quale livello di accesso deve avere l’utente? Esiste già o è necessario crearne una nuova? Per ulteriori informazioni, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* In quale gruppo predefinito deve essere l&#39;utente? La persona deve appartenere a più gruppi? Per informazioni sui gruppi, consulta [Panoramica sui gruppi](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* In quale team principale deve essere incluso questo utente? La persona dovrebbe far parte di più team? Per informazioni sui team, consulta [Panoramica sui team](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* Quali informazioni personalizzate è necessario associare a questo utente?

  Se le informazioni sugli utenti vengono acquisite nei campi personalizzati creati, è necessario disporre di un modulo personalizzato durante la creazione di un utente. Per informazioni sui moduli personalizzati, consulta [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Creare un utente da zero

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).

1. Clic **Nuovo utente > Nuovo utente** per aggiungere un utente che non è ancora stato aggiunto a Workfront.

   Oppure

   Clic **Nuovo utente > Importa utenti** per aggiungere utenti caricando un file di importazione foglio di calcolo.

   Se importi gli utenti, non è necessario continuare questi passaggi. Per ulteriori informazioni, consulta [Importa utenti](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. In **Nuovo utente** visualizzata, fare clic su **Mostra opzioni avanzate**, quindi configura le opzioni disponibili per immettere le informazioni della persona.

   Per informazioni su queste opzioni, vedi [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Esegui una delle operazioni seguenti:

   * Esci **Invia un&#39;e-mail di invito a questa persona** abilitato. In questo caso, l’utente riceve un’e-mail in cui può seguire un collegamento per creare una propria password per Workfront. Gli utenti che non accettano l’invito e-mail e che creano una password Workfront vengono elencati come Non registrati in Workfront.
   * Disattiva **Invia un&#39;e-mail di invito a questa persona**, quindi digita un **Password** per la persona e confermarlo nel **Conferma password** casella. Dovrai condividere questa password con l’utente al di fuori di Workfront.

   >[!NOTE]
   >
   >Se l’amministratore di Workfront ha abilitato un’integrazione SSO con Workfront, l’opzione Consenti solo &lt;sso configuration=&quot;&quot;> Il campo Autenticazione è nascosto se disattivi l’invito e-mail. L’ID federazione o &lt;sso configuration=&quot;&quot;> Il campo Nome utente rimane visibile.

   >[!NOTE]
   >
   Se la tua organizzazione è stata integrata nell’Admin Console e aggiungi un utente tramite Workfront, non puoi inviare un invito e-mail.
   >
   I nuovi utenti dell’Adobe vengono aggiunti all’Admin Console Admin Console, che a sua volta distribuisce un’e-mail per invitarli a completare la procedura di registrazione. Tutti gli utenti devono completare la procedura di registrazione per accedere a qualsiasi Adobe.
   >
   Per gli Adobi esistenti, l’utente potrebbe ricevere o meno un’e-mail sulla disponibilità di Workfront. Questa è una preferenza controllata dall’amministratore di Adobe per il prodotto.

1. Clic **Aggiungi questo utente**.

   Oppure

   Clic **Aggiungi utente persona e avviane un altro** per salvare il nuovo utente e aggiungerne un altro.

   >[!NOTE]
   >
   Se sei un amministratore gruppo e aggiungi un utente a un’organizzazione che è stata integrata in Adobe Admin Console, le opzioni per questo passaggio sono **Invia utente per approvazione dell&#39;amministratore** e **Invia per approvazione e avviane un altro**. L’utente viene creato con lo stato Disattivato e In attesa di approvazione. Un amministratore di Workfront deve approvare l’utente, che lo attiva in Workfront e lo aggiunge al Adobe Admin Console.

## Copiare un utente per crearne uno nuovo

Puoi creare un utente copiandone uno esistente.

>[!NOTE]
>
Quando si crea un utente in questo modo, tutte le informazioni vengono copiate dall&#39;utente originale all&#39;utente appena creato, ad eccezione dei seguenti elementi:
>
* Le informazioni nella sezione Informazioni personali.
* Quando effettuo l’accesso, mostra: in questa casella è selezionata la scheda di destinazione predefinita per il livello di accesso.
* I Report Diretti
>

Per creare un nuovo utente copiandone uno esistente:

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).
1. Seleziona l’utente da copiare, quindi fai clic sull’icona Copia ![](assets/copy-icon.png).
1. In **Nuovo utente** in cui viene visualizzato, modificare i campi disponibili per il nuovo utente.

   Per informazioni su tutti i campi associati a un utente, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Clic **Aggiungi questo utente**.

   Oppure

   Clic **Aggiungi utente persona e avviane un altro** per salvare il nuovo utente e aggiungerne un altro.

In questo modo viene creato un nuovo account in Workfront per l’utente.

Se hai selezionato l’opzione per inviare un invito all’utente, questo dovrebbe ricevere un’e-mail in cui può seguire un collegamento per creare la password Workfront.

>[!NOTE]
>
Se la tua organizzazione è stata integrata nell’Admin Console e aggiungi un utente tramite Workfront, non puoi inviare un invito e-mail.
>
I nuovi utenti dell’Adobe vengono aggiunti all’Admin Console Admin Console, che a sua volta distribuisce un’e-mail per invitarli a completare la procedura di registrazione. Tutti gli utenti devono completare la procedura di registrazione per accedere a qualsiasi Adobe.
>
Per gli Adobi esistenti, l’utente potrebbe ricevere o meno un’e-mail sulla disponibilità di Workfront. Questa è una preferenza controllata dall’amministratore di Adobe per il prodotto.
