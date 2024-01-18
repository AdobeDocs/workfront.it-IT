---
content-type: release-notes
navigation-topic: product-releases-archive
title: Anteprima R1 3
description: Questa pagina descrive tutte le modifiche disponibili nell’ambiente di anteprima con la versione R1.3. La funzionalità di questa pagina è stata resa disponibile nell’ambiente di anteprima il 1° febbraio 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1347'
ht-degree: 2%

---

# Anteprima R1 3

Questa pagina descrive tutte le modifiche disponibili nell’ambiente di anteprima con la versione R1.3. La funzionalità di questa pagina è stata resa disponibile nell’ambiente di anteprima il 1° febbraio 2017.

Per un elenco di tutte le modifiche apportate in R1, vedere [Panoramica dell’attività sulla versione R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Metodo migliorato per il collegamento di file esterni

L&#39;opzione per il collegamento di documenti da un&#39;origine esterna, ad esempio Google Drive, Box, Dropbox e così via, si trova ora in una posizione più evidente nell&#39;area Documenti. 

Inoltre, l’autorizzazione di un provider di documenti prima di collegare i file da tale provider per la prima volta è ora più intuitiva (si tratta semplicemente di un passaggio aggiuntivo quando si collegano i file da un provider esterno).

Prima di queste modifiche, l&#39;opzione per collegare i file da un&#39;origine esterna era disponibile nella finestra di dialogo Aggiungi documenti all&#39;interno dell&#39;area Documenti. Prima di collegare un documento da un’origine esterna per la prima volta, l’utente che lo collegava doveva autorizzare quel provider di documenti nell’area Setup.

Per ulteriori informazioni, consulta  [Collegare documenti da applicazioni esterne](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Calendario di lavoro del team aggiornato

>[!NOTE]
>
>Gli strumenti di pianificazione delle risorse sono stati dichiarati obsoleti e rimossi da Workfront con la versione 23.1. Per informazioni sulla programmazione delle risorse tramite il Bilanciatore dei carichi di lavoro, consulta [Panoramica del Bilanciatore dei carichi di lavoro](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Il calendario Lavori in corso disponibile per i team ora contiene funzionalità aggiuntive e un aspetto aggiornato. Il calendario Team Working On ora funziona in modo simile allo strumento di pianificazione delle risorse per i progetti.

Il calendario Team Working On aggiornato include i seguenti miglioramenti:

* Visualizza gli utenti in ordine alfabetico o raggruppati per ruolo.
* Filtra la sequenza temporale della pianificazione in base alle priorità del progetto, allo stato e ai singoli progetti. Puoi anche filtrare la timeline di pianificazione per ruoli e utenti. L’area Filtro include meno opzioni rispetto alla pianificazione delle risorse per i progetti.
* Includi problemi nella sequenza temporale di pianificazione.
* Visualizza le allocazioni utente e modifica il numero di ore assegnate agli utenti per determinate attività e problemi per ogni giorno.
* Visualizza gli indicatori che mostrano quando gli utenti sono sovrassegnati in un dato giorno.
* Consente di specificare se il lavoro completato deve essere visualizzato nella sequenza temporale di pianificazione.

Differenze rispetto allo strumento di programmazione delle risorse durante la programmazione delle risorse per i progetti:

* Tutti i membri del team vengono visualizzati nel calendario Team in esecuzione.\
  Quando si pianificano le risorse per i progetti, vengono visualizzati solo gli utenti a cui è associato un ruolo corrispondente a un ruolo di una o più attività nell’area Non assegnato.
* Lo strumento Scambia non è disponibile non è incluso nel calendario Team Working On.
* Qualsiasi membro del team può apportare modifiche al calendario Team Working On.\
  Durante la programmazione delle risorse per i progetti, solo i responsabili delle risorse possono prendere decisioni relative alle risorse per il progetto.
* I problemi vengono visualizzati per impostazione predefinita nel calendario Team Working On.\
  Quando si pianificano le risorse per i progetti, i problemi non vengono visualizzati per impostazione predefinita.

Per ulteriori informazioni sull&#39;utilizzo del calendario Team Working On aggiornato, vedere &quot;Programmazione delle risorse&quot;.

## Miglioramenti alla programmazione delle risorse

La timeline di pianificazione include i seguenti miglioramenti:

* &quot;Usa il filtro per controllare quali utenti vengono visualizzati nella timeline di pianificazione&quot;
* &quot;Gli utenti rimangono nella timeline dopo l’assegnazione di un’attività&quot;

### Utilizza il filtro per controllare quali utenti vengono visualizzati nella timeline di pianificazione {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

>[!NOTE]
>
>Gli strumenti di pianificazione delle risorse sono stati dichiarati obsoleti e rimossi da Workfront con la versione 23.1. Per informazioni sulla programmazione delle risorse tramite il Bilanciatore dei carichi di lavoro, consulta [Panoramica del Bilanciatore dei carichi di lavoro](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Ora è possibile utilizzare il filtro per controllare quali utenti vengono visualizzati nella timeline di pianificazione, oltre a quali attività e problemi vengono visualizzati nell’area Non assegnato. Quando gli utenti vengono selezionati nel filtro, vengono visualizzati solo gli utenti selezionati, indipendentemente dal fatto che abbiano un&#39;assegnazione di ruolo corrispondente all&#39;assegnazione di ruolo delle attività nell&#39;area Non assegnato. Vengono visualizzate anche tutte le attività attualmente assegnate a tale utente.

Prima di questa modifica, il filtro controllava solo quali attività e problemi venivano visualizzati nell’area Non assegnato. Gli utenti venivano visualizzati nella timeline di programmazione solo se corrispondevano all’assegnazione del ruolo di un’attività nell’area Non assegnato.

Per ulteriori informazioni sull&#39;utilizzo del filtro per controllare ciò che viene visualizzato nella sequenza temporale di pianificazione, vedere &quot;Filtrare le informazioni nell&#39;area Pianificazione&quot; e &quot;Assegnare manualmente le attività e i problemi non assegnati nelle aree Pianificazione&quot;.

### Gli utenti rimangono nella timeline dopo l’assegnazione di un’attività {#users-remain-on-the-timeline-after-being-assigned-a-task}

Gli utenti rimangono nella sequenza temporale di pianificazione dopo l’assegnazione di un’attività o di un problema, anche se non vi sono attività o problemi rimanenti con un’assegnazione di ruolo corrispondente. Questo consente di apportare tutte le modifiche necessarie dopo l’assegnazione degli utenti.

Prima di questa modifica, gli utenti scomparivano dalla timeline di pianificazione subito dopo l’assegnazione di un’attività o di un problema, se nell’area Non assegnato non vi erano attività o problemi rimanenti con un’assegnazione di ruolo corrispondente.

Per ulteriori informazioni, vedere &quot;Assegnazione manuale di attività e problemi non assegnati nelle aree Pianificazione&quot;.

## Personalizzare la terminologia di Workfront modificando i nomi degli oggetti

È ora possibile personalizzare la terminologia di Workfront modificando i nomi di alcuni oggetti.\
Utilizzando un modello di layout, è ora possibile modificare i nomi dei seguenti oggetti di lavoro in base alle esigenze dell&#39;organizzazione:

* Portfolio
* Programma
* Progetto
* Attività
* Problema

Ad esempio, se nella tua organizzazione lavori con campagne invece che con progetti, puoi sostituire il nome dell’oggetto &quot;Progetto&quot; con &quot;Campagna&quot;.

Quando si esegue questa sostituzione, nelle seguenti aree dell&#39;applicazione viene visualizzato il nome aggiornato degli oggetti:

* Barra di navigazione globale
* Tutte le schede
* Tutti i menu 
* Generatore di rapporti ed elementi di reporting (visualizzazioni, filtri e raggruppamenti)
* Pulsanti Salva
* File esportati
* E-mail

Nelle seguenti aree non viene visualizzato il nome aggiornato degli oggetti:

* Stime delle Risorse
* Gestore Budget Risorse
* Pianificazione capacità
* Tabella delle Risorse
* Assembla Squadra
* Ottimizzatore Portfolio 
* App mobili
* Componente aggiuntivo per Outlook

Per ulteriori informazioni su come personalizzare la terminologia di Workfront utilizzando un modello di layout, vedere la sezione &quot;Personalizzazione della terminologia&quot; in &quot;Creazione e gestione dei modelli di layout&quot; e la sezione &quot;Informazioni sulle implicazioni della personalizzazione dei nomi di oggetto&quot; in [Comprendere gli oggetti in Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Includi date di inizio e fine approvazione nei report

Durante la creazione o la modifica di rapporti è ora possibile includere i campi riportati di seguito.

* Data di inizio percorso di approvazione
* Data di completamento percorso di approvazione

Questi campi ti consentono di sapere quando è stato avviato il percorso di approvazione corrente o più recente e quando è stato contrassegnato come Completo.

Per ulteriori informazioni su questi campi, consulta [Glossario della terminologia di Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Per ulteriori informazioni sui percorsi di approvazione, su come vengono creati e attivati e sulla funzione che svolgono nei processi di approvazione, consulta [Creare un processo di approvazione per gli elementi di lavoro](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

I seguenti campi sono stati rimossi da Workfront e non possono più essere inclusi nei rapporti (questi campi forniscono informazioni sul progetto piuttosto che sulle approvazioni stesse, e spesso sono stati utilizzati in modo improprio):

* Approvazioni Data Inizio Pianificata
* Data di inizio prevista approvazione
* Data di inizio prevista approvazione

## Nuove opzioni di riepilogo e-mail per &quot;Richieste effettuate&quot;

L’opzione di consegna Riepilogo giornaliero è stata aggiunta all’area &quot;Richieste effettuate&quot; delle impostazioni delle notifiche.

Per ulteriori informazioni, consulta [Modifica le tue notifiche e-mail](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Ricorda di aggiornare l’indirizzo e-mail associato al tuo account per poter testare questa funzionalità. Questo è necessario perché la Sandbox di anteprima cancella gli indirizzi e-mail su tutti gli utenti.

## Aspetto aggiornato delle notifiche e-mail di approvazione del documento

L’aspetto della notifica di &quot;Approvazione documento&quot; è stato aggiornato con una nuova interfaccia:

Per ulteriori informazioni sulle notifiche e-mail, consulta [Notifiche Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).

Ricorda di aggiornare l’indirizzo e-mail associato al tuo account per poter testare questa funzionalità. Questo è necessario perché la Sandbox di anteprima cancella gli indirizzi e-mail su tutti gli utenti.

## Miglioramenti nella vista Milestone

La vista Milestone (Attività cardine) disponibile quando si visualizza un elenco di progetti o un report di progetti ora contiene i seguenti miglioramenti:

* Le date pianificate sono modificabili
* Viene visualizzata la percentuale di completamento per progetti e attività

Prima di questa modifica, per modificare le date o visualizzare la percentuale di completamento era necessario passare alla singola attività.

Per ulteriori informazioni, consulta [Utilizzare la vista Milestone](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
