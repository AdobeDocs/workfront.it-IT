---
title: Elimina record
description: È possibile eliminare i record creati dall'utente corrente o da un altro utente.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 2%

---


# Elimina record

<!--take Preview and Production references out at release-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

È possibile eliminare record non più rilevanti in Adobe Workfront Planning. Puoi recuperare i record eliminati per 30 giorni dopo la loro eliminazione. Per informazioni sul ripristino dei record eliminati, vedere [Recuperare i record eliminati](/help/quicksilver/planning/records/restore-deleted-records.md).

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
   <td>   <p>Autorizzazioni di Contribute o superiori per un'area di lavoro <!--<span class="preview">and record type</span>--> </a> </p>  
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

## Considerazioni sull&#39;eliminazione di record

* È possibile eliminare i record creati dall&#39;utente corrente o da un altro utente.
* Non è possibile recuperare i record eliminati nell’ambiente di produzione. È possibile recuperare i record eliminati nell’ambiente di anteprima.
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
   * Dalla vista Tabella, passa il puntatore del mouse sul nome di un record, quindi fai clic sul menu **Altro** ![](assets/more-menu.png), quindi fai clic su **Visualizza**

     ![](assets/contextual-menu-for-record-row.png)
   * In una visualizzazione Sequenza temporale, fare clic su una barra dei record.

   Viene visualizzata la pagina del record.

1. Fai clic sul menu **Altro** ![](assets/more-menu.png) a destra del nome del record, quindi fai clic di nuovo su **Elimina**, quindi su **Elimina** per confermare.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
Il record viene eliminato.
1. (Facoltativo e condizionale) Se elimini il record nell&#39;ambiente di anteprima, accedi alla visualizzazione a tabella della pagina del record e fai clic sull&#39;icona **Annulla** ![](assets/undo-icon.png) nell&#39;angolo superiore destro della visualizzazione, quindi fai clic su **Eliminati di recente** per recuperare i record eliminati.

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
   * Fai clic sul menu **Altro** ![](assets/more-menu.png) a destra del nome del record, quindi fai clic su **Elimina**.

     ![](assets/contextual-menu-for-record-row.png)

   * Fai clic sull&#39;icona ![](assets/open-details-icon-in-table-name-field.png) **Apri dettagli** per aprire la casella con le informazioni dettagliate del record, quindi fai clic su **Altro** ![](assets/more-menu.png) a destra del nome del record, quindi su **Elimina**.

   Il record viene eliminato.

1. (Facoltativo) Per annullare o ripristinare l&#39;eliminazione di un record, effettuare una delle seguenti operazioni:

   * Fai clic sull&#39;icona **Annulla** ![](assets/undo-icon.png), quindi **Eliminati di recente** per recuperare i record eliminati. Per informazioni sul ripristino dei record eliminati, vedere [Recuperare i record eliminati](/help/quicksilver/planning/records/restore-deleted-records.md).
   * Utilizzare le seguenti scelte rapide da tastiera per annullare o ripristinare l&#39;eliminazione di un record:

      * CTRL + Z (⌘ + Z per Mac) per annullare l’eliminazione di un record
      * CTRL + MAIUSC + Z (⌘ + MAIUSC + Z per Mac) per ripetere l’eliminazione del record




