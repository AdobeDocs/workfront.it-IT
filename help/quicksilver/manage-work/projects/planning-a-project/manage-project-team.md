---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Gestione del team di progetto
description: Il team del progetto è costituito da utenti associati al progetto. I membri del team di progetto vengono visualizzati nella sezione Persone del progetto.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# Gestione del team di progetto

Il team del progetto è costituito da utenti associati al progetto. I membri del team di progetto vengono visualizzati nella sezione Persone del progetto.

## Requisiti di accesso

<!--drafted for P&P:
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
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
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
-->

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai progetti</p> <p>Accesso di visualizzazione o superiore agli utenti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront.

## Aggiungere utenti a un team di progetto

Quando aggiungi utenti al team di progetto, questi ottengono le autorizzazioni di visualizzazione per il progetto e le attività, i problemi e i documenti del progetto. Per ulteriori informazioni, consulta l’articolo [Panoramica del team del progetto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Gli utenti del Team di progetto non vengono aggiunti automaticamente agli strumenti di gestione delle risorse per il progetto.

È possibile aggiungere utenti al team di progetto nei modi seguenti:

* [Aggiunta automatica di utenti a un team di progetto](#automatically-add-users-to-a-project-team)
* [Aggiungere manualmente utenti a un team di progetto](#manually-add-users-to-a-project-team)

### Aggiunta automatica di utenti a un team di progetto {#automatically-add-users-to-a-project-team}

Gli utenti che svolgono i seguenti ruoli nel progetto vengono aggiunti automaticamente al team del progetto e vengono visualizzati nella sezione Persone al momento della creazione del progetto:

* Il creatore del progetto
* Proprietario del progetto
* Lo sponsor del progetto

Gli utenti vengono inoltre aggiunti automaticamente al team di progetto quando vengono assegnati ai seguenti elementi:

* Attività
* Problemi

### Aggiungere manualmente utenti a un team di progetto {#manually-add-users-to-a-project-team}

Se gli utenti che non ricoprono alcun ruolo nel progetto desiderano ricevere una notifica su determinati aggiornamenti o modifiche durante il ciclo di vita del progetto, puoi aggiungerli manualmente al team di progetto.

Per ulteriori informazioni sulle notifiche che possono essere abilitate per gli utenti del team di progetto, vedi [Notifiche degli eventi disponibili in Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

1. Vai al progetto a cui desideri aggiungere utenti.

1. Clic **Persone** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro** prima.

1. Clic **Aggiungi utenti**.

   Viene visualizzata la finestra di dialogo Aggiungi utenti al team di progetto.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. In **Aggiungi utenti** digitare il nome di un utente Workfront attivo che si desidera aggiungere al team di progetto, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   Ripeti questo passaggio per aggiungere più utenti al team di progetto. Gli utenti devono appartenere al gruppo associato al progetto.

   >[!TIP]
   >
   >* Non puoi aggiungere utenti aggiungendo i loro team, gruppi, aziende o mansioni.
   >* Quando aggiungi gli utenti, osserva l’avatar, il Ruolo principale dell’utente e il suo indirizzo e-mail per distinguere gli utenti con nomi identici. Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono aggiunti.
   >
   >  Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, consulta [Concedere l’accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. Clic **Aggiungi**.

   Gli utenti ottengono le autorizzazioni di visualizzazione per il progetto e ricevono notifiche sul progetto come parte del team del progetto.

## Rimuovere utenti da un team di progetto

Quando rimuovi gli utenti dai loro ruoli sul progetto, questi rimangono parte del team del progetto.

Se si rimuove un utente dal team del progetto e l&#39;utente viene assegnato ad attività o problemi del progetto, l&#39;utente non viene assegnato alle attività e ai problemi non completati. In questo caso, le attività e i problemi tornano nell’area Lavoro non assegnato nel Bilanciatore dei carichi di lavoro.

Gli utenti assegnati ad attività e problemi completati rimangono assegnati anche dopo la loro rimozione dal team di progetto.

Per ulteriori informazioni sulla rimozione degli utenti dal team di progetto, vedi [Rimuovere utenti dai progetti](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).
