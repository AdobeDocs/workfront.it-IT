---
product-area: projects
navigation-topic: manage-issues
title: Assegna problemi
description: Puoi assegnare i problemi a utenti, ruoli e team per indicare chi è responsabile del completamento dei problemi. Per informazioni generali sull'assegnazione dei problemi, vedere Cenni preliminari sulla modifica delle assegnazioni dei problemi.
author: Lisa
feature: Work Management
role: User
exl-id: e2dce29e-7370-4580-8326-99c4437998bf
source-git-commit: 0358e79bd606d0035959bba2a47256456b529b18
workflow-type: tm+mt
source-wordcount: '1366'
ht-degree: 0%

---

# Assegna problemi

<!--Audited: 10/2024-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

Puoi assegnare i problemi a utenti, ruoli e team per indicare chi è responsabile del completamento dei problemi. Per informazioni generali sull&#39;assegnazione dei problemi, vedere [Panoramica sulla modifica delle assegnazioni dei problemi](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!TIP]
>
>Puoi assegnare più utenti, mansioni o team. Puoi assegnare solo utenti attivi, mansioni e team.
>
>Se un utente, una mansione o un team è stato assegnato prima della disattivazione, rimane assegnato all&#39;elemento di lavoro. In questo caso, consigliamo quanto segue:
>
>* Riassegnare l&#39;elemento di lavoro alle risorse attive.
>* Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.

Oltre a questo articolo, si consiglia di leggere i seguenti articoli per ulteriori informazioni sull’assegnazione dei problemi:

* [Panoramica sulla modifica delle assegnazioni dei problemi](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)
* [Modifica problemi](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Modifica le assegnazioni utente per più problemi in un elenco](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md)
* [Crea assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Assegnazioni intelligenti](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Panoramica assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Panoramica sull’assegnazione del lavoro nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

È possibile assegnare un problema a una o più risorse a livello di singolo problema oppure più risorse a più problemi contemporaneamente.

L’assegnazione di problemi e attività è simile in Adobe Workfront. Per informazioni generali sull&#39;assegnazione delle attività, vedere [Panoramica sulla modifica delle assegnazioni delle attività](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 </col>
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td> <p>Collaboratore o versione successiva</p>
   <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso alle Issues</p> <p>Accesso di visualizzazione o superiore a progetti e attività per assegnare un problema</p> </td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il problema</p> <p> Visualizzare le autorizzazioni o versioni successive per il progetto o l’attività in cui si trova il problema, quando si assegna un problema</p><p>Quando si assegnano più problemi, contribuire con autorizzazioni o versioni successive al progetto o all’attività in cui si trova il problema.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni per più assegnazioni a mansioni, team e utenti

Quando si assegnano più risorse a un elemento di lavoro, tenere presente quanto segue:

* Gli utenti possono avere più di una mansione associata al loro profilo. Per informazioni sull&#39;associazione degli utenti alle mansioni, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Le attività o i problemi vengono in genere prima assegnati a uno o più ruoli o team. Quando i progetti sono pronti per essere avviati, potrebbe essere necessario assegnarli anche agli utenti.

  Se un’attività o un problema è assegnato a uno o più ruoli e successivamente si assegna anche un utente, Adobe Workfront decide quale ruolo associare all’utente aggiuntivo (se presente) in base alle seguenti regole:

   * Se è stata assegnata una sola mansione e questa corrisponde alla mansione principale dell’utente, l’attività o il problema viene assegnato solo all’utente che svolge la sua mansione principale.
   * Se sono stati assegnati più ruoli e almeno uno dei ruoli corrisponde ai ruoli secondari dell’utente, l’attività o il problema viene assegnato all’utente che svolge uno dei suoi Altri ruoli, che Workfront seleziona in modo casuale in caso di più corrispondenze, nonché a eventuali ruoli aggiuntivi assegnati.
   * Se sono state assegnate una o più mansioni e non vi sono corrispondenze ai ruoli dell’utente, l’attività o il problema viene assegnato sia al ruolo o alle mansioni che all’utente.

* Se un’attività o un problema è assegnato a un team e si assegna anche un utente, l’attività o il problema rimane assegnato sia al team che all’utente.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2> </h2>
<h2>Considerations about removing assignments from issues</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to Modify issue assignments overview article)</p>
<p>You can remove assignments from one issue at a time, or you can remove assignments from multiple issues in bulk.</p>
<p>For more information about removing assignments from issues in bulk, see <a href="../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md" class="MCXref xref">Modify user assignments for multiple issues in a list</a>. </p>
<p>Consider the following when removing assignments from issues: </p>
<ul>
<li>When you unassign a user from an issue, the issue remains assigned to the job role that the user fulfilled on the issue.</li>
<li>When you unassign a job role or a team from an issue, the issue remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->

