---
title: Aggiungere una miniatura a un record
description: È possibile modificare le informazioni dei record in Adobe Workfront Planning e associare ogni record a singole miniature per renderle facilmente riconoscibili.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 0%

---

<!--update the metadata with real information-->

# Aggiungere una miniatura a un record

{{maestro-important-intro}}

È possibile associare record a miniature univoche in Adobe Workfront Planning per renderle facilmente riconoscibili.

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

{{step1-to-maestro}}

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
