---
title: Aggiungere una miniatura a un record
description: È possibile modificare le informazioni dei record in Adobe Workfront Planning e associare ogni record a singole miniature per renderle facilmente riconoscibili.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 3856e56036a9845387d7dc6498a6f20728c8234a
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

<!--update the metadata with real information-->

# Aggiungere una miniatura a un record

{{planning-important-intro}}

È possibile associare record a miniature univoche in Adobe Workfront Planning per renderle facilmente riconoscibili.

È necessario creare i tipi di record prima di iniziare a creare e modificare i record.
Per informazioni, consulta [Crea tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

## Requisiti di accesso

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <td role="rowheader"><p>Licenza Adobe Workfront</p></td>
   <td>
   <p>Qualsiasi</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td>
   <td> <p>Nessun controllo di accesso per Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Contribuire o concedere autorizzazioni superiori a un’area di lavoro </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td>  <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p> <p>Per informazioni, consulta <a href="/help/quicksilver/planning/access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## Considerazioni sulle miniature dei record

Per distinguere visivamente i record in una vista tabella, è possibile associare a ciascun record un&#39;immagine miniatura univoca.

Considera quanto segue:

* È possibile aggiungere solo file di immagine come miniature.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* È possibile aggiungere un&#39;immagine di anteprima ai singoli record nella visualizzazione per tabella.
* Le miniature appartengono alle informazioni sui record e vengono visualizzate nelle visualizzazioni in cui vengono visualizzati i record. Ad esempio, le miniature vengono visualizzate insieme alle informazioni del record nelle seguenti aree:

   * Campo principale di un record nella visualizzazione tabella
   * Barra dei record nella visualizzazione timeline.
* Non è possibile aggiungere miniature di record dalla pagina del record o da un altro tipo di visualizzazione.
* Le miniature non vengono visualizzate sulla pagina del record.

## Aggiungere una miniatura a un record

{{step1-to-planning}}

1. Selezionare l&#39;area di lavoro per i cui record si desidera aggiungere le miniature, quindi fare clic sulla scheda del tipo di record.

   Verrà aperta la pagina del tipo di record.
1. Selezionare una vista tabella dal menu **Visualizza** menu a discesa. Tutti i record del tipo selezionato vengono visualizzati in una tabella.
1. Passa il puntatore del mouse sulle informazioni del campo principale, fai clic sul pulsante **Altro** menu ![](assets/more-menu.png), quindi fai clic su **Miniatura**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   Il campo principale è il campo che viene visualizzato nella prima colonna di una visualizzazione tabella. Il campo principale è sempre bloccato e non può essere nascosto o spostato.

   Il **Miniatura record** viene visualizzata la casella.

   ![](assets/record-thumbnail-box-for-upload.png)

   <!--update screen shot with correct casing-->

1. In **Carica** , trascinare e rilasciare un file da aggiungere come miniatura o fare clic su **Seleziona per caricare**, quindi cerca un file di immagine da aggiungere. Il file deve essere salvato nel computer.
1. (Facoltativo) Usate lo strumento di ridimensionamento per ritagliare e ridimensionare l&#39;immagine.
1. Clic **Usa immagine** per aggiungere l&#39;immagine come miniatura.
Questo chiude il **Miniatura record** casella.
1. (Condizionale) Se disponete almeno delle autorizzazioni Contribute per la vista tabella, fate clic su **Campi** nell&#39;angolo superiore destro della vista tabella.
1. Seleziona la **Miniatura** per visualizzare la miniatura. Questa opzione è deselezionata per impostazione predefinita.

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   La miniatura viene visualizzata a sinistra del valore del campo primario.
1. (Facoltativo e condizionale) Se non disponete di autorizzazioni Contribute o di livello superiore per la visualizzazione, selezionate una nuova visualizzazione dal menu **Visualizza** menu a discesa o creare una vista.
1. (Facoltativo) Per rimuovere la miniatura, passa il cursore sul campo principale e fai clic sul pulsante **Altro** menu ![](assets/more-menu.png)> **Miniatura** > il **Rimuovi** icona ![](assets/remove-image-icon.png), quindi fai clic su **Salva modifiche**.

<!--
Replace the section above with the following when we release generate thumbnails:

## Add a thumbnail to a record

You can add a thumbnail to a record in the following ways:

* Upload a file from your computer
* Generate an image with a prompt

### Upload a thumbnail to a record

{{step1-to-planning}}

1. Select the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![](assets/more-menu.png), then click **Thumbnail**. 

   ![](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

   ![](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Upload** tab, and drag and drop a file to add as a thumbnail
   Or
   Click **Select to upload**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) Use the sizing tool to crop and resize the image.
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
1. (Conditional) If you have at least Contribute permissions to the table view, click **Fields** in the upper-right corner of the table view. 
1. Select the **Thumbnail** toggle to display the thumbnail. This is deselected by default. 

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   The thumbnail displays to the left of the primary field value. 
1. (Optional and conditional) If you do not have Contribute or higher permissions to the view, select a new view from the **View** drop-down menu, or create a view. 
1. (Optional) To remove the thumbnail, hover over the primary field and click the **More** menu ![](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![](assets/remove-image-icon.png), then click **Save changes**.

### Generate a thumbnail for a record

{{step1-to-planning}}

1. Select the workspace for whose records you want to add thumbnails, then click the record type card. 

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