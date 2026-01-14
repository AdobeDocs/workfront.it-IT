---
title: Panoramica sulle limitazioni degli oggetti di Adobe Workfront Planning
description: Adobe Workfront Planning prevede dei limiti per il numero di oggetti che è possibile creare nell’istanza. Sono stati definiti dei limiti di oggetto per migliorare le prestazioni dei prodotti e l'esperienza con Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 2a640cd5-f4a8-4ff3-81b6-32f85f6e4535
source-git-commit: 9a7ab1928bfd25c197fca65eddfba1bc01977ea7
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 4%

---


<!--keep the 30 connection limit in yellow till Jan 2026-->

# Panoramica sui limiti degli oggetti di Adobe Workfront Planning

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases.</span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}


Adobe Workfront Planning prevede dei limiti per il numero di oggetti che è possibile creare nell’istanza. Sono stati definiti dei limiti di oggetto per migliorare le prestazioni dei prodotti e l&#39;esperienza con Workfront Planning.

Nella tabella seguente vengono illustrati i limiti per il numero di oggetti che è possibile creare in Workfront Planning. Le limitazioni sono soggette a modifiche.

| Oggetto Adobe Workfront Planning | Limite |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Numero di aree di lavoro per un’istanza Workfront | Senza limiti* |
| Numero di sezioni per un’area di lavoro | 50 |
| Numero di tipi di record per un&#39;area di lavoro | 100 (sono inclusi i tipi di record di tutte le sezioni e quelli creati quando si utilizza un modello workspace) |
| Numero di record per un tipo di record | 25.000 |
| Numero di record per un&#39;area di lavoro | Selezione pianificazione: 25.000 <br> Prime pianificazione: 500.000 <br> Ultimate pianificazione: 1.000.000 |
| Numero di record totali per un&#39;istanza di Workfront Planning | Selezione pianificazione: 500.000 <br> Pianificazione Prime: 2.000.000 <br> Pianificazione Ultimate: Unlimited |
| Numero di campi per un tipo di record o una tassonomia | 500 |
| Numero di caratteri per un campo di testo a riga singola | 1.000 caratteri |
| Numero di caratteri per un campo paragrafo | 10.000 caratteri |
| Numero di campi paragrafo per un tipo di record | 20 campi paragrafo |
| Dimensione del file che è possibile utilizzare per importare informazioni in una tabella di tipo record | 1 MB |
| Dimensione del file che è possibile utilizzare per importare informazioni in una tabella del tipo di record tramite l’API | 1,5 MB |
| Frequenza con cui è possibile effettuare richieste API | 200 richieste al minuto |
| Numero di visualizzazioni che un utente può creare per un tipo di record | 100 |
| Dimensione del file CSV di Excel che puoi importare per creare tipi di record | 5 MB |
| Numero di righe che è possibile importare in un file CSV o Excel per creare tipi di record | 25.000 |
| Numero di colonne che è possibile importare in un file CSV o Excel per creare tipi di record | 500 |
| Numero di campi formula per un tipo di record | 20 |
| Numero di campi di connessione per un tipo di record | 30 |
| Numero di caratteri in un&#39;espressione del campo formula | 50.000 |
| Numero di entità (utenti, ruoli, team, società, gruppi) con cui è possibile condividere un oggetto Planning | 100 |
| Numero di tipi di record in una gerarchia | 4 |
| Numero di gerarchie in un’area di lavoro | 5 |
| Numero di record di un tipo di record padre connessi a un record di un tipo di record figlio all&#39;interno di una gerarchia | 10 |
| Numero di record connessi a un record in un tipo di connessione a selezione multipla, senza una gerarchia configurata tra i record | 500 |

*Si consiglia di non disporre di troppe aree di lavoro, in quanto potrebbero diventare difficili da gestire e i flussi di lavoro potrebbero essere troppo frammentati.

Per informazioni sui prezzi e sulla creazione di pacchetti di Workfront Planning, contattare l&#39;account manager.

<!--
****************KEEP THIS COMMENTED OUT:

**This functionality has been temporarily removed and it will be available at a later date.**********************
-->


<!--OLD limitations (before GA:)

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   1,000                                                                                                         |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   50,000                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Number of views one user can create for one record type | 100 |

-->
<!--| Size of CSV of Excel file you can import* | 5MB |-->

<!--[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.-->
