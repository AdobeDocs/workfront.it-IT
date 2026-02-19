---
title: 'Creare Bridge: connessione di un intento strategico ai progetti'
description: Scopri come creare un "thread strategico" tra i piani di alto livello in Adobe Workfront Planning e l’esecuzione quotidiana dei flussi di lavoro in Adobe Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 567ab223-b282-4b98-9655-7b9766fba869
source-git-commit: 7f3ca12d89a2a5fbebc12b3df8a40edbb17d0ead
workflow-type: tm+mt
source-wordcount: '1156'
ht-degree: 0%

---


# Costruire il ponte: collegare l’intento strategico ai progetti

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono ad Adobe Workfront Planning, una funzionalità aggiuntiva di Adobe Workfront.
>
>L&#39;organizzazione deve disporre di un pacchetto Workfront Planning Prime o di una versione successiva per supportare le funzionalità consigliate in questo articolo.
>
>Per un elenco dei requisiti per accedere a Workfront Planning, vedere [Panoramica dell&#39;accesso ad Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Per informazioni generali su Workfront Planning, vedere [Introduzione ad Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Scopri come creare un thread strategico tra i piani di alto livello in Adobe Workfront Planning e l’esecuzione giornaliera in Workfront. Puoi creare un ponte tra strategia ed esecuzione utilizzando le connessioni.

Questa guida è destinata agli amministratori di Workfront e ai manager di workspace che implementano Workfront Planning.

## Panoramica dell’allineamento della strategia all’esecuzione

Collegare la tua strategia al tuo lavoro quotidiano trasforma la visione in realtà. Quando i piani di alto livello sono sincronizzati con l&#39;esecuzione, si crea un thread strategico che assicura che ogni progetto e attività faccia avanzare l&#39;azienda.

Per ottenere questo allineamento è necessario disporre di una serie di collegamenti tecnici e guardrail dei processi che colleghino le attività in Workfront con i record strategici di Workfront Planning.

Colmando il divario tra la pianificazione e l&#39;azione, l&#39;energia del team sarà sempre focalizzata sugli obiettivi più prioritari.

## Stabilire la base creando una connessione

Prima di poter creare un bridge per la pianificazione e l&#39;esecuzione, in qualità di responsabile dell&#39;area di lavoro è necessario definire i tipi di record idonei per una connessione.

### Panoramica del campo di connessione

Il ponte inizia con la creazione di un campo di connessione.

Un campo di connessione funge da handshake tecnico tra tipi di record.

Questo tipo di campo è il motore di tutte le relazioni in Workfront Planning. Si tratta di un’espressione di intento, in quanto stabilisce che un tipo di record specifico (come una tattica di canale) può essere collegato ad altri tipi di oggetto, sia che risiedano in Planning che in Workfront.

Per informazioni, vedere [Panoramica sui tipi di record connessi](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

### Definire quando creare una connessione

In teoria, è necessario decidere se è necessario creare connessioni prima di creare qualsiasi lavoro.

Aggiungendo un campo di connessione, si progetta l&#39;ambiente in modo da supportare un thread strategico, indipendentemente dalla modalità di creazione dei singoli record.

## Impostare strategia ed esecuzione in sincronia

Per mantenere incentrato il livello strategico, consigliamo di concentrare i record di pianificazione su intenti di alto livello mentre si utilizza Workfront per l’esecuzione tattica.

Questo approccio utilizza i punti di forza univoci di entrambi i moduli nei seguenti modi:

* **Pianificazione Workfront (livello strategico):** rimane di alto livello. Tiene traccia di Campaign, Channel Tactic e Budget. È silenzioso e pronto per l&#39;ufficio.

* **Workfront (livello di esecuzione):** gestisce i dettagli tattici. Puoi gestire singole esperienze o attività come progetti, attività e problemi. Puoi assegnarli per la proprietà e generarli nelle approvazioni per l’esecuzione.

## Passare dall&#39;intento all&#39;azione attivando il ponte

Una volta configurata la connessione, devi decidere come attivare il collegamento tra un record strategico specifico e un progetto di esecuzione.

### Utilizza un percorso guidato da tabella

Gli strateghi e gli utenti esperti utilizzano spesso la vista tabella come workbench per perfezionare i piani nel tempo.

Per impostazione predefinita, la creazione di un record in una tabella non stabilisce un collegamento a Workfront.

La connessione a un progetto di esecuzione viene stabilita quando un utente decide di attivare il collegamento.

Questa operazione può essere eseguita nei seguenti modi:

* Creare manualmente un progetto connesso a valle direttamente dal campo di connessione in Workfront Planning o da una pagina Connessioni facoltativa nella visualizzazione dettagli del record.

  La creazione manuale dà luogo a un progetto vuoto senza moduli personalizzati specifici.

  Per informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

* Automaticamente, utilizzando le automazioni di Workfront Planning, per esigenze più complesse.

  Queste automazioni sono disponibili come pulsanti nella barra delle azioni quando si seleziona una riga in una tabella.

  Questo consente la supervisione umana o la creazione di segnaposto, garantendo che i progetti vengano generati nell’ambiente del flusso di lavoro solo quando sono realmente necessari.

  Per informazioni, vedere [Creare oggetti utilizzando le automazioni dei record di Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)


### Creare attivazioni automatizzate

Per le organizzazioni con richieste di volumi elevati o esigenze di automazione avanzate, il bridge può essere attivato automaticamente in base a eventi specifici o in base ai valori dei campi configurati in un modulo di richiesta.

Per questo approccio è necessaria una licenza per Adobe Workfront Fusion.

Per ulteriori informazioni, vedere [Configurazione e gestione di Workfront Fusion: indice articolo](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-workfront-fusion-toc).

* **Utilizzare i trigger di invio:** Poiché i moduli forniscono un singolo evento di invio pulito, possono essere utilizzati come trigger per le automazioni di Fusion. Uno scenario Fusion può rilevare l’invio di un modulo e generare immediatamente un progetto collegato in Workfront.

* **Usa trigger valore campo:** Per un&#39;automazione più approfondita, è possibile configurare Fusion per il monitoraggio di campi specifici. Ad esempio, una semplice casella di controllo denominata &quot;Pronto per l&#39;esecuzione&quot; può fungere da catalizzatore, stabilendo il ponte automaticamente nel momento in cui viene controllato.

## Aggiungi campi di ricerca alla visibilità superficiale

Una volta collegato un progetto, puoi ottenere dati in tempo reale da Workfront direttamente all’interno del record Planning aggiungendo campi di ricerca dal progetto.

In qualità di responsabile dell&#39;area di lavoro, puoi impostare campi di ricerca per estrarre qualsiasi campo personalizzato o di sistema dal progetto collegato (ad esempio Data di completamento effettiva o Lead Creative) al tipo di record Pianificazione. Una volta acquisiti, questi dati possono essere aggregati attraverso più livelli della gerarchia strategica, fino al livello della campagna. In questo modo le parti interessate possono disporre di potenti funzionalità di reporting aggregato per l’intero ciclo di vita del marketing, che consentono loro di essere informati senza uscire dall’ambiente di pianificazione.

## Ottenere visibilità collegando la strategia all&#39;azione

Il valore finale del ponte è la visibilità in tempo reale.

Collegando l&#39;intenzione all&#39;azione, è possibile rispondere rapidamente alle domande aziendali critiche. Di seguito sono riportati alcuni esempi di queste domande:

* La nostra campagna &#39;FY26 Brand Awareness&#39; sta dando risultati concreti in questo momento?

* In quali casi le nostre tattiche strategiche richiedono un supporto più creativo per rispettare i tempi previsti?

* Come allineiamo le nostre risorse ai nostri pilastri strategici di massima priorità?

## Best practice e suggerimenti

### Dos:

* **Utilizza la metafora &quot;thread strategico&quot;:** Ricorda ai team che ogni progetto deve essere un &quot;bead&quot; in una stringa strategica.

* **Automatizza il passaggio di consegne:** Utilizza le automazioni per attivare la creazione del progetto per risparmiare tempo e fatica, migliorando al contempo la connettività e la governance dei dati.

* **Collegamento, non duplicare:** Utilizza i campi di ricerca per far emergere i dati di esecuzione in tempo reale (come lo stato o le date di completamento) nei tuoi record strategici. In questo modo le viste strategiche saranno sempre precise senza richiedere aggiornamenti manuali da parte del team.

### Non:

* **Non trattare i record di pianificazione come elenchi di attività:** Il bridge è progettato per collegare l&#39;intento strategico ai progetti di esecuzione. Mantenere i record di pianificazione incentrati su &quot;cosa&quot; e &quot;perché&quot; e lasciare che il modulo del flusso di lavoro gestisca il &quot;come&quot; granulare attraverso attività e problemi.

* **Non sincronizzare in modo eccessivo:** Non è necessario sincronizzare tutti i dettagli a livello di progetto con Planning. Mantenere il livello strategico ad alto livello e senza rumore.

* **Non ignorare il bridge:** se il lavoro inizia nel modulo del flusso di lavoro senza un collegamento a Planning, è stato creato un &quot;Piano ombra&quot; invisibile alla leadership.

<!--original content:

# The Bridge: Connecting Strategic Intent to Projects 

 

## Goal 

Learn how to create a "strategic thread" between your high-level plans in Workfront Planning and your daily execution in the Workflow module. 

 

## Overview 

Connecting your strategy to your daily work turns vision into reality. When high-level plans are in sync with execution, you create a **strategic thread** that ensures every project and task moves the business forward. 

 

Achieving this alignment requires a set of technical links and process guardrails that connect efforts in the **Workflow module** with strategic records in **Workfront Planning (WFP)**. By bridging the gap between planning and action, you ensure that your team's energy is always focused on your highest-priority goals. 

 

## The foundation: Establishing the connection 

Before you can bridge planning and execution, a workspace manager must define which record types are eligible for a connection. 

 

### The connection field: The technical handshake 

The bridge begins with a **connection field**. This field type is the engine behind all relationships in WFP. It is an expression of intent, in that it establishes that a specific record type (like a *channel tactic*) is allowed to be linked to other objects, whether they live in the workflow module or within planning itself. 

 

### Deciding to connect 

Establishing this allowance is a configuration-level decision that typically happens before any work is created. By adding a connection field, you are architecting your environment to support a "strategic thread," regardless of how the individual records are eventually created. 

 

## Strategy and execution in sync 

To keep your strategic layer focused, we recommend focusing your planning records on high-level intent while using the Workflow module for tactical execution. This approach uses the unique strengths of both modules: 

 

*   **Workfront Planning (The strategic layer):** Stays high-level. It tracks the *Campaign*, the *Channel Tactic*, and the *Budget*. It is noise-free and executive-ready. 

*   **Workflow module (The execution layer):** Manages the tactical details. Individual "Experiences" or "Activities" are managed here as **projects, tasks, and issues**. 

 

## Activating the bridge: From intent to action 

Once the connection is configured, you must decide how to activate the link between a specific strategic record and an execution project. 

 

### Professional triage: The table-led path 

Strategists and power users often use the **table view** as their "workbench" to refine plans over time.  

*   **Deliberate handoff:** By default, creating a record in a table does not establish a link to the Workflow module. The connection to an execution project is established when a user decides to activate the link. This can be done by manually creating a downstream connected project directly from the connection field in WFP or an optional **connection view page** in the record's detail view. Note that manual creation results in a blank project without specific custom forms; for more complex needs, you can use a **native WFP automation**. These automations are available when you select a row in a table, appearing as buttons in the blue action bar at the bottom of your screen. This allows for human oversight or placeholder creation, ensuring that projects are only generated in your workflow environment when they are truly needed. 

 

### Automated activation 

For organizations with high-volume requests or advanced automation needs, the bridge can be activated automatically based on specific events or field values. 

*   **Submission triggers:** Because forms provide a single, clean "submission event," they can be used as triggers for **Fusion automations**. A scenario can detect a form submission and immediately generate a linked project in the workflow module. 

*   **Field-value triggers:** For deeper automation, you can configure **Fusion** to monitor specific fields. For example, a simple checkbox labeled "ready for execution" can serve as the catalyst, establishing the bridge automatically the moment it is checked. 

 

## Surfacing visibility: Lookup fields 

Once a project is linked, you can surface real-time data from the Workflow module directly within the WFP record. 

 

A workspace manager can set up **lookup fields** to pull any native or custom field from the linked project (such as *actual completion date* or *creative lead*) into the WFP record type. Once captured, this data can be rolled up through multiple levels of your strategic hierarchy—even all the way to the campaign level. This provides powerful aggregate reporting for stakeholders across the entire marketing lifecycle, keeping them informed without needing to leave the planning environment. 

 

## Strategy-to-action visibility 

The ultimate value of the bridge is **real-time visibility**. By connecting intent to action, you can answer critical business questions at a glance: 

 

*   "Is our 'FY26 Brand Awareness' campaign actively delivering results right now?" 

*   "Where do our strategic tactics need more creative support to stay on schedule?" 

*   "How are we aligning our resources with our highest-priority strategic pillars?" 

 

## Best practices & tips 

 

### Do: 

*   **Use the "strategic thread" metaphor.** Remind teams that every project should be a "bead" on a strategic string. 

*   **Automate the handoff.** Use automations to trigger project creation to save time and effort while also improving data connectivity and governance. 

*   **Link, don't duplicate.** Use lookup fields to surface real-time execution data (like status or completion dates) in your strategic records. This ensures your strategic views are always accurate without requiring manual updates from your team. 

 

### Don't: 

*   **Don't treat planning records as task lists.** The bridge is designed to connect strategic intent to execution projects. Keep your planning records focused on the "what" and "why," and let the workflow module handle the granular "how" through tasks and issues. 

*   **Don't over-sync.** You don't need to sync every project-level detail back to Planning. Keep the strategic layer high-level and noise-free. 

*   **Don't bypass the bridge.** If work starts in the Workflow module without a link to Planning, you've created a "Shadow Plan" that is invisible to leadership. 

-->



