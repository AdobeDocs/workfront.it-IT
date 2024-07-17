---
user-type: administrator
product-area: system-administration;user-management
keywords: visualizza,gruppo,evento,notifiche,configura,abilita,disabilita
navigation-topic: create-and-manage-groups
title: Visualizzare e configurare le notifiche degli eventi per un gruppo
description: In qualità di amministratore di gruppo, puoi visualizzare le notifiche degli eventi attivate per un gruppo che gestisci. Inoltre, se un amministratore di Adobe Workfront sblocca una notifica di evento, puoi configurarla per un gruppo di livello principale da gestire. La configurazione di una notifica di evento consiste nell’attivarla o disattivarla.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Visualizzare e configurare le notifiche degli eventi per un gruppo

In qualità di amministratore di gruppo, puoi visualizzare le notifiche degli eventi attivate per un gruppo che gestisci.

Inoltre, se un amministratore di Adobe Workfront sblocca una notifica di evento, puoi configurarla per un gruppo di livello principale da gestire. La configurazione di una notifica di evento consiste nell’attivarla o disattivarla.

Un amministratore di Workfront può eseguire questa operazione per qualsiasi gruppo.

La configurazione di una notifica di evento per un gruppo influisce sugli utenti per i quali tale gruppo, o uno dei suoi sottogruppi, è il proprio Gruppo predefinito. Nei profili utente, questi utenti visualizzano le notifiche degli eventi attivate per il proprio Gruppo predefinito anziché le notifiche degli eventi attivate a livello di sistema.

Per informazioni su come un amministratore di Workfront sblocca una notifica di evento, vedere [Sbloccare o bloccare la configurazione delle notifiche di evento per tutti i gruppi](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Per informazioni sull&#39;impostazione di notifica predefinita per un evento, vedere [Tipi di notifica evento](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>Devi essere un amministratore di gruppo del gruppo o un amministratore di Workfront. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppi</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza di cui si dispone, contattare l&#39;amministratore di Workfront.

## Visualizzare e configurare le notifiche degli eventi di un gruppo

1. (Condizionale e facoltativo) Se si è un amministratore di Workfront e si è già nella pagina Notifiche e-mail (Configurazione > E-mail > Notifiche), è possibile eseguire le operazioni seguenti e passare al passaggio 6: Elimina **Notifiche eventi di sistema** nella casella sopra l&#39;elenco, iniziare a digitare il nome del gruppo nella casella, quindi fare clic su di esso quando viene visualizzato.
1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Fare clic sul nome del gruppo di primo livello.
1. Nel menu a sinistra, fai clic su **Notifiche evento**.

   Nell&#39;elenco visualizzato, la colonna **Attivo** a sinistra mostra quali notifiche sono attive (blu) e inattive (grigio) per il gruppo.

1. Per attivare o disattivare una notifica di evento sbloccata: fare clic sul pulsante nella colonna <strong>Attivo</strong> per attivare <img src="assets/email-notification-enabled-unlocked.png"> o disattiva <img src="assets/email-notification-disabled-unlocked.png">.

   >[!INFO]
   >
   >**Esempio:** Puoi configurare le prime due notifiche di eventi del gruppo di marketing mostrate di seguito che sono state sbloccate per i gruppi.</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* Se un pulsante nella colonna <strong>Attivo</strong> è grigio e inattivo <img src="assets/email-notification-disabled-locked.png">, la notifica dell&#39;evento è disattivata per tutti gli utenti e gli amministratori dei gruppi non possono attivarla o modificarne l&#39;oggetto e-mail
   >* Se un pulsante nella colonna <strong>Attivo</strong> è grigio e non oscurato <img src="assets/email-notification-disabled-unlocked.png">, la notifica dell&#39;evento è <strong>disattivata per tutti gli utenti e</strong> gli amministratori dei gruppi possono attivarla per i loro gruppi.
   >* Se un pulsante nella colonna <strong>Attivo</strong> è blu e inattivo <img src="assets/email-notification-enabled-locked.png">, la notifica dell&#39;evento è attivata per tutti gli utenti e gli amministratori dei gruppi non possono disattivarla o modificare l&#39;oggetto dell&#39;e-mail per i loro gruppi.
   >* Se un pulsante nella colonna <strong>Attivo</strong> è blu e non oscurato <img src="assets/email-notification-enabled-unlocked.png">, la notifica dell&#39;evento è <strong>attivata per tutti gli utenti e</strong> gli amministratori dei gruppi possono disattivarla per i loro gruppi.

<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

