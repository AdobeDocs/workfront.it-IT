---
title: 'Playbook: ridimensionamento gestito, dopo la prima vittoria'
description: Scopri come implementare Adobe Workfront Planning dopo la prima implementazione riuscita
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
exl-id: 54df36b3-01a3-4fd3-b2d3-64ffb2fe5918
source-git-commit: 52bf41e146a11a4af4fbebfe5bb20a9765f2bc7b
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 0%

---

# Playbook: ridimensionamento gestito, dopo la prima vittoria

{{planning-important-intro}}

**Versione**: 1.0

**Contesto**: &quot;Abbiamo ottenuto il primo caso d&#39;uso e ora tutti lo desiderano.&quot;



## &#x200B;1. La &quot;trappola del successo&quot;

A volte può sembrare che la fase più pericolosa dell’adozione del programma WFP sia immediatamente successiva al primo caso d’uso riuscito o POC. L&#39;entusiasmo è alto, ma il timore di un &quot;debito tecnico&quot; e di una &quot;espansione amministrativa&quot; può portare a due risposte altrettanto dannose:

1. **Sovra-governance**: blocco del sistema così stretto che i nuovi team tornano ai fogli di calcolo.

2. **Governance zero**: ogni team può creare i propri campi e tipi di record, ricreando la frammentazione dei metadati negli ambienti legacy.



## &#x200B;2. La filosofia di base: WFP come &quot;motore di riconciliazione&quot;

Invece di cercare di impedire ai team di essere diversi, posizioniamo WFP come il luogo in cui tali differenze sono **rese visibili in modo che possano essere riconciliate**.



* **Gestione della velocità di adozione**: prima di &quot;pulire&quot; gli ambienti esistenti, è naturale prestare attenzione all&#39;espansione in un nuovo strumento. La scelta di **Semplifica primo** fornisce una base altamente gestita, ma può ritardare il time-to-value per i team pronti per l&#39;allineamento. Riteniamo che il modo più efficace per superare questo cambiamento sia riconoscere che la visibilità di **è il passaggio 1**. Lo slancio verso uno strumento condiviso e pronto per l’azienda (allontanandosi dalla proliferazione di PPT e fogli di calcolo) è ciò che alla fine sblocca gli obiettivi a lungo termine.



  **Consiglio**: invece di un mandato di pulizia, si consiglia di allocare una porzione più piccola di risorse alla manutenzione in corso e una porzione molto più grande per risolvere le esigenze aziendali più pressanti. Ad esempio, spendere un anno esclusivamente per &quot;ripulire&quot; le tassonomie produce un valore incrementale minimo. Tuttavia, offrire **visibilità cross-team** (ad esempio, tramite un calendario aziendale unificato o una roadmap GTM consolidata) fornisce il valore di trasformazione di cui le parti interessate hanno bisogno, fornendo al contempo la struttura dati unificata necessaria per governare l&#39;ambiente nel tempo.

* **Riconosci la realtà**: i team indipendenti sviluppano naturalmente i propri processi, che spesso rimangono nascosti in fogli di calcolo isolati. La transizione a Protezione file Windows non crea problemi, ma accende la luce su quella già esistente. Rendendo questi processi visibili in un ambiente condiviso, è possibile collocarli in un unico punto in cui possono essere infine affrontati e migliorati.

* **Segnale di avanzamento**: quando un team richiede i propri campi, non si tratta di &quot;espansione&quot;, ma di **Adozione**. Significa che vedono WFP come il loro spazio di lavoro.

* **Gestisci debito, non nasconderlo**: è naturale preoccuparsi dello sforzo necessario per ripulire tassonomie divergenti in un secondo momento. Tuttavia, l’alternativa, ovvero l’imposizione di standard rigorosi troppo presto, spesso spinge i team a tornare ai fogli di calcolo dove i processi (e il debito) rimangono nascosti. Consentendo ai team di iniziare in WFP con le classificazioni correnti, si sposta il debito in un ambiente visibile e gestito. Questo rende l&#39;eventuale riconciliazione un&#39;attività iterativa piuttosto che un singolo progetto di migrazione.



