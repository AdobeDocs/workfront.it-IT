---
content-type: api
navigation-topic: api-navigation-topic
title: Novità della versione 7 dell’API
description: Raccolte
author: Becky
feature: Workfront API
role: Developer
exl-id: 8c575251-677b-474d-84aa-02b637ef7760
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 47%

---

# Novità della versione 7 dell’API

## Nuovi oggetti

### Fagiolo bozza

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Ricerca |
| deadLine |   |   |   |   |   |   |
| name |   |   |   |   |   |   |

{style="table-layout:auto"}

### Collegamento DocMetadata

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Campi</th> 
   <th>Riferimenti</th> 
   <th> <p data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">Raccolte</p> <p data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">+++++++++++ </p> </th> 
   <th>Ricerca</th> 
   <th>Azioni</th> 
   <th>Query</th> 
   <th>Operazioni</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ID</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Aggiungi</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Count </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Elimina </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Ottenere  </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Rapporto </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>Ricerca </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Aggiungi |
|   |   |   |   |   |   | Count |
|   |   |   |   |   |   | Elimina |
|   |   |   |   |   |   | Ottenere |
|   |   |   |   |   |   | Rapporto |
|   |   |   |   |   |   | Ricerca |

{style="table-layout:auto"}

### ProofApproval

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Count |
|   |   |   |   |   |   | Ottenere |
|   |   |   |   |   |   | Rapporto |
|   |   |   |   |   |   | Ricerca |

{style="table-layout:auto"}

 

### ContornoRisorse

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Aggiungi |
|   |   |   |   |   |   | Count |
|   |   |   |   |   |   | Elimina |
|   |   |   |   |   |   | Modifica |
|   |   |   |   |   |   | Ottenere |
|   |   |   |   |   |   | Rapporto |
|   |   |   |   |   |   | Ricerca |

{style="table-layout:auto"}

 

### UserGroups

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| groupID | gruppo |   |   |   |   |   |
| isOwner  | utente  |   |   |   |   |   |
| userID  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### TimesheetProfile

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |  hourTypes |   |   |   | Aggiungi |
| name |   |   |   |   |   | Copia |
|   |   |   |   |   |   | Count |
|   |   |   |   |   |   | Elimina |
|   |   |   |   |   |   | Modifica |
|   |   |   |   |   |   | Ottenere |
|   |   |   |   |   |   | Rapporto |
|   |   |   |   |   |   | Ricerca |
|   |   |   |   |   |   | Sostituisci |

{style="table-layout:auto"}

 

### RsrcPool

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID | cliente | utenti |   |   |   | Aggiungi |
| customerID  | enteredBy  |   |   |   |   | Count |
| descrizione  | lastUpdatedBy  |   |   |   |   | Elimina |
| enteredByID  |   |   |   |   |   | Modifica |
| entryDate  |   |   |   |   |   | Ottenere |
| extRefID  |   |   |   |   |   | Rapporto |
| lastUpdateDate |   |   |   |   |   | Ricerca |
| lastUpdateByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### DocMetadataLinkGroup

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | Count |
| articleName  |   |   |   |   |   | Ottenere |
| pageID  |   |   |   |   |   | Rapporto |
| url  |   |   |   |   |   | Ricerca |

{style="table-layout:auto"}

 

 

 

## Oggetti aggiornati

Modifiche agli oggetti esistenti: le aggiunte sono semplicemente elencate, le rimozioni sono barrate, le modifiche a esistenti hanno una nota allegata dopo la tabella

### UpdateBean

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Modifiche ai valori possibili 

 

### ApprovalServiceObject

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate<sup>1</sup> |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |    |

{style="table-layout:auto"}

 

### AccessRule<sup>1</sup>

<sup>1</sup> Contrassegnato come segnalabile

 

### Processo di approvazione

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   | `AttachedApprovalPaths`  |   |   |   |   |

{style="table-layout:auto"}

  

### Percorso di approvazione<sup>1</sup>

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | `Add` |
|   |   |   |   |   |   | `Delete` |
|   |   |   |   |   |   | `Edit` |

