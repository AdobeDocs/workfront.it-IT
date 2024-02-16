---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versione definitiva Beta 2017.2
description: Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2017.2. La funzionalità di questa pagina è stata resa disponibile nell’ambiente di anteprima il 28 giugno 2017. Sarà disponibile nell’ambiente di produzione il 26 luglio 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 768e9aad-d7e7-4a3c-9f93-926cf588ddc7
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2314'
ht-degree: 0%

---

# Versione definitiva Beta 2017.2

Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2017.2. La funzionalità di questa pagina è stata resa disponibile nell’ambiente di anteprima il 28 giugno 2017. Sarà disponibile nell’ambiente di produzione il 26 luglio 2017.

>[!IMPORTANT]
>
>La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate in 2017.2, consulta [Panoramica sull’attività della versione 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

La versione finale della versione beta 2017.2 contiene miglioramenti sia per gli amministratori di Workfront che per altri utenti:

**Per gli amministratori:**

* [Determinare la disponibilità del visualizzatore di verifica video di HTML5 (ProofHQ e Workfront)](#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront)
* [Supporto dei certificati SHA-256 per SAML 2.0](#support-sha-256-certificates-for-saml-2-0)
* [Tipo-Avanti per la mappatura degli attributi](#type-ahead-for-mapping-attributes)
* [Miglioramento API: accedere alle allocazioni utente](#api-enhancement-access-user-allocations)

**Per tutti gli utenti:**

* [Pianificazione risorse](#resource-planner)
* [Nuova area di pianificazione in un progetto (Team Builder)](#new-scheduling-area-in-a-project-team-builder)
* [Programmazione delle risorse: Mostra meno articoli per impostazione predefinita](#resource-scheduling-show-fewer-items-by-default)
* [Programmazione delle risorse: visualizza l&#39;indicatore di rilascio e di sovrassegnazione quando si trascinano attività e problemi](#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues)
* [Pianificazione delle risorse: le allocazioni utente non vengono più arrotondate alla mezz&#39;ora più vicina](#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour)
* [Esportare il rapporto Utilizzo in formato TSV e PDF](#export-the-utilization-report-in-tsv-and-pdf-formats)
* [Versione definitiva Beta 2017.2](#user-calendar-enhancements-in-the-my-work-area%22)
* [Versione definitiva Beta 2017.2](#layout-template-determines-whether-the-new-or-legacy-calendar-displays-in-the-my-work-area)
* [Decisione bozza visualizzata nell’area Il mio lavoro (Workfront)](#proof-decision-displays-in-the-my-work-area-workfront)
* [Visualizzare le bozze rich media nelle risoluzioni predefinite (ProofHQ e Workfront)](#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront)
* [Visualizzare l’URL delle pagine secondarie nei Commenti sulle bozze Rich Media (ProofHQ e Workfront)](#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront)
* [Creare visualizzazioni personalizzate in base alle visualizzazioni standard esistenti (ProofHQ)](#create-custom-views-based-on-existing-standard-views-proofhq)
* [Filtrare l’area di reporting (ProofHQ)](#filter-the-reporting-area-proofhq)
* [Visualizzazione dei valori minimo e massimo nei rapporti (ProofHQ)](#display-minimum-and-maximum-values-in-reports-proofhq)
* [Notifica in-app per approvazione bozza](#in-app-notification-for-proof-approval)
* [Miglioramenti per dispositivi mobili](#mobile-improvements)
* [Barra aggiunta alle istruzioni di filtro per i valori di campo contenenti virgole](#slash-added-to-filter-statements-for-field-values-that-contain-commas)
* [Più tariffe di fatturazione](#multiple-billing-rates)
* [Nuovo campo Ore preventivate risorsa](#new-resource-budgeted-hour-field)
* [Mostra Ruolo Utente nell&#39;area &#39;Assegnato a&#39; della pagina dei dettagli per le attività e i problemi](#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues)

>[!NOTE]
>
>Gli strumenti di pianificazione delle risorse sono stati dichiarati obsoleti e rimossi da Workfront con la versione 23.1. Per informazioni sulla programmazione delle risorse tramite il Bilanciatore dei carichi di lavoro, consulta [Panoramica del Bilanciatore dei carichi di lavoro](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Nuova area di pianificazione in un progetto (Team Builder) {#new-scheduling-area-in-a-project-team-builder}

L’area Pianificazione in un progetto (precedentemente nota come Team Builder) è stata riprogettata con un’interfaccia utente aggiornata e più intuitiva. La nuova funzionalità Pianificazione ora corrisponde maggiormente alla funzionalità Pianificazione risorse attualmente disponibile in altre aree di Workfront.

I miglioramenti includono:

* Consente di visualizzare le allocazioni di risorse correnti per i membri del team di progetto, consentendo di prendere decisioni più informate quando si effettuano le assegnazioni
* Rappresentazione visiva delle durate delle attività nella sequenza temporale di pianificazione
* Filtra le informazioni visualizzate nella sequenza temporale di pianificazione
* Aggiungi e rimuovi facilmente gli utenti dal team di progetto, direttamente dalla timeline di pianificazione

La seguente funzionalità è disponibile in altre aree dello strumento durante la pianificazione delle risorse, ma non è disponibile durante la pianificazione delle risorse nell&#39;area Programmazione team:

* Configura le attività padre da visualizzare nella sequenza temporale di pianificazione
* Configura i nomi dei progetti da visualizzare nella timeline di programmazione
* Modificare le assegnazioni utente utilizzando lo strumento Scambio
* Filtra per portfolio, programmi e progetti

Per ulteriori informazioni sulle funzionalità disponibili nell&#39;area Programmazione team, vedere &quot;Introduzione alla programmazione delle risorse&quot;.

## Programmazione delle risorse: Mostra meno articoli per impostazione predefinita {#resource-scheduling-show-fewer-items-by-default}

Per impostazione predefinita, nella sequenza temporale di pianificazione di un utente specifico vengono ora visualizzati al massimo 10 elementi di lavoro al giorno. Puoi espandere l’elenco per visualizzare tutte le attività e i problemi attualmente assegnati a tale utente.

Questo consente di sfogliare più facilmente la timeline di pianificazione quando agli utenti vengono assegnate molte attività e problemi.

Prima di questa modifica, tutte le attività e i problemi venivano sempre visualizzati per tutti gli utenti.

Per ulteriori informazioni sull&#39;assegnazione di attività e problemi agli utenti nella sequenza temporale di pianificazione, vedere &quot;Assegnazione manuale di attività e problemi non assegnati nelle aree Pianificazione&quot;.

## Programmazione delle risorse: visualizza l&#39;indicatore di rilascio e di sovrassegnazione quando si trascinano attività e problemi {#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues}

Quando si assegna un’attività o un problema a un utente nella sequenza temporale di pianificazione mediante trascinamento della selezione, ora prima di rilasciare l’attività o il problema e di completare l’assegnazione vengono visualizzate le seguenti informazioni:

* Nella riga dell’utente viene visualizzato un indicatore di rilascio. In questo modo è possibile vedere dove viene assegnato un articolo prima di effettuare l&#39;assegnazione.
* Se nella sequenza temporale della programmazione sono abilitate le allocazioni utente, vengono visualizzati gli indicatori rossi di sovrassegnazione se il completamento dell&#39;assegnazione determina una sovrassegnazione dell&#39;utente.

Prima di queste modifiche, non venivano visualizzate informazioni prima di rilasciare l’attività o il problema.

Per ulteriori informazioni sull&#39;assegnazione di attività e problemi agli utenti nella sequenza temporale di pianificazione, vedere &quot;Assegnazione manuale di attività e problemi non assegnati nelle aree Pianificazione&quot;.

## Pianificazione delle risorse: le allocazioni utente non vengono più arrotondate alla mezz&#39;ora più vicina {#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour}

Quando a un’attività o a un problema sono assegnati più utenti, o quando un’attività o un problema si estende su più giorni, Workfront tenta di distribuire le ore pianificate in modo uniforme tra gli utenti e i giorni assegnati. Le ore vengono arrotondate al centesimo più vicino per impostazione predefinita (ad esempio, 1,33).

In precedenza, quando si modificavano manualmente le ore distribuite, queste venivano regolate e arrotondate alla mezz’ora più vicina (ad esempio, 1,33 viene arrotondato a 1,5).

Ora le ore non vengono più regolate e arrotondate alla mezz’ora più vicina (ad esempio, 1,33 rimane 1,33).

## Miglioramento API: accedere alle allocazioni utente {#api-enhancement-access-user-allocations}

Ora puoi accedere all’ombreggiatura dell’allocazione utente tramite l’API Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../../../wf-api/api/access-proj-allocation-info-api.md" class="MCXref xref" xrefformat="{para}">Access Project Allocation Information via the API</a>.</p>
-->

## Esportare il rapporto Utilizzo in formato TSV e PDF {#export-the-utilization-report-in-tsv-and-pdf-formats}

Ora puoi esportare il rapporto Utilizzo su un progetto in formato TSV e PDF, oltre al formato XLSX.

Prima di questa modifica, era possibile esportare il rapporto Utilizzo solo in formato XLSX.

Per ulteriori informazioni sull&#39;esportazione del rapporto Utilizzo, vedere [Panoramica del rapporto Utilizzo risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Panoramica del rapporto Utilizzo risorse](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Decisione bozza visualizzata nell’area Il mio lavoro (Workfront) {#proof-decision-displays-in-the-my-work-area-workfront}

Ora, quando si visualizzano le approvazioni di bozza nella scheda Approvazioni personali nell’area Il mio lavoro, la decisione di bozza viene visualizzata nell’area Il mio lavoro e rimane finché non si fa clic sul nuovo pulsante Aggiorna in Workfront o fino al successivo aggiornamento della pagina del browser.

Prima di questa modifica, non vi era alcuna indicazione che una decisione fosse già stata presa sulla bozza e la bozza rimaneva nella scheda Le mie approvazioni fino a quando non si aggiornava il browser.

Per ulteriori informazioni, consulta [Approvazione del lavoro](../../../../review-and-approve-work/manage-approvals/approving-work.md) in [Approvazione del lavoro](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Visualizzare le bozze rich media nelle risoluzioni predefinite (ProofHQ e Workfront) {#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront}

In una versione precedente dell’ambiente di anteprima, è stata introdotta la possibilità di regolare la risoluzione delle bozze Rich Media specificando una risoluzione personalizzata o trascinando l’immagine alla risoluzione desiderata.

È ora possibile scegliere tra le opzioni di risoluzione predefinite di vari telefoni, tablet, notebook e desktop.

Per ulteriori informazioni, consulta &quot;Visualizzazione di una risoluzione predefinita&quot; in [Modificare la risoluzione della bozza interattiva nel visualizzatore di bozze](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Visualizzare l’URL delle pagine secondarie nei Commenti sulle bozze Rich Media (ProofHQ e Workfront) {#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront}

>[!NOTE]
>
>Questa funzione è attualmente disponibile nell’ambiente di produzione.

Ora, quando si commenta una sottopagina in una bozza Rich Media, nel commento viene visualizzato l’URL della sottopagina.

Prima di questa modifica, non era chiaro a quale pagina secondaria si riferisse il commento.

Per ulteriori informazioni, consulta

## Determinare la disponibilità del visualizzatore di verifica video di HTML5 (ProofHQ e Workfront) {#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront}

In qualità di amministratore di Workfront in ProofHQ, puoi determinare se gli utenti dell’organizzazione hanno accesso al nuovo visualizzatore di bozze HTML5 per le bozze video.

Per ulteriori informazioni sulla configurazione di questa opzione in Workfront, consulta in .

## Creare visualizzazioni personalizzate in base alle visualizzazioni standard esistenti (ProofHQ) {#create-custom-views-based-on-existing-standard-views-proofhq}

Ora puoi creare una vista personalizzata basata su una vista standard. Le opzioni Colonne, Ordinamento e Filtri della visualizzazione standard sono incluse nella nuova visualizzazione per impostazione predefinita.

Prima di questa modifica, per creare una vista personalizzata era necessario creare la vista da zero. 

Per ulteriori informazioni, consulta [Creazione di una vista personalizzata](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md#creating) in [Creare e gestire visualizzazioni personalizzate in Bozza di Workfront](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Filtrare l’area di reporting (ProofHQ) {#filter-the-reporting-area-proofhq}

Per impostazione predefinita, i dati visualizzati nella scheda Rapporti includono tutte le informazioni del sistema ProofHQ. Ora è possibile utilizzare i filtri per mostrare solo le informazioni pertinenti alle proprie esigenze. 

Per ulteriori informazioni, consulta [Filtraggio dei rapporti](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#filtering-reports) in  [Eseguire rapporti in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Visualizzazione dei valori minimo e massimo nei rapporti (ProofHQ) {#display-minimum-and-maximum-values-in-reports-proofhq}

Ora puoi configurare se i valori minimo e massimo vengono visualizzati nel grafico durante la visualizzazione dei rapporti.

Per ulteriori informazioni, consulta [Visualizzazione dei rapporti](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#viewing-reports) in  [Eseguire rapporti in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Supporto dei certificati SHA-256 per SAML 2.0 {#support-sha-256-certificates-for-saml-2-0}

Ora è supportato Secure Hash Algorithm 256 (SHA-256) durante la configurazione di Workfront per l’SSO con SAML 2.0. Prima di questa versione, supportavamo solo Secure Hash Algorithm 1 (SHA-1).

Per ulteriori informazioni sulla configurazione di Workfront con SAML 2.0, consulta [Configurare Adobe Workfront con SAML 2.0](../../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)

## Tipo-Avanti per la mappatura degli attributi {#type-ahead-for-mapping-attributes}

Il tipo di campo Valore predefinito nella finestra di dialogo Mappatura attributi è stato aggiornato a un campo di tipo-ahead. Prima di questa modifica, il campo Valore predefinito era di tipo a discesa.

Questa modifica si applica ai seguenti protocolli SSO:

* Active Directory
* LDAP
* SAML 2.0

SAML 1.1 non supporta la mappatura degli attributi.

## Miglioramenti per dispositivi mobili {#mobile-improvements}

>[!NOTE]
>
> L’app mobile viene rilasciata in modo indipendente dall’applicazione principale di Workfront. La funzionalità descritta in questa sezione viene rilasciata all’inizio di agosto.

Nelle app mobili, per entrambe le piattaforme Android e iOS, verranno visualizzate le seguenti funzionalità aggiunte:

* Inviare richieste dall’app mobile
* Nuova voce scheda orario nell’app mobile
* Modifica di moduli personalizzati dall’app mobile
* Richieste di approvazione bozza nell’app mobile

Sarà disponibile un programma beta pubblico per alcune di queste funzioni per la piattaforma Android.

Per ulteriori informazioni sul prossimo programma beta per dispositivi mobili, consulta la  [&quot;Beta&quot;](https://support.workfront.com/hc/en-us/sections/115000743248) pagina.

Per ulteriori informazioni sull&#39;utilizzo dell&#39;app mobile Workfront, consulta .  

## Barra aggiunta alle istruzioni di filtro per i valori di campo contenenti virgole {#slash-added-to-filter-statements-for-field-values-that-contain-commas}

Quando si crea un filtro in modalità testo e si filtrano i valori di campo che contengono virgole, è necessario aggiungere una barra (&quot;/&quot;) prima delle virgole che separano i valori, per garantire che il valore venga letto come un’unica opzione di filtro. Questo vale solo per i seguenti tipi di campi:

* Elenchi a discesa
* Bottoni Circolari
* Checkboxe

Prima di questa modifica, non era possibile filtrare i campi con opzioni contenenti virgole.

Per ulteriori informazioni su questa modifica, consulta [Panoramica sui filtri](../../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Più tariffe di fatturazione {#multiple-billing-rates}

Ora puoi aggiungere più sostituzioni della tariffa di fatturazione per la stessa mansione a livello di progetto. Con questa nuova funzionalità, puoi definire intervalli di date per ogni sostituzione della tariffa di fatturazione. Durante l&#39;intervallo di date specificato, viene applicata una tariffa di fatturazione diversa alla mansione assegnata alle attività di un progetto. Le tariffe di fatturazione vengono moltiplicate per le ore sul progetto per calcolare i ricavi. I ricavi calcolati entro l&#39;intervallo di date di una tariffa di fatturazione rimangono bloccati a tale tariffa e non vengono aggiornati come le tariffe delle mansioni nell&#39;aggiornamento del progetto. Nel caso di Reddito Reale, le ore registrate prima della sostituzione della tariffa di fatturazione non verranno ricalcolate per riflettere la tariffa di fatturazione corrente. Le ore registrate prima dell’aggiunta della sostituzione della tariffa di fatturazione al progetto verranno associate alla tariffa di fatturazione della mansione in quel momento.

Prima di questa modifica, era possibile sostituire la tariffa di fatturazione di una mansione una sola volta e il Ricavo effettivo veniva ricalcolato per riflettere la tariffa di fatturazione corrente per tutte le ore registrate prima della modifica della tariffa di fatturazione.

Per ulteriori informazioni sulle tariffe di fatturazione e sui ricavi, consulta [Panoramica su fatturazione e ricavi](../../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Per ulteriori informazioni sulla sostituzione delle tariffe di fatturazione per le mansioni a livello di progetto, consulta [Panoramica sulla sostituzione delle tariffe di fatturazione dei ruoli e sul calcolo dei ricavi per un progetto](../../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Pianificazione risorse {#resource-planner}

Con questa versione, verrà introdotta la prima fase della pianificazione delle risorse, che fa parte della riprogettazione della nuova scheda Pianificazione nell’area Persone. Utilizzando la Programmazione risorse è possibile preventivare la quantità di ore assegnate agli utenti nei gruppi di risorse in tutti i progetti correnti per i quali si è Responsabile risorse. Nella Programmazione delle risorse è possibile visualizzare i seguenti numeri di allocazione per progetto, mansione e utente:

* Ore disponibili
* Lavoro Necessario
* Ore preventivate
* Variazione ore (tra le ore preventivate e quelle pianificate)
* Differenza netta tra ore disponibili e ore preventivate

Per ulteriori informazioni sull&#39;utilizzo della Programmazione delle risorse, consulta [Panoramica di Programmazione delle risorse](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Nuovo campo Ore preventivate risorsa {#new-resource-budgeted-hour-field}

Per supportare la nuova funzionalità Planning e la pianificazione risorse, è stato aggiunto un nuovo campo al generatore di rapporti, che consente di creare rapporti sulle ore risorse preventivate. Questo campo acquisisce la quantità di ore preventivate per una risorsa in un progetto. Questo campo non è disponibile quando si definiscono i budget delle risorse utilizzando la funzionalità Pianificazione risorse legacy.

Per ulteriori informazioni sull&#39;utilizzo delle ore preventivate nella programmazione delle risorse, vedere [Panoramica di Programmazione delle risorse](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Notifica in-app per approvazione bozza {#in-app-notification-for-proof-approval}

Quando sei designato come approvatore di una bozza, ricevi una notifica in-app sull’approvazione della bozza in attesa della tua decisione. Nella notifica viene visualizzato il testo seguente: `<User name>` desidera che tu approvi questa bozza&quot;. Se le informazioni utente non sono disponibili, la notifica diventa &quot;Questa bozza richiede la tua approvazione&quot;.

Prima di questo miglioramento, l’unica indicazione visiva per indicare che sei stato designato come approvatore su una bozza era una nuova richiesta di bozza nella tua area Il mio lavoro.

Per ulteriori informazioni sulle notifiche in-app, consulta [Visualizzare e gestire le notifiche in-app](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Mostra Ruolo Utente nell&#39;area &#39;Assegnato a&#39; della pagina dei dettagli per le attività e i problemi {#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues}

Ora, quando si visualizza la pagina dei dettagli di un’attività o di un problema, sotto il nome dell’assegnatario viene visualizzata una mansione nell’area Assegnato a. Questo ruolo rappresenta il ruolo dell’utente che corrisponde all’assegnazione del ruolo dell’attività o del problema. Se l’attività o il problema non è assegnato a una mansione, viene visualizzata la mansione principale dell’utente assegnato.

Prima di questa modifica, nell’area Assegnato a veniva visualizzato solo il titolo dell’utente sotto il nome dell’utente. 
