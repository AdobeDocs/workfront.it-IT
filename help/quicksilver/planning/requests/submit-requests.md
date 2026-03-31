---
title: Inviare richieste di Adobe Workfront Planning
description: Dopo che un utente ha condiviso un collegamento a un modulo di richiesta da una pagina di tipo di record in Adobe Workfront Planning, è possibile aggiungere una richiesta per la creazione di record per il tipo di record associato al modulo di richiesta.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '2026'
ht-degree: 2%

---

# Inviare richieste di Pianificazione di Adobe Workfront per creare record

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Dopo che un responsabile dell&#39;area di lavoro crea un modulo di richiesta per un tipo di record in Adobe Workfront Planning, è possibile utilizzare il modulo per inviare richieste che creeranno record per il tipo di record associato al modulo.

È possibile inviare una richiesta di Workfront Planning dalle aree seguenti:

* Dall’area Richieste di Workfront o dal widget Richieste personali nella Home.
* Da un collegamento diretto al modulo di richiesta condiviso.
* Dalla pagina del tipo di record, quando si aggiunge un nuovo record inviando una richiesta. Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).

Questo articolo descrive come inviare una richiesta per aggiungere nuovi record a un tipo di record dall’area Richieste di Workfront o da un collegamento condiviso.

I responsabili Workspace possono creare moduli di richiesta che è possibile utilizzare come utente o come persona esterna per inviare richieste ai tipi di record di Planning. Le richieste creano record per il tipo di record associato al modulo di richiesta.

Per informazioni su come un manager area di lavoro può creare un modulo di richiesta e associarlo a un tipo di record, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacchetti Adobe Workfront</p></td> 
   <td> 
<p>Qualsiasi pacchetto Workfront e qualsiasi pacchetto Planning</p>
Oppure
<p>Qualsiasi pacchetto del flusso di lavoro e qualsiasi pacchetto Planning</p>
<p>Per ulteriori informazioni su ciò che è incluso in ogni pacchetto Workfront Planning, contattare il rappresentante del proprio account Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licenza di Adobe Workfront</p></td> 
   <td><p>Qualsiasi</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorizzazioni sugli oggetti</p></td> 
   <td>   <p>Visualizza o autorizzazioni superiori per un’area di lavoro e un tipo di record, se sei un utente di Workfront</p>  </td> 
  </tr>  
</tbody> 
</table>

Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di inviare una richiesta a un modulo di richiesta Workfront Planning, è necessario disporre dei seguenti elementi:

* In Workfront Planning devono esistere gli elementi seguenti:

   * Un’area di lavoro
   * Un tipo di record
   * Modulo di richiesta associato a un tipo di record.

     Per informazioni, vedere [Creare un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* Il modulo di richiesta deve essere condiviso in modo da potervi accedere. Esistono i seguenti scenari:

   * Internamente, il modulo deve essere condiviso con utenti che dispongono di autorizzazioni di visualizzazione o di livello superiore per l&#39;area di lavoro.

     Gli utenti di Workfront possono accedere al modulo da un collegamento o trovare il modulo di richiesta nell’area Richieste di Workfront.

   * Esternamente, condividendo un collegamento al modulo record con utenti esterni che non dispongono di un account Workfront.

     Gli utenti di Workfront possono anche accedere al collegamento condiviso con persone esterne.

* Se condiviso con un collegamento, il collegamento al modulo non deve essere scaduto.

## Considerazioni sull&#39;invio di richieste a Workfront Planning

* Non è possibile modificare una richiesta in Workfront dopo averla inviata.
* Ogni richiesta sottomessa crea un record per il tipo di record associato al modulo utilizzato, se il modulo non è associato a un&#39;approvazione o se l&#39;approvazione è stata concessa da tutti gli approvatori.
* I record creati mediante l&#39;invio di moduli di richiesta sono identici ai record aggiunti tramite qualsiasi altro metodo in Workfront Planning.

  Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).
* I record creati mediante l’invio di moduli di richiesta sono collegati alla richiesta originale. Impossibile rimuovere la connessione.
* Puoi visualizzare sia i record creati che le richieste utilizzate per crearli nelle seguenti aree:
   * Area Richieste in Workfront.

  <div class="preview">

   * In un campo connesso di una pagina del tipo di record in Workfront Planning quando si aggiunge la richiesta come record connesso.
   * In un campo connesso dell&#39;area Dettagli di un record in Workfront Planning quando si aggiunge la richiesta come record connesso.

  </div>

  >[!TIP]
  >
  ><span class="preview">È possibile visualizzare il nome della richiesta nel campo Oggetto nell&#39;area Richieste di Workfront o nel campo Richiesta originale di connessione in Workfront Planning. </span>

