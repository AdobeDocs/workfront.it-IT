---
product-previous: workfront-goals
navigation-topic: goal-management
title: Copia obiettivi in Obiettivi di Adobe Workfront
description: Puoi copiare gli obiettivi in Obiettivi di Adobe Workfront per creare un obiettivo. Alcune delle informazioni originali sull’obiettivo vengono trasferite al nuovo obiettivo.
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 4%

---

# Copia obiettivi in Obiettivi di Adobe Workfront

Puoi copiare gli obiettivi in Obiettivi di Adobe Workfront per creare un obiettivo. Alcune delle informazioni originali sull’obiettivo vengono trasferite al nuovo obiettivo.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> 
   <p>Per il nuovo piano e la nuova struttura delle licenze:
  <ul><li>Un piano Ultimate </li>
  Oppure
  <li>Una licenza aggiuntiva per Adobe Workfront Goals per i piani Prime o Select Adobe Workfront. </li></ul> </p>
<p>Per il piano corrente e la struttura delle licenze: 
<ul><li> A Pro o superiore </li>
  <li>Una licenza Adobe Workfront Goals oltre a una licenza Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <tr>
 <td role="rowheader">Licenza Adobe Workfront*</td>
 <td>
 <p>Nuova licenza: Collaboratore o versione successiva</p>
 Oppure
 <p>Licenza corrente: richiesta o successiva</p> <p>Per ulteriori informazioni, consulta <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica sulle licenze di Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Prodotto*</td>
 <td>
 <p> Nuovo requisito del prodotto, uno dei seguenti: </p>
<ul>
<li>Un piano Select o Prime Adobe Workfront e un’ulteriore licenza Adobe Workfront Goals.</li>
<li>Un piano Workfront Ultimate che include gli obiettivi Workfront per impostazione predefinita. </li></ul>
 <p>Oppure</p>
 <p>Fabbisogno di prodotto corrente: un piano Workfront e una licenza aggiuntiva per gli obiettivi Adobe Workfront. </p> <p>Per informazioni, consulta <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisiti per l’utilizzo degli obiettivi di Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Livello di accesso</td>
 <td> <p>Modifica accesso agli obiettivi</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorizzazioni oggetto</td>
 <td>
  <div>
  <p>Visualizza o autorizzazioni superiori per l’obiettivo per visualizzarlo</p>
  <p>Gestire le autorizzazioni per l’obiettivo per modificarlo</p>
  <p>Per informazioni sulla condivisione degli obiettivi, consulta <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Condividere un obiettivo in Obiettivi di Workfront</a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l’area Obiettivi nel menu principale. </p>  
</td>
  </tr>
</tbody>
</table>

*Per ulteriori informazioni, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Considerazioni per la copia degli obiettivi

Prima di poter copiare gli obiettivi, devi avere accesso a Modifica obiettivi nel tuo livello di accesso. Per informazioni su come concedere l’accesso agli obiettivi, consulta [Concedere l’accesso agli obiettivi di Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Alcuni dei motivi per cui potresti voler copiare un obiettivo esistente sono:

* Alla fine di un periodo di tempo (trimestre o anno), quando desideri ricreare lo stesso obiettivo per il periodo successivo.
* Alla fine di un periodo di tempo, quando l’obiettivo non può essere completato e desideri lavorarci per un altro periodo di tempo.
* Quando più membri del gruppo hanno obiettivi simili e potrebbe essere necessario crearne uno per ciascuno di essi.

>[!TIP]
>
>Puoi copiare un obiettivo in qualsiasi stato. Per informazioni sugli stati degli obiettivi, vedi [Panoramica sullo stato degli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/goal-status-overview.md).

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


1. Vai a un obiettivo e fai clic su **Altro** menu ![](assets/more-icon.png), quindi fai clic su **Copia obiettivo**.

   ![](assets/copy-goal-box-unshimmed.png)

1. Aggiorna le seguenti informazioni per l&#39;obiettivo copiato:
   * **Nome obiettivo**: nome del nuovo obiettivo. Il nome predefinito per l’obiettivo copiato è &quot;Copia di&quot; &lt;original goal=&quot;&quot;>&quot;.
   * **Periodo**: il periodo di tempo durante il quale desideri raggiungere l’obiettivo. Seleziona un periodo di tempo dal menu a discesa

     Oppure

     Seleziona **Abilita date personalizzate** per specificare date personalizzate per l’obiettivo **Inizio** e **Date di fine**. L’impostazione Abilita date personalizzate è disabilitata per impostazione predefinita.

     >[!TIP]
     >
     >   Deselezionando l’opzione Abilita date personalizzate si ritorna al periodo di tempo dell’obiettivo originale.

      * **Proprietario obiettivo**: proprietario dell’obiettivo. Può essere un utente, un team, un gruppo o un’azienda. L’impostazione predefinita è il proprietario dell’obiettivo originale.
      * **Descrizione**: informazioni aggiuntive sull’obiettivo.
      * **Copia risultati**: seleziona questa opzione se desideri trasferire i risultati dall’obiettivo corrente all’obiettivo copiato. In questo modo i risultati originali vengono duplicati e associati all&#39;obiettivo copiato. I risultati dell&#39;obiettivo copiato hanno lo stesso proprietario, nomi e valori misurati dei risultati dell’obiettivo originale.

        >[!NOTE]
        >
        >* L&#39;avanzamento del risultato originale non viene trasferito all&#39;obiettivo copiato.
        >* Se il proprietario originale è stato eliminato o disattivato da Workfront, il nuovo risultato viene assegnato all&#39;utente connesso.

1. Clic **Copia obiettivo**.

   Viene creato un obiettivo simile a quello originale, che si trova nello stato Bozza.

   >[!NOTE]
   >
   >Se non hai copiato i risultati dall’obiettivo originale, devi innanzitutto associare il nuovo obiettivo a un indicatore di avanzamento prima di poterlo attivare e iniziare a lavorare per raggiungerlo.
   >Per informazioni sull&#39;associazione degli obiettivi agli indicatori di avanzamento, vedere gli articoli seguenti:
   >* [Aggiungere risultati agli obiettivi in Obiettivi di Adobe Workfront](../results-and-activities/add-results-to-goals.md)
   >* [Aggiungere attività agli obiettivi in Obiettivi di Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   >* [Allineare gli obiettivi collegandoli in Obiettivi di Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md)
   >
   >Per informazioni sull’attivazione degli obiettivi, consulta [Attiva obiettivi](../goal-management/activate-goals.md).

