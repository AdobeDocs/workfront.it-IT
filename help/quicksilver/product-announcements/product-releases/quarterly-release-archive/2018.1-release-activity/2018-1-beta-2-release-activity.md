---
content-type: release-notes
navigation-topic: product-releases-archive
title: Attività sulla versione 2018.1 di Beta 2
description: Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.1 di Beta 2. La funzionalità in questa pagina è stata resa disponibile nell’ambiente di anteprima il 14 dicembre 2017. Sarà disponibile nell’ambiente di produzione a marzo 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 22e3836c-c41e-48a6-9926-e832af91e616
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1327'
ht-degree: 2%

---

# Attività sulla versione 2018.1 di Beta 2

Questa pagina descrive tutte le modifiche più recenti disponibili nell’ambiente di anteprima con la versione 2018.1 di Beta 2. La funzionalità in questa pagina è stata resa disponibile nell’ambiente di anteprima il 14 dicembre 2017. Sarà disponibile nell’ambiente di produzione a marzo 2018.

>[!IMPORTANT]
>
> La funzionalità descritta in questa pagina è soggetta a modifiche prima della disponibilità nell’ambiente di produzione.

Per un elenco di tutte le modifiche apportate in 2018.1, consulta  Panoramica dell&#39;attività della versione di [2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La versione 2018.1 di Beta 2 contiene miglioramenti sia per gli amministratori di Workfront che per altri utenti:

**Per Amministratori**

