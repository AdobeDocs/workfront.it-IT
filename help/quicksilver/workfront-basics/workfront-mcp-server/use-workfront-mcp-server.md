---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Utilizzare il server MCP di Adobe Workfront
description: Utilizza il server MCP di Adobe Workfront per cercare, creare, aggiornare e gestire elementi Workfront tramite conversazioni in linguaggio naturale in una piattaforma di intelligenza artificiale.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 152486b7850e01f3de23f22bbe3729c5cd3d3aa2
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 0%

---


# Utilizzare il server MCP di Adobe Workfront

Il server MCP [!DNL Adobe Workfront] ti consente di trovare, creare, aggiornare e gestire elementi Workfront chiedendo a una piattaforma di agenti di intelligenza artificiale in inglese semplice. La piattaforma decide quali azioni Workfront chiamare e gestisce la conversazione con Workfront per te.

[!DNL Claude] è attualmente l&#39;unica piattaforma di IA agente supportata, ma gli esempi e i modelli riportati in questo articolo si applicano a qualsiasi piattaforma di IA agente che supporta il server MCP di Workfront.

Questo articolo presuppone che la connessione sia già stata impostata. Per informazioni sulla configurazione, vedere [Configurare il server Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md). Per ulteriori informazioni sul server Workfront MCP, vedere [Panoramica del server Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Strumenti disponibili

Il server MCP di Workfront espone un set di strumenti richiamati dalla piattaforma dell’agente di intelligenza artificiale per tuo conto, ad esempio strumenti per cercare in Workfront, creare elementi, aggiornare campi e gestire le approvazioni. Per l&#39;elenco completo dei riferimenti, raggruppati per area Workfront, vedere [Strumenti server MCP di Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

>[!IMPORTANT]
>
>Quando connetti una piattaforma di agenti di intelligenza artificiale a Workfront, agisce in Workfront utilizzando l’account e le autorizzazioni Workfront. Le azioni della piattaforma hanno lo stesso effetto delle azioni eseguite direttamente nell’interfaccia di Workfront.
>
>Tu e il provider di piattaforme AI agentic siete responsabili delle azioni che la piattaforma compie in Workfront. Adobe non è responsabile delle modifiche apportate dalla piattaforma AI ai dati Workfront.
>
>Prima di consentire alla piattaforma dell’agente di IA di procedere con una richiesta, conferma di comprendere cosa intende fare, in particolare per le azioni che modificano o eliminano i dati.


## Esempi di cosa chiedere

Dopo la connessione, digita le richieste in linguaggio naturale nella piattaforma dell’agente di intelligenza artificiale. La piattaforma per agenti di intelligenza artificiale decide quali azioni Workfront chiamare e restituisce i risultati.

### Trovare e visualizzare il lavoro

Per cercare in Workfront gli elementi che corrispondono a ciò che stai cercando, chiedi:

* *Mostra tutti i progetti attivi per il team Marketing marchio.*
* *Ottieni tutte le attività assegnate a Joan Harris.*
* *Mostra tutti i problemi nel progetto &quot;Riprogettazione sito Web&quot; nella categoria &quot;Tecnico&quot;.*

### Crea nuovi elementi

Per creare progetti, attività o altri elementi di Workfront, chiedi:

* *Crea un progetto vuoto denominato &quot;Q2 Innovation Sandbox&quot; a partire dal 10 marzo e fino al 30 aprile. Imposta come proprietario.*
* *Aggiungi al progetto una nuova attività denominata &quot;Controllo di qualità pagina di destinazione&quot; e pianificala dal 22 aprile al 26 aprile.*
* *Crea un nuovo record della campagna denominato &quot;Vendita estiva 2026.&quot;*

### Aggiorna elementi esistenti

Per apportare modifiche agli elementi già presenti in Workfront, chiedi:

* *Aggiorna l&#39;attività &quot;Design Review&quot; in modo che termini il 18 aprile e assegnala al team creativo.*
* *Per il progetto &quot;Lucent AI Launch - NA&quot;, esegui il push della fine a metà aprile e aumenta il budget a 150.000 dollari.*
* *Aggiorna il campo del budget nel record &quot;Campagna estiva&quot; a $75.000.*

### Elimina elementi

Per rimuovere gli elementi di Workfront, eseguire le operazioni seguenti:

* *Eliminare il progetto denominato &quot;Campagna test Q1&quot;*
* *Rimuovi l&#39;attività &quot;Produzione risorse di stampa&quot; dal progetto.*
* *Elimina il record della campagna denominato &quot;Old Promo&quot;*

>[!WARNING]
>
>L’eliminazione di elementi in Workfront tramite una piattaforma AI agente equivale all’eliminazione nell’interfaccia di Workfront. Prima di procedere, conferma cosa sta per eliminare la piattaforma dell’agente di intelligenza artificiale.

### Utilizzare le approvazioni

Per gestire le approvazioni di documenti e risorse, chiedi:

* *Aggiungere Sarah Chen e Miguel Alvarez come approvatori nel documento corrente.*
* *Invia un promemoria agli approvatori della risorsa &quot;Video campagna di primavera&quot; che non hanno risposto.*
* *Applica il modello di approvazione &quot;Lancio di marketing&quot; alla risorsa &quot;Video della campagna primaverile.&quot;*


### Utilizzare i record di Planning

Per gestire i record di pianificazione, eseguire le operazioni riportate di seguito.

* *Crea un nuovo record di pianificazione denominato &quot;Piano di marketing Q2&quot; per il team di marketing del marchio.*
* *Aggiungi al record di pianificazione una nuova attività denominata &quot;Audit social media&quot;.*
* *Aggiorna l&#39;attività &quot;Audit social media&quot; in modo che termini il 18 aprile e assegnala al team creativo.*

### Utilizzare il flusso di lavoro

Per gestire il flusso di lavoro, chiedi:

* *Indirizza il progetto &quot;Q2 Innovation Sandbox&quot; alla Commissione per la valutazione dell&#39;innovazione.*
* *Aggiornare il record &quot;Campagna estiva&quot; allo stato &quot;Pronto per il lancio&quot;.*
* *Approva il record &quot;Campagna estiva&quot;.*


### Incatenare le richieste in una conversazione

Puoi concatenare le richieste in una singola conversazione. La piattaforma dell’agente di intelligenza artificiale mantiene il contesto, in modo che ogni richiesta possa basarsi su quella precedente. Ad esempio:

1. Richiedi un set di elementi: *Trova le attività scadute.*
1. Dopo aver ricevuto l&#39;elenco, chiedere un&#39;azione sui risultati: *Aggiornarli tutti al venerdì successivo.*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## Considerazioni

Quando utilizzi il server MCP di Workfront, tieni presenti le seguenti considerazioni.

### La piattaforma dell’agente di IA può utilizzare informazioni precedenti nella conversazione

Le piattaforme basate sull’intelligenza artificiale a volte riutilizzano i dati precedenti in una conversazione, anziché chiedere a Workfront di usare la versione più recente. Se è cambiato qualcosa in Workfront dall’ultima visualizzazione della piattaforma dell’agente di intelligenza artificiale, potrebbero essere visualizzate informazioni obsolete.

Per forzare la piattaforma dell’agente di intelligenza artificiale a recuperare nuovi dati, richiedila esplicitamente. Ad esempio:

* *Scarica i dati più recenti da Workfront. Non utilizzare i risultati memorizzati nella cache.*

### Il server Workfront MCP viene aggiornato automaticamente

Quando Adobe rilascia una nuova versione del server Workfront MCP, la piattaforma dell’agente di intelligenza artificiale utilizza automaticamente la nuova versione. Non è necessario riconnettersi o cambiare nulla dalla propria parte.

## Dati e sicurezza

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI agentic platform. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI agentic platform provider, what happens to it after the conversation ends, and any differences between AI agentic platforms (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### Quali dati lasciano Workfront

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI agentic platform (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### Gestione dei dati Workfront da parte dei provider di piattaforme basate su IA

<!-- NEEDS DETAIL: For each supported AI agentic platform, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### Differenze tra le piattaforme di IA agente

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI agentic platform handles Workfront data once additional AI agentic platforms are supported. -->

## Risolvere i problemi relativi all’uso quotidiano

+++ Espandi per visualizzare suggerimenti per la risoluzione dei problemi relativi all’utilizzo quotidiano del server MCP di Workfront.

| Problema | Probabile causa | Correggi |
|---|---|---|
| La piattaforma dell’agente di intelligenza artificiale fornisce informazioni obsolete. | La piattaforma dell’agente di intelligenza artificiale sta riutilizzando i dati di precedenti momenti della conversazione. | Richiedi nuovi dati da Workfront. |
| La piattaforma dell’agente di intelligenza artificiale ha restituito dati dagli elementi Workfront errati. | La piattaforma dell’agente di intelligenza artificiale ha scelto gli elementi errati in base a una formulazione ambigua. | Chiedi di nuovo con nomi, ID o filtri più specifici. |
| Un aggiornamento o una cancellazione non ha avuto effetto in Workfront. | La piattaforma dell’agente di intelligenza artificiale non ha ancora chiamato l’azione o le tue autorizzazioni non lo consentono. | Conferma con la piattaforma dell’agente di intelligenza artificiale l’esecuzione dell’azione, quindi controlla le autorizzazioni Workfront. |

Per ulteriori informazioni sui problemi di installazione e autenticazione, vedere [Risoluzione dei problemi di installazione e autenticazione](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) in [Configurazione del server Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

+++

## Domande frequenti

+++ Espandi per visualizzare le domande frequenti sull’utilizzo del server MCP di Workfront.

### Con quali elementi di Workfront posso lavorare tramite una piattaforma di agenti di intelligenza artificiale?

Tutti gli elementi a cui hai accesso in Workfront tramite i livelli di accesso e le autorizzazioni per gli oggetti.

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### I miei dati Workfront vengono inviati al provider di piattaforme basate su IA o memorizzati da quest’ultimo?

Per ulteriori informazioni, vedere [Dati e sicurezza](#data-and-security) in questo articolo.

### Cosa succede quando viene rilasciata una nuova versione del server Workfront MCP?

Il server MCP viene aggiornato automaticamente. Non è necessario riconnettersi o modificare nulla.

### È necessario conoscere l&#39;API di Workfront per utilizzare il server Workfront MCP?

No. La piattaforma AI agentic traduce le richieste in linguaggio naturale nelle azioni Workfront giuste. Se conosci già l’API di Workfront, le azioni ti saranno familiari, ma non è un requisito.

+++
