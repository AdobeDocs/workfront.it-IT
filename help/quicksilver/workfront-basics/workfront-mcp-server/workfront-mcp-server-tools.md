---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Strumenti server Adobe Workfront MCP
description: Elenco di riferimento degli strumenti disponibili tramite il server Adobe Workfront MCP, raggruppati per area Workfront.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 98d5b93bcb99c468de2ad107a2aca3a9a1995429
workflow-type: tm+mt
source-wordcount: '1392'
ht-degree: 3%

---


# Strumenti server Adobe Workfront MCP

In questo articolo sono elencati gli strumenti esposti dal server MCP [!DNL Adobe Workfront] a una piattaforma agente di IA connessa. La piattaforma chiama questi strumenti per tuo conto quando gli chiedi di trovare, creare, aggiornare o eliminare elementi Workfront.

Gli strumenti sono raggruppati per area Workfront: Approvazioni, Pianificazione e Flusso di lavoro.

Per informazioni sull&#39;utilizzo di questi strumenti tramite una piattaforma di gestione dell&#39;intelligenza artificiale, vedere [Utilizzare il server MCP di Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md). Per informazioni sulla configurazione della connessione, vedere [Configurare il server MCP di Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

>[!IMPORTANT]
>
>La piattaforma dell’agente di intelligenza artificiale agisce in Workfront utilizzando il tuo account Workfront, il tuo livello di accesso e le autorizzazioni per gli oggetti. Uno strumento funziona solo se disponi dell’accesso corrispondente in Workfront. Adobe non è responsabile delle modifiche apportate dalla piattaforma AI ai dati Workfront.

## Strumenti di approvazione (23 in totale)

### Documenti

<!-- 
VERIFY BEFORE PUBLISHING: The following three tools may not be customer-facing. If engineering confirms they're internal-only, delete these rows from the table below:
- approvals_get_document_by_version_id
- approvals_list_aem_linked_folders
- approvals_send_documents_to_aem_folder
-->

| Titolo | Nome strumento | Funzionamento |
|---|---|---|
| Trova versione documento per nome | `approvals_find_document_version_by_name` | Cerca l&#39;ID versione corrente di un documento in base al nome file. Supporta le corrispondenze parziali. |
| Ottieni documento per ID versione | `approvals_get_document_by_version_id` | Recupera i dettagli del documento (nome, dimensione, data di caricamento, caricatore) per un ID versione documento noto. |
| Ottieni documenti per progetto | `approvals_get_documents_by_project` | Elenca i documenti all&#39;interno di un progetto Workfront, con l&#39;ID di versione corrente di ciascun documento. |
| Risolvi ambito documento | `approvals_resolve_document_scope` | Espande un progetto o una cartella nell&#39;elenco degli ID di versione del documento in esso contenuto. Supporta gli ambiti progetto, cartella e cartella per nome. |
| Elencare cartelle collegate ad AEM | `approvals_list_aem_linked_folders` | Elenca le cartelle di documenti di Workfront collegate a Adobe Experience Manager. |
| Inviare documenti alla cartella AEM | `approvals_send_documents_to_aem_folder` | Sposta uno o più documenti Workfront in una cartella collegata ad AEM. |

### Approvazione dei flussi di lavoro

| Titolo | Nome strumento | Funzionamento |
|---|---|---|
| Ottieni informazioni sul flusso di lavoro di approvazione | `approvals_get_approval_info` | Restituisce il flusso di lavoro di approvazione corrente (fasi, partecipanti, stato) per una versione del documento. |
| Crea o aggiorna flusso di lavoro di approvazione | `approvals_create_or_update_approval_workflow` | Crea o aggiorna le fasi del flusso di lavoro di approvazione per una versione del documento. Supporta le dipendenze degli stadi lineari e paralleli (grafi). |
| Crea approvazione da modello | `approvals_create_approval_from_template` | Crea un flusso di lavoro di approvazione su un documento utilizzando un modello esistente. |
| Richiedi approvazione documento | `approvals_request_document_approval` | Apre un modulo guidato per la richiesta di approvazione per una versione del documento (titolo, approvatori/revisori, data di scadenza facoltativa e messaggio). |
| Elimina fase di approvazione | `approvals_delete_approval_stage` | Elimina una singola fase da un flusso di lavoro di approvazione per nome o posizione. È possibile eliminare solo le fasi non avviate. |