* Le richieste Planning inviate sono visibili solo nella nuova esperienza di richiesta. Non è possibile visualizzare le richieste Planning nell’esperienza di richiesta legacy.

  Per informazioni, vedere [Creare e inviare richieste](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).
* Esistono limitazioni nella visualizzazione di determinati tipi di campo in un modulo di richiesta o nella pagina dei dettagli della richiesta dopo l’invio di un modulo.

  Per informazioni, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Inviare una richiesta a Workfront Planning nell&#39;area Richieste di Workfront

{{step1-to-requests}}

1. Attiva l&#39;impostazione **Usa nuova esperienza** nell&#39;angolo superiore destro dello schermo.
L&#39;attivazione di questa impostazione rende disponibili i moduli di richiesta di Workfront Planning nell&#39;area **Richieste** di Workfront.

   >[!TIP]
   >
   >Questa impostazione è disponibile solo quando l’istanza di Workfront è integrata in Adobe Unified Experience.
   >
   >Per poter inviare richieste di Workfront Planning in quest&#39;area, è necessario soddisfare le seguenti condizioni:
   >
   >* La società ha acquistato una licenza Workfront Planning.
   >
   >* Puoi accedere alla visualizzazione di almeno un’area di lavoro.

1. Fare clic su **Quale richiesta si desidera inviare?** barra per aprire un elenco di moduli di richiesta.
1. Selezionare un modulo di richiesta dall&#39;elenco o iniziare a digitare il nome del modulo di richiesta, quindi selezionarlo quando viene visualizzato nell&#39;elenco.

   Viene visualizzata una finestra con il nome del modulo di richiesta nella parte superiore.

   >[!TIP]
   >
   >Le code di richieste di Workfront contengono il nome della coda e il nome del modulo nell’elenco delle richieste. I moduli delle richieste di Planning visualizzano solo il nome del modulo nell&#39;elenco delle richieste.

1. Aggiorna il campo **Oggetto**. Questo è il nome della richiesta. Questo è un campo obbligatorio.
1. Aggiorna il campo **Name**. Questo è il nome del record futuro.

   >[!TIP]
   >
   >Il campo **Name** è univoco per la tua organizzazione e potrebbe contenere un&#39;etichetta diversa nella tua istanza di Workfront. Il campo è il campo principale del record.

1. Aggiorna i campi rimanenti nel modulo di richiesta. I campi con un asterisco rosso sono obbligatori.
1. (Condizionale) Se la tua organizzazione consente il **riempimento modulo** basato su AI, puoi caricare i documenti come prompt. IA utilizza questi documenti per compilare il modulo e puoi accettare o rifiutare i suggerimenti di IA prima di inviare la richiesta.


   Per istruzioni, consulta [Utilizzare il riempimento del modulo basato su IA per compilare una richiesta utilizzando prompt o documenti](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).
1. Fai clic su **Invia**.

   Il modulo di richiesta si chiude e si torna all&#39;area **Richieste**.

   Il modulo viene inviato e si verificano gli eventi seguenti:

   * Se il modulo di richiesta non è stato associato a un’approvazione, la richiesta viene aggiunta all’elenco Richieste nell’area Richieste Workfront e al widget Richieste personali nella Home e viene aggiunto un nuovo record al tipo di record associato al modulo.

     I campi seguenti visualizzano le informazioni sulle richieste e sui record nell&#39;area Richieste e nel widget Richieste personali nella Home:

      * **Oggetto**: nome della richiesta originale aggiunto nell&#39;area Richieste. Impossibile nascondere o rimuovere il campo **Oggetto** dall&#39;elenco delle richieste.
      * **Oggetto creato**: nome del record creato dalla richiesta visualizzato in Planning.
      * **Tipo di oggetto**: nome dell&#39;area di lavoro e del tipo di record in cui sono stati creati i record dalla richiesta in Planning.
      * **Stato**: lo stato dell&#39;oggetto della richiesta.
      * **Modulo di richiesta**: nome del modulo di richiesta associato al tipo di record in Planning.
     <!--* <span class="preview"**Created object status**: The status of the created record.</span> -->

   * Se il modulo di richiesta è stato associato a un&#39;approvazione, la richiesta viene aggiunta all&#39;elenco Richieste nell&#39;area Richieste Workfront e al widget Richieste personali con stato **Revisione in sospeso**. Un nuovo record viene aggiunto alla pagina del tipo di record solo dopo che è stato approvato dagli approvatori.

     Per informazioni, vedere [Aggiungere un&#39;approvazione a un modulo di richiesta](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

   * <span class="preview">È possibile aggiungere il campo di connessione **Richiesta originale** a un tipo di record in Planning per visualizzare il nome della richiesta originale che ha creato un record. Per informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md). </span>
   * La richiesta è visibile solo al proprietario, all&#39;approvatore e agli utenti che dispongono almeno delle autorizzazioni di visualizzazione per l&#39;area di lavoro. Gli amministratori di Workfront possono visualizzare tutte le richieste inviate a qualsiasi area di lavoro del sistema.
   * Ricevi una notifica in-app e un messaggio e-mail che informa che la richiesta è stata inviata correttamente o è stata inviata per la revisione.
   * Se il modulo di richiesta era associato a un’approvazione, gli approvatori ricevono una notifica in-app e un messaggio e-mail per rivedere e approvare la richiesta.

     >[!NOTE]
     >
     >L’e-mail e la notifica in-app sono visibili solo quando l’istanza di Workfront della tua organizzazione viene integrata in Adobe Unified Experience.
     >
     >L’e-mail di conferma o di notifica dell’approvazione contiene un collegamento alla richiesta.

