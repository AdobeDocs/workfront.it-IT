---
title: Condividere i record
description: È possibile condividere i record con altri utenti per aumentare la collaborazione.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 1%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

# Condividere i record

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

<!--take out preview and production references at release-->

{{planning-important-intro}}

Per collaborare con altri utenti, è possibile condividere i record con altri utenti.

È possibile condividere un record di Adobe Workfront Planning nei modi seguenti:

* Copiare il collegamento della pagina record dal browser quando la pagina è aperta.

* Copiare un collegamento alla pagina del record quando si visualizzano i record nella vista tabella del tipo di record.

* È possibile condividere tutti i record di un&#39;area di lavoro con altri utenti condividendo l&#39;area di lavoro <!--<span class="preview">and record type</span>-->. Per ulteriori informazioni, vedere [Condividere un&#39;area di lavoro](/help/quicksilver/planning/access/share-workspaces.md).

<!-- replace the last sentence above with this: 

For more information see the following articles:

* [Share a workspace](/help/quicksilver/planning/access/share-workspaces.md)


<div class="preview">

* [Share a record type](/help/quicksilver/planning/access/share-record-types.md)

</div>

-->

In questo articolo viene descritto come copiare un collegamento alla pagina di un record dalla vista tabella di un tipo di record.

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
   <td><p> Collaboratore, Light o Standard </p>
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
   <td>  <p>Visualizza o autorizzazioni superiori per un'area di lavoro per condividere <!--<span class="preview">and record type</span>--> un record utilizzando un collegamento </p>
   <p>Gestire le autorizzazioni per un'area di lavoro <!--<span class="preview">and record type</span>--> per condividere i record nell'area di lavoro </p>
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello di layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--OLD:

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
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace to share a record using a link </p>
   <p>Manage permissions to a workspace to share the workspace the record belongs to </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

-->

## Condividere i collegamenti ai record dalla vista tabella del tipo di record

{{step1-to-planning}}

Viene aperto l&#39;ultimo workspace a cui si è effettuato l&#39;accesso.
1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.
1. (Condizionale) Dal menu a discesa **Visualizza** nell&#39;angolo superiore destro della tabella, selezionare una vista tabella. Questa dovrebbe essere la vista predefinita, a meno che il tipo di record non sia stato visualizzato nella vista timeline al momento dell&#39;ultimo accesso.

   I record associati al tipo di record selezionato vengono visualizzati nella vista tabella.
1. Fare clic con il pulsante destro del mouse su una riga di record

   Oppure

   Passa il puntatore del mouse sul nome di un record, fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su **Copia collegamento**.

   ![Menu contestuale per riga record](assets/contextual-menu-for-record-row.png)

   Il collegamento viene copiato negli Appunti.

1. Incolla il collegamento in un’e-mail o in una finestra di chat per condividerlo con altri utenti. Quando gli utenti ricevono il collegamento, viene aperta la pagina di registrazione.

   >[!TIP]
   >
   >I campi nella pagina record sono gli stessi campi disponibili nella visualizzazione Tabella del record.


   <!--add there when it will be available: if they have access to this record-->

## Condividere tutti i record in un&#39;area di lavoro condividendo l&#39;area di lavoro

È possibile condividere tutti i record di un&#39;area di lavoro quando questa viene condivisa con altri utenti.

Solo gli utenti con le autorizzazioni di gestione di un’area di lavoro possono condividerla con altri utenti.

Per ulteriori informazioni, vedere [Condividere un&#39;area di lavoro](/help/quicksilver/planning/access/share-workspaces.md).


<!--
<div class="preview">

## Share all records in a record type by sharing the record type

In the Production environment, records inherit permissions from the workspace. 

In the Preview environment, records inherit permissions from the record type. 

By default, record types inherit permissions from the workspace. 

However, you can do any of the following:

* Turn off inherited permissions from the workspace on a record type. This removes permissions from the records. 
* Manually grant permissions to users to a record type, even when they have no permissions to the workspace. This automatically gives them View permissions to the workspace. This grants permissions to users to the records. 

Only users with Manage permissions to a workspace can share its record types and records with others. 

For more information, see [Share record types](/help/quicksilver/planning/access/share-record-types.md). 

</div>

-->