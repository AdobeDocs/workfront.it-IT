---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Rimuovere gli indicatori di progresso dagli obiettivi in Obiettivi di Adobe Workfront
description: Puoi rimuovere risultati, attività e progetti dagli obiettivi in Obiettivi di Adobe Workfront, quando non sono più rilevanti.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Rimuovere gli indicatori di progresso dagli obiettivi in Obiettivi di Adobe Workfront

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

Puoi rimuovere risultati, attività e progetti dagli obiettivi se non sono più rilevanti.

Per informazioni sulla creazione di obiettivi e sull’aggiunta di risultati e attività, consulta i seguenti articoli:

* [Crea obiettivi in Obiettivi Adobe Workfront](../../workfront-goals/goal-management/create-goals.md)
* [Aggiungi attività agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Aggiungi risultati agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Modificare risultati e attività in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

Gli obiettivi possono anche essere allineati agli obiettivi principali, diventando obiettivi secondari. Gli obiettivi figlio sono anche indicatori di progresso degli obiettivi padre.

È possibile rimuovere l’allineamento tra gli obiettivi rimuovendo la connessione tra di essi. Per informazioni, consulta [Rimuovere l&#39;allineamento dell&#39;obiettivo negli Obiettivi di Adobe Workfront](../goal-alignment/remove-goal-alignment.md).

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
 <td role="rowheader">Licenza Adobe Workfront*</td>
 <td>
 <p>Nuova licenza: Collaboratore o versione successiva</p>
 Oppure
 <p>Licenza corrente: richiesta o successiva</p> <p>Per ulteriori informazioni, vedere <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica delle licenze di Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Prodotto*</td>
 <td>
 <p> Nuovo requisito del prodotto, uno dei seguenti: </p>
<ul>
<li>Un piano Select o Prime Adobe Workfront e un’ulteriore licenza Adobe Workfront Goals.</li>
<li>Un piano Workfront Ultimate che include gli obiettivi Workfront per impostazione predefinita. </li></ul>
 <p>Oppure</p>
 <p>Fabbisogno di prodotto corrente: un piano Workfront e una licenza aggiuntiva per gli obiettivi Adobe Workfront. </p> <p>Per informazioni, vedere <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisiti per l'utilizzo degli obiettivi di Workfront</a>. </p> </td>
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
  <p>Per informazioni sulla condivisione degli obiettivi, vedere <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Condividere un obiettivo in Obiettivi di Workfront</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l’area Obiettivi nel menu principale. </p>  
</td>
  </tr>
</tbody>
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisiti

Devi avere un obiettivo associato a risultati, attività o progetti.

## Considerazioni sulla rimozione di risultati, attività e disconnessione di progetti dagli obiettivi

* Puoi rimuovere risultati e attività solo da obiettivi attivi.
* Puoi rimuovere risultati e attività da un obiettivo eliminandoli. Non è possibile recuperare i risultati e le attività eliminati.
* Quando rimuovi il risultato o l’attività da un obiettivo, l’avanzamento del risultato o dell’attività rimosso influisce sull’avanzamento complessivo dell’obiettivo.
* Non è possibile eliminare un progetto da un obiettivo, ma è possibile disconnetterlo dall’obiettivo. Disconnettendo il progetto dall’obiettivo, la percentuale di completamento del progetto non influisce più sull’avanzamento dell’obiettivo.

  Per informazioni su come i progetti influenzano l&#39;avanzamento dell&#39;obiettivo, vedi [Aggiungere progetti agli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Non è possibile rimuovere un risultato o un’attività da un obiettivo e non è possibile disconnettere un obiettivo figlio o un progetto, se sono l’ultimo indicatore di avanzamento dell’obiettivo.
* Se un progetto viene eliminato dall’area Progetti e rappresenta l’ultimo indicatore di avanzamento di un obiettivo, l’obiettivo diventa Inattivo.

## Elimina risultati e attività dagli obiettivi

Per rimuovere risultati e attività da un obiettivo, devi eliminarli. L&#39;eliminazione di risultati e attività da un obiettivo è identica.

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

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** in alto a destra, quindi fai clic su **Obiettivi**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   Viene visualizzata l&#39;area Obiettivi di Workfront e l&#39;elenco Obiettivi viene visualizzato per impostazione predefinita.

1. Fai clic sul nome di un obiettivo da cui desideri rimuovere risultati e attività.

   Viene visualizzata la pagina dell’obiettivo.

1. Fai clic su **Indicatori di avanzamento** nel pannello a sinistra.

1. Seleziona un risultato o un&#39;attività, quindi fai clic sull&#39;icona **Elimina** ![](assets/delete-icon.png) nella parte superiore dell&#39;elenco.

1. Fai clic su **Elimina** per confermare l&#39;eliminazione. Il risultato o l’attività viene eliminato e non può essere recuperato. La percentuale di completamento degli aggiornamenti dell’obiettivo per escludere l’attività o il risultato eliminato.


## Rimuovi progetti dagli obiettivi

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


1. Fai clic sull&#39;icona **Main Menu** nell&#39;angolo superiore destro, quindi fai clic su **Goals**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Viene visualizzata l&#39;area Obiettivi di Workfront e l&#39;elenco Obiettivi viene visualizzato per impostazione predefinita.

1. Fai clic sul nome di un obiettivo da cui desideri rimuovere risultati e attività.

   Viene visualizzata la pagina dell’obiettivo.
1. Fai clic su **Indicatori di avanzamento** nel pannello a sinistra.
1. Seleziona un progetto, quindi fai clic sull&#39;icona ![](assets/disconnect-icon.png) di **Disconnetti** nella parte superiore dell&#39;elenco.
1. Fai clic su **Disconnetti** per confermare.

   Il progetto non è più connesso all’obiettivo. La percentuale di completamento degli aggiornamenti dell’obiettivo per escludere il progetto disconnesso.

