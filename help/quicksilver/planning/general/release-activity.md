---
title: Attività della versione corrente di Adobe Workfront Planning
description: Le funzionalità di Adobe Workfront Planning sono attualmente disponibili per alcuni clienti Workfront. Consulta spesso questo articolo per scoprire le funzioni rilasciate di recente per le funzionalità di pianificazione.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
source-git-commit: 2742594d4f835bb2b81b314075ab374f22074d87
workflow-type: tm+mt
source-wordcount: '6694'
ht-degree: 0%

---


# Attività della versione corrente di Adobe Workfront Planning

<!--this article is linked to the WF Planning landing page - do not change URL or move it; send the team a new URL after we add the redirects for this page-->

<!--
At GA release, replace the Important below and all the text that follows before the weekly releases with this:

(***********At GA - change the title to: Adobe Workfront Planning early access release activity during 2024*******)

Also update the metadata: 

Adobe Workfront Planning capabilities are currently available to all customers. You must purchase a Workfront Planning license, in addition to a Workfront license to be able to access these capabilities.


>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning, a new offering from Adobe Workfront. 
>
>You must purchase a Workfront Planning license, in addition to a Workfront license to be able to access and use the Workfront Planning capabilities. 
>
>For more information about Workfront Planning, see [Adobe Workfront Planning overview](/help/quicksilver/planning/general/planning-overview.md).
>-->

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono alla pianificazione di Adobe Workfront, una nuova offerta di Adobe Workfront.
>
>Attualmente, Workfront Planning si trova in una fase di accesso anticipato aperta a un numero limitato di clienti.
>
>Per utilizzare queste funzionalità è necessario essere clienti di Workfront.
>
>Il rappresentante del tuo account ti informerà se partecipi a questa fase.
>
>Per ulteriori informazioni, vedere [Panoramica di Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
>
>In alcuni casi, la documentazione a cui si fa riferimento nelle sezioni seguenti potrebbe essere disponibile dopo il rilascio delle funzioni documentate in Produzione.

<!--Not sure if we should enable this - Richard: 

## Workfront Planning release timeline

| Time               | Release                                 |
|--------------------|-----------------------------------------|
| August - December 2023               | Workfront Planning beta release         |
| January - August 2024 | Workfront Planning early release        |
| August 28, 2024    | Workfront Planning general availability |-->

Gli articoli seguenti descrivono le funzioni rilasciate durante il rilascio di Workfront Planning:

* [Gli archivi delle attività di rilascio di Adobe Workfront Planning per il 2023](/help/quicksilver/planning/general/release-activity-archives-2023.md) elencano le funzionalità rilasciate durante la versione beta, nel 2023.
* In questo articolo sono elencate le funzioni rilasciate a Workfront Planning durante il periodo di accesso anticipato nel 2024.

  Le funzioni rilasciate sono elencate in ordine di rilascio, a partire da quelle più recenti. I clienti che partecipano al programma Workfront Planning possono accedere a tutte le funzioni degli ambienti di produzione.

<!--* See the current release overview documentation for features that were released after the general availability release on August 28, 2024. 
-->

Workfront Planning è stato temporaneamente rimosso dagli ambienti Anteprima e Sandbox da gennaio 2024. Tutte le funzioni descritte in questo articolo sono attualmente disponibili in Produzione.

<!--

### Reporting capabilities for Workfront Planning with the Canvas Dashboard 

Production: August 28, 2024 

Preview: To be determined 

You can now view Workfront Planning information in a report using the Workfront Canvas Dashboard. For information, see [Get started with Canvas Dashboards](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/get-started-canvas-dashboards.md).

### Define format for formula field values

Production: <date> 

Preview: To be determined 

As a workspace manager, you can now define the format for the values displayed in a formula field. You can choose from the following formats: 

* Single-line text 
* Number 
* Percentage 
* Currency 
* Date
* Tags

For information, see the "Formula" section of the article [Create fields](/help/quicksilver/planning/fields/create-fields.md). 

-->

## Settimana del 19 agosto 2024

### Miglioramenti alla pagina principale di Workfront Planning

Produzione: 20 agosto 2024

Anteprima: da determinare

Sono stati apportati i seguenti miglioramenti alla pagina principale dell&#39;area Pianificazione:

* Per gli amministratori di sistema, le aree di lavoro che non hanno creato sono state spostate dalla scheda &quot;Altre aree di lavoro&quot; alla scheda &quot;Aree di lavoro in cui si trova&quot;. La scheda &quot;Aree di lavoro personali&quot; è stata rimossa.

* Abbiamo aggiunto un menu &quot;More&quot; (Altro) per ogni scheda dell’area di lavoro per facilitare la modifica o l’eliminazione dell’area di lavoro dalla pagina principale.

* Sono stati aggiunti i collegamenti &quot;Mostra tutto&quot; e &quot;Mostra meno&quot; per controllare il numero di aree di lavoro visualizzate nella pagina principale. Quando nella pagina principale sono elencate più di due righe di schede dell’area di lavoro, il collegamento Mostra tutto viene visualizzato per consentire la visualizzazione di tutte le aree di lavoro, solo se necessario.

Per informazioni, vedere [Modifica aree di lavoro](/help/quicksilver/planning/architecture/edit-workspaces.md).

### Collegare i tipi di record in più aree di lavoro

Produzione: 20 agosto 2024

Anteprima: da determinare

È ora possibile connettere tipi di record appartenenti a aree di lavoro diverse.

Gli amministratori di sistema ora possono configurare i tipi di record da connettere da altre aree di lavoro. In seguito, un responsabile del workspace può connettersi a questi tipi di record da un workspace designato o da tutte le aree di lavoro del sistema.

Prima di questo miglioramento, era possibile collegare solo i tipi di record appartenenti allo stesso workspace, insieme ai tipi di oggetto di altre applicazioni.

Per informazioni, vedere [Modifica tipi di record](/help/quicksilver/planning/architecture/edit-record-types.md).

### Visualizzare i record connessi nella vista timeline utilizzando la funzione Raggruppamento

Produzione: 22 agosto 2024

Anteprima: da determinare

In qualità di gestore della visualizzazione Timeline, è ora possibile visualizzare le relazioni tra i record connessi suddividendoli in gerarchie visive nella visualizzazione Timeline.

Ad esempio, quando visualizzi le campagne nella visualizzazione timeline collegate a Prodotti e i Prodotti sono associati a Progetti, ora puoi visualizzare i Prodotti in Campagne e i Progetti nei rispettivi Prodotti.

Questo consente di navigare facilmente tra più livelli di relazioni, il tutto all’interno della stessa visualizzazione timeline.

Questa non è una gerarchia effettiva (nessun oggetto è più alto di un altro). Si tratta di una gerarchia visiva che visualizza i tipi di record connessi in un&#39;unica visualizzazione timeline.

È possibile visualizzare fino a 5 livelli di tipi di record nella stessa sequenza temporale per un record.

Per informazioni, vedere [Gestire la visualizzazione della sequenza temporale](/help/quicksilver/planning/views/manage-the-timeline-view.md).

### Nuova scheda Connessioni nell&#39;area dei dettagli del record

Produzione: 22 agosto 2024

Anteprima: da determinare

È stata aggiunta una nuova scheda alle aree anteprima e pagina del record. Ora, quando si fa clic sul nome del record in una visualizzazione, l&#39;anteprima del record e la pagina del record visualizzano le seguenti schede:

* **Dettagli**: visualizza tutti i campi record, la miniatura e l&#39;immagine di copertina. È possibile modificare i campi nella scheda Dettagli.

* **Connessioni**: visualizza tutti i tipi di record o di oggetti e i relativi record o oggetti connessi. È possibile aggiungere altri record dalla scheda Connessioni.

Per informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

### Creare record, progetti e portfolio durante la connessione

Produzione: 22 agosto 2024

Anteprima: da determinare

È ora possibile creare record, progetti e portafogli quando vengono collegati a record esistenti.

Se ad esempio si connettono campagne Workfront Planning a progetti Workfront e si determina che un determinato progetto non esiste, è possibile aggiungerlo come nuovo progetto nel campo record connesso. Il progetto viene quindi aggiunto a Workfront. I nuovi record aggiunti vengono aggiunti alle rispettive pagine dei tipi di record nella visualizzazione per tabella.

In questo momento è possibile creare quanto segue durante la connessione dei record:

* Record di Workfront Planning
* Progetti Workfront senza modello
* Portfoli Workfront

Non è possibile creare altri oggetti Workfront o risorse Experience Manager connessi quando vengono collegati a un record.

Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).

