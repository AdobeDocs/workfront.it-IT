---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Generare bozze in [!DNL Workfront Proof]
description: Workfront Proof consente di creare bozze da documenti o siti Web e di condividerle con altri utenti.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '2254'
ht-degree: 0%

---

# Generare bozze in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità del prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Bozza](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] consente di creare bozze da documenti o siti web e di condividerle con altri utenti. I passaggi seguenti descrivono le varie opzioni di configurazione disponibili:

## Generare una bozza per un documento

1. Per iniziare a creare una nuova bozza e visualizzare la [!UICONTROL Nuova bozza] pagina:

   * Fai clic sul pulsante verde **[!UICONTROL Nuova bozza]** nell&#39;angolo superiore sinistro di qualsiasi pagina.
   * In **[!UICONTROL Dashboard]** area, nel **[!UICONTROL Panoramica]** , fare clic sulla scheda **[!UICONTROL Nuova bozza]** collegamento.

   * Invia tramite Dropzone (funzione Enterprise).
   * Il **[!UICONTROL Nuova bozza]** viene visualizzata la pagina.

1. Per eseguire la bozza di uno o più documenti, aggiungete i documenti da sottoporre a bozza in uno dei seguenti modi (ripetete questo processo per aggiungere più documenti da sottoporre a bozza):

   * Trascinare un documento dal file system nell&#39;area di trascinamento della selezione in **[!UICONTROL Aggiungi file]** area.
   * Fai clic sull’area di trascinamento della selezione nella **[!UICONTROL Aggiungi file]** , quindi individuare e selezionare il documento che si desidera caricare dal file system della workstation.

     ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. Per eseguire la verifica di uno o più siti Web, specifica l’URL del sito Web da verificare in **[!UICONTROL Aggiungi file]** area, quindi premere **[!UICONTROL Invio]**.

