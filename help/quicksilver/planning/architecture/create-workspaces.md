---
title: Creare aree di lavoro
description: Un'area di lavoro è una raccolta di tipi di record utilizzati da un team e rappresenta il ciclo di vita del lavoro del team. È possibile personalizzare completamente le aree di lavoro in Adobe Workfront Planning. I tipi di record sono organizzati per sezioni in un'area di lavoro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: f252140e4fec01c7bb8092804532d79954cef618
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Creare aree di lavoro

{{planning-important-intro}}

In Adobe Workfront Planning, le aree di lavoro sono posizioni centralizzate in cui i team possono pianificare il lavoro.

Un&#39;area di lavoro è una raccolta di tipi di record utilizzati da un team e rappresenta il ciclo di vita del lavoro del team. È possibile personalizzare completamente le aree di lavoro in Adobe Workfront Planning.

Per informazioni generali sulle aree di lavoro, vedere [Panoramica delle aree di lavoro](/help/quicksilver/planning/architecture/workspaces-overview.md).

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per Workfront Planning.

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
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td>
   <td>
   <p>Nuovo: Standard</p>
   Oppure
   <p>Corrente: Piano</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td>
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Ricevi le autorizzazioni di gestione per le aree di lavoro create. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>È necessario aggiungere l'area Planning al modello di layout. Per informazioni, vedere <a href="/help/quicksilver/planning/access/access-overview.md">Panoramica dell'accesso</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Per ulteriori informazioni sui requisiti di accesso, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Crea un’area di lavoro

È possibile creare un workspace e aggiungervi tipi di record per organizzare gli oggetti in Workfront Planning. Per ulteriori informazioni sulla modifica di un&#39;area di lavoro, vedere [Modifica aree di lavoro](/help/quicksilver/planning/architecture/edit-workspaces.md).

{{step1-to-planning}}

1. Fai clic su **Crea area di lavoro**

   Viene visualizzata la casella Crea area di lavoro. È possibile creare un&#39;area di lavoro da zero utilizzando uno dei modelli disponibili.

1. (Facoltativo e condizionale) Fare clic su **Anteprima** in uno dei seguenti modelli di area di lavoro predefiniti:

   * Base: Marketing Management
   * Avanzato: Marketing Management
   * Enterprise: Marketing Management
   * Gestione vendite
   * Gestione dei prodotti

   Viene visualizzata la casella di anteprima del modello.

   È possibile indicare i tipi di record operativi, le tassonomie e il numero di campi associati a ciascun modello.

   ![](assets/previewing-a-workspace-template.png)

   Per informazioni sui modelli di area di lavoro di Workfront Planning, vedere [Elenco dei modelli di area di lavoro](/help/quicksilver/planning/architecture/workspace-templates.md).

1. Dalla casella di anteprima del modello, fai clic su **Usa modello** per iniziare a creare l&#39;area di lavoro dal modello selezionato

   Oppure

   Fai clic su **Indietro**, quindi su **Nuova area di lavoro** per creare un&#39;area di lavoro da zero.

   Viene creato uno dei seguenti tipi di aree di lavoro:

   * Area di lavoro vuota denominata **Workspace senza titolo** in cui è possibile iniziare ad aggiungere tipi di record manualmente quando si crea un&#39;area di lavoro da zero.
   * Area di lavoro denominata in base al modello selezionato, popolata con tipi di record di esempio. È possibile personalizzare ulteriormente i tipi di record e il workspace.

   Per gli amministratori di Workfront, la nuova area di lavoro viene visualizzata nella scheda **Aree di lavoro personali**. <!--replace this with: **Workspaces I'm on** tab-->
1. Fai clic sul nome del workspace nell’intestazione del nuovo workspace per rinominarlo, quindi premi Invio.

1. (Facoltativo e condizionale) Se l&#39;area di lavoro è stata creata da un modello, fare clic all&#39;interno del nome delle sezioni **Tipi di record operativi** o **Tassonomie**

   Oppure

   Passa il mouse sul nome di una sezione, quindi fai clic sul menu **Altro** ![](assets/more-menu.png), quindi fai clic su **Rinomina** per rinominare la sezione.

   >[!TIP]
   >
   >È possibile rinominare qualsiasi sezione da qualsiasi area di lavoro, anche se non è stata creata.

   Per ulteriori informazioni sulla modifica delle aree di lavoro, inclusa la modifica delle sezioni dell&#39;area di lavoro, vedere [Modifica aree di lavoro](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Facoltativo) Fai clic su **Aggiungi tipo di record** per aggiungere tipi di record all&#39;area di lavoro in qualsiasi sezione.

   Per informazioni, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

   Per ulteriori informazioni sulla modifica e l&#39;eliminazione di tipi di record in un&#39;area di lavoro, vedere [Modifica aree di lavoro](/help/quicksilver/planning/architecture/edit-workspaces.md).


