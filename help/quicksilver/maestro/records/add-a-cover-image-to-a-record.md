---
title: Aggiungere una copertina a un record
description: È possibile personalizzare i record aggiungendo un'immagine di copertina alla pagina dei record in Adobe Workfront Planning durante la modifica di un record.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 2f8a5b2d2183090029966a13c7af37f20eb44fd0
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---


<!--update the metadata with real information-->

# Aggiungere una copertina a un record

{{maestro-important-intro}}

È possibile personalizzare i record aggiungendo un&#39;immagine di copertina alla pagina dei record in Adobe Workfront Planning durante la modifica di un record.

Per informazioni sulla modifica dei record, vedere [Modifica record](/help/quicksilver/maestro/records/edit-records.md).

È necessario creare i tipi di record prima di iniziare a creare e modificare i record.

Per informazioni, consulta [Crea tipi di record](../architecture/create-record-types.md).

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
<p>La tua organizzazione deve essere iscritta al programma beta di Adobe Workfront Planning. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
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
   <td>  <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p> <p>Per informazioni, consulta <a href="/help/quicksilver/maestro/access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## Considerazioni sulle immagini di copertina della pagina di registrazione

È possibile personalizzare la pagina di un record aggiungendo un&#39;immagine di copertina.

Considera quanto segue:

* Un&#39;immagine di copertina è univoca per un record e non si applica a tutti i record dello stesso tipo.
* È possibile aggiungere solo file di immagine come immagini di copertina.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* È possibile aggiungere un&#39;immagine di copertina ai singoli record dalla casella del record in qualsiasi visualizzazione o dalla pagina del record.
* Non è possibile aggiungere immagini di copertina in linea da nessuna visualizzazione di record.

## Aggiungere una copertina a un record

È possibile personalizzare un record aggiungendo un&#39;immagine di copertina nella parte superiore della casella del record o della pagina.

{{step1-to-maestro}}

Viene aperto l&#39;ultimo workspace a cui si è autorizzati ad accedere.

1. (Facoltativo) Fare clic sulla freccia rivolta verso il basso a destra del nome del workspace per selezionare il workspace di cui si desidera aggiornare i record.

1. Fare clic su una scheda del tipo di record.

   Viene visualizzata la pagina del tipo di record.

1. In una visualizzazione di qualsiasi tipo fare clic sul nome di un record

   Oppure

   Nella vista tabella, fare clic sul pulsante **Apri dettagli** icona ![](assets/open-details-icon-in-table-name-field.png) a sinistra del nome di un record.

   La casella del record viene visualizzata nella vista.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >È possibile visualizzare **Apri dettagli** a sinistra del campo Nome di un record in una visualizzazione tabella solo quando il campo Nome è un campo primario.

1. (Facoltativo) Fai clic su **Apri in una nuova scheda** icona ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> nell&#39;angolo superiore destro della casella record per aprire la pagina del record in una nuova scheda.

   Viene visualizzata la pagina del record.

   ![](assets/details-page.png)

1. Nella casella o nella pagina del record fare clic su **Aggiungi copertina**. <!--check the casing here; I logged a bug for this-->
Il **Registra copertina** viene visualizzata la casella.

1. Clic **Seleziona per caricare** e cercare un&#39;immagine nel computer per selezionarla, aggiungerla, quindi fare clic su **Usa immagine**.

   L’immagine viene caricata nella parte superiore della casella o della pagina di record e le modifiche vengono salvate automaticamente.

   ![](assets/record-page-with-cover-image.png)

1. (Facoltativo) Passa il puntatore sull&#39;immagine, quindi fai clic sul pulsante **Altro** menu ![](assets/more-menu.png) nell&#39;angolo inferiore destro dell&#39;immagine di copertina, quindi eseguire una delle operazioni seguenti:

   * Clic **Carica** se si desidera sostituire l&#39;immagine di copertina e ripetere il passaggio 6 per caricare e salvare una nuova immagine.
   * Clic **Riposiziona**, e utilizzare il **Riposiziona** strumento ![](assets/reposition-tool-icon.png) per centrare l&#39;immagine di copertina, quindi fare clic su **Salva** al termine.
   * Clic **Rimuovi** per rimuovere l&#39;immagine di copertina

   Workfront salva automaticamente le modifiche.