## &#x200B;3. Il modello di governance &quot;Lanes on a Road&quot;

Scalabilità senza debiti attraverso la definizione di &quot;corsie globali&quot; e &quot;spazi di gioco locali&quot;.



### A. Le corsie globali

* **Oggetti controllati**: oggetti che ogni team deve utilizzare per il reporting aziendale (ad esempio, `Strategic Pillar`, `Region`, `Fiscal Quarter`).

* **Gestito Da**: L&#39;Amministratore Centrale Coe/Marketing Ops.

* **Regola**: questi campi sono &quot;condivisi&quot; e obbligatori.



### B. Sui Luoghi Locali (Spokes)

* **Oggetti sperimentali**: campi o tipi di record specifici per le esigenze tattiche di un team (ad esempio, `Influencer Handle` di un team social o `URL Slug` di un team Web).

* **Gestito da**: il lead del team (con indicazioni leggere).

* **Regola**: i team possono innovare qui. Se un campo &quot;Locale&quot; viene adottato da più di 3 team, viene &quot;Promosso&quot; a una corsia globale.



## &#x200B;4. Il Paradosso Della Governance: Prima I Team, Seguono Gli Standard

Una sfida comune nella scalabilità di WFP sta decidendo quale delle due viene prima: **Enterprise Governance** o **Allineamento operativo team**.



Riteniamo che il modo più efficace per risolvere questo problema sia riconoscere che il valore aziendale è costruito su una strada bidirezionale:

1. **I team hanno bisogno di rilevanza**: l&#39;azienda realizza valore solo quando i suoi team sono in esecuzione attiva. Pertanto, la governance deve **servire i team** fornendo una struttura che supporti le loro esigenze operative note.

2. **L&#39;azienda ha bisogno di visibilità**: la leadership può prendere decisioni informate solo quando i dati sono sufficientemente puliti per essere aggregati. Pertanto, i team devono **servire l&#39;azienda** fornendo i metadati minimi validi necessari per la visibilità del portfolio.



L&#39;obiettivo della &quot;scalabilità gestita&quot; è trovare l&#39;intersezione tra queste due esigenze, standardizzando abbastanza da fornire visibilità, ma non tanto da bloccare l&#39;esecuzione del team.



### A. Allineamento delle priorità: dati e visualizzazione

Quando esegui il ridimensionamento, considera che la definizione di &quot;Valore&quot; differisce tra gli utenti tipo:

* **L&#39;amministratore/proprietario prodotto**: valori **tassonomie e classificazioni unificate**. L’obiettivo è un’architettura dei dati pulita che supporti la scalabilità a lungo termine.

* **Interessato/Leader**: valori **visualizzazione e insight** (ad esempio, un calendario globale o una sequenza temporale Portfolio). Il loro obiettivo è il &quot;Momento di Fulmine&quot; che rende i dati fruibili.



**Strategia**: utilizza l&#39;esigenza di visualizzazione delle parti interessate come *incentivo* per la conformità del team con l&#39;esigenza dell&#39;amministratore di rispettare gli standard dei dati. Ottenete la tassonomia unificata distribuendo il &quot;Super Calendar&quot; richiesto dalla leadership.



### B. La Fase Di Osservazione &quot;Guidata Dai Servizi&quot;

Durante la scalabilità iniziale, il ruolo dell’amministratore è quello di facilitare questo scambio tra i team e l’azienda.

* **Assegna priorità all&#39;operazione rispetto alla standardizzazione**: è preferibile che i team pianifichino attivamente nelle aree di lavoro in silos piuttosto che bloccarli a causa della mancanza di definizioni globali. Questa attività è costituita dai &quot;dati grezzi&quot; necessari per creare standard salutari e reali.

