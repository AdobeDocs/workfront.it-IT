---
content-type: api
navigation-topic: api-navigation-topic
title: Novità della versione 6 dell’API
description: Novità della versione 6 dell’API
author: Becky
feature: Workfront API
role: Developer
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 38%

---

# Novità della versione 6 dell’API

## Nuovi oggetti

### Responsabile risorse

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID | cliente |   |   |   |   | Aggiungi |
| customerID | progetto |   |   |   |   | Count |
| projectID | resourceManager |   |   |   |   | Elimina |
| resourceManagerID | modello |   |   |   |   | Ottenere |
| templateID |   |   |   |   |   | Rapporto  |
|   |   |   |   |   |   | Ricerca  |


### Ews

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | caricare |   |
| maniglia |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### Etichetta personalizzata

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | Aggiungi |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | Count |
|   |   |   |   | removeCustomLabel |   | Elimina |
|   |   |   |   |   |   | Ottenere |
|   |   |   |   |   |   | Rapporto |
|   |   |   |   |   |   | Ricerca |


## Oggetti aggiornati

Modifiche agli oggetti esistenti: le aggiunte sono semplicemente elencate, le rimozioni sono barrate, le modifiche a esistenti hanno una nota allegata dopo la tabella

### Aggiorna

 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Modifiche ai valori possibili

<sup>2</sup> attributo hasFilters modificato in true

 

### Approval

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManagers | resourceManagerIDs |   |   |   |
| constraintDate<sup>1</sup> |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Convalida data aggiunta

<sup>2</sup> Flag NOT_FILTERABLE aggiunto

 

### Processo di approvazione

|   | Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### Passaggio di approvazione

 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Modifiche ai valori possibili

 

### Percorso di approvazione<sup>1</sup>

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| approvalStatus |   |   |   |   |   | Aggiungi |
| approvalStatusLabel |   |   |   |   |   | Count |
| commento |   |   |   |   |   | Elimina |
| enteredByID |   |   |   |   |   | Modifica |
| entryDate |   |   |   |   |   | Ottenere |
| globalPathID |   |   |   |   |   | Rapporto |
| isPrivate |   |   |   |   |   | Ricerca |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| nome<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Modificato in Segnalabile

<sup>2</sup> Convalida lunghezza massima aggiunta

 

### Oggetto servizio di lavoro

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired<sup>2</sup> |   |   |   | workItemStatusLabels  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Convalida data aggiunta

<sup>2</sup> Flag Not_Filterable aggiunto

 

### Assegnazione

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style="table-layout:auto"}

 

### Linea di base 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Flag Not_Filterable aggiunto

 

### Attività linea di base

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Flag Not_Filterable aggiunto

 

### Fatturazione

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| billingDate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> aggiunto flag di campo NO_TIME

### Evento Burndown 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style="table-layout:auto"}

 

### Categoria 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style="table-layout:auto"}

 

Enum personalizzata 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuses |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatuses |   |
|   |   |   |   |   | taskGroupStatus |   |

{style="table-layout:auto"}

 

Documento 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

Tasso di cambio 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| tariffa<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Convalida PRECISION modificata da 8 a 9

 

### Integrazione

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Voce del diario

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Modifiche ai valori possibili

 

### Optask (problema)<sup>1</sup> 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Contrassegnato come RIPRISTINABILE

<sup>2</sup> Flag Not_Filterable aggiunto

 

### Progetto<sup>1</sup> 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManagers | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| lavoro |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Contrassegnati come RESTORABLE e RESOURCE_MANAGEABLE

<sup>2</sup> Flag Not_Filterable aggiunto

 

### Attività<sup>1</sup>

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |   |   |   |   |   |   |
| workRequired<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Contrassegnato come RIPRISTINABILE

<sup>2</sup> Convalida AT_DATE_YEAR_BEFORE aggiunta

<sup>3</sup> Flag Not_Filterable aggiunto

 

### Team

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### Modello<sup>1</sup> 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   | resourceManagers | resourceManagerIDs |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Contrassegnati come RESTORABLE e RESOURCE_MANAGEABLE

### Attività modello<sup>1</sup> 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Contrassegnato come RIPRISTINABILE

<sup>2</sup> Flag Not_Filterable aggiunto

 

### Utente

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Violatori MAX_LENGTH

 

### Nota utente

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| eventType<sup>1</sup> |   |   |   |   | myNotifications<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Valori Possibili Modificati

<sup>2</sup> Filtri modificati in `[true]`

 

### Notifica

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
