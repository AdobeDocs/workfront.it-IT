---
title: Aggiungere una miniatura a un record
description: È possibile modificare le informazioni dei record in Adobe Workfront Planning e associare ogni record a singole miniature per renderle facilmente riconoscibili.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---


# Aggiungere una miniatura a un record

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

È possibile associare record a miniature univoche in Adobe Workfront Planning per renderle facilmente riconoscibili.

È necessario creare i tipi di record prima di iniziare a creare e modificare i record.
Per informazioni, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

## Requisiti di accesso

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <td><p> Standard </p>
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
   <td>   <p>Gestire le autorizzazioni per un’area di lavoro </p>  
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

## Considerazioni sulle miniature dei record

Per distinguere visivamente i record in una vista tabella, è possibile associare a ciascun record un&#39;immagine miniatura univoca.

Considera quanto segue:

* Una miniatura è univoca per un record e non si applica a tutti i record dello stesso tipo.
* È possibile aggiungere solo file di immagine come miniature.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* È possibile aggiungere un&#39;immagine di anteprima ai singoli record nella vista tabella o dalla pagina o dalla casella di anteprima del record.
* Workfront carica automaticamente una miniatura ogni volta che crei un record. In seguito potrai modificare questa immagine.
* Le miniature appartengono alle informazioni del record e vengono visualizzate nelle aree in cui vengono visualizzati i record. Ad esempio, le miniature vengono visualizzate insieme alle informazioni del record nelle seguenti aree:

   * Campo principale di un record nella visualizzazione tabella
   * Barra dei record nella visualizzazione timeline.
   * L&#39;anteprima e la pagina dei dettagli del record.

## Aggiungere una miniatura a un record

È possibile aggiungere una miniatura nei modi seguenti:

* [Aggiungere una miniatura a un record dalla vista tabella](#add-a-thumbnail-to-a-record-from-the-table-view)
* [Aggiungere una miniatura a un record dalla pagina dei dettagli](#add-a-thumbnail-to-a-record-from-the-details-page)

### Aggiungere una miniatura a un record dalla vista tabella

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro per i record ai quali si desidera aggiungere le miniature, quindi fare clic sulla scheda del tipo di record.

   Verrà aperta la pagina del tipo di record.
1. Selezionare una visualizzazione tabella dal menu a discesa **Visualizza**. Tutti i record del tipo selezionato vengono visualizzati in una tabella.
1. Passa il puntatore del mouse sulle informazioni del campo primario, fai clic sul menu **Altro** ![](assets/more-menu.png), quindi fai clic su **Miniatura**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   Il campo principale è il campo che viene visualizzato nella prima colonna di una visualizzazione tabella. Il campo principale è sempre bloccato e non può essere nascosto o spostato. L&#39;opzione Miniatura non è disponibile nel menu Altro quando il campo principale è un campo formula.

   Per impostazione predefinita, nella casella **Miniatura record** viene aperta la scheda **Carica**.

   Per ulteriori informazioni sul caricamento della miniatura, vedere la sezione [Aggiungere una miniatura a un record dalla pagina dei dettagli](#add-a-thumbnail-to-a-record-from-the-details-page) in questo articolo, a partire dal passaggio 6. <!--see if this is accurate-->

<!--
   ![](assets/record-thumbnail-box-for-upload.png) 

  *****update screen shot with correct casing****

1. Drag and drop a file to add as a thumbnail
   
   Or
   
   Click **Browse images**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) After the image uploads in the **Record thumbnail** box, use the sizing tool to crop and resize the image.
1. (Optional) Click the **Upload new image** icon ![](assets/upload-new-image-icon.png) to upload another image. 
1. (Optional) To remove a thumbnail before it is saved, click  **Remove uploaded image** icon ![](assets/remove-image-icon.png) to the right of the image. 
1. (Optional) Click the **Gallery** tab, then click an image. The gallery of images cannot be modified.

   ![](assets/record-thumbnail-box-for-gallery.png)
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
   The thumbnail displays in areas of Workfront Planning where the record displays. 

   >[!TIP]
   >
   >   You must enable the Thumbnail field in the table view to display thumbnails in this view. It is disabled by default.

1. (Optional) To remove the thumbnail after it is saved, hover over the primary field and click the **More** menu ![](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![](assets/remove-image-icon.png), then click **Save changes**. -->

### Aggiungere una miniatura a un record dalla pagina dei dettagli

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro per i record ai quali si desidera aggiungere le miniature, quindi fare clic sulla scheda del tipo di record.

   Verrà aperta la pagina del tipo di record.
1. In qualsiasi visualizzazione, fare clic su un record per aprirlo.

   Viene visualizzata la casella di anteprima dei dettagli.
1. (Facoltativo) Fai clic sull&#39;icona ![](assets/open-details-in-a-new-tab-icon.png) in alto a destra **Apri in una nuova scheda**.

   Viene visualizzata la pagina dei dettagli del record.

1. (Condizionale) Nell&#39;anteprima del record o nella pagina, passa il puntatore sull&#39;immagine miniatura o sull&#39;icona ![](assets/record-thumbnail-icon-on-details-page.png), quindi fai clic sul menu **Altro** ![](assets/more-menu.png) > **Modifica miniatura** nell&#39;ambiente di produzione

   Oppure

   <span class="preview">Passa il puntatore del mouse sullo spazio sopra il nome del record, quindi fai clic su **Aggiungi miniatura** o su **Modifica miniatura** nell&#39;ambiente di anteprima.</span>

   Per impostazione predefinita, nella casella **Miniatura record** viene aperta la scheda **Carica**.

   ![](assets/record-thumbnail-box-for-upload.png)

1. Trascina un file da aggiungere come miniatura

   Oppure

   Fai clic su **Sfoglia immagini**, quindi cerca un file di immagine da aggiungere. Il file deve essere salvato nel computer.

1. (Facoltativo) Dopo il caricamento dell&#39;immagine nella casella **Miniatura record**, utilizzare lo strumento di ridimensionamento per ritagliare e ridimensionare l&#39;immagine.
1. (Facoltativo) Fai clic sull&#39;icona ![](assets/upload-new-image-icon.png) di **Carica nuova immagine** per caricare un&#39;altra immagine.
1. (Facoltativo) Fai clic sulla scheda **Galleria**, quindi su un&#39;immagine. Impossibile modificare la raccolta di immagini.

   ![](assets/record-thumbnail-box-for-gallery.png)

1. (Facoltativo) Per rimuovere la miniatura prima del salvataggio, fare clic sull&#39;icona **Rimuovi** ![](assets/remove-image-icon.png) a destra dell&#39;immagine.

1. Fare clic su **Utilizza immagine** per aggiungere l&#39;immagine come miniatura.
Chiude la casella **Miniatura record**.
La miniatura viene visualizzata nelle aree di Workfront Planning in cui viene visualizzato il record.

   >[!TIP]
   >
   >   Per visualizzare le miniature in questa visualizzazione, è necessario attivare il campo Miniatura nella visualizzazione Tabella. Per impostazione predefinita, è disabilitata.

1. (Facoltativo) Per rimuovere la miniatura dopo averla salvata, fai clic su un record in una visualizzazione qualsiasi per aprire la pagina dei dettagli, quindi passa il puntatore sull&#39;immagine miniatura e fai clic sul menu **Altro** ![](assets/more-menu.png)> icona **Rimuovi** ![](assets/remove-image-icon.png). L&#39;immagine di anteprima viene rimossa.




<!--
### Generate a thumbnail for a record

{{step1-to-planning}}

1. Click the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![](assets/more-menu.png), then click **Thumbnail**. 

   ![](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->