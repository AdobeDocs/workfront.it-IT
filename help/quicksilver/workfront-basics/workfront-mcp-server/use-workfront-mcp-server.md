---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Utilizzare il server MCP di Adobe Workfront
description: Utilizza il server MCP di Adobe Workfront per cercare, creare, aggiornare e gestire elementi Workfront tramite conversazione in linguaggio naturale in un assistente AI.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '1243'
ht-degree: 2%

---


# Utilizzare il server MCP di Adobe Workfront

Il server MCP [!DNL Adobe Workfront] ti consente di trovare, creare, aggiornare e gestire gli elementi di Workfront chiedendo a un assistente AI in inglese semplice. L’assistente AI decide quali azioni Workfront chiamare e gestisce la conversazione con Workfront per te.

[!DNL Claude] è attualmente l&#39;unico assistente di intelligenza artificiale supportato, ma gli esempi e i modelli contenuti in questo articolo si applicano a qualsiasi assistente di intelligenza artificiale che supporta il server MCP di Workfront.

Questo articolo presuppone che la connessione sia già stata impostata. Per informazioni sulla configurazione, vedere [Configurare il server Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md). Per ulteriori informazioni sul server Workfront MCP, vedere [Panoramica del server Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).



## Azioni disponibili tramite il server Workfront MCP

Il server MCP di Workfront copre le azioni relative alle approvazioni, alla pianificazione e al flusso di lavoro.

<!-- NEEDS DETAIL: Confirm the full inventory of actions exposed through the Workfront MCP server. The five core actions below are confirmed from Hamilton's walkthrough. The approvals, planning, and workflow sections need to be filled in from Jeff's engineering channel post, hands-on access, and the deck Oznur published in the MCP external channel. -->

>[!IMPORTANT]
>
>Un assistente AI opera in Workfront utilizzando il tuo account e le tue autorizzazioni Workfront. Tu e il provider di assistenti AI siete responsabili delle azioni che l’assistente AI compie per tuo conto. Prima di procedere, conferma cosa sta per fare l’assistente AI.


## Responsabilità per le azioni dell’assistente di IA

Quando colleghi un assistente di IA a Workfront, l’assistente di IA agisce in Workfront utilizzando il tuo account e le tue autorizzazioni Workfront. Le azioni dell’assistente AI hanno lo stesso effetto delle azioni eseguite direttamente nell’interfaccia di Workfront.

Tu e il provider di assistenti AI siete responsabili delle azioni che l’assistente AI compie in Workfront. Adobe non è responsabile delle modifiche apportate dall’assistente AI ai dati Workfront.

Prima di consentire all’assistente AI di procedere con una richiesta, conferma di comprendere cosa intende fare, in particolare per le azioni che modificano o eliminano i dati.

### Azioni di base

Il server MCP di Workfront include le azioni di base seguenti:

| Azione | Funzionamento |
|---|---|
| Crea | Crea nuovi elementi in Workfront. |
| Ricerca | Trova e recupera elementi da Workfront. |
| Aggiorna | Modifica gli elementi esistenti in Workfront. |
| Elimina | Rimuove gli elementi da Workfront. |
| Risolvi nomi campi | Cerca i nomi dei campi Workfront corretti in modo che l’assistente AI possa creare richieste precise in base ai tuoi dati. |

<!-- NEEDS DETAIL: Confirm which Workfront object types are supported across the core actions (projects, tasks, issues, portfolios, programs, custom forms, planning records, approvals, etc.). -->

### Azioni di approvazione

<!-- NEEDS DETAIL: List the approval-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request a marketer might make. -->

### Azioni di pianificazione

<!-- NEEDS DETAIL: List the planning-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

### Azioni del flusso di lavoro

<!-- NEEDS DETAIL: List the workflow-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

## Esempi di cosa chiedere

Dopo aver effettuato la connessione, digita le richieste in linguaggio naturale nell’assistente AI. L’assistente AI decide quali azioni Workfront chiamare e restituisce i risultati.

