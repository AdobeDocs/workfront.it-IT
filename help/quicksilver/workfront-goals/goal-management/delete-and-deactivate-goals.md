---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Eliminare e disattivare gli obiettivi in Obiettivi di Adobe Workfront
description: Quando inizi a lavorare su un obiettivo e questo diventa irrilevante nell’organizzazione, ti consigliamo di disattivarlo, anziché eliminarlo. La disattivazione di un obiettivo ne mantiene le informazioni storiche e consente di riattivarlo in un secondo momento. Tuttavia, in alcuni casi, quando si elimina un obiettivo può avere senso, mantenere accurata la lista degli obiettivi.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Eliminare e disattivare gli obiettivi in Obiettivi di Adobe Workfront

Quando inizi a lavorare su un obiettivo e questo diventa irrilevante nell’organizzazione, ti consigliamo di disattivarlo, anziché eliminarlo. La disattivazione di un obiettivo ne mantiene le informazioni storiche e consente di riattivarlo in un secondo momento. Tuttavia, in alcuni casi, quando si elimina un obiettivo può avere senso, mantenere accurata la lista degli obiettivi.

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

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario disporre dei seguenti elementi prima di poter iniziare:

* Modello di layout che include l’area Obiettivi del menu principale.

## Disattivazione degli obiettivi

Puoi disattivare un obiettivo che non è più rilevante e che potrebbe essere necessario riattivare in futuro.

* [Considerazioni sulla disattivazione degli obiettivi](#considerations-when-deactivating-goals)
* [Disattivazione degli obiettivi](#deactivate-goals)

### Considerazioni sulla disattivazione degli obiettivi

Quando si disattivano gli obiettivi, tieni presente quanto segue:

* È possibile disattivare solo gli obiettivi in uno stato Attivo. Per informazioni sull&#39;attivazione di un obiettivo, vedi [Attivare gli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

   >[!TIP]
   >
   >Non è possibile disattivare gli obiettivi in uno stato Bozza.

* Workfront smette di calcolare l’avanzamento degli obiettivi disattivati.
* Gli obiettivi inattivi non vengono più visualizzati o vengono presi in considerazione nella sezione Grafici degli obiettivi di Workfront. Per informazioni sui grafici degli obiettivi di Workfront, vedi [Esamina i grafici per comprendere le tendenze di avanzamento degli obiettivi negli obiettivi di Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

   <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* Non è più possibile eseguire aggiornamenti sugli obiettivi disattivati.
* È possibile modificare le informazioni sull’obiettivo e il relativo allineamento.
* È possibile riattivare un obiettivo precedentemente disattivato.

### Disattivazione degli obiettivi

<!--
Deactivating goals differs depending on which environment you use.

### Deactivate goals in the Production environment


1. Go to the goal that you want to deactivate.

   For example, go to the Goal List and click the name of a goal.

   The Goal Details panel opens on the right.

   >[!TIP]
   >
   >You can open goals from any sections of Workfront Goals.

1. Click the **More icon** ![](assets/more-icon.png), then click **Deactivate**.

   ![](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell&#39;angolo in alto a destra, quindi fai clic su **Obiettivi**.

   Viene visualizzato l’elenco degli obiettivi.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Facoltativo) Modifica i filtri per visualizzare solo gli obiettivi attivi.

   Per informazioni sul filtro delle informazioni negli obiettivi di Workfront, vedi [Filtrare le informazioni negli obiettivi di Adobe Workfront](../goal-management/filter-information-wf-goals.md).

1. Fai clic su un obiettivo attivo.

   Viene visualizzata la pagina dell’obiettivo.

   ![](assets/goal-page-unshimmed.png)

1. Fai clic sul pulsante **Altro** menu ![](assets/more-icon.png) a destra del nome dell&#39;obiettivo, quindi fai clic su **Disattiva**.

1. L&#39;obiettivo viene disattivato e il suo stato diventa Inattivo.

## Eliminare gli obiettivi

Puoi eliminare gli obiettivi che non sono più rilevanti o che potrebbero non essere mai rilevanti.

* [Considerazioni sull&#39;eliminazione degli obiettivi](#considerations-when-deleting-goals)
* [Eliminare gli obiettivi](#delete-goals)

### Considerazioni sull&#39;eliminazione degli obiettivi {#considerations-when-deleting-goals}

* Puoi eliminare gli obiettivi in qualsiasi stato, inclusi gli obiettivi chiusi.
* Non è possibile recuperare gli obiettivi eliminati.
* Vengono inoltre eliminate le attività della barra di avanzamento dei risultati e manuale collegate all’obiettivo.
* I progetti associati agli obiettivi non vengono eliminati, ma la loro associazione all’obiettivo viene rimossa.

### Eliminare gli obiettivi

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![](assets/more-icon.png), then click **Delete**.

   ![](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon.png) nell&#39;angolo in alto a destra, quindi fai clic su **Obiettivi**.

   Viene visualizzato l’elenco degli obiettivi.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Fai clic sul nome di un obiettivo. Viene visualizzata la pagina dell’obiettivo.
1. Fai clic sul pulsante **Altro** menu ![](assets/more-icon.png) a destra del nome dell&#39;obiettivo, quindi fai clic su **Elimina obiettivo**, quindi **Elimina**.

   Anche l’obiettivo e le sue attività e i suoi risultati vengono eliminati e non possono essere recuperati. I progetti associati all’obiettivo o agli obiettivi figlio non vengono eliminati.


