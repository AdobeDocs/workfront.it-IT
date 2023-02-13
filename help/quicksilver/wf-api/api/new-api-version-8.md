---
content-type: api
navigation-topic: api-navigation-topic
title: Novità dell’API versione 8
description: Elenco delle risorse nuove dell’API versione 9. Per un elenco degli aggiornamenti apportati alle risorse della versione 8, visita Aggiornamenti alla versione 8 dell’API
author: John
feature: Workfront API
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 32%

---

# Novità dell’API versione 8

## Nuove risorse

Elenco delle risorse nuove dell’API versione 9. Per un elenco degli aggiornamenti apportati alle risorse della versione 8, visita [Aggiornamenti alla versione 8 dell’API](../../wf-api/api/new-api-version-8-updates.md)

**LavoroAgile**

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| backlogOrder | cliente |   |   | bulkCopy  |   | COPIA |
| color | iterazione  |   |   |   |   | CONTEGGIO |
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

{style=&quot;table-layout:auto&quot;}

### APIVersionMetadata

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | CONTEGGIO  |
| removeRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | RAPPORTO |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

**KanbanBoard**

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | AGGIUNGI |
| name |   |   |   |   |   | CONTEGGIO |
|   |   |   |   |   |   | ELIMINA |
|   |   |   |   |   |   | MODIFICA |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORTO |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### StatoApprovazioneProof

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovedStatusID |   |   |   |   |   |   |
| proofApprovedStatusLabel |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ProofFileMetadata**

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ResourceBudgetedHour**

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| allocateDate |   |   |   |   |   | AGGIUNGI |
| budgetedHours |   |   |   |   |   | CONTEGGIO |
| ScheduledBudgetedHours |   |   |   |   |   | ELIMINA |
| projectID |   |   |   |   |   | MODIFICA |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | RAPPORTO |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### ResourcePlannerFilter

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | AGGIUNGI |
| name |   |   |   |   |   | CONTEGGIO |
|   |   |   |   |   |   | ELIMINA |
|   |   |   |   |   |   | MODIFICA |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORTO |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

**NotaRichText**

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | CONTEGGIO |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORTO |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### Iscrizione

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | abbonati | AGGIUNGI |
|   |   |   |   | removeSubscribers |   | CONTEGGIO  |
|   |   |   |   | abbonati |   | ELIMINA |
|   |   |   |   | annulla sottoscrizione |   | GET |
|   |   |   |   |   |   | RAPPORTO |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### UserRole

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| roleID | ruolo |   |   |   |   |   |
| timePercentage | user |   |   |   |   |   |
| userID |   |   |   |   |   |   |
