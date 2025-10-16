---
title: Aggiungere una miniatura a un record
description: È possibile modificare le informazioni dei record in Adobe Workfront Planning e associare ogni record a singole miniature per renderle facilmente riconoscibili.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---


# Aggiungere una miniatura a un record

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

È possibile associare record a miniature univoche in Adobe Workfront Planning per renderle facilmente riconoscibili.

È necessario creare i tipi di record prima di iniziare a creare e modificare i record.
Per informazioni, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

## Requisiti di accesso

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <td><p> Standard </p>
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
   <td>   <p>Contribute or higher permissions to a workspace and record type  </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->


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
1. Passa il puntatore del mouse sulle informazioni del campo principale, fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png), quindi fai clic su **Miniatura**.

   ![Registra altro menu espanso](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   Il campo principale è il campo che viene visualizzato nella prima colonna di una visualizzazione tabella. Il campo principale è sempre bloccato e non può essere nascosto o spostato. L&#39;opzione Miniatura non è disponibile nel menu Altro quando il campo principale è un campo formula.

   Per impostazione predefinita, nella casella **Miniatura record** viene aperta la scheda **Carica**.

   Per ulteriori informazioni sul caricamento della miniatura, vedere la sezione [Aggiungere una miniatura a un record dalla pagina dei dettagli](#add-a-thumbnail-to-a-record-from-the-details-page) in questo articolo, a partire dal passaggio 6. <!--see if this is accurate-->

<!--
   ![Record thumbnail box for upload](assets/record-thumbnail-box-for-upload.png) 

  *****update screen shot with correct casing****

1. Drag and drop a file to add as a thumbnail
   
   Or
   
   Click **Browse images**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) After the image uploads in the **Record thumbnail** box, use the sizing tool to crop and resize the image.
1. (Optional) Click the **Upload new image** icon ![Upload new image icon](assets/upload-new-image-icon.png) to upload another image. 
1. (Optional) To remove a thumbnail before it is saved, click  **Remove uploaded image** icon ![Remove image icon](assets/remove-image-icon.png) to the right of the image. 
1. (Optional) Click the **Gallery** tab, then click an image. The gallery of images cannot be modified.

   ![Record thumbnail box for gallery](assets/record-thumbnail-box-for-gallery.png)
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
   The thumbnail displays in areas of Workfront Planning where the record displays. 

   >[!TIP]
   >
   >   You must enable the Thumbnail field in the table view to display thumbnails in this view. It is disabled by default.

1. (Optional) To remove the thumbnail after it is saved, hover over the primary field and click the **More** menu ![More menu](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![Remove image icon](assets/remove-image-icon.png), then click **Save changes**. -->

### Aggiungere una miniatura a un record dalla pagina dei dettagli

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro per i record ai quali si desidera aggiungere le miniature, quindi fare clic sulla scheda del tipo di record.

   Verrà aperta la pagina del tipo di record.
1. In qualsiasi visualizzazione, fare clic su un record per aprirlo.

   Viene visualizzata la casella di anteprima dei dettagli.
1. (Facoltativo) Fai clic sull&#39;icona **Apri in una nuova scheda** ![Apri i dettagli in una nuova scheda](assets/open-details-in-a-new-tab-icon.png) nell&#39;angolo superiore destro.

   Viene visualizzata la pagina dei dettagli del record.

1. (Facoltativo) Nella pagina dei dettagli o dell&#39;anteprima del record, passa il cursore del mouse sull&#39;immagine miniatura o sull&#39;icona ![Icona miniatura record nella pagina dei dettagli](assets/record-thumbnail-icon-on-details-page.png), passa il puntatore del mouse sullo spazio sopra il nome del record e fai clic su **Aggiungi miniatura** o **Modifica miniatura**.

   Per impostazione predefinita, nella casella **Miniatura record** viene aperta la scheda **Carica**.

   ![Casella delle miniature dei record da caricare](assets/record-thumbnail-box-for-upload.png)

1. Trascina un file da aggiungere come miniatura

   Oppure

   Fai clic su **Sfoglia immagini**, quindi cerca un file di immagine da aggiungere. Il file deve essere salvato nel computer.

1. (Facoltativo) Dopo il caricamento dell&#39;immagine nella casella **Miniatura record**, utilizzare lo strumento di ridimensionamento per ritagliare e ridimensionare l&#39;immagine.
1. (Facoltativo) Fai clic sull&#39;icona **Carica nuova immagine** ![Carica nuova immagine](assets/upload-new-image-icon.png) per caricare un&#39;altra immagine.
1. (Facoltativo) Fai clic sulla scheda **Galleria**, quindi su un&#39;immagine. Impossibile modificare la raccolta di immagini.

   ![Casella miniature record per la raccolta](assets/record-thumbnail-box-for-gallery.png)

1. (Facoltativo) Per rimuovere la miniatura prima del salvataggio, fare clic sull&#39;icona **Rimuovi** ![Rimuovi icona immagine](assets/remove-image-icon.png) a destra dell&#39;immagine.

1. Fare clic su **Utilizza immagine** per aggiungere l&#39;immagine come miniatura.
Chiude la casella **Miniatura record**.
La miniatura viene visualizzata nelle aree di Workfront Planning in cui viene visualizzato il record.

   >[!TIP]
   >
   >   Per visualizzare le miniature in questa visualizzazione, è necessario attivare il campo Miniatura nella visualizzazione Tabella. Per impostazione predefinita, è disabilitata.

1. (Facoltativo) Per rimuovere la miniatura dopo averla salvata, fai clic su un record in una visualizzazione qualsiasi per aprire la pagina dei dettagli, quindi passa il puntatore sull&#39;immagine miniatura e fai clic sul menu **Altro** ![Icona altro menu](assets/more-menu.png)> **Rimuovi** icona ![Rimuovi icona](assets/remove-image-icon.png). L&#39;immagine di anteprima viene rimossa.


<!--
### Generate a thumbnail for a record

{{step1-to-planning}}

1. Click the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![More menu](assets/more-menu.png), then click **Thumbnail**. 

   ![Record more menu expanded](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![Record thumbnail box for upload](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->
