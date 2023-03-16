---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Assegnare le attività
description: È possibile assegnare attività a utenti, ruoli o team per indicare chi è responsabile del completamento delle attività. È possibile assegnare un'attività a più di una risorsa alla volta.
author: Alina
feature: Work Management
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '1789'
ht-degree: 1%

---

# Assegnare le attività

È possibile assegnare attività a utenti, ruoli o team per indicare chi è responsabile del completamento delle attività. È possibile assegnare un&#39;attività a più di una risorsa alla volta.

>[!TIP]
>
>È possibile assegnare più utenti, ruoli o team. È possibile assegnare solo utenti attivi, ruoli e team.
>
>Se un utente, un ruolo di lavoro o un team è stato assegnato prima della disattivazione, rimangono assegnati all&#39;elemento di lavoro. In questo caso, si consiglia quanto segue:
>
>* Riassegna l&#39;elemento di lavoro alle risorse attive.
>* Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.
>


Il numero di utenti assegnati a un&#39;attività e la pianificazione del proprietario dell&#39;attività possono modificare le date pianificate di un&#39;attività, il che comporta la modifica della cronologia del progetto. Per informazioni sull&#39;impatto dell&#39;assegnazione di più utenti a un&#39;attività, vedere [Panoramica sulla modifica delle assegnazioni di attività](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

Oltre a questo articolo, si consiglia di leggere i seguenti articoli per ulteriori informazioni sull&#39;assegnazione delle attività:

* [Panoramica sulla modifica delle assegnazioni di attività](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [Panoramica delle assegnazioni intelligenti](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Esecuzione di assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Creazione di assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Modificare più assegnazioni utente in un elenco di attività](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [Modifica delle attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Pianificare una panoramica del progetto](../../../manage-work/projects/planning-a-project/plan-project.md)
* [Panoramica dell&#39;attività Data completamento pianificata](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Imposta la data di completamento pianificato del progetto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [Panoramica dell’assegnazione del lavoro nel servizio di bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## Requisiti di accesso

<!--drafted for P&P - replace table below with this:

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Tasks</p> <p>View or higher access to Users</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to tasks</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti e attività</p> <p>Visualizza o accesso più elevato agli utenti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Collaborare o autorizzazioni superiori per le attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Considerazioni relative a più assegnazioni a ruoli, team e utenti del processo

Quando si assegnano più risorse a un elemento di lavoro, tenere presente quanto segue:

* Gli utenti possono avere più di un ruolo di lavoro associato al loro profilo. Per informazioni sull’associazione degli utenti ai ruoli di lavoro, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Se si assegnano più utenti a un&#39;attività o a un problema, il primo utente selezionato viene designato automaticamente come proprietario dell&#39;attività o del problema.
Per istruzioni su come modificare questa impostazione, consulta le informazioni sull’opzione Rendi principale nell’articolo [Creazione di assegnazioni avanzate](create-advanced-assignments.md).

* Un team non può essere un assegnatario primario per un&#39;attività o un problema. Solo un utente o un ruolo di lavoro può essere designato come primario su un&#39;attività o un problema.

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* Le attività e i problemi relativi a un progetto possono essere assegnati per prime a uno o più team o ruoli di lavoro. Quando il progetto è pronto per essere avviato, potrebbe essere necessario assegnarli anche agli utenti:

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
   <td><p>Se assegni un'attività o un problema a uno o più ruoli e poi assegni anche un utente, decide quale ruolo di lavoro associare all'utente aggiuntivo (se presente) in base alle regole seguenti:</p>
     <ul>
      <li>Se è assegnato un solo ruolo di lavoro e corrisponde al ruolo principale dell’utente (configurato nel suo profilo), l’attività o il problema viene assegnato solo a tale utente.</li>
      <li>Se vengono assegnati più ruoli e almeno uno di essi corrisponde a uno degli altri ruoli dell’utente, l’attività o il problema viene assegnato all’utente (il ruolo viene selezionato in modo casuale se sono presenti più corrispondenze), insieme a eventuali ruoli aggiuntivi assegnati</li>
      <li>Se viene assegnato almeno un ruolo di lavoro e non sono presenti corrispondenze ai ruoli di lavoro dell'utente, l'attività o il problema viene assegnato sia al ruolo o ai ruoli che all'utente.</li>
     </ul>
   <p>Per informazioni sul ruolo principale di un utente e su altri ruoli, consulta <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Modificare il profilo di un utente</a>.</p>
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

## Assegnare una singola attività

1. Passare a un&#39;attività che si desidera assegnare.
1. Fai clic su **Assegna a** in **Assegnazioni** nell’intestazione dell’attività o del problema.

   Oppure

   Fare clic sul nome delle assegnazioni se l&#39;attività o il problema è già assegnato.

![](../assign-tasks/assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. Esegui una delle operazioni seguenti:

   * Iniziare a digitare il nome di un utente, un ruolo o un team che si desidera assegnare, quindi fare clic su di esso quando viene visualizzato nell&#39;elenco.


      >[!TIP]
      >
      >Quando aggiungi un&#39;assegnazione utente, osserva l&#39;avatar, il ruolo principale dell&#39;utente o il relativo indirizzo e-mail per distinguere tra utenti con nomi identici. Gli utenti devono essere associati ad almeno un ruolo di lavoro per visualizzarlo durante l&#39;aggiunta.


   * (Condizionale) Fai clic su uno dei nomi nel **Assegnazioni consigliate** se viene visualizzato questo elenco. Per ulteriori informazioni, consulta [Panoramica delle assegnazioni intelligenti](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

   * Fai clic su **Avanzate**

      Per informazioni su come effettuare assegnazioni avanzate, vedere [Creazione di assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Fai clic su **Salva**.
1. (Facoltativo e condizionale) Fai clic sul pulsante **Icona X** accanto al nome dell&#39;assegnazione nel pannello a destra dell&#39;attività da rimuovere, se si fa clic su **Avanzate**.

## Assegnare un’attività in un elenco

È possibile assegnare le attività in un elenco o in un rapporto quando uno dei campi delle assegnazioni è visibile nella visualizzazione dell&#39;elenco. Questo è un modo più veloce per assegnare le attività. Questo articolo descrive come modificare le assegnazioni per un&#39;attività in un elenco. Per informazioni sulla modifica di più assegnazioni per più attività in un elenco, vedere [Modificare più assegnazioni utente in un elenco di attività](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

A seconda del campo visibile nella visualizzazione, è possibile assegnare all&#39;attività le seguenti entità:

| Campo | Entità assegnate |
|---|---|
| **Assegna a** | Assegnare un utente |
| **Assgnt** | Assegnare un utente |
| **Assegnazioni** | Assegnare utenti, ruoli o team |

Per assegnare attività in un elenco:

1. Passare a un elenco di attività con i campi Assegnato a, Assegnato o Assegnazioni nella visualizzazione.
1. (Facoltativo) Fai clic sul pulsante **Salvataggio automatico** dal menu a discesa e seleziona una delle seguenti opzioni:

   | Opzione | Descrizione opzione |
   |---|---| 
   | Salvataggio automatico | Le modifiche apportate alle attività vengono salvate automaticamente e non è possibile ripristinarle |
   | Salvataggio manuale | È necessario salvare manualmente le modifiche. È possibile ripristinare le modifiche prima di salvarle. |
   | Pianificazione sequenza temporale | È necessario salvare manualmente le modifiche. È possibile ripristinare le modifiche prima di salvarle. Il salvataggio delle modifiche e di tutte le dipendenze del progetto è più rapido rispetto alla selezione del salvataggio manuale. |

   Per ulteriori informazioni sul salvataggio delle attività durante la modifica in un elenco, vedere [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Per assegnare le attività, eseguire una delle operazioni seguenti:

   * Fai clic all’interno del **Assegnato a** o **Assegnato** campi e iniziare a digitare il nome di un utente attivo che si desidera assegnare all&#39;attività, quindi fare clic su di esso quando viene visualizzato nell&#39;elenco.
   * Fai clic all’interno del **Assegnazioni** e iniziare a digitare il nome di un utente attivo, di un ruolo o di un team che si desidera assegnare all&#39;attività, quindi fare clic su di essa quando viene visualizzato nell&#39;elenco.

      >[!TIP]
      >Quando aggiungi un&#39;assegnazione utente, osserva l&#39;avatar, il ruolo principale dell&#39;utente o il relativo indirizzo e-mail per distinguere tra utenti con nomi identici. Gli utenti devono essere associati ad almeno un ruolo di lavoro per visualizzarlo durante l&#39;aggiunta.
      >
      >
   >

1. (Condizionale) Quando è visibile nel **Assegnazioni** fai clic sul campo **Persone** nell&#39;angolo superiore destro della casella assegnazioni per aprire **Assegnazioni avanzate** e creare assegnazioni avanzate.

   <!--
   there is a People icon in NWE but it's hard to see - you need to assign the task to at least 2 users, not roles, or teams, before it shows up</p>
   -->

   Per ulteriori informazioni, consulta [Creazione di assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   Non è possibile effettuare assegnazioni avanzate dai campi Assegnato a o Assegnato.

1. Dopo aver aggiunto gli assegnatari all&#39;attività, premi Invio o fai clic in un punto qualsiasi della pagina per salvare le modifiche se hai selezionato Salvataggio automatico. In caso contrario, fai clic su **Salva**.

## Assegnare più attività a un utente

1. Passare a un elenco delle attività che si desidera assegnare in blocco.
1. (Condizionale) Assicurati che il **Salvataggio automatico** se ti trovi in un elenco di attività di un progetto, l’opzione è selezionata.

   >[!IMPORTANT]
   Non è possibile modificare le attività in blocco quando si salvano le attività manualmente in un progetto.

1. Selezionare diverse attività nell&#39;elenco delle attività.
1. Fai clic su **Modifica**.

   La **Modifica attività** viene visualizzata la finestra di dialogo.

1. In **Assegnazioni** area, selezionare **Assegnatario** quindi iniziare a digitare il nome di un utente, di un ruolo o di un team che si desidera assegnare a tutte le attività.

   >[!IMPORTANT]
   Se una delle attività è già assegnata, le risorse indicate vengono aggiunte alle attività anziché sostituire le risorse esistenti sulle attività.

1. (Facoltativo) Seleziona il pulsante di scelta nel **Proprietario attività** per indicare quale risorsa è l&#39;assegnatario principale o il proprietario dell&#39;attività, quando si assegnano più risorse all&#39;attività. Non disponibile per i team.
1. (Condizionale) Specifica il **% allocazione** per ogni risorsa assegnata all&#39;attività, se tutte le attività selezionate hanno un tipo di durata guidata sforzo o un&#39;assegnazione calcolata. Indica quanto tempo devono trascorrere queste risorse per completare l’attività. Questa opzione è disponibile solo per gli utenti e i ruoli di lavoro.

   Oppure

   Specifica l&#39;importo di **Ore** per ogni risorsa assegnata all&#39;attività, se tutte le attività selezionate sono di tipo Durata semplice. Il totale di tutte le ore per tutte le risorse deve corrispondere al numero di ore pianificate per l&#39;attività.

   >[!IMPORTANT]
   Non è possibile specificare la percentuale di allocazione o il numero di ore per risorsa se le attività selezionate hanno tipi di durata diversi o le attività selezionate hanno tipi di durata diversi.

   Per informazioni sul tipo di durata per le attività, vedere [Panoramica del tipo di durata e durata dell’attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Facoltativo) Seleziona un ruolo che l’utente deve svolgere sull’attività dal **Scegli un ruolo** nel menu a discesa **Ruolo dell&#39;assegnatario** quando si assegnano gli utenti alle attività. Se non selezioni un ruolo, Workfront seleziona automaticamente il ruolo principale dell’utente.

1. (Facoltativo) Se desideri rimuovere gli assegnatari esistenti da tutte le attività, effettua una delle seguenti operazioni:

   1. Inizia a digitare il nome di un utente, un ruolo o un team da rimuovere dall&#39;attività, quindi selezionalo quando viene visualizzato nell&#39;elenco e fai clic su **Rimuovi assegnatario** per rimuovere altri assegnatari.
   1. Fai clic su **Rimuovi tutti gli assegnatari esistenti** per rimuovere tutti gli assegnatari da tutte le attività selezionate.

1. Fai clic su **Salva modifiche**.
1. (Facoltativo e condizionale) Quando i campi Assegnato a o Assegnazioni vengono visualizzati nell’elenco delle attività, fare clic all’interno di una di queste colonne per un’attività, quindi fare clic sul pulsante **Icona X** accanto al nome di un assegnatario per rimuoverlo dall&#39;attività.

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