### Promemoria

| Titolo | Nome strumento | Funzionamento |
|---|---|---|
| Invia promemoria ai partecipanti | `approvals_send_reminder_to_participants` | Invia e-mail di promemoria a partecipanti specifici in una fase di approvazione. Funziona solo per le fasi avviate, non completate, non bloccate. |
| Invia promemoria ai partecipanti indecisi | `approvals_send_reminder_to_undecided` | Invia e-mail di promemoria a tutti i partecipanti indecisi (notificati, aperti o commentati) in una fase di approvazione. |

### Modelli di approvazione

| Titolo | Nome strumento | Funzionamento |
|---|---|---|
| Elencare modelli di approvazione | `approvals_list_templates` | Elenca i modelli di approvazione disponibili in questa istanza di Workfront. Supporta il filtraggio per creatore, partecipante e l&#39;ordinamento per utilizzo. |
| Cerca modello per nome | `approvals_search_template_by_name` | Trova i modelli di approvazione per nome (corrispondenza parziale senza distinzione tra maiuscole e minuscole). |
| Crea modello di approvazione | `approvals_create_template` | Crea un nuovo modello di approvazione con dipendenze di fase lineari o basate su grafici. |
| Aggiorna modello di approvazione | `approvals_update_template` | Aggiorna un modello esistente con modifiche strutturate (aggiungere o rimuovere partecipanti, rinominare fasi, impostare scadenze, ecc.). |

### Ricerche e utenti

| Titolo | Nome strumento | Funzionamento |
|---|---|---|
| Ottieni utente corrente | `approvals_get_current_user` | Restituisce l&#39;identità Workfront dell&#39;utente chiamante, inclusi il nome, l&#39;ID utente, il nome del team principale e l&#39;ID del team principale. |
| Trova utente per nome | `approvals_find_user_by_name` | Cerca l&#39;ID di un utente di Workfront per nome (corrispondenza parziale o fuzzy). Restituisce nome, ID, e-mail, titolo e URL avatar. |
| Trova team per nome | `approvals_find_team_by_name` | Cerca l’ID di un team Workfront per nome (corrispondenza parziale o fuzzy). |
| Trova progetto per nome | `approvals_find_project_by_name` | Cerca i progetti Workfront per corrispondenza parziale dei nomi nel sistema. |
| Ottieni progetti per proprietario | `approvals_get_projects_by_owner` | Elenca i progetti Workfront di cui l&#39;utente chiamante è il proprietario. |
| Ottieni area geografica Adobe | `approvals_get_adobe_region` | Restituisce il nome Adobe di un’area del provider di cloud. |

## Strumenti di pianificazione (43 in totale)

### Aree di lavoro

| Titolo | Nome strumento | Funzionamento |
|---|---|---|
| Ottieni area di lavoro | `planning_get_workspace` | Recupera i dettagli completi di un’area di lavoro per ID o alias. |
| Ottieni elenco aree di lavoro | `planning_get_workspace_list` | Elenca tutte le aree di lavoro disponibili con impaginazione basata su cursore. |
| Crea area di lavoro | `planning_create_workspace` | Crea una nuova area di lavoro vuota per organizzare tipi di record, campi e dati. |
| Crea area di lavoro dal modello | `planning_create_workspace_from_template` | Crea una nuova area di lavoro precompilata utilizzando un modello esistente. |
| Aggiorna area di lavoro | `planning_update_workspace` | Aggiorna parzialmente un&#39;area di lavoro: nome, descrizione, icona, sezioni o proprietario. |
| Elimina area di lavoro | `planning_delete_workspace` | Elimina definitivamente un&#39;area di lavoro e tutti i relativi dati. |
| Converti area di lavoro in modello | `planning_convert_workspace_to_template` | Salva un&#39;area di lavoro esistente come modello riutilizzabile (richiede l&#39;amministratore). |
| Ottieni condivisione area di lavoro | `planning_get_workspace_sharing` | Restituisce la configurazione di condivisione e autorizzazioni corrente per un&#39;area di lavoro. |
| Modifica condivisione area di lavoro | `planning_modify_workspace_sharing` | Aggiorna chi ha accesso a un’area di lavoro e a quale livello di autorizzazione. |

