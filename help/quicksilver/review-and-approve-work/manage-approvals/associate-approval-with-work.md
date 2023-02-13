---
product-area: projects
navigation-topic: approvals
title: Associa un processo di approvazione nuovo o esistente al lavoro
description: Questo articolo descrive come associare i processi di approvazione agli elementi di lavoro. Per informazioni sull'associazione delle approvazioni a bozze o documenti, vedere i seguenti articoli.
author: Courtney and Alina
feature: Work Management
exl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
source-git-commit: 7dbb9ca9b26f17710a7897e98dca109b5c886bd7
workflow-type: tm+mt
source-wordcount: '1869'
ht-degree: 0%

---

# Associa un processo di approvazione nuovo o esistente al lavoro

Questo articolo descrive come associare i processi di approvazione agli elementi di lavoro. Per informazioni sull&#39;associazione delle approvazioni a bozze o documenti, vedere i seguenti articoli:

* [Creare una bozza avanzata con un flusso di lavoro automatizzato](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Richiedere l&#39;approvazione del documento](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

È possibile associare un processo di approvazione globale o a uso singolo a un elemento di lavoro in Adobe Workfront. Esistono i seguenti scenari:

* Associa un processo di approvazione globale esistente a un progetto, un&#39;attività, un problema, un modello o un&#39;attività modello. Alcuni processi di approvazione globale sono disponibili per tutti i gruppi del sistema. I processi di approvazione globale a livello di gruppo sono disponibili solo per determinati gruppi.
* Crea un processo di approvazione a uso singolo e associalo a un&#39;attività di progetto, task, problema, modello o modello esistente.

>[!NOTE]
>
>Questo articolo utilizza il termine &quot;processo di approvazione globale&quot; per differenziarsi dal &quot;processo di approvazione a uso singolo&quot;. È possibile utilizzare ripetutamente un processo di approvazione globale.
>
>Il termine &quot;processo di approvazione globale a livello di gruppo&quot; si riferisce a un processo di approvazione che può essere utilizzato ripetutamente per gli elementi e con gli stati associati solo a un gruppo specifico.

Per informazioni più generali sui processi di approvazione, vedi [Panoramica del processo di approvazione](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Per informazioni sulla creazione di un processo di approvazione globale, vedi [Creazione di un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modificare l’accesso o una versione successiva a Progetti, Attività, Problemi o Modelli</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestisci le autorizzazioni per il progetto, l'attività, il problema o il modello</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Considerazioni sull&#39;associazione dei processi di approvazione con gli elementi di lavoro

Oltre alle considerazioni descritte di seguito, ti consigliamo di rivedere le considerazioni generali sui processi di approvazione in Workfront. Per ulteriori informazioni, consulta [Panoramica del processo di approvazione](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Approvals can only be associated with the status of a project, task, or issue in Workfront.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Each approval process corresponds with a status option in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.</p> <p>(NOTE: the two drafted bullets have been moved to the approval-process-in-workfront article)</p> </li>
  -->

* È necessario creare il progetto, l&#39;attività, il problema, il modello o l&#39;attività del modello prima che il processo di approvazione possa essere associato ad essi.
* Quando alleghi un processo di approvazione a un elemento per uno stato passato e in cui l&#39;elemento è attualmente, il processo di approvazione non verrà attivato e non verranno inviate notifiche agli approvatori.

   **Esempio:** Se un&#39;attività si trova nello stato Completa e si allega un processo di approvazione associato allo stato Completa, l&#39;approvazione non viene attivata.

* Quando si allega un processo di approvazione al primo stato di un elemento (utilizzando un modello per attività e progetti, utilizzando le impostazioni di configurazione della coda per i problemi o definendo le impostazioni attività di un progetto per le nuove attività), i processi di approvazione vengono ignorati se l&#39;approvazione inviata viene richiamata. In questo caso, gli approvatori non ricevono alcuna notifica.

   Per ulteriori informazioni sul richiamo delle approvazioni, vedi [Visualizza approvazioni](../../review-and-approve-work/manage-approvals/view-approvals.md).

   >[!TIP]
   >
   >Il primo stato per un&#39;attività o un problema è Nuovo. Il primo stato di un progetto è lo stato selezionato dall’amministratore Workfront in Preferenze progetto nel sistema. Per informazioni, consulta [Configurare le preferenze del progetto a livello di sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* L&#39;associazione dei processi di approvazione con un oggetto non viene registrata nell&#39;area Aggiornamenti per l&#39;oggetto.
* Non è possibile associare un processo di approvazione a un&#39;attività padre.
* L&#39;aggiunta di un utente, un team o un ruolo come approvatore non concede automaticamente le autorizzazioni all&#39;oggetto associato a tale approvazione. Essi ricevono le autorizzazioni per l&#39;oggetto quando viene attivato il passaggio di approvazione. In caso contrario, gli oggetti devono essere condivisi con loro prima di poter prendere una decisione di approvazione.

Le sezioni seguenti descrivono i diversi metodi di associazione di un processo di approvazione a un progetto, un&#39;attività o un problema.

## Associa un processo di approvazione globale a un elemento di lavoro {#associate-a-global-approval-process-with-a-work-item}

È possibile associare un processo di approvazione globale a un elemento di lavoro (progetto, task, problema, modello, task modello).

Il processo di approvazione globale deve essere disponibile per il gruppo associato all&#39;elemento di lavoro o per tutti i gruppi del sistema.

>[!NOTE]
È possibile allegare i processi di approvazione dei progetti a un modello e i processi di approvazione delle attività a un&#39;attività modello. In questo modo, quando un utente utilizza il modello per creare un progetto, il processo di approvazione diventa rispettivamente un processo di approvazione del progetto o dell&#39;attività. Un processo di approvazione a uso singolo allegato a un modello o a un modello rimane un processo di approvazione a uso singolo per progetti e attività.

Per informazioni su come gli amministratori di Workfront possono configurare un processo di approvazione globale per tutti i gruppi del sistema e su come gli amministratori di gruppo possono creare approvazioni per un gruppo, consulta [Creazione di un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
Puoi anche modificare un processo di approvazione globale per soddisfare le tue esigenze specifiche. Per ulteriori informazioni, consulta la sezione . [Modificare un processo di approvazione globale da utilizzare su un oggetto specifico](#modify-a-global-approval-process-for-use-on-a-specific-object) in questo articolo.

Per associare un processo di approvazione globale esistente a un progetto, task, problema, modello o modello:

1. Passare all&#39;elemento di lavoro in cui si desidera associare un processo di approvazione.
1. Fai clic su **Approvazioni** nel pannello a sinistra.

   Potrebbe essere necessario fare clic su **Mostra altro**, quindi fai clic su **Approvazioni**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. ![](assets/use-existing-or-create-single-use-approvals-menus-on-pti-classic-350x50.png)

   Viene visualizzato il processo di approvazione selezionato.

1. Espandi la **Usa esistente** menu a discesa e selezionare un processo di approvazione esistente.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

   Viene visualizzato il processo di approvazione selezionato.

   ![](assets/existing-approval-attached-to-task-redesigned-nwe-350x355.png)

1. Fai clic su **Salva**.
1. (Facoltativo) Fare clic su Modifica processo di approvazione per modificare l&#39;approvazione esistente collegata all&#39;elemento. In questo modo il processo di approvazione globale viene modificato in un processo di approvazione a uso singolo. Per ulteriori informazioni, consulta la sezione . [Modificare un processo di approvazione globale da utilizzare su un oggetto specifico](#modify-a-global-approval-process-for-use-on-a-specific-object) in questo articolo.

## Modificare un processo di approvazione globale da utilizzare su un oggetto specifico {#modify-a-global-approval-process-for-use-on-a-specific-object}

L&#39;amministratore di Workfront o l&#39;amministratore di gruppo crea processi di approvazione globali da utilizzare, come descritto in [Creazione di un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

La modifica di un processo di approvazione globale allegato a un elemento è identica alla modifica di un processo di approvazione a uso singolo.

È possibile modificare un processo di approvazione globale in base alle esigenze specifiche del progetto, dell&#39;attività o del problema associato.

>[!IMPORTANT]
Quando si modifica un processo di approvazione globale, questo diventa un processo di approvazione a uso singolo che può essere utilizzato solo sull&#39;oggetto in cui è stato modificato. Il processo di approvazione globale rimane invariato.
Quando modifichi un processo di approvazione globale, considera le seguenti limitazioni:
* Il processo di approvazione viene modificato solo per il progetto, l&#39;attività o il problema a cui si sta associando il processo di approvazione.
* Eventuali modifiche future apportate da un amministratore al processo di approvazione globale originale non si riflettono sul processo di approvazione globale modificato.
>


Per modificare un processo di approvazione già associato a un elemento:

1. Aggiungi un processo di approvazione globale al progetto, all&#39;attività o al problema.

   Per istruzioni, consulta la sezione . [Associa un processo di approvazione globale a un elemento di lavoro](#associate-a-global-approval-process-with-a-work-item) in questo articolo.

   >[!IMPORTANT]
   Assicurati di fare clic su **Salva** quando aggiungi l’approvazione.

1. Dopo aver aggiunto il processo di approvazione globale, fai clic sul pulsante **Modifica** icona ![](assets/edit-icon.png) nell&#39;angolo superiore destro della pagina di approvazione. Questa azione trasforma il processo di approvazione a livello globale o di gruppo in un processo di approvazione a uso singolo.
1. Apporta eventuali modifiche al processo di approvazione esistente. Per ulteriori informazioni, consulta la sezione . [Associa un processo di approvazione a uso singolo a un progetto, un&#39;attività, un problema, un modello o un&#39;attività modello](#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task) in questo articolo.
1. Fai clic su **Salva**, quindi fai clic su **Salva** di nuovo per confermare che si desidera convertire il processo di approvazione globale in un processo di approvazione a uso singolo disponibile solo su questo oggetto.

## Associa un processo di approvazione a uso singolo a un progetto, un&#39;attività, un problema, un modello o un&#39;attività modello {#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task}

È possibile creare un processo di approvazione a uso singolo da utilizzare solo su un progetto, un&#39;attività o un problema specifico.

È inoltre possibile associare un processo di approvazione a uso singolo a un modello o a un&#39;attività modello in modo che sia disponibile per i progetti e le attività creati dal modello.

>[!NOTE]
È possibile associare un processo di approvazione a uso singolo a qualsiasi stato a livello di sistema o di gruppo per un progetto, un&#39;attività, un problema, un modello o un&#39;attività del modello. Per informazioni sugli stati di Workfront, consulta [Creare o modificare uno stato](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

La creazione di un processo di approvazione in questo modo consente di creare un processo di approvazione personalizzato per soddisfare le tue esigenze. Tuttavia, il processo di approvazione non può essere associato ad altri elementi di lavoro in futuro.

In alternativa, è possibile modificare un processo di approvazione globale per un elemento specifico e che diventa anche un processo di approvazione a uso singolo. Per informazioni, consulta la sezione . [Modificare un processo di approvazione globale da utilizzare su un oggetto specifico](#modify-a-global-approval-process-for-use-on-a-specific-object) in questo articolo.

Per creare un processo di approvazione a uso singolo:

1. Passare all&#39;attività del progetto, dell&#39;attività, del problema, del modello o del modello in cui si desidera associare un processo di approvazione.
1. Fai clic su **Approvazioni** nel pannello a sinistra.

   Potrebbe essere necessario fare clic su **Mostra altro** > **Approvazioni**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Fai clic su **Creare un utilizzo singolo**.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

1. Completa i passaggi che iniziano con il passaggio 6 nella sezione &quot;Creare un processo di approvazione globale a livello di sistema o di gruppo per gli elementi di lavoro&quot; nell&#39;articolo [Creazione di un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: overtime, ensure step 6 is still accurate here)&nbsp;</p>
   -->

   >[!TIP]
   Dopo aver allegato il processo di approvazione a uso singolo, viene visualizzato come &quot;`<Custom>`&quot; nel campo Processo di approvazione all&#39;interno della casella Modifica di modelli e task modello. Per informazioni sulla modifica di modelli o attività di modelli, vedere i seguenti articoli:
   * [Modificare i modelli di progetto](../../manage-work/projects/create-and-manage-templates/edit-templates.md)
   * [Modificare un’attività modello](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)


   <!--
   ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be removed when they bring the new Edit Template/ Template Task boxes to NWE) </p>   >
   -->

## Rimuovere o eliminare un processo di approvazione da un elemento di lavoro

È possibile rimuovere un processo di approvazione globale o a livello di gruppo oppure eliminare un processo di approvazione a uso singolo da un progetto, un&#39;attività o un problema precedentemente associato.

Esistono i seguenti scenari: 

* La rimozione del processo di approvazione a livello globale o di gruppo non comporta l&#39;eliminazione dell&#39;approvazione. L&#39;approvazione rimane disponibile per un utilizzo futuro.
* L&#39;eliminazione di un processo di approvazione per un singolo utente lo elimina da Workfront e non può essere recuperato.

Per rimuovere o eliminare un processo di approvazione da un elemento di lavoro:

1. Passare all&#39;attività di progetto, attività, problema, modello o modello in cui si desidera rimuovere un processo di approvazione aggiunto in precedenza.
1. Fai clic su **Approvazioni** nel pannello a sinistra.

   Potrebbe essere necessario fare clic su **Mostra altro** > **Approvazioni**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Fai clic su una delle seguenti icone nell&#39;angolo superiore destro della sezione Approvazioni , a seconda del tipo di approvazione associata all&#39;elemento:

   * **Rimuovi** icona ![](assets/remove-icon---x-in-circle.png) per le approvazioni globali o a livello di gruppo.
   * **Elimina** icona ![](assets/delete.png) per le approvazioni per uso singolo.

1. Fai clic su **Rimuovi** o **Elimina** per confermare.

   Il processo di approvazione viene rimosso dall&#39;elemento di lavoro.

## Associazione automatica del processo di approvazione agli elementi di lavoro

È possibile associare automaticamente un processo di approvazione agli elementi di lavoro utilizzando i seguenti flussi di lavoro:

* Per progetti e attività, è possibile associare un processo di approvazione utilizzando un modello. È possibile allegare un processo di approvazione esistente alla scheda Approvazioni modello o Approvazioni task modello. Per informazioni sull&#39;associazione di un&#39;approvazione esistente a un elemento di lavoro, vedere [Associa un processo di approvazione globale a un elemento di lavoro](#associate-a-global-approval-process-with-a-work-item) in questo articolo.
* Per le nuove attività di un progetto esistente, è possibile associare un processo di approvazione globale o un processo di approvazione globale a livello di gruppo nell&#39;area Impostazioni attività della casella Modifica progetto. Per informazioni, consulta la sezione &quot;Impostazioni attività&quot; nell’articolo [Modifica progetti](../../manage-work/projects/manage-projects/edit-projects.md).
* Per i problemi, puoi associare un’approvazione a ogni nuovo problema aggiunto a un progetto associando un processo di approvazione esistente a una coda di richiesta. Per informazioni sulla configurazione delle code di richiesta, vedi [Creare una coda di richiesta](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
