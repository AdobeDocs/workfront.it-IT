---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Genera bozze in [!DNL Workfront Proof]
description: Workfront Proof consente di creare bozze da documenti o siti Web e di condividerle con altri utenti.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: de23513976d7bc4fe34cbf7b007a41c3b9797347
workflow-type: tm+mt
source-wordcount: '1889'
ht-degree: 2%

---

# Genera bozze in [!DNL Workfront Proof]

<!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] consente di creare bozze da documenti o siti Web e di condividerle con altri utenti. I passaggi seguenti descrivono le varie opzioni di configurazione disponibili:

## Generare una bozza da un documento

1. Per aprire la pagina **[!UICONTROL Nuova bozza]**, eseguire una delle operazioni seguenti:

   * Fai clic sul pulsante **[!UICONTROL Nuova bozza]** nell&#39;angolo superiore sinistro di qualsiasi pagina.
   * Invia tramite Dropzone (funzione Enterprise).

1. Per eseguire la verifica di uno o più documenti, aggiungi i documenti da sottoporre a verifica in uno dei seguenti modi (ripeti questo processo per aggiungere più documenti):

   * Trascinare un documento dal file system nell&#39;area di trascinamento della selezione nell&#39;area **[!UICONTROL Aggiungi file]**.
   * Nell&#39;area **[!UICONTROL Aggiungi file]**, fare clic sul collegamento **Sfoglia** per trovare e selezionare il documento che si desidera caricare dal file system della workstation.

     ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. Per effettuare la verifica di un sito Web, immetti l&#39;URL del sito Web nell&#39;area **[!UICONTROL Aggiungi file]**, quindi premi **[!UICONTROL Invio]**. Ripeti questo passaggio per aggiungere più siti web alla bozza.

   Per ulteriori dettagli sulla verifica dei siti Web, vedere [Generare una bozza per un URL](#generate-a-proof-for-a-url).

   ![Sito Web bozza](assets/proof-website-350x65.png)

1. (Facoltativo) Modifica i nomi dei file caricati:

   1. Nell&#39;elenco dei documenti, passa il puntatore sul nome del documento che desideri modificare, quindi fai clic sull&#39;icona **[!UICONTROL Modifica]**.

      ![modifica_bozza.png](assets/proof-edit-350x53.png)

   1. Nel campo **[!UICONTROL Nome bozza]**, specifica un nuovo nome, quindi fai clic su **[!UICONTROL Fine]**.

   1. (Facoltativo) Per eliminare i file da caricare, passa il cursore del mouse sul documento da eliminare nell&#39;elenco dei documenti, quindi fai clic sull&#39;icona **[!UICONTROL Elimina]**.

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. (Facoltativo) Abilita l&#39;opzione **[!UICONTROL Combina tutti i file compatibili in un&#39;unica bozza]**.

      **Quando questa opzione è abilitata:** tutti i file statici e i siti Web sono disponibili in un&#39;unica bozza e puoi caricare fino a 50 file alla volta.

      >[!NOTE]
      >
      >I file interattivi, inclusi video e siti web interattivi, non possono essere combinati in un’unica bozza.

      **Se questa opzione è disabilitata:** tutti i documenti e i siti Web vengono generati come bozze singole e puoi caricare fino a 20 file alla volta.

      Per combinare tutti i file e i siti web caricati in un’unica bozza:

      1. Abilita l&#39;opzione **[!UICONTROL Combina tutti i file compatibili in un&#39;unica bozza]**.
      1. Nel campo **[!UICONTROL Nome bozza]** immettere un nuovo nome per la bozza combinata.
      1. Nell&#39;area **[!UICONTROL Aggiungi file]**, riordinare i file inclusi trascinandoli nell&#39;ordine desiderato. L’ordine dei file è l’ordine di pagina della bozza combinata. Per ulteriori informazioni sulla creazione di bozze combinate, vedere [Creare una bozza multipagina](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. (Facoltativo) Se desideri utilizzare un flusso di lavoro automatizzato che include più fasi, seleziona una delle seguenti opzioni nella sezione **[!UICONTROL Flusso di lavoro]**:

   * **Base:** Selezionare questa opzione per indicare gli utenti ai quali si desidera consentire l&#39;accesso alla bozza subito dopo la creazione. Puoi condividere la bozza con più utenti.

     Per ulteriori informazioni sulla condivisione di una bozza, vedere [Condividere una bozza in [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **Automatizzato:** Selezionare questa opzione per gestire la revisione e l&#39;approvazione del contenuto quando si utilizzano processi di revisione complessi o se si inviano regolarmente contenuti per la revisione agli stessi gruppi di persone. Con un flusso di lavoro automatizzato, la bozza si sposta da una fase all’altra fino all’approvazione finale. Gli utenti interessati vengono avvisati ogni volta che sono tenuti a effettuare un’approvazione.

     Per ulteriori informazioni sulla creazione di un flusso di lavoro automatico, vedere [Configurare una bozza con un flusso di lavoro automatico in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. Seleziona se inviare notifiche e-mail e un messaggio personalizzato agli utenti selezionati nel passaggio precedente:

   * **Notifica ai destinatari questa bozza:** Seleziona questa opzione per inviare una notifica e-mail agli utenti. Quando nella sezione **[!UICONTROL Flusso di lavoro]** è selezionata la condivisione di base **, viene inviata una notifica e-mail al momento della creazione della bozza.** Quando **[!UICONTROL Flusso di lavoro automatico]** è selezionato nella sezione **[!UICONTROL Flusso di lavoro]**, una notifica e-mail viene inviata quando la bozza entra nella fase del flusso di lavoro automatico a cui è associato l&#39;utente.

   * **Aggiungi messaggio personalizzato:** Selezionare questa opzione per includere un messaggio personalizzato nella notifica. È possibile specificare un oggetto e il corpo del messaggio. Il corpo del messaggio può includere formattazione RTF, ad esempio grassetto, punti elenco e collegamenti ipertestuali.

1. Seleziona una delle seguenti impostazioni di bozza:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Accesso obbligatorio. Impossibile condividere questa bozza con altri utenti</td> 
      <td> <p>Quando questa opzione è selezionata:</p> 
       <ul> 
        <li>Gli utenti non possono accedere alla bozza per visualizzarla a meno che non siano stati aggiunti a essa.</li> 
        <li>Le sottoscrizioni non possono essere abilitate.</li> 
       </ul> 
       <p>Questa opzione è disabilitata per impostazione predefinita.</p> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Richiedi la firma elettronica per le decisioni</td> 
      <td><p>Quando questa opzione è selezionata, gli utenti devono specificare il nome utente e la password al momento della decisione su una bozza.</p>
      <p>Questa opzione è disabilitata per impostazione predefinita.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Blocca la bozza quando vengono prese tutte le decisioni necessarie</td> 
      <td> <p>Quando questa impostazione è abilitata, lo stato della bozza viene bloccato dopo che tutte le decisioni sono state prese. Lo stato viene automaticamente modificato da sbloccato a bloccato quando l'approvatore finale prende la sua decisione.</p> 
      <p>Questa opzione è disabilitata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti il download del file originale</td> 
      <td> <p><strong></strong> Quando questa opzione è selezionata, i revisori possono scaricare il file originale da cui è stata creata la bozza.</p> <p>Quando questa opzione è deselezionata, l’icona Scarica non è più visibile.</p>
      <p>Questa opzione è attivata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti la condivisione bozza tramite URL pubblico o codice integrato</td> 
      <td><p>Quando questa opzione è selezionata, la bozza può essere condivisa tramite un URL pubblico o un codice di incorporamento.</p>
       <p>Questa opzione è attivata per impostazione predefinita.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consenti l’iscrizione alla bozza tramite un URL pubblico o un codice di incorporamento</td> 
      <td> <p>Quando questa opzione è selezionata, gli utenti che non sono stati aggiunti alla bozza possono effettuare la sottoscrizione alla bozza. Alla persona che si abbona alla bozza vengono assegnati il ruolo e l’e-mail definiti nelle seguenti impostazioni:</p> 
       <ul> 
        <li><strong>Ruolo sottoscrittore</strong>: ruolo bozza predefinito assegnato a tutti i revisori che sottoscrivono la bozza.</li> 
        <li><strong>Impostazioni degli avvisi e-mail per i sottoscrittori</strong>: L'avviso e-mail predefinito assegnato a tutti i revisori che si abbonano alla bozza.</li> 
        <li> <p><strong>Accesso alla bozza tramite collegamento e-mail richiesto per</strong>: configurare se il sottoscrittore riceve un'e-mail con un collegamento alla bozza. È possibile selezionare <strong>Nessuna e-mail</strong> (il collegamento e-mail non è necessario per accedere alla bozza), <strong>Solo e-mail di notifica bozza</strong> (l'abbonato riceve un collegamento alla bozza tramite e-mail senza alcuna verifica) o <strong>E-mail di notifica convalida e bozza</strong> (l'abbonato riceve un collegamento alla bozza tramite e-mail e deve fare clic sul collegamento per accedere a una bozza. Lo scopo di questa opzione è garantire che la persona abbia inserito un indirizzo e-mail corretto a cui ha accesso).</p> <p>Nota: se alle bozze è allegato un flusso di lavoro automatico, tutte le sottoscrizioni genereranno e-mail di conferma al proprietario della bozza in modo che possa decidere a quale fase deve essere aggiunta la persona.</p> </li> 
       </ul> 
        <p>Questa opzione è disabilitata per impostazione predefinita.</p>
       </td> 
     </tr> 
    </tbody> 
   </table>

1. Fare clic su **[!UICONTROL Crea bozza]**. Workfront genera una bozza dei documenti o dei siti Web selezionati.

   Il tempo di ritardo per il caricamento di un documento varia a seconda delle dimensioni e del tipo di file. La generazione di file più grandi richiede più tempo. Puoi spostarti dalla pagina man mano che Workfront continua a generare il file. La dimensione massima per il caricamento dei file è di 4 GB.

## Generare una bozza statica con un URL {#generate-a-proof-for-a-url}

Puoi generare una bozza statica utilizzando un URL del sito web.

>[!NOTE]
>
>È possibile generare una bozza interattiva per un URL solo se l&#39;ambiente [!DNL Workfront] è integrato con un account Premium [!DNL Workfront Proof]. Se non è possibile utilizzare gli strumenti di correzione come descritto in questa sezione, contattare l&#39;amministratore di Workfront.

1. Per aprire la pagina **[!UICONTROL Nuova bozza]**, eseguire una delle operazioni seguenti:

   * Fai clic sul pulsante **[!UICONTROL Nuova bozza]** nell&#39;angolo superiore sinistro di qualsiasi pagina.
   * Invia tramite Dropzone (funzione Enterprise).

1. Nella pagina **Nuova bozza**, immetti l&#39;URL del sito Web dal quale desideri creare una bozza nell&#39;area **[!UICONTROL Aggiungi file]**, quindi premi **[!UICONTROL Invio]** o **[!UICONTROL Ritorno]** sulla tastiera.

1. (Facoltativo) Ripeti questa procedura per aggiungere più siti web alla bozza.

   ![proof_website.png](assets/proof-website-350x65.png)

1. Nell&#39;area **[!UICONTROL Aggiungi file]**, fare clic sull&#39;icona **Modifica** a destra dell&#39;URL per aprire i dettagli della bozza del sito Web.

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. Immetti un **[!UICONTROL nome bozza]**. Per impostazione predefinita, il nome della bozza è lo stesso dell’URL del sito.

1. Selezionare una delle seguenti **[!UICONTROL opzioni per la gestione del contenuto del sito]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Acquisisci schermata</td> 
      <td>Crea la bozza di un’immagine statica della pagina principale dell’URL.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Interattiva</td> 
      <td> <p>Crea una bozza che consente ai revisori di navigare nel sito, visualizzare immagini HTML5, elementi Flash e così via.</p> <p>Per creare una bozza interattiva, il sito web deve essere ospitato con un protocollo sicuro (https). Inoltre, i siti web che non possono essere incorporati in un iframe non possono essere generati come bozza interattiva (le restrizioni di incorporamento iframe sono controllate dal sito web che si sta tentando di incorporare).</p> <p>Dopo la creazione della bozza iniziale, questa impostazione non può essere modificata durante la creazione di versioni successive.</p> <p>Per ulteriori informazioni sulla verifica interattiva, vedere <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">Generare una bozza per il contenuto interattivo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Risoluzione schermata</td> 
      <td> <p>Questa opzione non è disponibile per le bozze interattive. Puoi regolare la risoluzione di visualizzazione del contenuto oppure selezionare più risoluzioni.</p> <p>Questo consente agli utenti che revisionano la bozza di visualizzare come apparirà il contenuto su dispositivi diversi, come telefoni, tablet e monitor di varie dimensioni.</p> <p>Se selezioni più risoluzioni, viene creata una bozza separata per ogni risoluzione selezionata.</p> <p>Quando gli utenti commentano la bozza, la risoluzione dello schermo corrente viene visualizzata automaticamente nel commento per assicurarsi che gli altri utenti sappiano a quale risoluzione è associato il commento.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cerca pagine secondarie</td> 
      <td>Questa opzione non è disponibile per le bozze interattive. Seleziona questa opzione per navigare tra le pagine del sito web. Puoi espandere il sito web fino a 2 livelli di profondità dalla pagina principale. Passa il puntatore del mouse su una pagina per visualizzare l’URL della pagina e seleziona solo le pagine che desideri verificare. Per impostazione predefinita, ogni pagina selezionata viene creata come una singola bozza. In alternativa, è possibile abilitare l'opzione <strong>Combina tutti i file compatibili in un'unica bozza</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Configura le opzioni di verifica avanzate, ad esempio la condivisione della bozza, l’aggiunta di un flusso di lavoro automatico o la configurazione delle impostazioni di accesso e abbonamento. Per ulteriori dettagli su queste opzioni, vedi i seguenti articoli:

   * [Condividi bozza in [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Configura una bozza con un flusso di lavoro automatico in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Configurare le impostazioni di accesso e abbonamento per una bozza](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Fai clic su **[!UICONTROL Fine]**.

1. Fare clic su **[!UICONTROL Crea bozza]**.

## Generare una bozza per il contenuto interattivo {#generate-a-proof-for-interactive-content}

<!--A Pro Workfront Plan or higher is required to use this feature. For more information about the various plans available, see [Workfront Plans](https://www.workfront.com/plans).-->

Per ulteriori informazioni sul contenuto interattivo, vedere [Panoramica delle bozze del contenuto interattivo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Aggiungere contenuto interattivo come URL](#add-interactive-content-as-a-url)
* [Aggiungere contenuto interattivo come file ZIP](#add-interactive-content-as-a-zip-file)

### Aggiungere contenuto interattivo come URL {#add-interactive-content-as-a-url}

Per informazioni su come aggiungere una bozza URL interattiva, vedere [Generare una bozza per un URL](#generate-a-proof-for-a-url).

### Aggiungere contenuto interattivo come file ZIP {#add-interactive-content-as-a-zip-file}

1. Prepara il contenuto creando un file .zip.

   Per informazioni sulle specifiche dei file con bundle .zip, consulta [Panoramica delle bozze interattive dei contenuti](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Per aprire la pagina **[!UICONTROL Nuova bozza]**, eseguire una delle operazioni seguenti:

   * Fai clic sul pulsante **[!UICONTROL Nuova bozza]** nell&#39;angolo superiore sinistro di qualsiasi pagina.
   * Invia tramite Dropzone (funzione Enterprise).

1. Nella pagina **[!UICONTROL Nuova bozza]**, trascina e rilascia il bundle .zip interattivo nell&#39;area **[!UICONTROL Aggiungi file]**.

1. (Facoltativo) Configura le opzioni di verifica avanzate, ad esempio la condivisione della bozza, l’aggiunta di un flusso di lavoro automatizzato o la configurazione delle impostazioni di accesso e abbonamento. Per ulteriori dettagli su queste opzioni, vedi i seguenti articoli:

   * [Condividi bozza in [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Configurare le impostazioni di accesso e abbonamento per una bozza](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Fare clic su **[!UICONTROL Crea bozza]**. Workfront genera una bozza del file zip.

   Il tempo di ritardo per il caricamento di un documento varia a seconda delle dimensioni del file zip. Puoi spostarti dalla pagina man mano che Workfront continua a generare il file. La dimensione massima per il caricamento dei file è di 4 GB.
