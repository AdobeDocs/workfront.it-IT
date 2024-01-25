---
title: Gestisci commenti record
description: Puoi collaborare ai record Adobe Maestro aggiungendo commenti o risposte nel pannello destro di un record. In quest'area è inoltre possibile visualizzare altre modifiche apportate al record e registrate dal sistema.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 54c6adf51ab8ef4e7968e8fdeeb0025e42deecc5
workflow-type: tm+mt
source-wordcount: '1155'
ht-degree: 0%

---


# Gestisci commenti record

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Maestro records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

Puoi collaborare ai record Adobe Maestro aggiungendo commenti o risposte nel pannello destro di un record. In quest&#39;area è inoltre possibile visualizzare altre modifiche apportate al record e registrate dal sistema.

Nel pannello destro di un record vengono visualizzate le sezioni riportate di seguito.

* **Commenti**: visualizza i commenti e le risposte aggiunte dagli utenti ai record.
* **Cronologia**: visualizza le modifiche registrate dal sistema apportate dagli utenti ai campi record. Per ulteriori informazioni, consulta [Panoramica della sezione Cronologia](/help/quicksilver/maestro/records/history-section-overview.md).

>[!TIP]
>
>Il pannello a destra mostra sia i record operativi che quelli di tassonomia.


## Considerazioni sul commento a un record

* È possibile aggiungere commenti e risposte ai record operativi e alle tassonomie in Maestro, nella sezione Commenti di un record.

* I commenti aggiunti ai record collegati non vengono visualizzati nei record da cui si sta eseguendo il collegamento. Ad esempio, se commenti un record Prodotto Maestro collegato a un record Campagna, il commento viene visualizzato solo sul record Prodotto in Maestro e non sul record Campagna da cui stai effettuando il collegamento.

* È possibile aggiungere commenti ai record Maestro creati come risultato di una connessione tra un record Maestro e un oggetto di un&#39;altra applicazione.

  Ad esempio, puoi commentare il record Project Maestro dopo aver collegato i progetti Workfront ai record Maestro. Per ulteriori informazioni, consulta [Collega record](/help/quicksilver/maestro/records/connect-records.md).

* I commenti aggiunti agli oggetti collegati in altre applicazioni non vengono visualizzati in Maestro e i commenti aggiunti agli oggetti collegati in Maestro non vengono visualizzati in altre applicazioni.

  Ad esempio, i commenti aggiunti ai progetti in Workfront non vengono visualizzati sullo stesso progetto collegato a una campagna in Maestro e i commenti aggiunti al progetto Maestro non vengono visualizzati in Workfront.

* Puoi assegnare tag agli utenti per attirare la loro attenzione su un aggiornamento. Gli utenti taggati non ricevono una notifica in-app o un’e-mail relativa all’aggiornamento. <!--this might change??-->

* Puoi aggiungere un aggiornamento ai record e rivedere la cronologia delle modifiche dalle seguenti aree di Maestro:

   * Dalla pagina Dettagli di un record o di una tassonomia.

  <!--* From the table view.-->

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
<p>La tua organizzazione deve essere iscritta al programma beta chiuso Adobe Maestro. Per informazioni su questa nuova offerta, contatta il rappresentante del tuo account. </p>
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
   <td> <p>Maestro non dispone di controlli del livello di accesso. </p>  
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
   <td> <p>L’amministratore del Workfront o del gruppo deve aggiungere l’area Maestro nel modello di layout. Per informazioni, consulta <a href="../access/access-overview.md">Panoramica degli accessi</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

### Gestire i commenti sui record

{{step1-to-maestro}}

Per impostazione predefinita, viene aperta l’ultima area di lavoro a cui si è effettuato l’accesso.
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
1. (Facoltativo) Utilizza le opzioni nella barra degli strumenti Testo formattato per formattare il testo, aggiungere emoticon, collegamenti o immagini all’aggiornamento, per migliorare i contenuti. Per ulteriori informazioni, consulta la sezione &quot;Utilizzare Rich Text in un aggiornamento di Workfront&quot; nell’articolo [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

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

   Per ulteriori informazioni, consulta [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Facoltativo) Fai clic su **Altro** icona ![](assets/more-menu.png) nell’angolo superiore destro del commento, quindi fai clic su **Elimina** per eliminare il commento.
1. (Facoltativo) Fai clic su **Nascondi commenti** icona ![](assets/hide-comments-icon.png) per chiudere il pannello destro.

## Panoramica della sezione Cronologia

È possibile esaminare le modifiche apportate al record nella sezione Cronologia del pannello di destra di un record operativo o di una tassonomia.

Per ulteriori informazioni, consulta [Panoramica della sezione Cronologia](/help/quicksilver/maestro/records/history-section-overview.md).