* **Identificare i &quot;Minimi di visibilità&quot;**: utilizzare i responsabili per identificare i 3-5 campi che *devono* essere puliti per i report aziendali (ad esempio, `Strategic Alignment`, `Start Date`, `Budget`). Concentrare l&#39;energia di applicazione SOLO qui.



### B. Armonizzazione retroattiva (Governance as a Service)

Quando emerge un modello di &quot;esigenze note&quot; tra i team, l’azienda può consolidare tali modelli in un servizio globale.

1. **Osserva modelli riusciti**: identifica le tassonomie &quot;vincenti&quot; che i team hanno già creato e adottato.

2. **Collaborative Handshake**: riunisci i campioni del team per perfezionare i loro successi locali in uno standard aziendale condiviso.

3. **Distribuisci come servizio**: esegui il rollout delle nuove corsie globali non come &quot;restrizione&quot;, ma come modo per semplificare la generazione di rapporti e l&#39;allineamento tra team per le persone che svolgono il lavoro.



**Eliminazione delle chiavi**: la governance deve essere una risposta al successo operativo, non un prerequisito.



## &#x200B;5. Meccanica di scala: il modello di crescita basato su modelli

L’applicazione di questa filosofia richiede un approccio attento alla struttura dei dati. Per evitare una &quot;espansione della governance&quot;, resistere all&#39;urgenza di creare campi globali per ogni singola richiesta. Utilizza invece il **percorso di maturità del campo** per consentire l&#39;utilizzo reale degli standard aziendali:



1. **Livello 1: esperimento locale**: il team A crea un campo personalizzato nella propria area di lavoro.

2. **Livello 2: Riconoscimento pattern**: l&#39;amministratore informa che i team B e C utilizzano o richiedono un campo simile.

3. **Livello 3: Standardizzazione organizzazione**: l&#39;amministratore crea una singola versione standardizzata del campo come tipo di record nel **Workspace di tassonomia globale** e la invia in syndication ai team.



### La meccanica del &quot;pensionamento morbido&quot;

Poiché WFP non dispone attualmente di una funzione di &quot;archiviazione&quot; nativa per i campi, il ritiro di un campo locale richiede un processo di &quot;pensionamento morbido&quot; intenzionale per preservare i dati storici senza complicare l’interfaccia utente:



1. **Migrazione dati**: utilizzare una vista tabella (o Fusion) per copiare in blocco i valori dal campo &quot;Shadow&quot; locale nel nuovo campo Corsia globale. Assicurati che i dati siano convalidati e puliti durante questo spostamento.

2. **Rinomina per elementi obsoleti**: rinomina il campo locale con un prefisso come `[DEPRECATED]` o `z_` (ad esempio `z_Language (Old)`). Questo spinge il campo alla base dei selettori di campo e segnala agli utenti che non è più il &quot;Source of Truth&quot;.

3. **Rimozione modulo**: **Questo è il passaggio più critico.** Rimuovere il campo obsoleto da tutti i **Record Forms**. In questo modo si impedisce l’immissione di nuovi dati mantenendo visibili i dati precedenti nelle viste tabella o nei rapporti esistenti, se necessario.

4. **Periodo di interruzione**: mantenere il campo obsoleto (prefisso e non in formato) per 30-60 giorni per assicurarsi che nessun dato sia stato perso durante la migrazione. Dopo questo periodo, se i dati sono completamente riconciliati nella Corsia globale, il campo locale può essere eliminato dall’area di lavoro.



## &#x200B;6. Evitare la &quot;deriva di base&quot; (la regola di astrazione)

Per evitare che la pianificazione si accumuli come core:

* **Livello astrazione**: ogni campo in Protezione file Windows deve rispondere a **Domanda strategica**. Se un campo viene utilizzato solo per il tracciamento tattico (ad esempio, &quot;Questa bozza è stata approvata?&quot;), mantienilo in Core.

* **Primo consolidamento**: se un team desidera un nuovo campo di metadati, invitarlo a controllare prima la tassonomia globale. È necessario concedere ai lead del team **l&#39;accesso in sola lettura** all&#39;area di lavoro tassonomia globale (vedere la sezione 7). Mappando le loro esigenze tattiche su un campo strategico esistente, evitate inutili duplicazioni e mantenete l&#39;integrità dei rapporti.



