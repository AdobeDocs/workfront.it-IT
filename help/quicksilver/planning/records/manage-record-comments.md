---
title: Gestisci commenti record
description: È possibile collaborare ai record di Adobe Workfront Planning aggiungendo commenti o risposte nel pannello destro di un record. In quest'area è inoltre possibile visualizzare altre modifiche apportate al record e registrate dal sistema.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '959'
ht-degree: 0%

---

# Gestisci commenti record

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

È possibile collaborare ai record di Adobe Workfront Planning aggiungendo commenti o risposte nel pannello destro di un record. In quest&#39;area è inoltre possibile visualizzare altre modifiche apportate al record e registrate dal sistema.

Nel pannello destro di un record vengono visualizzate le sezioni riportate di seguito.

* **Commenti**: visualizza i commenti e le risposte aggiunte dagli utenti ai record.
* **Cronologia**: visualizza le modifiche registrate dal sistema apportate dagli utenti ai campi record. Per ulteriori informazioni, vedere [Panoramica della sezione Cronologia](/help/quicksilver/planning/records/history-section-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso.

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
   <td><p> Collaboratore, Light o Standard</p>
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
   <td>   <p>Visualizza o autorizzazioni superiori per un'area di lavoro <!--<span class="preview">and record type</span>--> </a> </p>  
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

## Considerazioni sul commento a un record

* È possibile aggiungere commenti e risposte ai record in Workfront Planning, nella sezione Commenti di un record.

* I commenti aggiunti ai record collegati non vengono visualizzati nei record da cui si sta eseguendo il collegamento. Se ad esempio si commenta un record di prodotto di Workfront Planning collegato a un record di Campaign, il commento verrà visualizzato solo nel record di prodotto di Workfront Planning e non nel record di campagna da cui si sta effettuando il collegamento.

* È possibile aggiungere commenti ai record di Workfront Planning creati come risultato di una connessione tra un record e un oggetto di un&#39;altra applicazione.

  È ad esempio possibile aggiungere un commento al record Pianificazione di Workfront Project dopo aver collegato i progetti Workfront ai record Pianificazione di Workfront. Per ulteriori informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

* I commenti aggiunti agli oggetti collegati in altre applicazioni non vengono visualizzati in Workfront Planning, mentre i commenti aggiunti agli oggetti collegati in Workfront Planning non vengono visualizzati in altre applicazioni.

  Ad esempio, i commenti aggiunti ai progetti in Workfront non vengono visualizzati sullo stesso progetto collegato a una campagna in Workfront Planning e i commenti aggiunti al record di pianificazione del progetto Workfront non vengono visualizzati in Workfront.

* Puoi assegnare tag agli utenti per attirare la loro attenzione su un aggiornamento. Gli utenti taggati non ricevono una notifica in-app o un’e-mail relativa all’aggiornamento. <!--this might change??-->

* Puoi assegnare tag agli utenti per attirare la loro attenzione su un aggiornamento. Gli utenti taggati ricevono una notifica in-app o una notifica e-mail relativa all’aggiornamento.

  >[!NOTE]
  >
  >   Solo gli utenti dei clienti che hanno effettuato l’onboarding con Adobe Unified Experience ricevono sia una notifica in-app che una notifica e-mail. Per determinare se la tua azienda utilizza l&#39;esperienza unificata di Adobe, consulta [Esperienza unificata di Adobe per Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* È possibile aggiungere un aggiornamento ai record ed esaminare la cronologia delle modifiche dalle seguenti aree di Workfront Planning:

   * Dalla pagina dei dettagli del record.
   * Da una visualizzazione, nella casella dei dettagli del record.

### Gestire i commenti sui record

{{step1-to-planning}}

1. Fai clic sulla scheda di un’area di lavoro.

   L&#39;area di lavoro si apre e i tipi di record vengono visualizzati sulle schede.

1. Fare clic su una scheda del tipo di record.
Viene visualizzata la pagina del tipo di record e vengono visualizzati tutti i record di quel tipo.

1. Scegliere una vista tabella dal menu a discesa **Visualizza**.
1. Fare clic sul nome di un record nella vista tabella.

   Viene aperta la pagina **Dettagli** del record. L’area Commenti (Comments) viene visualizzata per impostazione predefinita nel pannello di destra.

1. (Condizionale) Se per impostazione predefinita il pannello di destra non si apre, fai clic sull&#39;icona **Mostra commenti** ![Mostra commenti](assets/show-comments-icon.png) nell&#39;angolo superiore destro per aprire la sezione Commenti.

1. Inizia a immettere un commento nella casella **Nuovo commento**.

   ![Casella commenti vuota nel record](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Se si esce dalla sezione Commenti prima di completare la digitazione e l&#39;invio di un commento, il commento nella pagina viene mantenuto in modalità bozza anche dopo la disconnessione e la riconnessione. <!--this is no longer possible for records: Any images that are added to the comment are also saved in the draft. Drafts are saved for 7 days after which they are discarded and cannot be recovered. Drafted comments are only visible to the user entering them.-->

1. (Facoltativo) Per annullare o ripristinare una modifica, utilizzare i seguenti tasti di scelta rapida:
   * CTRL + Z (⌘+z per Mac) per annullare una modifica
   * CTRL+Y (⌘+y per Mac) per ripetere una modifica
1. (Facoltativo e condizionale) Se l&#39;istanza di Workfront fa parte di Adobe Unified Experience, aggiungi **@** seguito dal nome di un utente per assegnare un tag a qualcuno nell&#39;aggiornamento. Per ulteriori informazioni, vedere la sezione [Considerazioni sull&#39;inserimento di commenti in un record](#considerations-about-commenting-on-a-record) in questo articolo.

1. (Facoltativo) Utilizza le opzioni nella barra degli strumenti Testo formattato per formattare il testo, aggiungere emoticon o collegamenti all’aggiornamento per migliorare il contenuto.

   >[!TIP]
   >
   >Non è possibile aggiungere immagini a un commento di record.


1. Continuare ad aggiungere commenti al record.

   Per ulteriori informazioni sull&#39;aggiornamento degli oggetti, inclusi i record di Workfront Planning, vedere [Aggiorna lavoro](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Facoltativo) Fai clic sull&#39;icona **Altro** ![Altro menu](assets/more-menu.png) nell&#39;angolo superiore destro del commento, quindi fai clic su **Elimina** per eliminare il commento.
1. (Facoltativo) Fai clic sull&#39;icona **Nascondi commenti** ![Nascondi commenti](assets/hide-comments-icon.png) per chiudere il pannello di destra.

<!--
      >[!TIP]
      >
      >If another user submits a comment to the same item you are updating, there is a red line with a "New" indicator to inform you of the newer comments. 
      >
      >The indicator displays only after the comment was submitted on the item, and not when the comment is still composed. 
      >
      >![New line indicator in comments](assets/new-line-indicator-comments.png)
1. Click **Submit** to add the update to the record. 
1. (Optional) To edit a comment, click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner of the comment, then click **Edit**.
   >[!IMPORTANT]
   >
   >You can edit your comment only within 15 minutes from submitting it.  
1. Edit the information in the comment, add or remove images or remove any of the tagged users. An "edited" indicator is added to the left of the comment.
      >[!TIP]
      >
      >Comments from the current year do not display the year in the date stamp. Hovering over a timestamp displays the full date, including the year.
1. (Optional and conditional) To search for an existing comment, start typing a keyword in the search box in the upper-right corner of the **Comments** area.     
   ![Search box for comments](assets/search-box-for-comments-area.png)
1. (Optional) Click **Reply** or start typing a comment in the **Add reply ...** area, to reply to an existing comment, then follow steps 4-8 above. (**************accurate??***********)
1. (Conditional and optional) If other users have added comments that display outside of the visible area in the Comments section while you were adding your comments, click **View** inside the **new comments banner** at the bottom of the screen  to display these comments.
   ![New comments banner on record](assets/new-comments-banner-on-record.png)

    Additional comments display at the bottom of the screen.
1. (Optional) Click the **Like** icon to like an update or acknowledge that you read it. The icon updates with the number of likes.
1. (Conditional and optional) If you included additional people in your comment, click the avatars of the users included in the update to display a list of users that the comment is shared with. 
1. (Optional) Click the **More** icon ![More menu](assets/more-menu.png) in the upper-right corner of the comment and click one of the following options, to copy a information from a comment: 
    * **Copy link**: This copies a link to the comment to your clipboard.
    * **Copy body text**: This copies the text of the comment to your clipboard.
    * **Quote reply**: This copies the content of your comment into a new reply. Images are not included in the copied reply. 

    For more information, see [Update work](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md). -->

## Panoramica della sezione Cronologia

È possibile esaminare le modifiche apportate al record nella sezione Cronologia del pannello di destra di un record.

Per ulteriori informazioni, vedere [Panoramica della sezione Cronologia](/help/quicksilver/planning/records/history-section-overview.md).
