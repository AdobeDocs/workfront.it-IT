---
title: Elimina record
description: È possibile eliminare i record creati dall'utente corrente o da un altro utente.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 1%

---


# Elimina record

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->

{{planning-important-intro}}

È possibile eliminare record non più rilevanti in Adobe Workfront Planning. Puoi recuperare i record eliminati per 30 giorni dopo la loro eliminazione. Per informazioni sul ripristino dei record eliminati, vedere [Recuperare i record eliminati](/help/quicksilver/planning/records/restore-deleted-records.md).

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
<p>Qualsiasi pacchetto Workfront e Planning</p> <p>Qualsiasi flusso di lavoro e qualsiasi pacchetto di Planning</p>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Contribuire o concedere autorizzazioni superiori a un’area di lavoro e a un tipo di record  </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p> </td> 
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
   <td><p> Standard</p>
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
   <td>   <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## Considerazioni sull&#39;eliminazione di record

* È possibile eliminare i record creati dall&#39;utente corrente o da un altro utente.
* Puoi recuperare i record eliminati che tu o altri avete eliminato.
* Se i record eliminati sono collegati ad altri record, i record collegati non vengono eliminati, ma vengono eliminate anche le informazioni del record eliminato.
* Non è possibile eliminare record dalla visualizzazione timeline o calendario.

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
   * Dalla vista Tabella, passa il puntatore del mouse sul nome di un record, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su **Visualizza**

     ![Menu contestuale per riga record](assets/contextual-menu-for-record-row.png)
   * In una visualizzazione Sequenza temporale, fare clic su una barra dei record.

   Viene visualizzata la pagina del record.

1. Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del record, quindi fai clic su **Elimina**, quindi di nuovo su **Elimina** per confermare.

   ![Altre opzioni di menu dalla pagina dettagli record](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
Il record viene eliminato.
1. (Facoltativo) Vai alla visualizzazione tabella della pagina record e fai clic sull&#39;icona **Annulla** ![Annulla icona](assets/undo-icon.png) nell&#39;angolo superiore destro della visualizzazione, quindi fai clic su **Eliminati di recente** per recuperare i record eliminati.

Per informazioni sul ripristino dei record eliminati, vedere [Recuperare i record eliminati](/help/quicksilver/planning/records/restore-deleted-records.md).

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
   * Fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del record, quindi fai clic su **Elimina**.

     ![Menu contestuale per riga record](assets/contextual-menu-for-record-row.png)

   * Fai clic sull&#39;icona **Apri dettagli** ![Apri icona dettagli nel campo nome tabella](assets/open-details-icon-in-table-name-field.png) per aprire la casella con le informazioni dettagliate del record, quindi fai clic su **Altro** ![Altro menu](assets/more-menu.png) a destra del nome del record, quindi su **Elimina**.

   Il record viene eliminato.

1. (Facoltativo) Per annullare o ripristinare l&#39;eliminazione di un record, effettuare una delle seguenti operazioni:

   * Fai clic sull&#39;icona **Annulla** ![Annulla icona](assets/undo-icon.png), quindi **Eliminato di recente** per recuperare i record eliminati. Per informazioni sul ripristino dei record eliminati, vedere [Recuperare i record eliminati](/help/quicksilver/planning/records/restore-deleted-records.md).
   * Utilizzare le seguenti scelte rapide da tastiera per annullare o ripristinare l&#39;eliminazione di un record:

      * CTRL + Z (⌘ + Z per Mac) per annullare l&#39;eliminazione di un record
      * CTRL + MAIUSC + Z (⌘ + MAIUSC + Z per Mac) per ripetere l&#39;eliminazione del record




