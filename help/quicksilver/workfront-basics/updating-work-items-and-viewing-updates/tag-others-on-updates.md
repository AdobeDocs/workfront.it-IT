---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Assegna tag ad altri utenti in caso di aggiornamenti
description: Quando si forniscono commenti di aggiornamento su un oggetto Adobe Workfront, tutti gli utenti del progetto possono visualizzare le informazioni inviate. Tuttavia, in alcuni casi gli utenti che non fanno parte del progetto potrebbero trarre vantaggio dalla visualizzazione di tali informazioni. Invece di includere tali utenti nel progetto, puoi assegnare loro tag nell’aggiornamento per condividerlo con loro. Gli utenti taggati ricevono una notifica dell’evento.
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: a9cfeaadad136f503797794050e8bc23f1392f22
workflow-type: tm+mt
source-wordcount: '997'
ht-degree: 0%

---

# Assegna tag ad altri utenti in caso di aggiornamenti

<!--Audited: April, 2024-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span> 
-->

È possibile assegnare tag agli utenti quando si esegue un aggiornamento a un oggetto se si desidera attirare la loro attenzione su un oggetto che altrimenti potrebbero non seguire.

Invece di includere tali utenti nell’oggetto assegnandoli a esso o imponendo loro di abbonarsi ad esso, puoi assegnare loro tag nell’aggiornamento per condividerlo con loro. Gli utenti taggati ricevono una notifica Workfront relativa all’aggiornamento immesso. A seconda delle impostazioni di notifica, viene inoltre inviata un&#39;e-mail relativa all&#39;aggiornamento immesso.

## Considerazioni sull’assegnazione tag agli utenti negli aggiornamenti

