---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Eliminare e disattivare gli obiettivi in Obiettivi di Adobe Workfront
description: Quando inizi a lavorare su un obiettivo che diventa irrilevante nell’organizzazione, ti consigliamo di disattivarlo, invece di eliminarlo. La disattivazione di un obiettivo mantiene le informazioni storiche e consente di riattivarlo in un secondo momento. Tuttavia, in alcuni casi può essere utile eliminare un obiettivo per mantenerne accurato l’elenco.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 3%

---

# Eliminare e disattivare gli obiettivi in Obiettivi di Adobe Workfront

<!--Audited for P&P only: 10/2025-->

Quando inizi a lavorare su un obiettivo che diventa irrilevante nell’organizzazione, ti consigliamo di disattivarlo, invece di eliminarlo. La disattivazione di un obiettivo mantiene le informazioni storiche e consente di riattivarlo in un secondo momento. Tuttavia, in alcuni casi può essere utile eliminare un obiettivo per mantenerne accurato l’elenco.

## Requisiti di accesso

>[!NOTE]
>
>La tua azienda potrebbe scegliere di continuare a utilizzare gli obiettivi di Adobe Workfront se ha acquistato questo pacchetto in passato. Per ulteriori dettagli, rivolgiti al rappresentante del tuo account.
>
>Adobe Workfront Goals non è più disponibile per l’acquisto.

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

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
 <td role="rowheader">Licenza Adobe Workfront</td>
 <td>
 <p>Collaboratore o versione successiva</p>
<p>Richiedi o superiore</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configurazione del livello di accesso</td>
 <td> <p>Modifica accesso agli obiettivi</p> </td>
 </tr>
 <tr data-mc-conditions="">
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

{{step1-to-goals}}

Viene visualizzato l’elenco degli obiettivi.


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

{{step1-to-goals}}

Viene visualizzato l’elenco degli obiettivi.

1. Fai clic sul nome di un obiettivo. Viene visualizzata la pagina dell’obiettivo.
1. Fai clic sul menu **Altro** ![Icona Altro](assets/more-icon.png) a destra del nome dell&#39;obiettivo, quindi fai clic su **Elimina obiettivo**, quindi su **Elimina**.

   Anche l’obiettivo e le relative attività e risultati vengono eliminati e non possono essere recuperati. I progetti associati all’obiettivo o agli obiettivi secondari non vengono eliminati.


