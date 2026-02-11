---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Modificare più assegnazioni utente in un elenco attività
description: Quando si gestiscono le assegnazioni di attività, è possibile modificarle contemporaneamente per più attività contemporaneamente utilizzando la funzione di modifica in blocco in un elenco di attività.
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 21c98e443a6d6ca79045e2f4aba5f792340833cd
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 3%

---

# Modificare più assegnazioni utente in un elenco di attività

<!--Audited: 11/2025-->

<!--remove the old/new experience references when the toggles are removed-->

<!--
this article is similar and updates on this one might need to be repeated here: help/quicksilver/manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Second Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md).  

</div>-->

Quando si gestiscono le assegnazioni di attività, è possibile modificarle contemporaneamente per più attività contemporaneamente utilizzando la funzione di modifica in blocco in un elenco di attività.

Questo articolo fa riferimento alla modifica di più assegnazioni utente per più attività in un elenco di attività. Vedere anche i seguenti articoli per la modifica di assegnazioni su più attività in altre aree:

* Per informazioni sull&#39;assegnazione di attività tramite il Bilanciatore dei carichi di lavoro, vedere [Panoramica sull&#39;assegnazione di lavoro nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Per informazioni sull&#39;assegnazione di un&#39;attività a una risorsa di un elenco, vedere [Assegnare attività](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Work o successiva</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Progetti e Attività</p> <p>Accesso di visualizzazione o superiore agli utenti</p> </td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni oggetto</td>
   <td>Contribuire o accedere ad autorizzazioni superiori per le attività</td>
  </tr>
 </tbody>
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on tasks</h2>
<p>(NOTE: moved to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>You might want to modify the user assignments for multiple tasks for a variety of reasons, including the following:</p>
<ul>
<li>Users join or leave your team</li>
<li> <p>A user takes a vacation that extends beyond task due dates</p> <note type="note">
When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li>A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
<p><strong>How removing assignees affects task hours and allocation percentages</strong></p>
<p>(NOTE: move to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration Types:</p>
<ul>
<li> <p><strong>Simple:</strong> The planned hours assigned to that user are subtracted from the task's total planned hours.</p> <note type="important">
<span class="s1">This could negatively affect your project plan because it changes the total planned hours for the task and the project.</span>
</note> </li>
<li><span class="s1"><strong>Effort Driven:</strong> The allocation percentage does not change for other users.</span> </li>
<li><span class="s1"><strong>Calculated Assignment:</strong> The allocation percentages of other users are adjusted so that the total equals 100%.</span> </li>
<li><span class="s1"><strong>Calculated Work:</strong> The allocation percentage does not change for other users.</span> </li>
</ul>
</div>
-->

## Modifica assegnazioni per più attività

1. Passare all&#39;elenco contenente le attività in cui si desidera modificare le assegnazioni.
1. (Facoltativo) Crea un filtro per visualizzare solo le attività assegnate all’assegnatario che desideri modificare.

   Ad esempio, se il progetto contiene un ruolo specifico come assegnatario predefinito per più attività, è possibile creare un filtro per visualizzare solo le attività con tale ruolo come assegnatario. Quindi, puoi sostituire il ruolo con un utente specifico.

   Per informazioni sulla creazione di un filtro, vedere [Creare o modificare filtri](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. Per filtrare in base a un ruolo, seleziona **Ruoli di assegnazione**, quindi fai clic su **ID**.

   >[!TIP]
   >
   >Non utilizzare il campo **Assegnato a**. In questo modo viene trovato solo il Proprietario principale dell&#39;attività anziché i ruoli che potrebbero essere assegnati.

   Oppure

   Per filtrare un utente, seleziona **Utenti assegnazione,** quindi fai clic su **ID.**

   >[!TIP]
   >
   >Non utilizzare il campo **Assegnato a**. In questo modo viene trovato solo il proprietario principale dell&#39;attività e non gli utenti che potrebbero essere assegnati.

1. Seleziona le attività per le quali vuoi modificare le assegnazioni, quindi fai clic sull&#39;icona **Modifica** ![Modifica icona](assets/edit-icon.png).

   1. Per aggiungere o rimuovere assegnatari, effettuare una delle seguenti operazioni:

      * Per aggiungere gli assegnatari, inizia a digitare il nome di un assegnatario nel campo **Cerca persone, ruoli o team**, quindi selezionali quando vengono visualizzati nell&#39;elenco.

        Il nuovo assegnatario viene aggiunto a quelli esistenti per le attività selezionate.
      * Per rimuovere gli assegnatari, fare clic sul nome di un assegnatario nella casella **Rimuovi assegnatario**

        Oppure

        Fare clic su **Rimuovi tutti gli assegnatari esistenti**.

        Gli assegnatari vengono rimossi da tutte le attività selezionate.

        La rimozione degli utenti dalle attività può influire sulle ore delle attività e sulle percentuali di allocazione.

        Per ulteriori informazioni, vedere [Panoramica sulla modifica delle assegnazioni di attività](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).


        >[!TIP]
        >
        >* Puoi assegnare più utenti, mansioni o team. Puoi assegnare solo utenti attivi, mansioni e team.
        >   
        >* Quando aggiungi un’assegnazione utente, osserva l’avatar, il ruolo principale dell’utente o il suo indirizzo e-mail per distinguere gli utenti con nomi identici. Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono aggiunti. Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, vedere [Concedere l&#39;accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
        > 
        >   Se un utente, una mansione o un team è stato assegnato prima della disattivazione, rimane assegnato all&#39;elemento di lavoro. In questo caso, consigliamo quanto segue:
        >   
        >* Riassegnare l&#39;elemento di lavoro alle risorse attive.
        >* Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.


   1. (Facoltativo) Modifica una delle seguenti opzioni per gli assegnatari:

      * (Condizionale) **% allocazione o ore**: specificare una nuova percentuale di allocazione o ore.

      >[!NOTE]
      >
      >Questa opzione può essere modificata solo se il Tipo di Durata è lo stesso in tutte le attività che vengono modificate. Quando il tipo di durata è Lavoro calcolato o Basato sulle risorse, è possibile aggiornare la percentuale di allocazione. Quando il Tipo di Durata è Semplice, è possibile aggiornare le Ore. Per informazioni sul tipo di durata, vedere [Panoramica sulla durata dell&#39;attività e sul tipo di durata](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
      >
      >
      >Se il campo è vuoto, significa che il valore è diverso tra le varie attività, ma è comunque possibile modificarlo.

      * **Imposta come principale**: passa il puntatore del mouse sulle attività selezionate e seleziona questa opzione per fare dell&#39;assegnatario il proprietario dell&#39;attività per tutte le attività modificate.
      * **Ruolo assegnatario**: selezionare un ruolo dall&#39;elenco a discesa. Se non è selezionata, Adobe Workfront seleziona automaticamente il Ruolo principale dell’utente.
      * **Tipo di Durata**
      * **Durata**
      * **Ore pianificate**

   1. Fai clic su **Salva**.

<!-- temporary content - for Assignments redesign:

Editing assignments on tasks differs depending on which environment you choose. 

1. (Conditional) If you are using the Production environment to assign tasks, the **Edit Tasks** box opens in the new experience. Do the following in the Production environment: 

   1. To add or remove assignees, do one of the following:

      * To add assignees, start typing the name of an assignee in the **Search people, roles, or teams** field, then select them when they display in the list. 
      * To remove assignees, click the **x** icon to the right of their name. Only assignees that are common to all tasks display in the list. 
      * Click Assign to me to assign the selected tasks to yourself.

   1. (Conditional) When using the new experience, click **Save**.

   1. (Optional) Click **Switch to old experience** at the bottom of the **Edit Tasks** box.
      
      The **Edit Tasks** box opens in the old experience.

   1. (Conditional) In the old experience, do the following to modify the assignees:

      1. Go to the **Assignments** section.

         >[!IMPORTANT]
         >
         >Removing assignees can affect the task hours and allocation percentages. For more information, see the section [How removing assignees affects task hours and allocation percentages](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in this article.

      1. Do one of the following to add or remove assignees:

         * To add a new assignee:

            1. In the **Assignments** section, select **Assignee**.

               Information that is common across all tasks selected displays. For example, if the same user is assigned to all tasks, that user displays in the **Assignee** column. If information is not common across the tasks selected, no information displays.
            
            1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected tasks.

            >[!TIP]
            >
            > * You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
            >   
            > * When adding a user assignment, notice the avatar, the user's Primary Role, or their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them. You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
            > 
            >   If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
            >   
            >     * Reassign the work item to active resources.
            >     * Associate the users in a deactivated team with an active team and reassign the work item to the active team.


         * To remove individual assignees:

            1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.

               Or

               (Conditional) If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the tasks that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.

         * To remove all existing assignees:

            1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.

               This removes not only common assignees (assignees that are displayed in the edit dialog box), but also all assignees on all the selected tasks.

            Removing users from tasks can affect task hours and allocation percentages.
            
            For more information, see [Overview of modifying task assignments](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

      1. (Optional) Modify any of the following options for assignees:

         * (Conditional) **Allocation % or Hours**: Specify a new allocation percentage or hours.

         >[!NOTE]
         >
         >This option can be modified only if the Duration Type is the same across all tasks that are being edited. When the Duration Type is Calculated Work or Effort Driven you can update the Allocation %. When the Duration Type is Simple you can update the Hours. For information about Duration Type, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
         >
         >
         >If the field is blank, this means that the value is different across tasks; however, you are still able to modify it.

         * **Task Owner**: Select this option to make the assignee the owner of the task for all tasks being edited.
         * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Adobe Workfront automatically selects the Primary Role of the user. 

      1. Click **Save Changes.**
        

1. <span class="preview">(Conditional) If you are using the Preview environment to assign tasks, the **Edit Tasks** box opens. Do the following in the Preview environment: </span>

   <div class="preview">-->





