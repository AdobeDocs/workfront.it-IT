---
title: 'Architect Your Success: Modeling Your Campaign Hierarchy'
description: Scopri come tradurre i processi aziendali complessi in una gerarchia di campagne scalabile e gestita utilizzando "Centri di gravità" e un’architettura con più aree di lavoro.
feature: Workfront Planning
role: Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 02e3b55f-9188-42bf-8d0b-c9fed86c63c4
source-git-commit: a5f33f914dabaa9368dea919510375bcb6ee03e2
workflow-type: tm+mt
source-wordcount: '1541'
ht-degree: 0%

---

# Creare un’architettura di successo: modellare la gerarchia delle campagne

<!--see the file again for additional comments from Seth and others-->

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo si riferiscono ad Adobe Workfront Planning, una funzionalità aggiuntiva di Adobe Workfront.
>
>L&#39;organizzazione deve disporre di un pacchetto Workfront Planning Prime o di una versione successiva per supportare le funzionalità consigliate in questo articolo.
>
>Per un elenco dei requisiti per accedere a Workfront Planning, vedere [Panoramica dell&#39;accesso ad Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Per informazioni generali su Workfront Planning, vedere [Introduzione ad Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Scopri come tradurre i processi aziendali complessi in una gerarchia di campagne scalabile e gestita utilizzando i centri di gravità e un’architettura con più aree di lavoro in Adobe Workfront Planning.

Questa guida è destinata agli amministratori di Workfront e agli utenti esperti che implementano e progettano l&#39;architettura dell&#39;ambiente in Workfront Planning.

## Panoramica dell’architettura di successo

Con la maturazione delle operazioni di marketing, cresce anche la complessità dei dati. Senza una blueprint chiara, il tuo Marketing System of Record può rapidamente diventare un cassetto di posta indesiderata di record disconnessi, terminologia in conflitto e silos di reporting.

Quando crei un’architettura di successo, stabilisci un framework per modellare la gerarchia delle campagne in Workfront Planning. Si passa dal caos dei fogli di calcolo a un modello governato e orientato agli oggetti che garantisce che ogni team parli la stessa lingua mantenendo l’agilità necessaria per l’esecuzione.

## Creare una gerarchia per definire i livelli di intento

Per garantire chiarezza e scalabilità, si consiglia di iniziare con un percorso di base collaudato durante la progettazione del flusso di lavoro in Workfront Planning.

Da lì, puoi espandere la tua strategia aggiungendo più livelli all’architettura.

### Il percorso principale: come passare da strategia a azione

Anche se le organizzazioni possono espandere questa gerarchia man mano che le loro esigenze operative evolvono, a partire dai tre livelli descritti nelle sezioni seguenti garantisce un solido ponte tra strategia ed esecuzione.

Dalle nostre scoperte, abbiamo notato che la maggior parte delle implementazioni di successo di Workfront Planning prosperano su un modello pulito e a tre livelli che abbraccia sia Planning che Workfront.

Di seguito sono riportati i livelli di una corretta implementazione di Planning e gli artefatti che è possibile creare per supportare l&#39;utente nel processo:

* **Livello 1: Campagne (Workfront Planning)**

   * **Obiettivo:** definire i pilastri strategici a lungo termine e le iniziative annuali. Ad esempio, definisci un&#39;iniziativa per la tua organizzazione denominata &quot;Consapevolezza del marchio globale per l&#39;anno fiscale 2026&quot;. Questo è il tuo punto focale per un determinato intervallo di tempo. Crea campagne per supportare questa iniziativa.

   * **Persone:** Le parti interessate per questo livello possono essere Marketing Officer, Vice President Marketing o altri lead strategici.

  Per informazioni, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

* **Livello 2: tattiche di canale (Workfront Planning)**

   * **Stato attivo:** Definisci le istruzioni operative che definiscono il &quot;cosa&quot; per canali specifici. Questo è il livello finale dell&#39;intento strategico prima dell&#39;inizio dei lavori. Ad esempio, crea una tattica &quot;Blitz sui social media Q1&quot;. Puoi quindi associarlo alle campagne.

   * **Persone:** le principali parti interessate sono un leader delle operazioni di marketing, capi canale o responsabili delle campagne.

* **Livello 3: Progetti (Planning e Workfront)**

   * **Focus:** esegui le esperienze o le attività che alla fine consentiranno di completare l&#39;iniziativa. Alcuni dei risultati finali sono specifici, come post social, e-mail e pagine web.

   * **Implementazione:** è possibile creare le tattiche in Planning e collegarle direttamente ai **progetti** in Workfront, dove i singoli risultati finali vengono gestiti come attività e problemi.

   * **Persona:** Le principali parti interessate sono i creativi, i singoli collaboratori, chiunque sia responsabile del lavoro di supporto all&#39;iniziativa.

### Espansione strategica: come aggiungere altri livelli

Una volta stabilito il percorso di base, è possibile scegliere di aggiungere altri livelli dopo aver attentamente considerato la loro complessità aziendale specifica.

Può essere utile creare i seguenti elementi aggiuntivi:

* **Piani canale:** un livello tra campagne e tattiche per raggruppare strategie cross-functional. Ad esempio, un piano denominato &quot;Strategia digitale&quot;.

* **Attività:** Se si lavora in un ambiente con volumi inferiori (è possibile che siano presenti al massimo 5.000 deliverable all&#39;anno), alcuni team potrebbero preferire tenere traccia delle singole esperienze come record di Workfront Planning prima che diventino progetti Workfront.

>[!IMPORTANT]
>
>Se la tua organizzazione produce più di 5.000 attività all&#39;anno, devi spostare il tracciamento dei singoli deliverable in Workfront.
>
>La gestione di grandi volumi di record di esperienza in Planning può portare all’accumulo di dati che oscura la visibilità strategica.
>Per la massima efficienza consigliamo questa linea guida generale:
>
>* Utilizza Pianificazione per il &quot;perché&quot; e il &quot;cosa&quot;
>* Utilizza Workfront per il volume elevato &quot;come&quot;.

## Comprendere i centri di gravità per costruire la tua architettura

Un sistema di record di marketing di livello Enterprise non viene creato in un&#39;unica area di lavoro. Utilizza un&#39;architettura &quot;hub-and-spoke&quot; in cui i tipi di record vengono gestiti nei loro centri di gravità naturali.

Per ulteriori informazioni, consulta [Roll out della tua pagina iniziale strategica: un launchpad di 30 giorni](/help/quicksilver/planning/best-practices.md/30-day-launchpad.md).

Per creare l’architettura utilizzando l’approccio hub-and-spoke, è necessario creare quanto segue:

* Un hub di tassonomia
* Un&#39;area di lavoro di pianificazione strategica
* Raggi funzionali

### Creare l’hub della tassonomia come classificazioni

Devi innanzitutto stabilire un’area di lavoro centralizzata per le classificazioni globali, in modo da definire i concetti principali che tutti i membri dell’organizzazione devono comprendere. Ad esempio, crea i seguenti tipi di record in un’area di lavoro centrale: Marchi, Aree geografiche, Prodotti, Utenti tipo.

Per informazioni, consulta:

* [Crea tipi di record](/help/quicksilver/planning/architecture/create-record-types.md)

* [Panoramica del tipo di record in più aree di lavoro](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

Quando crei le classificazioni, stabilisci quanto segue:

* **Percorso principale:** Scegliere un&#39;area di lavoro principale. Questa area di lavoro deve essere l&#39;origine di verità per i tipi di record creati.

* **Vantaggio:** Sindacando queste definizioni al resto dell&#39;azienda, risolvi che concetti come &quot;Area geografica: EMEA&quot; significano la stessa cosa per ogni team.

### Creare l&#39;area di lavoro Pianificazione strategica come centro esecutivo

Il centro direzionale è il luogo in cui si svolgono le campagne di alto livello (e qualsiasi piano di canale).

* **Sede principale:** Questo è il centro di gravità esecutivo, che fornisce un ambiente privo di rumore per il processo decisionale strategico.

* **Vantaggio:** i dirigenti possono gestire il portfolio di campagne senza ascoltare il rumore tattico quotidiano.

### Definire i raggi funzionali come aree di lavoro dei team

Le unità funzionali (Social, Creative, E-mail) dispongono di aree di lavoro proprie per gestire le proprie tattiche.

* **Posizione primaria:** Queste aree di lavoro sono i singoli centri di gravità per l&#39;esecuzione del team locale.

* **Vantaggio:** i team utilizzano le campagne e le classificazioni globali dagli hub, mantenendo al contempo i propri oggetti locali.

  Ad esempio, il team può aggiungere il tipo di record Campaign dall’area di lavoro centrale all’area di lavoro del team, ma creare campagne rilevanti solo per la propria area di lavoro. Esempi di campagne sono &quot;Media outlets&quot; o &quot;Usage rights&quot; (Diritti di utilizzo).

## Utilizzare un approccio di governance basato su sostantivi

Per garantire che l’architettura rimanga sotto pressione, segui il principio della governance basata sul nome.

Durante la creazione di entità in Workfront Planning, è consigliabile effettuare le seguenti operazioni:

* **Utilizza sostantivi, non verbi:** Denomina i tipi di record dopo gli elementi che stai tracciando (chiamali &quot;Campagna&quot; o &quot;Tattico&quot;), non le azioni da eseguire (non denominarli &quot;Campagna&quot; o &quot;Pianificazione&quot;).

* **Nomenclatura standard:** Utilizzare gli stessi nomi in tutte le aree di lavoro. Questo consente di aggregare i dati nell’intero portfolio per i rapporti manageriali.

## E i programmi e i portafogli esistenti?

Una domanda comune per le organizzazioni mature è come gestire i Portfolio e i Programmi già integrati in Workfront. In passato, questi oggetti venivano spesso utilizzati per imitare la pianificazione strategica.

Ora consigliamo di adottare un approccio diverso alla pianificazione di Workfront, che si adatta perfettamente all&#39;approccio strategico alla pianificazione.

### Sostituzione di portafogli e programmi con tipi di record

In molte organizzazioni, i Portfolio vengono utilizzati per rappresentare marchi di alto livello o Business Unit, mentre i Programmi rappresentano temi strategici.

In Workfront Planning, è consigliabile modellarli come Tipi di record nell&#39;hub di tassonomia.

Trattando un marchio o un’unità aziendale come tipo di record, puoi collegarli a una campagna o a una tattica in tutta l’azienda, fornendo un reporting molto più flessibile rispetto a una struttura statica Portfolio - Programma.

### Utilizzare una strategia di reporting-bridge

Mentre Workfront Planning è il futuro dell’intento strategico, il reporting nativo tramite Canvas Dashboard è ancora in fase di maturazione.

Molte organizzazioni si affidano ancora alle solide funzionalità di reporting associate alle strutture legacy di Portfolio e Program in Workfront.

Consigliamo quanto segue:

* Non eliminare portafogli e programmi.
* Utilizzare le automazioni di Planning per creare un ponte tra i tipi di record, i portfolio e i programmi.

  Quando si crea una tattica o una campagna in Workfront Planning, tale record può generare un Portfolio o un programma corrispondente in Workfront.

  Per informazioni, vedere [Creare oggetti utilizzando le automazioni dei record di Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

Questo consente di:

* Approfitta della visualizzazione strategica superiore di Workfront Planning utilizzando timeline e calendari.

* Gestisci i rapporti legacy in Workfront per le parti interessate che non sono ancora pronte per il passaggio a Canvas.

## Best practice e suggerimenti

### Dos

* **Attieniti al primo approccio basato sul percorso principale:** Stabilisci il flusso da campagna a tattica a progetto prima di aggiungere ulteriore complessità.

* **Assegna aree di lavoro primarie:** Assicurarsi che ogni tipo di record disponga di un&#39;area di lavoro principale (considerare che il relativo baricentro) che funge da aggregatore per i rapporti.

* **Assegna priorità ai moduli di richiesta per il processo di assegnazione:** Utilizza i moduli di record per i gruppi meno sofisticati in Workfront Planning per garantire l&#39;integrità dei metadati.

  >[!CAUTION]
  >
  >Anche se gli utenti avanzati possono trarre vantaggio dall’inserimento diretto dei dati nelle visualizzazioni tabella, questo deve essere affrontato con cautela.
  >Le modifiche in blocco in una tabella possono creare facilmente problemi di dati per altre parti interessate.

### Non fare

* **Non utilizzare generalizzazioni:** Ad esempio, invece di parlare di un ambiente &quot;core&quot;, quando si parla di esecuzione fare riferimento in modo specifico a Workfront e all&#39;oggetto Project.

* **Non complicare eccessivamente:** Ogni ulteriore livello gerarchico aggiunge un&#39;imposta di gestione. Aggiungere solo livelli che rispondono a una domanda aziendale a cui non è attualmente possibile rispondere.

* **Non creare silos:** Verificare che i tipi di record siano condivisi tra le aree di lavoro in modo che i team non digitino nuovamente gli stessi dati.


<!--original content:


## Goal 

Learn how to translate your complex business processes into a scalable, governed campaign hierarchy using "Centers of Gravity" and a multi-workspace architecture. 

 

## Overview 

As your marketing operations scale, so does the complexity of your data. Without a clear blueprint, your Marketing System of Record (MSOR) can quickly become a "junk drawer" of disconnected records, conflicting terminology, and reporting silos. 

 

The "Blueprint of Success" is a framework for modeling your campaign hierarchy in Workfront Planning. It moves you from "spreadsheet chaos" to a governed, object-oriented model that ensures every team speaks the same language while maintaining the agility they need to execute. 

 

## The Hierarchy: Finding Your Levels of Intent 

To maintain clarity and scalability, we recommend starting with a proven **Core Path**. While organizations can expand this hierarchy as their operational needs evolve, beginning with these three levels ensures a strong bridge between strategy and execution. 

 

### The Core Path: Strategy to Action 

Most successful implementations thrive on a clean, three-tier model that spans both Planning and Workflow: 

 

1. **Level 1: Campaigns (Planning Module)** 

    * **Focus:** Long-term strategic pillars and annual initiatives (e.g., "FY26 Global Brand Awareness").  

    * **Persona:** CMO, VP of Marketing, Strategic Leads. 

2. **Level 2: Channel Tactics (Planning Module)** 

    * **Focus:** The operational briefs defining the "what" for specific channels (e.g., "Q1 Social Media Blitz"). This is the final layer of strategic intent before work begins. 

    * **Persona:** Marketing Ops, Channel Leads, Campaign Managers. 

3. **Level 3: Workflow Projects (Workflow Module)** 

    * **Focus:** The actual execution of "Experiences" or "Activities" (e.g., specific social posts, emails, web pages).  

    * **Implementation:** Tactics in Planning link directly to **Projects** in the Workflow module, where individual deliverables are managed as tasks and issues. 

    * **Persona:** Creatives, Individual Contributors. 

 

### Strategic Expansion: Adding More Levels 

Once the core path is established, organizations may choose to add additional layers after careful consideration of their specific business complexity: 

 

* **Channel Plans:** A layer between *Campaigns* and *Tactics* to group cross-functional strategies (e.g., "Digital Strategy"). 

* **Workfront Planning Activities:** In lower-volume environments (typically <5,000 deliverables/year), some teams prefer to track individual "Experiences" as Workfront Planning records before they become projects. 


>[!TIP]
>
>**Crucial Tip: The 5,000 Deliverable Threshold** 
>
>If your organization produces more than 5,000 activities per year, you should **always** offload individual deliverable tracking to the **Workflow module**. Managing high-volume "Experience" records in Planning can lead to data accumulation that obscures your strategic visibility. Use Planning for the "Why" and "What," and the Workflow module for the high-volume "How." 

 

## Architecture: Centers of Gravity 

An enterprise-grade MSOR isn't built in a single workspace. It uses a "Hub-and-Spoke" architecture where record types are managed in their natural **Centers of Gravity**. 

 

### 1. The Taxonomy Hub (Classifications) 

Establish one centralized workspace for your "Global Classifications" (e.g., Brands, Regions, Products, Personas). 

* **Primary Location:** This workspace is the "Source of Truth" for these objects. 

* **The Benefit:** By syndicating these definitions to the rest of the business, you solve "Semantic Drift"—ensuring that "Region: EMEA" means the same thing to every team. 

 

### 2. The Strategic Planning Workspace (Executive Center) 

This is where high-level **Campaigns** (and any **Channel Plans**) live.  

* **Primary Location:** This is the executive center of gravity, providing a noise-free environment for strategic decision-making. 

* **The Benefit:** Leadership can manage the portfolio without seeing the day-to-day tactical mess. 

 

### 3. Functional Spokes (Team Workspaces) 

Functional units (Social, Creative, Email) have their own workspaces to manage their **Tactics**. 

* **Primary Location:** These workspaces are the center of gravity for local team execution.  

* **The Benefit:** Teams "consume" the global campaigns and classifications from the hubs, while maintaining their own local objects (like *Media Outlets* or *Usage Rights*). 

 

## Noun-Based Governance: Speak One Language 

To ensure your blueprint holds up under pressure, follow the principle of **Noun-Based Governance**.  

 

* **Use Nouns, Not Verbs:** Name your record types after the "things" you are tracking (`Campaign`, `Tactic`), not the "actions" (`Campaigning`, `Planning`). 

* **Standardize Nomenclature:** Use the same names across all workspaces. This allows you to aggregate data across the entire portfolio for executive reporting. 

 

## What About Existing Portfolios and Programs? 

A common question for mature organizations is how to handle the Portfolios and Programs they've already built in the **Workflow module**. In the past, these objects were often used to mimic strategic planning. 

 

### 1. Portfolios & Programs → Record Types 

In many organizations, **Portfolios** are used to represent high-level Brands or Business Units (BUs), while **Programs** represent strategic themes. 

* **The Shift:** These are best modeled as **Record Types** in your **Taxonomy Hub**. By treating "Brand" or "Business Unit" as a record type, you can link them to any campaign or tactic across the entire enterprise, providing much more flexible reporting than a static Portfolio/Program structure. 

 

### 2. The "Reporting Bridge" Strategy 

While Workfront Planning is the future of strategic intent, its native reporting via **Canvas Dashboards** is still maturing. Many organizations still rely on the robust reporting capabilities tied to their legacy Portfolio and Program structures in the Workflow module. 

* **The Recommendation:** Don't delete your Portfolios and Programs yet. Instead, use **Fusion automations** to create a bridge.  

* **How it Works:** When a Tactic or Campaign is created in Workfront Planning, Fusion can automatically mirror that record into a corresponding Portfolio or Program in the Workflow module. This allows you to: 

    1. Enjoy Workfront Planning's superior **strategic visualization** (Timelines/Calendars). 

    2. Maintain your **legacy reporting** in the Workflow module for stakeholders who aren't yet ready to move to Canvas. 

## Best Practices & Tips 

### Do: 

* **Stick to the Core Path first.** Establish your Campaign-to-Tactic-to-Project flow before adding more complexity. 

* **Designate Primary Workspaces.** Ensure each record type has one "home" workspace (its center of gravity) that acts as the aggregator for reporting. 

* **Prioritize Forms for Intake.** Use record forms for groups with less sophistication in Workfront Planning to ensure metadata integrity. While Power Users may benefit from direct data entry in Table views, this should be approached with caution—bulk changes in a table can easily create data headaches for other stakeholders. 
 

### Don't: 

* **Don't say "Core".** Refer specifically to the **Workflow module** and the **Project** objects when talking about execution. 

* **Don't over-complicate.** Every additional level of hierarchy adds a "management tax." Only add levels that answer a business question you can't currently answer. 

* **Don't create silos.** Ensure your record types are shared across workspaces so teams aren't re-typing the same data.
-->