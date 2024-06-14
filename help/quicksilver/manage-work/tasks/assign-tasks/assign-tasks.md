---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Assegna attività
description: È possibile assegnare attività a utenti, ruoli o team per indicare chi è responsabile del completamento delle attività. È possibile assegnare un'attività a più risorse contemporaneamente.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 50e52f27f1f3f6f5b601b50303aba409559d8ca8
workflow-type: tm+mt
source-wordcount: '2070'
ht-degree: 1%

---

# Assegna attività

<!--remove the span class preview from everywhere but the Rate Card roles referencs must stay in yellow; replace the intro with preview and fast track only but not sure if with the link to third quarter release?!-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti oppure nell’ambiente di produzione per i clienti che hanno abilitato le versioni rapide.</span>

<span class="preview">Per informazioni sulle versioni rapide, consulta [Abilitare o disabilitare le versioni rapide per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Per informazioni sulla versione corrente, consulta [Panoramica sulla versione del terzo trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

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

Il numero di utenti assegnati a un&#39;attività e la pianificazione del proprietario dell&#39;attività possono modificare le date pianificate di un&#39;attività, modificando la sequenza temporale del progetto. Per informazioni sull&#39;impatto dell&#39;assegnazione di più utenti a un&#39;attività, vedere [Panoramica sulla modifica delle assegnazioni delle attività](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

Oltre a questo articolo, si consiglia di leggere i seguenti articoli per ulteriori informazioni sull&#39;assegnazione delle attività:

* [Panoramica sulla modifica delle assegnazioni delle attività](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [Panoramica delle assegnazioni intelligenti](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Effettua assegnazioni intelligenti](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Crea assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Modificare più assegnazioni utente in un elenco di attività](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Pianificare una panoramica del progetto](../../../manage-work/projects/planning-a-project/plan-project.md)
* [Panoramica della data di completamento pianificata dell&#39;attività](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Impostare la data di completamento pianificata del progetto](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [Panoramica sull’assegnazione del lavoro nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Progetti e Attività</p> <p>Accesso di visualizzazione o superiore agli utenti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Contribuire o accedere ad autorizzazioni superiori per le attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront.

+++

## Considerazioni per più assegnazioni a mansioni, team e utenti

Quando si assegnano più risorse a un elemento di lavoro, tenere presente quanto segue:

* Gli utenti possono avere più di una mansione associata al loro profilo. Per informazioni sull&#39;associazione degli utenti ai ruoli, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Se si assegnano più utenti a un&#39;attività o a un problema, il primo utente selezionato viene automaticamente designato come proprietario dell&#39;attività o del problema.
Per istruzioni su come modificare questa impostazione, vedere le informazioni sull&#39;opzione Imposta come principale nell&#39;articolo [Crea assegnazioni avanzate](create-advanced-assignments.md).

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
   <p>Per informazioni sul ruolo principale di un utente e su altri ruoli, vedi <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Modificare il profilo di un utente</a>.</p>
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
1. Clic **Assegna a** nel **Assegnazioni** campo nell’intestazione dell’attività

   Oppure

   Se l’attività o il problema è già assegnato, fai clic sul nome delle assegnazioni.

   Nell’ambiente di produzione:
   ![](../assign-tasks/assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

   <span class="preview">Nell’ambiente di anteprima:</span>
   ![Assegnazioni](assets/assignments-box-in-task-header.png)

1. Esegui una delle operazioni seguenti:

   * Inizia a digitare il nome di un utente, una mansione o un team che desideri assegnare, quindi fai clic su di esso quando viene visualizzato nell’elenco.


     >[!TIP]
     >
     >Quando aggiungi un’assegnazione utente, osserva l’avatar, il ruolo principale dell’utente o il suo indirizzo e-mail per distinguere gli utenti con nomi identici. Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono aggiunti.
     >
     >Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, consulta [Concedere l’accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     >
     ><span class="preview">Quando si aggiunge un&#39;assegnazione di una mansione, è possibile cercare la mansione o la posizione. Selezionare un ruolo dall&#39;elenco Ruoli per utilizzare la tariffa di fatturazione predefinita per l&#39;assegnazione oppure selezionare un ruolo di ruolo Scheda tariffa per utilizzare la tariffa di fatturazione dalla scheda tariffa. Per ulteriori informazioni sulle schede delle tariffe, consulta [Gestire le schede delle tariffe](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


   * (Condizionale) Fai clic su uno dei nomi nell’ <span class="preview">**Assegnazioni suggerite**, **Utente e team**, o **Ruoli**, o **Valuta ruoli scheda**</span> elenchi quando vengono visualizzati. Per ulteriori informazioni, consulta [Panoramica delle assegnazioni intelligenti](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

     È possibile iniziare a digitare il nome di qualsiasi utente, team o mansione da assegnare all&#39;attività, quindi selezionarlo quando viene visualizzato nell&#39;elenco.

   * Clic **Avanzate**

     Per informazioni su come effettuare assegnazioni avanzate, vedere [Crea assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Fai clic su **Salva**.
1. (Facoltativo e condizionale) Fai clic su **Icona X** accanto al nome dell&#39;assegnazione nel pannello destro dell&#39;attività per rimuovere un&#39;assegnazione, se si fa clic su **Avanzate**.

## Assegnare un&#39;attività in un elenco

È possibile assegnare attività in un elenco o in un report quando uno qualsiasi dei campi delle assegnazioni è visibile nella visualizzazione dell&#39;elenco. Si tratta di un metodo più veloce per assegnare le attività. In questo articolo viene descritto come modificare le assegnazioni di un&#39;attività in un elenco. Per informazioni sulla modifica di più assegnazioni per più attività in un elenco, vedere [Modificare più assegnazioni utente in un elenco di attività](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

A seconda del campo visibile nella visualizzazione, è possibile assegnare le seguenti entità all&#39;attività:

| Campo | Entità assegnate |
|---|---|
| **Assegna a** | Assegna un utente |
| **Assegnato** | Assegna un utente |
| **Assegnazioni** | Assegnare utenti, mansioni o team |

Per assegnare le attività in un elenco:

1. Consente di passare a un elenco di attività contenente i campi Assegnato a, Assegnato o Assegnazioni nella visualizzazione.
1. (Facoltativo) Fai clic su **Salvataggio automatico** e selezionare una delle seguenti opzioni:

   | Opzione | Descrizione opzione |
   |---|---| 
   | Salvataggio automatico | Le modifiche apportate alle attività vengono salvate automaticamente e non è possibile ripristinarle |
   | Salvataggio manuale | È necessario salvare manualmente le modifiche. È possibile ripristinare le modifiche prima di salvarle. |
   | Pianificazione sequenza temporale | È necessario salvare manualmente le modifiche. È possibile ripristinare le modifiche prima di salvarle. Il salvataggio delle modifiche e di tutte le dipendenze del progetto è più rapido rispetto a quando si seleziona Salvataggio manuale. |

   Per ulteriori informazioni sul salvataggio delle attività mentre vengono modificate in un elenco, vedere [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Per assegnare le attività, effettuare una delle seguenti operazioni:

   * Fai clic all’interno del **Assegnato a** o **Assegnato** e iniziare a digitare il nome di un utente attivo che si desidera assegnare all&#39;attività, quindi fare clic su di esso quando viene visualizzato nell&#39;elenco.
   * Fai clic all’interno del **Assegnazioni** e inizia a digitare il nome di un utente attivo, una mansione o un team che desideri assegnare all’attività, quindi fai clic su di esso quando viene visualizzato nell’elenco.

     >[!TIP]
     >
     >Quando aggiungi un’assegnazione utente, osserva l’avatar, il ruolo principale dell’utente o il suo indirizzo e-mail per distinguere gli utenti con nomi identici. Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono aggiunti.
     >
     >Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, consulta [Concedere l’accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
     >
     ><span class="preview">Quando si aggiunge un&#39;assegnazione di una mansione, è possibile cercare la mansione o la posizione. Selezionare la mansione predefinita/di sistema per utilizzare la tariffa di fatturazione predefinita per l&#39;assegnazione oppure selezionare una mansione scheda tariffa per utilizzare la tariffa di fatturazione dalla scheda tariffa. Per ulteriori informazioni sulle schede delle tariffe, consulta [Gestire le schede delle tariffe](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


1. (Condizionale) Quando è visibile in **Assegnazioni** , fare clic sul pulsante **Persone** nell&#39;angolo superiore destro della casella assegnazioni per aprire **Assegnazioni avanzate** e creare assegnazioni avanzate.

   <!--
   there is a People icon in NWE but it's hard to see - you need to assign the task to at least 2 users, not roles, or teams, before it shows up</p>
   -->

   Per ulteriori informazioni, consulta [Crea assegnazioni avanzate](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Non è possibile effettuare assegnazioni avanzate dai campi Assegnato a o Assegnato.

1. Dopo aver aggiunto gli assegnatari all’attività, premi Invio o fai clic in un punto qualsiasi della pagina per salvare le modifiche, se hai selezionato Salvataggio automatico. In caso contrario, fare clic su **Salva**.

## Assegnare più attività a un utente

1. Passare a un elenco di attività che si desidera assegnare in blocco.
1. (Condizionale) Assicurati che il **Salvataggio automatico** L&#39;opzione è selezionata se ci si trova in un elenco di attività di un progetto.

   >[!IMPORTANT]
   >
   >Non è possibile modificare le attività in blocco quando si salvano le attività manualmente in un progetto.

1. Selezionare più attività nell&#39;elenco delle attività.
1. Clic **Modifica**.

   Il **Modifica le Attività** viene visualizzata.

1. In **Assegnazioni** , selezionare la **Assegnatario** , quindi iniziare a digitare il nome di un utente, una mansione o un team che si desidera assegnare a tutte le attività.

   >[!IMPORTANT]
   >
   >Se una delle attività è già assegnata, le risorse indicate in questo campo vengono aggiunte alle attività anziché sostituire le risorse esistenti sulle attività.

1. (Facoltativo) Seleziona il pulsante di opzione nella **Proprietario attività** per indicare quale risorsa è l&#39;assegnatario principale o il proprietario dell&#39;attività, quando si assegnano più risorse all&#39;attività. Questa funzione non è disponibile per i team.
1. (Condizionale) Specifica la **% allocazione** per ogni risorsa assegnata all&#39;attività se tutte le attività selezionate hanno un Tipo di durata di Impegno o Assegnazione calcolata. Indica quanto tempo queste risorse devono dedicare al completamento dell&#39;attività. Questa opzione è disponibile solo per gli utenti e le mansioni.

   Oppure

   Specifica la quantità di **Ore** per ogni risorsa assegnata all&#39;attività se tutte le attività selezionate hanno un Tipo di durata semplice. Il totale di tutte le ore per tutte le risorse deve corrispondere al numero di ore pianificate per l&#39;attività.

   >[!IMPORTANT]
   >
   >Non è possibile specificare la percentuale di allocazione o il numero di ore per risorsa se le attività selezionate hanno tipi di durata diversi o se le attività selezionate hanno tipi di durata diversi.

   Per informazioni sul Tipo di Durata per le attività, vedi [Panoramica sulla durata e sul tipo di durata dell&#39;attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Facoltativo) Seleziona un ruolo che l’utente deve svolgere sull’attività dall’elenco **Scegli una mansione** menu a discesa nella **Ruolo dell&#39;assegnatario** quando si assegnano gli utenti alle attività. Se non si seleziona un ruolo, Workfront seleziona automaticamente il ruolo principale dell&#39;utente.

1. (Facoltativo) Se si desidera rimuovere assegnatari esistenti da tutte le attività, effettuare una delle seguenti operazioni:

   1. Inizia a digitare il nome di un utente, ruolo o team che desideri rimuovere dall’attività, quindi selezionalo quando viene visualizzato nell’elenco e fai clic su **Rimuovi assegnatario** per rimuovere altri assegnatari.
   1. Clic **Rimuovi tutti gli assegnatari esistenti** per rimuovere tutti gli assegnatari da tutte le attività selezionate.

1. Fai clic su **Salva modifiche**.
1. (Facoltativo e condizionale) Quando nell&#39;elenco delle attività vengono visualizzati i campi Assegnato a o Assegnazioni, fare clic in una di queste colonne per un&#39;attività, quindi fare clic su **Icona X** accanto al nome di un assegnatario per rimuoverlo dall&#39;attività.

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