{style="table-layout:auto"}

<sup>1</sup> Flag segnalabile rimosso

 

### Oggetto servizio di lavoro

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Convalida data aggiunta

<sup>2</sup> Flag Not_Filterable aggiunto

 

### Assegnazione

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|  workPerDayList |   |   |   | assignUserToRoleOnProjects<sup>1</sup> |   |   |
|   |   |   |   | swapUsersOnProjects<sup>1</sup> |   |   |
|   |   |   |   | unassignUserFromProjects<sup>1</sup> |   |   |

{style="table-layout:auto"}

<sup>1</sup> Il campo aggiunto includeIssues

 

### Cliente 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| bizRuleExclusions<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Modifiche ai valori possibili 

 

### Enum personalizzata 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| groupID  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Documento 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| checkOutTimestamp |   |   |   |  createProof |   |   |

{style="table-layout:auto"}

 

### DocumentVersion 

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   |  getProofingTokens |   |   |

{style="table-layout:auto"}

 

### Gruppo

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| isPublic |  layoutTemplate | userGroups  |   |   |   |   |
| layoutTemplateID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Convalida PRECISION modificata da 8 a 9

 

### HourType

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   |   | defaultOpTaskHourType |   |
|   |   |   |   |   | defaultProjectHourType |   |
|   |   |   |   |   | defaultTaskHourType  |   |
|   |   |   |   |   | globalHourTypes  |   |
|   |   |   |   |   | objectHourTypes  |   |

{style="table-layout:auto"}

 

### Voce del diario

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Modifiche ai valori possibili

 

### Optask (problema)

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |  assignMultiple |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

 

### Progetto

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

 

### DefCoda

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| allowedLegacyQueueTopicIDs |  |  |  | getQueueDefTree |   |   |

{style="table-layout:auto"}

 

### Argomento coda

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   |   |  queueTopicID |   |

{style="table-layout:auto"}

 

### Recente

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|   |   |   |   |  updateLastViewedObject |   |   |

{style="table-layout:auto"}

 

### Attività

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   | assignMultiple  |   |   |
| approvalStartDate |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### TemplateTask

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Tipo cambiato da Int a Double 

 

### Utente

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Campi</th> 
   <th>Riferimenti</th> 
   <th>Raccolte</th> 
   <th>Ricerca</th> 
   <th>Azioni</th> 
   <th>Query</th> 
   <th>Operazioni</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>
    <code>lastWhatsNew</code> </td> 
   <td> </td> 
   <td>
    <code>roles</code> </td> 
   <td> ruoli</td> 
   <td>addMobileDevice</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;scheduleDeactivationDate&quot;}" data-sheets-userformat="{&quot;2&quot;:8707,&quot;3&quot;:{&quot;1&quot;:0},&quot;4&quot;:{&quot;1&quot;:2,&quot;2&quot;:14277081},&quot;12&quot;:0,&quot;16&quot;:10}">scheduleDeactivationDate</span></td> 
   <td> </td> 
   <td><span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;timesheetProfileHourTypes&quot;}" data-sheets-userformat="{&quot;2&quot;:8707,&quot;3&quot;:{&quot;1&quot;:0},&quot;4&quot;:{&quot;1&quot;:2,&quot;2&quot;:14277081},&quot;12&quot;:0,&quot;16&quot;:10}">timesheetProfileHourTypes</span> </td> 
   <td> </td> 
   <td>getAvailableActions</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>hasAnyAccess</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>isUserTerminologyActive</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>removeMobileDevice</p> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>showShouldProofHQNavButton</td> 
   <td> </td> 
   <td>  </td> 
  </tr> 
 </tbody> 
</table>

### Nota utente

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
| `acknowledgedmentIDs` |   |   |   |  unackknowledgeMany |   |   |
| ackDate |   |   |   |   |   |   |
| ackType |   |   |   |   |   |   |

{style="table-layout:auto"}

 

 

### CustomerPrefObject

| Campi | Riferimenti | Raccolte | Ricerca | Azioni | Query | Operazioni |
|---|---|---|---|---|---|---|
|  name |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Modifiche ai valori possibili