* [Amministrazione di gruppi per utenti e modelli di layout](#group-administration-for-users-and-layout-templates)

**Per Tutti Gli Utenti**

* [Schermo widescreen a livello di sistema](#system-wide-widescreen-display)
* [Ridimensiona snapshot della sequenza temporale nel diagramma di Gantt](#resize-timeline-snapshot-on-the-gantt-chart)
* [Programmazione interattiva delle risorse nel caso di business](#interactive-resource-planner-in-the-business-case)
* [Visualizzazione in Pianificazione risorse - Grafico di allocazione utenti](#visualization-in-the-resource-planner-user-allocation-chart)
* [Miglioramenti nell&#39;area Home](#improvements-in-the-home-area)
* [Nuovi miglioramenti al visualizzatore di bozze](#new-proofing-viewer-improvements) 

## Amministrazione di gruppi per utenti e modelli di layout {#group-administration-for-users-and-layout-templates}

Ora puoi designare gli amministratori dei gruppi in Workfront. Il campo Proprietario gruppo è stato rinominato in Amministratore gruppo e gli utenti designati come amministratori di gruppo dispongono di autorizzazioni aggiuntive per gestire gli utenti e i modelli di layout per i gruppi che gestiscono.

* [Gestione utente per amministratore gruppo](#user-management-by-group-administrator)
* [Gestione dei modelli di layout per amministratori di gruppi](#layout-template-management-by-group-administrators)

### Gestione utente per amministratore gruppo {#user-management-by-group-administrator}

Stiamo introducendo il nuovo concetto di **amministratore gruppo**. Per supportare questa funzione, il campo **Proprietario gruppo** è stato rinominato **Amministratore gruppo** e gli utenti designati come amministratori di gruppi dispongono di autorizzazioni aggiuntive per gestire gli utenti e i gruppi.

Oltre alle autorizzazioni che il proprietario del gruppo aveva in precedenza per gestire gli utenti, l’amministratore del gruppo ora dispone del seguente accesso aggiuntivo per la gestione degli utenti all’interno dei gruppi in cui sono impostati come amministratore del gruppo:

* Accedi come altro utente che appartiene a un gruppo che gestisce.
* Reimpostare la password per un altro utente che appartiene a un gruppo che gestisce.
* Creare modelli di layout amministrati dal relativo gruppo. 

Prima di questa modifica, solo l’amministratore di Workfront poteva eseguire queste funzioni.

Per ulteriori informazioni sugli amministratori di gruppi, vedere la sezione &quot;Informazioni sugli amministratori di gruppi&quot; in [Creare un gruppo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Gestione dei modelli di layout per amministratori di gruppi {#layout-template-management-by-group-administrators}

Stiamo introducendo il nuovo concetto di **gruppo con accesso amministratore** che puoi associare a un modello di layout.

L’utente designato come amministratore di gruppo in questo gruppo ha accesso alla gestione del modello di layout e alla creazione di nuovi modelli di layout, in cui i gruppi da lui gestiti sono i gruppi amministrativi dei modelli. 

Prima di questa modifica, solo l’amministratore di Workfront poteva creare modelli di layout.

Per ulteriori informazioni sulla creazione di modelli di layout, vedere Creazione e gestione di modelli di layout.

## Schermo widescreen a livello di sistema {#system-wide-widescreen-display}

Quando visualizzi una pagina in Workfront, l’intera finestra del browser ora viene riempita automaticamente e si adatta alle dimensioni dello schermo.

Prima di questa modifica, venivano visualizzate in widescreen solo le pagine associate ai seguenti oggetti:

* Progetti
* Attività
* Problemi
* Report
* Dashboard
* Calendari

## Ridimensionamento dello snapshot della sequenza temporale nel diagramma di Gantt {#resize-timeline-snapshot-on-the-gantt-chart}

Ora puoi espandere lo snapshot della timeline per visualizzare l’intero progetto nel diagramma di Gantt.

Prima di questo miglioramento, era possibile selezionare un punto specifico nell’istantanea della timeline per spostarsi su di esso nel diagramma di Gantt.

Per ulteriori informazioni sulla configurazione della visualizzazione delle informazioni nel diagramma di Gantt, vedere [Configurare la visualizzazione delle informazioni nel diagramma di Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Pianificazione interattiva delle risorse nel Business Case {#interactive-resource-planner-in-the-business-case}

In qualità di Responsabile risorse, è ora possibile aggiungere gruppi di risorse nella sezione Budget risorse del caso aziendale. È inoltre possibile preventivare le risorse del progetto utilizzando la pianificazione risorse a livello di progetto. La definizione del budget delle risorse per un progetto genera il Costo manodopera preventivato del progetto.

Prima di questa modifica, è possibile visualizzare le informazioni sul budget risorse nel caso aziendale se il progetto è stato preventivato per le risorse nella Programmazione risorse globale.

Per ulteriori informazioni sul completamento del budget delle risorse di progetto nel Business Case, vedere [Risorse budget nel Business Case](../../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

## Visualizzazione in Pianificazione risorse - Grafico di allocazione utenti {#visualization-in-the-resource-planner-user-allocation-chart}

Ora puoi visualizzare l’allocazione pianificata complessiva di tutti gli utenti in base alla loro disponibilità in un grafico nella Programmazione delle risorse. Il grafico è disponibile quando si seleziona **Visualizza per utente** nella Programmazione delle risorse.

Il grafico visualizza le seguenti informazioni:

* % disponibilità senza allocazione eccessiva per tutti gli utenti
* % allocazione eccessiva per tutti gli utenti
* % sottoutilizzo per tutti gli utenti
* È presente un&#39;allocazione eccessiva per almeno un utente durante questo periodo

Prima di questa modifica, era possibile visualizzare l’allocazione e la disponibilità di singoli utenti solo in formato tabella.

Per ulteriori informazioni sul grafico di allocazione utente nella Programmazione delle risorse, vedere [Panoramica sulla Programmazione delle risorse](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Miglioramenti nell’area Home {#improvements-in-the-home-area}

Nell’area Home sono ora disponibili diversi miglioramenti, tra cui:

* Miglioramenti a livello di aspetto

   * Il pannello a destra è ora più grande e offre più spazio per le informazioni su attività e problemi.
   * Gli elementi scaduti vengono ora visualizzati in una tonalità di rosso più chiaro se selezionati nel pannello a sinistra.
   * Ora è più facile vedere la relazione tra il pannello sinistro e quello destro. Il documento selezionato nel pannello sinistro punta al pannello destro.

* I campi predefiniti vengono visualizzati per gli elementi selezionati. 

  Per ulteriori informazioni sui campi predefiniti, vedere &quot;Creazione e gestione di modelli di layout&quot;.

* Dopo aver fatto clic su &quot;Lavoraci&quot; su una richiesta, i campi associati al problema vengono visualizzati nel pannello di destra.

  Per ulteriori informazioni sull&#39;utilizzo delle richieste provenienti dall&#39;area Home, vedere [Gestire le richieste di lavoro e team nell&#39;area Home](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md) in [Gestire le richieste di lavoro e team nell&#39;area Home](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md).

* Per visualizzare il nome di un utente, posiziona il puntatore del mouse su un avatar utente in un elemento di lavoro nel pannello a sinistra.
* Espandere l&#39;area &quot;In ritardo&quot; nel pannello sinistro per visualizzare tutti gli elementi in ritardo (quando quest&#39;area è compressa, vengono visualizzati solo i primi 5 elementi).
* Dopo aver contrassegnato un elemento come Completo, l’elemento rimane nel pannello a sinistra fino a quando non ne selezioni un altro.\
  Per informazioni sulla visualizzazione degli elementi completati, vedere [Visualizzare gli elementi nell&#39;area Work List nell&#39;area Home](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) in [Visualizzare gli elementi nell&#39;area Work List nell&#39;area Home](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

Per ulteriori informazioni sull&#39;utilizzo della nuova area Home e per informazioni sulle differenze di funzionalità tra Il mio lavoro e Home, vedere [Utilizzare l&#39;area Home](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Nuovi miglioramenti del visualizzatore di bozze  {#new-proofing-viewer-improvements}

* [Layout e progettazione migliorati](#improved-layout-and-design)
* [Cerca commenti per numero di commento](#search-comments-by-comment-number)
* [Opzione per modificare il commento accanto all&#39;indicatore di markup](#option-to-edit-comment-next-to-the-markup-indicator)
* [Contrassegna tutti i commenti come letti](#mark-all-comments-as-read)
* [Miglioramenti al menu a sinistra](#left-menu-improvements)

### Layout e design migliorati {#improved-layout-and-design}

Il visualizzatore di bozze ha un aspetto aggiornato. Il  sono state aggiornate le seguenti aree del visualizzatore di bozze:

* Area miniature

  Per ulteriori informazioni sull&#39;utilizzo dell&#39;area delle miniature, vedere in.

* Area Commenti\
  Per ulteriori informazioni sull&#39;area commenti, vedere .
* Area del menu a sinistra

### Cerca commenti per numero commento {#search-comments-by-comment-number}

Ora, quando si cerca l’elenco dei commenti nel visualizzatore di bozze, è possibile immettere il numero del commento nel campo di ricerca. L’elenco dei commenti viene quindi filtrato per visualizzare il commento cercato. 

Per ulteriori informazioni, consulta in .

### Opzione per modificare il commento accanto all&#39;indicatore di markup {#option-to-edit-comment-next-to-the-markup-indicator}

È ora possibile modificare più facilmente un commento esistente. Dopo aver fatto clic su un indicatore di commento nella bozza, accanto al fumetto viene visualizzata un’icona di modifica. 

Prima di questa modifica, era necessario fare clic sull’icona di modifica nell’area Commento.  

Per ulteriori informazioni, consulta .

### Contrassegna tutti i commenti come letti {#mark-all-comments-as-read}

Quando si visualizza un documento nel visualizzatore di bozze, è ora possibile contrassegnare tutti i commenti come Letti.

### Miglioramenti al menu a sinistra {#left-menu-improvements}

Il menu sul lato sinistro del visualizzatore di bozze contiene i seguenti miglioramenti:

* Aspetto aggiornato
* Icona nella parte superiore del menu per mostrare o nascondere il menu

  ![proof_viewer_menu_hide.png](assets/proof-viewer-menu-hide.png)

* Passa il puntatore del mouse sul menu per espandere automaticamente il menu e visualizzare le etichette oltre alle icone. Oppure abilitate l&#39;opzione per mantenere il menu sempre nella vista compressa.
