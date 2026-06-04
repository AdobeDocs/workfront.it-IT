---
content-type: api
navigation-topic: api-navigation-topic
title: Novità nella versione API 8
description: Questo è un elenco di risorse nuove per la versione API 9. Per un elenco degli aggiornamenti apportati alle risorse della versione 8, visita Aggiornamenti all’API versione 8
author: Becky
feature: Workfront API
role: Developer
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
TQID: https://experienceleague.adobe.com/bKFAN--rVO1yxgFLiyhXolgUBajVGYQxM7pBUuqy3v8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 269
ht-degree: 44%

---

# Novità nella versione API 8

## Nuove risorse

Questo è un elenco di risorse nuove per la versione API 9. Per un elenco degli aggiornamenti apportati alle risorse della versione 8, visita [Aggiornamenti alla versione API 8](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| backlogOrder | cliente |   |   | bulkCopy  |   | COPIA |
| colore | iterazione  |   |   |   |   | CONTEGGIO |
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
| deprecationRelease |   |   |   |   |   | CONTEGGIO  |
| removeRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | RAPPORTO |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**KanbanBoard**

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | AGGIUNGI |
| name |   |   |   |   |   | CONTEGGIO |
|   |   |   |   |   |   | DELETE |
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
| BudgetedHours |   |   |   |   |   | CONTEGGIO |
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
| name |   |   |   |   |   | CONTEGGIO |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | MODIFICA |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORTO |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**RichTextNote**

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | CONTEGGIO |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORTO |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### Iscrizione

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | abbonati | AGGIUNGI |
|   |   |   |   | removeSubscribers |   | CONTEGGIO  |
|   |   |   |   | abbonamenti |   | DELETE |
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
