---
title: Condividere i record
description: È possibile condividere i record con altri utenti per aumentare la collaborazione.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# Condividere i record

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Per collaborare con altri utenti, è possibile condividere i record con altri utenti.

È possibile condividere un record di Adobe Workfront Planning nei modi seguenti:

* Copiare il collegamento della pagina record dal browser quando la pagina è aperta.

* Copiare un collegamento alla pagina del record quando si visualizzano i record nella vista tabella del tipo di record.

* È possibile condividere tutti i record di un&#39;area di lavoro con altri utenti condividendo l&#39;area di lavoro <span class="preview"> e il tipo di record.</span>

  Per ulteriori informazioni, consulta i seguenti articoli:

   * [Condividere un’area di lavoro](/help/quicksilver/planning/access/share-workspaces.md)

  <div class="preview">

   * [Condividere un tipo di record](/help/quicksilver/planning/access/share-record-types.md)

  </div>

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
   <td>  <p>Visualizza o autorizzazioni superiori per un'area di lavoro <span class="preview"> e tipo di record</span> da condividere   un record utilizzando un collegamento </p>
   <p>Gestisci le autorizzazioni per un'area di lavoro <span class="preview"> e un tipo di record</span> per condividere i record nell'area di lavoro </p>
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello layout</p></td> 
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


<div class="preview">

## Condividere tutti i record di un tipo di record condividendo il tipo di record

Nell’ambiente di produzione, i record ereditano le autorizzazioni dall’area di lavoro.

Nell&#39;ambiente di anteprima i record ereditano le autorizzazioni dal tipo di record.

Per impostazione predefinita, i tipi di record ereditano le autorizzazioni dal workspace.

Tuttavia, è possibile effettuare una delle seguenti operazioni:

* Disabilita le autorizzazioni ereditate dall&#39;area di lavoro in un tipo di record. In questo modo verranno rimosse le autorizzazioni di livello superiore per i record, ma verranno mantenute le autorizzazioni di visualizzazione per l&#39;area di lavoro, il tipo di record e i record.
* Concedere manualmente le autorizzazioni agli utenti per un tipo di record, anche quando non dispongono di autorizzazioni per l&#39;area di lavoro. In questo modo viene automaticamente concesso loro il permesso di visualizzazione per l&#39;area di lavoro. In questo modo vengono concesse autorizzazioni agli utenti per i record.

Solo gli utenti con le autorizzazioni Gestione di un&#39;area di lavoro possono condividere i tipi di record e i record con altri utenti.

Per ulteriori informazioni, vedere [Condividi tipi di record](/help/quicksilver/planning/access/share-record-types.md).

</div>