* Gli utenti taggati negli aggiornamenti devono abilitare una notifica personale nel loro profilo per poter ricevere la notifica e-mail. Per ulteriori informazioni, vedere [Modificare le proprie notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  Per informazioni sull&#39;aggiunta di aggiornamenti agli oggetti di Workfront, vedere [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* Quando un problema viene convertito in un progetto o in un’attività, gli aggiornamenti vengono copiati nel nuovo progetto o attività, ma non negli utenti taggati. Per continuare la conversazione, è necessario assegnare nuovamente i tag ai partecipanti.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>piano Adobe Workfront</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Nuovo: Collaboratore o versione successiva per problemi e documenti; Light o versione successiva per tutti gli altri oggetti</p>
   <p>Corrente: richiesta o successiva per problemi e documenti; revisione o successiva per tutti gli altri oggetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazione del livello di accesso</strong></td> 
   <td> <p>Accesso di visualizzazione o superiore agli oggetti in cui si desidera pubblicare la risposta</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazione oggetto</strong></td> 
   <td> <p>Visualizza o autorizzazioni superiori per gli oggetti in cui desideri pubblicare la risposta</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront. Per ulteriori informazioni, consulta [Requisiti di accesso per la documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Assegna tag ad altri utenti in caso di aggiornamenti

Puoi assegnare tag ad altri utenti in caso di aggiornamenti nei modi seguenti:

* **Automaticamente**: quando un utente avvia un thread, aggiunge un commento o aggiunge una risposta, vengono automaticamente taggati e aggiunti all&#39;area Tag persone o team della casella di commento.
* **Manualmente**: quando si aggiunge manualmente un utente all&#39;area Tag persone della casella di commento.

È inoltre possibile rimuovere gli utenti a cui vengono assegnati tag per errore quando si modifica o si risponde a un commento.

1. Inizia ad aggiornare un elemento di lavoro, come descritto in [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). In qualità di proprietario del commento, riceverai automaticamente i tag e verrai aggiunto all’area Tag persone o team della casella di commento.

   >[!TIP]
   >
   >Il proprietario del commento non può visualizzare il proprio nome nell’area Tag persone o team della casella di commento.

1. Nel campo **Assegna tag a persone o team**, inizia a digitare il nome dell&#39;utente o del team che desideri includere, quindi fai clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   Oppure

   Digitare il simbolo @ nell&#39;area **Scrivi un commento**, iniziare a digitare il nome dell&#39;utente o del team che si desidera includere nell&#39;aggiornamento, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   >[!TIP]
   > 
   >Per identificare l’utente corretto quando ci sono utenti con nomi simili o identici, nota l’avatar, il Ruolo principale dell’utente o il suo indirizzo e-mail.
   > 
   >Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono tag in un aggiornamento.
   > 
   >Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, vedere [Concedere l&#39;accesso agli utenti](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![Assegna tag a un utente](assets/tag-others-unified-commenting-with-all-tab.png)

1. (Facoltativo) Per rendere l&#39;aggiornamento privato, abilita **Privato per la mia società** nell&#39;angolo inferiore destro della casella di aggiornamento. In questo modo l’aggiornamento è visibile solo agli utenti della tua azienda. L&#39;opzione **Privato per la mia società** è disponibile solo quando nel profilo Workfront è specificata una società.

   >[!NOTE]
   >
   >* Questa opzione viene visualizzata solo quando l’utente è associato a una società.
   >* Gli utenti taggati esterni all’azienda potrebbero comunque ricevere una notifica o un’e-mail in-app, anche se non vedranno i commenti privati nella scheda Aggiornamenti. È consigliabile non assegnare tag agli utenti esterni in un aggiornamento se non si desidera condividere le informazioni con loro.

1. (Facoltativo) Per aggiungere più utenti e team, ripetere il passaggio 2. <!--insure this stays accurate-->

   >[!NOTE]
   >
   >Tutti gli utenti e i membri del gruppo elencati nel campo &quot;Assegna tag a persone o team&quot; ricevono una notifica in-app per l’aggiornamento e potrebbero ricevere un’e-mail, a seconda della configurazione delle impostazioni di notifica e-mail. Gli utenti che si applicano il tag in un commento o in una risposta ricevono una notifica per tale commento o risposta e possono vedere il proprio nome in elencato come membro del thread per il resto del thread, ma non ricevono un’altra notifica a meno che non si assegnino nuovamente il tag. Per ulteriori informazioni, vedere [Modificare le proprie notifiche e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) e [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Fai clic su **Invia**.\
   Agli utenti inclusi nell&#39;aggiornamento viene automaticamente concessa l&#39;autorizzazione Visualizzazione per l&#39;oggetto e possono visualizzare e rispondere agli aggiornamenti apportati all&#39;oggetto.

   I nomi delle entità con tag vengono visualizzati accanto ai relativi avatar, fino a due entità. Se vengono assegnate tag a più di due entità, viene visualizzato il nome della prima entità, oltre a un numero di quelle aggiuntive.

   ![](assets/members-icons-expanded-unshimmed.png)

   Quando si viene taggati nel testo del commento, il proprio nome viene evidenziato in tali commenti.

   Per informazioni sulle funzionalità aggiuntive disponibili durante l&#39;aggiornamento di un elemento di lavoro, vedere [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Facoltativo) Fai clic sul menu **Altro** ![](assets/more-menu.png) nell&#39;angolo superiore destro del commento, quindi fai clic su **Modifica**. Rimuovi gli utenti taggati, quindi fai clic su **Invia**.

   >[!IMPORTANT]
   >
   >È possibile modificare un commento solo entro 15 minuti dall&#39;immissione. Puoi modificare solo i commenti aggiunti.


<!--
   >[!TIP]
   >
   >When using the legacy commenting experience to add comments and replies, comment owners that were not specifically tagged cannot be manually removed by people who use the new commenting experience.
-->

<!--
### Tag others on updates in the legacy Updates section

You can manually tag users in the legacy Updates section. 

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Notify** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list.

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. 
   >
   >Users must be associated with at least one job role to view it as you tag them in an update. 
   >
   >You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-users-in-update.png)

1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company. The **Private to my company** option is available only when a Company is specified in your Workfront profile. 

   >[!NOTE]
   >
   >Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them.  

1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the Notify field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in the Notify field for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Update**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply at the top of the update thread. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.

   ![](assets/tagging-transparency-350x192.png)
-->

Per informazioni sulle funzionalità aggiuntive disponibili durante l&#39;aggiornamento di un elemento di lavoro, vedere [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).



