---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Panoramica sull’assegnazione del lavoro nel Bilanciatore dei carichi di lavoro
description: In qualità di responsabile delle risorse, puoi utilizzare il Bilanciatore dei carichi di lavoro di Adobe Workfront per visualizzare gli elementi di lavoro non ancora assegnati agli utenti e assegnare loro tali elementi.
author: Lisa
feature: Resource Management
exl-id: 98779b67-b975-4501-8426-63e255b1d7df
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '1033'
ht-degree: 1%

---

# Panoramica sull’assegnazione del lavoro nel Bilanciatore dei carichi di lavoro

In qualità di responsabile delle risorse, puoi utilizzare il Bilanciatore dei carichi di lavoro di Adobe Workfront per visualizzare gli elementi di lavoro non ancora assegnati agli utenti e assegnare loro tali elementi.

Per informazioni generali sul Bilanciatore dei carichi di lavoro, consulta [Panoramica sul Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

È possibile assegnare elementi di lavoro (attività e problemi) a utenti in altre aree di Workfront. Tuttavia, utilizzando il Bilanciatore dei carichi di lavoro è possibile comprendere facilmente la disponibilità degli utenti e vedere chiaramente tutti gli altri elementi a cui sono assegnati prima di assegnare loro più lavoro.

Per informazioni sull&#39;assegnazione di elementi di lavoro in altre aree di Workfront, vedere gli articoli seguenti:

* [Assegna attività](../../manage-work/tasks/assign-tasks/assign-tasks.md)
* [Assegna problemi](../../manage-work/issues/manage-issues/assign-issues.md)

## Disponibilità utente nel Bilanciatore dei carichi di lavoro

Puoi assegnare il lavoro nel Bilanciatore dei carichi di lavoro in modo che corrisponda al tempo disponibile degli utenti. Per assicurarsi di assegnare la giusta quantità di lavoro e non sovrassegnare l&#39;utente, il totale delle ore pianificate degli elementi di lavoro assegnati all&#39;utente deve corrispondere alle allocazioni giornaliere o settimanali dell&#39;utente.

È necessario comprendere in che modo Workfront calcola il tempo disponibile per un utente.

Workfront utilizza le seguenti informazioni per calcolare la capacità dell’utente nel Bilanciatore dei carichi di lavoro:

* Le Preferenze Di Gestione Risorse. L&#39;amministratore di Workfront determina il modo in cui viene calcolato il tempo disponibile per il sistema selezionando l&#39;opzione per utilizzare una delle opzioni seguenti nell&#39;area Gestione risorse in Configurazione:

   * La pianificazione predefinita del sistema Workfront e l&#39;FTE dell&#39;utente.
   * La pianificazione dell’utente, come indicato nell’area Profilo utente.

     In questo modo viene calcolata la disponibilità giornaliera e settimanale dell’utente. Eventuali eccezioni alla pianificazione selezionate si riflettono nella capacità dell’utente nel Bilanciatore dei carichi di lavoro.

  Per ulteriori informazioni, vedere [Configurare le preferenze di Gestione risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  Per informazioni sulle pianificazioni, vedere [Creare una pianificazione](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

* Indisponibilità dell&#39;utente. Indica i giorni previsti per il decollo dell&#39;utente.

  Per ulteriori informazioni, vedere [Configurare l&#39;indisponibilità personale](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* Il tempo di lavoro dell’utente. Indica la percentuale di tempo FTE che l&#39;utente è disponibile per eseguire il lavoro effettivo relativo al progetto, esclusi i costi comuni. Impostare il valore Tempo di lavoro su 1 per indicare che l&#39;utente è disponibile per il lavoro correlato al progetto per l&#39;intero equivalente a tempo pieno.


## Assegnare il lavoro nel Bilanciatore del carico di lavoro

È possibile assegnare elementi di lavoro non ancora assegnati a un utente o riassegnare elementi assegnati a utenti nel Bilanciatore dei carichi di lavoro.

È possibile assegnare il lavoro nel Bilanciatore dei carichi di lavoro nei modi seguenti:

* Un elemento alla volta assegnando manualmente ogni elemento.

  È possibile effettuare assegnazioni avanzate quando si assegnano gli elementi manualmente, uno alla volta.

  Per ulteriori informazioni, consulta [Assegnare il lavoro manualmente utilizzando il Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

* Un elemento alla volta, trascinando e rilasciando gli elementi di lavoro all&#39;utente che deve essere assegnato.

  Per ulteriori informazioni, consulta [Assegnare il lavoro nel Bilanciatore dei carichi di lavoro trascinandolo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md).

* Più elementi alla volta, utilizzando l&#39;opzione Assegnazioni in blocco. È possibile definire regole in base alle quali gli elementi vengono assegnati a più utenti alla volta.

  Per ulteriori informazioni, consulta [Assegnare il lavoro in blocco utilizzando il Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

Per informazioni sulla rimozione dell&#39;assegnazione del lavoro, vedere [Annullamento dell&#39;assegnazione del lavoro nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

## Aree di assegnazione nel Bilanciatore dei carichi di lavoro

È possibile assegnare il lavoro agli utenti utilizzando il Bilanciatore dei carichi di lavoro nell&#39;area Risorse, a livello di progetto o di team. Per ulteriori informazioni sulla posizione del Bilanciatore dei carichi di lavoro in Workfront, vedere [Individuare il Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

Nel Bilanciatore dei carichi di lavoro sono disponibili due aree in cui è possibile visualizzare gli elementi di lavoro:

* **Lavoro non assegnato**: visualizza gli elementi non assegnati agli utenti.
* **Lavoro assegnato**: visualizza gli elementi assegnati agli utenti.

Nella tabella seguente vengono descritti gli elementi da visualizzare in ogni area in base alle relative assegnazioni:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Tipo di assegnazione</strong> </td> 
   <td colspan="2"><strong>Aree in cui sono visibili le assegnazioni</strong> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td>Lavoro Non Assegnato </td> 
   <td>Lavoro non assegnato </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span style="font-weight: normal;">Elemento non assegnato</span> </td> 
   <td><span>✔</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span data-mc-edit-date="2020-04-08T15:57:40.7175506-04:00" data-mc-editor="alinawilson" data-mc-comment="Drafted because role only is not displayed; first it will be displayed in Unassigned - 20.2 beta" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:24:04.5189150-05:00">Ruolo</span> </td> 
   <td><span>✔</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ruolo e team</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Utente e team</td> 
   <td> <p> </p> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Utente, Ruolo e Team</td> 
   <td>✔*</td> 
   <td>✔**</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Utente e Ruolo</p> </td> 
   <td><span data-mc-edit-date="2019-11-15T13:37:42.5435254-05:00" data-mc-editor="alinawilson" data-mc-comment="drafted because it's not in the Unassigned" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:37:33.3097484-05:00">✔</span>*</td> 
   <td>✔**</td> 
  </tr> 
 </tbody> 
</table>

&#42;Quando un elemento di lavoro viene assegnato a un utente e a un ruolo, viene visualizzato nell&#39;area Lavoro non assegnato solo quando il ruolo è l&#39;assegnatario principale.

&#42;&#42;Quando un elemento di lavoro viene assegnato a un utente e a un&#39;altra entità, viene visualizzato nell&#39;area Lavoro assegnato solo quando l&#39;utente è l&#39;assegnatario principale.

Per ulteriori informazioni sulle aree Non assegnato e Assegnato del Bilanciatore dei carichi di lavoro, vedi [Navigare nel Bilanciatore dei carichi di lavoro](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Considerazioni per più assegnazioni a mansioni, team e utenti

Quando si assegnano più risorse a un elemento di lavoro, tenere presente quanto segue:

* Gli utenti possono avere più di una mansione associata al loro profilo. Per informazioni sull&#39;associazione degli utenti alle mansioni, vedere [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Le attività o i problemi vengono in genere prima assegnati a una o più mansioni o a un team. Quando i progetti sono pronti per essere avviati, potrebbe essere necessario assegnarli anche agli utenti.\
  Se un’attività o un problema è assegnato a uno o più ruoli e successivamente si assegna anche un utente, Adobe Workfront decide quale ruolo associare all’utente aggiuntivo (se presente) in base alle seguenti regole:

   * Se è stata assegnata una sola mansione e questa corrisponde alla mansione principale dell’utente, l’attività o il problema viene assegnato solo all’utente che svolge la sua mansione principale.
   * Se sono stati assegnati più ruoli e almeno uno dei ruoli corrisponde ai ruoli secondari dell’utente, l’attività o il problema viene assegnato all’utente che svolge uno dei suoi Altri ruoli, che Workfront seleziona in modo casuale in caso di più corrispondenze, nonché a eventuali ruoli aggiuntivi assegnati.
   * Se sono state assegnate una o più mansioni e non vi sono corrispondenze ai ruoli dell’utente, l’attività o il problema viene assegnato sia al ruolo o alle mansioni che all’utente.

* Se un’attività o un problema è assegnato a un team e si assegna anche un utente, l’attività o il problema rimane assegnato sia al team che all’utente.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2 data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Manually assign one item at a time</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Moved manual assignment and drag-and-drop to their own articles) </p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items</p> <p>Or</p> <p>Go to the <strong>Assigned Work</strong> area and expand the name of a user to view the work items assigned to them.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area. You can only reassign issues already assigned to users in the Assigned Work area. Otherwise,</span> you can assign issues from a list or at the issue level. For information, see
<a href="../../manage-work/issues/manage-issues/assign-issues.md" class="MCXref xref">Assign issues</a>.
</note> </li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> on the bar of a work item, then click <strong>Assign this to</strong>. </p> <p> <img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"> </p> <note type="tip">
<p><span>You can also use the following shortcuts to assign tasks or issues:</span> </p>
<ul>
<li><span>In Windows: CTRL+click the task or issue bar.</span> </li>
<li><span>In&nbsp;Mac: CMD+click the task or issue bar.</span> </li>
</ul>
</note> </li>
<li value="4"> <p>Start typing the name of a user, job role, or team that you want to assign to the item in the <strong>Search people, role or teams</strong> field, select it when it displays in the list, then click&nbsp;<strong>Save</strong>. </p> <p> <img src="assets/assignments-box-wb.png"> </p> <p>This assigns or reassigns the work item to the specified assignees.</p> <p>If you assign an item to just a team or a job role, the item displays only in the Unassigned Work area. You must assign work items to users in order to display them in the Assigned Work area of the Workload Balancer.</p> <note type="tip">
<p>You can assign multiple users or job roles, and you can assign only one team. <span>You can assign only active users, <span>job roles</span>, and teams.</span></p>
<p><span>If a user, <span>job role</span>, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:</span> </p>
<ul>
<li> <p><span>Reassign the work item to active resources.</span> </p> </li>
<li> <p><span>Associate the users in a deactivated team with an active team and reassign the work item to the active team.</span> </p> </li>
</ul>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>.</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2>Assign an item by dragging and dropping</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider retitling this to "Assign one item at a time by dragging and dropping" when bulk assignments will come???)&nbsp;</p>
<p>You can assign an item from the Unassigned Work area to a user, or you can reassign an already assigned item to another user in the Assigned Work area.</p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area.</span>
</note> </li>
<li value="3"> <p>Click the bar of a work item that indicates either the planned or the projected timeline and drag it over the name of a user in the <strong>Assigned</strong> area.</p> <p>The user you hover over to drop the work item to is highlighted.</p> <note type="tip">
The Planned Hours for the user you're hovering over update in real time with the number of daily Planned Hours from the work item, to indicate what the impact of adding a new item might be to their overall allocation.
</note> <p> <img src="assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png" style="width: 350;height: 152;"> </p> </li>
<li value="4"> <p>When you are ready, drop the selected work item in the same line as the user's name in the Assigned Area. The item is assigned and the allocated Planned Hours are updated for the user with the new hours from the work item.</p> <note type="tip">
<p>If you enabled Group by Project in the Settings area, the assigned task displays under the corresponding project. If the setting is disabled, the assigned task displays in the user area. </p>
<p>The item displays according to the Workload Balancer criteria for sorting work items.&nbsp;For more information, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>. (NOTE: make sure these are still called this, and that the icon has not changed)</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol> 
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Assign items in bulk</h2>
<p>(NOTE: This is also a separate article. Should we keep this section or the separate article?) </p>
</div>
<p>&nbsp;</p>
</div>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Unassign work items in the Workload Balancer</h2>
<p>(NOTE: moved this section to a new article. Draft here at release to preview) </p>
<p>You can either unassign items from users and move them to the Unassigned Work area, or reassign them to other users. </p>
<p>To unassign work items from users: </p>
<ol>
<li value="1">In the Workload Balancer, go to the <strong>Assigned Work</strong> area and expand a user.</li>
<li value="2">Do 
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
one of
</MadCap:conditionalText>
the following:
<ul>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Find the item you want to unassign in a user's area, click it, drag and drop it in the Unassigned area or in another user's area. </p></li>
<li><p>Click the <strong>More</strong> icon <img src="assets/more-icon-task-list.png"> to the right of the name of a work item, click&nbsp;<strong>Assign this to</strong> , then remove the name of the entities assigned to the work item or enter another name and click&nbsp;<strong>Save</strong>.</p><p><img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"></p></li>
</ul><p>The item displays in the Unassigned Work area if it matches the filtering criteria for that area and it is not assigned to any users or it displays in the user area if it is assigned to that user. </p><note type="tip">
Unassigned issues do not display in the Unassigned area.
</note><p>For information about filtering information in the Workload Balancer, see <a href="../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md" class="MCXref xref">Manage filters in the Workload Balancer</a>. </p></li>
</ol>
</div>
-->
