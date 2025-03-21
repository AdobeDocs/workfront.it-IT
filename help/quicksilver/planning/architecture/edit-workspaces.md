---
title: Modifica aree di lavoro
description: È possibile modificare le informazioni di un'area di lavoro esistente, ad esempio rinominarla.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: 609396b2eb6413c8f6e84361757f00c2cc5e3ad6
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---


# Modificare le aree di lavoro

{{planning-important-intro}}

In Adobe Workfront Planning, le aree di lavoro sono posizioni centralizzate in cui i team possono pianificare il lavoro.

Un&#39;area di lavoro è una raccolta di tipi di record utilizzati da un team e rappresenta il ciclo di vita del lavoro del team. È possibile personalizzare completamente le aree di lavoro in Adobe Workfront Planning.

Per informazioni sulla creazione di aree di lavoro, vedere [Creare aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md).

Tutte le modifiche apportate a un&#39;area di lavoro sono visibili a tutti coloro che dispongono almeno delle autorizzazioni di visualizzazione per l&#39;area di lavoro.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso.

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
   <p> Prodotti</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td> 
   <td> 
<p>Uno dei seguenti piani di Workfront:</p> 
<ul><li>Seleziona</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>  <p>Gestire le autorizzazioni per l’area di lavoro </p>   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello di layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--OLD

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to the workspace </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>You must add the Planning area to your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

For more information about access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Modificare un’area di lavoro

{{step1-to-planning}}

1. (Condizionale) Se sei un amministratore di Workfront, fai clic su **Aree di lavoro in cui sono presente** per accedere alle aree di lavoro create oppure su **Altre aree di lavoro** per accedere alle aree di lavoro condivise con te.

<!--***********Replace the steps from the next below till the "Update the following information in the Edit workspace box:" (but keep this last step)*******-->

1. (Facoltativo) Fai clic su **Mostra tutto** per visualizzare altre aree di lavoro. Il collegamento **Mostra tutto** viene visualizzato solo se sono presenti più di due righe di schede dell&#39;area di lavoro.
1. (Facoltativo) Fai clic su **Mostra meno** per limitare il numero di aree di lavoro visualizzate sullo schermo.
1. Per modificare un&#39;area di lavoro, effettuate una delle seguenti operazioni:

   * Passa il puntatore del mouse sulla scheda dell&#39;area di lavoro, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) nell&#39;angolo superiore destro della scheda
Oppure
   * Fai clic su una scheda dell&#39;area di lavoro per aprirla, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome dell&#39;area di lavoro.
1. Fai clic su **Modifica**.

   Viene visualizzata la casella **Modifica area di lavoro**.

   ![Casella di modifica area di lavoro](assets/edit-workspace-box.png)

1. Aggiorna le seguenti informazioni nella casella **Modifica area di lavoro**:

   * Aggiungi un nome per l’area di lavoro. <!--did they add a label for this field?-->
   * **Descrizione**: aggiungere informazioni sull&#39;area di lavoro.
   * Selezionate un&#39;icona da associare al workspace.

1. Fai clic su **Salva** per chiudere la casella Modifica area di lavoro e applicare le modifiche.

1. (Facoltativo) Per aggiungere una nuova sezione dell&#39;area di lavoro, effettuate una delle seguenti operazioni:

   * Fai clic su **Aggiungi sezione** nella parte inferiore dell&#39;area di lavoro.
   * Passa il puntatore del mouse sul nome di una sezione e fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su **Aggiungi sezione sopra** o **Aggiungi sezione sotto**.

1. (Facoltativo) Per modificare la posizione di una sezione, effettuate una delle seguenti operazioni:

   * Passa il puntatore del mouse sul nome di una sezione e fai clic sull&#39;icona **grab** ![Grab icon](assets/grab-icon.png), quindi trascinala nel punto giusto.
   * Passa il puntatore del mouse sul nome di una sezione e fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su **Sposta su** o su **Sposta giù**. La sezione si sposta verso l&#39;alto o verso il basso all&#39;interno dell&#39;area di lavoro.

1. (Facoltativo) Per eliminare una sezione dell&#39;area di lavoro, effettuare le seguenti operazioni:

   1. Passa il puntatore del mouse sul nome di una sezione, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su **Elimina**. <!--add screen shot when UI is final?-->
   1. Selezionare una nuova sezione per spostare tutti i tipi di record, quindi fare clic su **Elimina**. <!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      Tutti i tipi di record vengono spostati nella sezione di selezione e la sezione viene eliminata.

1. (Facoltativo) Fare clic su **Aggiungi tipo di record** per aggiungere tipi di record all&#39;area di lavoro.

   Per informazioni, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

1. (Facoltativo) Passa il puntatore del mouse su una scheda del tipo di record, fai clic sul menu **Altro** ![Altro](assets/more-menu.png) nell&#39;angolo superiore destro, quindi fai clic su **Modifica** per modificare l&#39;aspetto di un tipo di record.

   Per informazioni, vedere [Modifica tipi di record](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Facoltativo) Passa il puntatore del mouse su una scheda del tipo di record, fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) nell&#39;angolo superiore destro, quindi fai clic su **Elimina** per eliminare un tipo di record.

   Per informazioni, vedere [Eliminare i tipi di record](/help/quicksilver/planning/architecture/delete-record-types.md).

1. (Facoltativo) Fai clic su una scheda del tipo di record per trascinarla e rilasciarla in un nuovo punto. È possibile trascinare tipi di record da una sezione dell&#39;area di lavoro a un&#39;altra.

   ![Trascinare i tipi di record in un&#39;area di lavoro](assets/drag-and-drop-record-types-in-a-workspace.png)

1. (Facoltativo) Fai clic su **Condividi** nell&#39;angolo superiore destro dell&#39;area di lavoro per condividerla con altri utenti.

   Per informazioni, vedere [Condividi aree di lavoro](/help/quicksilver/planning/access/share-workspaces.md).
