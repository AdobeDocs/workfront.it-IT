---
content-type: release-notes
navigation-topic: product-releases-archive
title: Anteprima R1 3
description: Questa pagina descrive tutte le modifiche disponibili nell’ambiente Anteprima con la versione R1.3. La funzionalità di questa pagina è stata resa disponibile nell’ambiente Anteprima il 1° febbraio 2017.
author: Luke
feature: Product Announcements
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 2%

---

# Anteprima R1 3

Questa pagina descrive tutte le modifiche disponibili nell’ambiente Anteprima con la versione R1.3. La funzionalità di questa pagina è stata resa disponibile nell’ambiente Anteprima il 1° febbraio 2017.

Per un elenco di tutte le modifiche apportate in R1, vedi [Panoramica dell’attività di rilascio di R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Metodo migliorato per il collegamento di file esterni

L&#39;opzione per il collegamento di documenti da un&#39;origine esterna (ad esempio Google Drive, Box, Dropbox e così via) si trova ora in una posizione più prominente nell&#39;area Documenti. 

Inoltre, l&#39;azione di autorizzare un provider di documenti prima di collegare i file da quel provider per la prima volta è ora più intuitiva (si tratta semplicemente di un passaggio aggiuntivo quando si collegano i file da un provider esterno).

Prima di queste modifiche, l&#39;opzione per collegare i file da un&#39;origine esterna era disponibile nella finestra di dialogo Aggiungi documenti all&#39;interno dell&#39;area Documenti. Prima di collegare un documento da un&#39;origine esterna per la prima volta, l&#39;utente che ha eseguito il collegamento del documento ha dovuto autorizzare tale provider di documenti nell&#39;area Configurazione.

Per ulteriori informazioni, consulta  [Collegamento di documenti da applicazioni esterne](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Team Aggiornato Che Lavora Sul Calendario

Il calendario di lavoro disponibile per i team ora contiene funzionalità aggiuntive e un aspetto e un aspetto aggiornati. Il calendario di lavoro del team ora funziona in modo simile allo strumento di programmazione delle risorse per i progetti.

Il calendario di lavoro del team aggiornato include i seguenti miglioramenti:

* Visualizzare gli utenti in ordine alfabetico o raggruppati per ruolo.
* Filtra la tempistica della pianificazione in base alle priorità del progetto, allo stato e ai singoli progetti. Puoi anche filtrare la timeline della pianificazione in base a ruoli e utenti. L’area Filtro include meno opzioni rispetto alla pianificazione delle risorse per i progetti.
* Includi problemi nella tempistica di pianificazione.
* Visualizza le allocazioni degli utenti e modifica il numero di ore assegnate agli utenti a determinate attività e problemi per ogni giorno.
* Visualizzare gli indicatori che mostrano quando gli utenti vengono sovrassegnati in un dato giorno.
* Configura se il lavoro completato viene visualizzato nella timeline della pianificazione.

Differenze rispetto allo strumento di programmazione delle risorse quando si pianificano le risorse per i progetti:

* Tutti i membri del team vengono visualizzati nel calendario di lavoro del team.\
   Quando si pianificano risorse per i progetti, vengono visualizzati solo gli utenti a cui è associato un ruolo che corrisponde a un ruolo di una o più attività nell’area Non assegnata.
* Lo strumento Scambio non è disponibile non è incluso nel calendario di lavoro del team.
* Qualsiasi membro del team può apportare modifiche al calendario di lavoro del team.\
   Quando si pianificano risorse per i progetti, solo i responsabili risorse possono prendere decisioni sulle risorse per il progetto.
* I problemi vengono visualizzati per impostazione predefinita nel calendario di lavoro del team.\
   Quando si pianificano risorse per i progetti, i problemi non vengono visualizzati per impostazione predefinita.

Per ulteriori informazioni sull&#39;utilizzo del calendario di lavoro del team aggiornato, vedi [Pianificazione delle risorse](../../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

## Miglioramenti alla pianificazione delle risorse

La timeline della pianificazione include i seguenti miglioramenti:

* [Utilizza il filtro per controllare quali utenti vengono visualizzati nella Timeline di pianificazione](#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline)
* [Gli utenti rimangono sulla timeline dopo l’assegnazione di un’attività](#users-remain-on-the-timeline-after-being-assigned-a-task)

### Utilizza il filtro per controllare quali utenti vengono visualizzati nella Timeline di pianificazione {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

Il filtro può ora essere utilizzato per controllare quali utenti vengono visualizzati sulla timeline della pianificazione, oltre a quali attività e problemi vengono visualizzati nell&#39;area Non assegnata. Quando gli utenti sono selezionati nel filtro, vengono visualizzati solo gli utenti selezionati, indipendentemente dal fatto che abbiano un&#39;assegnazione di ruolo corrispondente all&#39;assegnazione di ruolo delle attività nell&#39;area Non assegnata. Vengono inoltre visualizzate tutte le attività attualmente assegnate a tale utente.

Prima di questa modifica, il filtro controllava solo le attività e i problemi visualizzati nell&#39;area Non assegnata. Gli utenti venivano visualizzati nella timeline della pianificazione solo se l’utente corrispondeva all’assegnazione del ruolo di un’attività nell’area Non assegnata.

Per ulteriori informazioni sull&#39;utilizzo del filtro per controllare ciò che viene visualizzato nella timeline della programmazione, vedi  [Filtrare le informazioni nell&#39;area Pianificazione](../../../../resource-mgmt/resource-scheduling/filter-scheduling-area.md)e  [Assegnazione manuale di attività e problemi non assegnati nelle aree di programmazione](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md#automatically-assigning-unassigned-tasks-and-issues) in [Assegnazione manuale di attività e problemi non assegnati nelle aree di programmazione](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Gli utenti rimangono sulla timeline dopo l’assegnazione di un’attività {#users-remain-on-the-timeline-after-being-assigned-a-task}

Gli utenti rimangono sulla timeline della pianificazione dopo aver ricevuto un’attività o un problema, anche se non vi sono altre attività o problemi con un’assegnazione di ruolo corrispondente. Questo consente di apportare le modifiche necessarie dopo l’assegnazione degli utenti.

Prima di questa modifica, gli utenti scompaiono dalla timeline della pianificazione immediatamente dopo l’assegnazione di un’attività o di un problema se nell’area Non assegnata non sono presenti altre attività o problemi con assegnazione di un ruolo corrispondente.

Per ulteriori informazioni, consulta  [Assegnazione manuale di attività e problemi non assegnati nelle aree di programmazione](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md#automatically-assigning-unassigned-tasks-and-issues) in [Assegnazione manuale di attività e problemi non assegnati nelle aree di programmazione](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

## Personalizzare la terminologia Workfront modificando i nomi degli oggetti

È ora possibile personalizzare la terminologia di Workfront modificando i nomi di determinati oggetti.\
Utilizzando un modello di layout, è ora possibile modificare i nomi dei seguenti oggetti di lavoro in base alle esigenze della propria organizzazione:

* Portfolio
* Programma
* Progetto
* Attività
* Problema

Ad esempio, se nella tua organizzazione lavori con campagne anziché con progetti, puoi sostituire il nome dell’oggetto &quot;Progetto&quot; con &quot;Campagna&quot;.

Quando si effettua questa sostituzione, nelle seguenti aree dell&#39;applicazione viene visualizzato il nome aggiornato degli oggetti:

* Barra di navigazione globale
* Tutte le schede
* Tutti i menu 
* Report builder ed elementi di reporting (visualizzazioni, filtri e raggruppamenti)
* Pulsanti Salva
* File esportati
* E-mail

Le aree seguenti non mostrano il nome aggiornato degli oggetti:

* Stime delle Risorse
* Gestore Budget Risorse
* Pianificazione capacità
* Tabella delle Risorse
* Assembla Squadra
* Ottimizzatore Portfolio 
* App mobili
* Componente aggiuntivo per Outlook

Per ulteriori informazioni su come personalizzare la terminologia di Workfront utilizzando un modello di layout, vedere la sezione &quot;Personalizzazione della terminologia&quot; in &quot;Creazione e gestione di modelli di layout&quot; e la sezione &quot;Informazioni sulle implicazioni della personalizzazione dei nomi oggetto&quot; in [Comprendere gli oggetti in Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Includi date di inizio e fine approvazione nei rapporti

È ora possibile includere i campi seguenti durante la creazione o la modifica dei rapporti:

* Data di inizio percorso di approvazione
* Data completamento percorso approvazione

Questi campi ti consentono di comprendere quando è stato avviato il percorso di approvazione corrente o più recente e quando è stato contrassegnato come Completo.

Per ulteriori informazioni su questi campi, consulta [Glossario della terminologia di Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Per ulteriori informazioni sui percorsi di approvazione, su come vengono creati e attivati e sulla funzione che svolgono nei processi di approvazione, consulta [Creazione di un processo di approvazione per gli elementi di lavoro](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

I campi seguenti sono stati rimossi da Workfront e non possono più essere inclusi nei rapporti (questi campi forniscono informazioni relative al progetto anziché informazioni sulle approvazioni stesse e sono stati spesso utilizzati in modo improprio):

* Approvazioni Data di inizio prevista
* Data di inizio prevista approvazione
* Data di inizio prevista approvazione

## Nuove opzioni di digest e-mail per &quot;Richieste effettuate&quot;

L’opzione di consegna Daily Digest è stata aggiunta all’area &quot;Richieste che ho effettuato&quot; delle impostazioni delle notifiche.

Per ulteriori informazioni, consulta [Attivare o disattivare le notifiche degli eventi personali](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Ricorda di aggiornare l’indirizzo e-mail associato al tuo account per poter testare questa funzionalità. Questo è necessario perché la Sandbox Anteprima cancella gli indirizzi e-mail su tutti gli utenti.

## Aspetto e notifiche e-mail di approvazione documenti aggiornate

L’aspetto della notifica per &quot;Approvazione documento&quot; è stato aggiornato con una nuova interfaccia utente:

Per ulteriori informazioni sulle notifiche e-mail, vedi [Notifiche Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).

Ricorda di aggiornare l’indirizzo e-mail associato al tuo account per poter testare questa funzionalità. Questo è necessario perché la Sandbox Anteprima cancella gli indirizzi e-mail su tutti gli utenti.

## Miglioramenti nella vista Milestone

La vista Milestone disponibile quando si visualizza un elenco di progetti o un rapporto di progetto ora contiene i seguenti miglioramenti:

* Le date pianificate sono modificabili
* Viene visualizzata la percentuale di completamento per progetti e attività

Prima di questa modifica, per modificare le date o visualizzare la percentuale di completamento, era necessario passare alla singola attività.

Per ulteriori informazioni, consulta [Utilizzare la vista Milestone](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
