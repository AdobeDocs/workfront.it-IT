---
product-previous: workfront-goals
navigation-topic: goal-management
title: Creare gli obiettivi in Obiettivi di Adobe Workfront
description: Che tu sia un amministratore delegato, un manager o un collaboratore singolo, puoi creare degli obiettivi in Obiettivi di Adobe Workfront per allineare il tuo lavoro con i tuoi obiettivi e gli obiettivi che delineano la strategia della tua organizzazione.
author: Alina
feature: Workfront Goals
exl-id: 14bf48b6-eb0c-4b00-a1a4-0d070ccc1392
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 5%

---

# Creare gli obiettivi in Obiettivi di Adobe Workfront

Che tu sia un amministratore delegato, un manager o un collaboratore singolo, puoi creare degli obiettivi in Obiettivi di Adobe Workfront per allineare il tuo lavoro con i tuoi obiettivi e gli obiettivi che delineano la strategia della tua organizzazione.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">piano Adobe Workfront</td>
 <td>
 <p>Qualsiasi</p>

</td>
 </tr>
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
<td role="rowheader">Livello di accesso*</td>
<td> <p>Modifica accesso agli obiettivi</p> </td>
</tr>
<tr data-mc-conditions="">
<td role="rowheader">Autorizzazioni oggetto</td>
<td>
<p>Visualizza o autorizzazioni superiori per l’obiettivo per visualizzarlo</p>
<p>Gestire le autorizzazioni per l’obiettivo per modificarlo</p>
<p>Per informazioni sulla condivisione degli obiettivi, consulta <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Condividere un obiettivo in Obiettivi di Workfront</a>. </p>
</td>
</tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l’area Obiettivi nel menu principale. </p>  
</td>
  </tr>
</tbody>
</table>

*Per ulteriori informazioni, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Linee guida per la creazione di obiettivi

Prima di iniziare a utilizzare gli obiettivi di Workfront, consigliamo di leggere le best practice consigliate e le linee guida per una gestione efficace degli obiettivi. Per ulteriori informazioni sulle linee guida per la creazione e la gestione degli obiettivi, consulta [Panoramica sugli obiettivi di Adobe Workfront](../../workfront-goals/goal-management/wf-goals-overview.md).

## Creare gli obiettivi

Questo articolo descrive come creare un obiettivo strategico negli Obiettivi di Workfront. Per informazioni sulla creazione di un obiettivo del caso di business, consulta [Creare obiettivi di business case](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

Puoi creare un obiettivo strategico in uno dei seguenti modi:

* [Creare un obiettivo da zero](#create-a-goal-from-scratch)
* [Copia un obiettivo esistente](#copy-an-existing-goal)
* [Convertire un risultato o un’attività in un obiettivo](#convert-a-result-or-activity-to-a-goal)

### Creare un obiettivo da zero {#create-a-goal-from-scratch}

<!--
Creating goals differs depending on what environment you use.

#### Create a goal from scratch in the Production environment 


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -)

   The Goal List displays.

1. (Conditional) Click **Goal List**, **Graphs**, **Pulse**, or **Check-in** in the left pane, then click **Add Goal** in the upper-right corner of the page. The Add Goal box displays.

   ![](assets/add-goal-box-350x235.png)

   >[!TIP]
   >
   >You can add a goal from any section in Workfront Goals. The process for creating a goal is identical regardless of the section you choose to add the goal from.

1. Start typing what you want to achieve in the **Goal** field. This is the name of the goal and a required field. 
1. Select a time period when the goal should be executed in the **Period** drop-down menu. This is a pre-filled field. The default is the current quarter.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a **Start date** and an **End date** for your goal, if you clicked **Define custom dates**.

   >[!TIP]
   >
   >* You can create a goal with dates in any time period, including up to 2 years in the past. 
   >* When defining custom dates, they are constrained by the initial date you selected. So if you select quarter and then custom dates, you can't go beyond that quarter.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same timeframes for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your over-arching strategy.

1. (Optional) Click your name in the **Owner** field, if you want to indicate someone else as the owner of the goal. By default, you are the owner of goals you create. 
1. Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. (Optional) Enter a **Description** for the goal. This field is optional. 
1. Click **Save**.

   The status of the new goal is Draft.

   >[!IMPORTANT]
   >
   >You must associate a goal with a progress indicator to activate it and start working on it. 
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

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

-->

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro, quindi fai clic su **Obiettivi**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Viene visualizzato l’elenco degli obiettivi.
1. Clic **Nuovo obiettivo**.

   Viene visualizzata la casella Nuovo obiettivo.

   ![](assets/new-goal-box-unshimmed.png)

1. Immettere le informazioni nei campi riportati di seguito.
   * **Nome obiettivo**: immetti un nome per l’obiettivo. Questo è un campo obbligatorio.
   * **Periodo**: seleziona un trimestre o un anno predefinito dal campo **Periodo** campo a discesa

     Oppure

     Seleziona la **Abilita date personalizzate** , quindi seleziona un **Inizio** e **Data di fine** per l&#39;obiettivo.

     Gli anni precedenti, correnti e successivi e i rispettivi trimestri sono elencati come opzioni predefinite nel campo a discesa Periodo.

     Il periodo dell’obiettivo indica l’intervallo di tempo in cui prevedi che l’obiettivo venga completato.

   * **Proprietario obiettivo**: inizia a digitare il nome di un utente, un team, un gruppo o della tua organizzazione per indicare chi è il proprietario dell’obiettivo. Per impostazione predefinita, l’utente è selezionato come proprietario dell’obiettivo.
   * **Descrizione**: immetti informazioni aggiuntive sull’obiettivo.
1. Clic **Crea obiettivo**.

   Il nuovo obiettivo è elencato nell’elenco Obiettivo e ha lo stato **Bozza**.

   È necessario associare un obiettivo a un indicatore di avanzamento per attivarlo e iniziare a lavorarci.

   Per preparare un obiettivo da attivare, effettua almeno una delle seguenti operazioni:
   * Aggiungi un risultato

     Per informazioni sull’aggiunta dei risultati, consulta [Aggiungere risultati agli obiettivi in Obiettivi di Adobe Workfront](../results-and-activities/add-results-to-goals.md).
   * Aggiungere un’attività

     Per informazioni sull’aggiunta di attività, consulta [Aggiungere attività agli obiettivi in Obiettivi di Adobe Workfront](../results-and-activities/add-activities-to-goals.md).
   * Allinea un altro obiettivo

     Per informazioni sull&#39;allineamento degli obiettivi, vedere [Allineare gli obiettivi collegandoli in Obiettivi di Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md).


### Copiare un obiettivo esistente {#copy-an-existing-goal}

Puoi creare un obiettivo copiandone uno esistente.

Per informazioni sulla copia degli obiettivi, consulta [Copia obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/copy-goals.md).

### Convertire un risultato o un’attività in un obiettivo {#convert-a-result-or-activity-to-a-goal}

Puoi creare un obiettivo convertendo il risultato o l’attività di un obiettivo esistente in un obiettivo. Il nuovo obiettivo viene allineato all&#39;obiettivo originale.

Per informazioni sulla conversione di risultati e attività in obiettivi, consulta [Allineare gli obiettivi convertendo risultati e attività in obiettivi](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

