---
title: Aggiungere una copertina a un record
description: È possibile personalizzare i record aggiungendo un'immagine di copertina alla pagina dei record in Adobe Workfront Planning durante la modifica di un record.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 8a4da96562b18977f56567f0fc5f72b369078432
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---


<!--update the metadata with real information-->

# Aggiungere una copertina a un record

{{planning-important-intro}}

È possibile personalizzare i record aggiungendo un&#39;immagine di copertina alla pagina dei record in Adobe Workfront Planning durante la modifica di un record.

Per informazioni sulla modifica dei record, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

È necessario creare i tipi di record prima di iniziare a creare e modificare i record.

Per informazioni, consulta [Crea tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

## Requisiti di accesso

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding cover images-->

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
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td>
   <td>
   <p>Nuovo: Standard</p>  
   <p>Corrente: Piano</p>   
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurazioni del livello di accesso</p></td>
   <td> <p>Nessun controllo di accesso per Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Gestire le autorizzazioni per un’area di lavoro </p>  
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

*Per ulteriori informazioni, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

   Nella vista tabella, fare clic sul pulsante **Apri dettagli** icona ![](assets/open-details-icon-in-table-name-field.png) nella prima colonna.

   L&#39;anteprima del record viene visualizzata nella vista.

   ![](assets/details-box.png)

1. (Facoltativo) Fai clic su **Apri in una nuova scheda** icona ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> nell&#39;angolo superiore destro dell&#39;anteprima del record per aprire la pagina del record in una nuova scheda.

   Viene visualizzata la pagina del record.

   ![](assets/details-page.png)

1. Nell&#39;anteprima del record o nella pagina, fare clic su **Aggiungi copertina**


   Oppure

   Passa il puntatore del mouse su un&#39;immagine di copertina esistente e fai clic su **Altro** menu ![](assets/more-menu.png) , quindi fai clic su **Carica**. <!--check the casing here; I logged a bug for this-->
Il **Registra copertina** La casella si apre in **Carica** scheda.

   ![](assets/record-cover-box-for-upload.png)

1. Clic **Sfoglia immagini** e cercare un&#39;immagine nel computer per selezionarla e aggiungerla.

1. (Facoltativo) Per rimuovere l&#39;immagine prima di salvarla, fare clic sul pulsante **Carica nuova immagine** icona ![](assets/upload-new-image-icon.png) , e carica una nuova immagine.

1. (Facoltativo) Fai clic su **Galleria** , quindi fare clic su un&#39;immagine nella raccolta di immagini. Impossibile modificare la raccolta di immagini.

   ![](assets/record-cover-box-for-gallery.png)

1. Clic **Usa immagine**.

   L’immagine viene caricata nella parte superiore dell’anteprima del record o della pagina e le modifiche vengono salvate automaticamente.

   ![](assets/record-page-with-cover-image.png)

1. (Facoltativo) Passa il puntatore sull&#39;immagine, quindi fai clic sul pulsante **Altro** menu ![](assets/more-menu.png) nell&#39;angolo inferiore destro dell&#39;immagine di copertina, quindi eseguire una delle operazioni seguenti:

   * Clic **Carica** se si desidera sostituire l&#39;immagine di copertina e ripetere il passaggio 6 per caricare e salvare una nuova immagine.
   * Clic **Riposiziona**, e utilizzare il **Riposiziona** strumento ![](assets/reposition-tool-icon.png) per centrare l&#39;immagine di copertina, quindi fare clic su **Salva** al termine.
   * Clic **Rimuovi** per rimuovere l&#39;immagine di copertina

   Workfront salva automaticamente le modifiche.
