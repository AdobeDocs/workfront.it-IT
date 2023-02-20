---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Rimuovere gli indicatori di avanzamento dagli obiettivi in Obiettivi di Adobe Workfront
description: Puoi rimuovere risultati, attività e progetti dagli obiettivi in Obiettivi di Adobe Workfront, quando non sono più rilevanti.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Rimuovere gli indicatori di avanzamento dagli obiettivi in Obiettivi di Adobe Workfront

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

Puoi rimuovere risultati, attività e progetti dagli obiettivi se non sono più rilevanti.

Per informazioni sulla creazione di obiettivi e sull’aggiunta di risultati e attività, consulta i seguenti articoli:

* [Creare obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/create-goals.md)
* [Aggiungere attività agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Aggiungere risultati agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Modificare risultati e attività in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

Gli obiettivi possono anche essere allineati agli obiettivi dei genitori, diventando obiettivi dei figli. Gli obiettivi figlio sono anche indicatori di progresso degli obiettivi padre.

È possibile rimuovere l&#39;allineamento tra gli obiettivi rimuovendo la connessione tra di essi. Per informazioni, consulta [Rimuovere l’allineamento dell’obiettivo negli obiettivi di Adobe Workfront](../goal-alignment/remove-goal-alignment.md).

## Requisiti di accesso

<!--drafted - replace the table below with this one when P&P releases: 

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
   <td> <p>Modificare l’accesso a Obiettivi o versioni successive</p> <p><b>NOTA</b><p>Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta:</p> 
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
* Un obiettivo con risultati, attività o progetti.

## Considerazioni sulla rimozione di risultati, attività e disconnessione di progetti dagli obiettivi

* Puoi rimuovere risultati e attività solo dagli obiettivi attivi.
* Puoi rimuovere risultati e attività da un obiettivo eliminandoli. I risultati e le attività eliminati non possono essere recuperati.
* Quando rimuovi il risultato o l’attività da un obiettivo, l’avanzamento del risultato rimosso o dell’attività influisce sul progresso complessivo dell’obiettivo.
* Non è possibile eliminare un progetto da un obiettivo, ma è possibile disconnetterlo dall&#39;obiettivo. Disconnettendo il progetto dall’obiettivo, la percentuale di completamento del progetto non influisce più sull’avanzamento dell’obiettivo.

   Per informazioni su come i progetti influiscono sul progresso dell’obiettivo, consulta [Aggiungere progetti agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Non è possibile rimuovere un risultato o un&#39;attività da un obiettivo e non è possibile scollegare un obiettivo secondario o un progetto, se si tratta dell&#39;ultimo indicatore di avanzamento dell&#39;obiettivo.
* Se un progetto viene eliminato dall’area Progetti ed è l’ultimo indicatore di avanzamento di un obiettivo, l’obiettivo diventa Inattivo.

## Eliminare risultati e attività dagli obiettivi

Puoi rimuovere risultati e attività da un obiettivo eliminandoli. L&#39;eliminazione di risultati e attività da un obiettivo è identica.

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell&#39;angolo in alto a destra, quindi fai clic su **Obiettivi**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   Viene visualizzata l’area Obiettivi di Workfront e l’elenco obiettivi per impostazione predefinita.

1. Fai clic sul nome di un obiettivo da cui desideri rimuovere i risultati e le attività.

   Viene visualizzata la pagina dell’obiettivo.

1. Fai clic su **Indicatori di progresso** nel pannello a sinistra.

1. Seleziona un risultato o un’attività, quindi fai clic sul pulsante **Elimina** icona ![](assets/delete-icon.png) in cima all&#39;elenco.

1. Fai clic su **Elimina** per confermare l’eliminazione. Il risultato o l&#39;attività viene eliminato e non può essere recuperato. La percentuale di completamento dell’obiettivo viene aggiornata per escludere l’attività o il risultato eliminato.


## Rimuovere progetti dagli obiettivi

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


1. Fai clic sul pulsante **Menu principale** nell&#39;angolo in alto a destra, quindi fai clic su **Obiettivi**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Viene visualizzata l’area Obiettivi di Workfront e l’elenco obiettivi per impostazione predefinita.

1. Fai clic sul nome di un obiettivo da cui desideri rimuovere i risultati e le attività.

   Viene visualizzata la pagina dell’obiettivo.
1. Fai clic su **Indicatori di progresso** nel pannello a sinistra.
1. Seleziona un progetto, quindi fai clic sul pulsante **Disconnetti** icona ![](assets/disconnect-icon.png) in cima all&#39;elenco.
1. Fai clic su **Disconnetti** per confermare.

   Il progetto non è più connesso all’obiettivo. La percentuale di completamento degli aggiornamenti dell&#39;obiettivo per escludere il progetto disconnesso.

