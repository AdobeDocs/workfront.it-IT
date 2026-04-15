---
product-area: documents
navigation-topic: approvals
title: Panoramica sulla revisione e sull’approvazione unificata
description: Ulteriori informazioni sulla revisione e l'approvazione unificate fornite da Workfront e Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 32cb95c2-8d12-492b-ad89-b38e2a337fc5
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453d4862883e299fea46b3dfe94548375bfc4209
workflow-type: tm+mt
source-wordcount: '3846'
ht-degree: 0%

---


# Panoramica sulla revisione e sull’approvazione unificata

La revisione e l’approvazione unificate riuniscono Adobe Workfront e Adobe Frame.io in un’unica esperienza profondamente connessa, che colma le lacune esistenti tra la gestione del marketing, la revisione creativa e la distribuzione dei contenuti.
I coordinatori dei progetti gestiscono il lavoro in Workfront, mentre i creativi, gli esperti di marketing e le parti interessate esaminano e approvano le risorse nel visualizzatore Frame.io di livello professionale, il tutto senza spostare i file tra strumenti disconnessi.

![Diagramma che mostra il flusso di lavoro unificato di revisione e approvazione, con i coordinatori del progetto che gestiscono il lavoro in Workfront e i revisori e gli approvatori che forniscono feedback e prendono decisioni nel visualizzatore Frame.io.](assets/Unified-Review-Approvals-Image.png)


## Requisiti di integrazione

* L’istanza di Workfront deve essere abilitata in Adobe Unified Experience.


## Basato sullo storage aziendale Adobe

La revisione e l&#39;approvazione unificate si basano sullo storage aziendale Adobe, una soluzione di storage basata su cloud che funge da archivio centrale per le risorse dei prodotti aziendali Adobe, inclusi Workfront e Frame.io. <!--, and Creative Cloud.-->

I principali vantaggi dello storage aziendale Adobe includono:

* Livello di storage unificato per risorse creative e di gestione del lavoro
* Autorizzazioni centralizzate con Adobe Identity Management System (IMS) per il controllo sicuro degli accessi
* Visibilità completa delle risorse in Workfront e Frame.io <!--, and Creative Cloud apps -->
* Storage scalabile e gestione delle quote per le esigenze aziendali

