---
title: Creare aree di lavoro
description: Un’area di lavoro è una raccolta di tipi di record operativi e tassonomie utilizzati da un team e rappresenta il ciclo di vita del lavoro del team. In Maestro è possibile personalizzare completamente le aree di lavoro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 74db651f8865965f943bc89e58e7130cffe0c450
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Creare aree di lavoro

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono a Adobe Maestro, una nuova offerta di Adobe Workfront.
>
>Attualmente, Adobe Maestro fa parte di un programma beta aperto a un numero limitato di clienti. Per utilizzare le funzionalità Maestro, devi essere un cliente Workfront.
>
>Contatta il rappresentante del tuo account per ulteriori informazioni su come partecipare al programma beta per Maestro.
>
>Per informazioni, consulta [Panoramica di Adobe Maestro](../maestro-overview.md).

Ad Adobe, Maestro, le aree di lavoro sono posizioni centralizzate in cui i team possono pianificare il lavoro.

Un’area di lavoro è una raccolta di tipi di record operativi e tassonomie utilizzati da un team e rappresenta il ciclo di vita del lavoro del team. In Maestro è possibile personalizzare completamente le aree di lavoro.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> prodotto Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
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
   <td role="rowheader">Livello di accesso</td>
   <td> <p>Qualsiasi</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modello di layout</td>
   <td> <p>L’amministratore di sistema deve aggiungere l’area Maestro nel modello di layout. Per informazioni, consulta <a href="../access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level*</p></td>
   <td> <p>System Administrator</p>  
   <p>The following license types:</p>
   <ul><li>New: Standard</li>
   <li>Current: Worker or higher </li></ul>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>You must add the Maestro area to your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

For more information, see [Access requirements in Workfront documentation](/help/quicksilver\administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 
-->




<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considerazioni sulle aree di lavoro

* Puoi creare aree di lavoro per specifiche unità organizzative all’interno dell’organizzazione, in base al funzionamento univoco di ciascuna unità.
* I tipi di record e le tassonomie contenuti in un&#39;area di lavoro devono riflettere il ciclo di vita di un&#39;unità organizzativa.
* Quando crei un’area di lavoro, tutti gli utenti dell’organizzazione possono visualizzarla, modificarla o eliminarla.  <!--this will change with access levels and permissions-->
* Nella tua organizzazione puoi avere un massimo di 1.000 aree di lavoro.
* Le aree di lavoro contengono tipi di record univoci per ogni area di lavoro. <!--this might change-->

## Creare un’area di lavoro

1. (Condizionale) Se nel sistema non è presente alcuna area di lavoro, fare clic sul pulsante **Menu principale** icona ![](assets/main-menu-workfront.png) nell&#39;angolo superiore destro di Workfront oppure **Menu principale** icona ![](assets/main-menu-shell.png)  nell’angolo superiore sinistro, se disponibile, fai clic su **Maestro** ![](assets/maestro-icon.png).

   In alternativa, da un workspace esistente, fare clic sul pulsante destro del mouse sul nome del workspace, quindi fare clic su **Crea area di lavoro**.

   ![](assets/workspace-drop-down-right-menu.png)

   Si apre l&#39;area Workspaces di Maestro.
1. (Facoltativo e condizionale) Fai clic su **Anteprima** in uno dei seguenti modelli predefiniti di workspace:

   * Gestione marketing
   * Gestione vendite
   * Gestione dei prodotti

   È possibile indicare i tipi di record operativi, le tassonomie e il numero di campi associati a ciascun modello.

   ![](assets/previewing-a-workspace-template.png)

   Per informazioni sui modelli di area di lavoro Maestro, consulta [Elenco dei modelli di Workspace](../architecture/workspace-templates.md).

1. Clic **Usa modello** per iniziare a creare l&#39;area di lavoro dal modello selezionato

   Oppure

   Clic **Crea area di lavoro** per creare un&#39;area di lavoro da zero.

   Viene creato uno dei seguenti tipi di aree di lavoro:

   * Area di lavoro vuota in cui è possibile iniziare ad aggiungere tipi di record manualmente.
   * Area di lavoro con tipi di record di esempio che è possibile personalizzare ulteriormente.

1. Fai clic sul nome dell’area di lavoro nell’intestazione della nuova area di lavoro per rinominarla, quindi premi Invio

   Oppure

   Fai clic su **Altro** menu ![](assets/more-menu.png)a destra del nome del workspace nell’intestazione, quindi fai clic su **Rinomina**.

1. (Facoltativo) Fai clic su **Aggiungi tipo di record** per aggiungere tipi di record al workspace.

   Per informazioni, consulta [Crea tipi di record](../architecture/create-record-types.md).

1. (Facoltativo) Fai clic su **Aggiungi tassonomia** per aggiungere tassonomie all&#39;area di lavoro.

   Per informazioni, consulta [Creare tassonomie](../architecture/create-a-taxonomy.md).
