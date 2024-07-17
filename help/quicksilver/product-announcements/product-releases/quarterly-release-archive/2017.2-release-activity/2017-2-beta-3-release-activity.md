---
content-type: release-notes
navigation-topic: product-releases-archive
title: Attività sulla versione 2017.2 di Beta 3
description: Questa pagina descrive tutte le modifiche disponibili nell’ambiente di anteprima con la versione 2017.2 di Beta 2. La funzionalità di questa pagina è stata resa disponibile nell’ambiente di anteprima il 24 maggio 2017. Sarà disponibile nell’ambiente di produzione tra la fine di luglio e l’inizio di agosto 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9647f3c6-f287-426c-a5e7-eb33b8b22a34
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 0%

---

# Attività sulla versione 2017.2 di Beta 3

Questa pagina descrive tutte le modifiche disponibili nell’ambiente di anteprima con la versione 2017.2 di Beta 2. La funzionalità di questa pagina è stata resa disponibile nell’ambiente di anteprima il 24 maggio 2017. Sarà disponibile nell’ambiente di produzione tra la fine di luglio e l’inizio di agosto 2017.

>[!IMPORTANT]
>
>La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate in 2017.2, consulta [Panoramica delle attività sulla versione 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

La versione 2017.2 di Beta 2 contiene miglioramenti sia per gli amministratori di Workfront che per altri utenti:

**Per gli amministratori:**

* [Ripristino di elementi in blocco dal Cestino](#restoring-items-in-bulk-from-the-recycle-bin)
* [Le informazioni utente vengono sincronizzate da Workfront a ProofHQ (ProofHQ e Workfront)](#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront)

**Per Tutti Gli Utenti:** 

* [Visualizza utenti sottoscritti](#view-subscribed-users)
* [Configura la visualizzazione delle attività cardine nel Diagramma di Gantt](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Includi la legenda del diagramma di Gantt durante l&#39;esportazione in PDF](#include-the-gantt-chart-legend-when-exporting-to-pdf)
* [Visualizza approvazioni bozze nell&#39;area Il mio lavoro (Workfront)](#view-proof-approvals-in-the-my-work-area-workfront)
* [Visualizza i nomi utente quando si gestiscono le richieste di approvazione delle bozze dall&#39;area di lavoro personale (Workfront)](#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront)
* [Visualizzatore di bozze migliorato per le bozze video (ProofHQ e Workfront)](#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront)
* [Visualizzare le bozze rich media in risoluzioni alternative (ProofHQ e Workfront)](#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront)
* [Nuovo oggetto &#39;Creatore di bozze&#39; nel report sulla versione del documento (Workfront)](#new-proof-creator-object-in-document-version-report-workfront)
* [Nuova funzionalità del pool di risorse temporaneamente rimossa dall’anteprima](#new-resource-pool-functionality-temporarily-removed-from-preview)

## Ripristino di elementi in blocco dal Cestino {#restoring-items-in-bulk-from-the-recycle-bin}

Ora è possibile ripristinare fino a 10 progetti, attività, problemi o documenti eliminati alla volta.

Prima di questa modifica, era possibile ripristinare un solo elemento eliminato alla volta.

Per ulteriori informazioni sul ripristino degli elementi, vedere [Ripristinare gli elementi eliminati](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Visualizza Utenti Iscritti {#view-subscribed-users}

Ora puoi vedere chi si abbona a un elemento espandendo il numero di abbonati che viene visualizzato accanto al collegamento di abbonamento.

Prima di questo miglioramento, non era visibile chi era abbonato a qualsiasi elemento.

Per ulteriori informazioni sulla sottoscrizione agli elementi, vedere [Sottoscrizione agli elementi in Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md). 

## Configurare la modalità di visualizzazione delle milestone nel diagramma di Gantt {#configure-how-milestones-are-displayed-on-the-gantt-chart}

Sono ora disponibili due opzioni per visualizzare le informazioni sulle milestone in un diagramma di Gantt. Puoi configurare uno o entrambi i seguenti indicatori milestone:

* Rombi milestone (icona)

  Questa icona viene visualizzata nel diagramma di Gantt dopo qualsiasi attività associata a un&#39;attività cardine.

* Linee milestone

  Dopo un&#39;attività associata alla fase cardine viene visualizzata una linea che si estende su tutte le attività del diagramma di Gantt.

Prima di questa modifica, era disponibile una sola opzione per consentire la visualizzazione delle Milestone in un diagramma di Gantt, denominata &quot;Milestone&quot;. Questa opzione consente di attivare sia l&#39;icona del rombo della milestone che la linea della milestone. Non è stato possibile separare questi indicatori.

Per ulteriori informazioni sulla configurazione della visualizzazione delle informazioni nel diagramma di Gantt, vedere [Configurare la visualizzazione delle informazioni nel diagramma di Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Includere la legenda del diagramma di Gantt durante l&#39;esportazione in PDF {#include-the-gantt-chart-legend-when-exporting-to-pdf}

Quando si esporta il grafico di Gantt in un PDF, è ora possibile scegliere se esportare anche la legenda del grafico insieme al grafico stesso. Gli elementi inclusi nella legenda sono solo le opzioni abilitate per la visualizzazione nel diagramma di Gantt nell’interfaccia utente. Queste opzioni sono incluse nella legenda se sono presenti nelle attività del progetto. Ad esempio, se si abilita la visualizzazione delle attività cardine nel diagramma di Gantt, anche queste verranno visualizzate nella legenda, ma solo se a un&#39;attività cardine è associata almeno un&#39;attività.

Prima di questa modifica, non era possibile escludere la legenda dal PDF esportato e la legenda includeva tutte le opzioni e i marcatori possibili del Gantt, indipendentemente dal fatto che fossero abilitati o esistessero nell’interfaccia utente.

Per ulteriori informazioni sull&#39;esportazione del grafico Gantt, vedere [Esportare il grafico Gantt in PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## Le informazioni utente vengono sincronizzate da Workfront a ProofHQ (ProofHQ e Workfront) {#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront}

Le informazioni utente (nome e indirizzo e-mail) vengono ora sincronizzate da Workfront a ProofHQ quando gli utenti vengono creati o aggiornati in Workfront. 

Per ulteriori informazioni sulla sincronizzazione degli utenti da Workfront a ProofHQ, consulta .

## Nuovo oggetto &quot;Creatore di bozze&quot; nel rapporto sulla versione del documento (Workfront)

{#new-proof-creator-object-in-document-version-report-workfront}

Ora, quando si crea un rapporto sulla versione di un documento, è presente un nuovo oggetto Proof Creator. Questo oggetto consente di creare rapporti sulle informazioni relative all’utente che ha creato la bozza. 

Il nuovo oggetto Proof Creator nel report Versione documento contiene tutti i campi disponibili con l&#39;oggetto User esistente in altri tipi di report oggetto.

>[!NOTE]
>
> Queste informazioni sono disponibili nel rapporto solo dal momento in cui questa funzione è stata introdotta per la prima volta nei rispettivi ambienti di anteprima o produzione; le informazioni nei rapporti relativi all’oggetto richiedente precedenti all’introduzione di questa funzionalità non sono disponibili.

È possibile accedere all&#39;oggetto Proof Creator durante la creazione di un report sulla versione del documento, come descritto in [Creare un report personalizzato](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Per ulteriori informazioni sul report di oggetti Document Version, vedere la sezione [Informazioni sugli oggetti in Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) in [Informazioni sugli oggetti in Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Visualizzare le approvazioni delle bozze nell’area Il mio lavoro (Workfront) {#view-proof-approvals-in-the-my-work-area-workfront}

Tutte le approvazioni delle bozze inviate per l&#39;approvazione vengono ora visualizzate nell&#39;area Il mio lavoro, nella scheda **Lavoro che ho inviato per l&#39;approvazione**.

Prima di questa modifica, la scheda **Lavoro che ho inviato per l&#39;approvazione** non includeva le approvazioni della bozza.

Le approvazioni delle bozze vengono visualizzate solo quando sono soddisfatti i seguenti criteri:

* L&#39;approvazione è attualmente in attesa di approvazione
* Il processo di approvazione viene assegnato a un utente con licenza Workfront (i processi di approvazione assegnati a utenti che non dispongono della licenza Workfront non vengono visualizzati)
* I processi di approvazione sono stati avviati dopo il rilascio di questa funzionalità (i processi di approvazione avviati prima del rilascio di questa funzionalità non vengono visualizzati)

Per ulteriori informazioni, vedere [Visualizza approvazioni](../../../../review-and-approve-work/manage-approvals/view-approvals.md) in [Visualizza approvazioni](../../../../review-and-approve-work/manage-approvals/view-approvals.md).

## Visualizzare i nomi utente quando si gestiscono le richieste di approvazione delle bozze dall&#39;area Il mio lavoro (Workfront) {#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront}

Ora, quando si approvano le approvazioni di bozze dall’area Il mio lavoro, viene visualizzato il nome dell’utente che ha richiesto l’approvazione.

Per ulteriori informazioni, vedere [Approvazione del lavoro](../../../../review-and-approve-work/manage-approvals/approving-work.md) in [Approvazione del lavoro](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## Visualizzatore di bozze migliorato per le bozze video (ProofHQ e Workfront) {#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront}

Il visualizzatore di bozze in Workfront e ProofHQ è stato aggiornato con un nuovo look and feel, architettura HTML5 per prestazioni migliori e supporto per nuove funzionalità.

Il nuovo visualizzatore di bozze contiene i seguenti miglioramenti:

* Prove fotogramma per fotogramma
* Buffering video
* Funzionalità di ricerca nell’elenco dei commenti
* Tutte le azioni impostate per il commento vengono visualizzate in ogni commento dell&#39;elenco
* Modalità a tutto schermo
* Revisione dei contenuti più veloce o più lenta
* Controllo ortografico quando si aggiungono commenti e risposte

### Anteprima

Il nuovo visualizzatore di bozze è disponibile per il test nei seguenti ambienti di anteprima:

* Ambiente di anteprima ProofHQ

  Per ulteriori informazioni sull&#39;ambiente di anteprima di ProofHQ, vedere [Anteprima ambiente di test sandbox- Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).

* Ambiente di anteprima Workfront, quando l’account è abilitato con la verifica

  Per ulteriori informazioni sull’ambiente di anteprima di Workfront, consulta  [Ambiente Sandbox Di Anteprima Di Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

In questa versione, il nuovo visualizzatore di bozze supporta solo la bozza video. Ciò significa che tutte le bozze video sfruttano il nuovo visualizzatore di bozze, mentre tutte le bozze statiche e rich media continuano a sfruttare il visualizzatore di bozze esistente.

### Production

Una volta rilasciato nell’ambiente di produzione con la versione 17.2, gli amministratori possono scegliere se il visualizzatore di bozze nuovo o legacy è adatto agli utenti della propria organizzazione. Per impostazione predefinita, viene utilizzato il visualizzatore di bozze legacy.

Per informazioni sull&#39;utilizzo del nuovo visualizzatore di bozze video, vedere  

## Visualizzare le bozze rich media in risoluzioni alternative (ProofHQ e Workfront) {#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront}

È ora possibile regolare la risoluzione delle bozze Rich Media specificando una risoluzione personalizzata o trascinando l’immagine alla risoluzione desiderata.

Prima di questa modifica, era possibile rivedere le bozze utilizzando solo la risoluzione inerente allo schermo o al dispositivo in cui si stava esaminando il contenuto.

Puoi utilizzare la modalità Confronta per confrontare diverse risoluzioni di bozze.

Per ulteriori informazioni, vedere [Apri bozze nel Visualizzatore bozze desktop](../../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/open-proofs-in-dpv.md). 

## Nuova funzionalità del pool di risorse temporaneamente rimossa dall’anteprima {#new-resource-pool-functionality-temporarily-removed-from-preview}

A causa di problemi di sviluppo, abbiamo deciso di rimuovere la nuova scheda Pianificazione risorse e rinominare la scheda Pianificazione risorse legacy nuovamente con il nome originale &quot;Pianificazione risorse&quot;.

Con questa modifica è stata rimossa anche la nuova funzionalità Pool di risorse. La nuova scheda di Pianificazione risorse e la funzionalità dei gruppi di risorse torneranno all’ambiente Sandbox di anteprima alla fine di giugno 2017.