<!-- NEEDS DETAIL: Example prompts in this section are adapted from the Workflow Optimization Agent (WOA) examples doc on another branch. Validate each example against a working Claude + Workfront MCP server setup before publication, since WOA and the MCP server may expose different action inventories. -->

### Trovare e visualizzare il lavoro

Chiedi all’assistente AI di cercare in Workfront gli elementi che corrispondono a ciò che stai cercando. Ad esempio:

* *Mostra tutti i progetti attivi per il team Marketing marchio.*
* *Ottieni tutte le attività assegnate a Joan Harris.*
* *Mostra tutti i problemi nel progetto &quot;Riprogettazione sito Web&quot; nella categoria &quot;Tecnico&quot;.*

### Crea nuovi elementi

Chiedi all’assistente AI di creare progetti, attività o altri elementi di Workfront. Ad esempio:

* *Crea un progetto vuoto denominato &quot;Q2 Innovation Sandbox&quot; a partire dal 10 marzo e fino al 30 aprile. Imposta come proprietario.*
* *Aggiungi al progetto una nuova attività denominata &quot;Controllo di qualità pagina di destinazione&quot; e pianificala dal 22 aprile al 26 aprile.*
* *Crea un nuovo record della campagna denominato &quot;Vendita estiva 2026.&quot;*

### Aggiorna elementi esistenti

Chiedi all’assistente AI di apportare modifiche agli elementi già in Workfront. Ad esempio:

* *Aggiorna l&#39;attività &quot;Design Review&quot; in modo che termini il 18 aprile e assegnala al team creativo.*
* *Per il progetto &quot;Lucent AI Launch - NA&quot;, esegui il push della fine a metà aprile e aumenta il budget a 150.000 dollari.*
* *Aggiorna il campo del budget nel record &quot;Campagna estiva&quot; a $75.000.*

### Elimina elementi

Chiedi all’assistente AI di rimuovere gli elementi Workfront. Ad esempio:

* *Eliminare il progetto denominato &quot;Campagna test Q1&quot;*
* *Rimuovi l&#39;attività &quot;Produzione risorse di stampa&quot; dal progetto.*
* *Elimina il record della campagna denominato &quot;Old Promo&quot;*

>[!WARNING]
>
>L’eliminazione di elementi in Workfront tramite un assistente AI equivale all’eliminazione nell’interfaccia di Workfront. Prima di procedere, conferma cosa sta per eliminare l’assistente AI.

### Utilizzare le approvazioni

Chiedi all’assistente AI di gestire le approvazioni di documenti e risorse. Ad esempio:

* *Aggiungere Sarah Chen e Miguel Alvarez come approvatori nel documento corrente.*
* *Invia un promemoria agli approvatori della risorsa &quot;Video campagna di primavera&quot; che non hanno risposto.*
* *Applica il modello di approvazione &quot;Lancio di marketing&quot; alla risorsa &quot;Video della campagna primaverile.&quot;*

<!-- NEEDS DETAIL: Add approvals-specific context from the WOA examples doc, including: content approvals must be enabled for the organization, the AI assistant cannot approve or reject on behalf of humans (except via the Workfront AI Reviewer), and best experience is with the Unified Approvals experience. -->

### Utilizzare i record di Planning

Chiedi all’assistente AI di gestire i record di pianificazione. Ad esempio:

* *Crea un nuovo record di pianificazione denominato &quot;Piano di marketing Q2&quot; per il team di marketing del marchio.*
* *Aggiungi al record di pianificazione una nuova attività denominata &quot;Audit social media&quot;.*
* *Aggiorna l&#39;attività &quot;Audit social media&quot; in modo che termini il 18 aprile e assegnala al team creativo.*

### Utilizzare il flusso di lavoro

Chiedi all’assistente AI di gestire il flusso di lavoro. Ad esempio:

* *Indirizza il progetto &quot;Q2 Innovation Sandbox&quot; alla Commissione per la valutazione dell&#39;innovazione.*
* *Aggiornare il record &quot;Campagna estiva&quot; allo stato &quot;Pronto per il lancio&quot;.*
* *Approva il record &quot;Campagna estiva&quot;.*


