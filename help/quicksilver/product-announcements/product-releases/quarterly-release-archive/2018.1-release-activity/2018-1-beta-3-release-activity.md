---
content-type: release-notes
navigation-topic: product-releases-archive
title: Attività sulla versione 2018.1 di Beta 3
description: Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.1 di Beta 3. La funzionalità è stata resa disponibile nell’ambiente di anteprima il 7 gennaio 2018. Sarà disponibile nell’ambiente di produzione all’inizio del 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 26bbc4a0-e5ed-4b5f-bfc2-f888362c1d22
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 0%

---

# Attività sulla versione 2018.1 di Beta 3

Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.1 di Beta 3. La funzionalità è stata resa disponibile nell’ambiente di anteprima il 7 gennaio 2018. Sarà disponibile nell’ambiente di produzione all’inizio del 2018.

>[!IMPORTANT]
>
> La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate in 2018.1, consulta  Panoramica dell&#39;attività della versione di [2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La versione 2018.1 di Beta 3 contiene miglioramenti sia per gli amministratori di Workfront che per altri utenti:

**Per Amministratori**

* [Miglioramenti per gli amministratori di gruppi](#group-administrator-improvements)

**Per Tutti Gli Utenti**

* [Miglioramenti del visualizzatore di bozze di HTML5](#html5-proofing-viewer-improvements)
* [Miglioramenti delle bozze in Workfront](#proofing-improvements-within-workfront)
* [Miglioramenti area Home](#home-area-improvements) 
* [Miglioramenti Agile](#agile-improvements)
* [Miglioramenti al diagramma di Gantt](#gantt-chart-improvements)
* [Miglioramenti alla programmazione delle risorse](#resource-planner-improvements)

## Miglioramenti per gli amministratori di gruppi {#group-administrator-improvements}

* [Interfaccia utente Reimposta password aggiornata per gli amministratori di gruppi](#reset-password-ui-updated-for-group-administrators)
* [Opzioni di configurazione del livello di accesso per gli amministratori di gruppi](#access-level-setup-options-for-group-administrators)
* [Crea profili scheda orario per gruppi](#create-timesheet-profiles-for-groups)
* [Recupera elementi eliminati per gli utenti come amministratore di gruppo](#recover-deleted-items-for-users-as-a-group-administrator)

### Interfaccia utente di ripristino password aggiornata per gli amministratori di gruppi {#reset-password-ui-updated-for-group-administrators}

In qualità di amministratore di gruppo, quando si reimposta la password per un altro utente, viene richiesta la propria password prima di poterla modificare. L’interfaccia utente di è stata aggiornata per riflettere questa funzionalità. Prima di questa modifica, l’interfaccia utente mostrava che era richiesta la password dell’amministratore di Workfront.

Per ulteriori informazioni sulla reimpostazione delle password per altri utenti, vedere [Modificare il profilo di un utente](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Per ulteriori informazioni sulle funzionalità di un amministratore di gruppo, vedere la sezione &quot;Capacità degli amministratori di gruppi&quot; in [Creare un gruppo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Opzioni di configurazione del livello di accesso per gli amministratori di gruppi {#access-level-setup-options-for-group-administrators}

In qualità di amministratore di Workfront, ora puoi controllare se gli amministratori dei gruppi possono accedere come altri utenti o se possono reimpostare le password di altri utenti. È stata aggiunta una nuova impostazione nel Livello di accesso per abilitare o disabilitare questo accesso. Prima di questa modifica, tutti gli amministratori di gruppi potevano accedere come altri utenti e reimpostare le password di altri utenti per impostazione predefinita. Questa modifica influisce solo sul livello di accesso Planner.

Per ulteriori informazioni sulla configurazione del livello di accesso per gli utenti, vedere [Concedere l&#39;accesso agli utenti](../../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Per ulteriori informazioni sulle funzionalità di un amministratore di gruppo, vedere la sezione &quot;Capacità degli amministratori di gruppi&quot; in [Creare un gruppo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Crea profili Timesheet per i gruppi {#create-timesheet-profiles-for-groups}

In qualità di amministratore di gruppo, ora puoi creare profili Scheda orario per i gruppi che amministri e associarli ai gruppi che amministri o agli utenti di questi gruppi. I profili delle schede orario garantiscono che le schede orario vengano create automaticamente per gli utenti ad esse associati.

Prima di questa modifica, solo un amministratore di Workfront poteva creare i profili delle schede orario.

Per ulteriori informazioni sulla creazione di profili di schede orario, vedere [Creare, modificare e assegnare profili di schede orario](../../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Per ulteriori informazioni sulle funzionalità di un amministratore di gruppo, vedere la sezione &quot;Capacità degli amministratori di gruppi&quot; in [Creare un gruppo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Recupera elementi eliminati per gli utenti come amministratore di gruppo {#recover-deleted-items-for-users-as-a-group-administrator}

Se un progetto è associato a un gruppo di cui si è l&#39;amministratore del gruppo, è possibile ripristinare il progetto o una qualsiasi delle attività, dei problemi o dei documenti eliminati dal Cestino. Prima di questa modifica, solo un amministratore di Workfront poteva ripristinare gli elementi dal Cestino.

Per ulteriori informazioni sul ripristino degli elementi eliminati in Workfront, vedere [Ripristinare gli elementi eliminati](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Per ulteriori informazioni sulle funzionalità di un amministratore di gruppo, vedere la sezione &quot;Capacità degli amministratori di gruppi&quot; in [Creare un gruppo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

## Miglioramenti del visualizzatore di bozze di HTML5  {#html5-proofing-viewer-improvements}

* [Modalità confronto](#compare-mode)
* [Filtra l&#39;elenco dei commenti](#filter-the-comment-list)
* [L’elenco dei commenti viene cercato dopo l’immissione del primo carattere](#comment-list-is-searched-after-the-first-character-is-entered)

### Modalità di confronto {#compare-mode}

È ora possibile utilizzare la modalità di confronto nel visualizzatore di bozze di HTML5 quando si visualizzano bozze statiche e video. 

La modalità di confronto nel visualizzatore di bozze di HTML5 differisce dal visualizzatore di bozze legacy nei seguenti modi:

* Quando si avvia la modalità di confronto, la versione più recente si sposta sul lato destro, con la versione che si sta confrontando che si apre a sinistra.

  In precedenza, la versione più recente si spostava a sinistra, con la versione che si sta confrontando che si apre a destra.

* Puoi scegliere la versione di una bozza da confrontare direttamente dal visualizzatore di bozze. 
* Il livello di zoom corrente e la posizione delle bozze nel visualizzatore di bozze vengono mantenuti quando si accede alla navigazione simultanea.
* Nuova opzione Reimposta quando si utilizza la navigazione simultanea.
* Quando esci dalla modalità di confronto, puoi scegliere la bozza da chiudere. 

  In precedenza, la versione precedente era sempre chiusa.

* Vari miglioramenti a livello di aspetto e fruibilità.

Per ulteriori informazioni, vedere [Confrontare le bozze nel visualizzatore di bozze](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/compare-proofs.md).

### Filtrare l’elenco dei commenti {#filter-the-comment-list}

È ora possibile filtrare i commenti nell’elenco dei commenti. Puoi filtrare per utente, azioni, non letto e altro ancora.

### L’elenco dei commenti viene cercato dopo l’immissione del primo carattere {#comment-list-is-searched-after-the-first-character-is-entered}

Ora, durante la ricerca nell&#39;elenco dei commenti, l&#39;elenco viene filtrato automaticamente dopo aver digitato il primo carattere.

Prima di questa modifica, era necessario digitare almeno 3 caratteri nel campo di ricerca prima che l’elenco dei commenti venisse filtrato.

Per ulteriori informazioni, consulta in .

## Miglioramenti delle bozze in Workfront {#proofing-improvements-within-workfront}

* [Collega bozze da Workfront Proof a Workfront](#link-proofs-from-workfront-proof-to-workfront)
* [Impossibile rimuovere più una bozza da un documento](#can-no-longer-remove-a-proof-from-a-document)
* [Aspetto aggiornato durante la generazione e l’apertura delle bozze](#updated-look-and-feel-when-generating-and-opening-proofs)

### Collegare bozze da Workfront Proof a Workfront {#link-proofs-from-workfront-proof-to-workfront}

Ora puoi collegare a Workfront le bozze dei documenti già esistenti nel tuo account Workfront Proof.

Prima di questa modifica, non era possibile accedere alle bozze che esistevano già in Workfront Proof in Workfront. 

Per ulteriori informazioni, vedere [Collegare documenti da applicazioni esterne](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) in [Collegare documenti da applicazioni esterne](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Impossibile rimuovere una bozza da un documento {#can-no-longer-remove-a-proof-from-a-document}

Impossibile rimuovere una bozza da un documento. Per rimuovere una bozza, è necessario eliminare l&#39;intero documento.

Questo miglioramento riduce il rischio che gli utenti eliminino inavvertitamente tutte le versioni di un documento sottoposto a bozza. 

Per informazioni sull&#39;eliminazione di un documento, vedere [Elimina una bozza](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md) in [Elimina una bozza](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md).

### Aspetto aggiornato durante la generazione e l’apertura delle bozze {#updated-look-and-feel-when-generating-and-opening-proofs}

Ora è disponibile un’animazione di rotazione aggiornata quando viene generata una bozza.

## Miglioramenti area Home {#home-area-improvements}

Sono stati apportati i seguenti miglioramenti all’area Home:

* [Visualizza approvazioni bozze dall&#39;area Home](#view-proof-approvals-from-the-home-area)
* [I campi predefiniti vengono visualizzati durante la configurazione del modello di layout per gli elementi nell’area Home](#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area)

### Visualizzare le approvazioni delle bozze dall’area Home {#view-proof-approvals-from-the-home-area}

Ora è possibile visualizzare le approvazioni delle bozze nell’area Home, oltre alle approvazioni standard.

In precedenza era possibile visualizzare le approvazioni di Workfront, ma non quelle di una bozza.  

Per ulteriori informazioni, vedere [Utilizzare l&#39;area Home](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

### I campi predefiniti vengono visualizzati durante la configurazione del modello di layout per gli elementi nell’area Home {#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area}

In precedenza, i campi predefiniti non erano visibili dal modello di layout.

Per ulteriori informazioni, vedere &quot;Creazione e gestione di modelli di layout.

## Miglioramenti Agile {#agile-improvements}

* [Aggiungi attività e problemi all&#39;iterazione direttamente dalla pagina Dettagli attività o problemi](#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page)
* [Includi problemi nel backlog Scrum e nella bacheca delle storie per un team Agile](#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team)
* [Applica raggruppamenti e filtri al backlog per un team Agile](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [Crea un&#39;iterazione vuota e aggiornala in seguito](#create-a-blank-iteration-and-update-it-later)
* [I campi &quot;Focus&quot; e &quot;Capacity&quot; sono precompilati durante la creazione di un&#39;iterazione](#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration)

### Aggiungere attività e problemi all’iterazione direttamente dalla pagina Dettagli attività o problemi {#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page}

Ora puoi aggiungere attività e problemi attualmente assegnati a un team Agile a un’iterazione direttamente dall’attività o dal problema.

In precedenza, era possibile aggiungere attività a un’iterazione solo dal backlog. 

Per ulteriori informazioni, vedere [Creare un&#39;iterazione](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md) in [Creare un&#39;iterazione](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### Includi problemi nel backlog Scrum e nella bacheca delle storie per un team agile {#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team}

I problemi ora sono inclusi per impostazione predefinita nel backlog del team Agile quando si utilizza la metodologia Scrum Agile (i problemi non vengono visualizzati nel backlog di un team Agile quando si utilizza la metodologia Kanban).

Prima di questa modifica, era possibile aggiungere al backlog solo le attività. Se desideri aggiungere un problema, devi prima convertirlo in un’attività prima di poterlo aggiungere.

Per informazioni sull’utilizzo dei problemi nel backlog, consulta  [Gestione del backlog Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Applicare raggruppamenti e filtri al backlog per un team agile {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

Le opzioni Raggruppamento e Filtro sono ora disponibili nel backlog Agile, consentendoti di organizzare il backlog per raggruppamenti e di filtrare per attività e problemi specifici.

Prima di questa modifica, era possibile applicare sulle viste il backlog Agile.

Per ulteriori informazioni, consulta  [Gestione del backlog Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) in  [Gestione del backlog Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Creare un’iterazione vuota e aggiornarla in un secondo momento {#create-a-blank-iteration-and-update-it-later}

Non è più necessario aggiungere un’attività o un problema a un’iterazione per crearla. Puoi creare un’iterazione vuota e aggiungere attività e problemi in un secondo momento.

Per ulteriori informazioni, vedere [Creare un&#39;iterazione](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### I campi &quot;Focus&quot; e &quot;Capacity&quot; sono precompilati durante la creazione di un&#39;iterazione {#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration}

Ora, quando si crea un’iterazione, i campi &quot;Focus&quot; e &quot;Capacità&quot; sono precompilati con i valori medi per tutte le iterazioni passate create dal team. Se il team non ha creato alcuna iterazione passata, questi campi vengono visualizzati come 0.

In precedenza, questi campi venivano sempre impostati su 0.

Per ulteriori informazioni, vedere [Creare un&#39;iterazione](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## Miglioramenti al diagramma di Gantt {#gantt-chart-improvements}

* [Attiva modalità di modifica nel diagramma di Gantt](#enable-edit-mode-in-the-gantt-chart)
* [Rimuovere i predecessori durante la modifica del diagramma di Gantt](#remove-predecessors-when-editing-the-gantt-chart)

### Abilitare la modalità di modifica nel diagramma di Gantt {#enable-edit-mode-in-the-gantt-chart}

Se si attiva la modalità di modifica nel diagramma di Gantt, è possibile apportare modifiche alle informazioni contenute nel grafico. Prima di questa modifica, non era possibile modificare le informazioni nel diagramma di Gantt. È possibile modificare solo le informazioni sull&#39;attività nell&#39;elenco delle attività.

Per ulteriori informazioni sulla modifica del diagramma di Gantt, vedere [Aggiornare le informazioni nell&#39;elenco delle attività Diagramma di Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

### Rimuovere i predecessori durante la modifica del diagramma di Gantt {#remove-predecessors-when-editing-the-gantt-chart}

Utilizzando la modalità di modifica per il diagramma di Gantt, è ora possibile rimuovere le relazioni predecessori tra attività nel diagramma di Gantt di un progetto. Prima di questo miglioramento, era possibile rimuovere la relazione predecessore solo nell’elenco delle attività o a livello di attività.

Per ulteriori informazioni sulla modifica del diagramma di Gantt, vedere [Aggiornare le informazioni nell&#39;elenco delle attività Diagramma di Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Miglioramenti alla programmazione delle risorse {#resource-planner-improvements}

* [Budget con durata zero nella Programmazione risorse](#budget-with-zero-duration-in-the-resource-planner)

* [Mostra dati per costo nella Programmazione delle risorse](#show-data-by-cost-in-the-resource-planner)

### Budget con durata zero nella programmazione delle risorse {#budget-with-zero-duration-in-the-resource-planner}

>[!NOTE]
>
>Questa funzione è stata rimossa dall’ambiente di anteprima e viene rilasciata con la versione 18.1.

È ora possibile preventivare le risorse nella Programmazione delle risorse per qualsiasi data, entro o fuori dall&#39;intervallo di tempo del progetto. Prima di questo miglioramento, era possibile preventivare le risorse solo per le date all’interno dell’intervallo di tempo del progetto.

Per ulteriori informazioni sulla definizione del budget delle risorse nella Programmazione delle risorse, vedere la sezione &quot;Budgeting Resources in the Resource Planner&quot; in [Panoramica sulla programmazione delle risorse](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Mostra dati per costo nella Programmazione delle risorse {#show-data-by-cost-in-the-resource-planner}

È ora possibile visualizzare le informazioni nella Programmazione delle risorse in base al costo, oltre ai valori Ore e FTE. È possibile visualizzare i costi nella Programmazione delle risorse nelle visualizzazioni Visualizza per progetto o Visualizza per ruolo. Non è possibile visualizzare i costi quando si visualizza la Programmazione delle risorse nella visualizzazione Visualizza per utente.

Per ulteriori informazioni sulla visualizzazione della Programmazione delle risorse per ore, FTE o valori di costo, vedere [Panoramica sulla navigazione di Programmazione delle risorse](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).
