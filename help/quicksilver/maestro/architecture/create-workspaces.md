---
title: Creare aree di lavoro
description: Un'area di lavoro è una raccolta di tipi di record utilizzati da un team e rappresenta il ciclo di vita del lavoro del team. È possibile personalizzare completamente le aree di lavoro nella pianificazione di Adobe Workfront.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Creare aree di lavoro

{{maestro-important-intro}}

Nella pianificazione di Adobe Workfront, le aree di lavoro sono posizioni centralizzate in cui i team possono pianificare il lavoro.

Un&#39;area di lavoro è una raccolta di tipi di record utilizzati da un team e rappresenta il ciclo di vita del lavoro del team. È possibile personalizzare completamente le aree di lavoro nella pianificazione di Adobe Workfront.

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
<p>La tua organizzazione deve essere iscritta al programma beta chiuso di Adobe Workfront Planning. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
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
   <td> <p>Non sono presenti controlli del livello di accesso per la pianificazione di Adobe Workfront</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Ricevi le autorizzazioni di gestione per le aree di lavoro create. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>È necessario aggiungere l'area Planning al modello di layout. Per informazioni, consulta <a href="../access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Per ulteriori informazioni sui requisiti di accesso, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considerazioni sulle aree di lavoro

* Puoi creare aree di lavoro per specifiche unità organizzative all’interno dell’organizzazione, in base al funzionamento univoco di ciascuna unità.
* I tipi di record contenuti in un&#39;area di lavoro devono riflettere il ciclo di vita lavorativo di un&#39;unità organizzativa.
* Quando crei un’area di lavoro, solo tu disponi dell’autorizzazione per accedere a essa e gestirla. È necessario condividerlo con altri utenti affinché possano collaborare con te nello stesso spazio. Per informazioni, consulta [Condividere un’area di lavoro](/help/quicksilver/maestro/access/share-workspaces.md). Gli amministratori di sistema possono gestire tutte le aree di lavoro, anche quelle che non hanno creato.
* Puoi avere un massimo di 1.000 aree di lavoro nell’istanza Workfront della tua organizzazione.
* Le aree di lavoro contengono tipi di record univoci per ogni area di lavoro. <!--this might change-->

## Creare un’area di lavoro

{{step1-to-maestro}}

1. (Condizionale) Se nell’ambiente non sono presenti aree di lavoro, fai clic su **Crea area di lavoro**

   In alternativa, da un workspace esistente, fare clic sul pulsante destro del mouse sul nome del workspace, quindi fare clic su **Crea area di lavoro**.

   ![](assets/workspace-drop-down-right-menu.png)

   Verrà aperta l&#39;area Aree di lavoro della pianificazione di Workfront.
1. (Facoltativo e condizionale) Fai clic su **Anteprima** in uno dei seguenti modelli predefiniti di workspace:

   * Gestione marketing
   * Gestione vendite
   * Gestione dei prodotti

   È possibile indicare i tipi di record operativi, le tassonomie e il numero di campi associati a ciascun modello.

   ![](assets/previewing-a-workspace-template.png)

   Per informazioni sui modelli dell&#39;area di lavoro di pianificazione di Workfront, vedere [Elenco dei modelli di Workspace](../architecture/workspace-templates.md).

1. Clic **Usa modello** per iniziare a creare l&#39;area di lavoro dal modello selezionato

   Oppure

   Clic **Crea area di lavoro** per creare un&#39;area di lavoro da zero.

   Viene creato uno dei seguenti tipi di aree di lavoro:

   * Area di lavoro vuota in cui è possibile iniziare ad aggiungere tipi di record manualmente quando si crea un&#39;area di lavoro da zero.
   * Area di lavoro con tipi di record di esempio che è possibile personalizzare ulteriormente quando si utilizza uno dei modelli.

1. Fai clic sul nome dell’area di lavoro nell’intestazione della nuova area di lavoro per rinominarla, quindi premi Invio

   Oppure

   Fai clic su **Altro** menu ![](assets/more-menu.png)a destra del nome del workspace nell’intestazione, quindi fai clic su **Rinomina**.

1. (Facoltativo e condizionale) Se l&#39;area di lavoro include già sezioni, fare clic su **Aggiungi sezione** per aggiungere una nuova sezione a un workspace. Una sezione può contenere diversi tipi di record.

1. (Facoltativo e condizionale) Se avete creato l&#39;area di lavoro da un modello, fate clic all&#39;interno del nome del **Tipi di record operativi** o **Tassonomie** sezioni

   Oppure

   Passa il puntatore del mouse sul nome di una sezione, quindi fai clic su **Altro** menu ![](assets/more-menu.png), quindi fai clic su **Rinomina** per rinominare la sezione.

   >[!TIP]
   >
   >È possibile rinominare qualsiasi sezione da qualsiasi area di lavoro, anche se la sezione è stata creata.

1. (Facoltativo) Per modificare la posizione di una sezione, effettuate una delle seguenti operazioni:

   * Passa il puntatore del mouse sul nome di una sezione e fai clic su **afferrare** icona ![](assets/grab-icon.png), quindi trascinarlo nel punto giusto.
   * Passa il puntatore del mouse sul nome di una sezione e fai clic su **Altro** menu ![](assets/more-menu.png), quindi fai clic su **Sposta su** o **Sposta in basso**. La sezione si sposta verso l&#39;alto o verso il basso all&#39;interno dell&#39;area di lavoro.

1. (Facoltativo) Per aggiungere una nuova sezione, effettuate una delle seguenti operazioni:

   * Clic **Aggiungi sezione** nella parte inferiore dell&#39;area di lavoro.
   * Passa il puntatore del mouse sul nome di una sezione e fai clic su **Altro** menu ![](assets/more-menu.png), quindi fai clic su **Aggiungi sezione sopra** o **Aggiungi sezione di seguito**.

1. (Facoltativo) Fai clic su **Aggiungi tipo di record** per aggiungere tipi di record al workspace.

   Per informazioni, consulta [Crea tipi di record](../architecture/create-record-types.md).