### Tipi di record

| Titolo | Nome strumento | Funzionamento |
|---|---|---|
| Ottieni tipo di record | `planning_get_record_type` | Recupera tutti i dettagli di un tipo di record, inclusi i campi e le visualizzazioni. |
| Creare tipi di record | `planning_create_record_types` | Crea uno o più tipi di record all&#39;interno di una sezione dell&#39;area di lavoro. |
| Aggiorna il tipo di record | `planning_update_record_type` | Aggiorna parzialmente il nome, la descrizione, l&#39;icona o il colore di un tipo di record. |
| Elimina tipo di record | `planning_delete_record_type` | Elimina definitivamente un tipo di record e tutti i relativi record, campi e visualizzazioni. |
| Elenca tipi di record globali | `planning_list_global_record_types` | Elenca tutti i tipi di record definiti a livello centrale (globali) visibili all&#39;utente corrente. |
| Elenca i tipi di record globali che è possibile aggiungere | `planning_list_addable_global_record_types` | Elenca i tipi di record globali che possono essere aggiunti a un&#39;area di lavoro specifica. |
| Aggiungi tipo di record globale all&#39;area di lavoro | `planning_add_global_record_type_to_workspace` | Collega un tipo di record globale a un&#39;area di lavoro specificata. |
| Rimuovi tipo di record globale dall&#39;area di lavoro | `planning_remove_global_record_type_from_workspace` | Scollega un tipo di record globale da un&#39;area di lavoro ed elimina tutti i relativi record. |
| Ottieni aree di lavoro record esterne | `planning_get_external_record_workspaces` | Trova le aree di lavoro e i tipi di record collegati a un record esterno specifico. |
| Ottieni condivisione tipo di record | `planning_get_record_type_sharing` | Restituisce la condivisione e le autorizzazioni per un tipo di record specifico. |
| Modifica condivisione tipo di record | `planning_modify_record_type_sharing` | Aggiorna chi può accedere a un tipo di record e a quale livello di autorizzazione. |

### Record

| Titolo | Nome strumento | Funzionamento |
|---|---|---|
| Ottieni record | `planning_get_record` | Recupera i dettagli completi di un singolo record per ID. |
| Cerca record | `planning_search_records` | Cerca e filtra i record di un tipo di record. |
| Azioni record in blocco | `planning_bulk_record_actions` | Crea, aggiorna, elimina o ripristina più record in una singola richiesta. |
| Crea record di connessione | `planning_create_connection_record` | Crea un nuovo record in un sistema esterno connesso, ad esempio un progetto Workfront. |
| Aggiorna ordine record | `planning_update_records_order` | Modifica l&#39;ordine di visualizzazione dei record all&#39;interno di un tipo di record. |
| Ottieni registro modifiche record | `planning_get_record_change_log` | Restituisce la cronologia di modifica a livello di campo di un record. |
| Ottieni condivisione record | `planning_get_record_sharing` | Restituisce la configurazione di condivisione per un record specifico. |
| Modificare la condivisione dei record | `planning_modify_records_sharing` | Aggiorna gli utenti che possono accedere a uno o più record e a quale livello di autorizzazione. |

### Campi

