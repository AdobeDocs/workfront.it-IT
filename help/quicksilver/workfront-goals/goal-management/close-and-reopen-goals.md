---
product-previous: workfront-goals
navigation-topic: goal-management
title: Chiudere e riaprire Obiettivi in Obiettivi di Adobe Workfront
description: È possibile chiudere un obiettivo quando si desidera indicare che è stato completato o che non si sta più lavorando su di esso perché è diventato obsoleto.
author: Alina
feature: Workfront Goals
exl-id: bbb549c1-aea6-4f5e-8a6b-01fc04cf06ef
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 0%

---

# Chiudere e riaprire gli obiettivi in Obiettivi di Adobe Workfront

<!--Audited for P&P only: 4/2025-->

È possibile chiudere un obiettivo quando si desidera indicare quanto segue:

* L’obiettivo viene raggiunto perché l’hai raggiunto o perché è trascorso il periodo di tempo.
* Non ci state più lavorando, né prevedete di farlo nell&#39;immediato futuro.

Puoi riaprire gli obiettivi che sono stati chiusi quando diventano di nuovo rilevanti.

## Requisiti di accesso

>[!NOTE]
>
>La tua azienda potrebbe scegliere di continuare a utilizzare gli obiettivi di Adobe Workfront se ha acquistato questo pacchetto in passato. Per ulteriori dettagli, rivolgiti al rappresentante del tuo account.
>
>Adobe Workfront Goals non è più disponibile per l’acquisto.

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

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
 <tr>
 <td role="rowheader">Licenza Adobe Workfront</td>
 <td>
 <p>Collaboratore o versione successiva</p>
 <p>Richiedi o superiore</p></td>
 </tr>
 <td role="rowheader">Configurazione del livello di accesso</td>
 <td> <p>Modifica accesso agli obiettivi</p> </td>
 </tr>
 <tr>
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

## Considerazioni per la chiusura o la riapertura degli obiettivi

* Per poter chiudere e riaprire gli obiettivi, è necessario disporre dell&#39;accesso Modifica obiettivi nel proprio livello di accesso. Per informazioni sulla concessione dell&#39;accesso agli obiettivi, vedere [Concedere l&#39;accesso agli obiettivi di Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).
* È possibile chiudere solo gli obiettivi attivi. Non è possibile chiudere gli obiettivi in stato Bozza.

  Per informazioni sugli stati degli obiettivi, vedere [Panoramica sullo stato degli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/goal-status-overview.md).

* La chiusura degli obiettivi si blocca nel suo avanzamento e consente di valutare il livello di successo ottenuto nel realizzarlo.

  >[!CAUTION]
  >
  >Quando si chiude un obiettivo con obiettivi attivi, l’avanzamento cambia dopo la chiusura per indicare l’avanzamento degli obiettivi attivi che contribuiscono. Per informazioni sull&#39;allineamento degli obiettivi, vedere [Allineare gli obiettivi collegandoli in Obiettivi di Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

* Aggiorna gli indicatori di avanzamento dell’obiettivo prima di chiuderlo, in modo che l’obiettivo venga chiuso con un valore di avanzamento accurato. Se tutti gli indicatori di progresso sono stati raggiunti, l&#39;obiettivo percentuale di completamento dovrebbe essere 100% e l&#39;obiettivo è stato raggiunto. Per informazioni sull&#39;aggiornamento degli obiettivi, vedere [Aggiornare lo stato di avanzamento degli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).
* Lascia eventuali commenti finali come aggiornamento degli obiettivi che chiudi. Per informazioni sull&#39;aggiunta di commenti agli obiettivi, vedere [Gestire i commenti degli obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/manage-goal-comments.md).
* Non puoi più aggiornare l’avanzamento dei risultati e delle attività in base a un obiettivo che hai chiuso.
* Puoi riaprire un obiettivo chiuso se desideri continuare a lavorarci.
* Se l’obiettivo non è stato raggiunto, è consigliabile copiare la maggior parte delle informazioni nel periodo di tempo successivo (trimestre o anno). Questa è un’ottima opzione per obiettivi che sono gli stessi da un periodo di tempo all’altro o per obiettivi che potresti dover ancora lavorare per raggiungere nel prossimo periodo di tempo. Per informazioni sulla copia degli obiettivi, vedi [Copia obiettivi in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/copy-goals.md). Puoi anche aggiornare il periodo di tempo sull’obiettivo invece di copiarlo in un altro periodo.
* Workfront elimina i commenti di un obiettivo chiuso quando lo riapri. Se devi conservare i commenti, ti consigliamo di copiare l’obiettivo chiuso, inclusi eventuali risultati associati, anziché riaprirlo.