Per ulteriori dettagli, consulta [Panoramica sull&#39;archiviazione aziendale di Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Revisione e approvazione unificate

Con la revisione e l&#39;approvazione unificate, puoi:

* Crea e gestisci revisioni e approvazioni direttamente da Workfront
* Monitorare lo stato di revisioni e approvazioni in tempo reale
* Centralizzare feedback e approvazioni in un&#39;unica posizione
* Assicurati che tutte le parti interessate abbiano accesso alle versioni più recenti delle risorse
* Utilizzare i revisori AI per automatizzare le revisioni di conformità al brand
* e molto altro

Per ulteriori informazioni, vedere [Unified document approvals: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### Utilizzare il visualizzatore Frame.io

Utilizza il visualizzatore Frame.io per rivedere e approvare le risorse. Il visualizzatore Frame.io fornisce

* Strumenti di markup e commento
* Cronologia e confronto delle versioni
* Commenti con marca temporale per le recensioni video
* Accesso mobile per revisioni e approvazioni in movimento

Per ulteriori informazioni, vedere [Introduzione alla revisione e all&#39;approvazione unificate](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

#### Limiti di revisione video

Per le richieste di bozze video, il limite massimo annuale è fissato al 10% del totale delle licenze Workfront a pagamento di un&#39;organizzazione: Standard e Light. Questo limite viene applicato a livello di organizzazione.

Gli amministratori di Workfront ricevono notifiche quando l’utilizzo raggiunge l’80% e il 100% del limite.

Questo limite non si applica ai clienti Frame.io Enterprise.

#### Tipi di file supportati nel visualizzatore Frame.io

Il visualizzatore Frame.io supporta tutti i tipi comuni di video, immagini, audio, PDF e MS® Office. Per un elenco dettagliato dei file supportati, vedere [Tipi di file supportati in Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Accesso e licenze per il visualizzatore Frame.io

Il visualizzatore Frame.io è il visualizzatore predefinito per tutti i flussi di lavoro di revisione e approvazione di Workfront. È incluso automaticamente per tutti gli utenti di Workfront con una licenza a pagamento. Non è richiesta alcuna licenza Frame.io aggiuntiva per utilizzare il visualizzatore Frame.io per le revisioni e le approvazioni.

Se la tua organizzazione desidera sfruttare le funzionalità Frame.io aggiuntive disponibili con questa integrazione, ad esempio per caricare le risorse direttamente nei progetti in Frame.io, puoi acquistare una licenza Frame.io Enterprise. Contatta il rappresentante del tuo account Adobe per pianificare una demo ed esplorare i vantaggi della soluzione Frame.io completa.

La funzionalità Workfront Proofing non è disponibile con questa integrazione.

## Potente gestione dei progetti in Workfront

I coordinatori dei progetti possono sfruttare le potenti funzionalità di gestione dei progetti di Workfront per pianificare, tracciare e gestire il lavoro.

Per ulteriori informazioni sulla gestione dei progetti in Workfront, vedere [Progetti: indice articolo](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Struttura imposta e convenzioni di denominazione

Poiché la revisione e l’approvazione unificate vengono create utilizzando lo storage aziendale Adobe, è necessario tenere presenti alcune convenzioni di denominazione e struttura applicate durante la gestione di progetti e documenti.

* I programmi e i progetti non possono avere lo stesso nome se appartengono allo stesso portfolio.
* I documenti non possono avere lo stesso nome se appartengono allo stesso progetto.
* I nomi degli oggetti non possono contenere i seguenti caratteri speciali: \ / : * ? &quot; | &lt; >
* I nomi degli oggetti possono contenere un massimo di 255 caratteri.

Tenendo presenti queste limitazioni, Workfront rinomina automaticamente gli oggetti o i documenti in base alle esigenze per evitare conflitti.

### Condivisione e autorizzazioni

Come parte dell&#39;integrazione, le autorizzazioni utente sono controllate in Workfront e si estendono fino a Frame.io. Ciò significa che non è possibile invitare un utente a un progetto in Frame.io o modificare le autorizzazioni utente in Frame.io. Queste azioni devono essere eseguite tramite la finestra modale Condivisione progetto in Workfront.

Nella tabella seguente viene illustrato il mapping delle autorizzazioni di Workfront alle autorizzazioni Frame.io:

<table>
<tr>
<th>Autorizzazione utente di Workfront</th>
<th>Autorizzazione utente Frame.io</th>
</tr>
<tr>
<td>Gestione</td>
<td>Modifica e condividi</td>
</tr>
<tr>
<td>Contribuisci</td>
<td>Modifica e condividi</td>
</tr>
<tr>
<td>Visualizzazione</td>
<td>Solo commento</td>
</tr>
</table>



### Gestione dei documenti in Workfront

I documenti caricati su Workfront vengono memorizzati nello storage aziendale di Adobe e sono accessibili sia in Workfront che in Frame.io. Quando carichi un documento in un’attività o un problema in Workfront, viene creata una cartella generata dal sistema nell’archiviazione aziendale di Adobe che eredita le autorizzazioni dall’attività o dal problema. Tutti i documenti caricati su tale attività o problema sono memorizzati in tale cartella e da essa ereditano le autorizzazioni. Per ulteriori informazioni sui documenti in Workfront, vedere [Panoramica sulla nuova area documenti](/help/quicksilver/documents/managing-documents/documents-area.md) e [Autorizzazioni oggetto e panoramica del livello di accesso per il modello di archiviazione aziendale Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

### Limitazioni dell’esperienza documentale

Le seguenti funzionalità di Document non sono incluse:

<!--* External document providers-->
* Accesso alle bozze in Workfront
* Visualizzatore documenti in Workfront
* Documenti preferiti
* Richiedi documenti

## Introduzione a revisione e approvazione unificate

Per iniziare a utilizzare la revisione e l&#39;approvazione unificate, consulta [Introduzione alla revisione e all&#39;approvazione unificate](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

## Domande frequenti

### Guida introduttiva alla revisione e all&#39;approvazione unificate

+++ Espandi per visualizzare le domande frequenti per iniziare a utilizzare la revisione e l’approvazione unificate.

**Che cos&#39;è la revisione e l&#39;approvazione unificate?**

Revisione e approvazione unificate è un&#39;integrazione nativa tra Adobe Workfront e Adobe Frame.io che riunisce gestione del lavoro e revisione creativa in un unico sistema connesso. I coordinatori dei progetti pianificano e tengono traccia del lavoro in Workfront, mentre i revisori e gli approvatori utilizzano il visualizzatore Frame.io di livello professionale per fornire feedback, contrassegnare le risorse e prendere decisioni di approvazione, senza dover passare da uno strumento separato all&#39;altro o spostare manualmente i file.

La revisione e l&#39;approvazione sono al centro di ogni operazione relativa ai contenuti. È qui che convergono il lavoro creativo, il contributo delle parti interessate e le decisioni aziendali. Quando il processo viene distribuito tra strumenti disconnessi (thread e-mail, messaggi di chat, markup di schermate), le conseguenze sono composte da: tempi di commercializzazione più lenti, feedback persi, confusione delle versioni e tempo impiegato per la gestione dei file anziché per la creazione dei contenuti.

La revisione e l&#39;approvazione unificate affrontano questo problema sostituendo il mosaico di strumenti di revisione disconnessi con un sistema moderno, un&#39;unica fonte di verità che vive dove il lavoro già avviene.

**Quali sono i requisiti per utilizzare questa integrazione?**

Per utilizzare la revisione e l’approvazione unificate, è necessario soddisfare le seguenti condizioni:

* Workfront e Frame.io devono essere distribuiti nella stessa organizzazione Adobe Identity Management System (IMS).

* Gli utenti possono appartenere a una sola istanza di Workfront all’interno dell’organizzazione IMS.

* L’istanza di Workfront deve essere abilitata sullo storage aziendale Adobe Unified Experience e Adobe.

* I clienti Workfront devono utilizzare una SKU V2 (potrebbe essere necessario un evento contrattuale: contatta il rappresentante del tuo account Adobe).

**È necessaria una licenza Frame.io per utilizzare questa integrazione?**

No. Il visualizzatore Frame.io viene incluso automaticamente per tutti gli utenti di Workfront con una licenza a pagamento senza costi aggiuntivi. Non è necessaria una licenza Frame.io separata per rivedere e approvare le risorse tramite Workfront.

Se la tua organizzazione desidera accedere a funzionalità Frame.io aggiuntive, ad esempio per caricare le risorse direttamente nei progetti in Frame.io, puoi acquistare una licenza Enterprise Frame.io. Per ulteriori informazioni, contatta il rappresentante del tuo account Adobe.

**Sostituisce Workfront Proof?**

Sì. Quando la revisione e l&#39;approvazione unificate sono abilitate, il visualizzatore Frame.io diventa la superficie di revisione principale in Workfront, sostituendo Workfront Proof.

I clienti esistenti manterranno l’accesso alla funzionalità di verifica di Workfront per tutti i progetti creati prima che l’integrazione fosse abilitata.

**Come posso accedere a Revisione e approvazione unificate?**

**Cosa devo fare per ottenere l&#39;accesso?**

Per accedere alla revisione e all’approvazione unificate, la tua organizzazione deve utilizzare una SKU di Workfront V2. Se non ti trovi attualmente in una SKU V2, sarà necessario un evento contrattuale con Adobe. Per iniziare:

* Contatta il rappresentante del tuo account Adobe per verificare se il piano Workfront corrente supporta la revisione e l’approvazione unificate.

* Se è necessario un aggiornamento SKU, il rappresentante del tuo account ti guiderà attraverso il processo di contrattazione.

* Una volta che il tuo account è nello SKU corretto, Adobe Professional Services configurerà l’integrazione per la tua organizzazione.

   * Se non sai chi sia il rappresentante del tuo account Adobe, puoi contattare il portale di assistenza Adobe o visitare Experience League per informazioni sulle opzioni di contatto.

+++

### Funzionamento della revisione e dell’approvazione unificate

+++ Espandi per visualizzare le domande frequenti sul funzionamento della revisione e dell’approvazione unificate.

**Come funziona il flusso di lavoro di revisione e approvazione?**

Il flusso di lavoro segue questi passaggi generali:

1. Un coordinatore di progetto crea un progetto in Workfront e carica o collega le risorse.

1. Quando una risorsa è pronta per la revisione, il coordinatore crea un flusso di lavoro di approvazione, un’approvazione per singolo utilizzo o applicando un modello di approvazione riutilizzabile.

1. I revisori e gli approvatori assegnati ricevono una notifica tramite e-mail e possono aprire la risorsa direttamente nel visualizzatore Frame.io.

1. I revisori possono aggiungere commenti e markup. Gli approvatori devono prendere una decisione formale.

1. Il coordinatore tiene traccia dello stato in tempo reale da Workfront.

**Qual è la differenza tra un revisore e un approvatore?**

I revisori possono aggiungere commenti e contrassegnare le risorse nel visualizzatore Frame.io. Al termine, contrassegnano la loro recensione come completa. Tuttavia, la loro azione non è necessaria per far avanzare il flusso di lavoro di approvazione.

Per portare avanti il flusso di lavoro di approvazione, gli approvatori devono effettuare una delle seguenti operazioni:

* **Approva**: la risorsa è pronta per essere utilizzata così com&#39;è.

* **È necessario lavorare**: la risorsa richiede modifiche e deve essere inviata nuovamente come nuova versione per la nuova approvazione.

**Quali tipi di flussi di lavoro di approvazione è possibile creare?**

* **Approvazioni per singolo utilizzo**: è possibile creare un&#39;approvazione per singolo utilizzo direttamente in un documento di un progetto, un&#39;attività o un problema. Se necessario, è possibile assegnare revisori e approvatori, impostare una scadenza e configurare più fasi. I promemoria e-mail automatizzati vengono inviati 72 ore prima, 24 ore prima e alla scadenza.

* **Modelli di approvazione**: è possibile creare modelli riutilizzabili in Installazione di Workfront. Un modello definisce i revisori, gli approvatori e un periodo di completamento relativo. Se necessario, puoi creare più fasi. Una volta applicato un modello a una risorsa, la scadenza viene calcolata automaticamente.

**In che modo gli utenti esterni partecipano alle revisioni?**

Gli utenti esterni di Workfront ricevono una notifica tramite e-mail quando vengono assegnati a una revisione o approvazione. Viene richiesto di creare un accesso Frame.io per accedere al visualizzatore e partecipare al processo di revisione.

**Come si tiene traccia dell&#39;avanzamento di revisione e approvazione?**

I coordinatori dei progetti possono monitorare tutte le approvazioni in volo in diversi modi:

* Il widget Approvazioni personali nell&#39;area Home di Workfront fornisce un riepilogo in tempo reale delle approvazioni in sospeso e in ritardo.

* Il widget Metriche di approvazione documento visualizza i tempi medi di approvazione e i raggruppamenti delle decisioni.

* Le dashboard dei rapporti personalizzati possono essere incorporate in dashboard di Canvas per una visibilità più approfondita delle attività di revisione e approvazione.

+++


### Revisione e approvazione di risorse e video

+++ Espandi per visualizzare le domande frequenti sulla revisione e l’approvazione di risorse e video.

**Esistono limiti alle recensioni video?**

Sì. È previsto un limite annuo per le richieste di bozze video, fissato al 10% del totale delle licenze utente Workfront a pagamento dell’organizzazione (Standard e Light). Questo limite si applica a livello di organizzazione.

Gli amministratori di Workfront riceveranno notifiche in-app quando l’utilizzo raggiunge l’80% e il 100% del limite.

Questo limite non si applica ai clienti Frame.io Enterprise. Se la tua organizzazione rivede regolarmente grandi quantità di contenuti video, contatta il rappresentante del tuo account Adobe per scoprire le licenze Enterprise di Frame.io.

**Lo stesso utente può essere visualizzato in più fasi di un flusso di lavoro di approvazione?**

Sì. Un utente può essere assegnato a più fasi all’interno dello stesso flusso di lavoro di approvazione.

**Posso aggiungere fasi per creare un flusso di lavoro di approvazione con più fasi?**

Sì. Sono supportati flussi di lavoro di approvazione in più fasi, che consentono di indirizzare le risorse attraverso cicli sequenziali di revisione e approvazione con partecipanti diversi in ogni fase.

<!--
**Can I modify the trigger for a later stage---for example, based on all approved versus the due date ending?**

Stages in a multi-stage approval workflow proceed sequentially based on all required decisions being made in the current stage. When all assigned approvers in a stage have made their decisions, the next stage begins and the previous stage is locked. There is no option to trigger a stage based on the due date ending. If the "One decision required" toggle is enabled on a stage, the first approver decision completes that stage and advances the workflow.

**Can I remove the due date from an approval?**

Yes. Due dates are optional for both single-use approvals and approval templates. When creating a single-use approval, you can leave the deadline field empty. For approval templates, the relative completion timeframe is also optional.

**Can I change the default due date on new approval templates?**

Yes. When creating or editing an approval template, the timeframe (or "Workdays until due date" for multi-stage templates) can be adjusted per stage or left empty. The deadline is calculated automatically from this timeframe when the template is applied to an asset, so updating the template changes the default for all future approvals that use it.

**What happens when the deadline is reached for a review stage?**

For both single-stage and multi-stage reviews, automated reminder emails are sent at 72 hours, 24 hours, and on the deadline. However, reaching the deadline does not automatically reject the asset, lock the stage, or advance the workflow. Approvers and reviewers can still make decisions or complete their review after the deadline has passed. In a multi-stage workflow, each stage has its own independent deadline, and stages still advance based on all required decisions being made---not based on the deadline.
-->

**I modelli di approvazione possono includere gruppi o team oppure solo singoli utenti?**

Attualmente, i modelli di approvazione supportano singoli utenti e team.

**Gli approvatori ricevono una notifica via e-mail quando hanno qualcosa da rivedere?**

Sì. Gli approvatori e i revisori ricevono notifiche e-mail quando vengono assegnati a una revisione o approvazione. Anche le e-mail di promemoria automatizzati vengono inviate 72 ore prima della scadenza, 24 ore prima e alla scadenza stessa.

La possibilità di personalizzare i messaggi di notifica e-mail non è attualmente disponibile, ma è inclusa nella roadmap del prodotto.

<!--
**Can I change the notification frequency for a unified approver or reviewer (for example, all comments, replies to my comments, or daily summaries)?**

No. Notification frequency settings such as receiving all comments, only replies to your comments, or daily digest summaries are not currently available for unified review and approval. The system sends email notifications automatically when a user is assigned as a reviewer or approver, and automated reminder emails are sent at 72 hours, 24 hours, and on the deadline. The ability to customize notification messages and frequency is on the product roadmap.
-->

**È possibile mantenere privata una fase di revisione rispetto agli altri partecipanti?**

Attualmente non è disponibile alcuna funzione di stage privato. Per mantenere una revisione privata rispetto agli altri partecipanti, l’approccio consigliato consiste nel creare una copia separata della risorsa specificamente per quel gruppo di revisione. I commenti non sono attualmente segmentati per gruppo di partecipanti all’interno di una singola risorsa.

La cronologia delle versioni, incluse quelle precedenti e correnti, è sempre visibile a chiunque abbia accesso alla visualizzazione della risorsa.

**È possibile contrassegnare i commenti come risolti?**

Sì. I commenti possono essere contrassegnati come risolti nel visualizzatore Frame.io.

**Quali strumenti di markup e annotazione sono disponibili nel visualizzatore Frame.io?**

Il visualizzatore Frame.io include un set completo di strumenti di markup visivo, inclusi disegno a mano libera e forme standard quali cerchi, frecce e quadrati. Per le risorse video, i commenti vengono contrassegnati con una precisione di frame che ne determina la posizione temporale e non solo quella generale.

**I commenti aggiunti nel visualizzatore Frame.io verranno visualizzati nel progetto Workfront?**

I commenti e le annotazioni rimangono all&#39;interno del visualizzatore Frame.io in modo che mantengano il contesto completo, inclusi i timestamp e le marcature visive. Questo comportamento potrebbe evolvere nelle versioni future.

**È possibile aggiungere commenti a una versione scaricata di una risorsa (ad esempio, un PDF)?**

Attualmente non è supportata, ma si tratta di una funzionalità comunemente richiesta e attualmente in fase di valutazione per una versione futura.

**È possibile esaminare più risorse insieme come gruppo?**

Le opzioni di revisione in blocco migliorate saranno presto disponibili. Nel frattempo, risorse di diversi tipi di file, come un video e un documento Word, possono essere incluse insieme in una revisione di risorse raggruppate.

**La revisione e l&#39;approvazione unificate sono valide solo per i video o supportano altri tipi di file?**

La revisione e l’approvazione unificate sono progettate per tutti i tipi di risorse, non solo per i video. Il visualizzatore Frame.io è stato aggiornato in modo significativo per supportare immagini, documenti, PDF e altri formati di file comuni oltre al video.

Per un elenco completo dei tipi di file supportati, consulta la documentazione sui tipi di file supportati da Frame.io in Experience League.

**Posso condividere risorse esternamente con soggetti interessati che non hanno accesso a Workfront?**

Sì. Assets può essere condiviso esternamente. Agli utenti esterni viene inviata una notifica tramite e-mail e viene richiesto di creare un accesso Frame.io per accedere al visualizzatore e partecipare alla revisione.

<!--
**Before unified review and approval, is a reviewer just directed to a proof?**

Yes. In the legacy proofing workflow (prior to unified review and approval), when a user was assigned as a reviewer they were directed to the Workfront Proof viewer (ProofHQ) to review the proof. With unified review and approval, reviewers are instead directed to the Frame.io viewer, which replaces the Workfront Proof viewer as the primary review surface.

**When I upload a document and not a proof, a proof gets generated. Will a proof always be generated?**

No. With unified review and approval enabled and Adobe enterprise storage active, uploading a document does not automatically generate a proof. Documents are stored in Adobe enterprise storage and are reviewed using the Frame.io viewer. A proof is only generated if you explicitly create one using the legacy proofing workflow. The Frame.io viewer serves as the primary review surface, so a separate proof is not needed for standard review and approval workflows.

**What is the difference between uploading a document and a proof after the 26.2 release?**

With unified review and approval enabled, uploading a document stores it in Adobe enterprise storage and makes it available for review in the Frame.io viewer. A unified approval workflow can be created directly on the document. Uploading a proof, by contrast, uses the legacy Workfront Proof viewer (ProofHQ) and its own proofing workflow. Both options are available for projects created before the integration was enabled, but the Frame.io viewer is the primary review surface going forward. The key difference is that a document uses the unified approval workflow and Frame.io viewer, while a proof uses the legacy proofing workflow and viewer.

**Reviews under My Approvals only show a "Complete my review" button and no link to the proofing viewer or the document. Is this intended?**

For unified review and approval, the My Approvals widget provides an "Open review" button that opens the asset in the Frame.io viewer, as well as action buttons to approve, request changes, or complete a review. Reviewers can complete their review directly from the widget. If you are only seeing a "Complete my review" button without a link to the viewer, this may reflect the reviewer role behavior---reviewers are not required to open the asset to mark their review as complete, though they can choose to open it in the Frame.io viewer to provide feedback before completing.

**Before unified review and approval, if a user is both an approver in a document approval and a reviewer/approver on a proof, both show up in the proof window. How do these work together?**

When using unified approvals alongside legacy proofing on the same document, the two workflows operate independently. Document approval participants are shown in the Document Summary panel, while proof participants are shown in the proofing workflow. The SOCD (Sent, Opened, Comment, Decision) indicators in the document list are proofing-related and do not reflect the unified approval decision status. These two workflows do not automatically sync---a decision made in one does not carry over to the other.

**If you upload a new version, the document approval users do not get repopulated. Is that intended?**

Yes. When a new version is uploaded, previous approval participants are not automatically repopulated. The previous version's approval process is closed and any outstanding approvals are marked as "Withdrawn." The document owner must manually add participants to the new version's approval workflow. An "Add all" button is available to quickly repopulate all participants from the previous version, and you can also selectively add previous participants or add new ones.
-->

+++

### Storage e gestione dei file

+++ Espandere per visualizzare le domande frequenti relative allo storage e alla gestione dei file.

**Cos&#39;è l&#39;archiviazione aziendale di Adobe e come si relaziona a questa integrazione?**

Lo storage aziendale Adobe è il livello di storage comune che collega Workfront, Frame.io e Adobe Creative Cloud. Assets live in un’unica posizione e sono accessibili da uno strumento all’altro senza trasferimenti manuali di file. I creativi possono lavorare sul posto e i revisori vedono sempre la versione più recente.

I principali vantaggi dello storage aziendale Adobe includono:

* Un unico livello di storage per tutte le risorse in esecuzione in Workfront e Frame.io

* Controllo centralizzato degli accessi gestito tramite Adobe Identity Management System (IMS)

* Visibilità completa delle risorse: nessuna deviazione delle versioni, nessuna perdita di metadati

* Gestione scalabile dello storage di livello enterprise

**Esistono requisiti di denominazione o struttura per file e progetti?**

Sì. Poiché l’integrazione utilizza lo storage aziendale Adobe, si applicano le seguenti convenzioni:

* I programmi e i progetti non possono avere lo stesso nome se appartengono allo stesso portfolio.

* I nomi dei documenti devono essere univoci all&#39;interno dello stesso elemento padre nella gerarchia delle cartelle.

* I documenti all’interno dello stesso progetto non possono condividere un nome.

* Programmi, portfolio, progetti, modelli, attività, problemi, documenti e nomi di cartelle di documenti non possono contenere i seguenti caratteri speciali: `\ / : * ? " | < >` e sono limitati a 255 caratteri.

Workfront rinomina automaticamente gli oggetti o i documenti in base alle esigenze per evitare conflitti.

**Quali tipi di file sono supportati nel visualizzatore Frame.io?**

Il visualizzatore Frame.io supporta oltre 40 formati di file, inclusi tutti i tipi comuni di file video, immagini, audio, PDF e Microsoft Office. Il supporto video include la riproduzione nativa per formati professionali quali ProRes, H.265 e DNxHD, con supporto per file fino a 500 GB.

Frame.io è stato creato appositamente per la revisione creativa, ossia per gestire l’intera gamma di tipi di risorse con cui lavorano i team di marketing e creativi.

+++

### Autorizzazioni e accesso

+++ Espandi per visualizzare le domande frequenti su autorizzazioni e accesso.

**Gestione delle autorizzazioni utente**

Le autorizzazioni utente vengono impostate e controllate in Workfront e passano automaticamente a Frame.io. Non puoi invitare utenti o modificare le autorizzazioni direttamente in Frame.io per questa integrazione. Tutta la gestione degli accessi deve essere eseguita utilizzando la finestra modale di condivisione del progetto in Workfront.

La tabella seguente mostra il mapping delle autorizzazioni di Workfront alle autorizzazioni Frame.io:

<table>
  <thead>
    <tr>
      <th>Autorizzazione Workfront</th>
      <th>Autorizzazione Frame.io</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Gestione</td>
      <td>Modifica e condividi</td>
    </tr>
    <tr>
      <td>Contribuisci</td>
      <td>Modifica e condividi</td>
    </tr>
    <tr>
      <td>Visualizzazione</td>
      <td>Solo commento</td>
    </tr>
  </tbody>
</table>

+++


### Integrazioni e funzionalità avanzate

+++ Espandi per visualizzare le domande frequenti sulle integrazioni e sulle funzionalità avanzate.

**Che impatto ha questo sulle integrazioni esistenti del plug-in Creative Cloud con Adobe Express e GenStudio?**

Le integrazioni che supportano l&#39;esperienza di visualizzazione Frame.io sono attualmente in fase di sviluppo per Adobe Express e GenStudio Performance Marketing. Le nuove integrazioni saranno basate sullo stesso sistema unificato di revisione e approvazione, in modo da sfruttare il visualizzatore Frame.io per un&#39;esperienza di revisione coerente su tutti e tre i prodotti.

**Frame.io è integrato in Workfront oppure gli utenti passano a un&#39;interfaccia separata?**

Gli utenti possono avviare il visualizzatore Frame.io direttamente da Workfront. Tutte le attività di revisione e approvazione si svolgono all&#39;interno del visualizzatore Frame.io e vengono sincronizzate automaticamente con Workfront.

**Posso inviare risorse approvate a Adobe Experience Manager (AEM)?**

Sì. Una volta che una risorsa completa il ciclo di revisione e approvazione, puoi trasferirla ad Adobe Experience Manager Assets per l’archiviazione e la distribuzione finali. Questo collega Workfront per la gestione del lavoro, Frame.io per la revisione e AEM per la gestione delle risorse digitali in un supply chain di contenuti unificato.

Per ulteriori informazioni, vedere [Utilizzare Adobe Experience Manager con l&#39;integrazione Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

**In che modo la revisione e l&#39;approvazione unificate si adattano ad Adobe GenStudio?**

La revisione e l’approvazione unificate sono un componente fondamentale di Adobe GenStudio, la visione più ampia di Adobe per un supply chain di contenuti connesso. GenStudio collega Workfront, Frame.io, Creative Cloud, Adobe Express, Adobe Experience Manager Assets e GenStudio for Performance Marketing in un flusso di lavoro unificato, dalla descrizione della campagna alla distribuzione dei contenuti.

All’interno di tale ecosistema, la revisione e l’approvazione fungono da punto di passaggio critico tra la creazione e la consegna. È dove il lavoro creativo incontra l’input delle parti interessate, la qualità viene convalidata e il contenuto può essere pubblicato. Quando questo passaggio è veloce, visibile e affidabile, sblocca la velocità sull’intero contenuto di supply chain: l’intelligenza artificiale può accelerare la creazione, l’automazione può gestire la distribuzione, ma un collo di bottiglia nella revisione limita i vantaggi su entrambi i lati. Il collegamento di Workfront e Frame.io rimuove il collo di bottiglia.

**Che cos&#39;è la funzionalità Revisore di intelligenza artificiale?**

La revisione e l’approvazione unificate includono una funzionalità IA Reviewer che automatizza i controlli di conformità del brand come parte del processo di revisione. Il revisore AI può valutare le risorse in base alle linee guida del brand e segnalare potenziali problemi prima che i revisori umani siano coinvolti, aiutando i team a individuare i problemi prima e a muoversi più rapidamente.

Per ulteriori informazioni sull’impostazione e l’utilizzo di AI Reviewer, consulta la documentazione di Workfront su Experience League.

+++

### Contratti, SKU e storage

+++ Espandi per visualizzare le domande frequenti su contratti, SKU e storage.

**Quando saranno disponibili la revisione e l&#39;approvazione unificate?**

È ora disponibile la revisione e l’approvazione unificate. Per accedere a è necessario eseguire un aggiornamento a una SKU di Workfront V2. Se il contratto è stato firmato prima che gli SKU V2 fossero disponibili, è possibile accedervi in uno dei due modi seguenti:

* Al rinnovo: l&#39;accesso verrà abilitato alla data di rinnovo del contratto successiva.

* Riassegnazione anticipata: il team del tuo account Adobe può stipulare un nuovo contratto in anticipo per aggiungere i nuovi diritti SKU mantenendo la data di fine del contratto esistente. Il passaggio a un pacchetto equivalente non comporta alcun aumento di prezzo.

Contatta il rappresentante del tuo account Adobe per determinare il percorso migliore per la tua organizzazione.

<!--
**Before we sign the contract, what changes will we see in Workfront?**

Before signing the V2 SKU contract, your Workfront instance will continue to operate using the existing document and proofing experience. No unified review and approval features---such as the Frame.io viewer, Adobe enterprise storage, or multi-stage approval templates---will be available until the V2 SKU is contracted and Adobe Professional Services configures the integration for your organization.
-->

**L&#39;aggiornamento allo SKU V2 mi offre più spazio di archiviazione?**

Sì. Con lo SKU V2, ogni utente con licenza riceve 60 GB di storage, rispetto ai 30 GB della versione precedente.

**Come scegliere tra lo storage aziendale Adobe e lo storage Workfront legacy?**

Lo storage aziendale abilita l&#39;esperienza di visualizzazione Frame.io ed è necessario per la revisione e l&#39;approvazione unificate. Lo storage legacy continua a utilizzare il visualizzatore Workfront Proof (ProofHQ) come impostazione predefinita.

Se nell’organizzazione sono presenti diversi flussi di lavoro semplici e più complessi, puoi assegnare la priorità a quali flussi di lavoro migrare per primi.

Lo storage aziendale offre la flessibilità di implementare la nuova esperienza in modo incrementale, a partire dai flussi di lavoro che ne trarranno maggior vantaggio.

**Gestione delle licenze Frame.io**

Dopo aver firmato lo SKU V2, tutti gli utenti di Workfront avranno accesso al visualizzatore Frame.io per i flussi di lavoro di revisione e approvazione; per questo non è richiesta alcuna licenza Frame.io Enterprise separata.

Se la tua organizzazione necessita di ulteriori funzioni Frame.io Enterprise come

* Filigrana avanzata (dinamica e forense)
* Digital Rights Management con eliminazione automatica delle risorse
* Credenziali del contenuto per il contenuto generato da AI
* Metadati creativi personalizzati
* Integrazioni da fotocamera a cloud
* La tua area di lavoro per il work in progress creativo

puoi lavorare con il tuo account team Adobe per determinare il numero appropriato di licenze Enterprise Frame.io. Tutte le licenze vengono gestite tramite Adobe Admin Console.

+++

### Sandbox e rollout

+++ Espandi per visualizzare le domande frequenti per sandbox e rollout.

**Posso testare l&#39;approvazione e la revisione unificate in un ambiente sandbox?**

Parzialmente. I flussi di lavoro di approvazione possono essere testati in un ambiente sandbox Workfront. Tuttavia, l’esperienza di visualizzazione Frame.io non è disponibile in sandbox. Il test della superficie di revisione stessa richiede un ambiente di produzione.

Per limitare l’esposizione durante il rollout, puoi abilitare la revisione e l’approvazione unificate per un gruppo specifico all’interno dell’ambiente di produzione Workfront. Questo consente di eseguire un programma pilota mirato con un set più piccolo di utenti prima di implementarlo in modo più ampio.

<!--
**How should we test future quarterly releases involving unified review and approval if the Frame.io viewer is not available in sandbox?**

Because the Frame.io viewer experience is not available in the Workfront sandbox environment, testing future quarterly releases should be done using a controlled pilot group in your production environment. You can enable unified review and approval for a specific group within your Workfront production instance, allowing a smaller set of users to validate new features as they release. Approval workflow configuration and template setup can still be tested in sandbox, but the full review experience---including the Frame.io viewer---must be validated in production.
-->

+++

### Bozze interattive e HTML

+++ Espandi per visualizzare le domande frequenti su bozze interattive e HTML.

**La revisione e l&#39;approvazione unificate supportano le bozze interattive o gli URL di HTML?**

I file Zip HTML sono attualmente supportati per la revisione interattiva. Il supporto per gli URL di HTML (revisione live degli URL web) è previsto per il terzo trimestre.

Per aggiornamenti, consulta le note sulla versione di Workfront su Experience League.

+++

### Fusione e automazione

+++ Espandi per visualizzare le domande frequenti su Fusion e Automation.

**È necessario che Workfront Fusion utilizzi la revisione e l&#39;approvazione unificate?**

No. La revisione e l’approvazione unificate rappresentano un’integrazione di prodotto nativa e non richiedono Fusion. Il flusso di lavoro è integrato direttamente in Workfront.

**I connettori Fusion saranno disponibili per la revisione e l&#39;approvazione unificate?**

Sì. Le azioni di fusione per la revisione e l’approvazione unificate sono attualmente in fase di sviluppo e dovrebbero essere disponibili nel terzo trimestre. Consulta le note sulla versione di Workfront su Experience League per aggiornamenti non appena diventano disponibili.

**Fusion può essere utilizzato per attivare automaticamente una revisione quando un documento viene caricato?**

Sì. Questo tipo di automazione è possibile utilizzando i webhook di Workfront in combinazione con Fusion.

**Che impatto ha sui flussi di lavoro di Fusion esistenti basati su Workfront Proof?**

L’impatto varia a seconda di come viene creato ogni flusso di lavoro. In generale:

* **Modifica o aggiorna**: i flussi di lavoro in cui l&#39;azione esistente relativa alla bozza ha un equivalente diretto nelle approvazioni unificate possono essere aggiornati per utilizzare la nuova azione.

* **Ricostruisci**: i flussi di lavoro in cui i passaggi sottostanti sono cambiati in modo significativo o in cui sono presenti nuove funzionalità potrebbero dover essere ricompilati da zero.

Una volta disponibili le API di Fusion per le approvazioni unificate, emergerà un quadro più chiaro. Si consiglia di controllare i flussi di lavoro di Fusion esistenti e di valutarli in base alle nuove funzionalità di approvazione unificate in quel momento.

+++