1. (Facoltativo) Fai clic su **Visualizza la richiesta** nel messaggio di conferma, per aprire la richiesta, oppure fai clic sull&#39;icona **X** per chiudere la conferma.
1. (Facoltativo) Per gestire la modalità di visualizzazione delle informazioni nell’elenco delle richieste, aggiorna i seguenti elementi di visualizzazione per l’elenco:

   * Visualizzazione
   * Filtro
   * Colonne

   <!--
   <div class="preview">
      * Group
   * Format cells
   * Row height
      </div>
   -->

   Per informazioni, vedere [Creare e gestire le visualizzazioni nell&#39;area Richieste](/help/quicksilver/manage-work/requests/create-requests/create-views-for-requests-list.md).

   <!--   
   1. (Optional) From the requests list, do any of the following:
      * Click **Filters** and start adding conditions for what requests you want to view in the Requests list. 
         ![Editing filters in the Requests area](assets/filters-editing-box-in-requests-planning-tab.png)
         You can filter by the following fields:  
         * **Workspace**: The workspace the request form is associated with.
         * **Object type**: The record type the request form is associated with.
         * **Entry date**: The date when the request was submitted.
         * **Request form**: The name of the request form used to submit the request.
         * **Status**: The status of the request.
         * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.
        You can have multiple filters joined by either **And** or **Or**.
         The request list is filtered automatically, as you add the filter conditions. 
      * Click **Columns** to open the **Fields visibility and order** box, then hide, show, or rearrange the columns in the request list. 
         >[!TIP]
         >
         >You cannot add any more columns. 
         ![Columns editing box in Requests area](assets/columns-editing-box-in-requests-planning-tab.png)
      * Click the **+** icon in the upper-right corner of the request list to open the **Column manager** and add or remove columns in the requests list. 
   -->

1. Fai clic sul nome di una richiesta nell’elenco.

   Viene visualizzata la pagina dei dettagli della richiesta.

   ![Pagina di richiesta con commento](assets/new-request-page-with-comment.png)

1. (Facoltativo) Immetti un commento nell&#39;area **Commenti**.
1. (Condizionale) Se il modulo di richiesta non è associato a un&#39;approvazione o se la richiesta è stata approvata, fare clic sul nome della richiesta, quindi sul nome del record nel campo **Oggetto creato**.

   La pagina del record viene visualizzata in Workfront Planning.

   >[!TIP]
   >
   >* Se il campo principale del record non è stato aggiornato nel modulo di richiesta, il nome del record nel campo Record della richiesta viene visualizzato come **Senza titolo**.
   >
   >* Se il modulo di richiesta è associato a un’approvazione, questa deve essere concessa prima di poter accedere al record dalla pagina della richiesta. Il record viene creato solo dopo la concessione dell’approvazione.

1. (Facoltativo) Fare clic sul nome del tipo di record **&#x200B;**.

   La pagina del tipo di record viene visualizzata in Workfront Planning.

## Inviare una richiesta a Workfront Planning da un collegamento condiviso a un modulo di richiesta

Le informazioni in questa sezione sono valide solo per gli utenti che inviano una richiesta da un collegamento condiviso e che potrebbero non disporre di un account Workfront.

Gli utenti esterni non possono accedere alle aree interne di Workfront, ad esempio **Richieste** o **Home**.

1. Passare al collegamento condiviso con l&#39;utente da un tipo di record di Workfront Planning.

1. Aggiorna i campi disponibili nel modulo. I campi con un asterisco sono obbligatori.

   >[!TIP]
   >
   >   Se il campo **Oggetto** è disponibile, non sarà visibile in Workfront Planning dopo l&#39;invio della richiesta.
   >
   >È consigliabile aggiornare il maggior numero possibile di campi nella richiesta per rendere il nuovo record identificabile quando viene aggiunto al tipo di record in Workfront Planning.

1. Fai clic su **Invia**.

   Il modulo viene inviato e si ottiene una conferma.

   Se il modulo è associato a un&#39;approvazione, è necessario approvarlo prima di creare un record.

1. (Facoltativo) Fai clic su **Invia un&#39;altra richiesta** per aggiungere un&#39;altra richiesta allo stesso collegamento condiviso.

<!--
   * If the request form was not associated with an approval, the request is added to the Requests list in the Workfront Requests area and My Requests widget in Home, and a new record is added to the record type associated with the form. This is available only when you log in to Workfront.
   
   * If the request form was associated with an approval, the request is added to the Requests list in the Workfront Requests area and My Requests widget. A new record is added to the record type page only after all the approvers have approved it. This is available only when you log in to Workfront.
   
      For information, see [Add an approval to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

      >[!IMPORTANT]
      >
      >You can view only the requests submitted by you or anyone else to the workspaces that you have at least permissions to View. Workfront administrators can view all requests submitted to any workspace in the system. <!--ensure this is correct; asking team in slack
   
   
   * You receive an in-app and an email notification that the request has either been submitted successfully or has been sent for review.
   * If the request form was associated with an approval, the approvers receive an in-app and an email notification to review and approve the request.
      >[!NOTE]
      >
      >The email and in-app notification are visible only when your organization's instance of Workfront is onboarded to the Adobe Unified Experience.
   
   <span class="preview"> After the request was approved and the record was created, the Approved by and Approved date fields display information about the approval on the record.</span>


1. (Optional) Click **View your request** to open the request in Workfront.


Or

Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.

   The request details page opens. 

   ![Request page with comment](assets/new-request-page-with-comment.png)

1. (Optional) Enter a comment in the **Comments** area.
1. (Conditional) If the request form is not associated with an approval, or if the request has been approved, click the name of the request, then click the name of the record in the **Created object** field. 

   The record's page opens in Workfront Planning. 

   >[!TIP]
   >
   >* If the record name was not added to the request form, the name of the record in the Record field of the request displays as **Untitled**. 
   >
   >* If the request form is associated with an approval, the approval must be granted before you can access the record from the request page. 

1. (Optional) Click the name of the **Object type**. 

   The record type page opens in Workfront Planning. 

-->

## Creare una richiesta copiando una richiesta esistente

È possibile copiare una richiesta nell’elenco delle richieste in Workfront, quindi modificarne i dettagli e inviarla come nuova richiesta.

Questa funzione è disponibile solo nella nuova esperienza di richiesta.

Copiare una richiesta Planning esistente e inviarla come nuova è simile a copiare una richiesta Workfront esistente.

Per ulteriori informazioni, vedere [Copiare e inviare richieste](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Creare bozze e richieste da bozze esistenti

Puoi creare una bozza di una richiesta, quindi tornare alla bozza e inviarla come richiesta in un secondo momento.

Questa funzione è disponibile solo nella nuova esperienza di richiesta. La creazione di bozze e richieste da bozze esistenti in Workfront Planning è identica alla creazione di bozze da Adobe Workfront.

Per ulteriori informazioni, vedere [Creare richieste dalle bozze](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md).

## Eliminare bozze o richieste inviate

È possibile eliminare le richieste inviate o le relative bozze quando si utilizza la nuova esperienza di richiesta.

Quando si elimina una richiesta di Planning, si verificano gli eventi seguenti:

* Impossibile recuperare la richiesta.
* Il record creato dalla richiesta non viene eliminato.
* Non è possibile recuperare le bozze eliminate. Nessun record associato alle bozze.

L&#39;eliminazione delle richieste Planning è simile all&#39;eliminazione delle richieste Workfront.

Per informazioni, vedere [Eliminare una richiesta inviata o una bozza di richiesta](/help/quicksilver/manage-work/requests/create-requests/delete-request-draft.md).







