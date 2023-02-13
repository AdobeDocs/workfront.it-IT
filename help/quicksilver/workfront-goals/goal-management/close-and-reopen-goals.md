---
product-previous: workfront-goals
navigation-topic: goal-management
title: Chiudere e riaprire gli obiettivi in Obiettivi di Adobe Workfront
description: È possibile chiudere un obiettivo quando si desidera indicare che è stato completato o che non si sta più lavorando su di esso perché è diventato obsoleto.
author: Alina
feature: Workfront Goals
exl-id: bbb549c1-aea6-4f5e-8a6b-01fc04cf06ef
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Chiudere e riaprire gli obiettivi in Obiettivi di Adobe Workfront

È possibile chiudere un obiettivo quando si desidera indicare quanto segue:

* L&#39;obiettivo viene raggiunto, sia perché lo avete raggiunto, sia perché è trascorso il periodo di tempo.
* Non ci state più lavorando, né intendete farlo nell&#39;immediato futuro.

È possibile riaprire gli obiettivi che sono stati chiusi quando diventano nuovamente rilevanti.

## Requisiti di accesso

<!--drafted for P&P release: 

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

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

È necessario disporre dei seguenti elementi prima di poter iniziare:

* Modello di layout che include l’area Obiettivi del menu principale.

## Considerazioni sulla chiusura o la riapertura degli obiettivi

* Per poter chiudere e riaprire gli obiettivi, devi avere accesso a Modifica obiettivi nel livello di accesso. Per informazioni sulla concessione dell&#39;accesso agli obiettivi, vedi [Concedere l’accesso agli obiettivi di Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).
* È possibile chiudere solo gli obiettivi attivi. Non è possibile chiudere gli obiettivi che si trovano nello stato Bozza.

   Per informazioni sugli stati degli obiettivi, consulta [Panoramica sullo stato dell&#39;obiettivo negli obiettivi di Adobe Workfront](../../workfront-goals/goal-management/goal-status-overview.md).

* Gli obiettivi di chiusura si bloccano nel suo progresso e ti permette di valutare quanto bene hai fatto nel realizzarlo.

   >[!CAUTION]
   >
   >Quando si chiude un obiettivo con obiettivi attivi che contribuiscono, il suo progresso cambia dopo la chiusura per indicare il progresso degli obiettivi attivi che contribuiscono. Per informazioni sull&#39;allineamento degli obiettivi, vedi [Allineare gli obiettivi collegandoli negli obiettivi di Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

* Aggiorna gli indicatori di avanzamento dell&#39;obiettivo prima di chiudere l&#39;obiettivo per assicurarti che l&#39;obiettivo si chiuda con un preciso valore di avanzamento. Se tutti gli indicatori di progresso sono stati raggiunti, l&#39;obiettivo percentuale di completamento dovrebbe essere 100% e il vostro obiettivo è stato raggiunto. Per informazioni sull&#39;aggiornamento degli obiettivi, vedi [Aggiornare lo stato dell’obiettivo negli obiettivi di Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).
* Lascia i commenti finali come aggiornamento agli obiettivi che chiudi. Per informazioni sull’aggiunta di commenti agli obiettivi, consulta [Gestire i commenti sull’obiettivo in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/manage-goal-comments.md).
* Non puoi più aggiornare l’avanzamento dei risultati e delle attività su un obiettivo che chiudi.
* Puoi riaprire un obiettivo chiuso se desideri continuare a lavorarci.
* Se l’obiettivo non è stato raggiunto, è consigliabile copiare la maggior parte delle informazioni nel periodo di tempo successivo (trimestre o anno). Questa è una grande opzione per gli obiettivi che sono gli stessi da un periodo di tempo all&#39;altro o per gli obiettivi che potrebbe ancora essere necessario lavorare per raggiungere nel prossimo arco temporale. Per informazioni sulla copia degli obiettivi, vedi [Copia degli obiettivi negli obiettivi di Adobe Workfront](../../workfront-goals/goal-management/copy-goals.md). È inoltre possibile aggiornare il periodo di tempo sull&#39;obiettivo anziché copiarlo in un altro periodo.
* Workfront elimina i commenti di un obiettivo chiuso quando lo si riapre. Se è necessario mantenere i commenti, è consigliabile copiare l’obiettivo chiuso, compresi eventuali risultati associati, anziché riaprirlo.


## Chiudi obiettivi

<!--
Closing goals differs depending on what environment you use. 

### Close goals in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are active.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md). 

1. Click an active goal.

   The Goal Details panel displays on the right. 

1. (Optional and recommended) Click the **Updates** tab and add an update in the **Comment here** field about the reason you are closing the goal, then click **Post**. 

1. Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Close** > **Close Goal**.

   This closes the goal and saves the current progress on the goal and its results and activities.

   >[!IMPORTANT]
   >
   >If the goal has contributing goals that are still active, the progress of the goal continues to update based on the progress of the aligned goals.
   >
   >
   >![](assets/closing-goals-with-active-aligned-goals-warning-350x71.png)   >
   >

1. (Optional) Modify your filters again to display only closed goals. The goals you closed display on the screen.
-->

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) > **Obiettivi** nell&#39;angolo in alto a destra.

   Viene visualizzato l’Elenco obiettivi.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Facoltativo) Modifica i filtri per visualizzare solo gli obiettivi attivi.

   Per informazioni sul filtro delle informazioni negli obiettivi di Workfront, vedi [Filtrare le informazioni negli obiettivi di Adobe Workfront](../goal-management/filter-information-wf-goals.md).
