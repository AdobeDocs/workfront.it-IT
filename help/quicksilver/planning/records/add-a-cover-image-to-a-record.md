---
title: Aggiungere un'immagine di copertina a un record
description: È possibile personalizzare i record aggiungendo un'immagine di copertina alla pagina dei record in Adobe Workfront Planning durante la modifica di un record.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---


# Aggiungere una copertina a un record

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

È possibile personalizzare i record aggiungendo un&#39;immagine di copertina alla pagina dei record in Adobe Workfront Planning durante la modifica di un record.

Per informazioni sulla modifica dei record, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

È necessario creare i tipi di record prima di iniziare a creare e modificare i record.

Per informazioni, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

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
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
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
   <td>   <p>Contribute or higher permissions to a workspace and record type  </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## Considerazioni sulle immagini di copertina della pagina di registrazione

È possibile personalizzare la pagina di un record aggiungendo un&#39;immagine di copertina.

Considera quanto segue:

* Un&#39;immagine di copertina è univoca per un record e non si applica a tutti i record dello stesso tipo.
* È possibile aggiungere solo file di immagine come immagini di copertina.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* È possibile aggiungere un&#39;immagine di copertina ai singoli record dall&#39;anteprima del record in qualsiasi visualizzazione o dalla pagina del record.
* Non è possibile aggiungere immagini di copertina da una visualizzazione record.
* Workfront carica automaticamente un&#39;immagine di copertina ogni volta che si crea un record. In seguito potrai modificare questa immagine.

## Aggiungere una copertina a un record

È possibile personalizzare un record aggiungendo un&#39;immagine di copertina nella parte superiore dell&#39;anteprima del record o della pagina.

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera personalizzare i record.

   Oppure

   Da un workspace, espandere la freccia rivolta verso il basso a destra del nome di un workspace esistente, cercare un workspace e selezionarlo quando viene visualizzato nell&#39;elenco.

   Viene aperto il workspace e vengono visualizzati i tipi di record.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

1. In una visualizzazione di qualsiasi tipo, fare clic su un record

   Oppure

   Dalla vista tabella, fare clic sull&#39;icona **Apri dettagli** ![Apri dettagli icona](assets/open-details-icon-in-table-name-field.png) nella prima colonna.

   L&#39;anteprima del record viene visualizzata nella vista.

   ![Anteprima dettagli](assets/details-box.png)


1. (Facoltativo) Fai clic sull&#39;icona **Apri in una nuova scheda** ![Apri in una nuova scheda](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> nell&#39;angolo superiore destro dell&#39;anteprima del record per aprire la pagina del record in una nuova scheda.

   Viene visualizzata la pagina del record.

   ![Pagina dettagli](assets/details-page.png)

1. Nella pagina di anteprima o dettagli del record, passa il cursore del mouse sullo spazio sopra il nome del record, quindi fai clic su **Aggiungi copertina**.

   Oppure

   Passa il puntatore del mouse su un&#39;immagine di copertina esistente e fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) , quindi su **Carica**. <!--check the casing here; I logged a bug for this-->
La casella **Copertina record** si apre nella scheda **Carica**.

   ![Casella di copertina record per il caricamento](assets/record-cover-box-for-upload.png)

1. Fare clic su **Sfoglia immagini** e cercare un&#39;immagine nel computer per selezionarla e aggiungerla.

1. (Facoltativo) Per rimuovere l&#39;immagine prima che venga salvata, fai clic sull&#39;icona **Carica nuova immagine** ![Carica nuova immagine](assets/upload-new-image-icon.png) e carica una nuova immagine.

1. (Facoltativo) Fai clic sulla scheda **Galleria**, quindi fai clic su un&#39;immagine nella raccolta di immagini. Impossibile modificare la raccolta di immagini.

   ![Casella di copertina record per la raccolta](assets/record-cover-box-for-gallery.png)

1. Fare clic su **Usa immagine**.

   L’immagine viene caricata nella parte superiore della pagina dei dettagli o dell’anteprima del record e le modifiche vengono salvate automaticamente.

   ![Registra pagina con immagine di copertina](assets/record-page-with-cover-image.png)

1. (Facoltativo) Passa il puntatore del mouse sull&#39;immagine, quindi fai clic sul menu **Altro** ![Altro menu](assets/more-menu.png) nell&#39;angolo inferiore destro dell&#39;immagine di copertina, quindi effettua una delle seguenti operazioni:

   * Fare clic su **Carica** se si desidera sostituire l&#39;immagine di copertina e ripetere il passaggio 6 per caricare e salvare una nuova immagine.
   * Fai clic su **Riposiziona** e utilizza lo strumento **Riposiziona** ![Icona strumento di riposizionamento](assets/reposition-tool-icon.png) per centrare l&#39;immagine di copertina, quindi al termine fai clic su **Salva**.
   * Fai clic su **Rimuovi** per rimuovere l&#39;immagine di copertina.

   Workfront salva automaticamente le modifiche.