## Chiudi obiettivi

<!--
Closing goals differs depending on what environment you use. 

### Close goals in the Production environment

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are active.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md). 

1. Click an active goal.

   The Goal Details panel displays on the right. 

1. (Optional and recommended) Click the **Updates** tab and add an update in the **Comment here** field about the reason you are closing the goal, then click **Post**. 

1. Click the **More icon** ![More icon](assets/more-icon.png) to the right of the goal name, then click **Close** > **Close Goal**.

   This closes the goal and saves the current progress on the goal and its results and activities.

   >[!IMPORTANT]
   >
   >If the goal has contributing goals that are still active, the progress of the goal continues to update based on the progress of the aligned goals.
   >
   >
   >![Closing goals with active aligned goals](assets/closing-goals-with-active-aligned-goals-warning-350x71.png)   >
   >

1. (Optional) Modify your filters again to display only closed goals. The goals you closed display on the screen.
-->

1. Fai clic sull&#39;icona **Menu principale** ![Icona Menu principale](assets/main-menu-icon.png) > **Obiettivi** nell&#39;angolo superiore destro.

   Viene visualizzato Elenco obiettivi (Goal List).

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Facoltativo) Modifica i filtri per visualizzare solo gli obiettivi attivi.

   Per informazioni sul filtro delle informazioni negli Obiettivi di Workfront, vedi [Filtrare le informazioni negli Obiettivi di Adobe Workfront](../goal-management/filter-information-wf-goals.md).
1. Fai clic su un obiettivo attivo.

   Viene visualizzata la pagina dell’obiettivo.

   ![Pagina obiettivo](assets/goal-page-unshimmed.png)
1. Fai clic sul menu **Altro** ![Icona Altro](assets/more-icon.png) a destra del nome dell&#39;obiettivo, quindi fai clic su **Chiudi**.

   L’obiettivo si chiude e ricevi una conferma nell’angolo in alto a destra dello schermo.

   ![Conferma chiusura obiettivo](assets/goal-close-confirmation-with-add-closing-notes-link.png)

1. (Facoltativo) Nella casella di conferma, fare clic su **Aggiungi note di chiusura** per aggiungere commenti su questo obiettivo e sul motivo per cui è necessario chiuderlo.
1. Aggiungi note di chiusura, quindi fai clic su **Aggiungi note**.

   ![Aggiungi note di chiusura](assets/add-closing-notes-box-unshimmed.png)

   I commenti vengono visualizzati nella sezione Dettagli obiettivo della pagina dell&#39;obiettivo, nell&#39;area Note di chiusura.

   >[!NOTE]
   >
   >Workfront elimina le note di chiusura se successivamente riapri un obiettivo chiuso.


## Riapri obiettivi

Puoi riaprire gli obiettivi chiusi se decidi che sono diventati di nuovo rilevanti e che devi continuare ad aggiornare il loro avanzamento.

<!--
Reopening goals differs depending on what environment you use.

### Reopen goals in the Production environment

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are closed.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).


1. Click a closed goal.

   This opens the Goal Details panel on the right. 

1. Click the **More icon** ![More icon](assets/more-icon.png) to the right of the goal name, then click **Reopen** > **Reopen**.

   This reopens the goal and places it in a status of Active. The progress of the goal is recalculated starting with the current date. 

1. (Optional) Modify your filters again to display only active goals. The goals you opened display on the screen.

-->

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png)> **Goals** nell&#39;angolo superiore destro.

   Viene visualizzato Elenco obiettivi (Goal List).

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Facoltativo) Modifica i filtri per visualizzare solo gli obiettivi chiusi.

   Per informazioni sul filtro delle informazioni negli Obiettivi di Workfront, vedi [Filtrare le informazioni negli Obiettivi di Adobe Workfront](../goal-management/filter-information-wf-goals.md).
1. Fai clic sul nome di un obiettivo chiuso.

   Viene visualizzata la pagina dell’obiettivo.
1. Fai clic sul menu **Altro** ![Icona Altro](assets/more-icon.png) a destra del nome dell&#39;obiettivo, quindi **Riapri** > **Riapri**.

   Si verificano le seguenti situazioni:
   * L’obiettivo è ora aperto e ha lo stato Attivo.
   * L’avanzamento dell’obiettivo viene ricalcolato a partire dalla data corrente.
   * Tutte le note di chiusura vengono eliminate dalla pagina dei dettagli Obiettivo. Non è possibile recuperare le note di chiusura eliminate.

1. (Facoltativo) Modifica nuovamente i filtri per visualizzare solo gli obiettivi attivi.

   Gli obiettivi aperti vengono visualizzati sullo schermo.

