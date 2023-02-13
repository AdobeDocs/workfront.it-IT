---
user-type: administrator
product-area: system-administration;user-management
keywords: visualizzazione, gruppo, evento, notifiche, configurare, abilitare, disabilitare
navigation-topic: create-and-manage-groups
title: Visualizzare e configurare le notifiche evento per un gruppo
description: In qualità di amministratore del gruppo, puoi visualizzare le notifiche dell’evento attivate per un gruppo gestito. Inoltre, se un amministratore di Adobe Workfront sblocca una notifica di evento, puoi configurarla per un gruppo di livello principale gestito. La configurazione di una notifica di evento consiste nell’attivarla o disattivarla.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: 306d6493ff0413d5814f4aed8ab44fb897f3568d
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# Visualizzare e configurare le notifiche evento per un gruppo

In qualità di amministratore del gruppo, puoi visualizzare le notifiche dell’evento attivate per un gruppo gestito.

Inoltre, se un amministratore di Adobe Workfront sblocca una notifica di evento, puoi configurarla per un gruppo di livello principale gestito. La configurazione di una notifica di evento consiste nell’attivarla o disattivarla.

Un amministratore Workfront può eseguire questa operazione anche per qualsiasi gruppo.

La configurazione di una notifica di evento per un gruppo riguarda gli utenti per i quali tale gruppo, o uno dei suoi sottogruppi, è il gruppo principale. Nei loro profili utente, questi utenti visualizzano le notifiche degli eventi che vengono attivate per il loro gruppo principale invece delle notifiche degli eventi che vengono attivate a livello di sistema.

Per informazioni su come un amministratore di Workfront sblocca una notifica di evento, vedi [Sblocca o blocca la configurazione delle notifiche degli eventi per tutti i gruppi](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Per informazioni sull&#39;impostazione di notifica predefinita per un evento, vedi [Notifiche di eventi disponibili in Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">piano Workfront</a>*</td> 
   <td> <p>Pro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Licenza Adobe Workfront</a>*</td> 
   <td> <p>Piano </p> <p>È necessario essere un amministratore del gruppo o un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Visualizzare e configurare le notifiche degli eventi di un gruppo

1. (Condizionale e facoltativo) Se sei un amministratore di Workfront e sei già nella pagina Notifiche e-mail (Configurazione > E-mail > Notifiche), puoi effettuare le seguenti operazioni e quindi passare al passaggio 6: Elimina **Notifiche degli eventi di sistema** nella casella sopra l&#39;elenco, inizia a digitare il nome del gruppo nella casella, quindi fai clic su di esso quando viene visualizzato.
1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Fai clic sul nome del gruppo di livello principale.
1. Nel menu a sinistra, fai clic su **Notifiche degli eventi**.

   Nell’elenco visualizzato, il **Attivo** la colonna a sinistra mostra quali notifiche sono attive (blu) e inattive (grigie) per il gruppo.

1. Per attivare o disattivare una notifica di evento sbloccato: Fai clic sul pulsante in <strong>Attivo</strong> colonna da attivare <img src="assets/email-notification-enabled-unlocked.png"> o disattivare <img src="assets/email-notification-disabled-unlocked.png"> .

   >[!INFO]
   >
   >**Esempio:** Puoi configurare le prime due notifiche evento del gruppo Marketing mostrate di seguito che sono state sbloccate per i gruppi.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* Se un pulsante nel <strong>Attivo</strong> la colonna è grigia e scura <img src="assets/email-notification-disabled-locked.png">, la notifica dell’evento è disattivata per tutti gli utenti e gli amministratori di gruppo non possono attivarla o modificarne l’oggetto dell’e-mail
   >* Se un pulsante nel <strong>Attivo</strong> la colonna è grigia e non è oscurata <img src="assets/email-notification-disabled-unlocked.png">, la notifica dell’evento è <strong>disattivato per tutti gli utenti e</strong> gli amministratori del gruppo possono attivarlo per i loro gruppi.
   >* Se un pulsante nel <strong>Attivo</strong> la colonna è blu e scura <img src="assets/email-notification-enabled-locked.png">, la notifica dell’evento viene attivata per tutti gli utenti e gli amministratori di gruppo non possono disattivarla o modificare l’oggetto dell’e-mail per i loro gruppi.
   >* Se un pulsante nel <strong>Attivo</strong> la colonna è blu e non è oscurata <img src="assets/email-notification-enabled-unlocked.png">, la notifica dell’evento è <strong>attivato per tutti gli utenti e</strong> gli amministratori del gruppo possono disattivarlo per i propri gruppi.


<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

