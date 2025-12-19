---
content-type: release-notes
title: Attività della versione del primo trimestre 2026 per Adobe Workfront Planning
description: Questa è l’attività di rilascio per il prodotto Adobe Workfront Planning per il primo trimestre 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 46f3be50925d2e830c572ce9bbad0d3b320f6a95
workflow-type: tm+mt
source-wordcount: '1501'
ht-degree: 0%

---

# Attività della versione del primo trimestre 2026 per Adobe Workfront Planning

Questo articolo descrive le funzioni rilasciate per Workfront Planning durante la versione del primo trimestre 2026.

<!--keep the sentence below for all future quarterly release pages-->

Per un elenco di tutte le funzionalità rilasciate per Adobe Workfront Planning, vedere [Attività di rilascio di Adobe Workfront Planning: indice articolo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Miglioramenti alle pagine dei record connessi

>[!NOTE]
>
>Anteprima: 19 dicembre 2025
>Velocità di produzione: 14 gennaio 2026
>Produzione per tutti: 15 gennaio 2026

Per offrire maggiore flessibilità nell&#39;utilizzo delle pagine dei record collegate, è stata migliorata la funzionalità delle visualizzazioni in quest&#39;area di Workfront Planning. Di seguito sono riportati i miglioramenti apportati alle pagine dei record connessi di un record:

* È ora possibile aggiungere una visualizzazione timeline e una visualizzazione calendario alla pagina dei record connessi di un record.
* È ora possibile condividere tutte le visualizzazioni da una pagina di record connessi. Le visualizzazioni condivise da queste pagine sono visibili a livello di sistema da tutti gli utenti con cui le condividi in qualsiasi altra area di Workfront Planning. Tutte le visualizzazioni condivise in qualsiasi altra area di Planning sono visibili anche nella pagina dei record connessi per gli stessi utenti con cui sono condivise.
* È stata aggiunta una restrizione per consentire una sola pagina di record connessi per ogni record o tipo di oggetto. Prima di questo miglioramento, era possibile aggiungere più pagine per lo stesso record o tipo di oggetto. È ora possibile utilizzare più visualizzazioni per lo stesso tipo di record in una pagina record connessi.
* È stato aggiunto un collegamento **Nuova riga** nella parte inferiore di una visualizzazione tabella e un pulsante **Connetti record** nell&#39;area superiore destra della pagina dei record connessi. Prima di questo miglioramento, il collegamento **Nuova riga** e il pulsante **Connetti record** esistevano solo in una pagina connessa al progetto.

Per informazioni, vedere [Aggiungere una pagina Record connessi a un record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

## Condividere le visualizzazioni nella pagina dei record Progetti connessi

>[!NOTE]
>
>Anteprima: 18 dicembre 2025
>Versione rapida di produzione: 14 gennaio 2026\
>Produzione per tutti: 15 gennaio 2026

Per essere certi di visualizzare le informazioni necessarie in modo più semplice, è stata aggiunta la possibilità di condividere le visualizzazioni nella pagina dei record Progetti connessi. Ora puoi condividere le visualizzazioni con altri utenti, team o gruppi.

Per informazioni, vedere [Aggiungere una pagina Record connessi a un record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

## Il carattere jolly dell&#39;utente corrente è ora disponibile nei filtri di visualizzazione della connessione del progetto

>[!NOTE]
>
>Anteprima: 18 dicembre 2025
>Versione rapida di produzione: 14 gennaio 2026\
>Produzione per tutti: 15 gennaio 2026

Per facilitare il filtraggio delle connessioni dei progetti a te applicabili, è stato creato un carattere jolly per l&#39;utente corrente. Ora, quando si filtra, è possibile selezionare &quot;Me (logged in user)&quot; (Io utente connesso). Il filtro verrà quindi applicato all’utente che sta visualizzando l’elenco delle richieste.

Questa funzione può risultare utile quando si aggiunge un filtro a una visualizzazione che verrà utilizzata da più utenti. Ogni utente visualizzerà i risultati dei filtri ad esso applicabili.

Il carattere jolly è disponibile nei campi in cui il valore è un utente.

Per ulteriori informazioni sulla configurazione delle visualizzazioni delle connessioni al progetto, inclusi i filtri, vedere [Aggiungere una pagina Record connessi a un record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

<!--

## Create record type hierarchies in workspaces

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production all: January 15, 2026 

You can now define flexible but structured hierarchies between record or object types.  

Hierarchies are connections between record types. You can have up to 4 record and object types connected in one hierarchy, and you can have multiple hierarchies in one workspace. The first record type in the hierarchy is a parent, and all the other record or object types are its children objects.  

You can use hierarchies to organize work in a way that reflects how your teams actually plan, operate, and deliver and to visualize how strategy flows into execution. 

Consider the following when building hierarchies: 

* You can have multiple hierarchies in a workspace 
* You can connect only Planning record types from one workspace and Workfront projects in a hierarchy.  
* A record type or a project can only have one parent in the same workspace. 
* A record type can be the parent in multiple hierarchies 
* Connectable record types cannot be used in hierarchies in other workspaces than their own. 
* Global record types can be used in hierarchies only in the workspaces that they were created in or have been added to.  

When you create hierarchies between record types, they generate breadcrumbs for records that belong to those record types. 

For more information, see [Hierarchy and breadcrumb overview](help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

-->

<!--

## New unified breadcrumbs added to records' pages

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production for all: January 15, 2026 

We have added breadcrumbs to a record's page to reflect its spot in a hierarchy. After you create hierarchies, you can see a record's breadcrumb at the top of its page, indicating what other parent or children objects are connected to it. Hierarchies are consistent across Workfront and Planning.  

For example, you can view a project's Planning hierarchy when it's connected to Planning record types in its Planning breadcrumb, and its Workfront hierarchy when it's connected to Workfront object types, like Portfolios or Programs, in Workfront.  

For information, see [Hierarchy and breadcrumb overview](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

-->

## Miglioramenti alla pagina principale di Workspace

>[!NOTE]
>
>Anteprima: 18 dicembre 2025
>Velocità di produzione: 14 gennaio 2026
>Produzione per tutti: 15 gennaio 2026

Sono stati apportati i seguenti miglioramenti alla pagina principale delle aree di lavoro in Workfront Planning:

* Esperienza di scorrimento più veloce e dinamica. Ciò è particolarmente visibile se l’organizzazione dispone di un numero elevato di aree di lavoro e per gli amministratori di sistema.

* È stata aggiunta una casella di ricerca che ora consente di cercare un’area di lavoro specifica per nome.

* La scheda **Altre aree di lavoro** è stata rinominata **Tutte le aree di lavoro** e include tutte le aree di lavoro per le quali si dispone almeno delle autorizzazioni di visualizzazione, incluse quelle create dall&#39;utente.

Per informazioni, vedere [Modifica aree di lavoro](/help/quicksilver/planning/architecture/edit-workspaces.md).



## Aggiunta del campo Connessione marchio a Prodotti e utenti tipo per impostazione predefinita nell’area di lavoro di GenStudio

>[!NOTE]
>
>Anteprima: 11 dicembre 2025
>Versione rapida di produzione: 11 dicembre 2025
>Produzione per tutti: 11 dicembre 2025
>[!BADGE Fuori programma]{type=Neutral}

Il campo di connessione con il marchio GenStudio for Performance Marketing viene ora aggiunto per impostazione predefinita ai tipi di record Prodotti e utenti tipo nell’area di lavoro GenStudio di Workfront Planning.

La tua organizzazione deve avere sia Workfront Planning che Adobe GenStudio for Performance Marketing.

Prima di questo miglioramento, era possibile aggiungere il campo di connessione al marchio solo manualmente a qualsiasi tipo di record, inclusi Prodotti e utenti tipo. È comunque possibile collegare manualmente il tipo di record di Brand GenStudio ad altri tipi di record in Workfront Planning.

Per informazioni, vedere [Introduzione all&#39;integrazione di Adobe Workfront Planning e Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

## Limita la rimozione delle autorizzazioni degli utenti di GenStudio for Performance Marketing da Planning

>[!NOTE]
>
>Anteprima: 11 dicembre 2025
>Versione rapida di produzione: 11 dicembre 2025
>Produzione per tutti: 11 dicembre 2025
>[!BADGE Fuori programma]{type=Neutral}

È stato aggiunto un guardrail che impedisce la rimozione delle autorizzazioni degli utenti di GenStudio for Performance Marketing dagli oggetti di Workfront Planning. Grazie a questo miglioramento, non sarà più possibile rimuovere gli utenti di GenStudio dall&#39;area di lavoro di GenStudio in Planning, né disabilitare le autorizzazioni ereditate per i tipi di record nell&#39;area di lavoro di GenStudio, se tali autorizzazioni includono gli utenti di GenStudio. Prima di questo miglioramento, se rimuovessi questi utenti dall’area di lavoro di GenStudio in Planning, perderebbero le autorizzazioni per i tipi di record anche in GenStudio.

La tua organizzazione deve avere sia Workfront Planning che Adobe GenStudio for Performance Marketing.

Per informazioni, vedere [Introduzione all&#39;integrazione di Adobe Workfront Planning e Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).


## È stata rimossa la condivisione pubblica delle viste su un tipo di record globale in un’area di lavoro secondaria


>[!NOTE]
>
>Anteprima: 3 dicembre 2025
>Versione rapida di produzione: 4 dicembre 2025
>Produzione per tutti: 15 gennaio 2026


È stata rimossa la scheda Condivisione pubblica quando si condivideva una vista per un record globale in un’area di lavoro secondaria. Non è possibile condividere una visualizzazione pubblicamente da un tipo di record globale aggiunto a un&#39;altra area di lavoro da un tipo di record globale esistente. È possibile condividere una visualizzazione del tipo di record globale pubblicamente dalla relativa area di lavoro originale.

Per informazioni, vedere [Condividi visualizzazioni](/help/quicksilver/planning/access/share-views.md).


## Collegare i marchi GenStudio for Performance Marketing ai tipi di record di Workfront Planning

>[!NOTE]
>
>Anteprima: 13 novembre 2025
>Versione rapida di produzione: 13 novembre 2025
>Produzione per tutti: 13 novembre 2025

È ora possibile collegare i tipi di record di Workfront Planning ai Marchi di Adobe GenStudio for Performance Marketing. La tua organizzazione deve avere sia Workfront Planning che Adobe GenStudio for Performance Marketing.

Per ulteriori informazioni, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).


## Nuova casella di ricerca dei campi nelle icone Filtri, Campi e Colori riga nelle visualizzazioni di Planning

>[!NOTE]
>
>Anteprima: 6 novembre 2025
>Versione rapida di produzione: 11 dicembre 2025
>Produzione per tutti: 15 gennaio 2026

È ora possibile cercare un campo specifico durante la creazione di un elemento di visualizzazione in una visualizzazione del tipo di record. Sono state aggiunte caselle di ricerca quando si crea un filtro, si ordina, si raggruppa o quando si configurano i campi o i colori delle righe. Prima di questo miglioramento, era sufficiente scorrere l’elenco dei campi disponibili.

Questo miglioramento è disponibile in tutte le visualizzazioni dei tipi di record.

Per informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).


## Tipi di record globali e la possibilità di aggiungerli come tipi di record esistenti ad altre aree di lavoro

>[!NOTE]
>
>Anteprima: 16 ottobre 2025
>Versione rapida di produzione: 13 novembre 2025
>Produzione per tutti: 15 gennaio 2026

Quando si implementa Workfront Planning per un’organizzazione con più team e flussi di lavoro comuni, potrebbe essere necessario definire una struttura coesa e i metadati per i tipi di record chiave (come Campagne o Deliverable) che possono essere aggiunti alle aree di lavoro di ciascun team per acquisire e gestire il proprio lavoro.

Inoltre, potrebbe essere necessario il lavoro di ogni team per raggiungere un livello centrale.

Con un flusso di lavoro di questo tipo, puoi fare in modo che i team acquisiscano in modo coerente il proprio lavoro e allo stesso tempo sblocchino la visibilità tra i team, senza dover aggiungere tutti gli utenti dell’organizzazione a ogni area di lavoro. A tale scopo, è possibile utilizzare i tipi di record globali.

È ora possibile designare un tipo di record come globale e utilizzarlo in più aree di lavoro. Gli utenti possono utilizzare la stessa struttura di campi e le stesse connessioni già configurate in un’area di lavoro centrale.

Per ulteriori informazioni, consulta i seguenti articoli:

* [Panoramica del tipo di record tra aree di lavoro](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

* [Configurare le funzionalità tra aree di lavoro diverse per il tipo di record](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)

* [Aggiungere tipi di record esistenti da un&#39;altra area di lavoro](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## Nuovo limite per i campi di connessione per un tipo di record

>[!NOTE]
>
>Anteprima: 16 ottobre 2025
>Versione rapida di produzione: 13 novembre 2025
>Produzione per tutti: 15 gennaio 2026

È stato introdotto un limite di 30 campi di connessione per ogni tipo di record.

NOTA: se l&#39;organizzazione dispone attualmente di più di 30 campi di connessione per un tipo di record, è possibile mantenere i campi aggiuntivi che superano il limite di 30. Non è tuttavia possibile aggiungere altri campi di connessione ai tipi di record che superano il limite. In futuro, verrà applicato il nuovo limite di 30 campi di connessione.

Per ulteriori informazioni, vedere [Panoramica sui tipi di record connessi](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Impostare valori descrittivi per le scelte dei campi di tipo selezionato

>[!NOTE]
>
>Anteprima: 16 ottobre 2025
>Versione rapida di produzione: 13 novembre 2025
>Produzione per tutti: 15 gennaio 2026

Quando si aggiungono scelte di campo a un campo a selezione singola o multipla, Workfront assegnerà valori univoci di facile utilizzo a ciascuna scelta. Prima di questo miglioramento, Workfront generava un ID alfanumerico difficile da comprendere e utilizzare nelle chiamate API e in altre integrazioni.

Considera quanto segue con questo miglioramento:

* I nuovi valori verranno aggiunti alle nuove scelte di campo. Le scelte di campo esistenti manterranno i loro ID alfanumerici.

* I valori di scelta sono univoci per un campo, ma possono essere ripetuti tra campi diversi.

* La ridenominazione di una scelta non ne aggiorna il valore originale.

* I valori di scelta vengono visualizzati in minuscolo e sono separati da trattini bassi nel caso di scelte tra più parole. Se utilizzi un’etichetta già utilizzata come altro nome di scelta per lo stesso campo, Workfront aggiunge al valore un numero sequenziale.

Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).






