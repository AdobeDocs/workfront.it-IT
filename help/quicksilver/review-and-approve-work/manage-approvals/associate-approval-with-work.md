---
product-area: projects
navigation-topic: approvals
title: Associa un processo di approvazione nuovo o esistente al lavoro
description: Questo articolo descrive come associare i processi di approvazione agli elementi di lavoro. Per informazioni sull’associazione delle approvazioni a bozze o documenti, consulta i seguenti articoli.
author: Courtney and Alina
feature: Work Management, Digital Content and Documents
sexl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
exl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1914'
ht-degree: 0%

---

# Associa un processo di approvazione nuovo o esistente al lavoro

Questo articolo descrive come associare i processi di approvazione agli elementi di lavoro. Per informazioni sull’associazione delle approvazioni a bozze o documenti, consulta i seguenti articoli:

* [Crea una bozza avanzata con un flusso di lavoro automatizzato](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Richiedere le approvazioni dei documenti](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

È possibile associare un processo di approvazione globale o monouso a un elemento di lavoro in Adobe Workfront. Esistono i seguenti scenari:

* Associare un processo di approvazione globale esistente a un progetto, un&#39;attività, un problema, un modello o un&#39;attività modello. Alcuni processi di approvazione globali sono disponibili per tutti i gruppi del sistema. I processi di approvazione globale a livello di gruppo sono disponibili solo per determinati gruppi.
* Crea un processo di approvazione a utente singolo e associalo a un progetto, un’attività, un problema, un modello o un’attività modello esistente.

>[!NOTE]
>
>In questo articolo viene utilizzato il termine &quot;processo di approvazione globale&quot; per differenziarlo dal termine &quot;processo di approvazione a utente singolo&quot;. Un processo di approvazione globale può essere utilizzato ripetutamente.
>
>Il termine &quot;processo di approvazione globale a livello di gruppo&quot; si riferisce a un processo di approvazione che può essere utilizzato ripetutamente per gli elementi e con stati associati solo a un gruppo specifico.

Per informazioni generali sui processi di approvazione, vedere [Panoramica sui processi di approvazione](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Per informazioni sulla creazione di un processo di approvazione globale, vedere [Creare un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modifica l'accesso o versione successiva a Progetti, Attività, Problemi o Modelli</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per il progetto, l’attività, il problema o il modello</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

+++

## Considerazioni sull&#39;associazione dei processi di approvazione agli elementi di lavoro

Oltre alle considerazioni descritte di seguito, è consigliabile rivedere le considerazioni generali sui processi di approvazione in Workfront. Per ulteriori informazioni, vedere [Panoramica del processo di approvazione](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Approvals can only be associated with the status of a project, task, or issue in Workfront.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Each approval process corresponds with a status option in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.</p> <p>(NOTE: the two drafted bullets have been moved to the approval-process-in-workfront article)</p> </li>
  -->

* È necessario creare il progetto, l’attività, il problema, il modello o l’attività modello prima di associare il processo di approvazione.
* Quando si allega un processo di approvazione a un elemento per uno stato che è stato superato e in cui si trova l&#39;elemento, il processo di approvazione non viene attivato e non viene inviata alcuna notifica agli approvatori.

  **Esempio:** se un&#39;attività è nello stato Completato e si allega un processo di approvazione associato allo stato Completato, l&#39;approvazione non viene attivata.

* Quando si allega un processo di approvazione al primo stato di un elemento (utilizzando un modello per le attività e i progetti, le impostazioni di Configurazione coda per i problemi o la definizione delle impostazioni attività di un progetto per le nuove attività), i processi di approvazione vengono ignorati se l&#39;approvazione inviata viene richiamata. In questo caso, gli approvatori non ricevono alcuna notifica.

  Per ulteriori informazioni sul richiamo delle approvazioni, vedere [Visualizza approvazioni](../../review-and-approve-work/manage-approvals/view-approvals.md).

  >[!TIP]
  >
  >Il primo stato di un’attività o di un problema è Nuovo. Il primo stato di un progetto è lo stato selezionato dall&#39;amministratore di Workfront nelle Preferenze progetto del sistema. Per informazioni, vedere [Configurare le preferenze di progetto a livello di sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* L&#39;associazione dei processi di approvazione a un oggetto non viene registrata nell&#39;area Aggiornamenti dell&#39;oggetto.
* Non è possibile associare un processo di approvazione a un task padre.
* L&#39;aggiunta di un utente, un team o un ruolo come approvatore non concede automaticamente le autorizzazioni per l&#39;oggetto associato a tale approvazione. Ricevono le autorizzazioni per l’oggetto quando viene attivato il passaggio di approvazione. In caso contrario, gli oggetti devono essere condivisi con loro prima di poter prendere una decisione di approvazione.

Nelle sezioni seguenti vengono descritti i diversi metodi di associazione di un processo di approvazione a un progetto, a un&#39;attività o a un problema.

## Associare un processo di approvazione globale a un elemento di lavoro {#associate-a-global-approval-process-with-a-work-item}

È possibile associare un processo di approvazione globale a un elemento di lavoro (progetto, attività, problema, modello, attività modello).

Il processo di approvazione globale deve essere disponibile per il gruppo associato all&#39;elemento di lavoro o per tutti i gruppi del sistema.

>[!NOTE]
>
>È possibile allegare i processi di approvazione del progetto a un modello e i processi di approvazione delle attività a un&#39;attività modello. Dopo questa operazione, quando un utente utilizza il modello per creare un progetto, il processo di approvazione diventa un processo di approvazione rispettivamente di un progetto o di un&#39;attività. Un processo di approvazione a utente singolo associato a un modello o a un&#39;attività modello rimane un processo di approvazione a utente singolo per progetti e attività.

Per informazioni su come gli amministratori di Workfront possono configurare un processo di approvazione globale per tutti i gruppi del sistema e su come gli amministratori di gruppi possono creare approvazioni per un gruppo, vedere [Creare un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>Puoi anche modificare un processo di approvazione globale per soddisfare esigenze specifiche. Per ulteriori informazioni, vedere la sezione [Modificare un processo di approvazione globale da utilizzare su un oggetto specifico](#modify-a-global-approval-process-for-use-on-a-specific-object) in questo articolo.

Per associare un processo di approvazione globale esistente a un progetto, un&#39;attività, un problema, un modello o un&#39;attività modello:

1. Passare all&#39;elemento di lavoro in cui si desidera associare un processo di approvazione.
1. Fai clic su **Approvazioni** nel pannello a sinistra.

   Potrebbe essere necessario fare clic su **Mostra altro**, quindi su **Approvazioni**.

   ![Sezione approvazioni sull&#39;attività](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. ![Utilizzare le approvazioni esistenti o creare approvazioni per utilizzo singolo](assets/use-existing-or-create-single-use-approvals-menus-on-pti-classic-350x50.png)

   Viene visualizzato il processo di approvazione selezionato.

1. Espandi il menu a discesa **Usa esistente** e seleziona un processo di approvazione esistente.

   ![Menu Approvazioni](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

   Viene visualizzato il processo di approvazione selezionato.

   ![Approvazione esistente allegata all&#39;attività](assets/existing-approval-attached-to-task-redesigned-nwe-350x355.png)

1. Fai clic su **Salva**.
1. (Facoltativo) Fare clic su Modifica processo di approvazione se si desidera modificare l&#39;approvazione esistente associata all&#39;elemento. In questo modo il processo di approvazione globale viene trasformato in un processo di approvazione a utente singolo. Per ulteriori informazioni, vedere la sezione [Modificare un processo di approvazione globale da utilizzare su un oggetto specifico](#modify-a-global-approval-process-for-use-on-a-specific-object) in questo articolo.

## Modificare un processo di approvazione globale da utilizzare su un oggetto specifico {#modify-a-global-approval-process-for-use-on-a-specific-object}

L&#39;amministratore di Workfront o l&#39;amministratore di gruppo crea processi di approvazione globali da utilizzare, come descritto in [Creare un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

La modifica di un processo di approvazione globale associato a un elemento è identica alla modifica di un processo di approvazione a utente singolo.

È possibile modificare un processo di approvazione globale in base alle esigenze specifiche del progetto, dell&#39;attività o del problema associato.

>[!IMPORTANT]
>
>Quando si modifica un processo di approvazione globale, questo diventa un processo di approvazione a uso singolo che può essere utilizzato solo sull&#39;oggetto in cui è stato modificato. Il processo di approvazione globale rimane invariato.
>
>Quando modifichi un processo di approvazione globale, considera le seguenti limitazioni:
>
>* Il processo di approvazione viene modificato solo per il progetto, l&#39;attività o il problema a cui si associa il processo di approvazione.
>* Eventuali modifiche future apportate da un amministratore al processo di approvazione globale originale non vengono applicate al processo di approvazione globale modificato.
>

Per modificare un processo di approvazione già associato a un elemento:

1. Aggiungi un processo di approvazione globale al progetto, all’attività o al problema.

   Per istruzioni, vedere la sezione [Associare un processo di approvazione globale a un elemento di lavoro](#associate-a-global-approval-process-with-a-work-item) in questo articolo.

   >[!IMPORTANT]
   >
   >Assicurati di fare clic su **Salva** durante l&#39;aggiunta dell&#39;approvazione.

1. Dopo aver aggiunto il processo di approvazione globale, fai clic sull&#39;icona **Modifica** icona ![Modifica](assets/edit-icon.png) nell&#39;angolo superiore destro della pagina di approvazione. Questa azione trasforma il processo di approvazione globale o a livello di gruppo in un processo di approvazione a utente singolo.
1. Apporta eventuali modifiche al processo di approvazione esistente. Per ulteriori informazioni, vedere la sezione [Associare un processo di approvazione a utente singolo a un progetto, un&#39;attività, un problema, un modello o un&#39;attività modello](#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task) in questo articolo.
1. Fai clic su **Salva**, quindi di nuovo su **Salva** per confermare che vuoi convertire il processo di approvazione globale in un processo di approvazione a utente singolo disponibile solo su questo oggetto.

## Associare un processo di approvazione a utente singolo a un progetto, un’attività, un problema, un modello o un’attività modello {#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task}

Puoi creare un processo di approvazione a utente singolo da utilizzare solo per un progetto, attività o problema specifico.

È inoltre possibile associare un processo di approvazione a utente singolo a un modello o a un&#39;attività modello in modo che sia disponibile nei progetti e nelle attività create dal modello.

>[!NOTE]
>
>È possibile associare un processo di approvazione a utente singolo a qualsiasi stato a livello di sistema o di gruppo per un progetto, un&#39;attività, un problema, un modello o un&#39;attività modello. Per informazioni sugli stati di Workfront, vedere [Creare o modificare uno stato](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

La creazione di un processo di approvazione consente di creare un processo di approvazione personalizzato in base alle esigenze. Tuttavia, il processo di approvazione non può essere associato ad altri elementi di lavoro in futuro.

In alternativa, è possibile modificare un processo di approvazione globale per un articolo specifico e che diventa anche un processo di approvazione a uso singolo. Per informazioni, vedere la sezione [Modificare un processo di approvazione globale da utilizzare su un oggetto specifico](#modify-a-global-approval-process-for-use-on-a-specific-object) in questo articolo.

Per creare un processo di approvazione per singolo utilizzo:

1. Passare al progetto, all&#39;attività, al problema, al modello o all&#39;attività modello a cui si desidera associare un processo di approvazione.
1. Fai clic su **Approvazioni** nel pannello a sinistra.

   Potrebbe essere necessario fare clic su **Mostra altro** > **Approvazioni**.

   ![Sezione approvazioni sull&#39;attività](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Fare clic su **Crea monouso**.

   ![Menu Approvazioni](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

1. Completare i passaggi che iniziano con il passaggio 6 della sezione &quot;Creare un processo di approvazione globale a livello di sistema o di gruppo per gli elementi di lavoro&quot; nell&#39;articolo [Creare un processo di approvazione per gli elementi di lavoro](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: overtime, ensure step 6 is still accurate here)&nbsp;</p>
   -->

   >[!TIP]
   >
   >Dopo aver allegato il processo di approvazione a utente singolo, viene visualizzato come &quot;`<Custom>`&quot; nel campo Processo di approvazione all&#39;interno della casella Modifica di modelli e attività modello. Per informazioni sulla modifica di modelli o attività modello, vedere i seguenti articoli:
   >
   >* [Modifica modelli di progetto](../../manage-work/projects/create-and-manage-templates/edit-templates.md)
   >* [Modifica un&#39;attività modello](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)

   <!--
   ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be removed when they bring the new Edit Template/ Template Task boxes to NWE) </p>   >
   -->

## Rimuovere o eliminare un processo di approvazione da un elemento di lavoro

È possibile rimuovere un processo di approvazione globale o a livello di gruppo oppure eliminare un processo di approvazione a utente singolo da un progetto, un&#39;attività o un problema precedentemente associato.

Esistono i seguenti scenari: 

* La rimozione del processo di approvazione globale o a livello di gruppo non comporta l’eliminazione dell’approvazione. L’approvazione rimane disponibile per un utilizzo futuro.
* Se si elimina un processo di approvazione per singolo utente, questo viene eliminato da Workfront e non può essere recuperato.

Per rimuovere o eliminare un processo di approvazione da un elemento di lavoro:

1. Vai al progetto, all’attività, al problema, al modello o all’attività modello in cui desideri rimuovere un processo di approvazione aggiunto in precedenza.
1. Fai clic su **Approvazioni** nel pannello a sinistra.

   Potrebbe essere necessario fare clic su **Mostra altro** > **Approvazioni**.

   ![Sezione approvazioni sull&#39;attività](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Fai clic su una delle seguenti icone nell&#39;angolo superiore destro della sezione Approvazioni, a seconda del tipo di approvazione associata all&#39;elemento:

   * **Icona Rimuovi** icona ![Icona Rimuovi](assets/remove-icon---x-in-circle.png) per le approvazioni globali o a livello di gruppo.
   * **Icona Elimina** icona ![Icona Elimina](assets/delete.png) per le approvazioni monouso.

1. Fai clic su **Rimuovi** o **Elimina** per confermare.

   Il processo di approvazione viene rimosso dall&#39;elemento di lavoro.

## Associare automaticamente un processo di approvazione agli elementi di lavoro

È possibile associare automaticamente un processo di approvazione agli elementi di lavoro utilizzando i seguenti flussi di lavoro:

* Per progetti e attività, è possibile associare un processo di approvazione utilizzando un modello. È possibile allegare un processo di approvazione esistente alla scheda Approvazioni modello o alla scheda Approvazioni attività modello. Per informazioni sull&#39;associazione di un&#39;approvazione esistente a un elemento di lavoro, vedere [Associare un processo di approvazione globale a un elemento di lavoro](#associate-a-global-approval-process-with-a-work-item) in questo articolo.
* Per le nuove attività di un progetto esistente, è possibile associare un processo di approvazione globale o un processo di approvazione globale a livello di gruppo nell&#39;area Impostazioni attività della casella Modifica progetto. Per informazioni, vedere la sezione &quot;Impostazioni attività&quot; nell&#39;articolo [Modifica progetti](../../manage-work/projects/manage-projects/edit-projects.md).
* Per i problemi, è possibile associare un’approvazione a ogni nuovo problema aggiunto a un progetto associando un processo di approvazione esistente a una coda di richieste. Per informazioni sulla configurazione delle code di richieste, vedere [Creare una coda di richieste](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
