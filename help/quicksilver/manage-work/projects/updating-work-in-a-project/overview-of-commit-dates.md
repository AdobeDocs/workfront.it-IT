---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: Panoramica sulla data di conferma
description: La data di conferma è la data entro la quale un utente assegnato a un’attività o a un problema si impegna a completare l’attività o il problema. Questa è diversa dalla Data di completamento pianificata, in quanto è una stima più realistica della data di completamento fornita dall’utente che è direttamente responsabile del lavoro.
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 0%

---

# Panoramica sulla data di conferma

{{highlighted-preview}}

La data di conferma è la data entro la quale un utente assegnato a un’attività o a un problema si impegna a completare l’attività o il problema.

Questa è diversa dalla Data di completamento pianificata di un&#39;attività o di un problema, in quanto è una stima più realistica della data di completamento fornita solo dall&#39;utente responsabile del lavoro.

Per informazioni sulla data di completamento pianificata, vedi [Panoramica della data di completamento pianificata dell&#39;attività](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

## Panoramica sulla data di conferma

Quando si lavora con le date di commit, considera quanto segue:

* Solo le attività e i problemi hanno una Data di conferma.
* Le date di conferma non vengono impostate automaticamente da Adobe Workfront.\
  Quando crei un’attività o un problema, non viene assegnata una data di conferma all’attività o al problema.
* Se si è assegnati a un&#39;attività o a un problema, è possibile impostare la data di conferma eseguendo una delle operazioni seguenti:

   * Consenti a Workfront di impostare la Data di conferma in modo che corrisponda alla Data di completamento pianificata esistente dell’attività o del problema facendo clic su Lavoraci, Avvia problema o Avvia attività sull’attività o sul problema. Per informazioni sulla sostituzione del pulsante Lavoraci con un pulsante Start, vedere  [Sostituire il pulsante Lavoraci con un pulsante Start](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * Imposta manualmente la Data impegno in base a quando ritieni che l’attività o il problema possa essere completato. In questo modo, l&#39;assegnatario si impegna nei confronti del project manager a fare in modo che l&#39;attività o il problema venga completato entro una data specifica.
Per informazioni, consulta [Aggiorna le date di conferma per attività e problemi](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

>[!NOTE]
>
>Per modificare la data di conferma, è necessario essere il proprietario di un&#39;attività. I seguenti utenti non possono modificare la Data di conferma di un’attività:
>
>* Proprietario progetto
>* Sponsor del progetto
>* Responsabile risorse
>* Amministratore di Sistema
>* Qualsiasi altro assegnatario dell&#39;attività
>* Qualsiasi altro utente con autorizzazioni per l’attività.
>
>Per ulteriori informazioni sul Proprietario dell&#39;attività, vedi [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Individuare la data di conferma delle attività e dei problemi

La data di conferma per le attività e i problemi è disponibile nelle seguenti aree di Workfront:

* Pagina Dettagli
* Il pannello Riepilogo, dopo che un amministratore di Workfront o di gruppo lo ha aggiunto al modello di layout. Per informazioni, consulta [Personalizzare Home e Riepilogo utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).
* <span class="preview">L’intestazione di un’attività o di un problema, dopo che un amministratore di Workfront o di un gruppo l’ha aggiunta al modello di layout. Per informazioni, consulta [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md). </span>

## Notifiche e aggiornamenti attivati dalla modifica della data di conferma {#notifications-and-updates-triggered-by-changing-the-commit-date}

Quando un assegnatario di un’attività o di un problema modifica manualmente una Data di conferma in una data diversa dalla Data di completamento pianificata impostata dal proprietario del progetto, vi sono una serie di notifiche e aggiornamenti che avvisano il proprietario del progetto e altri utenti di questa modifica.

>[!NOTE]
>
>Le modifiche apportate alla data di conferma non modificano automaticamente le date pianificate e le modifiche apportate alle date pianificate non modificano automaticamente la data di conferma.

L’impostazione manuale della data di conferma per un’attività o un problema attiva le seguenti modifiche:

* La modifica della data di conferma viene popolata nelle schede Attività di sistema e Tutte nella sezione Aggiornamento dell’attività o del problema.

  ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)

  La modifica della data di conferma viene visualizzata nell’area Aggiornamenti dell’attività o del problema quando l’amministratore di Workfront abilita questo aggiornamento nell’area Feed aggiornamenti in Configurazione. Per informazioni, consulta [Aggiornamenti monitorati dal sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

  Se un proprietario del progetto non desidera accettare la modifica, è consigliabile che ritorni all&#39;utente che propone una nuova data utilizzando la scheda Commenti nella sezione Aggiornamenti, per chiedere di ripristinare la Data pianificata originale oppure di selezionare una nuova data.

  Se un proprietario del progetto accetta la modifica, può regolare manualmente la Data di completamento pianificata in modo che corrisponda alla Data impegno offerta dall&#39;utente assegnato all&#39;elemento modificando l&#39;attività o il problema.

  Devi avere accesso per gestire l’attività o il problema per modificarli.

  >[!TIP]
  >
  >Puoi chiedere all’amministratore del sistema o del gruppo di aggiungere il campo Conferma data al pannello Riepilogo o all’intestazione per semplificarne l’aggiornamento.
  >
  >Per ulteriori informazioni, consulta i seguenti articoli:
  >
  >* [Panoramica di riepilogo](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
  >* [Personalizzare Home e Riepilogo utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
  >* [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

<!--this is no longer possible: 
>[!NOTE]
>
>If you want to see how the timeline of the project is affected by accepting to change the Planned Completion Date of the task, click **Project Timeline**. This opens the task list where you can evaluate the date changes and the project timeline.
>
>
>![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >
>
-->


* La Data di completamento prevista dell’attività o del problema è impostata sulla stessa data perché l’attività ora dispone di un’indicazione più precisa di quando è probabile che venga completata.

  Per ulteriori informazioni sulla data di completamento prevista, consulta [Panoramica della data di completamento prevista per progetti, attività e problemi](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

  ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* Nell’area Notifiche viene inviata una notifica al proprietario del progetto per segnalare che la data di conferma di un’attività o di un problema è stata modificata.

  ![](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

  >[!TIP]
  >
  >La notifica relativa alla modifica della data di conferma viene inviata al proprietario del progetto solo quando l’amministratore di Workfront abilita la visualizzazione della data di conferma nell’area Feed aggiornamenti di Configurazione. Per informazioni, consulta [Aggiornamenti monitorati dal sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

Per informazioni sulle funzionalità aggiuntive disponibili durante l&#39;aggiornamento di un elemento di lavoro, vedere  [Aggiorna lavoro](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Per informazioni sull&#39;aggiornamento delle date di conferma per attività e problemi, vedere [Aggiorna le date di conferma per attività e problemi](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update Commit Dates on tasks and issues</h2>
<p>(NOTE: moved to its own article) </p>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <strong>Task Owner</strong>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click Work on it in the task or issue header</p> <p>Or</p> <p>Click <strong>Start Task</strong> or <strong>Start Issue</strong> if the Work on it button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <strong>Undo</strong> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <strong>This will be done by</strong> date picker, and select a new Commit Date.</p>
<div>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>Updates</strong> in the left panel, then click the <strong>Start a new update</strong>><strong>Commit Date</strong></p>
<p>Or</p>
<p>Click <strong>Task Details</strong> or <strong>Issue Details</strong> in the left panel, then double click <strong>Commit Date</strong> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifications-and-updates-triggered-by-changing-the-commit-date" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->