## Esporta dettagli record in Word

Produzione: 22 agosto 2024

Anteprima: da determinare

È ora possibile esportare la pagina dei dettagli o l&#39;anteprima di un record in un documento di Word (.docx).

Per informazioni, vedere [Esportare i dettagli di un record](/help/quicksilver/planning/records/export-the-record-page.md).

### Aggiungi opzioni tipo di connessione

Produzione: 22 agosto 2024
Anteprima: da determinare

Ora, quando si configura una connessione tra due tipi di record, è possibile definire se gli utenti possono connettere uno o più record in ciascuno dei tipi di record della connessione. In questo modo puoi progettare in modo affidabile i flussi di lavoro del team e assicurarti che gli utenti selezionino solo le informazioni previste in base ai loro processi.

Quando si collegano due tipi di record, è ora possibile scegliere tra i seguenti tipi di connessione:

* Molti a molti. Quando si seleziona questo tipo di connessione, non è possibile modificarlo dopo averlo salvato.
* Da uno a molti
* Da uno a uno
* Molti a uno.

Questo consente di definire il numero di record dei tipi di record connessi che gli utenti possono connettere quando viene stabilita una connessione.

I nuovi tipi di connessione non sono supportati per le seguenti connessioni dei tipi di record:

* Quando si collegano tipi di record a risorse Experience Manager
* Quando si connettono tipi di record che non appartengono alla stessa area di lavoro

