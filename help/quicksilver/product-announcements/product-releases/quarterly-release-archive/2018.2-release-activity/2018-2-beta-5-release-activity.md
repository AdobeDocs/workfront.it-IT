---
content-type: release-notes
navigation-topic: product-releases-archive
title: Attività di rilascio della versione 2018.2 Beta 5
description: Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.2 Beta 5. La funzionalità sarà disponibile nell’ambiente di anteprima il 1° giugno 2018. I miglioramenti della bozza rilasciati con la versione beta 5 saranno disponibili nell’ambiente di anteprima lunedì 4 giugno. Sarà disponibile nell’ambiente di produzione a luglio 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0a8602aa-34c8-44d0-a102-9497d106f806
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '3165'
ht-degree: 1%

---

# Attività di rilascio della versione 2018.2 Beta 5

Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.2 Beta 5. La funzionalità sarà disponibile nell’ambiente di anteprima il 1° giugno 2018. I miglioramenti della bozza rilasciati con la versione beta 5 saranno disponibili nell’ambiente di anteprima lunedì 4 giugno. Sarà disponibile nell’ambiente di produzione a luglio 2018.

>[!IMPORTANT]
>
> La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate in 2018.2, consulta  [Panoramica sull’attività della versione 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La versione 2018.2 Beta 5 contiene i miglioramenti per gli amministratori di Workfront e altri utenti:

**Per gli amministratori**

* [Visualizzare le modifiche attivate dall&#39;utente con i registri di controllo](#view-user-triggered-changes-with-audit-logs)
* [Visualizzare le informazioni sulla licenza come amministratore di gruppo](#view-license-information-as-a-group-administrator)

**Per tutti gli utenti**

* [Vista calendario nell’area Home](#calendar-view-in-the-home-area)
* [Ulteriori aggiornamenti a Work List (Pannello a sinistra) nella Home](#additional-updates-to-the-work-list-left-panel-in-home)
* [Configurare i limiti dei ruoli per la pianificazione automatica delle risorse](#configure-job-role-limits-for-automated-resource-scheduling)
* [Miglioramenti alla vista Progetto e Ruolo nella Programmazione delle risorse](#project-and-role-view-improvements-in-the-resource-planner)
* [Ridimensionare le larghezze delle colonne per gli elenchi di progetti](#resize-column-widths-for-project-lists)
* [Icona Supporto per i nuovi elenchi di progetti](#icon-support-for-the-new-project-lists)
* [Aggiungere il campo &quot;Anteprima grande&quot; nelle visualizzazioni documento](#add-large-thumbnail-field-in-document-views)
* [Aumenta limite di esportazione Excel](#increase-excel-export-limit)
* [Filtri rapidi per gli elenchi di progetti](#quick-filters-for-project-lists)
* [Fare riferimento alle raccolte di problemi nei report di progetti e attività](#reference-issue-collections-in-project-and-task-reports)
* [Nuovo menu con versione più affidabile per l&#39;aggiunta di nuove versioni di documenti in Workfront](#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront)
* [Miglioramenti per dispositivi mobili nell’app mobile Android Beta](#mobile-improvements-in-the-android-beta-mobile-app)
* [miglioramenti del visualizzatore di verifica (Workfront e Workfront Proof)](#proofing-viewer-enhancements-workfront-and-workfront-proof)
* [Miglioramenti delle bozze in Workfront](#proofing-enhancements-in-workfront)
* [Miglioramenti delle bozze in Workfront Proof](#proofing-enhancements-in-workfront-proof)

## Vista calendario nell’area Home {#calendar-view-in-the-home-area}

Ora è possibile gestire le attività e le pianificazioni di lavoro personali utilizzando la visualizzazione Calendario Home di Workfront. La vista Calendario predefinito consente di effettuare le seguenti operazioni:

* Imposta la tua pianificazione per l&#39;esecuzione delle attività Workfront che ti sono state assegnate
* Visualizza rapidamente le attività in scadenza o scadute
* Visualizza il totale delle ore assegnate per una settimana
* Aggiornamenti alle attività assegnate

Se si utilizza un calendario in Outlook, è possibile integrare il calendario per visualizzare gli eventi di Outlook nella visualizzazione Calendario predefinito.

Per ulteriori informazioni, consulta [Vista Calendario predefinito](../../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

## Ulteriori aggiornamenti a Work List (Pannello a sinistra) nella Home {#additional-updates-to-the-work-list-left-panel-in-home}

Nell’area Home sono ora disponibili i seguenti miglioramenti per Work List (Elenco di lavoro):

* Il numero di elementi completati viene ora visualizzato tra parentesi accanto all’opzione Completati nel menu a discesa Filtro.

  In precedenza, il numero di elementi completati non veniva visualizzato nel menu Filtro. 

* Gli elementi completati vengono visualizzati per le 2 settimane precedenti.

  In precedenza, gli elementi completati venivano visualizzati per i 3 mesi precedenti.

  Per informazioni sulla visualizzazione del lavoro completato nell&#39;area Home, vedere [Visualizzare gli elementi in Work List (Elenco di lavoro) nell’area Home](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) nell’articolo [Visualizzare gli elementi in Work List (Elenco di lavoro) nell’area Home](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Aggiungere i campi Durata e Assegnazioni per visualizzare quando gli elementi vengono selezionati nell&#39;area Home.

  In precedenza, il campo Assegnazioni era disponibile per impostazione predefinita; tuttavia, se era stato eliminato, non poteva essere aggiunto nuovamente. Il campo Durata non era precedentemente disponibile per l’aggiunta.

  Per informazioni sull&#39;aggiunta di campi all&#39;area Home, vedere &quot;Creazione e gestione di modelli di layout&quot;.

Per ulteriori informazioni sull&#39;utilizzo dell&#39;area Home, vedere [Utilizzare l’area Home](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Visualizzare le modifiche attivate dall&#39;utente con i registri di controllo {#view-user-triggered-changes-with-audit-logs}

Abbiamo creato i seguenti registri di audit per gli amministratori di Workfront per monitorare le modifiche attivate dagli utenti:

* Registro di controllo utente
* Registro di controllo del livello di accesso
* Registri di controllo del gruppo
* Registri di controllo dei tentativi di accesso

In precedenza, non era possibile tenere traccia delle modifiche all’interno del sistema.

Per ulteriori informazioni, consulta [Visualizzare ed esportare i registri di audit](../../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Visualizzare le informazioni sulla licenza come amministratore di gruppo {#view-license-information-as-a-group-administrator}

È stata creata una pagina Licenze di sola lettura per consentire agli amministratori di gruppi di visualizzare il numero di licenze per i gruppi che amministrano.

Prima di questa modifica, gli amministratori di gruppi non potevano visualizzare le informazioni sulla licenza.

Per ulteriori informazioni, consulta [Amministratori di gruppi](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Configurare i limiti dei ruoli per la pianificazione automatica delle risorse {#configure-job-role-limits-for-automated-resource-scheduling}

>[!NOTE]
>
>Gli strumenti di pianificazione delle risorse sono stati dichiarati obsoleti e rimossi da Workfront con la versione 23.1. Per informazioni sulla programmazione delle risorse tramite il Bilanciatore dei carichi di lavoro, consulta [Panoramica del Bilanciatore dei carichi di lavoro](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Nelle impostazioni di Automated Resource Scheduling è ora possibile assegnare un limite a una mansione. Ciò ti consente di controllare il numero di risorse a cui viene assegnato il lavoro, con lo stesso ruolo.

In precedenza, non era possibile specificare il numero di utenti a cui era possibile assegnare un lavoro all’interno di una determinata mansione.

Per ulteriori informazioni, vedere &quot;Assegnazione manuale di attività e problemi non assegnati nelle aree Pianificazione&quot;.

## Miglioramenti alla vista Progetto e Ruolo nella Programmazione delle risorse {#project-and-role-view-improvements-in-the-resource-planner}

Le visualizzazioni Progetto e Ruolo della Programmazione delle risorse contengono ora i seguenti miglioramenti:

* Sono stati migliorati i filtri che estraggono informazioni dall’intero database, anziché solo quelle visualizzate sullo schermo.
* Modalità a tutto schermo.
* Le prestazioni sono ora più veloci ed efficienti.

   * Nuovi limiti per il numero di progetti, ruoli e utenti che è possibile visualizzare.
   * Caricamento lento, per un caricamento più rapido di progetti e ruoli.

* Accesso rapido a progetti e utenti direttamente da Programmazione risorse.
* Funzionalità di trascinamento della selezione più rapide nella vista Progetto, per assegnare la priorità ai progetti.

Prima di questi miglioramenti, è stato segnalato che la pianificazione delle risorse era lenta da caricare e che erano state notate incongruenze nei dati visualizzati. Grazie a questi miglioramenti, ora dovrebbero essere eliminati.

Per informazioni e per comprendere i nuovi limiti per la pianificazione delle risorse, consulta [Limitazioni della visualizzazione di Programmazione delle risorse](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref" xrefformat="{para}">Resource Planner performance beta </a></p>
-->

## Ridimensionare le larghezze delle colonne per gli elenchi di progetti {#resize-column-widths-for-project-lists}

Poiché stiamo lavorando sul miglioramento della funzionalità dei nostri elenchi, abbiamo temporaneamente disabilitato la possibilità di ridimensionare le larghezze delle colonne nei seguenti elenchi di progetti:

* Progetti di mia proprietà
* Progetti ai quali collaboro
* Tutti i progetti

Con questa versione, è ora possibile ridimensionare nuovamente le colonne di tutti gli elenchi di progetti.

Sono stati aggiunti ulteriori miglioramenti a questa funzionalità.

Ora, quando si trascina il bordo destro di una colonna per ridimensionarla, la colonna adiacente a destra mantiene le dimensioni rendendo l&#39;elenco più ampio, anziché essere modificata. È inoltre possibile trascinare il bordo di una colonna a destra oltre i bordi delle colonne adiacenti.

Prima di questo miglioramento, la colonna adiacente a destra della colonna ridimensionata veniva ridimensionata in modo proporzionale e adattata allo schermo. Non era possibile trascinare il bordo di una colonna oltre il bordo destro della colonna adiacente.  

Per informazioni sul ridimensionamento delle colonne negli elenchi, vedere [Modifica la larghezza e l&#39;ordine delle colonne](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Per partecipare al nostro programma di beta testing per i miglioramenti dell’elenco corrente, consulta [Nuovo studio elenchi.](http://community.workfront.com/discussions/community-home/digestviewer/viewthread?GroupId=457&amp;MessageKey=6b135c15-33dd-4fa2-8bc3-7cd7f7740c57&amp;CommunityKey=0425cafc-f0ec-47fc-be20-a21dc073d520&amp;tab=digestviewer&amp;ReturnUrl=%2fdiscussions%2fcommunity-home%2fdigestviewer%3fCommunityKey%3d0425cafc-f0ec-47fc-be20-a21dc073d520) (Accesso richiesto)

## Icona Supporto per i nuovi elenchi di progetti {#icon-support-for-the-new-project-lists}

Poiché abbiamo migliorato la funzionalità dei nostri elenchi, abbiamo temporaneamente disattivato la visualizzazione delle icone di stato nei seguenti elenchi di progetti:

* Progetti di mia proprietà
* Progetti ai quali collaboro
* Tutti i progetti

Con questa versione, le icone di stato possono essere nuovamente visualizzate negli elenchi dei progetti per i progetti o altri oggetti in un elenco di progetti.

Per informazioni sull&#39;utilizzo degli elenchi, vedere [Introduzione agli elenchi in Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Aggiungere il campo &quot;Anteprima grande&quot; nelle visualizzazioni documento {#add-large-thumbnail-field-in-document-views}

È in corso l&#39;aggiunta di un nuovo campo denominato Anteprima grande a una visualizzazione documento in un elenco o in un report. Quando viene selezionato in una visualizzazione documento, in questo campo viene visualizzata una miniatura del documento in un elenco o in un report di 400 pixel.

Prima di questa modifica, era possibile aggiungere solo il campo Miniatura a una visualizzazione del documento, in cui viene visualizzata una miniatura del documento larga 33-66 pixel.

Per informazioni sui campi negli elenchi e nei report, vedere [Glossario della terminologia di Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Aumenta limite di esportazione Excel {#increase-excel-export-limit}

È stato aumentato il limite del numero di righe che è possibile esportare in un file Excel. Ora puoi esportare i seguenti elementi:

* 65.000 righe in un file Excel .xls
* 100.000 righe in un file Excel .xlsx

I nuovi limiti si applicano quando si esportano i seguenti elementi da Workfront:

* Un elenco o un rapporto dall’interfaccia web
* Un elenco o un rapporto che utilizza l’API
* Un rapporto pianificato e consegnato

Prima di questo miglioramento, era possibile esportare solo 50.000 righe in qualsiasi file Excel.

Per informazioni sull’esportazione di dati da Workfront, consulta [Esporta dati](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Filtri rapidi per gli elenchi di progetti {#quick-filters-for-project-lists}

È ora possibile applicare un filtro rapido agli elenchi.

Lo scopo di un filtro rapido è quello di aiutarti a passare direttamente agli elementi dei tuoi elenchi di grandi dimensioni che ti interessano, in modo da poterli rivedere, aggiornare o condividere rapidamente con altri utenti.

Attualmente, i filtri rapidi sono disponibili solo per gli elenchi dei progetti nelle seguenti schede secondarie:

* Progetti ai quali collaboro
* Progetti di mia proprietà
* Tutti i progetti

Per informazioni sui filtri rapidi, consulta la sezione &quot;Applicazione di filtri rapidi agli elenchi&quot; in [Introduzione agli elenchi in Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Fare riferimento alle raccolte di problemi nei report di progetti e attività {#reference-issue-collections-in-project-and-task-reports}

È ora possibile fare riferimento a una raccolta di problemi nella visualizzazione e nel filtro di un progetto o di un’attività. Puoi farlo solo utilizzando la modalità Testo durante la creazione di un rapporto.

Prima di questo miglioramento, era possibile fare riferimento solo a una raccolta di attività in una visualizzazione o un filtro di progetto.

Per informazioni su come fare riferimento a una raccolta in un report, vedi [Fare riferimento alle raccolte in un rapporto](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

Per informazioni sull&#39;utilizzo della modalità testo, vedere  [Panoramica sugli usi comuni della modalità testo](../../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

>[!NOTE]
>
>Nel video seguente, la modalità di testo di esempio per le raccolte di problemi non era corretta. La modalità testo di esempio corretta è disponibile in [Fare riferimento alle raccolte in un rapporto](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

## Nuovo menu con versione più affidabile per l&#39;aggiunta di nuove versioni di documenti in Workfront {#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront}

Ora, quando si aggiungono nuove versioni ai documenti in Workfront, il menu Nuova versione contiene opzioni aggiuntive ed è ora coerente tra le aree di Workfront in cui è possibile aggiungere una nuova versione.

È possibile aggiungere una nuova versione del documento dalle seguenti aree di Workfront:

* Dal menu a discesa Altro nella scheda Documenti.
* Dal menu Azioni documento nella pagina dei dettagli del documento.
* Dalla scheda Tutte le versioni nella pagina dei dettagli del documento.

Prima di questa modifica, solo il menu a discesa Altro nella scheda Documenti conteneva tutte le opzioni per l’aggiunta di una nuova versione.

Nel menu Nuova versione sono ora disponibili le seguenti opzioni per tutte le aree in cui è possibile aggiungere una nuova versione:

* Bozza
* Solo documento
* Opzioni collegate (dal Dropbox, dall&#39;unità Google e così via)
* Incolla dagli Appunti (questa è una nuova opzione per l’aggiunta di versioni)

Per ulteriori informazioni, consulta [Aggiungere documenti ad Adobe Workfront dal file system](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md) nell’articolo [Aggiungere documenti ad Adobe Workfront dal file system](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

## Miglioramenti per dispositivi mobili nell’app mobile Android Beta {#mobile-improvements-in-the-android-beta-mobile-app}

I seguenti miglioramenti saranno disponibili sulla versione Android Beta dell’app mobile poco dopo il giorno di questa versione:

* Azioni Scorrimento rapido

  Puoi eseguire attività come volontariato per lavorare per un’attività, completare un’attività, contrassegnare una notifica come visualizzata o nuova, inviare un testo o chiamare un contatto scorrendo vari oggetti nell’app mobile di Workfront.

  Con questa funzionalità sono state migliorate le seguenti aree:

   * My Work and Home
   * Notifiche
   * Conttati
   * Approvazioni

* Nuovo aspetto nella scheda Dettagli di un elemento

  L’interfaccia è stata modificata durante la visualizzazione di un elemento nella versione Android Beta dell’app mobile per facilitarne la modifica, il completamento o l’allegato di un documento.

* Nuova esperienza durante la registrazione

  Il tempo di registrazione è più rapido e semplice rispetto a prima, con un pulsante di accesso più semplice e un&#39;interfaccia più semplice per le ore di registrazione.

Con questa versione, questi miglioramenti sono disponibili solo per la versione Android Beta dell’app mobile Workfront. Al momento non sono disponibili per iOS.

Per ulteriori informazioni su come iscriversi a un beta tester e scaricare la versione Android Beta dell&#39;app mobile Workfront, consulta .

## miglioramenti del visualizzatore di verifica (Workfront e Workfront Proof) {#proofing-viewer-enhancements-workfront-and-workfront-proof}

* [Pagina Stampa riepilogo aggiornata](#updated-print-summary-page)
* [Aggiungere utenti a una bozza direttamente dal visualizzatore di bozze](#add-users-to-a-proof-directly-from-the-proofing-viewer)
* [Visualizza tutti gli strumenti di markup nel visualizzatore di bozze](#display-all-markup-tools-in-the-proofing-viewer)
* [Configurare le opzioni di ordinamento predefinite nel visualizzatore di bozze](#configure-default-sorting-options-in-the-proofing-viewer)
* [Visualizzare le approvazioni dei documenti di Workfront nel Visualizzatore bozze desktop](#view-workfront-document-approvals-in-the-desktop-proofing-viewer)
* [Configurare i collegamenti che aprono nuove schede e finestre per l&#39;apertura nel Visualizzatore bozze del desktop](#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer)
* [Indicatore di presenza nel visualizzatore di bozze](#presence-indicator-in-the-proofing-viewer)
* [Filtrare i commenti per visualizzare una singola pagina per le bozze degli URL interattivi nel visualizzatore bozze desktop](#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer)
* [Visualizzatore bozze desktop per contenuti statici e video](#desktop-proofing-viewer-for-static-and-video-content)
* [Aggiungere dispositivi personalizzati al sistema](#add-custom-devices-to-your-system)

### Pagina Stampa riepilogo aggiornata {#updated-print-summary-page}

La pagina Stampa riepilogo è stata aggiornata con un nuovo aspetto e funzionalità migliorate.

Per informazioni, consulta [Stampare un riepilogo delle bozze in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### Aggiungere utenti a una bozza direttamente dal visualizzatore di bozze {#add-users-to-a-proof-directly-from-the-proofing-viewer}

Ora è possibile aggiungere utenti a una bozza direttamente dal visualizzatore bozze web e dal visualizzatore bozze desktop. 

In precedenza, non era possibile aggiungere singoli utenti a una bozza. È invece possibile copiare solo l’URL pubblico o il codice di incorporamento.

Per ulteriori informazioni, consulta [Condividere una bozza aggiungendovi utenti](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) nell’articolo  [Condividere una bozza dal visualizzatore di bozze](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

### Visualizza tutti gli strumenti di markup nel visualizzatore di bozze {#display-all-markup-tools-in-the-proofing-viewer}

Ora è possibile configurare lo strumento markup in modo che venga sempre visualizzato, anziché in un menu da aprire. Questo rende più veloce il passaggio tra gli strumenti. Se configurati in questo modo, gli strumenti di markup vengono visualizzati orizzontalmente nella parte superiore di Web Proofing Viewer e Desktop Proofing Viewer.

In precedenza, gli strumenti di markup erano disponibili solo all’interno di un menu a discesa.

Per ulteriori informazioni sulla configurazione di questa impostazione di markup, vedere [Configurare le impostazioni del visualizzatore di verifica](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

Per ulteriori informazioni sull’utilizzo delle opzioni di markup durante la revisione di una bozza, consulta l’articolo .

### Configurare le opzioni di ordinamento predefinite nel visualizzatore di bozze {#configure-default-sorting-options-in-the-proofing-viewer}

Ora, quando si modifica l’opzione di ordinamento all’interno dell’elenco dei commenti in una bozza, tale opzione diventa l’opzione di ordinamento predefinita alla successiva apertura di una bozza in Web Proofing Viewer (Visualizzatore di bozze web) o Desktop Proofing Viewer (Visualizzatore di bozze desktop). 

Per ulteriori informazioni, consulta l’articolo .

### Visualizzare le approvazioni dei documenti di Workfront nel Visualizzatore bozze desktop {#view-workfront-document-approvals-in-the-desktop-proofing-viewer}

Ora è possibile prendere una decisione di approvazione del documento di Workfront nel Visualizzatore bozze desktop.

In precedenza, solo Web Proofing Viewer (Visualizzatore di bozze web) consentiva di prendere una decisione di approvazione di un documento Workfront. 

Per ulteriori informazioni, consulta  [Decidi su una bozza nel visualizzatore di bozze](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) nell’articolo  [Decidi su una bozza nel visualizzatore di bozze](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

### Configurare i collegamenti che aprono nuove schede e finestre per l&#39;apertura nel Visualizzatore bozze del desktop {#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer}

Quando si esegue la verifica del contenuto interattivo nel Visualizzatore bozze desktop, è ora possibile configurare i collegamenti che si aprono in una nuova scheda o in una nuova finestra per aprirsi all’interno del Visualizzatore bozze desktop in modo da poter continuare la verifica.

Nel visualizzatore di bozze Legacy, i collegamenti aperti in una nuova scheda o in una nuova finestra non potevano essere esaminati nel visualizzatore di bozze.

Per ulteriori informazioni, consulta [Configurare le impostazioni del visualizzatore di verifica](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

### Indicatore di presenza nel visualizzatore di bozze {#presence-indicator-in-the-proofing-viewer}

Ora, quando esamini una bozza in Web Proofing Viewer (Visualizzatore di bozze web) o in Desktop Proofing Viewer (Visualizzatore di bozze desktop), nell’angolo superiore destro del visualizzatore di bozze viene visualizzato l’avatar di ogni utente che sta visualizzando la bozza.

Per ulteriori informazioni, consulta [Rivedere una bozza contemporaneamente con più revisori](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proof-with-multiple-reviewers.md).

### Filtrare i commenti per visualizzare una singola pagina per le bozze degli URL interattivi nel visualizzatore bozze desktop {#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer}

Quando rivedi un URL in una bozza interattiva nel Visualizzatore bozze desktop, ora puoi filtrare i commenti per visualizzare i commenti aggiunti solo nella pagina corrente. 

Prima di questa modifica, questa opzione era disponibile solo per le bozze statiche.

Per ulteriori informazioni, consulta l’articolo .

### Visualizzatore bozze desktop per contenuti statici e video {#desktop-proofing-viewer-for-static-and-video-content}

Il Visualizzatore bozze desktop ora supporta contenuti statici e video.

In precedenza, supportava solo contenuti interattivi.

Per informazioni sulla configurazione delle bozze statiche e video da aprire in Desktop Proofing Viewer, consulta [Configurare le impostazioni del visualizzatore di verifica](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

Per ulteriori informazioni su Visualizzatore bozze desktop, vedere [Analisi delle bozze nel Visualizzatore bozze desktop.](https://support.workfront.com/hc/en-us/sections/360000686434)

### Aggiungere dispositivi personalizzati al sistema {#add-custom-devices-to-your-system}

Ora è possibile aggiungere qualsiasi dispositivo personalizzato al sistema, consentendo agli utenti di rivedere il contenuto interattivo e simulare come appare su un dispositivo specifico durante la revisione di una bozza nel Visualizzatore bozze desktop.

Prima di questa modifica, gli utenti potevano scegliere solo da un elenco di dispositivi standard preconfigurati.

Per informazioni sull&#39;aggiunta di dispositivi personalizzati, vedere in

Per informazioni su come gli utenti possono selezionare i dispositivi durante la revisione dei contenuti interattivi, consulta [Modificare la risoluzione della bozza interattiva nel visualizzatore di bozze](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Miglioramenti delle bozze in Workfront {#proofing-enhancements-in-workfront}

* [Condividi il collegamento bozza direttamente da Workfront](#share-the-proof-link-directly-from-workfront)
* [Rapporto sui dati di verifica aggiuntivi in Workfront](#report-on-additional-proofing-data-in-workfront)
* [Visualizzare i dati storici per le approvazioni delle bozze in Workfront](#view-historical-data-for-proof-approvals-in-workfront)

### Condividi il collegamento bozza direttamente da Workfront {#share-the-proof-link-directly-from-workfront}

Ora è possibile generare un collegamento per una bozza in Workfront e condividerla direttamente da Workfront. In alternativa, puoi copiare l’URL e distribuirlo utilizzando un metodo alternativo.

Prima di questa modifica, era possibile copiare il collegamento della bozza solo in Workfront e distribuirlo con un metodo alternativo.

Per ulteriori informazioni, consulta [Condividere una bozza in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) nell’articolo [Condividere una bozza in Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

>[!NOTE]
>
>Il collegamento di incorporamento attualmente disponibile verrà rimosso in una versione futura. Il collegamento di incorporamento sarà ancora accessibile tramite l’API Workfront.

### Rapporto sui dati di verifica aggiuntivi in Workfront {#report-on-additional-proofing-data-in-workfront}

Nei report che contengono l&#39;oggetto Versione documento, ad esempio i report Versione documento e Approvazione bozza, sono ora disponibili diversi campi che consentono di visualizzare ulteriori informazioni sulla bozza.

* Scadenza bozza

  Visualizza il giorno della settimana, la data, l’ora del giorno e l’anno della scadenza della bozza.

* Decisione bozza

  Visualizza lo stato della decisione della bozza (in sospeso, modifiche necessarie o approvate).

* Nome bozza

  Visualizza il nome della bozza.

* Pagine bozza

  Visualizza il numero di pagine incluse nella bozza.

* Avanzamento bozza

  Visualizza lo stato di avanzamento della bozza (Inviata, Aperta, Commentata, Decisione eseguita).

Per ulteriori informazioni su ciascuno di questi campi, consulta  [Glossario della terminologia di Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Visualizzare i dati storici per le approvazioni delle bozze in Workfront {#view-historical-data-for-proof-approvals-in-workfront}

Nel rapporto Proof Approval (Approvazione bozza) è possibile aggiungere un campo che consente di visualizzare le decisioni di approvazione delle bozze per le bozze che non sono più attive. A tale scopo, aggiungere il campo Decisione approvatore al rapporto.

Prima di questa modifica, dopo aver preso una decisione sulla bozza, la decisione non poteva più essere visualizzata in un rapporto di Workfront.

Per ulteriori informazioni, consulta  [Glossario della terminologia di Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Miglioramenti delle bozze in Workfront Proof {#proofing-enhancements-in-workfront-proof}

* [Creare una nuova versione di una bozza direttamente dal visualizzatore di bozze (Workfront Proof)](#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof)
* [Nuovo collegamento Dettagli bozza nel visualizzatore di bozze e nel visualizzatore di bozze del desktop (Workfront Proof)](#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof)

### Creare una nuova versione di una bozza direttamente dal visualizzatore di bozze (Workfront Proof) {#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof}

È ora possibile creare una nuova versione di una bozza direttamente dal nuovo visualizzatore di bozze e dal Visualizzatore bozze desktop quando si esegue la bozza in Workfront Proof.

In precedenza, questa opzione era disponibile solo nel Visualizzatore di Flash legacy.

Per ulteriori informazioni, consulta [Copia delle bozze in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md) nell’articolo  [Copia delle bozze in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md).

### Nuovo collegamento Dettagli bozza nel visualizzatore di bozze e nel visualizzatore di bozze del desktop (Workfront Proof) {#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof}

Quando si visualizza una bozza nel visualizzatore di bozze, gli utenti di Workfront Proof possono ora passare rapidamente alla pagina dei dettagli della bozza in Workfront Proof.

Per ulteriori informazioni, consulta &quot;Visualizzazione dei dettagli della bozza&quot;.