1. Fai clic su un obiettivo attivo.

   Viene visualizzata la pagina dell’obiettivo.

   ![](assets/goal-page-unshimmed.png)
1. Fai clic sul pulsante **Altro** menu ![](assets/more-icon.png) a destra del nome dell&#39;obiettivo, quindi fai clic su **Chiudi**.

   L’obiettivo viene chiuso e viene visualizzata una conferma nell’angolo in alto a destra dello schermo.

   ![](assets/goal-close-confirmation-with-add-closing-notes-link.png)

1. (Facoltativo) Nella casella di conferma, fai clic su **Aggiungi note di chiusura** per aggiungere commenti su questo obiettivo e perché è necessario chiuderlo.
1. Aggiungi le note di chiusura, quindi fai clic su **Aggiungi note**.

   ![](assets/add-closing-notes-box-unshimmed.png)

   I commenti vengono visualizzati nella sezione Dettagli obiettivo della pagina dell’obiettivo, nell’area Note di chiusura .

   >[!NOTE]
   >
   >Workfront elimina le note di chiusura se in seguito riapri un obiettivo chiuso.


## Riapri obiettivi

È possibile riaprire gli obiettivi chiusi se si decide che sono diventati di nuovo rilevanti e che è necessario continuare ad aggiornare i loro progressi.

<!--
Reopening goals differs depending on what environment you use.

### Reopen goals in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are closed.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).


1. Click a closed goal.

   This opens the Goal Details panel on the right. 

1. Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Reopen** > **Reopen**.

   This reopens the goal and places it in a status of Active. The progress of the goal is recalculated starting with the current date. 

1. (Optional) Modify your filters again to display only active goals. The goals you opened display on the screen.

-->

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png)> **Obiettivi** nell&#39;angolo in alto a destra.

   Viene visualizzato l’Elenco obiettivi.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Facoltativo) Modifica i filtri per visualizzare solo gli obiettivi chiusi.

   Per informazioni sul filtro delle informazioni negli obiettivi di Workfront, vedi [Filtrare le informazioni negli obiettivi di Adobe Workfront](../goal-management/filter-information-wf-goals.md).
1. Fai clic sul nome di un obiettivo chiuso.

   Viene visualizzata la pagina dell’obiettivo.
1. Fai clic sul pulsante **Altro** menu ![](assets/more-icon.png) a destra del nome dell&#39;obiettivo, quindi **Riapri** > **Riapri**.

   Si verificano le seguenti situazioni:
   * L&#39;obiettivo è ora aperto e presenta lo stato Attivo.
   * L’avanzamento dell’obiettivo viene ricalcolato a partire dalla data corrente.
   * Tutte le note di chiusura vengono eliminate dalla pagina Dettagli obiettivo. Le note di chiusura eliminate non possono essere recuperate.

1. (Facoltativo) Modifica nuovamente i filtri per visualizzare solo gli obiettivi attivi.

   Gli obiettivi aperti vengono visualizzati sullo schermo.

