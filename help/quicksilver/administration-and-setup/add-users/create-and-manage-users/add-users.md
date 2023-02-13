---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Aggiungi utenti
description: In qualità di amministratore Workfront o di utente con accesso amministrativo completo, puoi aggiungere utenti in Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# Aggiungi utenti

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state integrate nell’Admin Console. Se l’organizzazione è stata configurata per Adobe Admin Console, devi eseguire questa azione tramite Adobe Admin Console.
>
>Per istruzioni su come aggiungere un utente in Adobe Admin Console:
>
>* Vedi [Creare utenti in Workfront con Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create)
>* Vedi la sezione &quot;Aggiungi utenti&quot; nell&#39;articolo [Gestire gli utenti individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Contattare l&#39;amministratore Adobe Admin Console.
>
>Per un elenco delle procedure che variano a seconda che l’organizzazione sia stata caricata in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Puoi aggiungere utenti in Adobe Workfront creando singoli utenti da zero o copiando quelli esistenti.

Per informazioni su come importare più utenti contemporaneamente, consulta [Importare utenti](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi disporre di una delle seguenti caratteristiche:</p> 
    <ul> 
     <li> <p>Livello di accesso amministratore di sistema. Per informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>. </p> </li> 
     <li> <p><b>Utenti</b> impostazione nel livello di accesso configurato per <b>Modifica</b> accesso, con <b>Crea</b> e almeno uno dei due <b>Amministratore utente</b> opzioni attivate in <b>Ottimizzare le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se Utente <b>Amministratore (utenti del gruppo)</b> è abilitato, devi essere un amministratore di gruppo di un gruppo in cui l’utente è membro.</p> <p>Per ulteriori informazioni sulla <b>Utenti</b> impostazione in un livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisiti

Prima di aggiungere un utente, raccogliere le informazioni relative all’utente elencato di seguito e determinare quali informazioni si desidera associare a tale utente:

* Quali sono le informazioni personali dell&#39;utente? Come minimo è necessario quanto segue:

   * Nome completo
   * Un nome utente
   * Password predefinita
   * Indirizzo e-mail

   >[!NOTE]
   >
   >È possibile determinare se gli utenti possono visualizzare le informazioni di contatto di altri utenti regolando in modo preciso l&#39;impostazione Visualizzazione utenti quando si specificano i livelli di accesso per gli oggetti Workfront. Per ulteriori informazioni, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Qual è la posizione del nuovo utente all’interno dell’azienda? Questa persona ha dei rapporti diretti? A chi riferisce questa persona?
* Quale ruolo occupa la persona? Questo ruolo di lavoro esiste in Workfront? Esiste un limite al numero di persone che possono svolgere questo ruolo? Per informazioni sulla creazione di ruoli di lavoro, consulta [Creare e gestire ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* Che livello di accesso deve avere l’utente? Esiste già o è necessario crearne uno nuovo? Per ulteriori informazioni, consulta [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* In quale home group dovrebbe essere questo utente? La persona dovrebbe essere in più di un gruppo? Per informazioni sui gruppi, consulta [Panoramica sui gruppi](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* In quale team principale deve trovarsi questo utente? La persona dovrebbe essere in più di una squadra? Per informazioni sui team, consulta [Panoramica sui team](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* Quali informazioni personalizzate è necessario associare a questo utente?

   Se le informazioni sugli utenti vengono acquisite nei campi personalizzati creati dall’utente, è necessario che il modulo personalizzato sia pronto per la creazione di un utente. Per informazioni sui moduli personalizzati, consulta [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Creare un utente da zero

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).

1. Fai clic su **Nuovo utente > Nuovo utente** per aggiungere un utente che non è ancora stato aggiunto a Workfront.

   Oppure

   Fai clic su **Nuovo utente > Importa utenti** per aggiungere utenti caricando un file di importazione di fogli di calcolo.

   Se stai importando degli utenti, non è necessario continuare questi passaggi. Per ulteriori informazioni, consulta [Importare utenti](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. In **Nuovo utente** casella visualizzata, fai clic su **Mostra opzioni avanzate**, quindi configura le opzioni disponibili per immettere le informazioni della persona.

   Per informazioni su queste opzioni, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Esegui una delle operazioni seguenti:

   * Esci **Invia un messaggio e-mail di invito a questa persona** abilitato. In questo caso, l’utente riceve un’e-mail in cui può seguire un collegamento per creare la propria password per Workfront. Gli utenti che non accettano l’invito e-mail e creano una password Workfront sono elencati come Non registrati in Workfront.
   * Disattiva **Invia un messaggio e-mail di invito a questa persona**, quindi digita a **Password** per la persona e confermarla nel **Conferma password** scatola. Dovrai condividere questa password con l’utente esterno a Workfront.

   >[!NOTE]
   >
   >Se l&#39;amministratore Workfront ha abilitato un&#39;integrazione SSO con Workfront, l&#39;opzione Consenti solo &lt;sso configuration=&quot;&quot;> Il campo di autenticazione è nascosto se disattivi l’invito e-mail. ID federazione o &lt;sso configuration=&quot;&quot;> Il campo Nome utente rimane visibile.

   >[!NOTE]
   Se l’organizzazione è stata imbarcata nell’Admin Console e aggiungi un utente tramite Workfront, non puoi scegliere di inviare un invito e-mail.
   All’Admin Console vengono aggiunti nuovi utenti di Adobe e l’Admin Console invia un messaggio e-mail per invitarli a completare il processo di registrazione. Tutti gli utenti devono completare il processo di registrazione per accedere a qualsiasi sistema di Adobe.
   Per gli utenti esistenti di Adobe, l’utente potrebbe ricevere o meno un’e-mail sulla disponibilità di Workfront. Si tratta di una preferenza controllata dall’amministratore di Adobe per il prodotto.

1. Fai clic su **Aggiungi utente**.

   Oppure

   Fai clic su **Aggiungi utente e avvia un altro** per salvare il nuovo utente e aggiungerne un altro.

## Copiare un utente per crearne uno nuovo

Puoi creare un utente copiando un utente esistente.

>[!NOTE]
Quando crei un utente in questo modo, tutte le informazioni vengono copiate dall&#39;utente originale all&#39;utente appena creato, fatta eccezione per quanto segue:
* Informazioni nella sezione Informazioni personali.
* Quando accedo, mostra: In questa casella viene selezionata la scheda di destinazione predefinita per il livello di accesso.
* I Report Diretti
>


Per creare un nuovo utente copiandone uno esistente:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).
1. Seleziona l’utente da copiare, quindi fai clic sull’icona Copia ![](assets/copy-icon.png).
1. In **Nuovo utente** in cui vengono visualizzati, modificare i campi disponibili per il nuovo utente.

   Per informazioni su tutti i campi associati a un utente, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Fai clic su **Aggiungi utente**.

   Oppure

   Fai clic su **Aggiungi utente e avvia un altro** per salvare il nuovo utente e aggiungerne un altro.

Questo crea un nuovo account in Workfront per l’utente.

Se hai selezionato l’opzione per inviare un invito all’utente, questi riceverà un’e-mail in cui potrà seguire un collegamento per creare la propria password Workfront.

>[!NOTE]
Se l’organizzazione è stata imbarcata nell’Admin Console e aggiungi un utente tramite Workfront, non puoi scegliere di inviare un invito e-mail.
All’Admin Console vengono aggiunti nuovi utenti di Adobe e l’Admin Console invia un messaggio e-mail per invitarli a completare il processo di registrazione. Tutti gli utenti devono completare il processo di registrazione per accedere a qualsiasi sistema di Adobe.
Per gli utenti esistenti di Adobe, l’utente potrebbe ricevere o meno un’e-mail sulla disponibilità di Workfront. Si tratta di una preferenza controllata dall’amministratore di Adobe per il prodotto.
