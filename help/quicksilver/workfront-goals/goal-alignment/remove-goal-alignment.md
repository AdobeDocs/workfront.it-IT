---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Rimuovere l’allineamento degli obiettivi negli obiettivi di Adobe Workfront
description: È possibile rimuovere l’allineamento tra due obiettivi se non ha più senso collegarli.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 2%

---

# Rimuovere l’allineamento dell’obiettivo in Obiettivi di Adobe Workfront

<!--Audited P&P only: 4/2025-->

È possibile rimuovere l’allineamento tra due obiettivi se non ha più senso collegarli.

Per informazioni sull&#39;allineamento degli obiettivi, vedere i seguenti articoli:

* [Allinea gli obiettivi collegandoli in Obiettivi Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [Allineare gli obiettivi convertendo risultati e attività in obiettivi](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
  <ul><li>Un piano Ultimate </li></ul>
   </p>
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
 <p>Licenza corrente: richiesta o successiva</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Prodotto*</td>
 <td>
   <p> Nuovo requisito prodotto: Workfront</p>
   Oppure
   <p>Requisiti attuali del prodotto: oltre a una licenza Workfront, è necessario acquistare una licenza per gli obiettivi Adobe Workfront. </p> <p>Per informazioni, vedere <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisiti per l'utilizzo degli obiettivi di Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Livello di accesso</td>
 <td> <p>Modifica accesso agli obiettivi</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorizzazioni oggetto</td>
 <td>
  <p>Visualizza o autorizzazioni superiori per l’obiettivo per visualizzarlo</p>
  <p>Gestire le autorizzazioni per l’obiettivo per modificarlo</p>
  <p>Per informazioni sulla condivisione degli obiettivi, vedere <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Condividere un obiettivo in Obiettivi di Workfront</a>. </p>
  </td>
 </tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l’area Obiettivi nel menu principale. </p>  
</td>
  </tr>
</tbody>
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare, è necessario disporre dei seguenti elementi:

* Un obiettivo principale a cui è associato almeno un obiettivo secondario. Gli obiettivi per bambini sono gli indicatori di progresso dell&#39;obiettivo.

## Considerazioni sulla rimozione dell’allineamento dell’obiettivo

Quando rimuovi l’allineamento tra due obiettivi, considera quanto segue:

* Per rimanere attivi, all&#39;obiettivo principale deve essere associato un altro obiettivo, attività o risultato.
* Non è possibile rimuovere un obiettivo figlio allineato da un obiettivo padre se è l&#39;unico indicatore di avanzamento dell&#39;obiettivo padre.
* L&#39;obiettivo secondario diventa un obiettivo autonomo quando ne rimuovete l&#39;allineamento all&#39;obiettivo principale.

## Rimuovere l’allineamento dell’obiettivo

<!--
Removing goal alignment differs depending on which environment you use.

### Remove goal alignment in the Production environment


1. Go to a child goal aligned to a parent goal. 
1. Click the goal name to open the **Goal Details** panel. 
1. Click the **gear icon** ![Gear icon](assets/gear-icon-settings.png) next to the parent goal, then click **Remove alignment**.

   ![Reove alignment](assets/edit-remove-alignment-350x88.png)

   The goal becomes a standalone goal and its progress no longer influences the progress of the original parent goal. 

1. (Optional) Click **Undo** in the lower-left corner of the screen if you want to revert this change and keep the goals aligned. 
1. (Optional) Add activities and results to either goals to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
-->

1. Accedi all&#39;area **Obiettivi** in Workfront e fai clic sul nome di un obiettivo per aprirne la pagina.
1. Dalla pagina dell&#39;obiettivo di un obiettivo principale, fai clic su **Indicatori di avanzamento** nel pannello a sinistra.

   ![Rimuovi allineamento obiettivo](assets/remove-goal-alignment-from-list-unshimmed.png)

1. Nel raggruppamento **Tipo: Obiettivo**, seleziona un obiettivo, quindi fai clic sull&#39;icona **Disconnetti** ![Icona Disconnetti](assets/disconnect-goal-to-remove-alignment-icon-unshimmed.png) nella parte superiore dell&#39;elenco.

   Viene visualizzata la casella Disconnetti.

1. Fare clic su **Disconnetti** per disconnettere l&#39;obiettivo selezionato dal relativo elemento padre.

   L’obiettivo diventa autonomo e non viene più elencato come indicatore di avanzamento dell’obiettivo originale. L’avanzamento dell’obiettivo disconnesso non influenza più l’avanzamento dell’obiettivo originale.

   Nell’angolo superiore destro della pagina viene visualizzato un messaggio di successo per confermare che l’obiettivo è stato disconnesso.
