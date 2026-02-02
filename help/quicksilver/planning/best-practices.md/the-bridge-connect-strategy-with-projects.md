---
title: 'Bridge: connessione di un intento strategico ai progetti'
description: Scopri come creare un "thread strategico" tra i piani di alto livello in Adobe Workfront Planning e l’esecuzione quotidiana dei flussi di lavoro in Adobe Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---


# Il ponte: collegare l&#39;intento strategico ai progetti


## Obiettivo

Scopri come creare un &quot;thread strategico&quot; tra i piani di alto livello in Workfront Planning e l’esecuzione quotidiana nel modulo Flusso di lavoro.



## Panoramica

Collegare la tua strategia al tuo lavoro quotidiano trasforma la visione in realtà. Quando i piani di alto livello sono sincronizzati con l&#39;esecuzione, si crea un **thread strategico** che assicura che ogni progetto e attività faccia avanzare l&#39;azienda.



Per raggiungere questo allineamento è necessario disporre di un set di collegamenti tecnici e guardrail di processo che colleghino le attività del **modulo flusso di lavoro** con record strategici in **Workfront Planning (WFP)**. Colmando il divario tra la pianificazione e l&#39;azione, l&#39;energia del team sarà sempre focalizzata sugli obiettivi più prioritari.



## La base: stabilire la connessione

Prima di poter creare un bridge per la pianificazione e l&#39;esecuzione, è necessario che un responsabile dell&#39;area di lavoro definisca i tipi di record idonei per una connessione.



### Campo di connessione: handshake tecnico

Il bridge inizia con un **campo connessione**. Questo tipo di campo è il motore di tutte le relazioni in WFP. Si tratta di un&#39;espressione di intento, in quanto stabilisce che un tipo di record specifico (come un *canale tattico*) può essere collegato ad altri oggetti, sia che risiedano nel modulo del flusso di lavoro che all&#39;interno della pianificazione stessa.



### Decidere di connettersi

La determinazione di questa tolleranza è una decisione a livello di configurazione che in genere si verifica prima della creazione di qualsiasi lavoro. Aggiungendo un campo di connessione, si progetta l&#39;ambiente in modo da supportare un &quot;thread strategico&quot;, indipendentemente dalla modalità di creazione dei singoli record.



## Strategia ed esecuzione sincronizzate

Per mantenere incentrato il livello strategico, consigliamo di concentrare i record di pianificazione su intenti di alto livello, utilizzando il modulo Flusso di lavoro per l’esecuzione tattica. Questo approccio utilizza i punti di forza univoci di entrambi i moduli:



* **Pianificazione Workfront (livello strategico):** rimane di alto livello. Tiene traccia di *Campaign*, *Channel Tactic* e *Budget*. È silenzioso e pronto per l&#39;ufficio.

* **Modulo flusso di lavoro (livello di esecuzione):** gestisce i dettagli tattici. Le singole &quot;esperienze&quot; o &quot;attività&quot; sono gestite qui come **progetti, attività e problemi**.



## Attivazione del ponte: dall’intento all’azione

Una volta configurata la connessione, devi decidere come attivare il collegamento tra un record strategico specifico e un progetto di esecuzione.



### Taglio professionale: il percorso guidato da tabella

Gli strateghi e gli utenti esperti spesso utilizzano la **vista tabella** come proprio &quot;workbench&quot; per perfezionare i piani nel tempo.

* **Handoff intenzionale:** Per impostazione predefinita, la creazione di un record in una tabella non stabilisce un collegamento al modulo del flusso di lavoro. La connessione a un progetto di esecuzione viene stabilita quando un utente decide di attivare il collegamento. Questa operazione può essere eseguita creando manualmente un progetto connesso a valle direttamente dal campo di connessione in Protezione file Windows o una **pagina di visualizzazione connessione** opzionale nella visualizzazione dettagli del record. La creazione manuale genera un progetto vuoto senza moduli personalizzati specifici. Per esigenze più complesse, è possibile utilizzare un&#39;automazione **WFP nativa**. Queste automatizzazioni sono disponibili quando si seleziona una riga in una tabella e vengono visualizzate come pulsanti nella barra delle azioni blu nella parte inferiore dello schermo. Questo consente la supervisione umana o la creazione di segnaposto, garantendo che i progetti vengano generati nell’ambiente del flusso di lavoro solo quando sono realmente necessari.



