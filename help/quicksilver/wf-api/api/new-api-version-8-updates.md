---
content-type: api
navigation-topic: api-navigation-topic
title: Aggiornamenti alla versione 8 dell’API
description: 'Con questa versione dell’API Adobe Workfront sono state aggiornate le seguenti risorse esistenti. Per visualizzare le risorse nuove della versione 8, consulta Novità della versione 8 dell’API. Le modifiche apportate a una risorsa sono indicate nel modo seguente: MODIFICA ME.'
author: Becky
feature: Workfront API
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 37%

---

# Aggiornamenti alla versione 8 dell’API

## Risorse aggiornate

Con questa versione dell’API Adobe Workfront sono state aggiornate le seguenti risorse esistenti. Per visualizzare le risorse nuove della versione 8, consulta [Novità dell’API versione 8](../../wf-api/api/new-api-version-8.md). Le modifiche apportate a una risorsa vengono indicate nel modo seguente:

* Le aggiunte sono semplicemente elencate
* Le rimozione sono indicate con testo barrato
* Le modifiche sono riportate nella nota dopo la tabella

### AccessRequest

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| azione¹  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori

### AccessRule¹ 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| coreAction²  |   |   |   |   |   |   |
| ForbiddenActions² |   |   |   |   |   |   |
| secondarioActions² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Flag rimosso: SEGNALABILE\
² Modifiche ai possibili valori

### Approval

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  | resourcePools |   |   |   |   |
| backlogOrder² | kanbanBoard  |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori\
Campi aggiunti: DYNAMIC, LAZY_READ e NOT_GROUPABLE

### Assegnazione

|   |   |   |   | Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnTasks | getAssignAssignmentsForTasks  |   |   |   |   |   |
|   |   |   |   | swapUsersOnTasks | getUnassignAssignmentsForTasks |   |   |   |   |   |
|   |   |   |   | unassignUserFromTasks |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Cliente

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| bizRuleExclusions¹ |   |   |   | getPackagingOptionValue |   |   |
| proofPlan¹ |   |   |   | isPackagingOptionEnabled |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori

### CustomerPreferences

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| name¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori

### Approvazione documento

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Flag aggiunto: NOT_FILTERABLE

### DocumentVersion

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| activeProofStages |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Gruppo

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   | proprietari |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### HourType

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| appGlobalID¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Flag aggiunto: NOT_FILTERABLE

### Iterazione

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   | moveStories |   |   |

{style=&quot;table-layout:auto&quot;}

### Come

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Nota

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| auditType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori

### OpTask

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   | defaultShownTimesheetIssues  |   |
| backlogOrder | iterazione |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| stima |   |   |   |   |   |   |
| iterationID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori

### Portfolio

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori

### Programma

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori

### Progetto

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| auditTypes¹ |   | resourcePools |   |   | defaultShownTimesheetProjects |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori

### Approvazione bozza

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| approverID | approvatore |   |   |   |   |   |
| documentVersionID | documentVersion |   |   |   |   |   |
| ID¹ |   |   |   |   |   |   |
| proofCreationDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Flag aggiunto: NOT_FILTERABLE

### QueueDef

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| requestorCoreAction¹ |   |   |   |   |   |   |
| requestorForbiddenActions¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori

### Trfa

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| endDate |   |   |   | setRatesForRole  |   |   |
| name |   |   |   |   |   |   |
| startDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### TempoRiservato

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| extRefID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### ResourceManager

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| projectPriority |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Attività

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   | allTasksOnIterations  |   |
| backlogParent | kanbanBoard |   |   |   | defaultShownTimesheetTasks |   |
| kanbanBoardID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori

### Team

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| agileMethodology |   |   |   |   |   |   |
| autoAddNextStory |   |   |   |   |   |   |
| includeIssues |   |   |   |   |   |   |
| teamStoryBoardIssueStatuses |   |   |   |   |   |   |
| wipLimit |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Modello

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### AttivitàModello

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori

Aggiorna

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| updateType¹ | `updateEndorsement` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori

### Utente

|   |   | Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |   |   |
|   |   | userGroups |   |   |   |   |   |   |
|   |   | userRuoli |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### NoteUtente

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |
| `endorsementShareID` | `endorsementShare` |   |   |   |   |   |
| eventType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori

### Lavoro

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   |   |   |
| backlogOrder² | kanbanBoard  |   |   |   |   |   |
| backlogParent  |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche ai possibili valori\
Campi aggiunti: DYNAMIC, LAZY_READ e NOT_GROUPABLE
