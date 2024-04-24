---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Rimuovere l’allineamento dell’obiettivo in Obiettivi di Adobe Workfront
description: È possibile rimuovere l’allineamento tra due obiettivi se non ha più senso collegarli.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: 2f8a5b2d2183090029966a13c7af37f20eb44fd0
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 1%

---

# Rimuovere l’allineamento dell’obiettivo in Obiettivi di Adobe Workfront

È possibile rimuovere l’allineamento tra due obiettivi se non ha più senso collegarli.

Per informazioni sull&#39;allineamento degli obiettivi, vedere i seguenti articoli:

* [Allineare gli obiettivi collegandoli in Obiettivi di Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [Allineare gli obiettivi convertendo risultati e attività in obiettivi](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

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
   <p>Nuovo piano: Seleziona o superiore</p>
   Oppure
   <p>Piano corrente: Pro o superiore</p>
   
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
    <p>Visualizza o autorizzazioni superiori per l’obiettivo per visualizzarlo</p>
     <p>Gestire le autorizzazioni per l’obiettivo per modificarlo</p>
     <p>Per informazioni sulla condivisione degli obiettivi, consulta <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Condividere un obiettivo in Obiettivi di Workfront</a>. </p>
    </td>
  </tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l’area Obiettivi nel menu principale. </p>  
</td>
  </tr>
 </tbody>
</table>

*Per ulteriori informazioni, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
1. Click the **gear icon** ![](assets/gear-icon-settings.png) next to the parent goal, then click **Remove alignment**.

   ![](assets/edit-remove-alignment-350x88.png)

   The goal becomes a standalone goal and its progress no longer influences the progress of the original parent goal. 

1. (Optional) Click **Undo** in the lower-left corner of the screen if you want to revert this change and keep the goals aligned. 
1. (Optional) Add activities and results to either goals to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
-->

1. Accedere a **Obiettivi** in Workfront e fai clic sul nome di un obiettivo per aprirne la pagina.
1. Dalla pagina dell’obiettivo di un obiettivo principale, fai clic su **Indicatori di avanzamento** nel pannello a sinistra.

   ![](assets/remove-goal-alignment-from-list-unshimmed.png)

1. In **Tipo: Obiettivo** raggruppamento, seleziona un obiettivo, quindi fai clic sul pulsante **Disconnetti** icona ![](assets/disconnect-goal-to-remove-alignment-icon-unshimmed.png) nella parte superiore dell’elenco.

   Viene visualizzata la casella Disconnetti.

1. Clic **Disconnetti** per disconnettere l&#39;obiettivo selezionato dal relativo elemento padre.

   L’obiettivo diventa autonomo e non viene più elencato come indicatore di avanzamento dell’obiettivo originale. L’avanzamento dell’obiettivo disconnesso non influenza più l’avanzamento dell’obiettivo originale.

   Nell’angolo superiore destro della pagina viene visualizzato un messaggio di successo per confermare che l’obiettivo è stato disconnesso.