---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: Miglioramenti al progetto 2020.2
description: Questa pagina descrive tutti i miglioramenti apportati all’ambiente di produzione con la versione 2020.2 di. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana dell’11 maggio 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 150bc838-d6a5-445a-af77-62c4ed74dd1b
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# Miglioramenti al progetto 2020.2

Questa pagina descrive tutti i miglioramenti apportati all’ambiente di produzione con la versione 2020.2 di. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana dell’11 maggio 2020.

Per un elenco di tutte le modifiche disponibili con la versione 2020.2, consulta [Panoramica sulla versione 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Per gli amministratori di Workfront: nuovo failsafe quando lo stato del progetto per i nuovi progetti è nascosto o sbloccato

In Configurazione, configura una preferenza per garantire che ogni nuovo progetto abbia un determinato stato al momento della creazione. Questo è importante perché un progetto ha sempre bisogno di uno stato per funzionare correttamente in Workfront, anche quando è nuovo di zecca.

Per fare in modo che i nuovi progetti abbiano sempre uno stato, anche se un amministratore nasconde o sblocca lo stato configurato per i nuovi progetti, il sistema ora assegna il primo stato nell&#39;elenco Stato a tutti i nuovi progetti fino a quando non configuri nuovamente il nuovo stato per i nuovi progetti.

Per informazioni sull&#39;impostazione della preferenza per lo stato di tutti i nuovi progetti, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (oppure, se si utilizza Adobe Workfront Classic, vedere [Impostazione delle preferenze di progetto](https://one.workfront.com/s/article/Setting-Project-Preferences-1883392298)).

**Disponibile in questi ambienti:**

* Adobe Workfront Classic
* La nuova esperienza Adobe Workfront

## Per gli amministratori di Workfront: progettazione migliorata nelle preferenze del progetto

L’impostazione delle preferenze di progetto ora è più intuitiva e facile da utilizzare:

* I titoli sono più grandi delle etichette delle opzioni, per trovare più rapidamente ciò che stai cercando.
* Le linee di divisione e gli spazi vuoti aggiuntivi separano ciascuna sezione in modo da poter mettere a fuoco più facilmente ciò che si sta facendo.
* Se si digita un numero non valido per un&#39;opzione, ad esempio &quot;Ore tipiche per giorno lavorativo&quot;, viene visualizzato immediatamente un messaggio di avviso invece di essere visualizzato dopo aver fatto clic su Salva.
* Le etichette delle opzioni corrispondono al testo dell’interfaccia corrispondente in altre aree di Workfront, ad esempio nell’area Dettagli e nei rapporti.

Per informazioni sull&#39;area Preferenze progetto, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (oppure, se si utilizza Adobe Workfront Classic, vedere [Impostazione delle preferenze progetto](https://one.workfront.com/s/article/Setting-Project-Preferences-1883392298)).

**Disponibile in questi ambienti:**

* Adobe Workfront Classic
* La nuova esperienza Adobe Workfront

## Filtro, visualizzazione e raggruppamento selezionati mantenuti negli elenchi Report

Ora viene selezionato l’ultimo filtro, visualizzazione o raggruppamento applicato a un rapporto specifico, anche se l’utente si disconnette e accede nuovamente a Workfront.

In precedenza, quando un utente applicava un filtro, una vista o un raggruppamento a un elenco di rapporti e poi si allontanava da tale pagina, il filtro, la vista o il raggruppamento predefiniti venivano visualizzati alla successiva navigazione dell’utente allo stesso rapporto.

**Disponibile in questi ambienti:**

* La nuova esperienza Adobe Workfront
* Adobe Workfront Classic

## Lo spostamento e la copia delle attività in un altro progetto mantengono il vincolo attività quando le attività possono rientrare nella sequenza temporale del progetto

È stato migliorato il modo in cui Workfront gestisce il vincolo attività specifico per data di un&#39;attività quando questa viene copiata o spostata in un altro progetto. Esempi di vincoli attività specifici per data sono Deve iniziare il, Deve finire il, Date fisse, Inizia non dopo il e così via.

Quando ad esempio si sposta o si copia un&#39;attività con un vincolo Deve iniziare il in un altro progetto la cui Data inizio pianificata è precedente alla Data inizio dell&#39;attività, l&#39;attività mantiene il vincolo dopo che è stata copiata o spostata. Quando si sposta o si copia un&#39;attività con un vincolo Deve iniziare il in un progetto la cui Data inizio pianificata è successiva alla Data inizio dell&#39;attività, il vincolo attività viene impostato su Il più presto possibile.

Prima di questa modifica, il vincolo dell’attività diventa sempre Appena possibile.

Per informazioni sullo spostamento delle attività, vedi [Sposta attività](../../../manage-work/tasks/manage-tasks/move-tasks.md) (o se utilizzi Adobe Workfront Classic, vedi [Spostamento delle attività](https://one.workfront.com/s/article/Moving-Tasks-2081996259)).

Per informazioni sulla copia delle attività, vedere [Copiare e duplicare le attività](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (oppure, se si utilizza Adobe Workfront Classic, vedere [Copiare e duplicare le attività](https://one.workfront.com/s/article/Copy-and-Duplicate-Tasks-218695605)).

Per una panoramica di tutti i vincoli di attività, vedere [Panoramica dei vincoli di attività](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (o se si utilizza Adobe Workfront Classic, vedere [Panoramica dei vincoli di attività](https://one.workfront.com/s/article/Task-Constraint-Overview-453396848)).

**Disponibile in questi ambienti:**

* Adobe Workfront Classic
* La nuova esperienza Adobe Workfront

## Impedire la perdita di dati durante l&#39;esecuzione di modifiche nella scheda Dettagli o in un elenco di attività

Per evitare la perdita di dati durante l&#39;aggiornamento manuale delle informazioni nella pagina Dettagli di un oggetto o di attività in un elenco di attività a livello di progetto, quando si salvano le modifiche viene visualizzato un messaggio di avvertenza per segnalare che sono presenti modifiche non salvate prima di tentare di modificare le informazioni nell&#39;intestazione. Le uniche azioni consentite prima di salvare le modifiche sono la sottoscrizione o l&#39;aggiunta dell&#39;oggetto ai preferiti.

Per informazioni sulla modifica delle attività in un elenco, vedere [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**Disponibile in questi ambienti:**

* La nuova esperienza Adobe Workfront