### Attivazione automatica

Per le organizzazioni con richieste di volumi elevati o esigenze di automazione avanzate, il bridge può essere attivato automaticamente in base a eventi specifici o a valori di campo.

* **Trigger invio:** Poiché i moduli forniscono un unico &quot;evento invio&quot;, possono essere utilizzati come trigger per **Automazioni Fusion**. Uno scenario può rilevare l’invio di un modulo e generare immediatamente un progetto collegato nel modulo del flusso di lavoro.

* **Trigger valore campo:** Per una maggiore automazione, puoi configurare **Fusion** per monitorare campi specifici. Ad esempio, una semplice casella di controllo etichettata &quot;pronto per l&#39;esecuzione&quot; può fungere da catalizzatore, stabilendo il ponte automaticamente nel momento in cui viene selezionato.



## Visibilità superficie: campi di ricerca

Una volta collegato un progetto, è possibile ottenere dati in tempo reale dal modulo Flusso di lavoro direttamente all&#39;interno del record WFP.



Un manager area di lavoro può impostare **campi di ricerca** per estrarre qualsiasi campo nativo o personalizzato dal progetto collegato (ad esempio *data di completamento effettiva* o *lead creativo*) nel tipo di record WFP. Una volta acquisiti, questi dati possono essere aggregati attraverso più livelli della gerarchia strategica, anche a livello di campagna. In questo modo le parti interessate possono disporre di potenti funzionalità di reporting aggregato per l’intero ciclo di vita del marketing, che consentono loro di essere informati senza uscire dall’ambiente di pianificazione.



## Visibilità strategia-azione

Il valore finale del bridge è **visibilità in tempo reale**. Collegando l&#39;intenzione all&#39;azione, è possibile rispondere rapidamente alle domande aziendali critiche:



* &quot;La nostra campagna &#39;FY26 Brand Awareness&#39; sta dando risultati concreti in questo momento?&quot;

* &quot;Quali sono le aree in cui le nostre tattiche strategiche richiedono un supporto più creativo per rispettare i tempi previsti?&quot;

* &quot;In che modo allineiamo le nostre risorse ai nostri pilastri strategici di massima priorità?&quot;



## Best practice e suggerimenti



### Effettua:

* **Utilizzare la metafora &quot;thread strategico&quot;.** Ricorda ai team che ogni progetto deve essere un &quot;bead&quot; su una stringa strategica.

* **Automatizzare il passaggio di consegne.** Utilizza le automazioni per attivare la creazione di progetti per risparmiare tempo e fatica, migliorando al contempo la connettività e la governance dei dati.

* **Collegamento, non duplicare.** Utilizza i campi di ricerca per far emergere i dati di esecuzione in tempo reale (come lo stato o le date di completamento) nei tuoi record strategici. In questo modo le viste strategiche saranno sempre precise senza richiedere aggiornamenti manuali da parte del team.



### Non:

* **Non considerare i record di pianificazione come elenchi di attività.** Il bridge è progettato per collegare l&#39;intento strategico ai progetti di esecuzione. Mantenere i record di pianificazione incentrati su &quot;cosa&quot; e &quot;perché&quot; e lasciare che il modulo del flusso di lavoro gestisca il &quot;come&quot; granulare attraverso attività e problemi.

* **Non sovrasincronizzare.** Non è necessario sincronizzare tutti i dettagli a livello di progetto con Planning. Mantenere il livello strategico ad alto livello e senza rumore.

* **Non aggirare il ponte.** Se il lavoro inizia nel modulo Flusso di lavoro senza un collegamento a Planning, è stato creato un &quot;Piano ombra&quot; invisibile alla leadership.




