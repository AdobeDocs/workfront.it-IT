---
product-previous: workfront-goals
navigation-topic: goal-management
title: Copia obiettivi in Obiettivi di Adobe Workfront
description: Puoi copiare gli obiettivi in Obiettivi di Adobe Workfront per creare un obiettivo. Alcune delle informazioni originali sull’obiettivo vengono trasferite al nuovo obiettivo.
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 4%

---

# Copia obiettivi in Obiettivi di Adobe Workfront

<!--Audited for P&P only: 4/2025-->

Puoi copiare gli obiettivi in Obiettivi di Adobe Workfront per creare un obiettivo. Alcune delle informazioni originali sull’obiettivo vengono trasferite al nuovo obiettivo.

## Requisiti di accesso

>[!NOTE]
>
>La tua azienda potrebbe scegliere di continuare a utilizzare gli obiettivi di Adobe Workfront se ha acquistato questo pacchetto in passato. Per ulteriori dettagli, rivolgiti al rappresentante del tuo account.
>
>Adobe Workfront Goals non è più disponibile per l’acquisto.

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Pacchetto Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
 <tr>
 <tr>
 <td role="rowheader">Licenza Adobe Workfront</td>
 <td>
 <p>Collaboratore o versione successiva</p>
 <p>Richiedi o superiore</p></td>
 </tr>
 <tr>
 <td role="rowheader">Configurazione del livello di accesso</td>
 <td> <p>Modifica accesso agli obiettivi</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Autorizzazioni oggetto</td>
 <td>
  <div>
  <p>Visualizza o autorizzazioni superiori per l’obiettivo per visualizzarlo</p>
  <p>Gestire le autorizzazioni per l’obiettivo per modificarlo</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di sistema, deve essere assegnato un modello di layout che includa l'area Obiettivi nel menu principale. </p>  
</td>
  </tr>
</tbody>
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td>  
  </tr>
 <tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
  <p> New product requirement: Workfront</p>
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Considerazioni per la copia degli obiettivi

Prima di poter copiare gli obiettivi, devi avere accesso a Modifica obiettivi nel tuo livello di accesso. Per informazioni sulla concessione dell&#39;accesso agli obiettivi, vedere [Concedere l&#39;accesso agli obiettivi di Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Alcuni dei motivi per cui potresti voler copiare un obiettivo esistente sono:

* Alla fine di un periodo di tempo (trimestre o anno), quando desideri ricreare lo stesso obiettivo per il periodo successivo.
* Alla fine di un periodo di tempo, quando l’obiettivo non può essere completato e desideri lavorarci per un altro periodo di tempo.
* Quando più membri del gruppo hanno obiettivi simili e potrebbe essere necessario crearne uno per ciascuno di essi.

>[!TIP]
>
>Puoi copiare un obiettivo in qualsiasi stato. Per informazioni sugli stati degli obiettivi, vedere [Panoramica sullo stato degli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/goal-status-overview.md).

Quando copi gli obiettivi, tieni presente quanto segue:

* Tutte le informazioni sull’obiettivo vengono copiate anche nel nuovo obiettivo.
* Puoi scegliere di copiare i risultati di un obiettivo esistente. Il nome dei risultati viene trasferito al nuovo obiettivo, ma l’avanzamento corrente dei risultati sull’obiettivo esistente non viene copiato nel nuovo obiettivo. Per impostazione predefinita, i risultati copiati vengono assegnati allo stesso proprietario.

  >[!NOTE]
  >
  >Se il proprietario originale è stato eliminato o disattivato da Workfront, il nuovo risultato viene assegnato all&#39;utente connesso.

* Non è possibile copiare le attività di un obiettivo quando si copia l’obiettivo.

## Copia obiettivi

<!--
Copying goals differs depending on what environment you use. 

To copy goals in the Production environment:

1. Go to a goal and click it to open the Goal Details panel.

   For information about accessing an individual goal, see the "Access individual goals" section in [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md).

   This opens the Goal Details panel.

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Copy**. 

1. Update any of the following information for the copied goal:

   | Field |Description  |
   |---|---|
   | New Goal |The name of the new goal. The default is the name of the original goal.  |
   | Period |The time period during which you want to achieve the goal. Select a time period from the drop-down menu or click **Define custom dates** to indicate a custom time period. By default, the Period is always the current quarter. |
   | Owner |The owner of the goal. It can be a user, team, group, or a company. The default is the owner of the original goal.  |
   | Description |Additional information about the goal.  |

