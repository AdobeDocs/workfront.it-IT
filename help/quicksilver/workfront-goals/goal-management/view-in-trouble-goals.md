---
product-previous: workfront-goals
navigation-topic: goal-management
title: Rivedere gli obiettivi nei guai negli obiettivi di Adobe Workfront
description: Gli obiettivi con avanzamento nei problemi rischiano di non essere raggiunti e sono rappresentati da una barra di avanzamento rossa negli obiettivi di Adobe Workfront. Devi rivedere spesso i tuoi obiettivi e capire perché i progressi sono in ritardo.
author: Alina
feature: Workfront Goals
exl-id: df2cdc12-9102-4759-9daa-1f8ae68f110b
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Rivedere gli obiettivi nei guai negli obiettivi di Adobe Workfront

<!--
<p>(NOTE: the status of goals in "red" used to be called At Risk. Now, it is "in trouble") </p>
-->

Gli obiettivi con avanzamento nei problemi rischiano di non essere raggiunti e sono rappresentati da una barra di avanzamento rossa negli obiettivi di Adobe Workfront. Devi rivedere spesso i tuoi obiettivi e capire perché i progressi sono in ritardo. Per informazioni sull&#39;avanzamento dell&#39;obiettivo, vedi [Panoramica dell’avanzamento e della condizione dell’obiettivo in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/calculate-goal-progress.md).

## Requisiti di accesso

<!--drafted for P&P release: replace the existing requirements with this:

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

## Recommendations per impedire che gli obiettivi raggiungano un progresso di In Trouble

Prima che gli obiettivi raggiungano un progresso di In Trouble, è possibile monitorarli spesso e modificarne il progresso quando raggiungono un progresso di At Risk. Gli obiettivi a rischio rischiano di finire nei guai. Per ulteriori informazioni sull’avanzamento dell’obiettivo, consulta [Panoramica dell’avanzamento e della condizione dell’obiettivo in Obiettivi di Adobe Workfront](../../workfront-goals/goal-management/calculate-goal-progress.md)

Prima che i tuoi obiettivi raggiungano un progresso di In Trouble, ti consigliamo quanto segue:

* Rivedi gli obiettivi che presentano una condizione di A rischio spesso assegnata a te e gli obiettivi organizzativi assegnati ai tuoi team, gruppi o alla tua organizzazione che potrebbero essere influenzati dall’avanzamento dei tuoi obiettivi. Gli obiettivi a rischio rischiano di diventare obiettivi in difficoltà. Gli obiettivi a rischio sono contrassegnati da una barra di avanzamento gialla. Utilizza l’Elenco obiettivi per visualizzare gli obiettivi che appartengono a te, ai tuoi team, gruppi o alla tua organizzazione.


## Rivedere gli obiettivi in difficoltà nella Lista obiettivi

Puoi rivedere gli obiettivi in qualsiasi sezione degli obiettivi di Workfront. Per informazioni sulle sezioni Obiettivi di Workfront, vedi [Panoramica delle sezioni Obiettivi di Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

Questo articolo descrive come rivedere gli obiettivi nell&#39;Elenco obiettivi.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) > **Obiettivi** nell&#39;angolo in alto a destra.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Viene visualizzata l’area Obiettivi di Workfront e per impostazione predefinita la sezione Elenco obiettivi .

1. (Consigliato) Per modificare gli obiettivi a rischio, regola i seguenti filtri per l’area Elenco obiettivi:

   * Fai clic su **Azienda**, quindi **I miei team**, quindi **Gruppi personali**, quindi **Personale** in questo modo puoi visualizzare gli obiettivi che appartengono alla tua organizzazione, i tuoi team, gruppi e quindi i tuoi obiettivi.

      >[!TIP]
      >
      >In Obiettivi di Adobe Workfront, il filtro Azienda visualizza gli obiettivi per i quali la tua organizzazione è selezionata come proprietario.
      >
      >
      >Non è possibile cercare le aziende che utilizzano questo campo. Per impostazione predefinita viene selezionata solo l’organizzazione proprietaria dell’istanza Workfront.

   * Per ciascuna delle unità organizzative selezionate in precedenza, fai clic su **Nuovo filtro** > **Avanzamento** > **In problemi** >**Applica.**
   * (Facoltativo) Seleziona il periodo di tempo per il quale visualizzare gli obiettivi.

      L’indicatore della barra di avanzamento viene visualizzato in rosso per ciascun obiettivo nell’elenco degli obiettivi.

      Per ulteriori informazioni sul filtro degli obiettivi utilizzando tutti gli altri criteri nel pannello di destra, consulta [Filtrare le informazioni negli obiettivi di Adobe Workfront](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. Passa il cursore del mouse sull’indicatore della barra di avanzamento per visualizzare la percentuale di avanzamento effettiva e il valore previsto per il giorno corrente.

   ![](assets/goal-progress-hover-over-detail-unshimmed.png)

1. (Facoltativo) Utilizza i filtri per trovare gli obiettivi che appartengono a un proprietario specifico.

   Gli obiettivi nei guai per gli utenti selezionati vengono visualizzati nell’elenco degli obiettivi.

1. Fai clic sul nome di un obiettivo per aprire la pagina dell’obiettivo, quindi fai clic su **Indicatori di avanzamento** nel pannello a sinistra. Visualizzare quale indicatore di avanzamento causa il ritardo dell&#39;obiettivo e aggiornare l&#39;avanzamento dell&#39;indicatore in linea, nella **Avanzamento effettivo** colonna dell&#39;elenco degli indicatori di avanzamento.

   Per informazioni sull&#39;aggiornamento dei risultati e delle attività, vedi [Aggiornare lo stato dell’obiettivo negli obiettivi di Adobe Workfront](../goal-review-and-workfront-goals-sections/check-in-goals.md)

   ![](assets/actual-progress-editable-column-in-indicator-list-unshimmed.png)

   >[!NOTE]
   >
   >È possibile aggiornare solo i risultati e le attività nell&#39;elenco degli indicatori di avanzamento. È necessario aggiornare gli indicatori di avanzamento degli obiettivi figlio accedendo agli obiettivi e aggiornare le attività relative ai progetti collegati per aggiornare lo stato di avanzamento dei progetti.


