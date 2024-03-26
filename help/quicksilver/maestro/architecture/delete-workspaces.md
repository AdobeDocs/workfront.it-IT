---
title: Eliminare le aree di lavoro
description: È possibile eliminare le aree di lavoro quando non sono più rilevanti.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Eliminare le aree di lavoro

{{maestro-important-intro}}

Nella pianificazione di Adobe Workfront, le aree di lavoro sono posizioni centralizzate in cui i team possono pianificare il lavoro. Per ulteriori informazioni, consulta [Creare aree di lavoro](../architecture/delete-workspaces.md).

È possibile eliminare le aree di lavoro non più rilevanti.

È consigliabile ricreare alcuni o tutti i tipi di record, i record, i campi e le visualizzazioni associati all&#39;area di lavoro che si desidera eliminare in un&#39;altra area di lavoro prima di eliminarla.

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
<p>La tua organizzazione deve essere iscritta al programma beta di pianificazione di Adobe Workfront. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>piano Adobe Workfront</p></td>
   <td>
<p>Qualsiasi</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td>
   <td>
   <p>Nuovo: Standard</p>
   <p>Corrente: Piano</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td>
   <td> <p>Non sono presenti controlli del livello di accesso per la pianificazione di Adobe Workfront</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestire le autorizzazioni per un’area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>

</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L'amministratore del Workfront o del gruppo deve aggiungere l'area Planning nel modello di layout. Per informazioni, consulta <a href="../access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Per ulteriori informazioni sui requisiti di accesso, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Considerazioni sull’eliminazione delle aree di lavoro

* Quando si eliminano le aree di lavoro, vengono eliminati anche tutti i tipi di record, i record, i relativi campi e le visualizzazioni.
* Le aree di lavoro eliminate e le informazioni in esse contenute non possono essere recuperate.

## Eliminare un’area di lavoro

{{step1-to-maestro}}

Verrà aperta l&#39;ultima area di lavoro a cui si è effettuato l&#39;accesso.

1. (Facoltativo) Espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente e selezionare il workspace che si desidera eliminare.
1. Fai clic su **Altro** menu ![](assets/more-menu.png) accanto al nome dell’area di lavoro, quindi fai clic su **Elimina**.
1. Clic **Elimina** per confermare.

   L’area di lavoro viene eliminata e non può essere recuperata. Verranno eliminati anche tutti i tipi di record, i record, i campi e le visualizzazioni ad essi associati. <!--ensure this is right after closed beta-->
