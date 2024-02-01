---
title: Creare tipi di record di tassonomia
description: Le tassonomie sono un tipo di tipi di record riutilizzabili che acquisisce attributi relativi a un tipo di record operativo in Adobe Workfront Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Creare tipi di record di tassonomia

{{maestro-important-intro}}

Le tassonomie sono tipi di record che acquisiscono attributi sui tipi di record operativi in Adobe Maestro.

Ad esempio, Campaign può essere un tipo di record operativo. Di seguito sono riportate le tassonomie che acquisiscono gli attributi relativi al tipo di record Campaign: Area geografica, Pubblico, Paese.

Per ulteriori informazioni sui tipi di record Maestro, vedi [Panoramica dei tipi di record e delle tassonomie](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <p> Adobe Workfront</p> <p>Per collegare i tipi di record Maestro a Experience Manager Assets, devi disporre di una licenza Adobe Experience Manager Assets e l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Business Platform o Adobe Admin Console.</p> </td>
  </tr>  
 <td role="rowheader"><p>Contratto Adobe Workfront</p></td>
   <td>
<p>La tua organizzazione deve essere iscritta al programma beta chiuso Adobe Maestro. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
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
   <td> <p>Non ci sono controlli del livello di accesso per Maestro</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L’amministratore del Workfront o del gruppo deve aggiungere l’area Maestro nel modello di layout. Per informazioni, consulta <a href="../access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestire le autorizzazioni per un’area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considerazioni sulla creazione di tassonomie

* È necessario creare un&#39;area di lavoro prima di poter creare tassonomie nell&#39;area di lavoro.

  Per informazioni sulle aree di lavoro, consulta [Creare aree di lavoro](../architecture/create-workspaces.md).
* È possibile creare un tipo di record di tassonomia eseguendo una delle operazioni seguenti:
   * Creali automaticamente quando crei un’area di lavoro utilizzando un modello. Per informazioni, consulta [Creare aree di lavoro](../architecture/create-workspaces.md).
   * Creale manualmente, da zero.
   * Per crearli manualmente, incollare le informazioni da un elenco esterno.

  <!--this is not possible yet:
  * You can taxonomies to a workspace by doing one of the following:
    * Create a connection to object types from other systems, when adding fields to a taxnomy record type. This creates a read-only record type in Maestro.  - update this sentence when you can connect taxonomies as well as operational records to a third-party system.-->

* Tutte le tassonomie create di recente sono disponibili nei campi seguenti:

   * Nome <!--if there won't be any more fields, consider rephrasing this-->

  È inoltre possibile aggiungere campi personalizzati alle tassonomie. Per ulteriori informazioni, consulta [Crea campi](../fields/create-fields.md).

  >[!NOTE]
  >
  >    Le tassonomie create quando si utilizza un modello di area di lavoro dispongono di campi aggiuntivi.

## Creare una tassonomia

La creazione di tassonomie è simile alla creazione di un tipo di record operativo da zero o da un modello di workspace.

Per informazioni, vedere la sezione &quot;Creare un tipo di record da zero&quot; nell&#39;articolo [Crea tipi di record](../architecture/create-record-types.md).

Per informazioni sulla creazione automatica di tassonomie durante la creazione di un&#39;area di lavoro da un modello, vedere [Creare aree di lavoro](../architecture/create-workspaces.md).
