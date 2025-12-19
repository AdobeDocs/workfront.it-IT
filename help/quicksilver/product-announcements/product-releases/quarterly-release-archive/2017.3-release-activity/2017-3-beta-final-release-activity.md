---
content-type: release-notes
navigation-topic: product-releases-archive
title: Attività sulla versione finale 2017.3 di Beta
description: Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione finale 2017.3 di Beta. La funzionalità in questa pagina è stata resa disponibile nell’ambiente di anteprima il 12 settembre 2017. Sarà disponibile nell’ambiente di produzione all’inizio di novembre 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 880828f4-3908-4ef0-ab1f-774f8dee72b6
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '3791'
ht-degree: 0%

---

# Attività sulla versione finale 2017.3 di Beta

Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione finale 2017.3 di Beta. La funzionalità in questa pagina è stata resa disponibile nell’ambiente di anteprima il 12 settembre 2017. Sarà disponibile nell’ambiente di produzione all’inizio di novembre 2017.

>[!IMPORTANT]
>
> La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate nel 2017.3, consulta  Panoramica sull&#39;attività della versione [2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

La versione finale 2017.3 di Beta contiene miglioramenti sia per gli amministratori di Workfront che per altri utenti:

**Per Amministratori**

* [Nuova configurazione per il richiamo di richieste nell&#39;area Impostazioni approvazione](#new-configuration-for-recalling-requests-in-the-approval-settings-area)
* [Configurare i ruoli di bozza predefiniti](#configure-default-proof-roles)

**Per Tutti Gli Utenti**

* [Area Home (Area di lavoro personale aggiornata)](#home-area-updated-my-work-area)

* [Modello di layout aggiornato per supportare l&#39;area Home](#updated-layout-template-to-support-the-home-area)

* [Kanban per Agile](#kanban-for-agile)
* [Includi problemi nel backlog Scrum per un team Agile](#include-issues-on-the-scrum-backlog-for-an-agile-team)
* [Includi problemi nella bacheca delle storie di Scrum Agile](#include-issues-on-the-scrum-agile-story-board)
* [Applica raggruppamenti e filtri al backlog per un team Agile](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [Funzionalità @Tagging avanzate restituite nell&#39;ambiente di anteprima](#enhanced-tagging-functionality-returns-in-the-preview-environment)
* [Filtra aggiornamenti di sistema nel flusso di aggiornamento ora è persistente tra gli oggetti](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Visualizza dati nel report utilizzo](#visualize-data-in-the-utilization-report)
* [Miglioramento prestazioni report utilizzo](#utilization-report-performance-improvement)
* [Miglioramenti ai documenti: interfaccia semplificata](#document-enhancements-streamlined-interface)
* [Miglioramenti delle bozze in Workfront](#proofing-enhancements-within-workfront)
* [Miglioramenti delle bozze in Workfront Proof e Workfront](#proofing-enhancements-within-both-workfront-proof-and-workfront)
* [Formattazione RTF per aggiornamenti e e-mail](#rich-text-formatting-for-updates-and-emails)
* [Nuova riprogettazione del grafico Gantt](#new-gantt-chart-redesign)
* [I Rapporti Incorporati Contengono Descrizioni Aggiornate](#built-in-reports-contain-updated-descriptions)
* [Branding in report, elenchi e dashboard esportati](#branding-in-exported-reports-lists-and-dashboards)
* [Miglioramenti durante la copia delle attività e lo spostamento di attività o problemi](#improvements-when-copying-tasks-and-moving-tasks-or-issues)
* [Nuovo raggruppamento per rapporti ore preventivate risorse: data di allocazione](#new-grouping-for-resource-budgeted-hour-reports-allocation-date)
* [Miglioramenti alla pianificazione delle risorse](#resource-planner-improvements)
* [Miglioramenti per dispositivi mobili](#mobile-improvements)
* Integrazione di [Workfront con Slack](#workfront-integration-with-slack)
* [Miglioramenti di Outlook 365](#outlook-365-improvements)
* [Modifiche API](#api-changes)

## Area Home (area di lavoro personale aggiornata) {#home-area-updated-my-work-area}

>[!NOTE]
>
>Questa funzionalità non verrà rilasciata nell’ambiente di produzione con la versione 17.3, ma rimarrà in anteprima fino all’inizio del 2018.

La nuova area Home offre una visualizzazione alternativa migliorata degli stessi dati attualmente disponibili nell&#39;area Il mio lavoro. L&#39;area Home offre i seguenti vantaggi rispetto all&#39;area Il mio lavoro:

* Un&#39;interfaccia più semplice e intuitiva
* Prestazioni migliorate

La seguente funzionalità è disponibile nell’area Il mio lavoro ma non è ancora implementata nell’area Home:

* Visualizzare il calendario personale
* Aggiornare attività e problemi con la formattazione del testo RTF
* Approvare le bozze
* Visualizza un elenco di lavori inviati per l&#39;approvazione
* Creare un problema ad hoc su un progetto
* Visualizza solo le approvazioni delegate all&#39;utente

Per ulteriori informazioni sull&#39;utilizzo della nuova area Home, vedere [Utilizzare l&#39;area Home](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Modello di layout aggiornato per supportare l’area Home {#updated-layout-template-to-support-the-home-area}

>[!NOTE]
>
>Questa funzionalità non verrà rilasciata nell’ambiente di produzione con la versione 17.3, ma rimarrà in anteprima fino all’inizio del 2018.

In qualità di amministratore di Workfront, puoi determinare se gli utenti dell’organizzazione hanno accesso all’area Home configurando il modello di layout a cui sono assegnati. Gli utenti ai quali non è assegnato un modello di layout possono sempre accedere all’area Home.

Per ulteriori informazioni, vedere &quot;Personalizzazione della home&quot; in &quot;Creazione e gestione dei modelli di layout&quot;.

## Kanban per Agile  {#kanban-for-agile}

I team Agile possono ora utilizzare una metodologia Kanban in Workfront, oltre alla metodologia Scrum Agile già supportata.

Le metodologie Scrum e Kanban Agile in Workfront differiscono nei seguenti modi:

**Vantaggi dell&#39;utilizzo di Kanban in Workfront**

* Visualizza il backlog sullo storyboard Kanban Agile.

  Per ulteriori informazioni, consulta in .

* Configura gli elementi nel backlog da aggiungere automaticamente allo storyboard Kanban Agile quando gli altri elementi vengono spostati in uno stato che equivale a Completato.

  Per ulteriori informazioni, vedere [Configurare i brani da aggiungere automaticamente dal backlog](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) in [Configurare Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configurare un limite WIP da visualizzare sullo storyboard Kanban Agile.

  Per ulteriori informazioni, vedere [Configurare il limite WIP](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) in [Configurare Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

**Vantaggi dell&#39;utilizzo di Scrum in Workfront**

* Aggiungi un set di storie a un’iterazione Agile e crea una bacheca delle storie per tale iterazione.
* Includi problemi nella bacheca delle storie Scrum.
* Includi i problemi nel backlog di un team Agile.

  Per ulteriori informazioni, vedere [Configurare le modalità di applicazione delle date quando si aggiungono elementi di lavoro a un&#39;iterazione](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) in [Configurare Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* Le sottoattività possono essere visualizzate sullo storyboard Scrum.
* Visualizzare un grafico a burn-down per visualizzare i progressi rispetto alle storie durante l&#39;iterazione.

  Per ulteriori informazioni, vedere [Panoramica del grafico a burn-down Agile](../../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

Per ulteriori informazioni sull&#39;abilitazione e la configurazione di Kanban per un team Agile, vedere [Decidere su una metodologia Agile](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md#deciding) in [Creare un team Agile](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

## Includi problemi nel backlog Scrum per un team Agile {#include-issues-on-the-scrum-backlog-for-an-agile-team}

>[!NOTE]
>
>Questa funzionalità è stata rimossa dall’ambiente di produzione il 14 novembre 2017. È previsto che venga reintrodotto nell’ambiente di anteprima all’inizio del 2018 con un design migliorato e una maggiore stabilità. Sarà disponibile nell’ambiente di produzione con la versione 2018.1.

Ora puoi includere i problemi nel backlog del team Agile quando utilizzi la metodologia Scrum Agile (i problemi non vengono visualizzati nel backlog di un team Agile quando si utilizza la metodologia Kanban). I team Scrum Agile esistenti devono abilitare questa funzionalità per includere i problemi. I problemi vengono inclusi automaticamente nel backlog per i team Scrum Agile creati dopo la versione 2017.3.

Prima di questa modifica, era possibile aggiungere al backlog solo le attività. Se desideri aggiungere un problema, devi prima convertirlo in un’attività prima di poterlo aggiungere.

Poiché ora è possibile accedere a più attività del backlog, tutte le visualizzazioni delle attività personalizzate disponibili in precedenza nel backlog vengono copiate e aggiunte al backlog come visualizzazioni personalizzate degli elementi di lavoro del backlog.

Per informazioni sull’utilizzo dei problemi nel backlog, consulta  [Gestione del backlog Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

Per informazioni sull’abilitazione della disponibilità dei problemi nel backlog di un team Scrum di Agile, consulta  [Configurare le modalità di applicazione delle date quando si aggiungono elementi di lavoro a un&#39;iterazione](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) in [Configurare Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Includi problemi nella bacheca delle storie di Scrum Agile {#include-issues-on-the-scrum-agile-story-board}

>[!NOTE]
>
>Questa funzionalità è stata rimossa dall’ambiente di produzione il 14 novembre 2017. È previsto che venga reintrodotto nell’ambiente di anteprima all’inizio del 2018 con un design migliorato e una maggiore stabilità. Sarà disponibile nell’ambiente di produzione con la versione 2018.1.

Ora puoi includere problemi nella bacheca delle storie quando utilizzi la metodologia Scrum Agile.

Per ulteriori informazioni, vedere [Configurare le colonne di stato sulla bacheca delle storie Agile](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur2) in [Configurare Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Applicare raggruppamenti e filtri al backlog per un team agile {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

>[!NOTE]
>
>Questa funzionalità è stata rimossa dall’ambiente di produzione il 14 novembre 2017. È previsto che venga reintrodotto nell’ambiente di anteprima all’inizio del 2018 con un design migliorato e una maggiore stabilità. Sarà disponibile nell’ambiente di produzione con la versione 2018.1.

Le opzioni Raggruppamento e Filtro sono ora disponibili nel backlog Agile, consentendoti di organizzare il backlog per raggruppamenti e di filtrare per attività e problemi specifici.

Prima di questa modifica, era possibile applicare sulle viste il backlog Agile.

Per ulteriori informazioni, consulta  [Gestione del backlog Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) in  [Gestione del backlog Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Formattazione Rich Text per aggiornamenti e e-mail {#rich-text-formatting-for-updates-and-emails}

>[!NOTE]
>
>Le modifiche di formattazione apportate nell’ambiente di anteprima potrebbero tornare allo stato non formattato.

È ora possibile evidenziare informazioni importanti formattando i commenti e gli aggiornamenti apportati agli oggetti di Workfront. 

Gli strumenti Testo formattato consentono di applicare attributi di formattazione al testo, creare elenchi puntati e numerati e aggiungere collegamenti ipertestuali ad altre risorse.

La formattazione applicata ai commenti nel flusso di aggiornamento viene visualizzata anche nelle notifiche e-mail di aggiornamento. Per ulteriori informazioni sulla formattazione dei commenti, vedere [Aggiorna lavoro](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Funzionalità @Tagging migliorate restituite nell’ambiente di anteprima {#enhanced-tagging-functionality-returns-in-the-preview-environment}

È possibile utilizzare nuovamente il simbolo @ per assegnare tag ad altri utenti nel flusso di aggiornamento di tutti gli oggetti nell&#39;ambiente di anteprima. In passato @tagging inserito il nome e il cognome dell’utente taggato nel flusso di aggiornamento. Ora la funzionalità di @tagging avanzata visualizza solo il nome dell’utente. Per ulteriori informazioni sui tag degli utenti negli aggiornamenti, consulta [Assegnare tag ad altri utenti negli aggiornamenti](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Filtra aggiornamenti di sistema nel flusso di aggiornamento ora è persistente tra gli oggetti {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

L’opzione Filtra aggiornamenti sistema è ora persistente tra gli oggetti in tutto il sito Workfront. Questo consente di nascondere gli aggiornamenti di sistema e visualizzare solo i commenti degli utenti nel flusso di aggiornamento su un oggetto e di mantenere tale impostazione mentre si passa ad altri oggetti.

Prima di questa modifica, era necessario scegliere di filtrare gli aggiornamenti di sistema per ogni oggetto durante l&#39;esplorazione del sito Workfront.

Per ulteriori informazioni, vedere [Aggiorna lavoro](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Visualizzare i dati nel rapporto Utilizzo {#visualize-data-in-the-utilization-report}

 È ora possibile visualizzare le informazioni sull&#39;utilizzo in una visualizzazione grafico. 

Per ulteriori informazioni, vedere [Panoramica del report sull&#39;utilizzo delle risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Panoramica del report sull&#39;utilizzo delle risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Miglioramento delle prestazioni dei rapporti sull&#39;utilizzo {#utilization-report-performance-improvement}

>[!NOTE]
>
>Questa funzione è stata rilasciata in una patch dopo il rilascio finale di Beta.

Ora, quando si esegue un rapporto Utilizzo, viene richiesto di applicare un filtro prima che venga eseguito il rapporto. Questa modifica assicura che le informazioni più pertinenti vengano generate nel rapporto Utilizzo il più rapidamente possibile.

Per ulteriori informazioni sull&#39;esecuzione di un report Utilizzo, vedere [Panoramica del report Utilizzo risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Panoramica del report Utilizzo risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Miglioramenti dei documenti: interfaccia semplificata {#document-enhancements-streamlined-interface}

L’esperienza utente per aggiungere documenti a Workfront è ora più semplice e intuitiva. Ora puoi caricare un documento dal file system, richiedere un documento o collegare un file da un’applicazione di terze parti (come Google o Dropbox), il tutto da un semplice menu a discesa. 

In precedenza, queste opzioni erano disponibili avviando la finestra di dialogo Aggiungi documenti. 

Per ulteriori informazioni, vedere le informazioni seguenti:

* [Aggiungi documenti ad Adobe Workfront dal file system](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)
* [Richiedi un documento](../../../../documents/adding-documents-to-workfront/request-a-document.md)
* [Collega documenti da applicazioni esterne](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) 

>[!NOTE]
>
>Con questa modifica, l’opzione per incollare un’immagine o un documento dagli Appunti non è più disponibile.

## Miglioramenti delle bozze in Workfront {#proofing-enhancements-within-workfront}

* [Esperienza utente migliorata e funzionalità aggiuntive](#improved-user-experience-and-additional-functionality)
* [Condividi direttamente dal visualizzatore di bozze](#share-directly-from-the-proofing-viewer)
* [Configurare i ruoli di bozza predefiniti](#configure-default-proof-roles)

### Esperienza utente migliorata e funzionalità aggiuntive {#improved-user-experience-and-additional-functionality}

Oltre a una migliore esperienza utente durante la creazione delle bozze in Workfront, ora sono disponibili le seguenti funzionalità aggiuntive:

* Unisci più immagini in un’unica bozza.
* Siti web di bozze in più risoluzioni (è possibile creare più risoluzioni come bozze singole o combinarle in un’unica bozza).
* Modifica il nome del file durante il caricamento.
* Includi campi personalizzati nel modulo di creazione bozza.
* Aggiungi un messaggio personalizzato per le notifiche e-mail delle bozze.
* Impostazioni bozza aggiuntive 
* Convalida degli errori in tempo reale durante la verifica di un URL (in precedenza era necessario attendere alcuni minuti prima della visualizzazione di un errore)

Per ulteriori informazioni, consulta .

>[!NOTE]
>
> Quando si crea una nuova bozza con un flusso di lavoro automatizzato, il trascinamento della selezione non è supportato per lo spostamento degli utenti da una fase all’altra. Al contrario, rimuovi l’utente da un passaggio e aggiungilo a un altro.

*Con la versione 2018.1 verrà reintrodotta l&#39;opzione di spostamento degli utenti da un passaggio all&#39;altro mediante trascinamento della selezione.*

### Condividi direttamente dal visualizzatore di bozze {#share-directly-from-the-proofing-viewer}

Ora è possibile condividere con utenti specifici di Workfront direttamente dal visualizzatore di bozze.

>[!NOTE]
>
>Questa funzionalità è disponibile solo per le nuove bozze (bozze create dopo la versione 2017.3) e solo per le istanze di Workfront integrate con un account Workfront Proof Premium.

Prima di questa modifica, era possibile condividere solo creando un collegamento e condividerlo con un utente. 

Per ulteriori informazioni, vedere [Condividi una bozza in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Condividi una bozza in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

### Configurare i ruoli di bozza predefiniti {#configure-default-proof-roles}

Ora puoi configurare i ruoli di bozza predefiniti di cui i nuovi utenti e gli utenti guest devono disporre per le nuove bozze all’interno del sistema Workfront. 

Questo è il ruolo predefinito a cui vengono assegnati gli utenti su una bozza quando questa viene condivisa con loro. 

## Miglioramenti delle bozze in Workfront Proof e Workfront {#proofing-enhancements-within-both-workfront-proof-and-workfront}

* [Riavvia e salta nel visualizzatore di bozze video di HTML5 (scelte rapide da tastiera)](#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts)
* [Aggiornamenti del visualizzatore di bozze di HTML5](#html5-proofing-viewer-updates)

### Riavvia e salta nel visualizzatore di verifica video HTML5 (scelte rapide da tastiera) {#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts}

Nel visualizzatore di bozze di HTML5 per i video sono ora disponibili scelte rapide da tastiera che consentono di riavviare il video dall’inizio e passare alla fine.

Per ulteriori informazioni sulle scelte rapide da tastiera disponibili, vedere [Scelte rapide da tastiera nel visualizzatore di bozze di Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/keyboard-shortcuts.md).

### Aggiornamenti del visualizzatore di bozze di HTML5 {#html5-proofing-viewer-updates}

Il visualizzatore HTML5 ora supporta le bozze statiche.

Prima di questa modifica, il visualizzatore HTML5 supportava solo bozze video. 

Il visualizzatore HTML include le seguenti nuove funzionalità durante la verifica del contenuto statico:

* Creare un singolo commento con markup su più pagine in visualizzazione Singola

  In precedenza era possibile solo nella vista Continuous (Continuo) o Magazine (Rivista)

* Navigare tra le bozze tramite le miniature delle bozze

   * Identifica facilmente la parte della bozza che viene esaminata. Questo è importante, soprattutto quando gli utenti lavorano con bozze di formato più grandi e pagine web lunghe, o in qualsiasi momento  è necessario un livello di zoom più grande per visualizzare i dettagli.
   * Modificare il livello di zoom
   * Sposta il contenuto

* Specificare valori personalizzati nello strumento di misurazione
* Quando si annota del testo all’interno di una bozza nel visualizzatore di bozze di Workfront Proof, è possibile includere opzioni per indicare che il testo deve essere in grassetto, in corsivo e sottolineato.

Il visualizzatore HTML5 non supporta ancora tutte le funzionalità attualmente disponibili nel visualizzatore Flash esistente. Le seguenti funzionalità non sono attualmente disponibili ma saranno incluse in una versione futura:

* Supporto di file rich media
* Modalità di confronto (video e statica)
* Filtra commenti (video e statici)
* Esaminare i collegamenti ipertestuali nei documenti (statici)
* Traduzioni (video e statiche)
* Indicatore di presenza che mostra gli utenti che stanno attualmente lavorando sulla bozza
* Condividi bozze

Per ulteriori informazioni sulla verifica delle bozze statiche nel visualizzatore HTML5, consulta .

In qualità di amministratore di Workfront in Workfront Proof, puoi determinare se gli utenti dell’organizzazione hanno accesso al nuovo visualizzatore di bozze di HTML5 per le bozze video.

## Nuova riprogettazione del diagramma di Gantt {#new-gantt-chart-redesign}

Il nuovo diagramma di Gantt include i seguenti miglioramenti:

* Nuove icone e marcatori
* Nuova opzione per ingrandire e ridurre un intervallo di tempo specifico
* Celle attività più piccole nella parte elenco del grafico
* Sono state riprogettate le opzioni per le impostazioni, la stampa e il passaggio a Date previste.

Per ulteriori informazioni sulla configurazione delle opzioni nel diagramma di Gantt, vedere [Configurare la modalità di visualizzazione delle informazioni nel diagramma di Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## I Rapporti Incorporati Contengono Descrizioni Aggiornate {#built-in-reports-contain-updated-descriptions}

Abbiamo aggiornato le descrizioni dei rapporti di sistema in Workfront, per includere informazioni sul tipo di rapporto e sui campi inclusi.  

Prima di questa modifica, la maggior parte dei rapporti incorporati non conteneva descrizioni o ne conteneva una molto limitata.

Per ulteriori informazioni sui report incorporati, vedere [Utilizzare i report incorporati di Adobe Workfront](../../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Branding in report, elenchi e dashboard esportati {#branding-in-exported-reports-lists-and-dashboards}

>[!NOTE]
>
>Questa funzione non è attualmente disponibile in tutti i cluster nell’ambiente di anteprima.

Se utilizzi il branding in Workfront, il logo utilizzato nella barra di navigazione globale è ora incluso nei file .pdf esportati da Workfront.

I seguenti file .pdf includeranno il logo della tua organizzazione nel documento esportato:

* Elenchi esportati
* Report esportati e consegnati
* Dashboard stampati

Per ulteriori informazioni sull&#39;esportazione di dati da Workfront, vedere [Esporta dati](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Miglioramenti durante la copia delle attività e lo spostamento di attività o problemi {#improvements-when-copying-tasks-and-moving-tasks-or-issues}

È stato migliorato il modo in cui si copia un’attività o si sposta un’attività o un problema, per facilitare la selezione di un elemento principale per l’attività o il problema copiato o spostato. Quando si seleziona un elemento padre durante la copia di un&#39;attività, ad esempio, è ora possibile visualizzare una gerarchia di attività, con la relativa relazione padre-figlio, nonché cercare un elemento padre nei progetti con numerose attività.

Prima di questa modifica, nel passaggio **Seleziona elemento padre** non era presente alcun campo di ricerca e la gerarchia delle attività non era visibile nell&#39;elenco delle attività.

Per ulteriori informazioni sulla copia delle attività, vedere [Copia e duplica attività](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Per ulteriori informazioni sullo spostamento dei problemi, vedi [Sposta problemi](../../../../manage-work/issues/manage-issues/move-issues.md).

## Nuova configurazione per Richiamo richieste nell&#39;area Impostazioni approvazione {#new-configuration-for-recalling-requests-in-the-approval-settings-area}

Nell’area Impostazioni approvazione a livello di sistema è stata introdotta una nuova impostazione che consente agli amministratori di Workfront di decidere se consentire agli utenti di richiamare un problema o una richiesta il cui primo stato è In attesa di approvazione. Se il richiamo è consentito, il problema viene eliminato; se il richiamo non è consentito, gli utenti non possono visualizzare un pulsante Richiama quando il primo stato di un problema è in attesa di approvazione.

Prima di questa modifica, era sempre consentito richiamare la pagina. Quando l’approvazione è stata richiamata, l’approvazione è stata completamente ignorata, ponendo il problema al suo primo stato, senza approvazione allegata.

Per ulteriori informazioni sulle impostazioni di approvazione, vedere [Configurare le impostazioni di approvazione globali](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md). 

>[!NOTE]
>
>Questa opzione verrà disabilitata per impostazione predefinita al rilascio di questa funzione. Il richiamo dei problemi è attualmente abilitato per impostazione predefinita per tutte le organizzazioni. Quando questa funzione viene rilasciata, l’amministratore di Workfront deve abilitare manualmente questa impostazione per mantenere la funzionalità invariata in Workfront.

## Nuovo raggruppamento per i rapporti Ore preventivate risorsa: data di allocazione {#new-grouping-for-resource-budgeted-hour-reports-allocation-date}

È stata aggiunta la possibilità di raggruppare i risultati per data di allocazione quando si crea un rapporto Ora risorse preventivate.

Prima di questa modifica, era possibile visualizzare la Data di allocazione nella visualizzazione del rapporto e utilizzarla in un filtro, ma non era possibile utilizzare questo campo in un raggruppamento.

Per ulteriori informazioni sulla data di allocazione, consulta [Glossario della terminologia di Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Per ulteriori informazioni sulla creazione di un report, vedere [Creare un report personalizzato](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Miglioramenti alla programmazione delle risorse {#resource-planner-improvements}

* [Pianificazione risorse: mostra dati per FTE](#resource-planner-show-data-by-fte)
* [Pianificazione risorse: mostra dati per settimana e trimestre](#resource-planner-show-data-by-week-and-quarter)
* [Pianificazione risorse: visualizzazione per utente](#resource-planner-view-by-user)
* [Pianificazione risorse: trascina i progetti per stabilire la priorità](#resource-planner-drag-and-drop-projects-to-establish-priority)
* [Pianificazione risorse: esporta in Excel i dati presenti nella Pianificazione risorse](#resource-planner-export-the-data-in-the-resource-planner-to-excel)

### Pianificazione risorse: Mostra dati per FTE {#resource-planner-show-data-by-fte}

Ora è possibile visualizzare l’allocazione e la disponibilità delle risorse in base all’FTE nella Programmazione delle risorse. Prima di questa modifica, era possibile visualizzare i valori solo in ore.

Per ulteriori informazioni sull&#39;utilizzo della Programmazione delle risorse, vedere [Panoramica sulla programmazione delle risorse](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Pianificazione risorse: Mostra dati per settimana e trimestre {#resource-planner-show-data-by-week-and-quarter}

È ora possibile modificare l&#39;intervallo di tempo per la programmazione delle risorse in modo da visualizzarlo per settimana o trimestre. Prima di questa modifica, era possibile visualizzare l&#39;allocazione e la disponibilità delle risorse e preventivarle solo per mese.

Per ulteriori informazioni sull&#39;utilizzo della Programmazione delle risorse, vedere [Panoramica sulla programmazione delle risorse](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Pianificazione risorse: Visualizza per utente {#resource-planner-view-by-user}

Ora è possibile visualizzare le informazioni nella Programmazione delle risorse per utente, prima, quindi per progetti, ruoli e attività. Puoi anche visualizzare una differenza tra le ore pianificate e le ore disponibili o FTE per gli utenti. Prima di questa modifica, era possibile visualizzare le informazioni nella Programmazione delle risorse per progetti e ruoli.

Per ulteriori informazioni sull&#39;utilizzo della Programmazione delle risorse, vedere [Panoramica sulla programmazione delle risorse](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Programmazione delle risorse: trascinamento dei progetti per stabilire la priorità {#resource-planner-drag-and-drop-projects-to-establish-priority}

Ora puoi trascinare e rilasciare i progetti nell’ordine di priorità desiderato. Prima di questa modifica, era possibile stabilire la priorità dei progetti solo assegnando manualmente un numero.

Per ulteriori informazioni sull&#39;utilizzo della Programmazione delle risorse, vedere [Panoramica sulla programmazione delle risorse](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Pianificazione risorse: esporta in Excel i dati presenti nella Pianificazione risorse {#resource-planner-export-the-data-in-the-resource-planner-to-excel}

È ora possibile esportare le informazioni nella Programmazione delle risorse in un file Excel.

Per ulteriori informazioni sull&#39;utilizzo della Programmazione delle risorse, vedere [Panoramica sulla programmazione delle risorse](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Miglioramenti per dispositivi mobili {#mobile-improvements}

Abbiamo aggiunto la possibilità di accedere ai tuoi progetti e gestirli dall’app mobile di Workfront. Ora tramite l’app mobile Workfront puoi effettuare le seguenti operazioni:

* Accedere a un elenco dei progetti
* Accedere a un elenco di attività e sottoattività in un progetto
* Accedere a un elenco di problemi su un progetto
* Segnala un nuovo problema su un progetto

Puoi installare questa funzionalità quando aggiorni l’app mobile Workfront. L’aggiornamento sarà disponibile negli store mobili Apple e Android a novembre 2017.

## Integrazione di Workfront con Slack {#workfront-integration-with-slack}

>[!NOTE]
>
>L’integrazione con Slack non è attualmente disponibile. Sarà disponibile per l’utilizzo con il tuo ambiente di produzione a novembre 2017.

Stiamo lanciando una nuova integrazione tra Workfront e Slack. Se la tua organizzazione ha già utilizzato Slack per le comunicazioni, ora puoi integrarlo con Workfront ed eseguire azioni comuni di Workfront senza uscire dai canali di comunicazione in Slack. Ora puoi eseguire le seguenti azioni dal tuo account Slack:

* Cerca un elemento in Workfront
* Accedere agli elenchi di lavoro e di approvazione
* Creare un’attività
* Crea un problema
* Sottoscrivi qualsiasi elemento da un collegamento condiviso con te a tale elemento
* Assegna attività e problemi da un collegamento condiviso con te
* Approva il tuo lavoro
* Accedere agli elenchi Preferiti e Elementi recenti

Per ulteriori informazioni sull&#39;accesso a Workfront da Slack, vedere [Utilizzo di Workfront con Slack.](https://support.workfront.com/hc/en-us/sections/115000458033)

## Miglioramenti di Outlook 365 {#outlook-365-improvements}

Sono stati apportati i seguenti miglioramenti al componente aggiuntivo Workfront per  Outlook 365:

* Aggiungere un’attività o un problema a un progetto in Workfront: ora è possibile convertire un’e-mail in un’attività o un problema in Workfront utilizzando il componente aggiuntivo Outlook 365. In questo processo, puoi specificare un progetto a cui desideri aggiungere l’attività o il problema, nonché un assegnatario e una data di scadenza. Prima di questo miglioramento, era possibile inviare una richiesta solo a una coda di richieste o aggiungere un’attività personale all’elenco Lavori in Outlook 365. 
* Mantenere un collegamento agli oggetti di Workfront nell&#39;e-mail originale convertito in attività, problemi o richieste: quando si converte un messaggio e-mail da Outlook 365 a un&#39;attività, un problema o una richiesta, Outlook 365 mantiene un collegamento all&#39;attività o al problema convertito da tale messaggio e-mail nell&#39;e-mail originale. Prima di questa modifica, in Outlook non era indicato se un messaggio e-mail fosse stato convertito in un’attività o inviato come richiesta. 

## Modifiche API {#api-changes}

* [API 8 ora disponibile](#api-8-now-available)
* [Versioni rimosse e obsolete dell&#39;API](#removed-and-deprecated-versions-of-the-api)
* [Attività sulla versione finale di Beta 2017.3](#updated-message-format-for-event-subscriptions)
* [Tentativi di sottoscrizione eventi per messaggi non recapitabili](#event-subscription-retries-for-undeliverable-messages)

### API 8 ora disponibile {#api-8-now-available}

È ora disponibile la versione 8 dell’API di Workfront, che offre risorse nuove e aggiornate per le integrazioni Workfront.

Per un elenco delle modifiche apportate all&#39;API Workfront, vedere [Aggiornamenti alla versione 8](../../../../wf-api/api/new-api-version-8-updates.md) dell&#39;API.

### Versioni rimosse e obsolete dell’API {#removed-and-deprecated-versions-of-the-api}

### È stato aggiornato il formato dei messaggi per le sottoscrizioni agli eventi

Per fornire informazioni più utili per le integrazioni che includono l’API Workfront Event Subscriptions, abbiamo modificato il formato dei messaggi in uscita per le risorse supportate includendo i valori vecchi e nuovi associati a tali risorse. Per evitare errori, tutte le integrazioni disponibili che utilizzano l&#39;API sottoscrizioni eventi di Workfront dovranno essere aggiornate nel nuovo formato, come descritto in [API sottoscrizioni eventi](../../../../wf-api/general/event-subs-api.md).

### Tentativi di sottoscrizione eventi per messaggi non recapitabili {#event-subscription-retries-for-undeliverable-messages}

Il framework Workfront Event Subscription ora fornisce un meccanismo per gestire i messaggi in uscita attivati da eventi che non vengono consegnati agli endpoint del cliente. Per garantire la consegna continua dei messaggi, i clienti devono assicurarsi che tutti gli endpoint che utilizzano messaggi in uscita dalle sottoscrizioni di eventi siano configurati correttamente. Per ulteriori informazioni, vedere [Nuovi tentativi di sottoscrizione evento](../../../../wf-api/api/event-sub-retries.md).
