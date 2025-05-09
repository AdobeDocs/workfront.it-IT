---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Eliminare e disattivare gli obiettivi in Obiettivi di Adobe Workfront
description: Quando inizi a lavorare su un obiettivo che diventa irrilevante nell’organizzazione, ti consigliamo di disattivarlo, invece di eliminarlo. La disattivazione di un obiettivo mantiene le informazioni storiche e consente di riattivarlo in un secondo momento. Tuttavia, in alcuni casi può essere utile eliminare un obiettivo per mantenerne accurato l’elenco.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# Eliminare e disattivare gli obiettivi in Obiettivi di Adobe Workfront

<!--Audited for P&P only: 4/2025-->

Quando inizi a lavorare su un obiettivo che diventa irrilevante nell’organizzazione, ti consigliamo di disattivarlo, invece di eliminarlo. La disattivazione di un obiettivo mantiene le informazioni storiche e consente di riattivarlo in un secondo momento. Tuttavia, in alcuni casi può essere utile eliminare un obiettivo per mantenerne accurato l’elenco.

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
  <p> Nuovo requisito prodotto: Workfront</p>
 <p>Oppure</p>
  <p>Requisiti attuali del prodotto: oltre a una licenza Workfront, è necessario acquistare una licenza per gli obiettivi Adobe Workfront. </p> <p>Per informazioni, vedere <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisiti per l'utilizzo degli obiettivi di Workfront</a>. </p> </td>
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
   <td role="rowheader"><p>Modello layout</p></td>
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l’area Obiettivi nel menu principale. </p>  
</td>
  </tr>
</tbody>
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Disattiva obiettivi

Puoi disattivare un obiettivo che non è più pertinente e che potresti voler riattivare in futuro.

* [Considerazioni durante la disattivazione degli obiettivi](#considerations-when-deactivating-goals)
* [Disattiva obiettivi](#deactivate-goals)

### Considerazioni durante la disattivazione degli obiettivi

Durante la disattivazione degli obiettivi, tieni presente quanto segue:

* È possibile disattivare solo gli obiettivi in stato Attivo. Per informazioni sull&#39;attivazione di un obiettivo, vedere [Attivare gli obiettivi negli Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

  >[!TIP]
  >
  >Impossibile disattivare gli obiettivi in stato Bozza.

* Workfront non calcola più l’avanzamento degli obiettivi disattivati.
* Gli obiettivi inattivi non vengono più visualizzati o vengono presi in considerazione nella sezione Grafici degli Obiettivi di Workfront. Per informazioni sui grafici degli obiettivi di Workfront, consulta [Rivedere i grafici per comprendere le tendenze di avanzamento degli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

  <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* Non è più possibile apportare aggiornamenti agli obiettivi disattivati.
* Puoi modificare le informazioni sull’obiettivo e sul relativo allineamento.
* Puoi riattivare un obiettivo precedentemente disattivato.

### Disattiva obiettivi

<!--
Deactivating goals differs depending on which environment you use.

### Deactivate goals in the Production environment


1. Go to the goal that you want to deactivate.

   For example, go to the Goal List and click the name of a goal.

   The Goal Details panel opens on the right.

   >[!TIP]
   >
   >You can open goals from any sections of Workfront Goals.

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Deactivate**.

   ![Deactivate goal](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **Goals**.

   Viene visualizzato l’elenco degli obiettivi.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Facoltativo) Modifica i filtri per visualizzare solo gli obiettivi attivi.

   Per informazioni sul filtro delle informazioni negli Obiettivi di Workfront, vedi [Filtrare le informazioni negli Obiettivi di Adobe Workfront](../goal-management/filter-information-wf-goals.md).

1. Fai clic su un obiettivo attivo.

   Viene visualizzata la pagina dell’obiettivo.

   ![Pagina obiettivo](assets/goal-page-unshimmed.png)

1. Fai clic sul menu **Altro** ![Icona Altro](assets/more-icon.png) a destra del nome dell&#39;obiettivo, quindi fai clic su **Disattiva**.

1. L’obiettivo viene disattivato e il suo stato diventa Inattivo.

## Elimina obiettivi

Puoi eliminare obiettivi che non sono più rilevanti o che potrebbero non esserlo più.

* [Considerazioni durante l&#39;eliminazione degli obiettivi](#considerations-when-deleting-goals)
* [Elimina obiettivi](#delete-goals)

### Considerazioni durante l’eliminazione degli obiettivi {#considerations-when-deleting-goals}

* Puoi eliminare gli obiettivi in qualsiasi stato, compresi quelli chiusi.
* Non puoi recuperare gli obiettivi eliminati.
* Vengono eliminate anche le attività dei risultati e le attività della barra di avanzamento manuale associate all’obiettivo.
* I progetti associati agli obiettivi non vengono eliminati, ma la loro associazione con l’obiettivo viene rimossa.

### Elimina obiettivi

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Delete**.

   ![Delete goal](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. Fai clic sull&#39;icona del menu principale ![icona del menu principale](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **Obiettivi**.

   Viene visualizzato l’elenco degli obiettivi.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Fai clic sul nome di un obiettivo. Viene visualizzata la pagina dell’obiettivo.
1. Fai clic sul menu **Altro** ![Icona Altro](assets/more-icon.png) a destra del nome dell&#39;obiettivo, quindi fai clic su **Elimina obiettivo**, quindi su **Elimina**.

   Anche l’obiettivo e le relative attività e risultati vengono eliminati e non possono essere recuperati. I progetti associati all’obiettivo o agli obiettivi secondari non vengono eliminati.