## &#x200B;7. Modello di visibilità &quot;Accesso in sola lettura&quot;

Risolvere la sensazione di &quot;Siloed&quot; senza il rumore del lavoro &quot;Siloed&quot;.

* **Il problema**: i team in spoke si sentono isolati perché visualizzano solo i propri record.

* **Correzione**: concedere ai team **l&#39;accesso in sola lettura alle aree di lavoro designate come &#39;Primarie&#39; per i tipi di record condivisi**.

* **Risultato**: possono visualizzare il contesto aziendale più ampio per l&#39;ispirazione e l&#39;allineamento, ma la loro area di lavoro locale rimane pulita e focalizzata sulle loro attività specifiche.



## &#x200B;8. Gestire la crescita attraverso workshop

Il potenziamento del PAM è una sfida culturale quanto tecnica. Organizzare workshop mirati per colmare il &quot;divario di governance&quot;.



### A. Il workshop di scoperta del &quot;pasticcio necessario&quot;

* **Pubblico**: responsabili marketing regionali e campioni di operazioni.

* **Obiettivo**: documentare la &quot;Siloed Reality&quot; corrente (i dati operativi frammentati).

* **Messaggio**: &quot;Non siamo qui per eliminare i tuoi campi. Siamo qui per capire come si collegano alla strategia globale.&quot;

* **Risultato**: bozza di mappatura dei campi tattici locali su corsie strategiche globali.



### B. La sessione di allineamento &quot;Visibilità strategica&quot;

* **Pubblico**: soggetti interessati al marketing di alto livello (leadership).

* **Obiettivo**: riformulare l&#39;ansia &quot;Semplifica prima&quot;.

* **Messaggio**: &quot;Non è necessaria una tassonomia perfetta per iniziare. Stiamo utilizzando WFP come ambiente per *compilare* la tassonomia perfetta.&quot;

* **Risultato**: approvazione per l&#39;avanzamento con Protezione file Windows come motore di riconciliazione mentre Core rimane nello stato corrente.



### C. La vetrina &quot;Spoke-to-Global&quot;

* **Pubblico**: nuovi team esplorano WFP.

* **Obiettivo**: riduci la sensazione di &quot;silos&quot;.

* **Messaggio**: &quot;Vedere come il lavoro locale del Team A alimenta automaticamente il Workspace primario designato? Puoi avere la stessa visibilità anche per il tuo lavoro.&quot;

* **Risultato**: consenso da parte di nuovi dipartimenti che vedono il vantaggio di essere &quot;connessi&quot; senza perdere la loro indipendenza locale.



### D. Orario &quot;Assistenza continua&quot;

* **Pubblico**: tutti gli utenti WFP (correnti e potenziali).

* **Obiettivo**: fornisci un ambiente ricorrente e a bassa posta per la risoluzione dei problemi e indicazioni tattiche.

* **Messaggio**: &quot;Non ci sono domande sbagliate. Siamo a tua disposizione per aiutarti a risolvere in tempo reale le tue specifiche sfide di pianificazione&quot;.

* **Risultato**: maggiore fiducia degli utenti, risoluzione più rapida degli attriti tecnici e identificazione di nuovi modelli che potrebbero richiedere una standardizzazione globale.



## &#x200B;9. Personale per la scala: ruoli e responsabilità

Il successo in un modello di scalabilità gestito richiede molto di più della semplice configurazione dello strumento; richiede una chiara distribuzione dei ruoli tra i team globali e spoke.



### A. L’architetto aziendale (Central COE/Marketing Ops)

* **Stato attivo**: integrità dell&#39;organizzazione, prestazioni del sistema e **tassonomia dei dati unificata**.