Per informazioni, vedere [Panoramica sui tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Settimana del 12 agosto 2024

### L&#39;Assistente IA è stato temporaneamente rimosso

Produzione: 12 agosto 2024
Anteprima: da determinare

L&#39;Assistente di Workfront AI è stato temporaneamente rimosso e sarà disponibile in un secondo momento. Per ulteriori informazioni sull&#39;Assistente di IA, vedere [Panoramica dell&#39;Assistente di Adobe Workfront Planning AI](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

### Mantenere l’ultimo intervallo di tempo visualizzato nella vista timeline

Produzione: 14 agosto 2024

Anteprima: da determinare

Ora, quando si apre una visualizzazione timeline e si scorre fino a una data nel passato o nel futuro, la data selezionata viene mantenuta dopo l’aggiornamento della pagina. Prima di questo miglioramento, la pagina mostrava la data odierna.

Per informazioni, vedere [Gestire la visualizzazione della sequenza temporale](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Settimana del 29 luglio 2024

### L’API pubblica di Adobe Workfront Planning è ora disponibile

Produzione: 30 luglio 2024

Anteprima: da determinare

È ora disponibile l’API pubblica di Adobe Workfront Planning.

Per informazioni, vedere [Nozioni di base sulle API di Adobe Workfront Planning](/help/quicksilver/planning/general/planning-api-basics.md).

### Inserire e duplicare i record nella vista tabella

Produzione: 1 agosto 2024
Anteprima: da determinare

Sono state introdotte le seguenti funzionalità per l’utilizzo dei record nella vista a tabella:

* Record duplicati: puoi creare rapidamente un record duplicandone uno esistente.  Viene creato un record identico. Questa funzionalità è disponibile solo nella vista tabella.

* È possibile inserire un nuovo record sopra o sotto un record esistente nella vista tabella. Prima di questo miglioramento, è possibile aggiungere record solo nella parte inferiore della visualizzazione tabella.

Puoi eseguire le nuove funzionalità dalle seguenti aree:

* Menu Altro di un record

* La nuova barra degli strumenti che è stata aggiunta nella parte inferiore della pagina del record nella visualizzazione tabella

Per informazioni, vedere [Crea record](/help/quicksilver/planning/records/create-records.md)

### Condividere le visualizzazioni di Workfront Planning pubblicamente

Produzione: 2 agosto 2024

Anteprima: da determinare

Per lavorare senza problemi con le parti interessate esterne, ora puoi condividere le visualizzazioni dei record con altre persone esterne all’organizzazione. Puoi condividere un collegamento pubblico alla visualizzazione a cui desideri che altri utenti abbiano accesso.

Questo aggiornamento include le seguenti funzionalità:

* Condividere la visualizzazione di una pagina di tipo record con un collegamento pubblico che scadrebbe in una data specifica.

* Il collegamento condiviso è accessibile da chiunque non faccia parte della società per un periodo di tempo limitato, indicato dalla data di scadenza. Non è necessario effettuare l&#39;accesso per visualizzare la visualizzazione condivisa.

* Gli utenti che accedono alla visualizzazione dal collegamento pubblico non possono creare altre visualizzazioni, modificare la visualizzazione condivisa, aggiungere, eliminare o modificare informazioni sui record.

Per ulteriori informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).

## Settimana dell’8 luglio 2024

### Apri oggetto connesso direttamente in Workfront

Produzione: 9 luglio 2024

Anteprima: da determinare

È stato eliminato un passaggio per accedere agli oggetti Workfront connessi ai record di Workfront Planning.

Ora, quando si fa clic sul nome di un oggetto Workfront dal record Planning a esso collegato, viene aperta la pagina dell&#39;oggetto Workfront. Prima di questo miglioramento, veniva aperta una pagina Workfront Planning di sola lettura per l&#39;oggetto Workfront connesso, da cui era possibile passare alla pagina oggetto di Workfront.

Per informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

### Solo gli utenti con licenza Standard o Plan possono creare visualizzazioni

Produzione: 11 luglio 2024

Anteprima: da determinare

Sono stati modificati i tipi di utenti che possono creare visualizzazioni. Ora solo gli utenti con licenza Standard o Plan possono creare visualizzazioni. Tutti gli altri utenti hanno accesso in sola visualizzazione alle visualizzazioni condivise con loro. Prima di questo aggiornamento, gli utenti con licenza Light e Worker potevano creare visualizzazioni.

Per ulteriori informazioni, vedere [Panoramica del tipo di licenza quando si utilizza Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).

### Ordinare e raggruppare i record in base ai campi di ricerca con più valori

Produzione: 11 luglio 2024

Anteprima: da determinare

È ora possibile ordinare e raggruppare i record in qualsiasi visualizzazione utilizzando campi di ricerca con più valori che non vengono riepilogati. Prima di questo miglioramento, era possibile ordinare e raggruppare solo i campi di ricerca riepilogati.

Se il campo di ricerca contiene più valori, considera quanto segue:

* L’ordinamento viene eseguito dal primo valore

* I record sono raggruppati per ogni combinazione univoca di valori di campo

* La timeline viene creata in base al primo valore di data.

Per ulteriori informazioni, consulta i seguenti articoli:

* [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md)
* [Gestisci la vista tabella](/help/quicksilver/planning/views/manage-the-table-view.md).


## Settimana del 24 giugno 2024

### Workfront AI Assistant (beta) ora disponibile per Workfront Planning

L&#39;Assistente AI (beta) è ora disponibile per Workfront Planning.

L’assistente AI funziona nel contesto della pagina selezionata e con il tuo livello di accesso e autorizzazioni per eseguire le seguenti azioni: generare, aggiornare, rimuovere o ripristinare i record.

L’Assistente AI è attualmente in fase beta ed è disponibile per alcuni clienti. Contatta il rappresentante del tuo account per sapere se sei idoneo a partecipare a questa fase.

Per informazioni, vedere [Panoramica dell&#39;Assistente di Adobe Workfront Planning AI](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

### Nuova casella di ricerca quando si seleziona un&#39;area di lavoro o un tipo di record

Produzione: 27 giugno 2024

Anteprima: da determinare

Per facilitare la navigazione tra aree di lavoro o tra tipi di record, ora puoi cercare un’area di lavoro o un tipo di record nel menu a discesa a destra del loro nome nell’intestazione della pagina.

Per informazioni, vedere [Modifica tipi di record](/help/quicksilver/planning/architecture/edit-record-types.md).

### Inserisce un nuovo campo a destra o a sinistra di un campo esistente nella vista tabella

Produzione: 27 giugno 2024

Anteprima: da determinare

Per migliorare e velocizzare l’esperienza nella vista della tabella di record, è stata aggiunta la possibilità di aggiungere un nuovo campo tra due colonne, inserendolo a destra o a sinistra di uno esistente.

Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

## Settimana del 17 giugno 2024

### Aspetto aggiornato della pagina Dettagli

Produzione: 17 giugno 2024

Anteprima: da determinare

Abbiamo aggiornato l’aspetto della pagina Dettagli dei record. Come parte di questo aggiornamento, le icone dei campi sono state rimosse.

Per informazioni, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

### Modelli Workspace aggiornati

Produzione: 17 giugno 2024

Anteprima: da determinare

Sono stati aggiornati l&#39;aspetto e il campo delle schede dei modelli dell&#39;area di lavoro in Workfront Planning.

Questo aggiornamento include i seguenti miglioramenti:

* I tipi di record appartenenti a ciascun modello vengono visualizzati come schede.

* Il modello Gestione marketing è stato rimosso. Abbiamo aggiunto i seguenti modelli per la gestione del marketing e consigliamo di utilizzarne uno appropriato a seconda della complessità dei flussi di lavoro:

   * Base: Marketing Management
   * Avanzato: Marketing Management
   * Enterprise: Marketing Management

Per informazioni, vedere i seguenti articoli:

* [Elenco dei modelli dell&#39;area di lavoro](/help/quicksilver/planning/architecture/workspace-templates.md)

* [Crea aree di lavoro](/help/quicksilver/planning/architecture/create-workspaces.md)

### Nuova esperienza durante l’aggiunta di una miniatura o di una copertina a un record

Produzione: 17 giugno 2024

Anteprima: da determinare

È stata aggiornata l’esperienza per aggiungere una miniatura o un’immagine di copertina a un record dalla pagina Dettagli. I miglioramenti includono i seguenti aggiornamenti:

* Le miniature e le immagini di copertina vengono automaticamente assegnate a un record quando lo si crea. In seguito sarà possibile modificare queste immagini.

* È possibile aggiungere una miniatura dalla pagina Dettagli. Prima di questo miglioramento, era possibile aggiungere una miniatura solo dalla vista tabella.

* È possibile sfogliare una raccolta di immagini per selezionare un&#39;immagine per la copertina o la miniatura di un record. Prima di questo miglioramento, era possibile caricare solo il proprio file di immagine.

Per ulteriori informazioni, consulta i seguenti articoli:

* [Aggiungere un&#39;immagine di copertina a un record](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)

* [Aggiungere una miniatura a un record](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

### Aggiornare il titolo del record nella pagina Dettagli

Produzione: 17 giugno 2024

Anteprima: da determinare

Il titolo della pagina Dettagli di un record visualizza il campo principale di un record. Prima di questo aggiornamento, nel titolo della pagina Dettagli di un record veniva visualizzato il nome del record. È possibile modificare il titolo in linea nella pagina Dettagli, a meno che il campo principale non sia di tipo formula.

Per ulteriori informazioni, consulta i seguenti articoli:

* [Gestisci la vista tabella](/help/quicksilver/planning/views/manage-the-table-view.md)

* [Modifica record](/help/quicksilver/planning/records/edit-records.md)

### Aggiunta di un collegamento &quot;Mostra altro/Mostra meno&quot; nei campi del record connessi

Produzione: 17 giugno 2024

Anteprima: da determinare

È stato aggiunto il collegamento &quot;Mostra altro/Mostra meno&quot; in un campo record collegato, quando sono presenti record che altrimenti verrebbero visualizzati su più di due righe nella pagina Dettagli di un record.

Per informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

### Compilare automaticamente il campo Nome con il nome del record, durante la connessione dei tipi di record

Produzione: 20 giugno 2024

Anteprima: da determinare

Quando si crea una connessione tra due record o tra un record e un oggetto da un&#39;altra applicazione, il campo Nome connessione viene compilato automaticamente con il nome del record connesso. Prima di questo miglioramento, era necessario aggiungere manualmente un Nome per il campo di connessione.

Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).

### Definire la modalità di visualizzazione dei record connessi nei campi connessi

Produzione: 20 giugno 2024

Anteprima: da determinare

È ora possibile decidere la modalità di visualizzazione dei record connessi nei campi connessi. Durante l&#39;aggiunta di una nuova connessione a un tipo di record, è ora possibile visualizzare il titolo del record collegato e la relativa miniatura oppure solo la miniatura.

Il titolo di un record è il nome del record o qualsiasi campo impostato come campo principale nella visualizzazione tabella del tipo di record.

Questo miglioramento è disponibile per i record connessi da Workfront Planning e per le risorse collegate da Adobe Experience Manager.

Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).

### Solo gli utenti con licenza Standard o Plan possono disporre delle autorizzazioni Manage per le aree di lavoro (titolo)

Produzione: 21 giugno 2024

Anteprima: da determinare

Sono stati modificati i tipi di utenti che possono avere accesso completo alle aree di lavoro. Ora solo gli utenti con licenza Standard o Plan possono disporre delle autorizzazioni Manage per le aree di lavoro. L&#39;accesso ai tipi di record, ai record e ai campi viene ereditato da un&#39;area di lavoro. Tutti gli altri utenti hanno accesso in sola visualizzazione alle aree di lavoro e ai relativi tipi di oggetto. Prima di questo aggiornamento, gli utenti con licenza Light e Worker potevano ricevere le autorizzazioni Contribute per le aree di lavoro.

Per ulteriori informazioni, vedere [Panoramica del tipo di licenza quando si utilizza Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).

## Settimana del 10 giugno 2024

### Riferimento fino a 4 livelli per i campi di ricerca dei record

Produzione: 12 giugno 2024

Anteprima: da determinare

È ora possibile fare riferimento a campi che si trovano fino a 4 livelli di distanza dal record quando si crea uno dei seguenti elementi:

* Filtro

* Ordina

* Raggruppamento

* Campo formula

Per ulteriori informazioni, consulta i seguenti articoli:

* [Crea campi](/help/quicksilver/planning/fields/create-fields.md)

* [Gestisci la vista tabella](/help/quicksilver/planning/views/manage-the-table-view.md)

## Settimana del 3 giugno 2024

### Nuova pagina di destinazione per Workfront Planning

Produzione: 7 giugno 2024

Anteprima: da determinare

Verrà visualizzata una nuova pagina di destinazione per Workfront Planning, dopo aver fatto clic su Pianificazione nel menu principale.

Alcune delle informazioni sulla pagina di destinazione includono:

* Area in cui vengono visualizzate le aree di lavoro e le aree di lavoro condivise con l&#39;utente. Il proprietario dell’area di lavoro viene visualizzato su ogni scheda dell’area di lavoro.

* Se sei un amministratore di Workfront, vengono visualizzate le seguenti schede:

   * Aree di lavoro personali: visualizza solo le aree di lavoro create.

   * Altre aree di lavoro: visualizza le aree di lavoro create o condivise con l&#39;utente.

* Collegamenti alla documentazione e all&#39;attività di rilascio per Workfront Planning

* Tutorial introduttivo per Workfront Planning

Per ulteriori informazioni, vedere [Panoramica di Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

### Nuova esperienza di onboarding per Workfront Planning

Produzione: 7 giugno 2024

Anteprima: da determinare

Quando i nuovi utenti accedono a Workfront Planning per la prima volta, sono ora ben accolti da un tutorial di onboarding che li guida attraverso attività semplici e definendo i concetti principali della soluzione.

Puoi seguire il processo di onboarding, completare le attività o ridurlo a icona e rivederlo in un secondo momento.

## Settimana del 27 maggio 2024

### Introduzione dell’operatore di rollup UNIQUE per i campi di ricerca

Produzione: 27 maggio 2024

Anteprima: da determinare

È stato aggiunto l’operatore UNIQUE durante l’aggregazione dei valori dei campi di ricerca.

L’operatore UNIQUE rimuove i duplicati dai valori dei campi di ricerca e mostra solo un valore univoco. Se ad esempio si aggiungono più record connessi e i valori di un campo di ricerca sono identici tra più record, Workfront visualizza solo uno dei valori nel campo di ricerca del record originale.

L’operatore UNIQUE è disponibile per tutti i tipi di campo, ad eccezione dei seguenti:

* Paragrafo
* Persone
* Campo casella di controllo

Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).

### Per impostazione predefinita, condividi le viste con tutti i membri di un’area di lavoro

Produzione: 30 maggio 2024

Anteprima: da determinare

È stata introdotta un&#39;opzione che consente di assegnare rapidamente le autorizzazioni di visualizzazione a tutti i membri di un&#39;area di lavoro. Prima di questo miglioramento, solo gli utenti con cui hai condiviso specificamente una visualizzazione potevano accedere alla visualizzazione. Questa opzione non è attivata per impostazione predefinita.

Per informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).

### Aggiornamento dell&#39;aspetto dell&#39;icona Planning nel menu principale

Produzione: 30 maggio 2024

Anteprima: da determinare

È stato aggiornato l’aspetto dell’icona per l’area Pianificazione nel menu principale. Per informazioni, vedere [Panoramica di Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

### Ridenominazione del programma Workfront Planning

A partire dal 30 maggio 2024, il programma Adobe Workfront Planning sta passando dalla fase beta a una fase di accesso anticipato. Stai per vedere questo cambiamento nella terminologia della nostra documentazione.

La fase di accesso anticipato è inoltre limitata ad alcuni clienti Workfront.

Il rappresentante del tuo account ti informerà se hai i requisiti per partecipare alla fase di accesso anticipato.

### Nuovo processo per eliminare un’area di lavoro

Produzione: 30 maggio 2024

Anteprima: da determinare

Poiché l’impatto dell’eliminazione di un’area di lavoro può essere significativo, stiamo aggiungendo un ulteriore passaggio per confermare l’eliminazione. Ora gli utenti devono digitare &quot;delete&quot; (elimina) prima di poter completare l’eliminazione definitiva di un’area di lavoro.

Le aree di lavoro eliminate e le relative informazioni non possono essere recuperate.

Per ulteriori informazioni, vedere [Elimina aree di lavoro](/help/quicksilver/planning/architecture/delete-workspaces.md).

### I campi della data di ricerca sono ora disponibili nella vista Timeline

Produzione: 31 maggio 2024

Anteprima: da determinare

È ora possibile impostare le date di inizio e di fine della visualizzazione timeline su un campo di ricerca da un record o un tipo di oggetto connesso.

Per ulteriori informazioni sulla creazione delle visualizzazioni, vedere [Gestire le visualizzazioni dei record](/help/quicksilver/planning/views/manage-record-views.md).

## Settimana del 20 maggio 2024

### Collegare i record di Workfront Planning dagli oggetti di Workfront utilizzando la sezione Planning

Produzione: 23 maggio 2024

Anteprima: da determinare

Nel pannello a sinistra di progetti, portfolio e programmi Workfront è stata aggiunta una nuova sezione Planning. Nella nuova sezione Planning vengono visualizzati i record di Workfront Planning connessi all&#39;oggetto Workfront.

Nella sezione Pianificazione di Workfront sono disponibili le azioni seguenti:

* Visualizza record di Planning connessi

* Collegare i record di Workfront Planning all&#39;oggetto Workfront

* Disconnetti record

* Aprire la casella o la pagina di anteprima dei dettagli per visualizzare ulteriori informazioni sui record connessi

Per informazioni, vedere [Gestire i record nella sezione Pianificazione degli oggetti Adobe Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

## Settimana del 13 maggio 2024

### Aggiornamenti in tempo reale nella vista timeline dopo la modifica dei record

Produzione: 14 maggio 2024

Anteprima: da determinare.

Quando un utente aggiorna le informazioni di un record, gli altri utenti possono visualizzare le informazioni aggiornate nella visualizzazione della sequenza temporale del record in tempo reale. In questo modo tutti gli utenti visualizzano le informazioni aggiornate contemporaneamente, in sincronia con il momento in cui si verificano le modifiche.

### Aggiungi record dall’intestazione della vista

Produzione: 14 maggio 2024

Anteprima: da determinare

È stato aggiunto il pulsante &quot;Nuovo record&quot; nell’intestazione di una pagina del tipo di record. È ora possibile creare record da qualsiasi visualizzazione. Prima di questo miglioramento, era possibile creare record solo dalla vista tabella.

Per ulteriori informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).


### Nuovo avviso sulla visibilità degli oggetti durante la connessione dei record

Produzione: 15 maggio 2024

Anteprima: da determinare

Quando si creano connessioni a tipi di oggetto esterni a Workfront Planning, viene visualizzato un messaggio che informa che tutti gli utenti che lavorano nell&#39;area di lavoro corrente avranno visibilità su tutti gli oggetti collegati e sui relativi campi di ricerca, indipendentemente dalle autorizzazioni e dai livelli di accesso nell&#39;altra applicazione.

Se ad esempio si collegano progetti da campagne Workfront Planning, tutti gli utenti con accesso a Visualizza campagna avranno accesso anche alla visualizzazione dei progetti collegati e delle informazioni dai campi di ricerca, anche se non dispongono di autorizzazioni per i progetti collegati o di accesso ai progetti in generale. Quando si ricevono le autorizzazioni per le aree di lavoro, è possibile accedere ai record di Planning.

Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).

### Aggiungere sezioni alle pagine di anteprima e dettagli del record

Produzione: 15 maggio 2024

Anteprima: da determinare

Per una migliore organizzazione delle informazioni sulla pagina del record, per una migliore leggibilità e navigazione, sono state introdotte sezioni nella pagina del record. I titoli delle sezioni fungono da intestazioni che organizzano i campi in categorie distinte. Le sezioni sono completamente personalizzabili e, se necessario, possono essere espanse o compresse.

Per informazioni, vedere [Gestire il layout della pagina record](/help/quicksilver/planning/records/manage-the-record-page.md).

### Aggiornamenti in tempo reale per le modifiche alla configurazione dei campi

Produzione: 16 maggio 2024

Anteprima: da determinare

Quando un utente modifica una configurazione di campo (nome, descrizione, elenco di opzioni e così via) in un tipo di record, gli altri utenti visualizzano tali modifiche in tempo reale. In questo modo, tutti possono visualizzare i campi corretti e le relative informazioni contemporaneamente.

>[!WARNING]
>
>Quando si modificano le espressioni della formula o si aggiungono o si rimuovono opzioni da un campo di tipo selezionato, si verifica una perdita di dati per i record che contengono già informazioni memorizzate nei campi la cui configurazione viene modificata.
>
>Non viene visualizzato alcun avviso o indicazione che possa verificarsi questa perdita di dati quando si modifica la configurazione dei campi.
>
>Non viene inviata alcuna notifica agli altri utenti circa la modifica della configurazione del campo.

Per ulteriori informazioni, vedere [Modifica impostazioni campo](/help/quicksilver/planning/fields/edit-fields.md).

## Settimana del 6 maggio 2024

### Aspetto aggiornato delle schede del tipo di record in un’area di lavoro

Produzione: 7 maggio 2024

Anteprima: da determinare

È stato aggiornato l’aspetto delle schede del tipo di record quando vengono visualizzate in un’area di lavoro. Gli aggiornamenti includono:

* Rimozione del numero di campi e connessioni per ogni tipo di record

* Aggiunta della descrizione del tipo di record

Per informazioni, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

### Abilita le notifiche di Workfront Planning per i clienti di Adobe Unified Experience

Produzione: 8 maggio 2024

Anteprima: da determinare

Se sei un cliente di Adobe di Unified Experience e qualcuno ti aggiunge a un commento nella pagina di registrazione, riceverai una notifica in-app e un’e-mail relativa al commento. Puoi gestire le preferenze per le notifiche nell’area Preferenze del tuo profilo Adobe Experience Cloud. Per ulteriori informazioni, vedere [Preferenze account e notifiche](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

Per ulteriori informazioni sulle notifiche di Workfront Planning, vedere [Notifiche di Adobe Workfront Planning: indice articolo](/help/quicksilver/planning/notifications/notifications-information.md).


## Settimana del 29 aprile 2029

### Aggiornamenti in tempo reale nella casella e nella pagina dei dettagli dei record dopo la modifica dei record nella vista Tabella

Produzione: 2 maggio 2024

Anteprima: da determinare

Quando un utente aggiorna le informazioni di un record nella vista a tabella, gli altri utenti possono visualizzare le informazioni aggiornate nella casella dei dettagli del record (all’interno di una vista) o nella pagina in tempo reale. In questo modo tutti gli utenti visualizzano le informazioni aggiornate contemporaneamente, in sincronia con il momento in cui si verificano le modifiche.

Per informazioni sulla modifica dei record, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

### Aggiornamenti in tempo reale nella vista calendario dopo la modifica dei record

Produzione: 3 maggio 2024

Anteprima: da determinare.

Quando un utente aggiorna le informazioni di un record, gli altri utenti possono visualizzare le informazioni aggiornate nella visualizzazione calendario del record in tempo reale. In questo modo tutti gli utenti visualizzano le informazioni aggiornate contemporaneamente, in sincronia con il momento in cui si verificano le modifiche.

## Settimana del 22 aprile 2024

### Flusso di lavoro aggiornato durante la modifica di un’area di lavoro o di un tipo di record

Produzione: 23 aprile 2024

Anteprima: da determinare

È stato aggiornato l’aspetto delle caselle Modifica area di lavoro e Modifica tipo di record.

Quando modifichi un’area di lavoro o un tipo di record, ora puoi definire un nome, una descrizione e assegnare loro un colore e un’icona.

Per ulteriori informazioni, consulta i seguenti articoli:

* [Modifica aree di lavoro](/help/quicksilver/planning/architecture/edit-workspaces.md)

* [Modifica tipi di record](/help/quicksilver/planning/architecture/edit-record-types.md).

## Settimana dell’8 aprile 2024

### Copiare il contenuto di una cella e incollarlo in più celle selezionate

Produzione: 10 aprile 2024

Anteprima: da determinare

È ora possibile copiare il contenuto di una cella nella vista tabella e incollarlo in più celle selezionate. È inoltre possibile copiare informazioni da origini esterne e incollarle nelle celle della vista tabella.

Questa funzionalità è supportata per tutti i tipi di campo, ad eccezione dei campi calcolati.

Per ulteriori informazioni, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

## Settimana del 1° aprile 2024

### Riordinare i campi nelle pagine record

Produzione: 4 aprile 2024

Anteprima: da determinare

In qualità di manager di Workspace, ora puoi riordinare i campi elencati nella pagina di record o nell’anteprima. L&#39;aggiornamento dell&#39;ordine dei campi modifica l&#39;ordine dei campi di tutti i record dello stesso tipo, per tutti gli utenti che visualizzano la pagina record o l&#39;anteprima record.

Per ulteriori informazioni, vedere [Gestire il layout della pagina record](/help/quicksilver/planning/records/manage-the-record-page.md).


### Aggiungi immagine di copertina per registrare le pagine

Produzione: 4 aprile 2024

Anteprima: da determinare

Durante la gestione delle pagine di record, è ora possibile aggiungere, riposizionare e sostituire un&#39;immagine di copertina in una pagina di record o in anteprima, per arricchire la presentazione del record e il coinvolgimento delle parti interessate. Le immagini di copertina sono visibili a tutti gli utenti che visualizzano i record.

Per ulteriori informazioni, vedere [Gestire il layout della pagina record](/help/quicksilver/planning/records/manage-the-record-page.md).

## Settimana del 25 marzo 2024

### Nuova organizzazione di tipo record flessibile per le aree di lavoro

Produzione: 25 marzo 2024

Anteprima: da determinare

Per rendere più efficiente l&#39;impostazione delle aree di lavoro, è stata modificata la modalità di organizzazione dei tipi di record in un&#39;area di lavoro. Alcuni dei miglioramenti includono:

* Crea fino a 50 sezioni di tipi di record in ogni area di lavoro. Le sezioni dei tipi di record operativi e delle tassonomie esistenti rimangono nelle aree di lavoro esistenti.

* Personalizza completamente tutte le nuove aree di lavoro e le relative nuove sezioni per riflettere i processi e le esigenze dell’organizzazione.

* Spostare dinamicamente i tipi di record all’interno di un’area di lavoro trascinandoli nella posizione desiderata, anche in sezioni diverse.

Per ulteriori informazioni, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

### Visualizzazioni duplicate

Produzione: 25 marzo 2024

Anteprima: da determinare

Per risparmiare tempo e mantenere la coerenza, ora puoi duplicare una vista esistente a cui hai autorizzazioni di accesso.

La duplicazione di una vista crea una vista identica, utilizzando gli stessi filtri, criteri di ordinamento e raggruppamenti. La duplicazione di una vista non mantiene le autorizzazioni della vista originale.

Per ulteriori informazioni, vedere [Gestire le visualizzazioni dei record](/help/quicksilver/planning/views/manage-record-views.md).

### Rinominata area Maestro nel menu principale come Planning

Produzione: 27 marzo 2024

Anteprima: da determinare

Abbiamo rinominato l’area Maestro nel Main Menu in Planning.

Per una panoramica di Adobe Workfront Planning, vedere [Panoramica di Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

### Nuova esperienza durante l’eliminazione di un tipo di record

Produzione: 27 marzo 2024

Anteprima: da determinare

La casella di conferma durante l’eliminazione di un tipo di record è stata riprogettata. L&#39;eliminazione di un tipo di record ha un impatto notevole, in quanto elimina anche tutti i record, i relativi campi, le informazioni contenute nei campi e le visualizzazioni associate al tipo di record. Non è possibile recuperare i tipi di record eliminati e le relative informazioni eliminate.

Per questo motivo, volevamo garantire che l’intento dell’utente fosse accurato durante l’eliminazione di un tipo di record, per cui abbiamo introdotto un passaggio aggiuntivo nella conferma dell’eliminazione. Per ulteriori informazioni, vedere [Elimina tipi di record](/help/quicksilver/planning/architecture/delete-record-types.md).

## Settimana del 18 marzo 2024

### Filtri disponibili nella vista calendario

Produzione: 19 marzo 2024

Anteprima: da determinare

È ora possibile filtrare le informazioni nella vista calendario. Per ulteriori informazioni, vedere [Gestire la visualizzazione del calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md).

### Anteprima con i dettagli dei record aggiunti alla timeline e alle visualizzazioni del calendario

Produzione: 19 marzo 2024

Anteprima: da determinare

È ora possibile accedere all’anteprima con i dettagli dei record dalle viste timeline e calendario. È possibile modificare i record nella casella di anteprima del record all&#39;interno delle visualizzazioni Timeline e Calendario.

Dall&#39;anteprima del record è possibile aprire la pagina di registrazione in una nuova scheda del browser.

Per ulteriori informazioni, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

### Il tipo di record Importazione di Excel è stato temporaneamente rimosso

Produzione: 21 marzo 2024

Anteprima: da determinare

È in corso la rimozione temporanea dei tipi di record importati utilizzando un file Excel o CSV. Questa funzionalità sarà disponibile in un secondo momento.

## Settimana dell’11 marzo 2024

### Panoramica dei dettagli dei record nella vista a tabella

Produzione: 14 marzo 2024

Anteprima: da determinare

Per semplificare la visualizzazione di informazioni aggiuntive sui record quando si utilizza la vista a tabella, è stata introdotta una nuova anteprima Dettagli che consente di visualizzare rapidamente i dettagli del record. Di seguito sono riportate alcune delle informazioni incluse nell&#39;anteprima del record:

* Panoramica dei dettagli dei record rilevanti

* Possibilità di modificare le informazioni del record

* Un collegamento per aprire la pagina del record

Per ulteriori informazioni, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

### Nuova struttura a schede per le visualizzazioni record

Produzione: 14 marzo 2024

Anteprima: da determinare

Per migliorare la navigazione e la facilità d’uso, abbiamo riprogettato la visualizzazione delle visualizzazioni di record. Ora le visualizzazioni vengono visualizzate orizzontalmente, come schede nella pagina del tipo di record, in modo da potervi navigare facilmente. Prima di questo miglioramento, le viste venivano visualizzate nel menu a discesa Vista.

Le visualizzazioni vengono visualizzate in ordine cronologico per data aggiunta, da sinistra a destra. Anche le viste condivise vengono visualizzate in ordine cronologico in base al momento in cui sono state condivise.

Per ulteriori informazioni, vedere [Gestire le visualizzazioni dei record](/help/quicksilver/planning/views/manage-record-views.md).

### Progettazione dinamica di una visualizzazione record

Produzione: 14 marzo 2024
Anteprima: da determinare

Nella pagina del tipo di record è stato aggiornato l’aspetto delle visualizzazioni. Le nuove viste rispondono dinamicamente e si adattano rapidamente alle dimensioni dello schermo. Le etichette delle opzioni della barra degli strumenti sono nascoste su schermi più piccoli per facilitarne l’utilizzo.

Per ulteriori informazioni, consulta i seguenti articoli:

* [Gestire la vista tabella](/help/quicksilver/planning/views/manage-the-table-view.md)
* [Gestione della visualizzazione della sequenza temporale](/help/quicksilver/planning/views/manage-the-timeline-view.md).

### Consenti agli amministratori di sistema di gestire tutte le visualizzazioni condivise

Produzione: 14 marzo 2024

Anteprima: da determinare

Per essere coerente con tutte le altre aree del sistema e per essere in grado di gestire e controllare qualsiasi visualizzazione disponibile come amministratore di sistema, ora si dispone delle autorizzazioni di gestione per qualsiasi visualizzazione condivisa con te nella pagina del tipo di record. Prima di questo miglioramento, gli autori delle visualizzazioni potevano concedere le autorizzazioni per visualizzare o gestire la visualizzazione. Ora, se la vista è condivisa con l’utente e l’utente è amministratore di sistema, per impostazione predefinita disporrà delle autorizzazioni di gestione per la vista.

Per ulteriori informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).

### Pagina non autorizzata quando si condivide una visualizzazione senza autorizzazioni

Produzione: 14 marzo 2024

Anteprima: da determinare

Quando un utente riceve un collegamento a un tipo di record e ha accesso all’area di lavoro ma non alla vista condivisa nel collegamento, viene visualizzata una pagina che notifica che non è autorizzato a visualizzare il tipo di record.

Per ulteriori informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).


### Nuova etichetta per gli amministratori di sistema nelle finestre di dialogo di condivisione

Produzione: 14 marzo 2024

Anteprima: da determinare

Nella finestra di dialogo di condivisione, accanto al nome dell’amministratore di sistema viene ora visualizzata l’etichetta &quot;Amministratore&quot; quando si condivide una visualizzazione o un’area di lavoro.

Per informazioni, vedere [Panoramica delle autorizzazioni di condivisione](/help/quicksilver/planning/access/sharing-permissions-overview.md).

### Pagina non autorizzata quando si condivide una visualizzazione senza autorizzazioni

Produzione: 14 marzo 2024

Anteprima: da determinare

Quando un utente riceve un collegamento a un tipo di record e ha accesso all’area di lavoro ma non alla vista condivisa nel collegamento, viene visualizzata una pagina che notifica che non è autorizzato a visualizzare il tipo di record.

Oltre a condividere le aree di lavoro, è necessario condividere le visualizzazioni per consentire ad altri utenti di accedere alla stessa pagina del tipo di record condivisa con un collegamento.

Per ulteriori informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).

## Settimana del 4 marzo 2024

### Modificare l&#39;altezza delle righe nella vista tabella

Produzione: 7 marzo 2024

Anteprima: da determinare

È ora disponibile un&#39;opzione per modificare l&#39;altezza di una riga durante la visualizzazione dei record nella vista tabella.

È possibile aggiornare l&#39;altezza della riga a una delle seguenti dimensioni:

* Piccolo
* Medio
* Alto.

Per ulteriori informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

### Nuova vista calendario per i record

Produzione: 7 marzo 2024

Anteprima: da determinare

È ora possibile visualizzare i record in una vista calendario. Per creare la visualizzazione calendario è necessario disporre di almeno due campi data in un tipo di record.

Per ulteriori informazioni, vedere [Gestire la visualizzazione del calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md).

## Settimana del 26 febbraio 2024

### Filtra, ordina e raggruppa per record o campi di ricerca connessi

Produzione: 28 febbraio 2024

Anteprima: da determinare

È ora possibile filtrare, ordinare e raggruppare in base ai record connessi o ai relativi campi di ricerca. Questo miglioramento consente di organizzare e visualizzare in modo efficiente i dati sia nelle viste tabella che nella timeline.

Non è possibile filtrare, ordinare o raggruppare per campi di ricerca che consentono connessioni con più record.

Per informazioni, vedere [Gestire la vista tabella](/help/quicksilver/planning/views/manage-the-table-view.md) e [Gestire la vista timeline](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Settimana del 5 febbraio 2024

### Modificare le autorizzazioni in base ai tipi di licenza

Produzione: 6 febbraio 2024

Anteprima: da determinare

Sono stati modificati i livelli di autorizzazione per tenere conto dei tipi di licenza degli utenti. Prima di questo miglioramento, non vi erano differenze nelle autorizzazioni dell’area di lavoro in base ai tipi di licenza degli utenti.

Di seguito sono riportati i livelli più elevati di autorizzazioni che gli utenti possono ricevere in base al tipo di licenza dell&#39;utente:

* Gli utenti con una licenza Pianificazione (o Standard, nel nuovo modello di licenza) possono creare e gestire aree di lavoro, tipi di record e record.

* Gli utenti con una licenza Lavoro (o Light, nel nuovo modello di licenza) possono visualizzare e contribuire a un’area di lavoro condivisa con loro, nonché i tipi di record e i record di tale area di lavoro.  Gli utenti con licenza Lavoro (o Light) possono inoltre creare, modificare ed eliminare record nelle aree di lavoro in cui dispongono dell’accesso a Contribute.

* Gli utenti con una licenza Revisione o Richiedente (o Collaboratore, nel nuovo modello di licenza) possono visualizzare solo le aree di lavoro condivise con loro, nonché i tipi di record e i record di tali aree di lavoro. Non possono creare, modificare o eliminare tipi di record o record.

Per informazioni sul nuovo modello di licenza, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Per informazioni sulla connessione tra il tipo di licenza e le autorizzazioni nelle funzionalità di pianificazione, vedere [Panoramica sul tipo di licenza quando si utilizza Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Nuovo aspetto della barra degli strumenti Testo formattato per i campi record

Produzione: 7 febbraio 2024

Anteprima: da determinare

È stato aggiornato l’aspetto della barra degli strumenti Testo formattato quando si modifica un campo di tipo Paragrafo.

Per informazioni, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

### Esperienza migliorata durante la modifica dei campi Selezione singola, Selezione multipla, Persone e durante l’aggiunta di oggetti connessi

Produzione: 8 febbraio 2024

Anteprima: da determinare

Abbiamo riprogettato e migliorato l’esperienza di aggiunta di opzioni o oggetti per i seguenti tipi di campi:

* Selezione singola
* Selezione multipla
* Persone
* Campi record collegati (quando si collegano tipi di record di capacità di pianificazione o oggetti Workfront)

Con il nuovo miglioramento, viene visualizzata prima una casella più piccola e più reattiva.

Per i campi connessi, è possibile aggiungerli eseguendo una delle operazioni seguenti:

* Aggiungere oggetti al campo connesso eseguendo ricerche e selezionandoli da un elenco nella visualizzazione tabella, mentre si modifica il campo in linea
* Fare clic per aprire la casella più grande Connetti oggetti, in cui è possibile visualizzare tutti i nomi degli elementi oltre a ulteriori informazioni sugli elementi.

I miglioramenti sono ora disponibili quando si aggiornano i campi nella vista tabella di un tipo di record.

Per ulteriori informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

## Settimana del 29 gennaio 2024

### Migliore condivisione di viste e aree di lavoro

Produzione: 30 gennaio 2024

Anteprima: da determinare

È stata migliorata l’esperienza di condivisione per le aree di lavoro e le visualizzazioni con i seguenti miglioramenti:

* Per chiarezza su ciò che ogni livello di autorizzazione consente a un utente di fare, sono stati aggiunti dettagli per ogni livello di autorizzazione durante la condivisione di un’area di lavoro e di una vista.

* Ora puoi copiare un collegamento in un’area di lavoro o visualizzarlo e condividerlo con altri utenti. Per accedere agli utenti dal collegamento copiato, è necessario disporre almeno delle autorizzazioni Visualizzazione per l&#39;area di lavoro o la visualizzazione.

Per ulteriori informazioni, consulta i seguenti articoli:

* [Condividi aree di lavoro](/help/quicksilver/planning/access/share-workspaces.md)
* [Condividere le visualizzazioni](/help/quicksilver/planning/access/share-views.md)

### Aggiungi miniature ai record

Produzione: 1 febbraio 2024

Anteprima: da determinare

È ora possibile aggiungere singole miniature a ciascun record per distinguerle in una visualizzazione. Nella vista a tabella è possibile aggiungere come miniature file immagine precedentemente salvati nel computer. Le miniature possono essere univoche per ciascun record e possono essere visualizzate sia nella vista tabella che nella vista timeline della pagina del tipo di record.

Per ulteriori informazioni, vedere [Aggiungere una miniatura a un record](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

### Rimuovi schede di tipo record collegate

Produzione: 1 febbraio 2024

Anteprima: da determinare

Per evitare confusione e semplificare la gestione delle aree di lavoro, sono state rimosse da un workspace le schede dei tipi di record generati automaticamente e di sola lettura per gli oggetti esterni connessi.

Per ulteriori informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

## Settimana del 22 gennaio 2024

### Nella nuova sezione Cronologia viene visualizzata l&#39;attività di sistema per i record delle funzionalità di pianificazione

Produzione: 25 gennaio 2024

Anteprima: da determinare

Per migliorare le funzionalità di controllo, è stata introdotta una nuova sezione nel pannello destro di un record in cui è possibile esaminare le modifiche apportate al record registrato dal sistema.

Le seguenti informazioni vengono registrate nella nuova sezione Cronologia:

* Qualsiasi modifica apportata ai campi

* I vecchi e i nuovi valori dei campi, quando i valori cambiano

* Nome completo dell&#39;utente che ha apportato la modifica

* Indicatore di data e ora in cui è avvenuta la modifica.

Per ulteriori informazioni, vedere [Panoramica della sezione Cronologia](/help/quicksilver/planning/records/history-section-overview.md).

### Nuova etichetta per collegamento nuovo record

Produzione: 25 gennaio 2024

Anteprima: da determinare

Per garantire coerenza durante la creazione dei record, il collegamento + Nuovo è stato rinominato per la creazione dei record in &quot;+ Nuovo record&quot;.  Prima di questo aggiornamento, il collegamento conteneva il nome del tipo di record. Il nuovo collegamento è ora disponibile durante la creazione di record operativi e di tassonomia. Per informazioni, vedere [Creare record](/help/quicksilver/planning/records/create-records.md).

## Settimana dell’8 gennaio 2024

### Le funzionalità di pianificazione vengono rimosse dagli ambienti di anteprima e sandbox

Anteprima e sandbox: 11 gennaio 2024

Le funzionalità di Adobe Workfront Planning sono state temporaneamente rimosse dagli ambienti di anteprima e sandbox. Gli ambienti verranno aggiunti a questi in una data successiva, come verrà comunicato nelle note sull’attività di rilascio.

### Autorizzazioni delle funzionalità di pianificazione per aree di lavoro e viste

Produzione: 11 gennaio 2024

Anteprima: da determinare

Ora puoi condividere un’area di lavoro o una vista con utenti e gruppi. È possibile impostare le relative autorizzazioni su livelli diversi, a seconda delle informazioni da visualizzare o modificare.

Quando si condivide un&#39;area di lavoro, gli utenti dispongono delle autorizzazioni per i tipi di record, i record e i campi in tale spazio.

Quando si condivide un&#39;area di lavoro, gli utenti non ricevono autorizzazioni di condivisione per le visualizzazioni associate ai tipi di record dell&#39;area di lavoro. È necessario concedere autorizzazioni separate alle visualizzazioni.

Di seguito sono riportati i livelli di autorizzazione per le aree di lavoro:

* Visualizzazione: gli utenti possono visualizzare le aree di lavoro condivise con loro. Possono inoltre visualizzare i tipi di record e i record dall&#39;area di lavoro condivisa.

* Contribute: gli utenti possono creare, modificare o eliminare i record nell’area di lavoro condivisa con loro.  Non possono creare o modificare tipi di record o aree di lavoro condivisi con loro.

* Gestione: gli utenti possono creare, modificare ed eliminare aree di lavoro, tipi di record, record e campi nelle aree di lavoro condivise.

Di seguito sono riportati i livelli di autorizzazione per le visualizzazioni record:

* Visualizza: gli utenti possono selezionare la visualizzazione dal menu a discesa Visualizza di una pagina del tipo di record.
* Gestisci: gli utenti possono modificare, condividere ed eliminare la visualizzazione.

Per ulteriori informazioni, vedere [Panoramica dell&#39;accesso](/help/quicksilver/planning/access/access-overview.md) e [Panoramica delle autorizzazioni di condivisione nelle funzionalità di Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

### Nuovo tipo di campo Formula

Produzione: 11 gennaio 2024

Anteprima: da determinare

È ora possibile aggiungere un campo di tipo Formula a un tipo di record.

I campi formula generano un nuovo valore utilizzando i valori esistenti di altri campi di un tipo di record e una funzione che indica come devono essere calcolati i valori esistenti.

Non è possibile utilizzare campi di ricerca da tipi di record collegati in un calcolo di formula. Questa funzionalità sarà disponibile in un secondo momento.

Per informazioni, vedere [Panoramica dei campi formula](/help/quicksilver/planning/fields/formula-fields.md).

### Azioni Annulla/Ripristina durante la gestione dei record nella vista a tabella

Produzione: 11 gennaio 2024

Anteprima: da determinare

È ora possibile annullare o ripristinare le modifiche apportate durante l&#39;esecuzione delle azioni seguenti nella vista a tabella:

* Copiare/incollare dati
* Modifica record
* Aggiungi record
* Elimina record

Per annullare o ripristinare le azioni, potete utilizzare le seguenti sequenze di tasti:

* Annulla: CTRL/COMANDO + Z
* Ripeti: CTRL/ COMANDO + MAIUSC+Z

Per ulteriori informazioni, consulta i seguenti articoli:

* [Modifica record](/help/quicksilver/planning/records/edit-records.md)

* [Elimina record](/help/quicksilver/planning/records/delete-records.md)

* [Crea record](/help/quicksilver/planning/records/create-records.md)


