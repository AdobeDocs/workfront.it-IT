---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Assegnare tag agli altri utenti in caso di aggiornamenti
description: Quando si forniscono commenti di aggiornamento su un oggetto Adobe Workfront, tutte le informazioni inviate vengono visualizzate da tutti gli utenti del progetto. Tuttavia, in alcuni casi gli utenti che non fanno parte del progetto potrebbero trarre vantaggio dalla visualizzazione di queste informazioni. Invece di includere tali utenti nel progetto, puoi assegnare loro tag nell’aggiornamento per condividerlo con loro. Gli utenti con tag ricevono una notifica dell’evento.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: ba1d8d5a23da7e252e8c182a6bdb1cdd1e304eab
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Assegnare tag agli altri utenti in caso di aggiornamenti

<!--take "Beta" references out when we remove the beta-->

<!-- Drafted for commenting experience: 

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>For more information about the new updating experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 
>
>You can access the new design for the following objects:
> * <span class="preview">Issues, when enabling the commenting Beta. </span>
> * Goals
>   The new commenting experience is the default for goals. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 

-->
È possibile assegnare tag agli utenti durante l’aggiornamento a un oggetto se si desidera attirare l’attenzione su un oggetto che altrimenti non potrebbero seguire.
Anziché includere gli utenti nell’oggetto assegnandoli ad esso o facendoli sottoscrivere, puoi assegnare loro tag sull’aggiornamento per condividerlo con loro. Gli utenti con tag ricevono una notifica relativa all’aggiornamento inserito.

>[!NOTE]
>
>È necessario abilitare una notifica evento affinché un utente riceva la notifica e-mail. Gli amministratori possono abilitare le notifiche per l’intero sistema o per un gruppo di livello superiore. Un utente può inoltre abilitare e disabilitare le notifiche di singoli eventi nel proprio profilo utente. Per ulteriori informazioni, consulta quanto segue:
>
>* [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
>* [Visualizzare e configurare le notifiche evento per un gruppo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)
>* [Attivare o disattivare le notifiche degli eventi personali](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>


Per informazioni sull’aggiunta di aggiornamenti agli oggetti Workfront, consulta [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Quando un problema viene convertito in un progetto o in un&#39;attività, gli aggiornamenti vengono copiati nel nuovo progetto o attività, ma gli utenti con tag non lo sono. Per continuare la conversazione, devi assegnare nuovamente i tag ai partecipanti.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>piano Adobe Workfront*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Richiesta o superiore di problemi e documenti; Revisione o superiore per tutti gli altri oggetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Richiedente o superiore per le emissioni e i documenti; Revisore o superiore per tutti gli altri oggetti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Visualizza l’accesso all’oggetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Assegnare tag agli altri utenti in caso di aggiornamenti

<!--
Tagging others in an update differs depending on which experience and which object you select.

### Tag others on updates in the current Updates section
-->

1. Inizia l&#39;aggiornamento di un elemento di lavoro, come descritto in [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In **Notifica** inizia a digitare il nome dell&#39;utente o del team che desideri includere, quindi fai clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   Oppure

   Digita il simbolo @ nel **Avvia un nuovo aggiornamento** area, inizia a digitare il nome dell&#39;utente o del team che desideri includere nell&#39;aggiornamento, quindi fai clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   >[!TIP]
   >
   >Per identificare l&#39;utente corretto quando ci sono utenti con nomi simili o identici, notate l&#39;avatar, il ruolo principale dell&#39;utente o il loro indirizzo e-mail. Gli utenti devono essere associati ad almeno un ruolo di lavoro per visualizzarlo durante l&#39;assegnazione dei tag in un aggiornamento.

   ![](assets/tag-users-in-update.png)

1. (Facoltativo) Per rendere privato l&#39;aggiornamento, abilita **Privato per la mia azienda** nell&#39;angolo in basso a destra della casella di aggiornamento. Questo rende l’aggiornamento visibile solo agli utenti della tua azienda.

   >[!NOTE]
   >
   >Gli utenti con tag esterni all’azienda potrebbero comunque ricevere una notifica o un’e-mail in-app, anche se non visualizzeranno i commenti privati nella scheda Aggiornamenti . Consigliamo di non assegnare tag agli utenti esterni in un aggiornamento se non desideri condividere le informazioni con loro.

1. (Facoltativo) Per aggiungere più utenti e team, ripeti il passaggio 2.

   >[!NOTE]
   >
   >Tutti gli utenti e i membri del team elencati nel campo Notifica ricevono una notifica in-app per l’aggiornamento e potrebbero ricevere un’e-mail, a seconda della configurazione delle impostazioni di notifica e-mail. Gli utenti che si taggano in un commento o in una risposta ricevono una notifica per quel commento o risposta e possono visualizzare il loro nome nel campo Notifica per il resto del thread, ma non ricevono un&#39;altra notifica a meno che non si taggino di nuovo. Per ulteriori informazioni, consulta [Attivare o disattivare le notifiche degli eventi personali](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) e [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Fai clic su **Aggiorna**.\
   Gli utenti inclusi nell’aggiornamento ricevono automaticamente l’autorizzazione Visualizza per l’oggetto e possono visualizzare e rispondere agli aggiornamenti apportati all’oggetto.

   Puoi vedere chi è stato taggato in ogni risposta nella parte superiore del thread di aggiornamento. Questi utenti, insieme a tutti gli utenti abbonati all’oggetto, ricevono una notifica ogni volta che viene effettuato un aggiornamento o una risposta sull’oggetto.

   ![](assets/tagging-transparency-350x192.png)

   Per informazioni sulle funzionalità aggiuntive disponibili durante l&#39;aggiornamento di un elemento di lavoro, vedere [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

<!--
<div class="preview">

### Tag others on updates in the commenting Beta experience

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Tag people or teams** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   <!- ********************* this doesn't seem to work in Beta - keep drafted for now: 
   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list. ************close draft

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. Users must be associated with at least one job role to view it as you tag them in an update.

   ![](assets/tag-others-unified-commenting.png)

      <!-******************* this might not be there for issues yet - keep drafted if not: 
      1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company.

         >[!NOTE]
         >
         >* This option displays only when the user is associated with a Company.
         >* Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them. - ************close draft 
      
1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the "Tag people or teams" field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in listed as a member of the thread for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Activate or deactivate your own event notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Submit**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply under the text of the update, in the Members area. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.
1. (Optional) Cick the number of members included in the update to display a list of entities that the update you entered is shared with. 

   ![](assets/members-icons-expanded-unshimmed.png)

   For information about the additional functionality that is available when updating a work item, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

-->