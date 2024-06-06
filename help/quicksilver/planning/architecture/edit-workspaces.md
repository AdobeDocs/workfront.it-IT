---
title: Modificare le aree di lavoro
description: È possibile modificare le informazioni di un'area di lavoro esistente, ad esempio rinominarla.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: 3a819fc18e0b5f438a55265ea0c5c9679ef0fdd6
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Modificare le aree di lavoro

{{planning-important-intro}}

In Adobe Workfront Planning, le aree di lavoro sono posizioni centralizzate in cui i team possono pianificare il lavoro.

Un&#39;area di lavoro è una raccolta di tipi di record utilizzati da un team e rappresenta il ciclo di vita del lavoro del team. È possibile personalizzare completamente le aree di lavoro in Adobe Workfront Planning.

Per informazioni sulla creazione delle aree di lavoro, consulta [Creare aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md).

Tutte le modifiche apportate a un&#39;area di lavoro sono visibili a tutti coloro che dispongono almeno delle autorizzazioni di visualizzazione per l&#39;area di lavoro.

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
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td>
   <td>
   <p>Nuovo: Standard</p>
   <p>Corrente: Piano</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td>
   <td> <p>Nessun controllo del livello di accesso per Workfront Planning</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestire le autorizzazioni per l’area di lavoro </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>È necessario aggiungere l'area Planning al modello di layout. Per informazioni, consulta <a href="/help/quicksilver/planning/access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Per ulteriori informazioni sui requisiti di accesso, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Modificare un’area di lavoro

{{step1-to-planning}}

1. Fai clic sul nome dell’area di lavoro nell’intestazione della nuova area di lavoro per rinominarla, quindi premi **Invio**.
1. Fai clic su **Altro** menu ![](assets/more-menu.png)a destra del nome del workspace nell’intestazione, quindi fai clic su **Modifica**.

   ![](assets/edit-workspace-box.png)

   Aggiorna le seguenti informazioni in **Modifica area di lavoro** casella:

   * Aggiungi un nome per l’area di lavoro. <!--did they add a label for this field?-->
   * **Descrizione**: aggiungi informazioni sull’area di lavoro.
   * Selezionate un&#39;icona da associare al workspace.

1. Clic **Salva** per chiudere la casella Modifica area di lavoro e applicare le modifiche.

1. (Facoltativo) Per aggiungere una nuova sezione dell&#39;area di lavoro, effettuate una delle seguenti operazioni:

   * Clic **Aggiungi sezione** nella parte inferiore dell&#39;area di lavoro.
   * Passa il puntatore del mouse sul nome di una sezione e fai clic su **Altro** menu ![](assets/more-menu.png), quindi fai clic su **Aggiungi sezione sopra** o **Aggiungi sezione di seguito**.

1. (Facoltativo) Per modificare la posizione di una sezione, effettuate una delle seguenti operazioni:

   * Passa il puntatore del mouse sul nome di una sezione e fai clic su **afferrare** icona ![](assets/grab-icon.png), quindi trascinarlo nel punto giusto.
   * Passa il puntatore del mouse sul nome di una sezione e fai clic su **Altro** menu ![](assets/more-menu.png), quindi fai clic su **Sposta su** o **Sposta in basso**. La sezione si sposta verso l&#39;alto o verso il basso all&#39;interno dell&#39;area di lavoro.

1. (Facoltativo) Per eliminare una sezione dell&#39;area di lavoro, effettuare le seguenti operazioni:

   1. Passa il puntatore del mouse sul nome di una sezione, quindi fai clic sul pulsante **Altro** menu ![](assets/more-menu.png), quindi fai clic su **Elimina**. <!--add screen shot when UI is final?-->
   1. Selezionare una nuova sezione in cui spostare tutti i tipi di record, quindi fare clic su **Elimina**. <!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      Tutti i tipi di record vengono spostati nella sezione di selezione e la sezione viene eliminata.

1. (Facoltativo) Fai clic su **Aggiungi tipo di record** per aggiungere tipi di record al workspace.

   Per informazioni, consulta [Crea tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

1. (Facoltativo) Passa il puntatore del mouse su una scheda del tipo di record e fai clic sul pulsante **Altro** menu ![](assets/more-menu.png) nell’angolo superiore destro, quindi fai clic su **Modifica** per modificare l&#39;aspetto di un tipo di record

   Per informazioni, consulta [Modifica tipi di record](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Facoltativo) Passa il puntatore del mouse su una scheda del tipo di record e fai clic sul pulsante **Altro** menu ![](assets/more-menu.png) nell’angolo superiore destro, quindi fai clic su **Elimina** per eliminare un tipo di record.

   Per informazioni, consulta [Elimina tipi di record](/help/quicksilver/planning/architecture/delete-record-types.md)).

1. (Facoltativo) Fai clic su una scheda del tipo di record per trascinarla e rilasciarla in un nuovo punto. È possibile trascinare tipi di record da una sezione dell&#39;area di lavoro a un&#39;altra.

   ![](assets/drag-and-drop-record-types-in-a-workspace.png)

1. (Facoltativo) Fai clic su **Condividi** nell’angolo superiore destro dell’area di lavoro per condividerla con altri utenti.

   Per informazioni, consulta [Condividere le aree di lavoro](/help/quicksilver/planning/access/share-workspaces.md).