### Incatenare le richieste in una conversazione

Puoi concatenare le richieste in una singola conversazione. L’assistente AI mantiene il contesto, in modo che ogni richiesta possa basarsi su quella precedente. Ad esempio:

1. Chiedi all&#39;assistente AI di trovare un set di elementi: *Trova le attività scadute.*
1. Quando l&#39;assistente AI restituisce l&#39;elenco, chiedere di agire sui risultati: *Aggiorna tutti i risultati al venerdì successivo.*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## Considerazioni

Quando utilizzi il server MCP di Workfront, tieni presenti le seguenti considerazioni.

### L’assistente AI può utilizzare informazioni precedenti nella conversazione

Gli assistenti AI a volte riutilizzano i dati di precedenti conversazioni invece di chiedere a Workfront l’ultima versione. Se è cambiato qualcosa in Workfront dall’ultima ricerca dell’assistente di intelligenza artificiale, potresti visualizzare informazioni obsolete.

Per forzare l’assistente AI a recuperare i dati aggiornati, richiedilo esplicitamente. Ad esempio:

* *Scarica i dati più recenti da Workfront. Non utilizzare i risultati memorizzati nella cache.*

### Il server Workfront MCP viene aggiornato automaticamente

Quando Adobe rilascia una nuova versione del server Workfront MCP, l’assistente AI utilizza automaticamente la nuova versione. Non è necessario riconnettersi o cambiare nulla dalla propria parte.

## Dati e sicurezza

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI assistant. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI assistant provider, what happens to it after the conversation ends, and any differences between AI assistants (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### Quali dati lasciano Workfront

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI assistant (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### Gestione dei dati Workfront da parte dei provider di assistenti AI

<!-- NEEDS DETAIL: For each supported AI assistant, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### Differenze tra gli assistenti AI

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI assistant handles Workfront data once additional AI assistants are supported. -->

## Risolvere i problemi relativi all’uso quotidiano

Per ulteriori informazioni sui problemi di installazione e autenticazione, vedere [Risoluzione dei problemi di installazione e autenticazione](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) in [Configurazione del server Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

| Problema | Probabile causa | Correggi |
|---|---|---|
| L’assistente AI ti sta fornendo informazioni obsolete. | L’assistente AI sta riutilizzando i dati di una fase precedente della conversazione. | Chiedi all’assistente AI di recuperare i dati aggiornati da Workfront. |
| L’assistente AI ha restituito dati dagli elementi Workfront errati. | L’assistente AI ha scelto gli elementi errati in base a una formulazione ambigua. | Chiedi di nuovo con nomi, ID o filtri più specifici. |
| Un aggiornamento o una cancellazione non ha avuto effetto in Workfront. | L’assistente AI non ha ancora chiamato l’azione o le tue autorizzazioni non lo consentono. | Conferma con l’assistente AI l’esecuzione dell’azione, quindi controlla le autorizzazioni Workfront. |

<!-- NEEDS DETAIL: Add additional day-to-day troubleshooting scenarios discovered during hands-on testing. -->

## Domande frequenti

### Con quali elementi di Workfront posso lavorare tramite un assistente AI?

Tutti gli elementi a cui hai accesso in Workfront tramite i livelli di accesso e le autorizzazioni per gli oggetti.

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### I miei dati Workfront vengono inviati al provider di assistenza AI o memorizzati da loro?

Per ulteriori informazioni, vedere [Dati e sicurezza](#data-and-security) in questo articolo.

### Cosa succede quando viene rilasciata una nuova versione del server Workfront MCP?

Il server MCP viene aggiornato automaticamente. Non è necessario riconnettersi o modificare nulla.

### È necessario conoscere l&#39;API di Workfront per utilizzare il server Workfront MCP?

No. L’assistente AI traduce le richieste in linguaggio naturale nelle azioni Workfront corrette. Se conosci già l’API di Workfront, le azioni ti saranno familiari, ma non è un requisito.
