---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Utilizzare il server MCP di Adobe Workfront
description: Utilizza il server MCP di Adobe Workfront per cercare, creare, aggiornare e gestire elementi Workfront tramite conversazioni in linguaggio naturale in una piattaforma di intelligenza artificiale.
author: Courtney
feature: Get Started with Workfront
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c042179c-157b-516d-b27c-e3bf303e8567
    internal-label: Get Started with Workfront
source-git-commit: 1043dde02b6d66f9a0d041846b74184013989764
workflow-type: tm+mt
source-wordcount: '2383'
ht-degree: 0%
---

# Utilizzare il server MCP di Adobe Workfront

Il server MCP [!DNL Adobe Workfront] ti consente di trovare, creare, aggiornare e gestire elementi Workfront chiedendo a una piattaforma di agenti di intelligenza artificiale in linguaggio naturale. La piattaforma decide quali azioni Workfront chiamare e gestisce la conversazione con Workfront per te.

## Prerequisiti

* È necessario impostare la connessione tra la piattaforma AI agente e il server MCP di Workfront. Per le istruzioni di installazione, vedere [Configurare il server Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).
* L’istanza di Workfront deve essere abilitata su Adobe Identity Management System (IMS).
* È necessario disporre di un account Workfront con il livello di accesso e le autorizzazioni di oggetto necessari per gli elementi che si desidera utilizzare.
* Per utilizzare MCP con Workfront Planning, l&#39;organizzazione deve essere inclusa in un pacchetto Workfront che includa Adobe Workfront Planning.

