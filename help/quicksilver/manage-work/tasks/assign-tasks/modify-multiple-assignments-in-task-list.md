---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Modificare più assegnazioni utente in un elenco di attività
description: Quando si gestiscono le assegnazioni di attività, è possibile modificarle contemporaneamente per più attività alla volta utilizzando la funzione di modifica collettiva in un elenco di attività.
author: Alina
feature: Work Management
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 0%

---

# Modificare più assegnazioni utente in un elenco di attività

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

Quando si gestiscono le assegnazioni di attività, è possibile modificarle contemporaneamente per più attività alla volta utilizzando la funzione di modifica collettiva in un elenco di attività.

Questo articolo fa riferimento alla modifica di più assegnazioni utente per più attività in un elenco di attività. Vedere anche gli articoli seguenti per modificare le assegnazioni su più attività in altre aree:

* Per informazioni sull&#39;assegnazione di attività tramite il servizio di bilanciamento del carico di lavoro, consulta [Panoramica dell’assegnazione del lavoro nel servizio di bilanciamento del carico di lavoro](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Per informazioni sull&#39;assegnazione di un&#39;attività a una risorsa in un elenco, consulta [Assegnare le attività](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Requisiti di accesso

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
   <td> <p>Modifica accesso a progetti e attività</p> <p>Visualizza o accesso più elevato agli utenti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Collaborare o autorizzazioni superiori per le attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

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

## Modificare le assegnazioni per più attività

1. Passare all&#39;elenco contenente le attività in cui si desidera modificare le assegnazioni.
1. (Facoltativo) Crea un filtro per visualizzare solo le attività assegnate all’assegnatario che desideri modificare.

   Ad esempio, se il progetto contiene un ruolo specifico come assegnatario predefinito per più attività, è possibile creare un filtro per visualizzare solo le attività con tale ruolo come assegnatario. Quindi, puoi sostituire il ruolo con un utente specifico.

   Per informazioni sulla creazione di un filtro, consulta [Creare o modificare filtri](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. Per filtrare un ruolo, seleziona **Ruoli assegnazione**, quindi fai clic su **ID**.

   >[!TIP]
   >
   >Non utilizzare il **Assegnato a** campo . In questo modo viene trovato solo il proprietario principale dell&#39;attività, anziché uno dei ruoli che è possibile assegnare loro.

   Oppure

   Per filtrare un utente, seleziona **Utenti assegnazione,** quindi fai clic su **ID.**

   >[!TIP]
   >
   >Non utilizzare il **Assegnato a** campo . In questo modo viene trovato solo il proprietario principale per l&#39;attività, anziché uno degli utenti che possono essere assegnati loro.

1. Selezionare le attività per le quali si desidera modificare le assegnazioni, quindi fare clic sul pulsante **Modifica** icona ![](assets/edit-icon.png).

   Viene visualizzata la pagina Modifica attività . Gli elementi modificati vengono visualizzati nell’angolo in alto a sinistra della pagina.

1. Vai a **Assegnazioni** sezione .
1. Per aggiungere o rimuovere gli assegnatari, effettuare una delle seguenti operazioni:

   >[!IMPORTANT]
   >
   >La rimozione degli assegnatari può influenzare le ore di attività e le percentuali di allocazione. Per ulteriori informazioni, consulta la sezione . [La rimozione degli assegnatari influisce sulle ore delle attività e sulle percentuali di allocazione](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in questo articolo.

   * Per aggiungere un nuovo assegnatario:

      1. In **Assegnazioni** sezione , seleziona **Assegnatario**.

         Vengono visualizzate le informazioni comuni a tutte le attività selezionate. Ad esempio, se lo stesso utente viene assegnato a tutte le attività, viene visualizzato nel **Assegnatario** colonna. Se le informazioni non sono comuni tra le attività selezionate, non vengono visualizzate informazioni.

      1. Inizia a digitare il nome di un utente, un ruolo o un team, quindi selezionalo quando viene visualizzato nell’elenco. L&#39;assegnazione viene aggiunta e non sostituisce le assegnazioni correnti nelle attività selezionate.
      >[!TIP]
      >
      > * È possibile assegnare più utenti, ruoli o team. È possibile assegnare solo utenti attivi, ruoli e team.
      >   
      > * Quando aggiungi un&#39;assegnazione utente, osserva l&#39;avatar, il ruolo principale dell&#39;utente o il relativo indirizzo e-mail per distinguere tra utenti con nomi identici. Gli utenti devono essere associati ad almeno un ruolo di lavoro per visualizzarlo durante l&#39;aggiunta.

         > 
         >   Se un utente, un ruolo di lavoro o un team è stato assegnato prima della disattivazione, rimangono assegnati all&#39;elemento di lavoro. In questo caso, si consiglia quanto segue:
         >   
         >     * Riassegna l&#39;elemento di lavoro alle risorse attive.
         >     * Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.



   * Per rimuovere singoli assegnatari:

      1. Fai clic sul pulsante **Icona X** accanto al nome dell&#39;assegnatario che si desidera rimuovere se l&#39;assegnatario viene visualizzato nell&#39;elenco Assegnazioni.

         Oppure

         (Condizionale) Se l&#39;assegnatario che si desidera rimuovere non viene visualizzato nella sezione Assegnazioni in quanto l&#39;assegnatario è assegnato solo ad alcune delle attività selezionate, fare clic su **Rimuovi assegnatario** e iniziare a digitare il nome dell&#39;assegnatario che si desidera rimuovere, quindi fare clic sul nome quando viene visualizzato nell&#39;elenco a discesa.
   * Per rimuovere tutti gli assegnatari esistenti:

      1. Fai clic su **Rimuovi tutti gli assegnatari esistenti**, quindi fai clic su **Sì, Elimina tutti gli assegnatari**.

         Questo rimuove non solo gli assegnatari comuni (assegnatari visualizzati nella finestra di dialogo di modifica), ma anche tutti gli assegnatari su tutte le attività selezionate.
      La rimozione degli utenti dalle attività può influire sulle ore delle attività e sulle percentuali di allocazione.

      Per ulteriori informazioni, consulta [Panoramica sulla modifica delle assegnazioni di attività](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).





1. (Facoltativo) Modifica una delle seguenti opzioni per gli assegnatari:

   * (Condizionale) **% o ore di allocazione**: Specificare una nuova percentuale o ore di allocazione.

      >[!NOTE]
      >
      >Questa opzione può essere modificata solo se il Tipo di durata è lo stesso per tutte le attività in corso di modifica. Quando il tipo di durata è Lavoro calcolato o Basato su sforzo è possibile aggiornare la percentuale di allocazione. Quando il tipo di durata è semplice, puoi aggiornare le ore. Per informazioni sul tipo di durata, consulta [Panoramica del tipo di durata e durata dell’attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
      Se il campo è vuoto, significa che il valore è diverso tra le attività; tuttavia, puoi comunque modificarlo.

   * **Proprietario attività**: Selezionare questa opzione per rendere l&#39;assegnatario proprietario dell&#39;attività per tutte le attività in corso di modifica.
   * **Ruolo dell&#39;assegnatario**: Seleziona un ruolo dall’elenco a discesa. Se non è selezionato, Adobe Workfront seleziona automaticamente il Ruolo principale dell’utente.

1. Fai clic su **Salva le modifiche.**
