---
content-type: release-notes
navigation-topic: product-releases-archive
title: Attività sulla versione 2018.1 Beta 4
description: Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.1 Beta 4. La funzionalità è stata resa disponibile nell’ambiente di anteprima il 24 gennaio 2018. Sarà disponibile nell’ambiente di produzione a marzo 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 8e016f12-bc72-475c-a8cc-38ded4351f88
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2435'
ht-degree: 0%

---

# Attività sulla versione 2018.1 Beta 4

Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.1 Beta 4. La funzionalità è stata resa disponibile nell’ambiente di anteprima il 24 gennaio 2018. Sarà disponibile nell’ambiente di produzione a marzo 2018.

>[!IMPORTANT]
>
> La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate in 2018.1, consulta  [Panoramica sull’attività della versione 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La versione 2018.1 Beta 4 contiene miglioramenti sia per gli amministratori di Workfront che per altri utenti:

**Per gli amministratori**

* [Pianificazioni gestite dagli amministratori di gruppi](#schedules-managed-by-group-administrators)

**Per tutti gli utenti**

* [Miglioramenti delle bozze in Workfront](#proofing-improvements-within-workfront)
* [Creazione di bozze in Workfront Proof: esperienza utente migliorata e funzionalità aggiuntive](#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality)
* [Miglioramenti delle bozze in Workfront e Workfront Proof](#proofing-improvements-within-workfront-and-workfront-proof)
* [Aspetto aggiornato con l’integrazione di Basecamp in Workfront Proof](#updated-look-and-feel-with-basecamp-integration-in-workfront-proof)
* [Incolla immagini in Workfront dagli Appunti](#paste-images-to-workfront-from-the-clipboard)
* [Miglioramenti al rapporto Utilizzo](#utilization-report-improvements)
* [Rimuovi l&#39;oggetto Ora preventivata risorsa da Workfront](#remove-the-resource-budgeted-hour-object-from-workfront)
* [Statistiche utilizzo report](#report-usage-statistics)
* [Aggiornamenti del Diagramma di Gantt](#gantt-chart-updates)
* [Nuovo Ottimizzatore Portfolio](#new-portfolio-optimizer)
* [Opzione di adeguamento data budget nella Programmazione risorse](#budget-date-adjustment-option-in-the-resource-planner)
* [Pianificazione risorse: limita le assegnazioni agli utenti in base all&#39;appartenenza al gruppo](#resource-scheduling-restrict-assignments-to-users-based-on-group-membership)
* [Programmazione delle risorse: consenti assegnazioni agli utenti indipendentemente dal ruolo](#resource-scheduling-allow-assignments-to-users-regardless-of-role)
* [Supporto Emoji](#emoji-support)

## Miglioramenti delle bozze in Workfront {#proofing-improvements-within-workfront}

Sono stati apportati i seguenti miglioramenti all’elenco dei documenti in Workfront: 

* [Visualizza avanzamento bozza dall&#39;elenco documenti](#view-proof-progress-from-the-document-list)
* [Nuova opzione per visualizzare il riepilogo di stampa dall&#39;elenco dei documenti](#new-option-to-view-the-print-summary-from-the-document-list)
* [Aspetto aggiornato per la generazione o l’apertura della bozza dall’elenco dei documenti](#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list)
* [Vari collegamenti rimossi dai documenti nell&#39;elenco dei documenti](#various-links-removed-from-documents-on-the-document-list)
* [Visualizza nomi file in bozze combinate](#view-file-names-on-combined-proofs)
* [Visualizzare la fase attiva corrente di una bozza dall&#39;elenco dei documenti](#view-the-current-active-stage-of-a-proof-from-the-document-list)

### Visualizza avanzamento bozza dall&#39;elenco documenti {#view-proof-progress-from-the-document-list}

Ora durante la visualizzazione dell’elenco dei documenti vengono visualizzati gli indicatori di avanzamento della bozza per tutte le bozze. (inclusi Inviato, Aperto, Commenti effettuati e Decisione).

Prima di questa modifica, per visualizzare lo stato della bozza nel pannello di destra era necessario selezionare una bozza nell’elenco del documento. 

Per ulteriori informazioni, consulta [Panoramica sullo stato e sull’avanzamento della bozza](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

### Nuova opzione per visualizzare il riepilogo di stampa dall&#39;elenco dei documenti {#new-option-to-view-the-print-summary-from-the-document-list}

È ora possibile visualizzare il riepilogo di stampa di una bozza direttamente dall’elenco dei documenti.

Prima di questa modifica, era possibile visualizzare il riepilogo di stampa solo dal visualizzatore di bozze. 

Per ulteriori informazioni sulla visualizzazione del riepilogo di stampa dall&#39;elenco dei documenti, vedere [Stampare un riepilogo delle bozze in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### Aspetto aggiornato per la generazione o l’apertura della bozza dall’elenco dei documenti {#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list}

Ora, quando si passa il mouse su un documento nell’elenco dei documenti, le opzioni per la generazione della bozza o l’apertura della bozza sono state aggiornate. Queste opzioni sono ora più evidenti e vengono visualizzate come pulsanti.

Prima di questa modifica, queste opzioni erano disponibili come collegamenti sotto il nome del documento.

Per ulteriori informazioni, vedere le sezioni seguenti:

* .
* in .

### Vari collegamenti rimossi dai documenti nell&#39;elenco dei documenti {#various-links-removed-from-documents-on-the-document-list}

Le azioni seguenti non sono più disponibili come collegamenti su singoli documenti all&#39;interno dell&#39;elenco dei documenti:

* Crea bozza
* Bozza
* Dettagli
* Condividi
* Check-Out/Check-In

Le azioni seguenti sono ora disponibili come pulsante nel documento all&#39;interno dell&#39;elenco dei documenti:

* Apri bozza (disponibile dopo la generazione della bozza) 
* Genera bozza (disponibile quando la bozza non è ancora stata generata)

Nel menu a discesa accanto al pulsante Apri bozza o Genera bozza sono ora disponibili le seguenti azioni:

* Dettagli bozza
* Dettagli Documento
* Stampa riepilogo

Per ulteriori informazioni, vedere le sezioni seguenti:

* .
* in .

### Visualizza nomi file in bozze combinate {#view-file-names-on-combined-proofs}

Ora è possibile visualizzare i singoli nomi di file che compongono una bozza combinata. Queste informazioni vengono visualizzate nella scheda Dettagli quando la bozza viene selezionata nell&#39;elenco del documento.

Per ulteriori informazioni, consulta Visualizzazione di tutti i file contenuti in una bozza combinata. 

### Visualizzare la fase attiva corrente di una bozza dall&#39;elenco dei documenti {#view-the-current-active-stage-of-a-proof-from-the-document-list}

Ora, quando si seleziona una bozza nell’elenco dei documenti, le fasi attive correnti vengono visualizzate nella colonna di destra della scheda Dettagli. 

Per ulteriori informazioni, consulta [Visualizzare le fasi attive su una bozza](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/view-active-stages-proof.md).  

## Creazione di bozze in Workfront Proof: esperienza utente migliorata e funzionalità aggiuntive {#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality}

Oltre a una migliore esperienza utente durante la creazione di bozze in Workfront Proof, ora sono disponibili le seguenti funzionalità aggiuntive:

* Unisci più immagini in un’unica bozza.
* Siti web di bozze in più risoluzioni (è possibile creare più risoluzioni come bozze singole o combinarle in un’unica bozza).
* Modifica il nome del file durante il caricamento.
* Includi campi personalizzati nel modulo di creazione bozza.
* Aggiungi un messaggio personalizzato per le notifiche e-mail delle bozze.
* Impostazioni bozza aggiuntive 
* Convalida degli errori in tempo reale durante la verifica di un URL (in precedenza era necessario attendere alcuni minuti prima della visualizzazione di un errore)

>[!NOTE]
>
>Questa nuova pagina di creazione delle bozze in Workfront Proof ora corrisponde alla pagina di creazione delle bozze che era stata recentemente resa disponibile durante la creazione di bozze in Workfront. 

Per ulteriori informazioni, consulta  [Genera bozze in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Miglioramenti delle bozze in Workfront e Workfront Proof {#proofing-improvements-within-workfront-and-workfront-proof}

Le seguenti modifiche vengono applicate quando si aggiungono documenti a Workfront e a Workfront Proof:

* [Ridimensionare l’elenco dei commenti durante l’esame delle bozze](#resize-the-comment-list-when-reviewing-proofs)
* [I Collegamenti Ipertestuali Sono Attivi Durante La Revisione Delle Bozze Statiche](#hyperlinks-are-active-when-reviewing-static-proofs)
* [Miglioramenti Durante L’Aggiunta Di Bozze](#improvements-when-adding-proofs)

### Ridimensionare l’elenco dei commenti durante l’esame delle bozze {#resize-the-comment-list-when-reviewing-proofs}

Ora è possibile ridimensionare l’elenco dei commenti quando si esaminano le bozze nel visualizzatore di bozze.

Per ulteriori informazioni, consulta in .

### I Collegamenti Ipertestuali Sono Attivi Durante La Revisione Delle Bozze Statiche {#hyperlinks-are-active-when-reviewing-static-proofs}

I collegamenti ipertestuali sono ora attivi quando si rivede una bozza statica nel visualizzatore di bozze. Fare clic su un collegamento ipertestuale per passare alla pagina collegata.

Questa funzionalità è supportata in tutti i tipi di file che contengono testo, ad esempio PDF, DOC e così via. I file di immagine non sono supportati.

### Miglioramenti Durante L’Aggiunta Di Bozze {#improvements-when-adding-proofs}

Sono disponibili i seguenti miglioramenti quando si aggiungono documenti da sottoporre a bozza. 

* Le informazioni nell’elenco Destinatari sono ora disponibili in una visualizzazione a 3 colonne, per facilitarne la visualizzazione e la modifica. 

  In precedenza, le informazioni venivano visualizzate in una visualizzazione a colonna singola, richiedendo più clic quando erano necessarie modifiche. 

  Per ulteriori informazioni, consulta in .

* Trascina uno o più destinatari da una fase del flusso di lavoro a un’altra quando utilizzi il flusso di lavoro automatico. È possibile trascinare direttamente in un&#39;area di visualizzazione oppure in un&#39;area di visualizzazione del diagramma, situata nella parte superiore della pagina.

  Per ulteriori informazioni, consulta in .

* Il diagramma del flusso di lavoro rimane visibile nella parte superiore della pagina anche durante lo scorrimento. Per impostazione predefinita, il diagramma è compresso. Espandere il diagramma per visualizzarlo completamente.

  Per ulteriori informazioni, consulta in .

* Quando si aggiunge un modello a un flusso di lavoro automatico in una bozza, viene visualizzata un’animazione di caricamento che indica che il modello è in fase di caricamento.

  Per ulteriori informazioni, consulta in .

* Le seguenti impostazioni sono state spostate dalla sezione Impostazioni bozza alla sezione Flusso di lavoro nella pagina Nuova bozza:

   * Decisore principale
   * Richiedi una sola decisione

## Aspetto aggiornato con l’integrazione di Basecamp in Workfront Proof {#updated-look-and-feel-with-basecamp-integration-in-workfront-proof}

L’aspetto dell’integrazione Basecamp con Workfront Proof è stato aggiornato. La funzionalità rimane invariata.

## Incolla immagini in Workfront dagli Appunti {#paste-images-to-workfront-from-the-clipboard}

È ora possibile aggiungere file immagine a Workfront incollando un&#39;immagine dagli Appunti di sistema.

La possibilità di incollare dagli Appunti è stata rimossa da Workfront in una versione precedente; viene reintrodotta con questa versione. Il nuovo metodo è più semplice e intuitivo.

Per ulteriori informazioni, consulta [Incolla immagini dagli Appunti](../../../../documents/managing-documents/paste-image-clipboard.md). 

## Miglioramenti al rapporto Utilizzo {#utilization-report-improvements}

Il rapporto Utilizzo contiene i seguenti miglioramenti:

* Visualizza retribuzione nel rapporto Utilizzo di un progetto

  Consente di visualizzare la Retribuzione preventivata, la Retribuzione pianificata, la Retribuzione effettiva, la Variazione preventivata e la Variazione pianificata.

* Confronto dei ricavi con i costi pianificati ed effettivi

  Consente di visualizzare il Costo pianificato o effettivo insieme alla Retribuzione pianificata. Viene inoltre visualizzato il margine (%), che viene calcolato come Ricavo - Costo / Ricavo.

* Le entrate vengono visualizzate quando si visualizza il grafico.
* Le intestazioni rimangono visibili durante lo scorrimento.

  Ora, quando si scorrono le informazioni nel rapporto Utilizzo, l’intestazione nella parte superiore del rapporto Utilizzo è sempre visibile, consentendo di comprendere più facilmente i dati nel rapporto.

  In precedenza, l’intestazione nella parte superiore del rapporto Utilizzo si allontanava dalla vista durante lo scorrimento.

* Il rapporto Utilizzo su un singolo progetto viene caricato automaticamente

  Quando si visualizza il rapporto Utilizzo su un progetto, il rapporto viene caricato automaticamente.

  Prima di questa modifica, era necessario fare clic su &quot;Esegui&quot; prima di eseguire il report.

* Prestazioni migliorate

Per ulteriori informazioni sul rapporto Utilizzo, vedere [Panoramica del rapporto Utilizzo risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Rimuovi l&#39;oggetto Ora preventivata risorsa da Workfront {#remove-the-resource-budgeted-hour-object-from-workfront}

Per risolvere i problemi relativi alle prestazioni, il campo Ore preventivate risorse è stato temporaneamente rimosso da Workfront.

Come promemoria, le ore preventivate delle risorse sono le ore preventivate per le risorse o i progetti in Pianificazione risorse. Per il momento, non è più possibile creare rapporti su questo campo nell’applicazione web o tramite l’API. Il campo verrà ripristinato in una versione futura, quando i problemi di prestazioni saranno stati risolti.

Per ulteriori informazioni sull&#39;impostazione del budget per le ore nella Programmazione delle risorse, vedere [Panoramica di Programmazione delle risorse](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md). 

## Statistiche utilizzo report {#report-usage-statistics}

In un elenco di rapporti è ora possibile visualizzare le seguenti informazioni sull’utilizzo per i rapporti di Workfront:

* Ultima visualizzazione di
* Data ultima visualizzazione
* Ultimi 10 visualizzatori
* Visualizzazioni questo mese/ trimestre/ anno
* Visualizzazioni ultimo mese/ trimestre/ anno
* Tutte le Viste

Prima di questo aggiornamento, le informazioni di utilizzo visualizzate nei rapporti erano limitate.

Per ulteriori informazioni sull’utilizzo dei rapporti, consulta [Visualizza utilizzo report](../../../../reports-and-dashboards/reports/report-usage/view-report-usage.md)

## Pianificazioni gestite dagli amministratori di gruppi {#schedules-managed-by-group-administrators}

In qualità di amministratore di gruppo, puoi creare e modificare le pianificazioni associate ai gruppi amministrati e ai relativi sottogruppi. Prima di questa modifica, solo gli amministratori di Workfront potevano creare e modificare le pianificazioni.

Per ulteriori informazioni sulla gestione delle pianificazioni, consulta [Creare una pianificazione](../../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

## Aggiornamenti del Diagramma di Gantt {#gantt-chart-updates}

Il diagramma di Gantt è ora modificabile. Tramite il diagramma di Gantt è possibile apportare i seguenti aggiornamenti alle attività:

* Creare relazioni predecessore
* Modifica durata attività
* Aggiorna la percentuale di completamento dell&#39;attività
* Applica livellamento risorse

Prima di questa modifica, era possibile rimuovere solo le relazioni dei predecessori nel diagramma di Gantt e modificare le attività solo nell&#39;elenco delle attività.

Per ulteriori informazioni sul diagramma di Gantt, vedi [Aggiorna informazioni nell&#39;elenco delle attività Diagramma di Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)

## Nuovo Ottimizzatore Portfolio {#new-portfolio-optimizer}

L’area Portfoli Optimizer di Workfront è ora aggiornata con un nuovo aspetto. La funzionalità non è stata modificata.

Per ulteriori informazioni su Ottimizzatore Portfolio, consulta [Panoramica di Portfoli Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)

## Opzione di adeguamento data budget nella Programmazione risorse {#budget-date-adjustment-option-in-the-resource-planner}

È stata aggiunta un’opzione per darti una rapida visibilità negli intervalli di tempo senza conflitti di budget. Dopo aver visualizzato quando si verificano gli intervalli di tempo senza conflitti di budget, è possibile spostare manualmente le ore preventivate in tali orari. Questo adeguerà anche le date preventivate delle ore. Prima di questo aggiornamento, non era possibile visualizzare a colpo d’occhio i conflitti di budget per un progetto.

Per ulteriori informazioni sull&#39;adeguamento delle date preventivate nella Programmazione delle risorse, vedere la sezione &quot;Adeguamento delle date preventivate&quot; nella [Panoramica di Programmazione delle risorse](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)

## Pianificazione risorse: limita le assegnazioni agli utenti in base all&#39;appartenenza al gruppo {#resource-scheduling-restrict-assignments-to-users-based-on-group-membership}

>[!NOTE]
>
>Gli strumenti di pianificazione delle risorse sono stati dichiarati obsoleti e rimossi da Workfront con la versione 23.1. Per informazioni sulla programmazione delle risorse tramite il Bilanciatore dei carichi di lavoro, consulta [Panoramica del Bilanciatore dei carichi di lavoro](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Quando si effettuano assegnazioni utente nell’area Pianificazione (come descritto in &quot;Assegnazione manuale di attività e problemi non assegnati nelle aree Pianificazione&quot;), è ora possibile configurare Workfront in modo da limitare le assegnazioni di attività e problemi solo agli utenti membri del gruppo definito sul progetto da cui ha origine l’attività o il problema. 

Ciò si applica quando si effettuano assegnazioni nei modi seguenti:

* Quando si assegna un utente a tutte le attività e ai problemi per un ruolo specifico, come descritto in &quot;Assegnare manualmente le attività e i problemi non assegnati nelle aree Pianificazione&quot;.

  Prima di questa modifica, un’attività o un problema poteva sempre essere assegnato a qualsiasi utente, indipendentemente dall’appartenenza al gruppo dell’utente. 

* Quando si scambiano le assegnazioni con un altro utente, come descritto in &quot;Assegnazione manuale di attività e problemi non assegnati nelle aree Pianificazione&quot;.

  Prima di questa modifica, un’attività o un problema poteva sempre essere assegnato a qualsiasi utente, indipendentemente dall’appartenenza al gruppo dell’utente. 

* Quando si assegna manualmente un’attività o un problema dalla timeline di programmazione, come descritto in &quot;Assegnare manualmente attività e problemi non assegnati nelle aree Programmazione&quot;.

  Prima di questa modifica, un’attività o un problema poteva sempre essere assegnato a qualsiasi utente, indipendentemente dall’appartenenza al gruppo dell’utente. 

* Quando Workfront consente di assegnare automaticamente gli utenti, come descritto in &quot;Assegnazione manuale di attività e problemi non assegnati nelle aree Pianificazione&quot;.

  Prima di questa modifica, Workfront assegnava attività e problemi agli utenti indipendentemente dall’iscrizione al gruppo.

Per ulteriori informazioni sulla configurazione di questa opzione, vedere &quot;Introduzione alla pianificazione delle risorse&quot;.

## Programmazione delle risorse: consenti assegnazioni agli utenti indipendentemente dal ruolo {#resource-scheduling-allow-assignments-to-users-regardless-of-role}

Quando si effettuano assegnazioni di utenti nell’area Pianificazione (come descritto in &quot;Assegnazione manuale di attività e problemi non assegnati nelle aree Pianificazione&quot;), ora è possibile configurare Workfront per consentire l’assegnazione di attività e problemi a qualsiasi utente, indipendentemente dal fatto che tale utente abbia un ruolo definito nel proprio profilo utente che corrisponde all’assegnazione del ruolo dell’attività o del problema che viene assegnato a lui.

Ciò si applica quando si effettuano assegnazioni nei modi seguenti:

* Quando si assegna un utente a tutte le attività e ai problemi per un ruolo specifico, come descritto in &quot;Assegnare manualmente le attività e i problemi non assegnati nelle aree Pianificazione&quot; in &quot;Assegnare manualmente le attività e i problemi non assegnati nelle aree Pianificazione&quot;.

  Prima di questa modifica, il ruolo principale dell’utente che stai assegnando doveva corrispondere al ruolo già definito nel campo Seleziona ruolo.

* Quando si scambiano le assegnazioni con un altro utente, come descritto in &quot;Assegnazione manuale di attività e problemi non assegnati nelle aree Pianificazione&quot;.

  Prima di questa modifica, il ruolo principale dell’utente che stai assegnando doveva corrispondere al ruolo già definito nel campo Seleziona ruolo.

* Quando si assegna manualmente un’attività o un problema dalla timeline di programmazione, come descritto in &quot;Assegnare manualmente attività e problemi non assegnati nelle aree Programmazione&quot;.

  Prima di questa modifica, nella timeline di pianificazione venivano visualizzati solo gli utenti il cui ruolo corrispondeva a quello dell’attività o del problema che stavi assegnando.

>[!NOTE]
>
>Ciò non si applica quando si consente a Workfront di assegnare automaticamente gli utenti, come descritto in &quot;Assegnazione manuale di attività e problemi non assegnati nelle aree Pianificazione&quot;. Quando si assegnano automaticamente gli utenti, le attività e i problemi possono essere assegnati solo agli utenti con un ruolo corrispondente.

Per ulteriori informazioni sulla configurazione di questa opzione, vedere &quot;Introduzione alla pianificazione delle risorse&quot;.

## Supporto Emoji {#emoji-support}

È ora possibile impostare il tono per i commenti e gli aggiornamenti effettuati in Workfront inserendo emoji. Eventuali emoticon aggiunte ai commenti inseriti nella scheda Aggiornamenti vengono visualizzate anche nella notifica e-mail di aggiornamento. 

Per ulteriori informazioni, consulta [Aggiorna lavoro](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
