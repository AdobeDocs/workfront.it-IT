---
title: Add Existing Record Types from Another Workspace
description: I tipi di record sono i tipi di oggetto di Adobe Workfront Planning. In Workfront Planning è possibile aggiungere un tipo di record esistente creato in un'altra area di lavoro.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 2%

---


# Aggiungere tipi di record esistenti da un’altra area di lavoro

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

In qualità di responsabile dell&#39;area di lavoro, è possibile aggiungere un tipo di record esistente in un&#39;altra area di lavoro a un&#39;area di lavoro gestita in Adobe Workfront Planning.

A workspace manager must first designate a record type as a global record type before you can add it into workspaces you manage as an existing record type. Workspace managers can designate a record type as global when they create or edit them, by defining the record type&#39;s cross-workspace settings.

Per informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

This article describes how you can add a record type from an existing one.

Before adding records to a workspace from a global record type, also see the article [Cross-workspace record types overview](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<ul><li><p>Qualsiasi pacchetto Workfront e un pacchetto Planning Plus</p></li>
Oppure
<li><p>Qualsiasi flusso di lavoro e un pacchetto Planning Prime o Ultimate</p></p></li></ul>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--
Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 

  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul><li><p>Any Workfront package</p></li>
<p>And</p>
<li><p>Any Planning package to create connectable record types</p></li>
<li><p>A Planning Plus package to create global record types</p></li>
</ul>
Or:
<ul><li><p>A Prime or Ultimate Workflow package</p> </li>
And
<li><p>A Planning Prime or Ultimate package</p></li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 

  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and to the record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table>
-->

## Creare un tipo di record aggiungendo un record esistente da un&#39;altra area di lavoro

>[!NOTE]
>
>Verificare che in almeno un&#39;altra area di lavoro principale sia presente almeno un tipo di record designato come globale.
>
>Per informazioni, vedere [Configurare le funzionalità tra aree di lavoro diverse per i tipi di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

1. Passare a un&#39;area di lavoro in cui si desidera creare un tipo di record (area di lavoro secondaria).
1. Inizia a creare un tipo di record come descritto nell&#39;articolo [Crea tipi di record](/help/quicksilver/planning/architecture/create-record-types.md), quindi fai clic su **Aggiungi esistente**. <!--check this - the option might have been renamed in the UI-->

   ![Modal to add record type with option to add from another workspace](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >When there are no record types configured to be added to other workspaces in your system, the **Add existing** option does not display.

1. Fai clic su **Continue** (Continua).
1. In the **Choose the record type** box, click the card for the record type that you want to add from an existing workspace, then click **Add**.

   The record type is added to the secondary workspace that you selected and the **global record type** icon ![Global record icon on the secondary workspace](assets/global-icon-secondary-workspace.png) displays on the record type&#39;s card.
The global record type icon includes an arrow when displayed on a record type in the secondary workspace, to indicate that the record type was added from an existing record type.

   The following things occur:

   * The following information is also added from the existing global record type:

      * Tutti i campi originali
      * Tutte le connessioni record
   * Non è possibile visualizzare i record aggiunti dall&#39;area di lavoro originale del tipo di record dall&#39;area di lavoro secondaria.
   * You can view records added from the original workspace of the record type in that workspace, only in the original workspace, if you have at least View permissions to that workspace.
   * The read-only **Workspace** field is added to the new record type table view. The field displays the workspace where each record was created.

     >[!NOTE]
     >
     >You cannot edit the new record type&#39;s appearance, additional settings, or original fields. You can edit the record type and all its original fields and settings only from the original workspace.
     >

1. (Optional) Hover over the global record type icon ![Global record icon on the secondary workspace](assets/global-icon-secondary-workspace.png) to view the name of the original workspace where the record type was added from.
1. (Optional) Click, then drag and drop the newly added record type to any section within the workspace.
1. (Optional) Click the **More** menu on the new record type&#39;s card or to the right of the record type name on its page, then click one of the following:

   * **Condividi** per condividere il tipo di record dall&#39;area di lavoro secondaria.
   * **Elimina** per eliminare il tipo di record dall&#39;area di lavoro secondaria. L&#39;eliminazione dei tipi di record dall&#39;area di lavoro secondaria comporta anche l&#39;eliminazione dei record aggiunti dall&#39;area di lavoro secondaria.

     Le viste aggiunte dall&#39;area di lavoro secondaria non vengono eliminate. <!--checking with Lilit - not sure if this is by design??-->

   Per ulteriori informazioni, vedere la sezione &quot;Eliminare tipi di record globali&quot; nell&#39;articolo [Eliminare tipi di record](/help/quicksilver/planning/architecture/delete-record-types.md).

<!--
This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

&lt;!—verificare con Lilit se è possibile aggiungere automazioni o moduli di richiesta a RT globali secondari??—aggiungere un passaggio con collegamenti a tali articoli se/quando sì—>