* **Responsabilità**:

   * Gestisce la **tassonomia globale Workspace**.

   * Facilita il **percorso di maturità del campo** (promozione dei successi locali agli standard globali).

   * Mantiene le **visualizzazioni primarie di Workspace** per i report esecutivi.

   * Lead il **controllo semantico** mensile tra le aree di lavoro.



### B. Il campione parlato (proprietario processo team)

* **Focus**: rilevanza del team e velocità di adozione.

* **Responsabilità**:

   * Funge da punto di contatto unico per il team funzionale.

   * È il proprietario della struttura dell’area di lavoro locale e degli esperimenti sui campi personalizzati.

   * Assicura che il team utilizzi il **gateway gestito** (Forms) per l&#39;immissione dei dati.

   * Partecipa a **Collaborative Handshake** durante l&#39;armonizzazione.



### C. Lo Sponsor Esecutivo (Leadership Marketing)

* **Focus**: allineamento strategico, visibilità OKR e visualizzazione **portfolio (ad esempio, Calendaring globale)**.

* **Responsabilità**:

   * Definisce l&#39;organizzazione **OKR marketing** nell&#39;area di lavoro tassonomia globale.

   * Promuove il valore di &quot;Visibility Step 1&quot; per altri leader.

   * Rafforza l’allocazione delle risorse 80/20 (valore rispetto alla pulizia).



### D. Lead di abilitazione (Gestione modifiche)

* **Obiettivo**: spostamento culturale e sviluppo delle competenze.

* **Responsabilità**:

   * Ospita **Office Hours** e **Workshop di individuazione** ricorrenti.

   * Mantiene la vetrina &quot;Success Story&quot; interna.

   * Identifica i punti di attrito tecnici che Enterprise Architect deve risolvere.



## &#x200B;10. Elenco di controllo per il ridimensionamento del team successivo

* [ ] **Identificare il campione**: chi è il &quot;Proprietario del processo&quot; o &quot;Campione&quot; di questo nuovo team?

* [ ] **Definisci il &quot;Delta locale&quot;**: quali 2-3 campi sono necessari al team perché lo standard globale non fornisce attualmente?

* [ ] **Mappa su percorsi globali**: quali campi globali esistenti possono soddisfare l&#39;80% delle loro esigenze?

* [ ] **Concedi visibilità globale**: concedi loro l&#39;accesso in sola lettura alle aree di lavoro primarie e all&#39;area di lavoro di tassonomia globale il giorno 1.

* [ ] **Stabilire l&#39;handoff**: in che modo il loro lavoro &quot;alimenta&quot; le aree di lavoro primarie pertinenti? (ad esempio, tramite un tipo di record globale o una ricerca specifica).

<!--original content: 

**Version**: 1.0 

**Context**: "We've landed our first use case, and now everyone wants in." 

 

## 1. The "Success Trap" 

Sometimes it can feel like the most dangerous phase of WFP adoption is immediately after the first successful use case or POC. Enthusiasm is high, but the fear of "technical debt" and "administrative sprawl" can lead to two equally damaging responses: 

1.  **Over-Governance**: Locking down the system so tightly that new teams revert to spreadsheets. 

2.  **Zero-Governance**: Letting every team create their own fields and record types, recreating the fragmented metadata sprawl found in legacy environments. 

 

## 2. The Core Philosophy: WFP as the "Reconciliation Engine" 

Instead of trying to stop teams from being different, we position WFP as the place where those differences are **made visible so they can be reconciled**. 

 

*   **Managing Adoption Velocity**: It is natural to feel cautious about expanding into a new tool before "cleaning up" existing environments. While choosing to **Simplify First** provides a highly governed foundation, it can delay time-to-value for teams ready to align. We believe the most effective way to lead through this change is to recognize that **visibility is Step 1**. Momentum toward a shared, enterprise-ready tool (moving away from the sprawl of PPTs and spreadsheets) is what ultimately unblocks long-term goals.  

 

    **Recommendation**: Instead of a "Clean Up First" mandate, we recommend allocating a smaller portion of resources to ongoing maintenance and a significantly larger portion to solving pressing business needs. For example, spending a year solely on "cleaning up" taxonomies yields little incremental value. However, delivering **cross-team visibility** (e.g., through a Unified Enterprise Calendar or a consolidated GTM roadmap) provides the transformative value your stakeholders need, while providing the unified data structure you need to govern the environment over time. 

