---
title: Panoramica sulle limitazioni degli oggetti di Adobe Workfront Planning
description: Adobe Workfront Planning prevede dei limiti per il numero di oggetti che è possibile creare nell’istanza. Sono stati definiti dei limiti di oggetto per migliorare le prestazioni dei prodotti e l'esperienza con Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 2%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Panoramica sui limiti degli oggetti di Adobe Workfront Planning

Adobe Workfront Planning prevede dei limiti per il numero di oggetti che è possibile creare nell’istanza. Sono stati definiti dei limiti di oggetto per migliorare le prestazioni dei prodotti e l&#39;esperienza con Workfront Planning.

Nella tabella seguente vengono illustrati i limiti per il numero di oggetti che è possibile creare in Workfront Planning. I limiti sono soggetti a modifiche man mano che passiamo alle fasi successive di sviluppo.

| Oggetto Adobe Workfront Planning | Limite |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Numero di aree di lavoro per un’istanza Workfront | 1.000 |
| Numero di sezioni per un’area di lavoro | 50 |
| Numero di tipi di record per un&#39;area di lavoro | 1.000 (sono inclusi i tipi di record di tutte le sezioni e quelli creati quando si utilizza un modello di workspace) |
| Numero di record per un tipo di record | 50.000 |
| Numero di campi per un tipo di record o una tassonomia | 500 |
| Numero di caratteri per un campo di testo | 1.000 caratteri |
| Dimensione del file che è possibile incollare in una tabella del tipo di record | 1 MB |
| Dimensione del file che è possibile importare tramite l’API per una tabella del tipo di record | 1,5 MB |
| Frequenza con cui è possibile effettuare richieste API | 200 richieste al minuto |
| Numero di visualizzazioni che un utente può creare per un tipo di record | 100 |

<!--| Size of CSV of Excel file you can import* | 5MB |-->

<!--[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.-->

<!--At GA, replace the table above with this:

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   unlimited*                                                                                                        |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   25,000                                                                                                        |
|     Number of records for one workspace                                               |   25,000 for customers with the Planning plan <br> 500,000 for customers with the Planning Plus  plan                                                                                                         |
|     Number of total records for one instance of Workfront Planning type                                               |   500,000 for customers with the Planning plan <br>2 million for customers with the Planning Plus plan                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Number of views one user can create for one record type | 100 |

*We recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.

****************KEEP THIS COMMENTED OUT:
| Size of CSV of Excel file you can import** | 5MB |
**This functionality has been temporarily removed and it will be available at a later date.**********************
-->