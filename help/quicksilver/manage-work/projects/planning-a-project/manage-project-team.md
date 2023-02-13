---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Gestione del team del progetto
description: Il team di progetto è costituito da utenti associati al progetto. I membri del team di progetto vengono visualizzati nella sezione Persone del progetto.
author: Alina
feature: Work Management
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# Gestione del team del progetto

Il team di progetto è costituito da utenti associati al progetto. I membri del team di progetto vengono visualizzati nella sezione Persone del progetto.

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
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti</p> <p>Visualizza o accesso più elevato agli utenti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Aggiungere utenti a un team di progetto

Quando aggiungi utenti al team di progetto, ottengono le autorizzazioni di visualizzazione per il progetto e per le attività, i problemi e i documenti del progetto. Per ulteriori informazioni, consulta l’articolo [Panoramica del team di progetto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Gli utenti del team di progetto non vengono aggiunti automaticamente agli strumenti di gestione delle risorse per il progetto.

Puoi aggiungere utenti al team del progetto nei seguenti modi:

* [Aggiunta automatica di utenti a un team di progetto](#automatically-add-users-to-a-project-team)
* [Aggiunta manuale di utenti a un team di progetto](#manually-add-users-to-a-project-team)

### Aggiunta automatica di utenti a un team di progetto {#automatically-add-users-to-a-project-team}

Gli utenti che svolgono i seguenti ruoli nel progetto vengono aggiunti automaticamente al team del progetto e vengono visualizzati nella sezione Persone al momento della creazione del progetto:

* Il creatore del progetto
* Proprietario del progetto
* Lo sponsor del progetto

Gli utenti vengono inoltre aggiunti automaticamente al team del progetto quando vengono assegnati ai seguenti elementi:

* Attività
* Problemi

### Aggiunta manuale di utenti a un team di progetto {#manually-add-users-to-a-project-team}

Se gli utenti che non svolgono alcun ruolo nel progetto desiderano ricevere notifiche su alcuni aggiornamenti o modifiche durante la durata del progetto, puoi aggiungerli manualmente al team del progetto.

Per ulteriori informazioni sulle notifiche che possono essere abilitate per gli utenti del team di progetto, vedi [Notifiche di eventi disponibili in Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

1. Vai al progetto a cui desideri aggiungere gli utenti.

1. Fai clic su **Persone** nel pannello a sinistra. Potrebbe essere necessario fare clic su **Mostra altro** prima.

1. Fai clic su **Aggiungi utenti**.

   Viene visualizzata la finestra di dialogo Aggiungi utenti al team di progetto.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. In **Aggiungi utenti** inizia a digitare il nome di un utente Workfront attivo che desideri aggiungere al team di progetto, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.

   Ripeti questo passaggio per aggiungere più utenti al team di progetto. Gli utenti devono appartenere al gruppo associato al progetto.

   >[!TIP]
   >
   >* Non è possibile aggiungere utenti aggiungendo i relativi team, gruppi, aziende o ruoli di lavoro.
   >* Man mano che aggiungi gli utenti, noterai l’avatar, il ruolo principale dell’utente e il loro indirizzo e-mail per distinguere tra utenti con nomi identici. Gli utenti devono essere associati ad almeno un ruolo di lavoro per visualizzarlo durante l&#39;aggiunta.



1. Fai clic su **Aggiungi**.

   Gli utenti ottengono le autorizzazioni di visualizzazione per il progetto e ricevono le notifiche relative al progetto come parte del team del progetto.

## Rimuovere utenti da un team di progetto

Quando rimuovi gli utenti dai loro ruoli nel progetto, rimangono parte del team del progetto.

Se si rimuove un utente dal team del progetto e l’utente viene assegnato alle attività o ai problemi del progetto, l’utente viene rimosso dalle attività e dai problemi non completati. In questo caso, le attività e i problemi ritornano all&#39;area di lavoro non assegnata nel bilanciamento del carico di lavoro.

Gli utenti assegnati a attività e problemi completati rimangono assegnati anche dopo la loro rimozione dal team del progetto.

Per ulteriori informazioni sulla rimozione degli utenti dal team del progetto, consulta [Rimuovere utenti dai progetti](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).