| Titolo | Nome strumento | Funzionamento |
|---|---|---|
| Ottieni campo | `planning_get_field` | Recupera i dettagli completi e lo schema del valore di un campo in base all’ID. |
| Creare campi | `planning_create_fields` | Aggiunge uno o più campi (colonne) a un tipo di record. |
| Aggiorna campo | `planning_update_field` | Aggiorna parzialmente il nome, la descrizione, le opzioni o la configurazione di un campo. |
| Elimina campo | `planning_delete_field` | Rimuove definitivamente un campo e tutti i relativi dati da un tipo di record. |

### Viste

| Titolo | Nome strumento | Funzionamento |
|---|---|---|
| Ottieni visualizzazione | `planning_get_view` | Restituisce i dettagli completi di una visualizzazione per ID. |
| Crea vista | `planning_create_view` | Crea una nuova vista tabella, timeline o calendario per un tipo di record. |
| Aggiorna vista | `planning_update_view` | Aggiorna parzialmente la configurazione, i filtri o l&#39;ordinamento di una vista esistente. |
| Elimina visualizzazione | `planning_delete_view` | Elimina definitivamente una visualizzazione (i record non sono interessati). |
| Ottieni condivisione visualizzazione | `planning_get_view_sharing` | Restituisce la configurazione di condivisione per una visualizzazione specifica. |
| Modifica condivisione delle visualizzazioni | `planning_modify_view_sharing` | Aggiorna gli utenti che possono accedere a una visualizzazione e a quale livello di autorizzazione. |

### Modelli

| Titolo | Nome strumento | Funzionamento |
|---|---|---|
| Ottieni elenco modelli | `planning_get_template_list` | Elenca tutti i modelli di area di lavoro disponibili con informazioni di riepilogo. |
| Ottieni modello | `planning_get_template` | Recupera i dettagli completi di un modello specifico per ID. |

### Ricerca e utility

| Titolo | Nome strumento | Funzionamento |
|---|---|---|
| Cercare risorse | `planning_search_resources` | Esegue ricerche in aree di lavoro, tipi di record e visualizzazioni per nome. |
| Ricerca e condivisione dei dati | `planning_search_sharing_data` | Trova utenti, gruppi, team, ruoli e società per nome per la condivisione e le autorizzazioni. |
| Cerca utenti | `planning_search_users` | Cerca gli utenti con supporto di impaginazione. |

## Strumenti del flusso di lavoro (5 in totale)

Gli strumenti del flusso di lavoro sono le azioni generiche che la piattaforma dell’agente di intelligenza artificiale utilizza per lavorare con qualsiasi oggetto Workfront: progetti, attività, problemi, ore, assegnazioni, programmi, portfolio e così via.

| Titolo | Nome strumento | Funzionamento |
|---|---|---|
| Cerca oggetti | `workflow_search_any_object` | Cerca oggetti Workfront con parametri di filtro flessibili, ordinamento e impaginazione. |
| Crea oggetto | `workflow_create_any_object` | Crea un nuovo oggetto Workfront, ad esempio un progetto, un&#39;attività, un problema, un&#39;ora, un&#39;assegnazione, un programma o un portfolio. |
| Aggiorna oggetto | `workflow_update_any_object` | Aggiorna i campi su un oggetto Workfront esistente. |
| Elimina oggetto | `workflow_delete_any_object` | Elimina un oggetto Workfront in base all&#39;ID. Richiede una conferma utente esplicita prima di eseguire l’azione. |
| Risolvi nomi campi | `workflow_resolve_field_names_any_object` | Converte i nomi o le etichette dei campi forniti dall’utente nei nomi dei campi API di Workfront sottostanti in modo che la piattaforma dell’agente di IA possa creare richieste precise. |

## Come vengono aggiornati gli strumenti

Quando Adobe rilascia una nuova versione del server Workfront MCP, la piattaforma dell’agente di IA utilizza automaticamente il nuovo set di strumenti. Non è necessario riconnettersi o cambiare nulla dalla propria parte.