*   **Acknowledge the Reality**: Independent teams naturally develop their own processes, which often stay hidden in siloed spreadsheets. Transitioning to WFP doesn't create a mess; it shines a light on the one that already exists. By making these processes visible in a shared environment, you put them in the one place where they can finally be addressed and improved. 

*   **The Progress Signal**: When a team asks for their own fields, it's not "sprawl"—it's **Adoption**. It means they see WFP as their workspace. 

*   **Manage Debt, Don't Hide It**: It is natural to be concerned about the effort required to clean up divergent taxonomies later. However, the alternative—forcing strict standards too early—often drives teams back to spreadsheets where their processes (and their debt) remain hidden. By allowing teams to begin in WFP with their current classifications, you are moving that debt into a visible, governed environment. This makes the eventual reconciliation an iterative task rather than a single, overwhelming migration project. 

 

## 3. The "Lanes on a Road" Governance Model 

Scale without debt by defining "Global Lanes" and "Local Playgrounds." 

 

### A. The Global Lanes 

*   **Controlled Objects**: Objects that every team must use for enterprise reporting (e.g., `Strategic Pillar`, `Region`, `Fiscal Quarter`). 

*   **Managed By**: The Central COE/Marketing Ops Admin. 

*   **Rule**: These fields are "Shared" and mandatory. 

 

### B. The Local Playgrounds (Spokes) 

*   **Experimental Objects**: Fields or record types specific to a team's tactical needs (e.g., a Social team's `Influencer Handle` or a Web team's `URL Slug`). 

*   **Managed By**: The Team Lead (with light guidance). 

*   **Rule**: Teams can innovate here. If a "Local" field is adopted by >3 teams, it is "Promoted" to a Global Lane. 

 

## 4. The Governance Paradox: Teams First, Standards Follow 

A common challenge in scaling WFP is deciding which comes first: **Enterprise Governance** or **Team Operational Alignment**.  

 

We believe the most effective way to navigate this is to recognize that enterprise value is built on a two-way street: 

1.  **Teams need relevance**: The enterprise only realizes value when its teams are actively executing. Therefore, governance must **serve the teams** by providing structure that supports their known operational needs. 

2.  **The Enterprise needs visibility**: Leadership can only make informed decisions when data is clean enough to aggregate. Therefore, the teams must **serve the enterprise** by providing the minimum viable metadata required for portfolio visibility. 

 

The goal of "Managed Scaling" is to find the intersection of these two needs—standardizing enough to provide visibility, but not so much that you stall team execution. 

 

### A. Aligning Priorities: Data vs. Visualization 

When scaling, recognize that the definition of "Value" differs between personas: 

*   **The Admin/Product Owner**: Values **unified taxonomies and classifications**. Their goal is a clean data architecture that supports long-term scalability. 

*   **The Stakeholder/Leader**: Values **visualization and insight** (e.g., a Global Calendar or a Portfolio Timeline). Their goal is the "Lightning Moment" that makes the data actionable. 

 

**The Strategy**: Use the stakeholder's need for visualization as the *incentive* for the team's compliance with the admin's need for data standards. You get the unified taxonomy by delivering the "Super Calendar" that leadership demands. 

 

### B. The "Service-Led" Observation Phase 

During early scale-up, the Admin's role is to facilitate this exchange between teams and the enterprise. 

*   **Prioritize Operation over Standardization**: It is better to have teams actively planning in siloed workspaces than to have them stalled by a lack of global definitions. This activity is the "raw data" required to build healthy, real-world standards. 

