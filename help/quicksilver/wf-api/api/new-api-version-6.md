---
content-type: api
navigation-topic: api-navigation-topic
title: Novità dell’API versione 6
description: Novità dell’API versione 6
author: Becky
feature: Workfront API
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 42%

---

# Novità dell’API versione 6

## Nuovi oggetti

### Responsabile risorse

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID | cliente |   |   |   |   | Aggiungi |
| customerID | progetto |   |   |   |   | Count |
| projectID | resourceManager |   |   |   |   | Elimina |
| resourceManagerID | template |   |   |   |   | Get |
| templateID |   |   |   |   |   | Rapporto  |
|   |   |   |   |   |   | Ricerca  |


### Ews

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | caricare |   |
| impugnatura |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### Etichetta personalizzata

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | Aggiungi |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | Count |
|   |   |   |   | removeCustomLabel |   | Elimina |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | Rapporto |
|   |   |   |   |   |   | Ricerca |


## Oggetti aggiornati

Modifiche agli oggetti esistenti: le aggiunte sono semplicemente elencate, le rimozioni hanno barrato, le modifiche a esistenti hanno una nota allegata dopo la tabella

### Aggiorna

 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| updateType¹ |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID² |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori

² l&#39;attributo hasFilters è stato modificato in true

 

### Approval

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManager | resourceManagerIDs |   |   |   |
| ConstrDate¹ |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Convalida della data aggiunta

² Aggiunta del flag NOT_FILTERABLE

 

### Processo di approvazione

|   | Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|---|
|  |  | `attachedApprovalPaths` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Passaggio di approvazione

 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| authorizationType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori

 

### Percorso di approvazione¹

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| approvatoStatus |   |   |   |   |   | Aggiungi |
| approvatoStatusLabel |   |   |   |   |   | Count |
| commento |   |   |   |   |   | Elimina |
| enterByID |   |   |   |   |   | Modifica |
| entryDate |   |   |   |   |   | Get |
| globalPathID |   |   |   |   |   | Rapporto |
| isPrivate |   |   |   |   |   | Ricerca |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| name² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modificato in Oggetto di Comunicazione

² Convalida della lunghezza massima aggiunta

 

### Oggetto del servizio di lavoro

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ConstrDate¹ |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired² |   |   |   | workItemStatusLabels  |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Aggiunta convalida data

² Flag non_filtrabile aggiunto

 

### Assegnazione

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Linea di base 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Contrassegno non_filtrabile aggiunto

 

### Attività linea di base

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Contrassegno non_filtrabile aggiunto

 

### Fatturazione

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| billingDate¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Aggiunta del flag del campo NO_TIME

### Evento Burndown 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style=&quot;table-layout:auto&quot;}

 

### Categoria 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style=&quot;table-layout:auto&quot;}

 

Enum personalizzata 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuses |   |
|   |   |   |   | isPossibileToUnlockStatus | projectGroupStatuses |   |
|   |   |   |   |   | taskGroupStatuses |   |

{style=&quot;table-layout:auto&quot;}

 

Documento 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

Tasso di cambio 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| tasso¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Convalida PRECISION modificata per 8 a 9

 

### Integrazione

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Voce del diario

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| changeType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori

 

### Optask (problema)¹ 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Contrassegnato come RESTORABLE

² Flag non_filtrabile aggiunto

 

### Progetto¹ 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManager | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| lavorare |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Contrassegnato come RESTORABLE e RESOURCE_MANAGEABLE

² Flag non_filtrabile aggiunto

 

### Attività¹

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ConstrDate² |   |   |   |   |   |   |
| workRequired³ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Contrassegnato come RESTORABLE

² Aggiunta della convalida AT_DATE_YEAR_BEFORE

³ Flag non_filtrabile aggiunto

 

### Team

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Modello¹ 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   | resourceManager | resourceManagerIDs |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Contrassegnato come RESTORABLE e RESOURCE_MANAGEABLE

### Attività modello¹ 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Contrassegnato come RESTORABLE

² Flag non_filtrabile aggiunto

 

### Utente

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| myInfo¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Violatori MAX_LENGTH

 

### Nota utente

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| eventType¹ |   |   |   |   | myNotifications² |   |

{style=&quot;table-layout:auto&quot;}

¹ Valori possibili modificati

² presenta filtri modificati in `[true]`

 

### Notifica

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
