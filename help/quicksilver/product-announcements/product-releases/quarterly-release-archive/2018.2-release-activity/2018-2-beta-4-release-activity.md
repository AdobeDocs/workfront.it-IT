---
content-type: release-notes
navigation-topic: product-releases-archive
title: Attività sulla versione 2018.2 di Beta 4
description: Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.2 di Beta 4. La funzionalità sarà disponibile nell’ambiente di anteprima il 17 maggio 2018. Sarà disponibile nell’ambiente di produzione a luglio 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4b54b9e6-d1bf-4802-9d6c-9c3d3b6a6583
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 0%

---

# Attività sulla versione 2018.2 di Beta 4

Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.2 di Beta 4. La funzionalità sarà disponibile nell’ambiente di anteprima il 17 maggio 2018. Sarà disponibile nell’ambiente di produzione a luglio 2018.

>[!IMPORTANT]
>
> La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate in 2018.2, consulta  Panoramica dell&#39;attività di [versione 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La versione 2018.2 di Beta 4 contiene i miglioramenti per gli amministratori di Workfront e altri utenti:

**Per Amministratori**

* [Impostazioni di sistema: Informazioni sulla sessione nelle pagine esterne](#system-setting-session-information-in-external-pages)

**Per Tutti Gli Utenti**

* [Miglioramenti del limite WIP (Work In Progress) sulla bacheca Kanban](#work-in-progress-wip-limit-enhancements-on-the-kanban-board)
* [Interfaccia migliorata per la configurazione degli stati per un team Agile](#improved-interface-for-configuring-statuses-for-an-agile-team)
* [Elenco lavori aggiornato (pannello sinistro) nell&#39;area Home](#updated-work-list-left-panel-in-the-home-area)
* [Nuovo visualizzatore bozze desktop per il contenuto interattivo (Rich Media)](#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content) 
* [Esporta la visualizzazione utente nella Programmazione risorse](#export-the-user-view-in-the-resource-planner)
* [Supporto per le unità del team Google](#support-for-google-team-drives)
* [Nuovo limite di esportazione per il Diagramma di Gantt](#new-export-limit-for-the-gantt-chart)
* [L&#39;opzione Incolla dagli Appunti viene ora visualizzata come inattiva quando si utilizza Internet Explorer o Safari](#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari)
* [Nuovo ambiente Beta per Android con nuove funzionalità](#new-beta-environment-for-android-along-with-new-features)
* [Esempi di filtri per i messaggi di abbonamento agli eventi](#examples-of-filters-for-event-subscriptions-messages)

## Miglioramenti dei limiti WIP (Work In Progress) nel Kanban Board {#work-in-progress-wip-limit-enhancements-on-the-kanban-board}

### Configurare i limiti WIP per ogni colonna nel Kanban Board

Ora è possibile configurare i limiti WIP (Work In Progress) per ogni colonna della bacheca Kanban. 

Prima di questa modifica, era possibile configurare un solo limite WIP applicato a tutte le colonne della bacheca Kanban. 

Per ulteriori informazioni, consulta la sezione  [Configurare il limite WIP](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) nell&#39;articolo  [Configura Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

### Aggiorna il limite WIP direttamente dal Kanban Board

Ora i membri del team con diritti di modifica per il team possono aggiornare il limite WIP direttamente dal Kanban Board.

Prima di questa modifica, era possibile aggiornare il limite WIP solo dall&#39;area Impostazioni team.

Per ulteriori informazioni, consulta  nell&#39;articolo .

## È stata migliorata l’interfaccia per la configurazione degli stati per un team agile {#improved-interface-for-configuring-statuses-for-an-agile-team}

L’interfaccia per la configurazione degli stati per un team agile è stata aggiornata con i seguenti miglioramenti:

* Nuovo look and feel
* Riordinare le colonne di stato tramite trascinamento della selezione 

Per ulteriori informazioni, consulta i seguenti articoli:

* [Configura Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
* [Configura Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Elenco lavori aggiornato (pannello a sinistra) nell’area Home {#updated-work-list-left-panel-in-the-home-area}

La sezione Work List (Elenco di lavoro) nell’area Home contiene i seguenti miglioramenti:

* Gli elementi non letti ora spiccano con il grassetto e un punto blu.

  Gli elementi visualizzati al di fuori dell&#39;area Home vengono comunque visualizzati come non letti nell&#39;area Home.

  Per ulteriori informazioni, vedere [Visualizzare gli elementi nell&#39;elenco di lavoro nell&#39;area Home](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Ora i problemi sono distinti e accanto al problema viene visualizzata l’icona del problema.
* Le omologazioni sono ora distinte in base al tipo di omologazione, con il tipo di omologazione visualizzato. I possibili tipi di approvazione sono Attività, Progetto, Problema, Accesso, Documento, Scheda orario e Bozza.

  Prima di questa modifica, le approvazioni si distinguevano solo per la parola &quot;Approvazione&quot;.

* Gli elementi ora si distinguono a seconda che siano pronti per iniziare. Le opzioni possibili sono Pronto per l&#39;avvio, Non pronto o In corso.

  Queste informazioni non vengono visualizzate per le approvazioni perché sono sempre pronte per l’avvio.

* Ogni volta che un documento viene allegato all&#39;elemento viene visualizzata un&#39;icona di documento sotto il nome dell&#39;elemento.
* È ora possibile comprimere ed espandere i raggruppamenti all’interno di Work List (Elenco di lavoro) per controllare meglio quali informazioni sono visibili. I raggruppamenti sono In ritardo, Progetti, Date e Completato.

  Per impostazione predefinita, la sezione Questa settimana è espansa e tutti gli altri raggruppamenti sono compressi.

* Scegliere se ordinare gli articoli in base alla data di completamento pianificata o alla data di commit.
* Il numero di elementi in ciascun raggruppamento viene ora visualizzato tra parentesi accanto al titolo del raggruppamento.

  Questo numero non è disponibile per il raggruppamento Completati.

  Per ulteriori informazioni, vedere [Visualizzare gli elementi nell&#39;elenco di lavoro nell&#39;area Home](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Ridimensionare l’elenco di lavoro tramite trascinamento della selezione. È possibile ridimensionare l’elenco lavori in modo da occupare fino a metà dello schermo. La dimensione impostata viene mantenuta al successivo accesso a Home.

  Prima di questa modifica, non era possibile modificare le dimensioni dell’elenco di lavoro.

* Per le richieste, ora viene visualizzato l&#39;avatar dell&#39;utente che ha effettuato la richiesta con il testo &quot;[Nome_approvatore] richiede la tua approvazione su.&quot;
* Quando si crea una nuova attività personale, il pulsante &quot;Da fare&quot; è ora denominato &quot;Personale&quot;.

  Per ulteriori informazioni, vedere [Creare elementi di lavoro dalla sezione Home](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md) nell&#39;articolo [Creare elementi di lavoro dalla sezione Home](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* Gli articoli in ritardo vengono indicati come In ritardo solo dopo un&#39;ora dalla data di completamento pianificata.

Per ulteriori informazioni sull&#39;area Home, vedere [Utilizzare l&#39;area Home](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Nuovo visualizzatore bozze desktop per la correzione di contenuti interattivi (rich media) {#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content}

Il nuovo Visualizzatore bozze desktop consente di verificare i contenuti interattivi. A differenza del visualizzatore di bozze legacy esistente e del nuovo visualizzatore di bozze eseguito nel browser, il visualizzatore di bozze desktop è un&#39;applicazione che viene eseguita sulla workstation.

Prima del nuovo Visualizzatore bozze desktop, era possibile verificare il contenuto interattivo solo nel Visualizzatore bozze legacy. 

Il Visualizzatore bozze desktop include i seguenti miglioramenti rispetto al Visualizzatore bozze legacy per la verifica del contenuto interattivo:

* Esamina siti non protetti (HTTP)

  Il visualizzatore di bozze legacy consente di esaminare solo i siti protetti (HTTPS)

* Esamina i siti protetti da iframe (siti protetti dalla visualizzazione all’interno di un iframe).

  Il visualizzatore di bozze legacy non supporta la revisione per i siti protetti dalla visualizzazione all’interno di un iframe.

* Visualizza contenuti con risoluzioni preconfigurate per vari dispositivi. Ad esempio, puoi vedere come il contenuto viene visualizzato su varie risoluzioni standard del desktop o su singoli dispositivi come un iPhone 8. 

Per ulteriori informazioni sul download, l&#39;installazione e l&#39;utilizzo del Visualizzatore bozze desktop, vedere .

Per informazioni sulle differenze di funzionalità tra il Visualizzatore bozze desktop e i visualizzatori di bozze basati su browser, vedere [Differenze tra il Visualizzatore bozze web e la panoramica del Visualizzatore bozze desktop](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

## Esportare la visualizzazione utente nella Programmazione delle risorse {#export-the-user-view-in-the-resource-planner}

Per risolvere alcuni problemi di prestazioni, è stata temporaneamente disabilitata l’esportazione dei dati dalla Programmazione delle risorse quando questi vengono visualizzati nella Visualizzazione utente. Con questa versione, si riabilita l’esportazione dei dati durante la visualizzazione della Programmazione delle risorse nella Vista utente.

Per ulteriori informazioni sull&#39;esportazione dei dati di Programmazione delle risorse in Excel, vedere la sezione &quot;Opzione di esportazione&quot; in [Panoramica sulla navigazione di Programmazione delle risorse](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Per partecipare al nostro programma beta corrente per la Programmazione delle risorse, consulta [Performance Beta della Programmazione delle risorse.](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront)

## Impostazioni di sistema: Informazioni sulla sessione nelle pagine esterne {#system-setting-session-information-in-external-pages}

L’amministratore di Workfront ora può limitare l’utilizzo delle informazioni della sessione (ad esempio, ID sessione) durante la creazione di una pagina esterna.

Prima di questa modifica, gli utenti che potevano creare pagine esterne potevano utilizzare qualsiasi informazione di sessione durante l’incorporamento di altri siti in un dashboard di Workfront. 

Per ulteriori informazioni sulla configurazione delle preferenze di sistema in Workfront, vedere [Configurare le preferenze di sicurezza del sistema](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Supporto per le unità di team Google {#support-for-google-team-drives}

È ora possibile collegare da Workfront un documento o una cartella che si trova in un Google Team Drive.

Prima di questo miglioramento, era possibile collegare un documento o una cartella che si trova solo su Google My Drive.

Per ulteriori informazioni sul collegamento di documenti e cartelle da varie applicazioni a Workfront, vedere [Collegare documenti da applicazioni esterne](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Nuovo limite di esportazione per il diagramma di Gantt {#new-export-limit-for-the-gantt-chart}

È ora possibile esportare fino a 500 attività nel diagramma di Gantt.

In precedenza era possibile esportare solo fino a 250 attività.

Per ulteriori informazioni, vedere [Esportare il diagramma di Gantt in PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## L’opzione Incolla dagli Appunti ora viene visualizzata come inattiva quando si utilizza Internet Explorer o Safari {#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari}

L’opzione Incolla dagli Appunti viene ora visualizzata in grigio quando si utilizzano i browser Internet Explorer o Safari, con una descrizione che spiega che per questa funzione sono supportati solo i browser Chrome e Firefox.

Prima di questa modifica, questa opzione non veniva visualizzata quando si utilizzava Internet Explorer o Safari. 

Per ulteriori informazioni su come incollare le immagini dagli Appunti, vedere [Incollare le immagini dagli Appunti](../../../../documents/managing-documents/paste-image-clipboard.md).

## Nuovo ambiente Beta per Android e nuove funzioni {#new-beta-environment-for-android-along-with-new-features}

Ora puoi scoprire le funzioni più recenti su cui il nostro team sta lavorando per l’app mobile prima che vengano rilasciate al pubblico registrandoti per diventare un beta tester. Questo ambiente è attualmente supportato per l’app mobile Workfront solo per telefoni Android.

Per ulteriori informazioni su come registrarsi come beta tester per l’app mobile Workfront, consulta .

Nella versione beta dell’app mobile sono ora disponibili i seguenti miglioramenti:

* Pagina nuovo account

  Ora puoi visualizzare le informazioni sul tuo account, gestire le impostazioni del cellulare, inviare feedback o disconnetterti dalla nuova pagina Account.

  Prima di questo miglioramento, non era possibile visualizzare le informazioni sull’account nell’app mobile e accedere alle impostazioni, inviare feedback e disconnettersi dal menu principale di Workfront.

* Nuovo pannello inferiore di navigazione

  Nella parte inferiore dello schermo è ora disponibile una barra di navigazione più prominente che avvia tutte le aree dell’app mobile.

  Prima di questo miglioramento, le aree di funzionalità erano elencate nel menu principale di Workfront. Il menu principale di Workfront è stato rimosso ed è stato sostituito dalla nuova barra di navigazione inferiore.

  Per ulteriori informazioni sulla configurazione della nuova barra di navigazione, consulta la sezione &quot;Configurazione dell’app mobile&quot; in .

* Nuova visualizzazione elenco notifiche

  Un aspetto migliorato dell’elenco Notifiche consente di distinguere facilmente le notifiche nell’elenco a seconda del tipo e del fatto che siano state lette.

* La casella di ricerca è stata spostata in una posizione più prominente.

* Nuova esperienza di accessoÈ disponibile una nuova esperienza di accesso più semplice.

* Nuova esperienza tutorial

  Sono ora disponibili nuovi tutorial per guidare brevemente gli utenti nell’app al primo accesso. Prima di questa esperienza, i tutorial venivano avviati solo quando gli utenti accedevano ad aree specifiche di funzionalità.

## Esempi di filtri per i messaggi di abbonamento agli eventi {#examples-of-filters-for-event-subscriptions-messages}

Per dimostrare come è possibile filtrare gli abbonamenti agli eventi in modo da ricevere solo i messaggi rilevanti per la tua organizzazione, ora sono disponibili snippet di codice di esempio per filtrare il flusso di eventi che arrivano agli endpoint. Per ulteriori informazioni sulla visualizzazione degli esempi di filtro, vedere [Filtrare i messaggi di abbonamento agli eventi](../../../../wf-api/api/filter-event-sub-messages.md).