*   **Identify the "Visibility Minimums"**: Work with leadership to identify the 3-5 fields that *must* be clean for enterprise reporting (e.g., `Strategic Alignment`, `Start Date`, `Budget`). Focus your enforcement energy ONLY here. 

 

### B. Retroactive Harmonization (Governance as a Service) 

Once a pattern of "known needs" emerges across teams, the enterprise can move to consolidate those patterns into a global service. 

1.  **Observe Successful Patterns**: Identify the "winning" taxonomies that teams have already built and adopted. 

2.  **The Collaborative Handshake**: Bring team champions together to refine their local successes into a shared enterprise standard. 

3.  **Deploy as a Service**: Roll out the new global lanes not as a "restriction," but as a way to simplify reporting and cross-team alignment for the people doing the work. 

 

**Key Takeaway**: Governance should be a response to operational success, not a prerequisite for it.  

 

## 5. Scaling Mechanics: The Pattern-Based Growth Model 

Applying this philosophy requires a thoughtful approach to data structure. To avoid "Governance Sprawl," resist the urge to build global fields for every individual request. Instead, use the **Field Maturity Path** to let real-world usage guide your enterprise standards: 

 

1.  **Level 1: Local Experiment**: Team A creates a custom field in their workspace. 

2.  **Level 2: Pattern Recognition**: The Admin notices Teams B and C are using or asking for a similar field. 

3.  **Level 3: Enterprise Standardization**: The Admin creates a single, standardized version of that field as a record type in the **Global Taxonomy Workspace** and syndicates it to teams. 

 

### The Mechanics of "Soft Retirement" 

Because WFP does not currently have a native "Archive" feature for fields, retiring a local field requires a deliberate "Soft Retirement" process to preserve historical data without cluttering the UI: 

 

1.  **Data Migration**: Use a table view (or Fusion) to bulk-copy values from the local "Shadow" field into the new Global Lane field. Ensure the data is validated and cleaned during this move. 

2.  **Rename for Deprecation**: Rename the local field with a prefix like `[DEPRECATED]` or `z_` (e.g., `z_Language (Old)`). This pushes the field to the bottom of field pickers and signals to users that it is no longer the "Source of Truth." 

3.  **Form Removal**: **This is the most critical step.** Remove the deprecated field from all **Record Forms**. This prevents new data from being entered while keeping the old data visible in existing table views or reports if needed. 

4.  **The "Sunset" Period**: Keep the deprecated field (prefixed and off-form) for 30-60 days to ensure no data was missed during migration. After this period, if the data is fully reconciled in the Global Lane, the local field can be deleted from the workspace. 

 

## 6. Avoiding the "Core Drift" (The Abstraction Rule) 

To prevent Planning from becoming as cluttered as Core: 

*   **The Abstraction Layer**: Every field in WFP should answer a **Strategic Question**. If a field is only used for tactical tracking (e.g., "Was this proof approved?"), keep it in Core. 

*   **Consolidation First**: If a team wants a new metadata field, invite them to check the Global Taxonomy first. This requires granting team leads **Read-Only access** to the Global Taxonomy workspace (see Section 7). By mapping their tactical needs to an existing strategic field, you prevent unnecessary duplication and maintain reporting integrity. 

 

## 7. The "Read-Only Access" Visibility Model 

Solve the "Siloed" feeling without the noise of "Siloed" work. 

*   **The Problem**: Teams in spokes feel isolated because they only see their own records. 

*   **The Fix**: Grant teams **Read-Only access to the workspaces designated as 'Primary' for those shared record types**.  

*   **The Result**: They can see the broader enterprise context for inspiration and alignment, but their local workspace remains clean and focused on their specific tasks. 

 

## 8. Managing Growth through Workshops 

Scaling WFP is as much a cultural challenge as a technical one. Use targeted workshops to bridge the "Governance Gap." 

 

### A. The "Necessary Mess" Discovery Workshop 

*   **Audience**: Regional Marketing Leads and Ops Champions. 

*   **Goal**: Document the current "Siloed Reality" (the fragmented operational data). 

