---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Assegnare tag agli altri utenti in caso di aggiornamenti
description: Quando si forniscono commenti di aggiornamento su un oggetto Adobe Workfront, tutte le informazioni inviate vengono visualizzate da tutti gli utenti del progetto. Tuttavia, in alcuni casi gli utenti che non fanno parte del progetto potrebbero trarre vantaggio dalla visualizzazione di queste informazioni. Invece di includere tali utenti nel progetto, puoi assegnare loro tag nell’aggiornamento per condividerlo con loro. Gli utenti con tag ricevono una notifica dell’evento.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 1eba586f4d3ce6db667839b0620dfeb65f6e28be
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# Assegnare tag agli altri utenti in caso di aggiornamenti

Quando si forniscono commenti di aggiornamento su un oggetto Adobe Workfront, tutte le informazioni inviate vengono visualizzate da tutti gli utenti del progetto. Tuttavia, in alcuni casi gli utenti che non fanno parte del progetto potrebbero trarre vantaggio dalla visualizzazione di queste informazioni. Invece di includere tali utenti nel progetto, puoi assegnare loro tag nell’aggiornamento per condividerlo con loro. Gli utenti con tag ricevono una notifica dell’evento.

>[!NOTE]
>
>È necessario abilitare una notifica di evento affinché un utente possa riceverla. Gli amministratori possono abilitare le notifiche per l’intero sistema o per un gruppo di livello superiore. Un utente può inoltre abilitare e disabilitare le notifiche di singoli eventi nel proprio profilo utente. Per ulteriori informazioni, consulta quanto segue:
>
>* [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
>* [Visualizzare e configurare le notifiche evento per un gruppo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)
>* [Attivare o disattivare le notifiche degli eventi personali](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>


>[!NOTE]
>
>Quando un problema viene convertito in un progetto o in un&#39;attività, gli aggiornamenti vengono copiati nel nuovo progetto o attività, ma gli utenti con tag non lo sono. Per continuare la conversazione, devi assegnare nuovamente i tag ai partecipanti.

Per informazioni sull’aggiunta di aggiornamenti agli oggetti Workfront, consulta [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

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
   >Gli utenti con tag esterni all’azienda potrebbero comunque ricevere una notifica o un’e-mail in-app, anche se non visualizzeranno i commenti privati nella scheda Aggiornamenti . È consigliabile non assegnare tag agli utenti esterni in un aggiornamento se non si desidera condividere le informazioni con loro.

1. (Facoltativo) Per aggiungere più utenti e team, ripeti il passaggio 2.

   >[!NOTE]
   >
   >Tutti gli utenti e i membri del team elencati nel campo Notifica ricevono una notifica in-app per l’aggiornamento e potrebbero ricevere un’e-mail, a seconda della configurazione delle impostazioni di notifica e-mail. Gli utenti che si taggano in un commento o in una risposta ricevono una notifica per quel commento o risposta e possono visualizzare il loro nome nel campo Notifica per il resto del thread, ma non ricevono un&#39;altra notifica a meno che non si taggino di nuovo. Per ulteriori informazioni, consulta [Attivare o disattivare le notifiche degli eventi personali](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) e [Configurare le notifiche degli eventi per tutti gli utenti del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Fai clic su **Aggiorna**.\
   Gli utenti inclusi nell’aggiornamento ricevono automaticamente l’autorizzazione Visualizza per l’oggetto e possono visualizzare e rispondere agli aggiornamenti apportati all’oggetto.

   Puoi vedere chi è stato taggato in ogni risposta nella parte superiore del thread di aggiornamento. Questi utenti, insieme a tutti gli utenti abbonati all’oggetto, ricevono una notifica ogni volta che viene effettuato un aggiornamento o una risposta sull’oggetto.

   ![](assets/tagging-transparency-350x192.png)

   Per informazioni sulle funzionalità aggiuntive disponibili durante l&#39;aggiornamento di un elemento di lavoro, vedere [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
