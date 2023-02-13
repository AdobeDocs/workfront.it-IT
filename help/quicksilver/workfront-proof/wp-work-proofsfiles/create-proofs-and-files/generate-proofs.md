---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Genera bozze in [!DNL Workfront Proof]
description: 'Workfront Proof consente di creare bozze da documenti o siti web e di condividerle con altri. I passaggi seguenti descrivono le varie opzioni di configurazione disponibili: EDIT ME.'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '2267'
ht-degree: 0%

---

# Genera bozze in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] consente di creare bozze da documenti o siti web e di condividerle con altri. I passaggi seguenti descrivono le varie opzioni di configurazione disponibili:

## Genera una bozza per un documento

1. Effettua una delle seguenti operazioni per iniziare a creare una nuova bozza e visualizzare il [!UICONTROL Nuova bozza] pagina:

   * Fai clic sul verde **[!UICONTROL Nuova prova]** nell’angolo in alto a sinistra di qualsiasi pagina.
   * In **[!UICONTROL Dashboard]** nella zona **[!UICONTROL Panoramica]** fai clic sulla scheda **[!UICONTROL Nuova prova]** link.

   * Invia tramite Dropzone (funzionalità Enterprise).
   * La **[!UICONTROL Nuova bozza]** viene visualizzata la pagina .

1. Per provare uno o più documenti, aggiungere i documenti da verificare in uno dei modi seguenti (ripetere questo processo per aggiungere più documenti da controllare):

   * Trascina un documento dal file system nell&#39;area di trascinamento nella **[!UICONTROL Aggiungi file]** area.
   * Fai clic nell’area di trascinamento nella **[!UICONTROL Aggiungi file]** , quindi sfoglia per trovare e selezionare il documento da caricare dal file system della workstation.

      ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. Per eseguire la bozza di uno o più siti web, specifica l’URL del sito web da verificare nel **[!UICONTROL Aggiungi file]** area, quindi premere **[!UICONTROL Invio]**.

