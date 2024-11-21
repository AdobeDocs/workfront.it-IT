---
title: Elimina record
description: È possibile eliminare i record creati dall'utente corrente o da un altro utente. Non è possibile recuperare i record eliminati.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 2%

---


# Elimina record

{{planning-important-intro}}

È possibile eliminare record non più rilevanti in Adobe Workfront Planning.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per Workfront Planning.

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
   <td>   <p>Autorizzazioni Contribute o superiori per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello di layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--

OLD

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
   <td role="rowheader"><p>Adobe Workfront license*</p>
   </td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning </p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
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

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Considerazioni sull&#39;eliminazione di record

* È possibile eliminare i record creati dall&#39;utente corrente o da un altro utente.
* Non è possibile recuperare i record eliminati. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* Se i record eliminati sono collegati ad altri record, i record collegati non vengono eliminati, ma vengono eliminate anche le informazioni del record eliminato.
* Non è possibile eliminare i record in blocco. <!--this will probably change-->
* Non è possibile eliminare record dalla visualizzazione timeline.

## Elimina record

È possibile eliminare un record dalle seguenti aree:

* [Dalla pagina del record](#delete-a-record-from-the-records-page)
* [Dalla vista tabella di un tipo di record](#delete-a-record-from-the-record-type-table-view)

### Eliminare un record dalla pagina del record

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera eliminare i record.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.
1. Esegui una delle operazioni seguenti:

   * In una visualizzazione Tabella fare clic sul nome di un record.
   * Dalla vista Tabella, passa il puntatore del mouse sul nome di un record, quindi fai clic sul menu **Altro** ![](assets/more-menu.png), quindi fai clic su **Visualizza**

     ![](assets/contextual-menu-for-record-row.png)
   * In una visualizzazione Sequenza temporale, fare clic su una barra dei record.

   Viene visualizzata la pagina del record.

1. Fai clic sul menu **Altro** ![](assets/more-menu.png) a destra del nome del record, quindi fai clic di nuovo su **Elimina**, quindi su **Elimina** per confermare.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
Il record viene eliminato e non può essere recuperato.

### Eliminare un record dalla vista tabella del tipo di record

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera eliminare i record.

   Viene aperto il workspace e i tipi di record vengono visualizzati come schede.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.
1. (Condizionale) Dal menu a discesa **Visualizza** nell&#39;angolo superiore sinistro della tabella, selezionare una visualizzazione Tabella. Questa dovrebbe essere la vista predefinita, a meno che il tipo di record non sia stato visualizzato nella vista timeline al momento dell&#39;ultimo accesso.

   I record associati al tipo di record selezionato vengono visualizzati nella vista tabella.
1. Esegui una delle operazioni seguenti:

   * Fare clic con il pulsante destro del mouse su una riga di record, quindi scegliere **Elimina**.
   * Fai clic sul menu **Altro** ![](assets/more-menu.png) a destra del nome del record, quindi fai clic su **Elimina**

     ![](assets/contextual-menu-for-record-row.png)

   * Fai clic sull&#39;icona ![](assets/open-details-icon-in-table-name-field.png) **Apri dettagli** per aprire la casella con le informazioni dettagliate del record, quindi fai clic su **Altro** ![](assets/more-menu.png) a destra del nome del record, quindi su **Elimina**.

   Il record viene eliminato e non può essere recuperato.

1. (Facoltativo) Utilizzare le seguenti scelte rapide da tastiera per annullare o ripristinare l&#39;eliminazione di un record:

   * CTRL + Z (⌘ + Z per Mac) per annullare una modifica
   * CTRL + MAIUSC + Z (⌘ + MAIUSC + Z per Mac) per ripetere una modifica