1. (Conditional) Select **Copy results** if the original goal had results added to it and you want to copy them to the new goal. This duplicates the original results to the new goal. The results of the copied goal have the same owner, names and measured values as the results of the original goal.

   >[!TIP]
   >
   >* The progress of the original result does not transfer to the copied goal. 
   >* If the original owner was deleted or deactivated from Workfront, the new result is assigned to the logged in user.

1. Click **Save**.

   The copied goal is saved with a status of Draft and displays in the Goal Details panel.

   >[!IMPORTANT]
   >
   >If you have not copied the results from the original goal, you must first associate the new goal with a progress indicator before you can activate it and start working towards achieving it. 
   >
   >Do at least one of the following to be able to activate a goal: 
   >   
   >* Add a Result
   >   
   >  For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >   
   >* Add an Activity
   >   
   >  For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >   
   >* Align another goal to it
   >   
   >  For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).
   >
   > For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../goal-management/activate-goals.md). 

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

   The copied goal displays in the following sections:

   * Goal List 
   * Check-in (after it is activated)
   * Goal Alignment section (after it is activated) 
   * Pulse
(!--drafted - this was important when we could not update the goal timeframe in the past but we can do that now - not needed
1. (Optional and conditional) If you have copied a goal that was not achieved in a previous time period to continue working on it in the following time period, do the following:

   1. Go to the original goal in the Goal List, Check-in page, or Pulse section and comment on the goal, to indicate that this goal was copied to another, more current goal. For information about commenting on a goal, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md).
   1. Close the original goal, to preserve the progress in its original time period. For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   1. Update the the **Initial** value of the new Result to match the **End At** value of the previous result, so that your new goal progress will start calculating from the point you achieved in the previous period.
   
-->


1. Vai a un obiettivo e fai clic sul menu **Altro** ![Icona Altro](assets/more-icon.png), quindi fai clic su **Copia obiettivo**.

   ![Copia casella obiettivo](assets/copy-goal-box-unshimmed.png)

1. Aggiorna le seguenti informazioni per l&#39;obiettivo copiato:
   * **Nome obiettivo**: nome del nuovo obiettivo. Il nome predefinito per l&#39;obiettivo copiato è &quot;Copia di &lt;obiettivo originale>&quot;.
   * **Periodo**: il periodo di tempo durante il quale desideri raggiungere l&#39;obiettivo. Seleziona un periodo di tempo dal menu a discesa

     Oppure

     Seleziona **Abilita date personalizzate** per specificare date personalizzate per le date di **Inizio** e **Fine** dell&#39;obiettivo. L’impostazione Abilita date personalizzate è disabilitata per impostazione predefinita.

     >[!TIP]
     >
     >   Deselezionando l’opzione Abilita date personalizzate si ritorna al periodo di tempo dell’obiettivo originale.

      * **Proprietario obiettivo**: proprietario dell&#39;obiettivo. Può essere un utente, un team, un gruppo o un’azienda. L’impostazione predefinita è il proprietario dell’obiettivo originale.
      * **Descrizione**: informazioni aggiuntive sull&#39;obiettivo.
      * **Copia risultati**: selezionare questa opzione per trasferire i risultati dall&#39;obiettivo corrente all&#39;obiettivo copiato. In questo modo i risultati originali vengono duplicati e associati all&#39;obiettivo copiato. I risultati dell&#39;obiettivo copiato hanno lo stesso proprietario, nomi e valori misurati dei risultati dell’obiettivo originale.

        >[!NOTE]
        >
        >* L&#39;avanzamento del risultato originale non viene trasferito all&#39;obiettivo copiato.
        >* Se il proprietario originale è stato eliminato o disattivato da Workfront, il nuovo risultato viene assegnato all&#39;utente connesso.

1. Fai clic su **Copia obiettivo**.

   Viene creato un obiettivo simile a quello originale, che si trova nello stato Bozza.

   >[!NOTE]
   >
   >Se non hai copiato i risultati dall’obiettivo originale, devi innanzitutto associare il nuovo obiettivo a un indicatore di avanzamento prima di poterlo attivare e iniziare a lavorare per raggiungerlo.
   >Per informazioni sull&#39;associazione degli obiettivi agli indicatori di avanzamento, vedere gli articoli seguenti:
   >* [Aggiungi risultati agli obiettivi in Obiettivi di Adobe Workfront](../results-and-activities/add-results-to-goals.md)
   >* [Aggiungi attività agli obiettivi in Obiettivi di Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   >* [Allinea gli obiettivi collegandoli in Obiettivi Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md)
   >
   >Per informazioni sull&#39;attivazione degli obiettivi, vedere [Attiva obiettivi](../goal-management/activate-goals.md).

