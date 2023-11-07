---
content-type: api
navigation-topic: api-navigation-topic
title: Novità della versione 8 dell’API
description: Questo è un elenco di risorse nuove per la versione API 9. Per un elenco degli aggiornamenti apportati alle risorse della versione 8, visita Aggiornamenti all’API versione 8
author: Becky
feature: Workfront API
role: Developer
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 30%

---

# Novità della versione 8 dell’API

## Nuove risorse

Questo è un elenco di risorse nuove per la versione API 9. Per un elenco degli aggiornamenti apportati alle risorse della versione 8, visita [Aggiornamenti a API versione 8](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| backlogOrder | cliente |   |   | bulkCopy  |   | COPIA |
| colore | iterazione  |   |   |   |   | COUNT |
| customerID | lastUpdatedBy |   |   |   |   | ELIMINA |
| stima | opTask |   |   |   |   | MODIFICA |
| ID | progetto |   |   |   |   | GET  |
| isReady | storyboardParent |   |   |   |   | RAPPORTO |
| iterationID | attività |   |   |   |   | SEARCH |
| lastUpdateDate | team |   |   |   |   |   |
| lastUpdatedByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |
| opTaskID |   |   |   |   |   |   |
| parentStoryBoardOrder |   |   |   |   |   |   |
| projectID |   |   |   |   |   |   |
| storyBoardOrder |   |   |   |   |   |   |
| storyBoardParentID |   |   |   |   |   |   |
| taskID  |   |   |   |   |   |   |
| teamID |   |   |   |   |   |   |
| tipo |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style="table-layout:auto"}

### APIVersionMetadata

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | COUNT  |
| removeRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | RAPPORTO |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**KanbanBoard**

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | AGGIUNGI |
| name |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | ELIMINA |
|   |   |   |   |   |   | MODIFICA |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORTO |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ProofApprovalStatus

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style="table-layout:auto"}

**MetadatiFileBozza**

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style="table-layout:auto"}

**OraRisorsePreventivate**

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | AGGIUNGI |
| BudgetedHours |   |   |   |   |   | COUNT |
| plannedBudgetedHours |   |   |   |   |   | ELIMINA |
| projectID |   |   |   |   |   | MODIFICA |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | RAPPORTO |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ResourcePlannerFilter

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | AGGIUNGI |
| name |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | ELIMINA |
|   |   |   |   |   |   | MODIFICA |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORTO |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**RichTextNote**

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORTO |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### Iscrizione

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | abbonati | AGGIUNGI |
|   |   |   |   | removeSubscribers |   | COUNT  |
|   |   |   |   | abbonamenti |   | ELIMINA |
|   |   |   |   | annulla abbonamenti |   | GET |
|   |   |   |   |   |   | RAPPORTO |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### UserRole

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| roleID | ruolo |   |   |   |   |   |
| timePercentage | utente |   |   |   |   |   |
| userID |   |   |   |   |   |   |
