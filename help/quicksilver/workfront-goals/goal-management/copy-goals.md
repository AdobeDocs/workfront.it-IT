---
product-previous: workfront-goals
navigation-topic: goal-management
title: Copia degli obiettivi negli obiettivi di Adobe Workfront
description: Puoi copiare gli obiettivi in Obiettivi di Adobe Workfront per creare un obiettivo. Alcune delle informazioni di obiettivo originali vengono trasferite al nuovo obiettivo.
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Copia degli obiettivi negli obiettivi di Adobe Workfront

Puoi copiare gli obiettivi in Obiettivi di Adobe Workfront per creare un obiettivo. Alcune delle informazioni di obiettivo originali vengono trasferite al nuovo obiettivo.

## Requisiti di accesso

<!--drafted for P&P release: 

You must have the following:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
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
 </tbody>
</table>

-->

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Richiesta o superiore</p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica sulle licenze di Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td> <p>Devi acquistare una licenza aggiuntiva per la funzionalità Obiettivi di Adobe Workfront per accedere alla descritta in questo articolo. </p> <p>Per informazioni, consulta <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisiti per l'utilizzo degli obiettivi di Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Obiettivi o versioni successive</p> <p><b>NOTA</b>

<p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Concedere l’accesso agli obiettivi di Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> 
    <div> 
     <p>Gestione delle autorizzazioni per l'obiettivo</p> 
     <p>Per informazioni sulla condivisione degli obiettivi, vedi <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Condividere un obiettivo in Obiettivi di Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario disporre dei seguenti elementi prima di poter iniziare:

* Modello di layout che include l’area Obiettivi del menu principale.

## Considerazioni sulla copia degli obiettivi

Per poter copiare gli obiettivi, devi disporre dell&#39;accesso a Modifica obiettivi nel livello di accesso. Per informazioni sulla concessione dell&#39;accesso agli obiettivi, vedi [Concedere l’accesso agli obiettivi di Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Alcuni dei motivi per cui potrebbe essere utile copiare un obiettivo esistente sono:

* Al termine di un periodo di tempo (trimestre o anno), quando si desidera ricreare lo stesso obiettivo per il periodo successivo.
* Al termine di un periodo di tempo, quando l’obiettivo non può essere completato e si desidera utilizzarlo per un altro periodo di tempo.
* Quando più membri del team hanno obiettivi simili e potrebbe essere necessario crearne uno per ciascuno di essi.

>[!TIP]
>
>Puoi copiare un obiettivo in qualsiasi stato. Per informazioni sugli stati degli obiettivi, consulta [Panoramica sullo stato dell&#39;obiettivo negli obiettivi di Adobe Workfront](../../workfront-goals/goal-management/goal-status-overview.md).

Quando copi gli obiettivi, considera quanto segue:

* Tutte le informazioni sull&#39;obiettivo vengono copiate anche nel nuovo obiettivo.
* Puoi selezionare per copiare i risultati di un obiettivo esistente. Il nome dei risultati viene trasferito al nuovo obiettivo, ma l&#39;avanzamento corrente dei risultati sull&#39;obiettivo esistente non viene copiato nel nuovo obiettivo. Per impostazione predefinita, i risultati copiati vengono assegnati allo stesso proprietario.

   >[!NOTE]
   >
   >Se il proprietario originale è stato eliminato o disattivato da Workfront, il nuovo risultato viene assegnato all&#39;utente connesso.

* Non puoi copiare le attività di un obiettivo quando copi l’obiettivo.

## Copia obiettivi

<!--
Copying goals differs depending on what environment you use. 

To copy goals in the Production environment:

1. Go to a goal and click it to open the Goal Details panel.

   For information about accessing an individual goal, see the "Access individual goals" section in [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md).

   This opens the Goal Details panel.

1. Click the **More icon** ![](assets/more-icon.png), then click **Copy**. 

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


1. Vai a un obiettivo e fai clic sul pulsante **Altro** menu ![](assets/more-icon.png), quindi fai clic su **Obiettivo copia**.

   ![](assets/copy-goal-box-unshimmed.png)

1. Aggiorna le seguenti informazioni per l&#39;obiettivo copiato:
   * **Nome dell&#39;obiettivo**: Nome del nuovo obiettivo. Il nome predefinito per l&#39;obiettivo copiato è &quot;Copia di &lt;original goal=&quot;&quot;>&quot;.
   * **Punto**: Periodo di tempo durante il quale desideri raggiungere l’obiettivo. Selezionare un periodo di tempo dal menu a discesa

      Oppure

      Seleziona **Abilita date personalizzate** per specificare date personalizzate per l&#39;obiettivo **Inizio** e **Date di fine**. L’impostazione Abilita date personalizzate è disabilitata per impostazione predefinita.

      >[!TIP]
      >
      >   Deselezionando l&#39;opzione Abilita date personalizzate, viene ripristinato il periodo di tempo dell&#39;obiettivo originale.

      * **Proprietario dell&#39;obiettivo**: Il proprietario dell&#39;obiettivo. Può essere un utente, un team, un gruppo o un&#39;azienda. Il valore predefinito è il proprietario dell&#39;obiettivo originale.
      * **Descrizione**: Informazioni aggiuntive sull&#39;obiettivo.
      * **Copia risultati**: Selezionare questa opzione se si desidera trasferire i risultati dall&#39;obiettivo corrente all&#39;obiettivo copiato. Questo duplica i risultati originali e li allega all&#39;obiettivo copiato. I risultati dell&#39;obiettivo copiato hanno gli stessi proprietari, nomi e valori misurati dei risultati dell&#39;obiettivo originale.

         >[!NOTE]
         >
         >* L&#39;avanzamento del risultato originale non viene trasferito all&#39;obiettivo copiato.
         >* Se il proprietario originale è stato eliminato o disattivato da Workfront, il nuovo risultato viene assegnato all&#39;utente connesso.


1. Fai clic su **Copia obiettivo**.

   Viene creato un obiettivo simile a quello originale ed è nello stato Bozza.

   >[!NOTE]
   >
   >Se i risultati dell&#39;obiettivo originale non sono stati copiati, prima di attivarli è necessario associare il nuovo obiettivo a un indicatore di avanzamento e iniziare a lavorare per raggiungerlo.
   >Per informazioni sull’associazione degli obiettivi agli indicatori di avanzamento, consulta i seguenti articoli:
   >* [Aggiungere risultati agli obiettivi in Obiettivi di Adobe Workfront](../results-and-activities/add-results-to-goals.md)
   >* [Aggiungere attività agli obiettivi in Obiettivi di Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   >* [Allineare gli obiettivi collegandoli negli obiettivi di Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md)

   >
   >Per informazioni sull’attivazione degli obiettivi, vedi [Attivare gli obiettivi](../goal-management/activate-goals.md).

