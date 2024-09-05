---
title: Esportare la pagina record
description: È possibile esportare l'anteprima o la pagina dei dettagli del record in Word.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8de68b70-dd87-4aad-9137-980ea9fc0d69
source-git-commit: 3823afdc14aaf5646d8edc60f5ad633e48336af7
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 1%

---

# Esportare i dettagli di un record

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambiente Sandbox di anteprima.</span>

Per collaborare in modo più efficiente con altri utenti che potrebbero non disporre di un account Workfront, è possibile esportare i dettagli di un record in un file e condividerlo con loro.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso per Workfront Planning.

Per accedere a Workfront Planning, è necessario disporre dei seguenti elementi:

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
   <td role="rowheader"><p>Piano di pianificazione Adobe Workfront*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata di Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td> <p>Standard</p>
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
   <td>   <p>Visualizza o autorizzazioni superiori per un'area di lavoro</a> </p>  
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
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
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

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Considerazioni sull&#39;esportazione dei dettagli di un record:

* È possibile esportare i dettagli di un record nei seguenti formati di file:

   * .docx Word
   * <span class="preview">.pdf</span>

* È possibile esportare la scheda Dettagli della pagina di un record. Non è possibile esportare la scheda Connessioni.

* Il file esportato mantiene il layout della pagina di registrazione, incluse le miniature e le immagini di copertina.

## Esportare i dettagli di un record

{{step1-to-planning}}

1. Fai clic sulla scheda di un’area di lavoro.

   L&#39;area di lavoro si apre e i tipi di record vengono visualizzati sulle schede.

1. Fare clic su una scheda del tipo di record.
Viene visualizzata la pagina del tipo di record e vengono visualizzati tutti i record di quel tipo.

1. In qualsiasi visualizzazione fare clic sul nome di un record.

   Viene visualizzata la casella di anteprima del record.

1. (Facoltativo) Fai clic sull&#39;icona ![](assets/open-details-in-a-new-tab-icon.png) di **Apri in una nuova scheda** per aprire la pagina del record.

1. Scegliere la scheda **Dettagli**. Per impostazione predefinita, viene aperta la scheda Dettagli.

1. Fai clic sull&#39;icona **Esporta** ![](assets/export-icon-in-record-details-page.png) nell&#39;anteprima o nella pagina del record, quindi fai clic su una delle seguenti opzioni:

   * **Microsoft Word**
   * <span class="preview">**Adobe PDF**</span>

   Un file Word (.docx) <span class="preview">o PDF</span> viene scaricato e salvato nel computer.

   Il nome del file esportato è il campo Principale del record.

   ![](assets/exported-word-file.png)

   >[!NOTE]
   >
   >    Le informazioni aggiuntive non visualizzate nella pagina e visibili solo dopo aver fatto clic su Mostra altro nella scheda Dettagli non vengono visualizzate nel file PDF esportato. Nel file esportato vengono visualizzate solo le informazioni visibili nella pagina.


1. (Facoltativo) Vai al file scaricato, aprilo e modificalo (se è un file di Word), o condividilo con altri.

