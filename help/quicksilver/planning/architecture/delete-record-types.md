---
title: Elimina tipi di record
description: È possibile eliminare i tipi di record quando non sono più rilevanti. L'eliminazione dei tipi di record comporta anche l'eliminazione di tutte le informazioni associate ai tipi di record, ad esempio record, campi e visualizzazioni.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 2%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:
---
title: Delete record types
description: You can delete record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# Elimina tipi di record

{{planning-important-intro}}

È possibile eliminare i tipi di record quando non sono più rilevanti.

Tuttavia, l&#39;eliminazione dei tipi di record comporta anche l&#39;eliminazione di tutte le informazioni associate ai tipi di record. Per ulteriori informazioni, vedere [Considerazioni durante l’eliminazione dei tipi di record](#considerations-when-deleting-record-types) in questo articolo.

Per informazioni sui tipi di record, vedere [Panoramica sui tipi di record](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Prodotto</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>L'organizzazione deve essere iscritta alla fase di accesso anticipato per Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>piano Adobe Workfront</p></td>
   <td>
<p>Qualsiasi</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td>
   <td>
   <p>Qualsiasi</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td>
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestire le autorizzazioni per un’area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L'amministratore del Workfront o del gruppo deve aggiungere l'area Planning nel modello di layout. Per informazioni, consulta <a href="/help/quicksilver/planning/access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considerazioni durante l’eliminazione dei tipi di record

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* È possibile eliminare solo i tipi di record dalle aree di lavoro per le quali si dispone delle autorizzazioni Gestione.
* L&#39;eliminazione dei tipi di record comporta la rimozione delle seguenti informazioni ad essi associate:

   * Tutti i record di quel tipo.
   * Tutti i campi associati al tipo di record.
   * Tutte le visualizzazioni (inclusi filtri, raggruppamenti e criteri di ordinamento) del tipo di record.
* Il tipo di record viene rimosso da tutti gli utenti che accedono all’area di lavoro.
* Non è possibile recuperare i tipi di record eliminati o le relative informazioni.
* È consigliabile ricreare i campi e i record associati al tipo di record che si desidera eliminare in un altro tipo di record prima di eliminarli.

## Elimina tipi di record

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera eliminare i tipi di record.

   Oppure

   Da un workspace, espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente e selezionare il workspace dal quale si desidera eliminare i tipi di record.

   Viene aperto il workspace e vengono visualizzati i tipi di record.
1. Esegui una delle operazioni seguenti:

   * Passa il puntatore del mouse sulla scheda del tipo di record, fai clic sul menu Altro, quindi **Elimina**.
   * Fare clic sulla scheda del tipo di record che si desidera eliminare e nella pagina del tipo di record fare clic su **Altro** menu ![](assets/more-menu.png) a destra del nome del tipo di record, quindi fare clic su **Elimina**.

   ![](assets/permanently-delete-record-type-confirmation.png)

1. Tipo **eliminare** nella casella di conferma, fai clic su **Elimina definitivamente**. Non fa distinzione tra maiuscole e minuscole.

   Il tipo di record selezionato e i relativi campi, record associati e viste vengono eliminati.
