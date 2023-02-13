---
content-type: api
navigation-topic: api-navigation-topic
title: Novità dell’API versione 10
description: Risorse aggiornate
author: John
feature: Workfront API
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 46%

---

# Novità dell’API versione 10

* [Nuove risorse](#new-resources)
* [Risorse aggiornate](#updated-resources)
* [Risorse rimosse](#removed-resources)

## Nuove risorse {#new-resources}

### ActivityLog

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | AGGIUNGI |
|   |   |   |   |   |   | CONTEGGIO |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### CalendarEntry

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | AGGIUNGI |
|   |   |   |   |   |   | CONTEGGIO  |
|   |   |   |   |   |   | ELIMINA  |
|   |   |   |   |   |   | MODIFICA  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RAPPORTO  |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### CalendarEntryExternalReference

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | CONTEGGIO |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RAPPORTO  |
|   |   |   |   |   |   | SEARCH  |

{style=&quot;table-layout:auto&quot;}

### ExternalAuthToken

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | AGGIUNGI |
|   |   |   |   |   |   | CONTEGGIO |
|   |   |   |   |   |   | ELIMINA  |
|   |   |   |   |   |   | MODIFICA  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RAPPORTO  |
|   |   |   |   |   |   | SEARCH  |

{style=&quot;table-layout:auto&quot;}

### LicenseTypeGroupLimit

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| customerID | cliente |   |   |   |   |   |
| groupID | gruppo |   |   |   |   |   |
| planLimit |   |   |   |   |   |   |
| usedLicense |   |   |   |   |   |   |
| limite di lavoro |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### UserHomeCalendarPreference

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| customerID | cliente |   |   |   |   | AGGIUNGI |
| edTime | user |   |   |   |   | CONTEGGIO |
| firstDayOfWeek |   |   |   |   |   | ELIMINA |
| ID |   |   |   |   |   | MODIFICA |
| showPTO |   |   |   |   |   | GET |
| startTime |   |   |   |   |   | RAPPORTO |
| userID |   |   |   |   |   | SEARCH |
| workDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**Risorse aggiornate**

Con questa versione dell’API Workfront sono state aggiornate le seguenti risorse esistenti. Le modifiche apportate a una risorsa sono indicate come segue:

* Le aggiunte sono semplicemente elencate
* Le rimozione sono indicate con testo barrato
* Le modifiche sono elencate nella nota dopo la tabella

### Approval

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproved `¹`   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |
| projectBudgetedCost  |   |   |   |   |   |   |
| projectNetValue  |   |   |   |   |   |   |
| projectRoi  |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

`¹ Type changed from null to boolean`

### Assegnazione

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| assegnazionePercentuale `¹` |   |   |   |   |   |   |
| viewedByAssignedToUser |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

`¹`aggiunta convalida LESS_THAN_EQUAL

### A budget

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### CustomerPreferences

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| name `¹` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche a possibiliValues

### DocMetadataLinkGroup

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style=&quot;table-layout:auto&quot;}

### Documento

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### DocumentRequest

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

DocumentVersion

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| externalIntegrationType ¹ |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche a possibiliValues

Spesa

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Gruppo

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style=&quot;table-layout:auto&quot;}

### LinkedFolder

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| externalIntegrationType¹ |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹ Modifiche a possibiliValues

### OpTask

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| priorityColor |  |  | pendingApproved¹ |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹ Tipo modificato da null a booleano

### PortalSection

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|  |  |  | groupIDs |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Portfolio

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| portfolioNetValue |  |  |  |  |  |  |
| portfolioRoi |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Progetto

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| projectBudgetedCost  |   |   |   | linkExternalObject  |   |   |
| projectNetValue |   |   |   | unlinkExternalObject |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Approvazione bozza

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| approverDecision |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Trfa

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| rateValue ¹ |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹ validatore aggiunto CURRENCY

### Attività

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| kanbanFlag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Team

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| hoursPerPoint ¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ validatore aggiunto LESS_THAN

### Assegnazione team

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### AttivitàTeam

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Scheda orario

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Aggiorna

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| updateType `¹` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style=&quot;table-layout:auto&quot;}

¹ modifiche a possibleValues

### Utente

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   | accessLevel  |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### NoteUtente

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| eventType ¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ modifiche a possibleValues

### Lavoro

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | in attesa di approvazione ¹  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Tipo modificato da null a booleano

## Risorse rimosse {#removed-resources}

### ResourceBudgetedHour

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| allocateDate |   |   |   |   |   | AGGIUNGI  |
| budgetedHours |   |   |   |   |   | CONTEGGIO  |
| ID |   |   |   |   |   | ELIMINA  |
| ScheduledBudgetedHours |   |   |   |   |   | MODIFICA  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | RAPPORTO  |
| userID |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

 

 

 