Questo articolo presuppone che la connessione sia già stata impostata. Per informazioni sulla configurazione, vedere [Configurare il server Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

## Strumenti disponibili

Il server MCP di Workfront espone un set di strumenti che la piattaforma dell’agente di intelligenza artificiale chiama per tuo conto. Ad esempio, strumenti per cercare in Workfront, creare elementi, aggiornare campi e gestire le approvazioni. Per l&#39;elenco completo dei riferimenti, vedere [Strumenti server Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

La disponibilità dello strumento dipende dalle adesioni ai prodotti della tua organizzazione, oltre al livello di accesso a Workfront, alle autorizzazioni per gli oggetti e a tutti i controlli di amministrazione MCP.

>[!IMPORTANT]
>
>Quando connetti una piattaforma di agenti di intelligenza artificiale a Workfront, agisce in Workfront utilizzando l’account e le autorizzazioni Workfront. Le azioni della piattaforma hanno lo stesso effetto delle azioni eseguite direttamente nell&#39;interfaccia di Workfront.<br>
>
>Tu e il provider di piattaforme AI agentic siete responsabili delle azioni che la piattaforma compie in Workfront. Adobe non è responsabile delle modifiche apportate dalla piattaforma AI ai dati Workfront.<br>
>
>Prima di consentire alla piattaforma dell’agente di IA di procedere con una richiesta, conferma di comprendere cosa intende fare, in particolare per le azioni che modificano o eliminano i dati.

## Effetti delle adesioni ai prodotti sugli strumenti disponibili

Il server MCP di Workfront mostra solo gli strumenti che la tua organizzazione è autorizzata a utilizzare.

Si applicano i seguenti scenari:

* Se la tua organizzazione dispone solo di Workfront Planning, la piattaforma dell’agente di IA mostra gli strumenti di Planning, ma non gli strumenti del flusso di lavoro.
* Se la tua organizzazione dispone solo di Workfront Workflow, la piattaforma dell’agente di IA mostra gli strumenti del flusso di lavoro, ma non gli strumenti di Planning.
* Se la tua organizzazione dispone sia di Workfront Workflow che di Workfront Planning, la piattaforma dell’agente di IA mostra entrambi i set di strumenti.
* Approfondimenti e strumenti contestuali sono disponibili per tutti i clienti.

Se uno strumento non è disponibile per i diritti dell’organizzazione, non viene visualizzato nell’elenco degli strumenti per tale connessione. Se una piattaforma di agenti di intelligenza artificiale tenta di chiamare direttamente lo strumento comunque, la richiesta viene bloccata e restituisce un errore relativo all’adesione.

Per i generatori di agenti e gli utenti avanzati, tieni presente quanto segue:

* L’elenco degli strumenti disponibili può variare tra i clienti.
* L&#39;elenco degli strumenti viene stabilito all&#39;avvio della connessione.
* Se i diritti di un cliente cambiano, l&#39;elenco degli strumenti aggiornato viene visualizzato alla successiva connessione del cliente al server Workfront MCP.

>[!NOTE]
>
>Workfront Workflow è attualmente considerata l’area di prodotto di base per la disponibilità dello strumento MCP. Gli strumenti di pianificazione vengono filtrati in base al diritto. Non vi sono attualmente limitazioni di adesione sugli strumenti di approvazione.


## Esempi di cosa chiedere

Dopo la connessione, digita le richieste in linguaggio naturale nella piattaforma dell’agente di intelligenza artificiale. La piattaforma per agenti di intelligenza artificiale decide quali azioni Workfront chiamare e restituisce i risultati.

>[!NOTE]
>
>Alcune azioni potrebbero non essere disponibili a causa di controlli di amministrazione nell’area di configurazione di Workfront o perché la tua organizzazione non dispone dei diritti necessari per l’area di prodotto correlata. Ad esempio, potrebbe non essere possibile creare articoli se l&#39;amministratore di Workfront ha disabilitato le azioni di scrittura per il server MCP oppure gli strumenti di Planning potrebbero non essere disponibili se l&#39;organizzazione non dispone della licenza per Workfront Planning.


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

<!--
* *Remove Anna Jones from all approvals in this project, and replace with Sione Carter.*
-->


### Utilizzare i record di Planning

>[!IMPORTANT]
>
>* Per utilizzare MCP con Workfront Planning, l&#39;organizzazione deve essere inclusa in un pacchetto Workfront che includa Adobe Workfront Planning.

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


## Considerazioni

Quando si utilizza il server MCP di Workfront, tenere presenti le seguenti considerazioni:

### La piattaforma dell’agente di IA può utilizzare informazioni precedenti nella conversazione

Le piattaforme basate sull’intelligenza artificiale a volte riutilizzano i dati precedenti in una conversazione, anziché chiedere a Workfront di usare la versione più recente. Se è cambiato qualcosa in Workfront dall’ultima visualizzazione della piattaforma dell’agente di intelligenza artificiale, potrebbero essere visualizzate informazioni obsolete.

Per forzare la piattaforma dell’agente di intelligenza artificiale a recuperare nuovi dati, richiedila esplicitamente. Ad esempio:

* *Scarica i dati più recenti da Workfront. Non utilizzare i risultati memorizzati nella cache.*

### I dati di Insights sono quasi in tempo reale, non istantanei

Gli strumenti Insights utilizzati per trovare, filtrare e generare rapporti sui dati di Workfront riflettono le modifiche quasi in tempo reale, con un service level agreement (SLA) di circa 15 minuti. Se apporti una modifica in Workfront e chiedi immediatamente informazioni al riguardo, la risposta potrebbe non riflettere tale modifica.

Se devi confermare una modifica molto recente, attendi qualche minuto e chiedi di nuovo, oppure controlla direttamente in Workfront.

### Verifica la disponibilità di aggiornamenti per il server Workfront MCP

È possibile aggiornare periodicamente la connessione al server Workfront MCP per assicurarsi di disporre degli strumenti e delle funzionalità più recenti.

La maggior parte degli aggiornamenti dovrebbe avvenire automaticamente. Tuttavia, è consigliabile controllare periodicamente le note sulla versione di Workfront.


## Dati e sicurezza

Gli strumenti server MCP di Workfront sono coerenti con il funzionamento delle chiamate API. In Workfront non vengono memorizzati prompt, risposte o altri dati. Tutti i dati Workfront richiesti sono accessibili nella piattaforma Workfront.

Il livello di accesso e le autorizzazioni per gli oggetti determinano gli elementi che è possibile eseguire query o scrivere in Workfront. L&#39;amministratore di Workfront ha il controllo delle azioni di lettura e scrittura MCP nell&#39;area di configurazione di Workfront.

### Quali dati lasciano Workfront

Il provider di piattaforme AI ha accesso ai dati Workfront con cui interagisci tramite il server MCP di Workfront. Per informazioni dettagliate, rivolgiti al provider di piattaforme basate su AI.


### Gestione dei dati Workfront da parte dei provider di piattaforme basate su IA

Workfront non ha il controllo sul modo in cui il provider della piattaforma di gestione dell’intelligenza artificiale gestisce i dati Workfront. Per informazioni dettagliate, rivolgiti al provider di piattaforme basate su AI.

## Risolvere i problemi relativi all’uso quotidiano

+++ Espandi per visualizzare suggerimenti per la risoluzione dei problemi relativi all’utilizzo quotidiano del server MCP di Workfront.

| Problema | Probabile causa | Correggi |
| --- | --- | --- |
| La piattaforma dell’agente di intelligenza artificiale fornisce informazioni obsolete. | La piattaforma dell’agente di intelligenza artificiale sta riutilizzando i dati di precedenti momenti della conversazione. | Richiedi nuovi dati da Workfront. |
| I dati che hai appena modificato in Workfront non vengono ancora visualizzati. | I dati di Insights sono quasi in tempo reale, con un SLA di circa 15 minuti. | Attendi alcuni minuti e chiedi di nuovo, oppure controlla direttamente in Workfront. |
| La piattaforma dell’agente di intelligenza artificiale ha restituito dati dagli elementi Workfront errati. | La piattaforma dell’agente di intelligenza artificiale ha scelto gli elementi errati in base a una formulazione ambigua. | Chiedi di nuovo con nomi, ID o filtri più specifici. |
| Un aggiornamento o una cancellazione non ha avuto effetto in Workfront. | L&#39;amministratore di Workfront ha disabilitato le azioni di scrittura per il server Workfront MCP oppure non si dispone dell&#39;autorizzazione per eseguire l&#39;azione sull&#39;elemento specifico. | Conferma con la piattaforma dell’agente di intelligenza artificiale l’esecuzione dell’azione. Verificare quindi che le azioni di scrittura siano abilitate per il server Workfront MCP e di disporre dell&#39;autorizzazione per modificare l&#39;elemento. |
| Uno strumento che un altro cliente può utilizzare non viene visualizzato automaticamente. | L&#39;organizzazione non ha diritto a quell&#39;area di prodotto oppure la connessione è stata avviata prima dell&#39;entrata in vigore di una modifica del diritto. | Conferma per quali prodotti Workfront la tua organizzazione dispone della licenza. Se i diritti sono stati modificati di recente, avvia una nuova connessione MCP e controlla nuovamente l’elenco degli strumenti. |

Per ulteriori informazioni sui problemi di installazione e autenticazione, vedere [Risoluzione dei problemi di installazione e autenticazione](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) in [Configurazione del server Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

+++

## Domande frequenti

+++ Espandi per visualizzare le domande frequenti sull’utilizzo del server MCP di Workfront.

### Che cos’è una piattaforma di intelligenza artificiale?

Una piattaforma per l’agente di intelligenza artificiale è uno strumento di intelligenza artificiale che può intraprendere azioni per tuo conto in
altri sistemi, non solo rispondere alle domande. Quando ne connetti uno a Workfront
attraverso il server MCP, è possibile trovare, creare, aggiornare ed eliminare Workfront
articoli in base a ciò che gli viene chiesto nel linguaggio naturale. Alcuni esempi includono Claude
Desktop, ChatGPT e altri client di intelligenza artificiale compatibili con MCP.


### È necessario essere un amministratore Workfront per utilizzare il server Workfront MCP?

No. Qualsiasi utente di Workfront può utilizzare il server Workfront MCP tramite un
Piattaforma di intelligenza artificiale. La piattaforma dell’agente di intelligenza artificiale agisce utilizzando il Workfront
autorizzazioni di account, livello di accesso e oggetto, in modo da poter eseguire solo le operazioni
poteva già fare direttamente in Workfront.

### Perché la piattaforma dell’agente di intelligenza artificiale non può creare, aggiornare o eliminare elementi?

L’amministratore di Workfront controlla quali azioni MCP sono consentite nel
Area di configurazione di Workfront. Se le azioni di scrittura sono disabilitate, la piattaforma dell’agente di intelligenza artificiale
è ancora in grado di trovare e leggere gli elementi di Workfront, ma non può apportare modifiche. Anche tu
è necessario disporre del livello di accesso e delle autorizzazioni oggetto appropriati per gli elementi specifici
stai lavorando con.

### La piattaforma per agenti di intelligenza artificiale mi chiederà prima di modificare o eliminare i dati di Workfront?

Questo dipende dalla piattaforma dell’agente di intelligenza artificiale, non da Workfront. La maggior parte delle piattaforme
chiedi conferma prima di eseguire un’azione, in particolare per le eliminazioni.
Prima di approvare una richiesta, leggi cosa dice la piattaforma che sta per fare —
le modifiche vengono apportate in Workfront nello stesso modo in cui accadrebbero se fossero apportate
nell’interfaccia.

<!--

### Can I undo something the AI agentic platform did in Workfront?

Changes the AI agentic platform makes in Workfront work the same way as 
changes you make in the interface. If Workfront supports undoing or 
restoring a particular action (for example, restoring a deleted item from 
the Recycle Bin), the same options apply. If Workfront doesn't normally let 
you undo an action, you can't undo it through the AI agentic platform either.

-->

### Perché la piattaforma dell’agente di intelligenza artificiale ha restituito gli elementi Workfront errati?

La piattaforma di gestione dell’intelligenza artificiale seleziona gli elementi in base alle parole utilizzate. Se il
richiesta ambigua, ad esempio due progetti con nomi simili
potrebbe scegliere quella sbagliata. Chiedi di nuovo con nomi, ID, date più specifici,
o filtri per limitare i risultati.


### Con quali elementi di Workfront posso lavorare tramite una piattaforma di agenti di intelligenza artificiale?

Tutti gli elementi a cui hai accesso in Workfront tramite il tuo livello di accesso e
autorizzazioni oggetto. Ciò include progetti, attività, problemi, documenti,
approvazioni, record di Planning e altro ancora.

### Altre persone possono vedere le mie conversazioni con la piattaforma di agenti di intelligenza artificiale?

Workfront non memorizza le richieste o le risposte della piattaforma di agente di intelligenza artificiale.
Chiunque fornisca la piattaforma di agenti di intelligenza artificiale controlla in che modo le conversazioni
sono archiviati o condivisi. Rivolgiti al provider di piattaforme AI per sapere
dettagli.

### Devo conoscere l’API di Workfront o quale strumento MCP utilizzare?

No. La piattaforma AI agentic traduce la richiesta in lingua naturale in
le azioni giuste di Workfront e seleziona gli strumenti giusti per te. Se sei
hanno già familiarità con l’API di Workfront, le azioni avranno familiarità con
ma non è un requisito.

### I miei dati Workfront vengono inviati al provider di piattaforme basate su IA o memorizzati da quest’ultimo?

Per ulteriori informazioni, vedere [Dati e sicurezza](#data-and-security) in questo
articolo.

### Cosa succede quando viene rilasciata una nuova versione del server Workfront MCP?

Il server MCP in genere si aggiorna automaticamente, ma potrebbe essere necessario aggiornare la connessione al server MCP in alcuni momenti per visualizzare gli strumenti e le funzionalità più recenti.

### Perché non vedo gli stessi strumenti MCP visualizzati da un altro cliente?

Gli strumenti MCP disponibili possono variare a seconda del cliente, in quanto il server MCP di Workfront filtra alcuni strumenti in base alle adesioni dei prodotti. Ad esempio, i clienti con licenza per Workfront Planning possono visualizzare gli strumenti di Planning, mentre i clienti senza tale autorizzazione non possono visualizzarli. I clienti con licenza per Workfront Workflow possono visualizzare gli strumenti del flusso di lavoro.

L&#39;elenco degli strumenti viene impostato all&#39;avvio della connessione. Se i diritti della tua organizzazione cambiano, avvia una nuova connessione per visualizzare l’elenco aggiornato.

### Posso utilizzare il server Workfront MCP se la mia istanza Workfront non è abilitata su Adobe Identity Management System (IMS)?

No. Per utilizzare il server MCP di Workfront, l’istanza di Workfront deve essere abilitata su Adobe Identity Management System (IMS). Se non sei sicuro se la tua istanza è abilitata su IMS, contatta il tuo amministratore Workfront.


+++
