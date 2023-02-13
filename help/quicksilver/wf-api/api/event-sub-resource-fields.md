---
content-type: api
navigation-topic: api-navigation-topic
title: Campi delle risorse della sottoscrizione evento
description: Campi delle risorse della sottoscrizione evento
author: John
feature: Workfront API
exl-id: 54859930-7619-4b93-8dff-29b10e43d6d5
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 11%

---

# Campi delle risorse della sottoscrizione evento

I campi delle risorse della sottoscrizione degli eventi rappresentano i trigger per gli eventi che fanno sì che una sottoscrizione di eventi invii un messaggio in uscita a un endpoint configurato. Quando un campo di risorsa viene modificato, viene attivato un evento UPDATE.

Nella tabella seguente sono elencati i campi disponibili per le risorse di abbonamento all’evento:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Risorsa</th> 
   <th>objCode</th> 
   <th>Campo</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Assegnazione</td> 
   <td>ASSEGNARE</td> 
   <td>effectiveWorkCompleted</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>effectiveWorkPerDayStartDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> assegnazionePercentuale </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> avgWorkPerDay </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> customerID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isPrimary</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isTeamAssignment </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> opTaskID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> proiettatoAvgWorkPerDay </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectionUserAllocationPercentage </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>stato</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lavorare</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workPerDayList</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workRequired</td> 
  </tr> 
  <tr> 
   <td>Azienda</td> 
   <td>CMPY</td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enterByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td>Dashboard</td> 
   <td>PTLTAB</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrizione</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> <p>lastUpdateDate</p> <p>Nota: LastUpdateDate attiverà un evento solo la prima volta che viene aggiornato in ogni giorno. </p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td>Documento</td> 
   <td>DOCU</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentVersionID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>cliente:isAdvancedDocMgmtEnabled</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrizione</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>gruppi</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> lastUpdatedByID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> <p>referenceNumber</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>DocumentVersion</span> </td> 
   <td><span>DOCV</span> </td> 
   <td><span>activeProofStages</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>documentID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>docSize</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>entryDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>enterByID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>int.</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>externalIntegrationType</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>externalStorageID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>fileName</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>fileType</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>posizione</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofedByUserID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofDeadlineDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofName</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofOwnerID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofPages</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofProgress</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofApprovedStatusID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>version</span> </td> 
  </tr> 
  <tr> 
   <td>Spesa</td> 
   <td>EXPNS</td> 
   <td> effectiveAmount </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> effectiveUnitAmount </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> billingRecordID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> categoryID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customFormsIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrizione</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>effectiveDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enterByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>expObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>costTypeID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isBillable</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isRimborsabile </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isRimborsato </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>masterTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objectCategories</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduledAmount</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduledDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduledUnitAmount</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjectName</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topReferenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topReferenceObjID</td> 
  </tr> 
  <tr> 
   <td>Ora</td> 
   <td>HOUR</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> effectiveCost </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>authorizedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvatoOnDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>billingRecordID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrizione</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ore</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hourTypeID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>stato</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetID</td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>OPTASK</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrizione</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enterByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduledCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>priorità</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>stato</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td>Nota</td> 
   <td>NOTA</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>noteText</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>soggetto</td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>PORTA</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrizione</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enterByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td>Programma</td> 
   <td>PRGM</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrizione</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enterByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td>PROJ</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>valuta</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrizione</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enterByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduledCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>priorità</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>sponsorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>stato</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Approvazione bozza</span> </td> 
   <td><span>PRFAPL</span> </td> 
   <td><span>documentVersionID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>approverDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>approverID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>isAwaitDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofCreationDate</span> </td> 
  </tr> 
  <tr> 
   <td>Rapporto</td> 
   <td>PTLSEC</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrizione</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enterByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>uiObjCode</td> 
  </tr> 
  <tr> 
   <td>Attività</td> 
   <td>ATTIVITÀ</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrizione</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enterByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduledCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>priorità</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>stato</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td>Modello</td> 
   <td>TMPL</td> 
   <td>accessorIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>descrizione</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>priorità</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>sponsorID</td> 
  </tr> 
  <tr> 
   <td>Scheda orario</td> 
   <td>TAGLIA</td> 
   <td>approversListString</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>displayName</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>endDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hasNotes</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hoursDuration</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isEditable</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>overtimeHours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>regolarmenteHours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>startDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>stato</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetProfileID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>totalHours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td>UTENTE</td> 
   <td>accessLevelID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>homeGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>homeTeamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isActive</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastLoginDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>managerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>title</td> 
  </tr> 
 </tbody> 
</table>

&#42;Un parameterValue è un valore di campo personalizzato associato a varie risorse (o oggetti) Workfront. Un messaggio in uscita per la sottoscrizione di un evento include un elenco completo dei valori dei parametri popolati (campi personalizzati).