*   **The Message**: "We aren't here to delete your fields. We're here to understand how they link to the global strategy." 

*   **Outcome**: A draft mapping of local tactical fields to global strategic lanes. 

 

### B. The "Strategic Visibility" Alignment Session 

*   **Audience**: High-level Marketing Stakeholders (leadership). 

*   **Goal**: Reframe the "Simplify First" anxiety. 

*   **The Message**: "We don't need a perfect taxonomy to start. We are using WFP as the environment to *build* the perfect taxonomy." 

*   **Outcome**: Approval to move forward with WFP as the reconciliation engine while Core remains in its current state. 

 

### C. The "Spoke-to-Global" Showcase 

*   **Audience**: New teams exploring WFP. 

*   **Goal**: Reduce the "siloed" feeling. 

*   **The Message**: "See how Team A's local work automatically feeds the designated Primary Workspace? You can have that same visibility for your work too." 

*   **Outcome**: Opt-in from new departments who see the benefit of being "connected" without losing their local independence. 

 

### D. The "Ongoing Support" Office Hours 

*   **Audience**: All WFP users (current and prospective). 

*   **Goal**: Provide a recurring, low-stakes environment for troubleshooting and tactical guidance. 

*   **The Message**: "There are no wrong questions. We are here to help you solve your specific planning challenges in real-time." 

*   **Outcome**: Increased user confidence, faster resolution of technical friction, and the identification of new patterns that might warrant global standardization. 

 

## 9. Staffing for Scale: Roles and Responsibilities 

Success in a managed scaling model requires more than just tool configuration; it requires a clear distribution of roles across the Global and Spoke teams. 

 

### A. The Enterprise Architect (Central COE/Marketing Ops) 

*   **Focus**: Enterprise integrity, system performance, and **unified data taxonomy**. 

*   **Responsibilities**: 

    *   Manages the **Global Taxonomy Workspace**. 

    *   Facilitates the **Field Maturity Path** (promoting local successes to global standards). 

    *   Maintains the **Primary Workspace** views for executive reporting. 

    *   Leads the monthly **Semantic Audit** across workspaces. 

 

### B. The Spoke Champion (Team Process Owner) 

*   **Focus**: Team relevance and adoption velocity. 

*   **Responsibilities**: 

    *   Acts as the single point of contact for the functional team. 

    *   Owns the local workspace structure and custom field experiments. 

    *   Ensures the team uses the **Governed Gateway** (Forms) for data entry. 

    *   Participates in the **Collaborative Handshake** during harmonization. 

 

### C. The Executive Sponsor (Marketing Leadership) 

*   **Focus**: Strategic alignment, OKR visibility, and **portfolio visualization (e.g., Global Calendaring)**. 

*   **Responsibilities**: 

    *   Defines the enterprise **Marketing OKRs** in the Global Taxonomy workspace. 

    *   Champions the value of "Visibility Step 1" to other leaders. 

    *   Reinforces the 80/20 resource allocation (Value over Cleanup). 

 

### D. The Enablement Lead (Change Management) 

*   **Focus**: Cultural shift and skill development. 

*   **Responsibilities**: 

    *   Hosts recurring **Office Hours** and **Discovery Workshops**. 

    *   Maintains the internal "Success Story" showcase. 

    *   Identifies technical friction points for the Enterprise Architect to resolve. 

 

## 10. Checklist for Scaling the Next Team 

* [ ] **Identify the Champion**: Who is the "Process Owner" or "Champion" of this new team? 

* [ ] **Define the "Local Delta"**: What 2-3 fields does this team need that the Global standard doesn't currently provide? 

* [ ] **Map to Global Lanes**: Which existing Global fields can satisfy 80% of their needs? 

* [ ] **Grant Global Visibility**: Give them Read-Only access to the relevant Primary Workspaces and the Global Taxonomy workspace on Day 1. 

* [ ] **Establish the Handoff**: How does their work "feed" the relevant Primary Workspaces? (e.g., via a Global Record Type or a specific lookup).

-->