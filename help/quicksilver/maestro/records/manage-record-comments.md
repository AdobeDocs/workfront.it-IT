---
title: Gestisci commenti record
description: Puoi collaborare ai record Adobe Maestro aggiungendo aggiornamenti e facendo domande o risposte nell’area Commenti di un record.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 3ffb6fdebb54682abc737e55186850458a133f7c
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Gestisci commenti record

Puoi collaborare ai record Adobe Maestro aggiungendo aggiornamenti e facendo domande o risposte nell’area Commenti di un record.

## Considerazioni sul commento a un record

* È possibile aggiungere commenti e risposte ai record operativi e alle tassonomie in Maestro, nella sezione Commenti di un record.

* I commenti aggiunti ai record collegati non vengono visualizzati nei record da cui si sta eseguendo il collegamento. Ad esempio, se commenti un progetto collegato a un record Campagna, il commento viene visualizzato solo sul record del progetto in Maestro e non sul record della campagna da cui stai effettuando il collegamento.

* I commenti aggiunti agli oggetti collegati in altre applicazioni non vengono visualizzati in Maestro.
I commenti aggiunti agli oggetti collegati in Maestro non vengono visualizzati in altre applicazioni.\
  Ad esempio, i commenti aggiunti ai progetti in Workfront non vengono visualizzati sullo stesso progetto collegato a una campagna in Maestro.

* Puoi assegnare tag agli utenti per attirare la loro attenzione su un aggiornamento. Gli utenti taggati non ricevono una notifica in-app o un’e-mail relativa all’aggiornamento. Non è possibile assegnare tag ai team in un commento Maestro.

  >[!TIP]
  >
  >* I proprietari dei commenti non vengono automaticamente taggati in un aggiornamento.
  >
  >* Non è possibile rimuovere utenti con tag da un aggiornamento quando si risponde.

* Puoi aggiungere un aggiornamento ai record dalle seguenti aree di Maestro:

   * Dalla pagina Dettagli.

  <!--* From the table view.-->

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> prodotto Adobe</p> </td>
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
   <td role="rowheader">Livello di accesso</td>
   <td> <p>Qualsiasi</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modello di layout</td>
   <td> <p>L’amministratore di sistema deve aggiungere l’area Maestro nel modello di layout. Per informazioni, consulta <a href="../access/grant-access.md">Concedere l’accesso a Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permissions - replace the table with: **************CHECK ON THE VIEW PERMISSIONS TO THE WORKSPACE; RIGHT NOW, WE SAY THAT VIEW USERS CAN COMMENT BUT THE PAGE BLOWS OUT WHEN I TRY - ASKED PM TO CONFIRM*****************

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

### Gestire i commenti sui record

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](assets/dots-main-menu.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](assets/lines-main-menu.png) nell’angolo superiore sinistro, quindi fai clic su **[!UICONTROL Maestro]**.

   Per impostazione predefinita, viene aperta l’ultima area di lavoro a cui si è effettuato l’accesso.
1. Scegliere una vista tabella dal menu **Visualizza** menu a discesa.
1. Fare clic sul nome di un record nella vista tabella.

   Il record **Dettagli** viene visualizzata la pagina.

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
   * **Copia testo corpo** t: copia il testo del commento negli Appunti.
   * **Risposta preventivo**: copia il contenuto del commento in una nuova risposta. Le immagini non sono incluse nella risposta copiata.

   Per ulteriori informazioni, consulta [Aggiorna lavoro](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Facoltativo) Fai clic su **Altro** icona ![](assets/more-menu.png) nell’angolo superiore destro del commento, quindi fai clic su **Elimina** per eliminare il commento.

