---
title: Richieste e best practice per CX Collaborator
content-type: reference
description: Scopri le best practice per l’utilizzo di Coworker in Workfront e visualizza un elenco di esempi di prompt.
author: Becky
feature: Get Started with Workfront
source-git-commit: 01de260893e5bbf7a228479df2f3fc6a1337d31d
workflow-type: tm+mt
source-wordcount: '2247'
ht-degree: 2%

---

# Richieste e best practice per CX Collaborator

&lt;!—DO NOT USE THIS—Collegamento invece all&#39;articolo di richiesta di esempio MCP, assicurarsi che sia aggiornato con le versioni recenti di MCP—>

>[!IMPORTANT]
>
>CX Coworker non è attualmente disponibile per le organizzazioni del settore sanitario, finanziario o di altri settori con dati sensibili. L’Assistente AI è disponibile per queste organizzazioni. Per ulteriori informazioni, vedere [Panoramica dell&#39;Assistente AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

Con CX Coworker è possibile utilizzare il linguaggio naturale per interagire con Workfront Workflow e Workfront Planning.

Collaboratore fa parte di Adobe Experience Cloud Agent Orchestrator.

Per ulteriori informazioni su Agent Orchestrator, vedere [Adobe Experience Platform Agent Orchestrator](https://experienceleague.adobe.com/it/docs/experience-cloud-ai/experience-cloud-ai/agents/agent-orchestrator).

## Requisiti di accesso

<!--Add info about how to qualify for agent orchestrator stuff-->

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Seleziona, Prime o Ultimate </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td><p>Standard o Light</p>
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td><p>Per qualsiasi funzionalità al di fuori delle competenze di base, la tua organizzazione deve aver acquistato Adobe Agent Orchestrator.</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td><p>È necessario disporre delle autorizzazioni appropriate per interagire con qualsiasi oggetto tramite Collaboratore.</p> <p>Ad esempio, per ricevere informazioni su un progetto tramite Collaboratore, è necessario disporre almeno dell'autorizzazione Visualizzazione per tale progetto.</p></td>
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

* L’amministratore di Workfront deve aver abilitato l’Assistente AI per la tua organizzazione.

  Per ulteriori informazioni, vedere [Prerequisiti per l&#39;Assistente IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant) nell&#39;articolo Panoramica dell&#39;Assistente IA.
* L&#39;amministratore di Workfront deve aver abilitato l&#39;Assistente AI per il proprio livello di accesso.

  Per ulteriori informazioni, consulta [Abilitare o disabilitare l’Assistente IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

## Considerazioni

Quando si utilizza CX Collaborator, tenere presenti i seguenti vincoli:

### Reversibilità

Alcune azioni possono essere annullate. Ad esempio, se viene creato un oggetto, tale creazione può essere annullata.

Tuttavia, alcune azioni, ad esempio l&#39;eliminazione di un oggetto, possono **non** essere annullate. È consigliabile tenerlo presente quando esegui azioni sui dati tramite Collaboratore.

### Vincoli di copertura di dati/oggetti

* La query e il reporting sui campi personalizzati si trovano in fase iniziale e alcune abilità (come gli helper per query basati su API) non gestiscono ancora campi personalizzati arbitrari per l’aggregazione e il filtraggio.

### Limitazioni di interazione/interfaccia utente

* CX Coworker attualmente non &quot;impara&quot; a lungo termine dallo stile o dalle preferenze di un singolo utente. Ogni chat utilizza solo la conversazione corrente e la conoscenza del prodotto.
* Il contesto della conversazione viene mantenuto all’interno di una singola sessione di chat. L&#39;apertura di una nuova pagina o la chiusura dell&#39;assistente ripristina la cronologia delle conversazioni.
* Se le procedure di approvazione si trovano in un’applicazione esterna come Confluence o SharePoint e sono collegate solo tramite campi URL, al momento Collaboratore non recupera e motiva tali pagine.

### Archiviazione dati/chiavi gestite dal cliente

* Poiché CX Coworker fa parte di Adobe Experience Platform Agent Orchestrator, i dati provenienti dalle interazioni con Coworker vengono memorizzati in Adobe Experience Platform, non in Workfront. Pertanto, questi dati non sono coperti dagli accordi BYOK (Customer Managed Keys) di Workfront.

## Competenze di intelligenza artificiale fondamentali per uso generale

>[!IMPORTANT]
>
>Queste funzioni generali sono disponibili per tutti gli utenti la cui organizzazione dispone di un accordo Adobe AI firmato su file.

Per le best practice e i prompt per queste abilità di utilizzo generale, consulta [Suggerimenti dell&#39;Assistente AI e best practice](/help/quicksilver/workfront-basics/ai-assistant/ai-prompts-best-practices.md).

<!--Follow up with Oznur-->

### Conoscenza del prodotto

CX Coworker è in grado di fornire istruzioni o informazioni di riferimento ricavate dalla documentazione Workfront.

Per ulteriori informazioni sull&#39;estrazione di informazioni dalla documentazione di Workfront, vedere [Ottenere assistenza dall&#39;Assistente AI](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

Esempio: come si modifica il tipo di durata dell&#39;attività?

### Riepilogo di progetto, attività e problema

CX Coworker è in grado di riepilogare progetti, attività o problemi <!--, or documents--> caricati in Workfront.

Per ulteriori informazioni sui riepiloghi di progetti, attività e problemi, consulta [Riepilogare utilizzando l&#39;Assistente AI](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

Esempio: riepiloga il progetto denominato Fall Campaign 2026.

<!--

### Locate work items

CX Coworker can find work items like projects, tasks, and issues

Example: Find all tasks assigned to me that are due this week.

For more information on using AI Assistant to locate project, tasks, and issues, see [se AI Assistant to work with projects, tasks, and issues](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

-->

<!--

Follow up on this to see if it's going away or what

### Catch Me Up 

Catch Me Up summarizes updates, uploaded documents, and other notable changes that have about your projects that have occurred in the last 24 hours, 3 days, or 7 days.  

For more information on Catch me up, see [Catch up on work in Priorities](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).

-->

<!--

### Smart filters

You can use natural language filters in Priorities to replace status, pre-built views to help you filter your work.

For more information on using Smart Filters, see [Filter your work with Smart filters](/help/quicksilver/workfront-basics/priorities/filter-group-work-priorities.md) in the article Filter and group your work with Priorities.

-->

## CX Coworker in Workfront

* [Informazioni su progetto, attività e problema](#project-task-and-issue-information)
* [Gestione dei progetti e del lavoro](#project-and-work-management)
* [Contenuto e approvazioni](#content-and-approvals)

### Informazioni su progetto, attività e problema

CX Collaborator può fornire informazioni su progetti, attività e problemi, inclusi riepiloghi e stato del progetto.

Consulta gli esempi di prompt per le approvazioni di documenti e risorse nelle seguenti aree:

* [Trova informazioni su progetti, attività o problemi](#find-information-about-projects-tasks-or-issues)
* [Riepiloga progetti, attività o problemi](#summarize-projects-tasks-or-issues)
* [Mostra stato progetto per progetti, programmi o portfolio](#show-project-health-for-projects-programs-or-portfolios) <!--remove any mention of project health-->

#### Trova informazioni su progetti, attività o problemi

* Progetti
  * Mostra tutti i progetti attivi per il team Marketing marchio
  * è necessario un elenco di progetti nel portfolio delle campagne del quarto trimestre nella categoria &quot;Digitale&quot;.
  * Mostra i progetti gestiti dagli utenti della società di servizi Creative che sono project manager.
* Attività
  * Mi dia tutti i compiti assegnati a Joan Harris.
  * Mostra le attività nella categoria &quot;Progettazione&quot; assegnate al team UX.
  * Ho bisogno di attività assegnate a Copywriter nel programma Holiday Promotions.
* Problemi
  * Mostra tutti i problemi nel progetto &quot;Riprogettazione del sito web&quot; nella categoria &quot;Tecnico&quot;.
  * Ottieni tutti i problemi non risolti segnalati dal gruppo di controllo qualità.
  * Ho bisogno di problemi assegnati agli sviluppatori della società Global Tech.

#### Riepiloga progetti, attività o problemi

* &quot;Riepiloga questo progetto&quot;
* &quot;Riepiloga l’ultima settimana per questo progetto&quot;

#### Mostra stato progetto per progetti, programmi o portfolio

>[!NOTE]
>
>Per utilizzare questa funzione, la tua organizzazione deve essere iscritta alla versione beta di Project Health.

* &quot;Mostrami lo stato dei miei progetti attivi&quot;
* &quot;Mostrami lo stato di questo programma&quot;

### Gestione dei progetti e del lavoro

È possibile utilizzare CX Collaborator per creare e gestire progetti, incluse attività e assegnazioni.

Vedi gli esempi di prompt per la gestione del progetto e del lavoro nelle seguenti aree:

* [Creare, aggiornare o eliminare progetti](#create-update-or-delete-projects)
* [Identificare il modello di progetto corretto in base al prompt dell&#39;utente](#identify-the-right-project-template-based-on-user-prompt)
* [Aggiungere, modificare o personalizzare attività in un progetto](#add-edit-or-customize-tasks-in-a-project)
  <!--* [Create, update, or delete assignments](#create-update-or-delete-assignments)-->
  <!--* [Recommend best matching user assignments for the task based on users' job role and availability](#recommend-best-matching-user-assignments-for-the-task-based-on-users-job-role-and-availability)-->

#### Creare, aggiornare o eliminare progetti

Puoi creare progetti da zero o da modelli, aggiornare i progetti ed eliminarli.

* Crea un progetto vuoto denominato Q2 Innovation Sandbox a partire dal 10 marzo e fino al 30 aprile. Impostami come proprietario.
* Crea un progetto denominato Lucent AI Launch - NA utilizzando il modello Campagna di marketing integrata. Iniziare il 5 febbraio e impostarlo su Corrente.
* Crea un progetto chiamato Riprogettazione del sito web - EMEA a partire dal 1° marzo e fino al 15 giugno. È altamente prioritario, di proprietà di EMEA Marketing, sponsorizzato dal VP of Marketing, preventivato a $ 250.000 con circa 1.200 ore pianificate, concentrato sull&#39;Europa con l&#39;obiettivo di migliorare le conversioni.
* Per il progetto Lucent AI Launch - NA, spostalo al secondo trimestre, modifica l’obiettivo per l’esecuzione di prove gratuite, porta la fine a metà aprile, aumenta il budget a 150.000 dollari e segnalalo come urgente.
* Mostra tutti i progetti di marketing in corso che terminano nel secondo trimestre con priorità alta o urgente, ordinati in base alla prima data di fine.

#### Aggiungere o modificare le attività

È possibile aggiungere o modificare le attività di un progetto e personalizzare l&#39;elenco delle attività del modello utilizzato per creare un progetto.

* Aggiungi al progetto una nuova attività denominata Controllo di qualità pagina di destinazione e programmalo dal 22 aprile al 26 aprile.
* Aggiorna l’attività Design Review in modo che termini il 18 aprile e assegnala al team creativo.
* Rimuove dal progetto l&#39;attività Stampa produzione risorse.
* Mostra tutte le attività di questo progetto che non sono state completate e il cui inizio è pianificato tra il 1 aprile e il 30 aprile.
* Imposta Approvazione legale come predecessore dell’attività di Campaign Launch.
* Aggiungi una nuova attività denominata Final Copy Polish programmata dal 15 aprile al 16 aprile, sposta l’attività Copy Review al 10 aprile, rimuovi l’attività Extra Review Round e imposta Final Copy Polish come predecessore di Email Build.
* Durante la creazione del progetto, prova a fornire quante più informazioni possibili sui risultati finali, che idealmente dovrebbero diventare attività sotto il progetto.

#### Crea, aggiorna o elimina assegnazioni

È possibile creare, aggiornare ed eliminare assegnazioni utente o mansione.

* Per il progetto &quot;Pagina di destinazione per progettazione per lancio prodotto&quot;, identifica i ruoli appropriati e le ore pianificate consigliate per tutte le attività attualmente non assegnate.
* Ho diverse attività non assegnate, tra cui &quot;Implementa il tracciamento GA4 per il sito della campagna&quot;, &quot;Imposta eventi di conversione&quot; e &quot;Convalida dati di analisi&quot;. Puoi suggerire i ruoli giusti e le ore stimate per ciascuno?
* Per le attività creative &quot;Crea 3 varianti di banner per annunci display EMEA&quot;, &quot;Applica revisioni&quot; ed &quot;Esporta risorse finali&quot;, assegna i ruoli migliori e stima lo sforzo necessario per ogni attività.
* Nei progetti &quot;Lancio prodotto Q2&quot;, &quot;Riprogettazione sito web - EMEA&quot; e &quot;Campagna media a pagamento - NA&quot;, identifica tutte le attività non assegnate e assegna i ruoli appropriati con le ore pianificate consigliate per ciascuno di essi.

<!--

#### Identify the right project template based on user prompt

* We're launching a new product feature with a landing page, emails, paid ads, and social posts. Which project template should we use?
* Create a project for a global marketing campaign with multiple channels and regional rollouts. (should suggest a template if provided more info)
* For Website Redesign – EMEA project, recommend and attach the correct project template.

-->

<!--

#### Recommend best matching user assignments for the task based on users' job role and availability

* Who is the best available user to assign to 'Design Landing Page Hero', considering who still has capacity today?
* Who should be assigned to 'Backend API integration for campaign reporting', considering engineering role alignment?
* For all unassigned tasks in this project, recommend the best users based on job role match and daily availability.
* Recommend users for the tasks 'QA testing for website launch' and 'Content review', prioritizing users whose job roles match and who are not over-allocated today.

-->

### Contenuto e approvazioni

CX Collaborator consente di gestire le approvazioni di documenti e risorse in Workfront.

Quando si lavora con le approvazioni di documenti e risorse, considera quanto segue:

* Prima di poter utilizzare questa funzionalità in Collaboratore, è necessario abilitare le approvazioni dei contenuti per la tua organizzazione.
* L&#39;IA non può approvare o rifiutare per conto degli esseri umani. Le decisioni si basano sugli utenti, ad eccezione di Workfront AI Reviewer.

  Per ulteriori informazioni su Workfront AI Reviewer, consulta [Introduzione a Workfront AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).
* Questa funzionalità esiste in Workfront e non può essere utilizzata per interagire con strumenti o provider di documenti esterni.
* Per una migliore esperienza, utilizza questa funzionalità con l’esperienza Approvazioni unificate.

  Per ulteriori informazioni sulle approvazioni unificate, vedere [Panoramica sulle approvazioni unificate](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

Consulta gli esempi di prompt per le approvazioni di documenti e risorse nelle seguenti aree:

* [Aggiungi o rimuovi partecipanti all&#39;approvazione](#add-or-remove-approval-participants)
* [Ricordare alle parti interessate di una singola risorsa in attesa di revisione](#remind-stakeholders-of-a-single-asset-waiting-for-review)
* [Aggiungere, aggiornare o applicare modelli di approvazione per una singola risorsa](#add-update-or-apply-approval-templates-for-a-single-asset)

#### Aggiungi o rimuovi partecipanti all&#39;approvazione

* Aggiungi Sarah Chen e Miguel Alvarez come approvatori nel documento corrente.
* Rimuovi Jennifer Otto da questa approvazione.
* Rimuovere tutti coloro che non hanno preso una decisione di approvazione.
* Aggiungi una nuova fase al Spring-Campaign.pdf denominata &quot;Final Review&quot;.
* Aggiungi Mark e Sarah come approvatori e Phil come revisore nella seconda fase della campagna invernale.pdf
* Per la campagna invernale.pdf, assegna alla prima fase un termine per oggi alle 17.00 e alla revisione finale un termine per domani alle 17.00
* Aggiungi una fase di controllo finale al fall-campaign.png con una scadenza per giovedì alle 17 e includi Jim e Pam come approvatori, anche Oscar come revisore
* Aggiungi Mark Jones al fall-campaign.png alla prima e all’ultima fase come revisore.
* Ottieni un’approvazione in più fasi creata per il file fall-campaign.png con 3 fasi, 1 design 2 copywriting e 3 Legal. Mi serve solo una decisione per ogni fase. Aggiungi Mike, Sally, Jane al design, Chris, Richard, Mark al copywriting e Phil, Tom e Sarah all&#39;Ufficio legale.

#### Ricordare alle parti interessate di una singola risorsa in attesa di revisione

* Invia un promemoria agli approvatori della risorsa &quot;Video campagna di primavera&quot; che non hanno risposto.
* Ricordate a tutti coloro che non hanno approvato questa risorsa &quot;Video sulla campagna di primavera&quot;.
* Chi non ha ancora preso una decisione sulla risorsa &quot;Brand Guidelines PDF&quot;? Ricordategli.

#### Aggiungere, aggiornare o applicare modelli di approvazione per una singola risorsa

* Applica il modello di approvazione &quot;Marketing Launch&quot; alla risorsa denominata &quot;Video campagna di primavera&quot;.
* Crea un nuovo modello di approvazione con 3 fasi: Revisione Creative, Approvazione legale e Approvazione finale.
* Aggiungere Julia Santos e Shane Baker al livello 1.
* Modifica il modello &quot;Product Launch&quot; per aggiungere Elizabeth Peterson alla fase di approvazione finale.
* Crea un modello denominato &quot;Urgent Review&quot; con una fase e assegnalo a Olivia Kim.
* Aggiorna il modello &quot;Creative Review&quot; rimuovendo Rick Kuvec e aggiungendo Karen Sterling alla fase 2.


## Collaboratore CX in Workfront Planning

### Utilizzare i record di Planning

* [Creare, eliminare, duplicare o ripristinare record](#create-delete-duplicate-or-restore-records)
* [Collega record ad altri record](#link-records-to-other-records)
* [Modificare, aggiornare o aggiungere un campo a un record](#edit-update-or-append-a-field-to-a-record)
* [Cronologia modifiche record di accesso](#access-record-change-history)

#### Creare, eliminare, duplicare o ripristinare record

* Crea un nuovo record della campagna denominato Summer Sale 2026
* Aggiungi un nuovo record di prodotto con nome Widget Pro e prezzo $299
* Puoi creare un nuovo record di lead per John Smith?
* Elimina il record della campagna denominato Old Promo
* Rimuovi il record di test appena creato
* È possibile eliminare il record ID Rc123abc456?
* Duplica il record della campagna Q1
* È possibile copiare questa campagna per crearne una nuova?
* Crea una copia della campagna di promozione festività
* Ripristina la campagna che ho eliminato accidentalmente
* È possibile recuperare il record di progetto eliminato?
* Se un record è stato eliminato accidentalmente, è possibile ripristinarlo?

#### Collega record ad altri record

* Collega il record della campagna estiva all’iniziativa Q2
* È possibile collegare questo prodotto alle relative campagne di marketing?
* Devo associare questi tre lead al record Account aziendale

#### Modificare, aggiornare o aggiungere un campo a un record

* Aggiorna il campo del budget nella campagna estiva a $ 75.000
* È possibile modificare lo stato di questo record di progetto in Completato?
* Aggiungi John Doe al campo dei membri del team per questa iniziativa

#### Cronologia modifiche record di accesso

* Mostrami la cronologia delle modifiche per il record della campagna estiva
* È possibile visualizzare chi ha modificato questo progetto e cosa è cambiato?
* Devo visualizzare tutti gli aggiornamenti apportati a questo record nell’ultima settimana

### Utilizzare System Designer in Workfront Planning

* [Creare e configurare le aree di lavoro](#create-and-configure-workspaces)
* [Definire i tipi di record](#define-record-types)
* [Progettare campi e campi formula](#design-fields-and-formula-fields)
* [Creare viste personalizzate](#build-custom-views)


#### Creare e configurare le aree di lavoro

* Crea una nuova area di lavoro di Planning denominata Campagne di marketing 2026
* Aggiorna la mia area di lavoro di pianificazione del prodotto per cambiare il colore in blu e aggiungere una descrizione
* Mostra tutte le aree di lavoro di Planning a cui ho accesso

#### Definire i tipi di record

* Crea un nuovo tipo di record denominato Campagne nella mia area di lavoro di Planning
* Aggiornare il tipo di record Iniziative per modificarne l&#39;icona e la descrizione
* Mostra tutti i tipi di record nell&#39;area di lavoro Marketing Planning

#### Progettare campi e campi formula

* Aggiungi un campo Budget al tipo di record Campagne pianificazione con tipo di valuta
* Creare un campo formula in Planning che calcola i giorni rimanenti alla data di fine della campagna
* Aggiorna il campo Priorità nella mia area di lavoro Planning per aggiungere altre opzioni a discesa

#### Creare viste personalizzate

* Crea una vista timeline in Planning per visualizzare la pianificazione della campagna in base alle date di inizio e fine
* Aggiungi una nuova vista tabella alle mie iniziative Planning che filtra solo lo stato attivo
* Duplicare la vista di Planning Active Campaigns e modificare l&#39;ordinamento.
