---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Gestione del team di progetto
description: Il team del progetto è costituito da utenti associati al progetto. I membri del team di progetto vengono visualizzati nella sezione Persone del progetto o nella sezione Persone del modello che può essere utilizzato per creare un progetto.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: fe51ded26c57e3b7137e42ad2218d79adf032b85
workflow-type: tm+mt
source-wordcount: '1280'
ht-degree: 1%

---

# Gestione del team di progetto

<!--take preview and production references out at production - August 7-->

<div class="preview">

Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Le stesse funzioni saranno disponibili anche nell’ambiente di produzione per tutti i clienti dopo una settimana dalla versione di anteprima.

Per ulteriori informazioni, vedere [Modernizzazione interfaccia](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

Il team del progetto è costituito da utenti associati al progetto. Per ulteriori informazioni, vedere [Panoramica team di progetto](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md).

I membri del team di progetto vengono visualizzati nella sezione Persone del progetto.

Gli utenti visualizzati nella sezione Persone di un modello di progetto diventeranno il team di progetto dopo che il progetto è stato creato dal modello.

I seguenti utenti vengono aggiunti automaticamente al team di progetto, sia per i progetti che per i modelli:

* Proprietario
* Sponsor
* Utenti assegnati alle attività
* Utenti assegnati ai problemi (solo per un progetto)

Gli utenti del team di progetto ricevono notifiche sul progetto. Per ulteriori informazioni, vedere [Tipi di notifica eventi](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Puoi gestire gli utenti del progetto e i team del modello aggiungendoli (solo per il progetto), rimuovendoli o inviando loro un aggiornamento.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuovo: Standard </p>
    <p>Corrente: Piano </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso</td> 
   <td> <p>Modificare l’accesso a progetti e modelli</p> <p>Accesso di visualizzazione o superiore agli utenti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare o autorizzazioni superiori per un progetto o un modello</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old access: 

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>View or higher access to Users</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator.

## Add users to a Project Team

When you add users to the project team, they gain View permissions on the project and the tasks, issues, and documents of the project. For more information, see the article [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Users on the Project Team are not automatically added to the resource management tools for the project.

You can add users to the project team in the following ways:

* [Automatically add users to a Project Team](#automatically-add-users-to-a-project-team) 
* [Manually add users to a Project Team](#manually-add-users-to-a-project-team)

### Automatically add users to a Project Team {#automatically-add-users-to-a-project-team}

The users that fulfill the following roles on the project are automatically added to the project team and appear  in the People section when the project is created:

* The creator of the project
* The project owner
* The project sponsor

Users are also automatically added to the project team when they are assigned to the following:

* Tasks
* Issues

### Manually add users to a Project Team {#manually-add-users-to-a-project-team}

If users that don't fulfill any role on the project want to be notified about certain updates or changes during the life of the project, you can manually add them to the project team. 

 For more information about what notifications can be enabled for users on the project team, see [Event notification types](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md). 

 <!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

## Gestire le persone in un progetto

1. Passare al progetto per il quale si desidera gestire il team di progetto.

   >[!TIP]
   >
   >Affinché gli utenti possano essere visualizzati nella sezione Persone, è necessario che siano assegnati ad attività, problemi o come soggetti interessati al progetto.

1. Fai clic su **Persone** nel pannello a sinistra.

1. Fare clic su **Aggiungi utenti**.

   Viene visualizzata la casella **Aggiungi utenti al team di progetto**.

   ![aggiungi_utenti_dialogo.png](assets/add-users-dialog-350x217.png)

1. Nella casella **Aggiungi utenti** digitare il nome di un utente Workfront attivo che si desidera aggiungere al team del progetto, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco.

   Ripeti questo passaggio per aggiungere più utenti al team di progetto. Gli utenti devono appartenere al gruppo associato al progetto.

   >[!TIP]
   >
   >* Non puoi aggiungere utenti aggiungendo i loro team, gruppi, aziende o mansioni.
   >* Quando aggiungi gli utenti, osserva l’avatar, il Ruolo principale dell’utente e il suo indirizzo e-mail per distinguere gli utenti con nomi identici. Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono aggiunti.
   >
   >  Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, vedere [Concedere l&#39;accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. Fare clic su **Aggiungi**.

   Gli utenti ottengono le autorizzazioni di visualizzazione per il progetto e ricevono notifiche sul progetto come parte del team del progetto.

1. (Facoltativo) Se desideri che un utente riceva una notifica quando la sua mansione viene aggiunta a un&#39;attività, a un problema o all&#39;approvazione di un progetto, fai clic nella colonna **Mansione** per l&#39;utente e seleziona una mansione che sarà associata all&#39;approvazione.

   Gli utenti riceveranno notifiche relative alle approvazioni assegnate alla mansione selezionata.

   Per ulteriori informazioni, vedere la sezione &quot;Role-based approvals&quot; nell&#39;articolo [Project Team overview](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md).

1. Seleziona uno o più utenti nell&#39;elenco, quindi fai clic sull&#39;icona **Rimuovi** ![Rimuovi icona](assets/remove-icon.png) per rimuoverli dal team.

1. Fare clic su **Sì, Rimuovi utenti selezionati** per confermare e rimuovere gli utenti.

   Gli utenti vengono rimossi e non assegnati a elementi di lavoro incompleti.

   Per ulteriori informazioni, vedere la sezione [Considerazioni per la rimozione di utenti da un team di progetto](#considerations-for-removing-users-from-a-project-team) in questo articolo.
1. (Facoltativo) Per inviare un aggiornamento per questo progetto agli utenti, fai clic su Aggiorna tutto per inviare l’aggiornamento a tutti gli utenti del team

   Oppure

   Selezionare uno o più utenti nell&#39;elenco, quindi fare clic su **Invia aggiornamento all&#39;utente**.

   ![Invia aggiornamento all&#39;utente in un progetto](assets/send-update-to-user-on-project-box.png)

   Viene visualizzata la casella **Invia aggiornamento all&#39;utente**.

1. Esegui una delle operazioni seguenti:

   * Aggiungi un aggiornamento per gli utenti selezionati.
   * Fai clic sull’icona del lucchetto per rendere l’aggiornamento privato per gli utenti della tua azienda.
   * Assegna tag ad altri utenti per ricevere lo stesso aggiornamento.
   * Fai clic su **Invia**.

   L&#39;aggiornamento viene aggiunto alla sezione **Aggiornamenti** del progetto e tutti gli utenti selezionati vengono visualizzati come utenti taggati.

   Gli utenti possono ricevere una notifica e-mail, se sono abilitati per loro, e una notifica in-app sul nuovo aggiornamento.

1. (Facoltativo) Fai clic sull&#39;icona **Esporta** ![Icona Esporta](assets/export-icon.png) per esportare l&#39;elenco degli utenti in un file

   Oppure

   Seleziona gli utenti, quindi fai clic sull&#39;icona **Esporta** per esportare solo utenti specifici.

## Gestire le persone su un modello

1. Vai al modello per il quale desideri gestire il team di progetto.

   >[!TIP]
   >
   >Affinché gli utenti siano visualizzati nella sezione Persone, è necessario che siano assegnati alle attività o come stakeholder del modello.

1. Fai clic su **Persone** nel pannello a sinistra.

1. Seleziona uno o più utenti nell&#39;elenco, quindi fai clic su **Rimuovi** per rimuoverli dal team.

1. Fare clic su **Sì, Rimuovi utenti selezionati** per confermare e rimuovere gli utenti.

   Gli utenti vengono rimossi e non assegnati alle attività modello.

   Per ulteriori informazioni, vedere la sezione [Considerazioni per la rimozione di utenti da un team di progetto](#considerations-for-removing-users-from-a-project-team) in questo articolo.

1. (Facoltativo) Per inviare un aggiornamento agli utenti, fare clic su Aggiorna tutto per inviare l&#39;aggiornamento a tutti gli utenti nell&#39;elenco

   Oppure

   Selezionare uno o più utenti nell&#39;elenco, quindi fare clic su **Aggiorna**.

   <!--update screen shot for unshim production, notice the text above the box - it needs to say "Post an update to each person's profile"-->

   ![Invia aggiornamento alla casella utente nel modello](assets/send-update-to-user-on-template-box.png)

   Viene visualizzata la casella **Invia aggiornamento all&#39;utente**.

1. Effettua le seguenti operazioni:

   * Nell’ambiente di produzione:

      * Aggiungi un aggiornamento per gli utenti selezionati.
      * Fai clic sull’icona persone per assegnare un tag ad altri utenti per ricevere lo stesso aggiornamento.
      * Fai clic sull’icona del lucchetto per rendere l’aggiornamento privato per gli utenti della tua azienda.
      * Fai clic su **Invia**.

   * <span class="preview">Nell&#39;ambiente di anteprima: </span>

   <div class="preview">

   * Aggiungi un aggiornamento per gli utenti selezionati.
   * Fai clic su **Assegna tag a persone** per assegnare tag ad altri utenti per ricevere lo stesso aggiornamento.
   * Seleziona l&#39;opzione **Privato per la mia azienda** per rendere l&#39;aggiornamento privato per gli utenti della tua azienda.
   * Fai clic su **Invia**.

   </div>

   L&#39;aggiornamento viene aggiunto alla sezione **Aggiornamenti** del profilo di ciascun utente taggato.

   Gli utenti possono ricevere una notifica e-mail, se sono abilitati per loro, e una notifica in-app sul nuovo aggiornamento.

1. (Facoltativo) Fai clic su **Esporta** per esportare l&#39;elenco degli utenti in un file

   Oppure

   Seleziona gli utenti, quindi fai clic su **Esporta** per esportare solo utenti specifici.

## Considerazioni per la rimozione di utenti da un team di progetto

Quando rimuovi gli utenti dai loro ruoli sul progetto, questi rimangono parte del team del progetto.

È necessario rimuoverli dal team del progetto, dalla sezione Persone del progetto, affinché non ricevano più le notifiche inviate al team del progetto.

Se si rimuove un utente dal team del progetto e l&#39;utente viene assegnato ad attività o problemi del progetto, l&#39;utente non viene assegnato alle attività e ai problemi non completati. In questo caso, le attività e i problemi tornano nell’area Lavoro non assegnato nel Bilanciatore dei carichi di lavoro.

Gli utenti assegnati ad attività e problemi completati rimangono assegnati ad attività e problemi, anche dopo che sono stati rimossi dal team di progetto.

I seguenti utenti vengono rimossi dai loro ruoli nel progetto quando li rimuovi dalla sezione Persone di un progetto o di un modello:

* Utenti assegnati ad attività incomplete
* Utenti assegnati a problemi incompleti

I seguenti utenti non vengono rimossi dai loro ruoli nel progetto quando li rimuovi dalla sezione Persone di un progetto o di un modello:

* Proprietario
* Sponsor

Per ulteriori informazioni sulla rimozione degli utenti dal team di progetto, vedere [Rimuovere gli utenti dai progetti](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).

