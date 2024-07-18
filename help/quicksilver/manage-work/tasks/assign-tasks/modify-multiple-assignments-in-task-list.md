---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Modificare più assegnazioni utente in un elenco di attività
description: Quando si gestiscono le assegnazioni di attività, è possibile modificarle contemporaneamente per più attività contemporaneamente utilizzando la funzione di modifica in blocco in un elenco di attività.
author: Alina
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 070b0525f0cb2880d3c7daf88777ba48968ce759
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Modificare più assegnazioni utente in un elenco di attività

<!--Audited: 07/2024-->

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

Quando si gestiscono le assegnazioni di attività, è possibile modificarle contemporaneamente per più attività contemporaneamente utilizzando la funzione di modifica in blocco in un elenco di attività.

Questo articolo fa riferimento alla modifica di più assegnazioni utente per più attività in un elenco di attività. Vedere anche i seguenti articoli per la modifica di assegnazioni su più attività in altre aree:

* Per informazioni sull&#39;assegnazione di attività tramite il Bilanciatore dei carichi di lavoro, vedere [Panoramica sull&#39;assegnazione di lavoro nel Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Per informazioni sull&#39;assegnazione di un&#39;attività a una risorsa di un elenco, vedere [Assegnare attività](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuovo: Standard</p>
   <p>Corrente: Lavoro o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Progetti e Attività</p> <p>Accesso di visualizzazione o superiore agli utenti</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Contribute o autorizzazioni superiori per le attività</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration&nbsp;Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration&nbsp;Types:</p>
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

1. Seleziona le attività per le quali vuoi modificare le assegnazioni, quindi fai clic sull&#39;icona **Modifica** ![](assets/edit-icon.png).

   Viene visualizzata la pagina Modifica attività. Gli elementi modificati vengono visualizzati nell&#39;angolo superiore sinistro della pagina.

1. Vai alla sezione **Assegnazioni**.
1. Per aggiungere o rimuovere assegnatari, effettuare una delle seguenti operazioni:

   >[!IMPORTANT]
   >
   >La rimozione degli assegnatari può influire sulle ore delle attività e sulle percentuali di allocazione. Per ulteriori informazioni, vedere la sezione [Come la rimozione degli assegnatari influisce sulle ore delle attività e sulle percentuali di allocazione](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in questo articolo.

   * Per aggiungere un nuovo assegnatario:

      1. Nella sezione **Assegnazioni**, seleziona **Assegnatario**.

         Vengono visualizzate le informazioni comuni a tutte le attività selezionate. Ad esempio, se lo stesso utente viene assegnato a tutte le attività, viene visualizzato nella colonna **Assegnatario**. Se le informazioni non sono comuni tra le attività selezionate, non vengono visualizzate.

      1. Inizia a digitare il nome di un utente, ruolo o team, quindi selezionalo quando viene visualizzato nell’elenco. L&#39;assegnazione viene aggiunta e non sostituisce le assegnazioni correnti sulle attività selezionate.


     >[!TIP]
     >
     > * Puoi assegnare più utenti, mansioni o team. Puoi assegnare solo utenti attivi, mansioni e team.
     >   
     > * Quando aggiungi un’assegnazione utente, osserva l’avatar, il ruolo principale dell’utente o il suo indirizzo e-mail per distinguere gli utenti con nomi identici. Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono aggiunti. Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, vedere [Concedere l&#39;accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     > 
     >   Se un utente, una mansione o un team è stato assegnato prima della disattivazione, rimane assegnato all&#39;elemento di lavoro. In questo caso, consigliamo quanto segue:
     >   
     >     * Riassegnare l&#39;elemento di lavoro alle risorse attive.
     >     * Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.


   * Per rimuovere singoli assegnatari:

      1. Fare clic sull&#39;icona **X** accanto al nome dell&#39;assegnatario che si desidera rimuovere se l&#39;assegnatario viene visualizzato nell&#39;elenco Assegnazioni.

         Oppure

         (Condizionale) Se l&#39;assegnatario che si desidera rimuovere non viene visualizzato nella sezione Assegnazioni perché l&#39;assegnatario è assegnato solo ad alcune delle attività selezionate, fare clic su **Rimuovi assegnatario** e iniziare a digitare il nome dell&#39;assegnatario che si desidera rimuovere, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   * Per rimuovere tutti gli assegnatari:

      1. Fai clic su **Rimuovi tutti gli assegnatari esistenti**, quindi fai clic su **Sì, elimina tutti gli assegnatari**.

         In questo modo vengono rimossi non solo gli assegnatari comuni (assegnatari visualizzati nella finestra di dialogo di modifica), ma anche tutti gli assegnatari di tutte le attività selezionate.

     La rimozione degli utenti dalle attività può influire sulle ore delle attività e sulle percentuali di allocazione.

     Per ulteriori informazioni, vedere [Panoramica sulla modifica delle assegnazioni di attività](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

1. (Facoltativo) Modifica una delle seguenti opzioni per gli assegnatari:

   * (Condizionale) **% allocazione o ore**: specificare una nuova percentuale di allocazione o ore.

     >[!NOTE]
     >
     >Questa opzione può essere modificata solo se il Tipo di Durata è lo stesso in tutte le attività che vengono modificate. Quando il tipo di durata è Lavoro calcolato o Basato sulle risorse, è possibile aggiornare la percentuale di allocazione. Quando il Tipo di Durata è Semplice, è possibile aggiornare le Ore. Per informazioni sul tipo di durata, vedere [Panoramica sulla durata dell&#39;attività e sul tipo di durata](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
     >
     >
     >Se il campo è vuoto, significa che il valore è diverso tra le varie attività, ma è comunque possibile modificarlo.

   * **Proprietario attività**: selezionare questa opzione per fare dell&#39;assegnatario il proprietario dell&#39;attività per tutte le attività da modificare.
   * **Ruolo assegnatario**: selezionare un ruolo dall&#39;elenco a discesa. Se non è selezionata, Adobe Workfront seleziona automaticamente il Ruolo principale dell’utente.

1. Fai clic su **Salva modifiche.**