1. (Facoltativo) Ripeti questa procedura per aggiungere più siti web alla bozza.

   Per ulteriori dettagli sulla verifica dei siti Web, vedere [Generare una bozza per un URL](#generate-a-proof-for-a-url).

   ![](assets/proof-website-350x65.png)

1. (Facoltativo) Modifica i nomi dei file caricati:

   1. Passare il puntatore del mouse sul nome del documento che si desidera modificare nell&#39;elenco dei documenti in **[!UICONTROL Aggiungi file]** , quindi fare clic sul pulsante **[!UICONTROL Modifica]** icona.

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. In **[!UICONTROL Nome bozza]** , specifica un nuovo nome e fai clic su **[!UICONTROL Fine]**.

   1. (Facoltativo) Per eliminare i file caricati, posiziona il cursore del mouse sul documento da eliminare nell’elenco dei documenti in **[!UICONTROL Aggiungi file]** , quindi fare clic sul pulsante **[!UICONTROL Elimina]** icona.

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. (Facoltativo) Abilita l’opzione, **[!UICONTROL Combina tutti i file compatibili in un’unica bozza]**.

      **Quando questa opzione è abilitata:** Tutti i file statici e i siti web sono disponibili in un’unica bozza e puoi caricare fino a 50 file alla volta.

      >[!NOTE]
      >
      >I file interattivi, inclusi video e siti web interattivi, non possono essere combinati in un’unica bozza.

      **Quando questa opzione è disabilitata:** Tutti i documenti e i siti web vengono generati come bozze individuali e puoi caricare fino a 20 file alla volta.

      Per combinare tutti i file e i siti web caricati in un’unica bozza:

      1. Abilita l’opzione, **[!UICONTROL Combina tutti i file compatibili in un’unica bozza]**.
      1. In **[!UICONTROL Nome bozza]** , specifica un nuovo nome per la bozza combinata.
      1. In **[!UICONTROL Aggiungi file]** riordinare i file inclusi trascinandoli nell&#39;ordine desiderato. L’ordine dei file è l’ordine di pagina della bozza combinata. Per ulteriori informazioni sulla creazione di bozze combinate, consulta [Creare una bozza con più pagine](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. (Facoltativo) Se desideri utilizzare un flusso di lavoro automatizzato che includa più fasi, nel **[!UICONTROL Flusso di lavoro]** , seleziona una delle seguenti opzioni:

   * **Di base:** Seleziona questa opzione per designare gli utenti a cui desideri accedere subito dopo la creazione della bozza. Puoi condividere la bozza con più utenti.

     Per ulteriori informazioni sulla condivisione di una bozza, consulta &quot;Aggiunta di utenti a una bozza&quot; in [Condividere una bozza in [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **Automatizzato:** Selezionare questa opzione per gestire la revisione e l&#39;approvazione del contenuto quando si utilizzano processi di revisione complessi o se si inviano regolarmente contenuti per la revisione agli stessi gruppi di persone. Con il flusso di lavoro automatizzato, la bozza si sposta da un’area all’altra fino all’approvazione finale. Gli utenti interessati ricevono una notifica ogni volta che sono tenuti a effettuare un’approvazione.

     Per ulteriori informazioni sulla creazione di un flusso di lavoro automatizzato, consulta [Configurare una bozza con un flusso di lavoro automatico in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. Seleziona se inviare notifiche e-mail e un messaggio personalizzato agli utenti selezionati nel passaggio precedente:

   * **Notifica i destinatari relativamente a questa bozza:** Seleziona questa opzione per inviare una notifica e-mail agli utenti. Quando **[!UICONTROL Condivisione di base]** è selezionato in **[!UICONTROL Flusso di lavoro]** sezione, una notifica e-mail viene inviata al momento della creazione della bozza. Quando **[!UICONTROL Flusso di lavoro automatico]** è selezionato in **[!UICONTROL Flusso di lavoro]** , una notifica e-mail viene inviata quando la bozza entra nella fase del flusso di lavoro automatico a cui è associato l’utente.

   * **Aggiungi messaggio personalizzato:** Seleziona questa opzione per includere un messaggio personalizzato nella notifica. È possibile specificare un oggetto e il corpo del messaggio. Il corpo del messaggio può includere formattazione RTF, ad esempio grassetto, punti elenco e collegamenti ipertestuali.

1. Seleziona una delle seguenti impostazioni di bozza:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Accesso necessario: la bozza può essere condivisa solo con altri utenti</td> 
      <td> <p><strong>Accesso obbligatorio - la bozza può essere condivisa solo con altri utenti:</strong> Quando questa opzione è selezionata, solo [!DNL Workfront Proof] Gli utenti possono visualizzare la bozza.</p> <p>Questa opzione è disabilitata per impostazione predefinita; qualsiasi persona con l’URL può visualizzare la bozza.</p> <p>Quando questa opzione è selezionata:</p> 
       <ul> 
        <li>Gli utenti non possono accedere alla bozza a meno che non siano stati aggiunti alla bozza.</li> 
        <li>Le sottoscrizioni non possono essere abilitate.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Per questa bozza è necessaria una sola decisione</td> 
      <td> <p>Quando questa opzione è selezionata, la revisione viene completata dopo che un decisore prende la sua decisione.</p> <p>Questa opzione è disabilitata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Richiedi la firma elettronica per le decisioni</td> 
      <td>Gli utenti devono specificare il nome utente e la password nel momento in cui prendono una decisione sulla bozza.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Blocca la bozza quando vengono prese tutte le decisioni necessarie</td> 
      <td> <p><strong></strong> Quando questa impostazione è abilitata, lo stato della bozza viene bloccato dopo che tutte le decisioni sono state prese. Lo stato viene automaticamente modificato da sbloccato a bloccato quando l'approvatore finale prende la sua decisione.</p> <p>Questa opzione è disabilitata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Scarica il file originale</td> 
      <td> <p><strong></strong> Quando questa opzione è selezionata, i revisori possono scaricare il file originale da cui è stata creata la bozza.</p> <p>Quando questa opzione è deselezionata, l’icona Scarica non è più visibile.<br>Questa opzione è attivata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Condividi bozza tramite URL pubblico o codice incorporato</td> 
      <td>Quando questa opzione è selezionata, la bozza può essere condivisa tramite un URL pubblico o un codice di incorporamento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Iscriviti alla bozza tramite URL pubblico o codice di incorporamento</td> 
      <td> <p>Quando questa opzione è selezionata, le persone che non sono state aggiunte esplicitamente alla bozza possono abbonarsi alla bozza. Alla persona che si abbona alla bozza vengono assegnati il ruolo e l’e-mail definiti nelle seguenti impostazioni:</p> 
       <ul> 
        <li><strong>Ruolo del sottoscrittore</strong>: ruolo di bozza predefinito assegnato a tutti i revisori che si abbonano alla bozza.</li> 
        <li><strong>Impostazioni degli avvisi e-mail per gli abbonati</strong>: avviso e-mail predefinito assegnato a tutti i revisori abbonati alla bozza.</li> 
        <li> <p><strong>Accesso alla bozza tramite collegamento e-mail richiesto per</strong>: configura se il sottoscrittore riceve un’e-mail con un collegamento alla bozza. Puoi selezionare <strong>Nessuna e-mail</strong> (non è necessario un collegamento e-mail per accedere alla bozza), <strong>Solo e-mail di notifica bozza</strong> (l’abbonato riceve un collegamento alla bozza via e-mail senza alcuna verifica), oppure <strong>E-mail di notifica per convalida e bozza</strong> (L’abbonato riceve un collegamento alla bozza tramite e-mail e deve fare clic sul collegamento per accedere a una bozza; lo scopo di questa opzione è garantire che l’utente abbia inserito un indirizzo e-mail corretto al quale ha accesso).</p> <p>Nota: se alle bozze è allegato un flusso di lavoro automatico, tutti gli abbonamenti genereranno e-mail di conferma al proprietario della bozza, in modo che possa decidere a quale fase aggiungere la persona.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Crea bozza]**.

   Workfront inizia a generare una bozza dei documenti o dei siti web selezionati. A seconda delle dimensioni e del tipo di file, il tempo di ritardo per il caricamento di un documento varia. Attendi, poiché la generazione di file più grandi richiede più tempo. Puoi spostarti dalla pagina e Workfront continua a generare il file. La dimensione massima per il caricamento dei file è di 4 GB.

   Una volta generata la bozza, fai clic su **[!UICONTROL Vai alla bozza]** per avviare lo strumento di correzione.

   ![Screenshot_2018-05-16_08-59-34.png](assets/screenshot-2018-05-16-08-59-34-350x134.png)

   Il documento viene visualizzato nello strumento di correzione.

   Gli utenti che non dispongono di un account di verifica abilitato possono comunque visualizzare il documento e aggiungere commenti alla bozza.

## Generare una bozza per un URL {#generate-a-proof-for-a-url}

Puoi generare una bozza per un URL per la prima volta. In alternativa, puoi generare una nuova versione di una bozza URL in cui è stata precedentemente generata una bozza.

>[!NOTE]
>
>Puoi generare una bozza interattiva per un URL solo se [!DNL Workfront] l&#39;ambiente è integrato con [!DNL Workfront Proof] Account Premium. Se non è possibile utilizzare la verifica come descritto in questa sezione, contattare l&#39;amministratore di sistema.

Per generare una bozza per un URL:

1. Per iniziare a creare una nuova bozza e visualizzare la [!UICONTROL Nuova bozza] pagina:

   * Fai clic sul pulsante verde **[!UICONTROL Nuova bozza]** nell&#39;angolo superiore sinistro di qualsiasi pagina.
   * In **[!UICONTROL Dashboard]** area, nel **[!UICONTROL Panoramica]** , fare clic sulla scheda **[!UICONTROL Nuova bozza]** collegamento.

   * Invia tramite Dropzone (funzione Enterprise).

1. (Condizionale) In **[!UICONTROL Nuova bozza]** per creare una nuova versione di una bozza esistente:

   1. Seleziona la bozza URL in cui desideri aggiungere una nuova versione.
   1. Fai clic su **[!UICONTROL Nuova versione]** nella parte superiore della pagina.

      ![Screenshot_2018-05-15_10-59-56.png](assets/screenshot-2018-05-15-10-59-56-350x80.png)

1. Nella pagina Nuova versione bozza visualizzata, specifica l’URL del sito web da sottoporre a bozza in **[!UICONTROL Aggiungi file]** area, quindi premere **[!UICONTROL Invio]**.

1. (Facoltativo) Ripeti questa procedura per aggiungere più siti web alla bozza.

   ![proof_website.png](assets/proof-website-350x65.png)

1. Fare clic sul sito Web nell&#39;elenco dei documenti nel **[!UICONTROL Aggiungi file]** area.

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. Specifica un **[!UICONTROL Nome bozza]** per la bozza.

   Per impostazione predefinita, il nome della bozza è lo stesso dell’URL del sito.

1. Seleziona **[!UICONTROL Gestire i contenuti del sito]** opzioni:

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
      <td> <p>Crea una bozza che consente ai revisori di navigare nel sito, visualizzare immagini HTML5, elementi del Flash e così via.</p> <p>Per creare una bozza interattiva, il sito web deve essere ospitato con un protocollo sicuro (https). Inoltre, i siti web che non possono essere incorporati in un iframe non possono essere generati come bozza interattiva (le restrizioni di incorporamento di iframe sono controllate dal sito web che si sta tentando di incorporare).</p> <p>Dopo la creazione della bozza iniziale, questa impostazione non può essere modificata durante la creazione di versioni successive.</p> <p>Per ulteriori informazioni sulla verifica interattiva, vedere <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">Generare una bozza per il contenuto interattivo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Risoluzione schermata</td> 
      <td> <p>Questa opzione non è disponibile per le bozze interattive. Puoi regolare la risoluzione di visualizzazione del contenuto oppure selezionare più risoluzioni.</p> <p>Questo consente agli utenti che revisionano la bozza di visualizzare come apparirà il contenuto su dispositivi diversi, come telefoni, tablet e monitor di varie dimensioni.</p> <p>Se selezioni più risoluzioni, viene creata una bozza separata per ogni risoluzione selezionata.</p> <p>Quando gli utenti commentano la bozza, la risoluzione dello schermo corrente viene visualizzata automaticamente nel commento per assicurarsi che gli altri utenti sappiano a quale risoluzione è associato il commento.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cerca pagine secondarie</td> 
      <td>Questa opzione non è disponibile per le bozze interattive. Seleziona questa opzione per navigare tra le pagine del sito web. Puoi espandere il sito web fino a 2 livelli di profondità dalla pagina principale. Passa il puntatore del mouse su una pagina per visualizzarne l’URL. Seleziona solo le pagine per le quali desideri eseguire la verifica. Per impostazione predefinita, ogni pagina selezionata viene creata come bozza singola; oppure, abilita <strong>Combina in una singola bozza</strong> per combinare tutte le pagine selezionate in un’unica bozza.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Configura le opzioni di verifica avanzate, ad esempio la condivisione della bozza, l’aggiunta di un flusso di lavoro automatico o la configurazione delle impostazioni di accesso e abbonamento. Per ulteriori dettagli su queste opzioni, vedi i seguenti articoli:

   * [Condividere una bozza in [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Configurare una bozza con un flusso di lavoro automatico in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Configurare le impostazioni di accesso e abbonamento per una bozza](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Clic **[!UICONTROL Fine]**.

   Se stai aggiungendo una nuova versione a una bozza URL esistente, tutte le opzioni configurate sulla bozza originale o sulla versione precedente vengono mantenute in questa versione.Se stai aggiungendo una nuova versione a una bozza URL esistente, tutte le opzioni configurate sulla bozza originale o sulla versione precedente vengono mantenute in questa versione.

1. Clic **[!UICONTROL Crea bozza]**.

## Generare una bozza per il contenuto interattivo {#generate-a-proof-for-interactive-content}

Per utilizzare questa funzione è necessario un piano Pro Workfront o superiore. Per ulteriori informazioni sui vari piani disponibili, vedere [Piani Workfront](https://www.workfront.com/plans).

Per ulteriori informazioni sui contenuti interattivi, consulta [Panoramica delle bozze dei contenuti interattivi](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Aggiungere contenuto interattivo come URL](#add-interactive-content-as-a-url)
* [Aggiungere contenuto interattivo come file ZIP](#add-interactive-content-as-a-zip-file)

### Aggiungere contenuto interattivo come URL {#add-interactive-content-as-a-url}

Per informazioni su come aggiungere una bozza URL interattiva, consulta  [Generare una bozza per un URL](#generate-a-proof-for-a-url).

### Aggiungere contenuto interattivo come file ZIP {#add-interactive-content-as-a-zip-file}

1. Prepara il contenuto creando un file .zip.

   Per informazioni sulle specifiche dei file in bundle .zip, consulta [Informazioni sulla preparazione di contenuto interattivo in un file ZIP per la verifica](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md#howtoprepareaninteractiveziparchive) nell’articolo [Panoramica delle bozze dei contenuti interattivi](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Per iniziare a creare una nuova bozza e visualizzare la [!UICONTROL Nuova bozza] pagina:

   * Fai clic sul pulsante verde **[!UICONTROL Nuova bozza]** nell&#39;angolo superiore sinistro di qualsiasi pagina.
   * In **[!UICONTROL Dashboard]** area, nel **[!UICONTROL Panoramica]** , fare clic sulla scheda **[!UICONTROL Nuova bozza]** collegamento.

   * Invia tramite Dropzone (funzione Enterprise).

1. In **[!UICONTROL Nuova bozza]** che viene visualizzata, trascina e rilascia il pacchetto .zip interattivo nel **[!UICONTROL Aggiungi file]** area.

1. (Facoltativo) Configura le opzioni di verifica avanzate, ad esempio la condivisione della bozza, l’aggiunta di un flusso di lavoro automatizzato o la configurazione delle impostazioni di accesso e abbonamento. Per ulteriori dettagli su queste opzioni, vedi i seguenti articoli:

   * [Condividere una bozza in [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * nell’articolo
   * [Configurare le impostazioni di accesso e abbonamento per una bozza](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Clic **[!UICONTROL Crea bozza]**.

   Workfront inizia a generare una bozza del bundle .zip. A seconda delle dimensioni del bundle, il tempo di ritardo per il caricamento di un documento varia. La generazione di file più grandi richiede più tempo. Puoi spostarti dalla pagina e Workfront continua a generare il file. La dimensione massima per il caricamento dei file è di 4 GB.

   Una volta generata la bozza, puoi fare clic sul pulsante **[!UICONTROL Vai alla bozza]** che viene visualizzato per aprire la bozza.
