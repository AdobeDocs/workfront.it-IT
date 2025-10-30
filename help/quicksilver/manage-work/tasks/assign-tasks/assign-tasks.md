---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Assegna le Attività
description: È possibile assegnare attività a utenti, ruoli o team per indicare chi è responsabile del completamento delle attività. È possibile assegnare un'attività a più risorse contemporaneamente.
author: Lisa
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: ac5552f1c235f595b1c0d2558fcf88b1e03f5a8e
workflow-type: tm+mt
source-wordcount: '1829'
ht-degree: 1%

---

# Assegna attività

<!--Audited: 10/2025-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 
-->

È possibile assegnare attività a utenti, mansioni o team per indicare chi è responsabile del completamento delle attività. È possibile assegnare un&#39;attività a più risorse contemporaneamente.

>[!TIP]
>
>Puoi assegnare più utenti, mansioni o team. Puoi assegnare solo utenti attivi, mansioni e team.
>
>Se un utente, una mansione o un team è stato assegnato prima della disattivazione, rimane assegnato all&#39;elemento di lavoro. In questo caso, consigliamo quanto segue:
>
>* Riassegnare l&#39;elemento di lavoro alle risorse attive.
>* Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.
>

Il numero di utenti assegnati a un&#39;attività e la pianificazione del proprietario dell&#39;attività possono modificare le date pianificate di un&#39;attività, modificando la sequenza temporale del progetto. Per informazioni sull&#39;impatto dell&#39;assegnazione di più utenti a un&#39;attività, vedere [Panoramica sulla modifica delle assegnazioni di attività](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

Oltre a questo articolo, si consiglia di leggere i seguenti articoli per ulteriori informazioni sull&#39;assegnazione delle attività:

* [Panoramica sulla modifica delle assegnazioni di attività](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [Panoramica assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Assegnazioni intelligenti](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Crea assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Modificare più assegnazioni utente in un elenco attività](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Pianifica una panoramica del progetto](../../../manage-work/projects/planning-a-project/plan-project.md)
* [Panoramica della data di completamento pianificata dell&#39;attività](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Imposta la data di completamento pianificata del progetto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [Panoramica sull’assegnazione del lavoro nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Lavoro o superiore</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Progetti e Attività</p> <p>Accesso di visualizzazione o superiore agli utenti</p> </td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni oggetto</td>
   <td>Autorizzazioni di contribuzione o di livello superiore per l'attività</td>
  </tr>
 </tbody>
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni per più assegnazioni a mansioni, team e utenti

Quando si assegnano più risorse a un elemento di lavoro, tenere presente quanto segue:

* Gli utenti possono avere più di una mansione associata al loro profilo. Per informazioni sull&#39;associazione degli utenti alle mansioni, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Se si assegnano più utenti a un&#39;attività o a un problema, il primo utente selezionato viene automaticamente designato come proprietario dell&#39;attività o del problema.
Per istruzioni su come modificare questa impostazione, vedere le informazioni sull&#39;opzione Rendi primario nell&#39;articolo [Crea assegnazioni avanzate](create-advanced-assignments.md).

* Un team non può essere un assegnatario principale di un&#39;attività o di un problema. Solo un utente o una mansione può essere designata come principale per un’attività o un problema.

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* Le attività e i problemi di un progetto possono essere assegnati prima a uno o più team o mansioni. Quando il progetto è pronto per iniziare, potrebbe essere necessario assegnarlo anche agli utenti:

  <table>
  <col> 
  <col> 
  <tbody>
  <tr>
   <td>Team</td>
   <td>Se si assegna un'attività a un team e si assegna anche un utente, l'attività rimane assegnata al team e all'utente, anche se l'utente non è membro del team.</td>
  </tr>
  <tr>
   <td>Mansioni</td>
   <td><p>Se assegni un’attività o un problema a uno o più ruoli e successivamente assegni anche un utente, decide quale ruolo associare all’utente aggiuntivo (se presente) in base alle seguenti regole:</p>
     <ul>
      <li>Se a un ruolo è assegnato un solo e questo corrisponde al ruolo principale dell’utente (configurato nel suo profilo), l’attività o il problema viene assegnato solo a tale utente.</li>
      <li>Se vengono assegnati più ruoli e almeno uno di essi corrisponde a uno degli altri ruoli dell’utente, l’attività o il problema viene assegnato all’utente (il ruolo viene selezionato in modo casuale se ci sono più corrispondenze), insieme a eventuali ruoli aggiuntivi assegnati</li>
      <li>Se viene assegnata almeno una mansione e non vi sono corrispondenze con le mansioni dell’utente, l’attività o il problema viene assegnato sia alla mansione o alle mansioni che all’utente.</li>
     </ul>
   <p>Per informazioni sul ruolo principale di un utente e altri ruoli, vedere <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Modificare il profilo di un utente</a>.</p>
   </td> 
     </tr>
  </tbody>
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations for multiple user assignments and using schedules</h2>
<p>(NOTE: moved to the Modify task assignments overview standalone article)</p>
<p>You can assign multiple resources to a task. When you assign a user to a task, Workfront uses the user's schedule to calculate the planned dates for the task which ultimately determine the timeline of the project. Using the schedule of the user takes into account their time off, holidays, and weekend days which are considered non-working days when task activity cannot occur. </p>
<p>When you assign multiple users to a task, your Workfront administrator <span>or a group administrator</span> determines which one of the following schedules Workfront uses to determine the planned dates of the tasks, based on schedules: </p>
<ul>
<li> <p><strong>The Primary Assignee's schedule</strong>: this is the schedule associated with the user designated as the task Owner.</p> <p>For information about associating users with schedules, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li>
<li><strong>The Project's schedule</strong>: this is the schedule associated with the project. For adding a schedule to a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
</ul>
<p>For information about setting up which schedule a project uses in the case of multiple assignments, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p>
</div>
-->

## Assegna una singola attività

1. Passare a un&#39;attività che si desidera assegnare.
1. Fai clic su **Assegna a** nel campo **Assegnazioni** nell&#39;intestazione dell&#39;attività

   Oppure

   Fare clic sul nome delle assegnazioni se l&#39;attività è già assegnata.

   ![Assegnazioni](assets/assignments-from-task-header-0825.png)

1. Esegui una delle operazioni seguenti:

   * Inizia a digitare il nome di un utente, una mansione o un team che desideri assegnare, quindi fai clic su di esso quando viene visualizzato nell’elenco.

     >[!TIP]
     >
     >Quando aggiungi un’assegnazione utente, osserva l’avatar, il ruolo principale dell’utente o il suo indirizzo e-mail per distinguere gli utenti con nomi identici. Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono aggiunti.
     >
     >Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, vedere [Concedere l&#39;accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

     <!--When adding a job role assignment, you can search for the job role or location. Select a role from the Job roles list to use the default billing rate for the assignment, or select a Rate card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md). -->

   * (Condizionale) Fai clic su uno dei nomi negli elenchi **Utenti e team** o **Ruoli** quando vengono visualizzati. Per ulteriori informazioni, vedere [Panoramica assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

     È possibile iniziare a digitare il nome di qualsiasi utente, team o mansione da assegnare all&#39;attività, quindi selezionarlo quando viene visualizzato nell&#39;elenco.

   * Fai clic su **Avanzate**

     Per informazioni su come effettuare assegnazioni avanzate, vedere [Creare assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Fai clic su **Salva**.
1. (Facoltativo e condizionale) Se hai fatto clic su **Avanzate**, fai clic sull&#39;icona **X** accanto al nome dell&#39;assegnazione nel pannello di destra dell&#39;attività per rimuovere un&#39;assegnazione.

## Assegnare un&#39;attività in un elenco quando viene modificato in linea

È possibile assegnare attività in un elenco o in un report quando uno qualsiasi dei campi delle assegnazioni è visibile nella visualizzazione dell&#39;elenco. Si tratta di un metodo più veloce per assegnare le attività. In questo articolo viene descritto come modificare le assegnazioni di un&#39;attività in un elenco. Per informazioni sulla modifica di più assegnazioni per più attività in un elenco, vedere [Modificare più assegnazioni utente in un elenco attività](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

A seconda del campo visibile nella visualizzazione, è possibile assegnare le seguenti entità all&#39;attività:

| Campo | Entità assegnate |
|---|---|
| **Assegna a** | Assegna un utente |
| **Assegnato** | Assegna un utente |
| **Assegnazioni** | Assegnare utenti, mansioni o team |

Per assegnare le attività in un elenco:

1. Consente di passare a un elenco di attività contenente i campi Assegnato a, Assegnato o Assegnazioni nella visualizzazione.
1. (Facoltativo) Fai clic sul menu a discesa **Salvataggio automatico** e seleziona una delle seguenti opzioni:

   | Opzione | Descrizione opzione |
   |---|---| 
   | Salvataggio automatico | Le modifiche apportate alle attività vengono salvate automaticamente e non è possibile ripristinarle |
   | Salvataggio manuale | È necessario salvare manualmente le modifiche. È possibile ripristinare le modifiche prima di salvarle. |
   | Pianificazione timeline | È necessario salvare manualmente le modifiche. È possibile ripristinare le modifiche prima di salvarle. Il salvataggio delle modifiche e di tutte le dipendenze del progetto è più rapido rispetto a quando si seleziona Salvataggio manuale. |

   Per ulteriori informazioni sul salvataggio delle attività durante la modifica in un elenco, vedere [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Per assegnare le attività, effettuare una delle seguenti operazioni:

   * Fai clic all&#39;interno dei campi **Assegnato a** o **Assegnato** e inizia a digitare il nome di un utente attivo che desideri assegnare all&#39;attività, quindi fai clic su di esso quando viene visualizzato nell&#39;elenco.
   * Fai clic all&#39;interno del campo **Assegnazioni** e inizia a digitare il nome di un utente attivo, una mansione o un team che desideri assegnare all&#39;attività, quindi fai clic su di esso quando viene visualizzato nell&#39;elenco.

     >[!TIP]
     >
     >Quando aggiungi un’assegnazione utente, osserva l’avatar, il ruolo principale dell’utente o il suo indirizzo e-mail per distinguere gli utenti con nomi identici. Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono aggiunti.
     >
     >Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, vedere [Concedere l&#39;accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)

     <!--<span class="preview">When adding a job role assignment, you can search for the job role or location. Select a Job role to use the default billing rate for the assignment, or select a Rate Card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>-->


1. (Condizionale) Nel campo Assegnazioni, fai clic su **Avanzate** nella parte inferiore dell&#39;elenco oppure sull&#39;icona **Persone** ![Persone](assets/teams.png) nell&#39;angolo superiore destro della casella Assegnazioni, per aprire la casella **Assegnazioni avanzate** e creare assegnazioni avanzate.

   Per ulteriori informazioni, vedere [Creare assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Non è possibile effettuare assegnazioni avanzate dai campi Assegnato a o Assegnato.

1. Dopo aver aggiunto gli assegnatari all’attività, premi Invio o fai clic in un punto qualsiasi della pagina per salvare le modifiche, se hai selezionato Salvataggio automatico. In caso contrario, fare clic su **Salva**.

## Assegnare più attività a un utente in blocco da un elenco

<!--Assigning multiple tasks to a user is different, depending on what environment you use to assign the tasks. 

### Assign multiple tasks to a user in the Production environment-->

1. Passare a un elenco di attività che si desidera assegnare in blocco.
1. (Condizionale) Verificare che l&#39;opzione **Salvataggio automatico** sia selezionata se ci si trova in un elenco di attività di un progetto.

   >[!IMPORTANT]
   >
   >Non è possibile modificare le attività in blocco quando si salvano le attività manualmente in un progetto.

1. Selezionare più attività nell&#39;elenco delle attività.
1. Fai clic su **Modifica**.

   Viene visualizzata la finestra di dialogo **Modifica attività**.

1. Nell&#39;area **Assegnazioni** selezionare la casella **Assegnatario**, quindi iniziare a digitare il nome di un utente, una mansione o un team che si desidera assegnare a tutte le attività.

   >[!IMPORTANT]
   >
   >Se una delle attività è già assegnata, le risorse indicate in questo campo vengono aggiunte alle attività anziché sostituire le risorse esistenti sulle attività.

1. (Facoltativo) Selezionare il pulsante di opzione nella colonna **Proprietario attività** per indicare quale risorsa è l&#39;assegnatario principale o il proprietario dell&#39;attività quando si assegnano più risorse all&#39;attività. Questa funzione non è disponibile per i team.
1. (Condizionale) Specificare l&#39;**Allocazione %** per ogni risorsa assegnata all&#39;attività se tutte le attività selezionate hanno un Tipo di durata di Impegno o Assegnazione calcolata. Indica quanto tempo queste risorse devono dedicare al completamento dell&#39;attività. Questa opzione è disponibile solo per gli utenti e le mansioni.

   Oppure

   Specifica la quantità di **Ore** per ogni risorsa assegnata all&#39;attività se tutte le attività selezionate hanno un Tipo di durata semplice. Il totale di tutte le ore per tutte le risorse deve corrispondere al numero di ore pianificate per l&#39;attività.

   >[!IMPORTANT]
   >
   >Non è possibile specificare la percentuale di allocazione o il numero di ore per risorsa se le attività selezionate hanno tipi di durata diversi o se le attività selezionate hanno tipi di durata diversi.

   Per informazioni sul Tipo di Durata per le attività, vedere [Panoramica sulla Durata dell&#39;Attività e sul Tipo di Durata](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Facoltativo) Seleziona un ruolo che l&#39;utente deve svolgere sull&#39;attività dal menu a discesa **Scegli un ruolo** nella colonna **Ruolo dell&#39;assegnatario** quando assegni gli utenti alle attività. Se non si seleziona un ruolo, Workfront seleziona automaticamente il ruolo principale dell&#39;utente.

1. (Facoltativo) Se si desidera rimuovere assegnatari esistenti da tutte le attività, effettuare una delle seguenti operazioni:

   1. Inizia a digitare il nome di un utente, una mansione o un team che desideri rimuovere dall&#39;attività, quindi selezionalo quando viene visualizzato nell&#39;elenco e fai clic su **Rimuovi assegnatario** per rimuovere altri assegnatari.
   1. Fare clic su **Rimuovi tutti gli assegnatari esistenti** per rimuovere tutti gli assegnatari da tutte le attività selezionate.

1. Fai clic su **Salva modifiche**.
1. (Facoltativo e condizionale) Quando i campi Assegnato a o Assegnazioni vengono visualizzati nell&#39;elenco delle attività, fare clic all&#39;interno di una di queste colonne per un&#39;attività, quindi fare clic sull&#39;icona **X** accanto al nome di un assegnatario per rimuoverlo dall&#39;attività.

<!--
<div class="preview">

### Assign multiple tasks to a user in the Preview environment

1. Go to a list of tasks that you want to assign in bulk in the Preview environment. 
1. (Conditional) Ensure that the **Autosave** option is selected if you are on a list of tasks under a project.

   >[!IMPORTANT]
   >
   >You cannot edit tasks in bulk when saving tasks manually on a project.

1. Select several tasks in the tasks list. 
1. Click **Edit**.

   The **Edit Tasks** dialog box opens.

1. In the **Assignments** area, start typing the name of users, teams, or roles in the **Search people, roles, or teams** field provided, then click them when they display in the list

   Or 

   Click **Assign to me** to assign it to yourself.

   >[!IMPORTANT]
   >
   >If any of the tasks is already assigned, the resources you indicate here are added to the tasks instead of replacing the existing resources on the tasks.

1. Click inside the **Duration Type** field and choose a Duration Type. 

   For information about Duration Type on tasks, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Conditional) Depending on what **Duration Type** you selected, update the following fields: 

   * Duration
   * Planned Hours

      For more information, see [Edit tasks](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md). 

1. (Optional) If you want to remove existing assignees from all tasks, click the **x** next to their name in the **Search people, roles, or teams** field.

1. Click **Save**.
1. (Optional and conditional) When the Assigned to or the Assignments fields display in your list of tasks, click inside one of these columns for a task, then click the **X icon** next to the name of an assignee to remove it from the task.


</div>
-->



<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations about unassigning tasks</h2>
<p>(NOTE: moved this to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm)</p>
<p>You can remove assignments from one task at a time, or you can remove assignments from multiple tasks in bulk.</p>
<p>For more information about removing assignments from tasks in bulk, see <a href="../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md" class="MCXref xref">Modify multiple user assignments in a task list</a>. </p>
<p>Consider the following when removing assignments from tasks: </p>
<ul>
<li>When you unassign a user from a task, the task remains assigned to the job role that the user fulfilled on the task.</li>
<li>When you unassign a job role or a team from a task, the task remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->


