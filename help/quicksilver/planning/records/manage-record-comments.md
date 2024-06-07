---
title: Gestisci commenti record
description: È possibile collaborare ai record di Adobe Workfront Planning aggiungendo commenti o risposte nel pannello destro di un record. In quest'area è inoltre possibile visualizzare altre modifiche apportate al record e registrate dal sistema.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 0%

---

# Gestisci commenti record

{{planning-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

È possibile collaborare ai record di Adobe Workfront Planning aggiungendo commenti o risposte nel pannello destro di un record. In quest&#39;area è inoltre possibile visualizzare altre modifiche apportate al record e registrate dal sistema.

Nel pannello destro di un record vengono visualizzate le sezioni riportate di seguito.

* **Commenti**: visualizza i commenti e le risposte aggiunte dagli utenti ai record.
* **Cronologia**: visualizza le modifiche registrate dal sistema apportate dagli utenti ai campi record. Per ulteriori informazioni, consulta [Panoramica della sezione Cronologia](/help/quicksilver/planning/records/history-section-overview.md).

## Considerazioni sul commento a un record

* È possibile aggiungere commenti e risposte ai record in Workfront Planning, nella sezione Commenti di un record.

* I commenti aggiunti ai record collegati non vengono visualizzati nei record da cui si sta eseguendo il collegamento. Se ad esempio si commenta un record di prodotto di Workfront Planning collegato a un record di Campaign, il commento verrà visualizzato solo nel record di prodotto di Workfront Planning e non nel record di campagna da cui si sta effettuando il collegamento.

* È possibile aggiungere commenti ai record di Workfront Planning creati come risultato di una connessione tra un record e un oggetto di un&#39;altra applicazione.

  È ad esempio possibile aggiungere un commento al record Pianificazione di Workfront Project dopo aver collegato i progetti Workfront ai record Pianificazione di Workfront. Per ulteriori informazioni, consulta [Collega record](/help/quicksilver/planning/records/connect-records.md).

* I commenti aggiunti agli oggetti collegati in altre applicazioni non vengono visualizzati in Workfront Planning, mentre i commenti aggiunti agli oggetti collegati in Workfront Planning non vengono visualizzati in altre applicazioni.

  Ad esempio, i commenti aggiunti ai progetti in Workfront non vengono visualizzati sullo stesso progetto collegato a una campagna in Workfront Planning e i commenti aggiunti al record di pianificazione del progetto Workfront non vengono visualizzati in Workfront.

* Puoi assegnare tag agli utenti per attirare la loro attenzione su un aggiornamento. Gli utenti taggati non ricevono una notifica in-app o un’e-mail relativa all’aggiornamento. <!--this might change??-->

<!--replace the bullet above with this: * You can tag users to bring their attention to an update. Tagged users receive an in-app notification or an email notification about your update. 
   The following scenario exists:   

   * Adobe Unified Experience users receive both an in-app notification and an email notification. 
   * Users who are not in the Adobe Unified Experience receive only an email notification. 

      For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md)
   
      To determine whether your company is using the Adobe Unified Experience, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
      -->

* È possibile aggiungere un aggiornamento ai record ed esaminare la cronologia delle modifiche dalle seguenti aree di Workfront Planning:

   * Dalla pagina dei dettagli del record.
   * Da una visualizzazione, nella casella dei dettagli del record.

## Requisiti di accesso

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
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td>
   <td> <p>Nessun controllo del livello di accesso in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorizzazioni</p></td>
   <td> <p>Visualizzare o modificare le autorizzazioni per un'area di lavoro</a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle non create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modello di layout</p></td>
   <td> <p>L'amministratore del Workfront o del gruppo deve aggiungere l'area Planning nel modello di layout. Per informazioni, consulta <a href="/help/quicksilver/planning/access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

### Gestire i commenti sui record

{{step1-to-planning}}

1. Fai clic sulla scheda di un’area di lavoro.

   L&#39;area di lavoro si apre e i tipi di record vengono visualizzati sulle schede.

1. Fare clic su una scheda del tipo di record.
Viene visualizzata la pagina del tipo di record e vengono visualizzati tutti i record di quel tipo.

1. Scegliere una vista tabella dal menu **Visualizza** menu a discesa.
1. Fare clic sul nome di un record nella vista tabella.

   Il record **Dettagli** viene visualizzata la pagina. L’area Commenti (Comments) viene visualizzata per impostazione predefinita nel pannello di destra.

1. (Condizionale) Se il pannello a destra non si apre per impostazione predefinita, fai clic sul pulsante **Mostra commenti** ![](assets/show-comments-icon.png) nell’angolo in alto a destra per aprire la sezione Commenti.

1. Inizia a immettere un commento in **Nuovo commento** casella.

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Se si esce dalla sezione Commenti prima di completare la digitazione e l&#39;invio di un commento, il commento nella pagina viene mantenuto in modalità bozza anche dopo la disconnessione e la riconnessione. Nella bozza vengono salvate anche tutte le immagini aggiunte al commento. Le bozze vengono salvate per 7 giorni dopo i quali vengono eliminate e non possono essere recuperate. I commenti bozza sono visibili solo all&#39;utente che li inserisce.

1. (Facoltativo) Per annullare o ripristinare una modifica, utilizzare i seguenti tasti di scelta rapida:
   * CTRL + Z (⌘+z per Mac) per annullare una modifica
   * CTRL+Y (⌘+y per Mac) per ripetere una modifica
1. (Facoltativo) Aggiungi **@** seguito dal nome di un utente per assegnare un tag a qualcuno nell’aggiornamento.

   <!--Adobe Unified Experience users can receive an in-app and an email notification when they are tagged. All other users receive an email when they are tagged. For more information, see the section [Considerations about commenting on a record](#considerations-about-commenting-on-a-record) in this article. -->

1. (Facoltativo) Utilizza le opzioni nella barra degli strumenti Testo formattato per formattare il testo, aggiungere emoticon, collegamenti o immagini all’aggiornamento, per migliorare i contenuti. Per ulteriori informazioni, consulta la sezione &quot;Utilizzare Rich Text in un aggiornamento di Workfront&quot; nell’articolo [Aggiorna lavoro](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >Se un altro utente invia un commento allo stesso elemento che si sta aggiornando, viene visualizzata una linea rossa con un indicatore &quot;Nuovo&quot; per informare l&#39;utente dei commenti più recenti.
   >
   >L’indicatore viene visualizzato solo dopo che il commento è stato inviato sull’elemento e non quando il commento è ancora composto.
   >
   >![](assets/new-line-indicator-comments.png)

1. Clic **Invia** per aggiungere l&#39;aggiornamento al record.
1. (Facoltativo) Per modificare un commento, fai clic su **Altro** menu ![](assets/more-menu.png) nell’angolo superiore destro del commento, quindi fai clic su **Modifica**.

   >[!IMPORTANT]
   >
   >È possibile modificare il commento solo entro 15 minuti dall&#39;invio.

1. Modifica le informazioni nel commento, aggiungi o rimuovi immagini o rimuovi gli utenti taggati. Un indicatore &quot;modificato&quot; viene aggiunto a sinistra del commento.

   >[!TIP]
   >
   >Nei commenti relativi all&#39;anno corrente non viene visualizzato l&#39;anno nel timbro data. Passando il puntatore del mouse su una marca temporale viene visualizzata la data completa, incluso l’anno.

1. (Facoltativo e condizionale) Per cercare un commento esistente, inizia a digitare una parola chiave nella casella di ricerca nell&#39;angolo superiore destro del **Commenti** area.

   ![](assets/search-box-for-comments-area.png)

1. (Facoltativo) Fai clic su **Rispondi** o inizia a digitare un commento nel **Aggiungi risposta...** per rispondere a un commento esistente, quindi seguire i passaggi 4-8 sopra. <!--(**************accurate??***********)-->

1. (Condizionale e facoltativo) Se altri utenti hanno aggiunto commenti visualizzati al di fuori dell’area visibile nella sezione Commenti durante l’aggiunta dei commenti, fai clic su **Visualizza** all&#39;interno del **banner nuovi commenti** nella parte inferiore dello schermo per visualizzare questi commenti.

   ![](assets/new-comments-banner-on-record.png)

   Ulteriori commenti vengono visualizzati nella parte inferiore dello schermo.

1. (Facoltativo) Fai clic su **Mi piace** o confermare di averlo letto. L’icona si aggiorna con il numero di Mi piace.
1. (Condizionale e facoltativo) Se hai incluso altre persone nel commento, fai clic sugli avatar degli utenti inclusi nell’aggiornamento per visualizzare un elenco di utenti con cui il commento è condiviso.
1. (Facoltativo) Fai clic su **Altro** icona ![](assets/more-menu.png) nell&#39;angolo superiore destro del commento e fare clic su una delle opzioni seguenti per copiare un&#39;informazione da un commento:

   * **Copia collegamento**: copia negli Appunti un collegamento al commento.
   * **Copia corpo del testo**: copia il testo del commento negli Appunti.
   * **Risposta preventivo**: copia il contenuto del commento in una nuova risposta. Le immagini non sono incluse nella risposta copiata.

   Per ulteriori informazioni, consulta [Aggiorna lavoro](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Facoltativo) Fai clic su **Altro** icona ![](assets/more-menu.png) nell’angolo superiore destro del commento, quindi fai clic su **Elimina** per eliminare il commento.
1. (Facoltativo) Fai clic su **Nascondi commenti** icona ![](assets/hide-comments-icon.png) per chiudere il pannello destro.

## Panoramica della sezione Cronologia

È possibile esaminare le modifiche apportate al record nella sezione Cronologia del pannello di destra di un record.

Per ulteriori informazioni, consulta [Panoramica della sezione Cronologia](/help/quicksilver/planning/records/history-section-overview.md).
