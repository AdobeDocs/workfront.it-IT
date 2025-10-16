---
title: Condividere i record
description: È possibile condividere i record con altri utenti per aumentare la collaborazione.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# Condividere i record

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->

{{planning-important-intro}}

Per collaborare con altri utenti, è possibile condividere i record con altri utenti.

È possibile condividere un record di Adobe Workfront Planning nei modi seguenti:

* Copiare il collegamento della pagina record dal browser quando la pagina è aperta.

* Copiare un collegamento alla pagina del record quando si visualizzano i record nella vista tabella del tipo di record.

* È possibile condividere tutti i record di un&#39;area di lavoro con altri utenti condividendo l&#39;area di lavoro e il tipo di record.

  Per ulteriori informazioni, consulta i seguenti articoli:

   * [Condividere un’area di lavoro](/help/quicksilver/planning/access/share-workspaces.md)

   * [Condividere un tipo di record](/help/quicksilver/planning/access/share-record-types.md)

In questo articolo viene descritto come copiare un collegamento alla pagina di un record dalla vista tabella di un tipo di record.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Qualsiasi pacchetto Workfront e Planning</p></li>
Oppure
<li><p>Qualsiasi flusso di lavoro e qualsiasi pacchetto di Planning</p></li></ul>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Collaboratore o versione successiva</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>  <p>Visualizza o autorizzazioni superiori per un'area di lavoro e tipo di record per condividere un record utilizzando un collegamento</p>
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Modello layout</p></td>
   <td> Agli utenti con una licenza Light o Contributor deve essere assegnato un modello di layout che includa Planning.
   <p>Per impostazione predefinita, le aree Pianificazione sono attivate dagli utenti standard e dagli amministratori di sistema.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  


<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Contributor or higher license </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  <p>View or higher permissions to a workspace and record typeto share   a record using a link </p>
   <p>Manage permissions to a workspace and record type to share the records in the workspace </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table> -->


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

I tipi di record e i record ereditano le stesse autorizzazioni dall&#39;area di lavoro.

Solo gli utenti con le autorizzazioni di gestione di un’area di lavoro possono condividerla con altri utenti.

Per ulteriori informazioni, vedere [Condividere un&#39;area di lavoro](/help/quicksilver/planning/access/share-workspaces.md).

## Condividere tutti i record di un tipo di record condividendo il tipo di record

I record ereditano le autorizzazioni dal tipo di record.

Per impostazione predefinita, i tipi di record ereditano le autorizzazioni dal workspace.

Tuttavia, è possibile effettuare una delle seguenti operazioni:

* Disabilita le autorizzazioni ereditate dall&#39;area di lavoro in un tipo di record. In questo modo verranno rimosse le autorizzazioni di livello superiore per i record, ma verranno mantenute le autorizzazioni di visualizzazione per l&#39;area di lavoro, il tipo di record e i record.
* Concedere manualmente le autorizzazioni agli utenti per un tipo di record, anche quando non dispongono di autorizzazioni per l&#39;area di lavoro. In questo modo viene automaticamente concesso loro il permesso di visualizzazione per l&#39;area di lavoro. In questo modo vengono concesse autorizzazioni agli utenti per i record.

Solo gli utenti con le autorizzazioni Gestione di un&#39;area di lavoro possono condividere i tipi di record e i record con altri utenti.

Per ulteriori informazioni, vedere [Condividi tipi di record](/help/quicksilver/planning/access/share-record-types.md).