1. (Facoltativo) Ripeti questa procedura per aggiungere più siti web alla bozza.

   Per ulteriori dettagli sulla correzione dei siti web, consulta [Genera una bozza per un URL](#generate-a-proof-for-a-url).

   ![](assets/proof-website-350x65.png)

1. (Facoltativo) Modifica i nomi dei file di qualsiasi file caricato:

   1. Passa il puntatore del mouse sul nome del documento che si desidera modificare nell&#39;elenco dei documenti nel **[!UICONTROL Aggiungi file]** fai clic sull’area **[!UICONTROL Modifica]** icona.

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. In **[!UICONTROL Nome della bozza]** campo , specifica un nuovo nome, quindi fai clic su **[!UICONTROL Fine]**.

   1. (Facoltativo) Per eliminare i file da caricare, passa il mouse sul documento da eliminare nell&#39;elenco dei documenti nel **[!UICONTROL Aggiungi file]** fai clic sull’area **[!UICONTROL Elimina]** icona.

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. (Facoltativo) Abilita l’opzione , **[!UICONTROL Combinare tutti i file compatibili in un’unica bozza]**.

      **Quando questa opzione è attivata:** Tutti i file statici e i siti web sono disponibili in un’unica bozza e puoi caricare fino a 50 file alla volta.

      >[!NOTE]
      >
      >I file interattivi, compresi i video e i siti web interattivi, non possono essere combinati in un’unica bozza.

      **Quando questa opzione è disabilitata:** Tutti i documenti e i siti web vengono generati come singole bozze e puoi caricare fino a 20 file alla volta.

      Per combinare tutti i file e i siti web caricati in un’unica bozza:

      1. Abilita l’opzione , **[!UICONTROL Combinare tutti i file compatibili in un’unica bozza]**.
      1. In **[!UICONTROL Nome della bozza]** Specifica un nuovo nome per la bozza combinata.
      1. In **[!UICONTROL Aggiungi file]** riordinare i file inclusi trascinando un file nell&#39;ordine desiderato. L’ordine dei file corrisponde all’ordine di pagina della bozza combinata. Per ulteriori informazioni sulla creazione di bozze combinate, consulta [Creare una bozza a più pagine](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. (Facoltativo) Se desideri utilizzare un flusso di lavoro automatizzato che include più fasi, nella **[!UICONTROL Flusso di lavoro]** seleziona una delle seguenti opzioni:

   * **Base:** Seleziona questa opzione per designare gli utenti a cui desideri accedere subito dopo la creazione della bozza. Puoi condividere la bozza con più utenti.

      Per ulteriori informazioni sulla condivisione di una bozza, consulta &quot;Aggiunta di utenti a una bozza&quot; in [Condividi una bozza in [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **Automatizzato:** Selezionare questa opzione per gestire la revisione e l’approvazione dei contenuti quando si hanno processi di revisione complessi o se si inviano regolarmente contenuti da rivedere agli stessi gruppi di persone. Con il flusso di lavoro automatizzato, la bozza si sposta da un passaggio all&#39;altro fino all&#39;approvazione finale. Gli utenti interessati vengono informati ogni volta che sono tenuti a rilasciare un&#39;approvazione.

      Per ulteriori informazioni sulla creazione di un flusso di lavoro automatizzato, consulta [Imposta una bozza con un flusso di lavoro automatizzato in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. Seleziona se inviare notifiche e-mail e un messaggio personalizzato agli utenti selezionati nel passaggio precedente:

   * **Notifica ai destinatari questa bozza:** Seleziona questa opzione per inviare una notifica e-mail agli utenti. Quando **[!UICONTROL Condivisione di base]** è selezionato in **[!UICONTROL Flusso di lavoro]** una notifica e-mail invia quando viene creata la bozza. Quando **[!UICONTROL Flusso di lavoro automatizzato]** è selezionato in **[!UICONTROL Flusso di lavoro]** una notifica e-mail invia quando la bozza entra nella fase del flusso di lavoro automatizzato a cui l’utente è associato.

   * **Aggiungi messaggio personalizzato:** Seleziona questa opzione per includere un messaggio personalizzato nella notifica. Puoi specificare un oggetto e il corpo del messaggio. Il corpo del messaggio può includere formattazione RTF, ad esempio grassetto, punti elenco e collegamenti ipertestuali.

1. Seleziona una delle seguenti impostazioni di bozza:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Richiedi accesso: la bozza può essere condivisa solo con altri utenti</td> 
      <td> <p><strong>Richiedi accesso: la bozza può essere condivisa solo con altri utenti:</strong> Quando questa opzione è selezionata, solo [!DNL Workfront Proof] Gli utenti possono visualizzare la bozza.</p> <p>Questa opzione è disabilitata per impostazione predefinita; chiunque disponga dell’URL può visualizzare la bozza.</p> <p>Quando questa opzione è selezionata:</p> 
       <ul> 
        <li>Gli utenti non possono accedere alla bozza a meno che non siano stati aggiunti alla bozza.</li> 
        <li>Impossibile abilitare le sottoscrizioni.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">È necessaria una sola decisione per questa prova</td> 
      <td> <p>Quando questa opzione è selezionata, la revisione viene completata dopo che uno dei decisori ha preso la loro decisione.</p> <p>Questa opzione è disabilitata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Richiedi la firma elettronica per le decisioni</td> 
      <td>Gli utenti devono specificare il proprio nome utente e la propria password al momento della decisione su una bozza.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Blocca la prova quando vengono prese tutte le decisioni necessarie</td> 
      <td> <p><strong></strong> Quando questa impostazione è abilitata, lo stato della bozza viene bloccato dopo tutte le decisioni. Lo stato viene automaticamente modificato da sbloccato a bloccato quando l’approvatore finale decide.</p> <p>Questa opzione è disabilitata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Scarica il file originale</td> 
      <td> <p><strong></strong> Quando questa opzione è selezionata, i revisori possono scaricare il file originale da cui è stata creata la bozza.</p> <p>Quando questa opzione è deselezionata, l’icona Scarica non è più visibile.<br>Questa opzione è attivata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Condividere la bozza tramite URL pubblico o codice di incorporamento</td> 
      <td>Quando questa opzione è selezionata, la bozza può essere condivisa tramite un URL pubblico o un codice di incorporamento.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Iscriviti alla bozza tramite URL pubblico o codice di incorporamento</td> 
      <td> <p>Quando questa opzione è selezionata, le persone che non sono state aggiunte esplicitamente alla bozza possono abbonarsi alla bozza. Alla persona che si abbona alla bozza viene assegnato il ruolo e l’e-mail definiti nelle seguenti impostazioni:</p> 
       <ul> 
        <li><strong>Ruolo del sottoscrittore</strong>: Il ruolo di bozza predefinito assegnato a tutti i revisori che si abbonano alla bozza.</li> 
        <li><strong>Impostazioni avvisi e-mail per gli abbonati</strong>: L’avviso e-mail predefinito assegnato a tutti i revisori che si abbonano alla bozza.</li> 
        <li> <p><strong>Accesso a prova tramite collegamento e-mail richiesto per</strong>: Configura se il sottoscrittore riceve un'e-mail con un collegamento alla bozza. È possibile selezionare <strong>Nessuna e-mail</strong> (il collegamento e-mail non è necessario per accedere alla bozza), <strong>Solo e-mail di notifica della bozza</strong> (l’abbonato riceve un collegamento alla prova via e-mail senza alcuna verifica), o <strong>E-mail di notifica di convalida e prova</strong> (L’utente iscritto riceve un collegamento alla bozza tramite e-mail e deve fare clic sul collegamento per accedere a una bozza; questa opzione ha lo scopo di garantire che la persona abbia inserito un indirizzo e-mail corretto al quale ha accesso).</p> <p>Nota: Se le bozze dispongono di Flusso di lavoro automatico allegato a tutte le sottoscrizioni genereranno e-mail di conferma al proprietario della bozza, in modo che possano decidere a quale fase aggiungere la persona.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Crea bozza]**.

   Workfront inizia a generare una bozza dei documenti o dei siti Web selezionati. A seconda delle dimensioni e del tipo di file, il tempo di ritardo nel caricamento di un documento varia. Sii paziente, perché i file più grandi richiedono più tempo per generare. Puoi allontanarti dalla pagina e Workfront continua a generare il file. La dimensione massima di caricamento dei file è 4 GB.

   Dopo aver generato la bozza, fai clic su **[!UICONTROL Vai alla bozza]** per avviare lo strumento di correzione.

   ![Screenshot_2018-05-16_08-59-34.png](assets/screenshot-2018-05-16-08-59-34-350x134.png)

   Il documento viene visualizzato nello strumento di correzione.

   Gli utenti che non dispongono di prove abilitate sul proprio account possono comunque visualizzare il documento e inviare commenti alla bozza.

## Genera una bozza per un URL {#generate-a-proof-for-a-url}

Puoi generare una bozza per un URL per la prima volta. Oppure puoi generare una nuova versione di una bozza URL in cui è stata precedentemente generata una bozza.

>[!NOTE]
>
>Puoi generare una bozza interattiva per un URL solo se [!DNL Workfront] l&#39;ambiente è integrato con un [!DNL Workfront Proof] Account Premium. Se non è possibile utilizzare le bozze come descritto in questa sezione, contatta l’amministratore di sistema.

Per generare una bozza per un URL:

1. Effettua una delle seguenti operazioni per iniziare a creare una nuova bozza e visualizzare il [!UICONTROL Nuova bozza] pagina:

   * Fai clic sul verde **[!UICONTROL Nuova prova]** nell’angolo in alto a sinistra di qualsiasi pagina.
   * In **[!UICONTROL Dashboard]** nella zona **[!UICONTROL Panoramica]** fai clic sulla scheda **[!UICONTROL Nuova prova]** link.

   * Invia tramite Dropzone (funzionalità Enterprise).

1. (Condizionale) Nel **[!UICONTROL Nuova prova]** per creare una nuova versione di una bozza esistente:

   1. Seleziona la bozza URL in cui desideri aggiungere una nuova versione.
   1. Fai clic sul pulsante **[!UICONTROL Nuova versione]** nella parte superiore della pagina.

      ![Screenshot_2018-05-15_10-59-56.png](assets/screenshot-2018-05-15-10-59-56-350x80.png)

1. Nella pagina Nuova versione di prova visualizzata, specifica l’URL del sito web da verificare nel **[!UICONTROL Aggiungi file]** area, quindi premere **[!UICONTROL Invio]**.

1. (Facoltativo) Ripeti questa procedura per aggiungere più siti web alla bozza.

   ![proof_website.png](assets/proof-website-350x65.png)

1. Fai clic sul sito web nell’elenco dei documenti nel **[!UICONTROL Aggiungi file]** area.

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. Specifica una **[!UICONTROL Nome della bozza]** per la prova.

   Per impostazione predefinita, il nome della bozza è lo stesso dell’URL del sito.

1. Seleziona **[!UICONTROL Gestire il contenuto del sito]** opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Schermata di acquisizione</td> 
      <td>Crea una bozza di un’immagine statica della prima pagina dell’URL.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Interattiva</td> 
      <td> <p>Crea una bozza che consente ai revisori di navigare nel sito, visualizzare immagini HTML5, elementi Flash e così via.</p> <p>Per creare una bozza interattiva, il sito web deve essere ospitato con un protocollo sicuro (https). Inoltre, i siti web che non possono essere incorporati in un iframe non possono essere generati come bozza interattiva (le restrizioni relative all’incorporamento di iframe sono controllate dal sito web che si sta tentando di incorporare).</p> <p>Dopo la creazione della bozza iniziale, questa impostazione non può essere modificata quando si creano versioni successive.</p> <p>Per ulteriori informazioni sulla correzione interattiva, consulta <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">Genera una bozza per il contenuto interattivo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Risoluzione dello schermo</td> 
      <td> <p>Questa opzione non è disponibile per le bozze interattive. È possibile regolare la risoluzione in cui viene visualizzato il contenuto oppure selezionare più risoluzioni.</p> <p>Questo consente agli utenti di esaminare la bozza per vedere come verrà visualizzato il contenuto su diversi dispositivi, come telefoni, tablet e monitor di varie dimensioni.</p> <p>Se selezioni più risoluzioni, viene creata una bozza separata per ogni risoluzione selezionata.</p> <p>Quando gli utenti commentano la bozza, la risoluzione attuale dello schermo viene visualizzata automaticamente nel commento per assicurarsi che gli altri utenti siano a conoscenza della risoluzione a cui è associato il commento.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cercare pagine secondarie</td> 
      <td>Questa opzione non è disponibile per le bozze interattive. Seleziona questa opzione per navigare tra le pagine del sito web. È possibile espandere il sito web fino a 2 livelli di profondità dalla pagina principale. Passa il puntatore del mouse su una pagina per visualizzare l’URL della pagina. Seleziona solo le pagine da provare. Per impostazione predefinita, ogni pagina selezionata viene creata come bozza singola; o, <strong>Combinare in un'unica bozza</strong> per combinare tutte le pagine selezionate in un’unica bozza.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Configura eventuali opzioni di correzione avanzate, ad esempio condivisione della bozza, aggiunta di un flusso di lavoro automatizzato o configurazione delle impostazioni di accesso e abbonamento. Per ulteriori dettagli su queste opzioni, vedi i seguenti articoli:

   * [Condividi una bozza in [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Imposta una bozza con un flusso di lavoro automatizzato in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Configurare le impostazioni di accesso e sottoscrizione per una bozza](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Fai clic su **[!UICONTROL Fine]**.

   Se aggiungi una nuova versione a una bozza URL esistente, tutte le opzioni configurate sulla bozza originale o sulla versione precedente vengono mantenute in questa versione. Se aggiungi una nuova versione a una bozza URL esistente, tutte le opzioni configurate sulla bozza originale o sulla versione precedente verranno mantenute in questa versione.

1. Fai clic su **[!UICONTROL Crea bozza]**.

## Genera una bozza per il contenuto interattivo {#generate-a-proof-for-interactive-content}

Per utilizzare questa funzione è necessario un piano Workfront Pro o superiore. Per ulteriori informazioni sui vari piani disponibili, vedi [Piani Workfront](https://www.workfront.com/plans).

Per ulteriori informazioni sul contenuto interattivo, consulta [Panoramica delle bozze dei contenuti interattivi](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Aggiungere contenuto interattivo come URL](#add-interactive-content-as-a-url)
* [Aggiungere contenuto interattivo come file ZIP](#add-interactive-content-as-a-zip-file)

### Aggiungere contenuto interattivo come URL {#add-interactive-content-as-a-url}

Per informazioni su come aggiungere una bozza URL interattiva, consulta  [Genera una bozza per un URL](#generate-a-proof-for-a-url).

### Aggiungere contenuto interattivo come file ZIP {#add-interactive-content-as-a-zip-file}

1. Prepara il contenuto creando un file .zip in bundle.

   Per informazioni sulle specifiche dei file .zip raggruppati, vedi [Informazioni sulla preparazione del contenuto interattivo in un file ZIP per la correzione del contenuto](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md#howtoprepareaninteractiveziparchive) nell&#39;articolo [Panoramica delle bozze dei contenuti interattivi](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Effettua una delle seguenti operazioni per iniziare a creare una nuova bozza e visualizzare il [!UICONTROL Nuova bozza] pagina:

   * Fai clic sul verde **[!UICONTROL Nuova prova]** nell’angolo in alto a sinistra di qualsiasi pagina.
   * In **[!UICONTROL Dashboard]** nella zona **[!UICONTROL Panoramica]** fai clic sulla scheda **[!UICONTROL Nuova prova]** link.

   * Invia tramite Dropzone (funzionalità Enterprise).

1. In **[!UICONTROL Nuova prova]** pagina visualizzata, trascina e rilascia il bundle .zip interattivo nel **[!UICONTROL Aggiungi file]** area.

1. (Facoltativo) Configura eventuali opzioni di correzione avanzate, ad esempio condivisione della bozza, aggiunta di un flusso di lavoro automatizzato o configurazione delle impostazioni di accesso e abbonamento. Per ulteriori dettagli su queste opzioni, vedi i seguenti articoli:

   * [Condividi una bozza in [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * nell&#39;articolo
   * [Configurare le impostazioni di accesso e sottoscrizione per una bozza](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Fai clic su **[!UICONTROL Crea bozza]**.

   Workfront inizia a generare una bozza del bundle .zip. A seconda delle dimensioni del bundle, il tempo di ritardo nel caricamento di un documento varia. La generazione di file più grandi richiede più tempo. Puoi allontanarti dalla pagina e Workfront continua a generare il file. La dimensione massima di caricamento dei file è 4 GB.

   Dopo la generazione della bozza, puoi fare clic sul pulsante **[!UICONTROL Vai alla bozza]** pulsante che consente di aprire la bozza.