## Assegnare un singolo problema nell’intestazione del problema

1. Passa al problema che desideri assegnare.
1. Fai clic su **Assegna a** nell&#39;angolo superiore destro dell&#39;intestazione del problema, nell&#39;area **Assegnazioni**

   Oppure

   Se il problema è già stato assegnato, fai clic sul nome delle assegnazioni correnti.

   ![Assegna al pulsante](assets/assign-to-button-in-header.png)

1. Esegui una delle operazioni seguenti:

   * Inizia a digitare il nome di un utente, una mansione o un team che desideri assegnare, quindi fai clic su di esso quando viene visualizzato nell’elenco.

     ![Ricerca assegnazioni](assets/smart-assignments-issue-header.png)

   * (Condizionale) Fai clic su uno dei nomi, dei ruoli o dei team negli elenchi disponibili
   * Fai clic su **Assegna a me** per assegnarti
   * Fare clic su **Avanzate**.

     La creazione di assegnazioni avanzate è simile per attività e problemi. Per informazioni su come effettuare assegnazioni avanzate, vedere [Creare assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

     >[!TIP]
     >
     >Quando aggiungi un’assegnazione utente, osserva l’avatar, il ruolo principale dell’utente o il suo indirizzo e-mail per distinguere gli utenti con nomi identici.
     >
     >Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono aggiunti.
     >
     >Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, vedere [Concedere l&#39;accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
     >

     <!-- this doesn't apply to issues; if it does, add this to the TIP above: 
      ><span class="preview">When adding a job role assignment, you can search for the job role or location. Select a role from the Job roles list to use the default billing rate for the assignment, or select a Rate card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>-->


1. Fai clic su **Salva** per completare l&#39;assegnazione del problema.
1. (Facoltativo) Fai clic sull&#39;icona **X** accanto al nome delle assegnazioni nell&#39;area Assegnazioni nell&#39;intestazione del problema per rimuovere un&#39;assegnazione.

## Assegnare un problema modificandolo in linea in un elenco

È possibile assegnare problemi in un elenco o in un report quando uno qualsiasi dei campi di assegnazione è visibile nella visualizzazione dell&#39;elenco. Questo è un modo più veloce per assegnare i problemi.

A seconda del campo visibile nella vista, puoi assegnare le seguenti entità al problema:

| Opzione | Entità assegnate |
|---|---|
| **Assegna a** | Assegna un utente |
| **Assegnato** | Assegna un utente |
| **Assegnazioni** | Assegna utenti, mansioni o team. |

Per assegnare i problemi in un elenco:

1. Consente di passare a un elenco di problemi con i campi Assegnato a, Assegnato o Assegnazioni nella visualizzazione.
1. Per assegnare i problemi, effettuare una delle seguenti operazioni:

   * Fai clic all&#39;interno dei campi **Assegnato a** o **Assegnato** e inizia a digitare il nome di un utente attivo che desideri assegnare al problema, quindi fai clic su di esso quando viene visualizzato nell&#39;elenco.

     ![Assegnato al campo](assets/assigned-to-field-task-list-nwe.png)

   * Fai clic all&#39;interno del campo **Assegnazioni** e inizia a digitare il nome di un utente attivo, una mansione o un team attivo che desideri assegnare al problema, quindi fai clic su di esso quando viene visualizzato nell&#39;elenco.

     ![Campo assegnazioni](assets/assignments-field-0825.png)

   >[!TIP]
   >
   >Quando aggiungi un’assegnazione utente, osserva l’avatar, il ruolo principale dell’utente o il suo indirizzo e-mail per distinguere gli utenti con nomi identici.
   >
   >Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono aggiunti.
   >
   >Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, vedere [Concedere l&#39;accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. (Condizionale) Nel campo Assegnazioni fare clic su **Avanzate** nella parte inferiore dell&#39;elenco oppure sull&#39;icona **Persone** ![Persone](assets/teams.png) nell&#39;angolo superiore destro della casella Assegnazioni per aprire la casella Assegnazioni avanzate e creare assegnazioni avanzate. Per ulteriori informazioni, vedere [Creare assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Non è possibile effettuare assegnazioni avanzate dai campi Assegnato a o Assegnato.

1. Dopo aver aggiunto gli assegnatari al problema, premi Invio o fai clic in un punto qualsiasi della pagina per salvare le modifiche.

## Assegnare un problema nella casella Modifica problema

Puoi assegnare un problema quando lo modifichi nella casella Modifica problema.

Per informazioni, vedere la sezione &quot;Assegnazioni&quot; nell&#39;articolo [Modifica problemi](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).

## Assegna problemi in blocco

<!--
Assigning issues in bulk is different depending on what environment you choose to do this. 

### Assign issues in bulk in the Production environment 

1. Go to a list of issues that you want to assign in bulk. 
1. Select several issues in the list. 
1. Click the **Edit icon** ![Edit icon](assets/qs-edit-icon.png).

   The **Edit Issues** dialog box opens.

1. In the **Assignments** area, select the **Assignee** box, then start typing the name of a user, job role, or team that you want to assign to all the issues.

   >[!IMPORTANT]
   >
   >If any of the issues is already assigned, the resources you indicate here are added to the issues instead of replacing the existing resources on the issues. 
   
1. (Optional) Select the radio button in the **Issue Owner** column to indicate which resource is the primary assignee or the Owner of the issue, when you assign more than one resource to the issue. This is not available for teams. 
1. (Optional) Select a role that the user should fulfill on the issue from the **Pick a role** drop-down menu in the **Assignee's Role** column when you assign users to issues. If you do not select a role, Workfront automatically selects the user's Primary Role. 

1. (Optional) If you want to remove existing assignees from all issues do one of the following:

   1. Start typing the name of a user, role, or team you want to remove from the issue, then select it when it appears on the list and click **Remove Assignee** to add additional assignees to remove. 
   1. Click **Remove All Existing Assignees** to remove all assignees from all selected issues.

1. Click **Save Changes**.
1. (Optional and conditional) When the Assigned to or the Assignments fields display in your list of issues, click inside one of these columns for an issue, then click the **X icon** next to the name of an assignee to remove it from the issue.

<div class="preview">

### Assign issues in bulk in the Preview environment

-->

1. Passare a un elenco di problemi che si desidera assegnare in blocco.
1. Seleziona diversi problemi nell’elenco.
1. Fai clic sull&#39;icona **Modifica** ![Modifica](assets/qs-edit-icon.png).

   Viene visualizzata la finestra di dialogo **Modifica problemi**.

1. Fai clic su **Assegnazioni** nel pannello a sinistra e, nell&#39;area **Assegnazioni**, inizia a digitare il nome di un utente, una mansione o un team nel campo **Cerca persone, ruoli o team**, quindi fai clic su di esso quando viene visualizzato nell&#39;elenco

   Oppure

   Fai clic su **Assegna a me** per assegnare i problemi a te stesso.

   >[!IMPORTANT]
   >
   >Se uno dei problemi è già assegnato, le risorse indicate qui vengono aggiunte ai problemi invece di sostituire le risorse esistenti sui problemi.

1. (Facoltativo) Se vuoi rimuovere assegnatari esistenti da tutti i problemi, fai clic su **x** accanto al loro nome.

1. (Facoltativo) Aggiorna il campo P **Ore pianificate**. Per ulteriori informazioni, vedere [Modifica problemi](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).

1. Fai clic su **Salva**.
1. (Facoltativo e condizionale) Quando i campi **Assegnato a** o **Assegnazioni** vengono visualizzati nell&#39;elenco dei problemi, fai clic su una di queste colonne per segnalare un problema, quindi fai clic sull&#39;icona **X** accanto al nome di un assegnatario per rimuoverlo dal problema.


