---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Dizionario dei dati di Workfront Data Connect
description: Questa pagina contiene informazioni sulla struttura e sul contenuto dei dati in Workfront Data Connect.
author: Courtney
feature: Reports and Dashboards
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: cfc4bcf9d3956a50839a6da26fc98a645782bdc1
workflow-type: tm+mt
source-wordcount: '11896'
ht-degree: 7%

---

# Dizionario dei dati di Workfront Data Connect

Questa pagina contiene informazioni sulla struttura e sul contenuto dei dati in Workfront Data Connect.

>[!NOTE]
>
>I dati in Data Connect vengono aggiornati ogni 4 ore, pertanto le modifiche recenti potrebbero non essere applicate immediatamente.

## Tipi di visualizzazione

Esistono diversi tipi di visualizzazione che è possibile utilizzare in Data Connect per visualizzare i dati di Workfront in modo da fornire il maggior numero di insight.

* **Visualizzazione corrente**

  La visualizzazione Corrente riflette i dati in modo simile a come esistono in Workfront, in ogni oggetto e nel relativo stato corrente. Tuttavia, può essere navigato con una latenza molto più bassa rispetto a Workfront.

* **Visualizzazione evento**

  La visualizzazione Evento tiene traccia di ogni record di modifica in Workfront, ovvero ogni volta che un oggetto cambia stato, viene creato un record che mostra quando è avvenuta la modifica, chi ha apportato la modifica e cosa è stato modificato. Pertanto, questa visualizzazione è utile per confronti point-in-time. Questa visualizzazione include solo i record degli ultimi tre anni.

* **Visualizzazione cronologia giornaliera**

  La visualizzazione Cronologia giornaliera offre una versione abbreviata della visualizzazione Evento, in quanto mostra lo stato di ciascun oggetto su base giornaliera anziché nel momento in cui si è verificato ogni singolo evento. Di conseguenza, questa visualizzazione è utile per l’analisi delle tendenze.

<!-- Custom view -->

## Diagrammi delle relazioni di entità

Gli oggetti in Workfront (e, pertanto, nel data lake di Data Connect) sono definiti non solo dai singoli valori, ma anche dalle relazioni con altri oggetti.

I diagrammi delle relazioni tra entità (ERD) riportati di seguito forniscono una mappatura di alto livello delle relazioni tra oggetti in Data Connect per gli oggetti principali di Workfront.

>[!IMPORTANT]
>
>I diagrammi sono centrati su singoli oggetti e non rappresentano un diagramma di relazione entità completo per l&#39;intera applicazione Workfront. <br>
>Questi diagrammi forniscono esempi di come le relazioni possono essere utilizzate per unire i dati a oggetti adiacenti.

### Esempio di diagrammi di relazioni tra entità

+++ Espandere per visualizzare i diagrammi di esempio

>[!TIP]
>
>Per visualizzare un diagramma in modo più dettagliato, fare clic con il pulsante destro del mouse sull&#39;immagine e selezionare **Apri immagine in una nuova scheda**.


### Assegnazioni

![Diagramma relazioni entità assegnazioni](assets/Assignment-centered-ERD.png)


### Documenti e approvazioni di documenti

![Diagramma relazioni entità documenti e approvazione documenti](assets/Document-and-Document-Approvals-centered-ERD.png)

### Ore e schede orario

![Diagramma delle relazioni tra le entità Ore e Schede orario](assets/Hours-and-Timesheet-centered-ERD.png)


### Problemi

![Diagramma relazioni entità problemi](assets/Issue-centered-ERD.png)

### Progetti

![Diagramma relazioni entità progetti](assets/Project-centered-ERD.png)


### Attività

![Diagramma relazioni entità attività](assets/Task-centered-ERD.png)


### Utenti

![Diagramma relazioni entità utenti](assets/User-centered-ERD.png)

+++

## Tipi di date

Esistono diversi oggetti data che forniscono informazioni su quando si verificano eventi specifici.

* `DL_LOAD_TIMESTAMP`: questa data viene aggiornata dopo il completamento di un aggiornamento dei dati riuscito e include la marca temporale dell&#39;inizio del processo di aggiornamento che ha fornito la versione più recente di un record.
* `CALENDAR_DATE`: data presente solo nella visualizzazione Cronologia giornaliera. La visualizzazione Cronologia giornaliera consente di registrare l&#39;aspetto dei dati alle 11:59 UTC per ogni data specificata in `CALENDAR_DATE`.
* `BEGIN_EFFECTIVE_TIMESTAMP`: questa data è presente nelle visualizzazioni Evento e Cronologia giornaliera e rappresenta il momento in cui un record diventa il valore corrente nell&#39;applicazione.
* `END_EFFECTIVE_TIMESTAMP`: questa data è presente sia nelle visualizzazioni Evento che Cronologia giornaliera e registra esattamente quando un record ha cambiato _da_ il valore nella riga corrente a un valore in una riga diversa. Per consentire l&#39;esecuzione di query tra `BEGIN_EFFECTIVE_TIMESTAMP` e `END_EFFECTIVE_TIMESTAMP`, questo valore non è mai nullo, anche se non è presente un nuovo valore. Nel caso in cui un record sia ancora valido, ovvero il valore non sia stato modificato, `END_EFFECTIVE_TIMESTAMP` avrà il valore 2300-01-01.

## Tabella terminologica e descrizioni di Workfront

La tabella seguente mette in correlazione i nomi degli oggetti in Workfront (nonché i relativi nomi nell&#39;interfaccia e nell&#39;API) con i nomi equivalenti in Data Connect e include campi di riferimento per ogni oggetto con altri oggetti Workfront.

>[!NOTE]
>
>È possibile aggiungere nuovi campi alle visualizzazioni oggetti senza preavviso per supportare le esigenze di dati in continua evoluzione dell’applicazione Workfront. Si consiglia di non utilizzare query &quot;SELECT&quot; in cui il destinatario dei dati downstream non è preparato a gestire colonne aggiuntive durante l&#39;aggiunta.<br>
>Se è necessario rinominare o rimuovere una colonna, avviseremo in anticipo di queste modifiche.

### Livello di accesso

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Livello di accesso</td>
            <td>Livello di accesso</td>
            <td>ACSLVL</td>
            <td>Livello di accesso</td>
            <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LEGACYACCESSLEVELID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Regola di accesso

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Regola di accesso</td>
            <td>Condividi</td>
            <td>ACSRUL</td>
            <td>Condividi</td>
            <td>ACCESSRULES_CURRENT<br>ACCESSRULES_DAILY_HISTORY<br>ACCESSRULES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSORID</td>
             <td>FK</td>
             <td>Variabile basata su ACCESSOROBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo ACCESSOROBJCODE</td>
        </tr>
        <tr>
             <td>ACCESSRULEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ANCESTORID</td>
             <td>PK</td>
             <td>Variabile, basata su ANCESTOROBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo ANCESTOROBJCODE</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SECURITYOBJID</td>
             <td>FK</td>
             <td>Variabile, basata su SECURITYOBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo SECURITYOBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Percorso di approvazione

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Percorso di approvazione</td>
            <td>Percorso di approvazione</td>
            <td>ARVPTH</td>
            <td>Approvazione</td>
            <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPATHID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GLOBALPATHID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Processo di approvazione

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Processo di approvazione</td>
            <td>Processo di approvazione</td>
            <td>ARVPRC</td>
            <td>Processo di approvazione</td>
            <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Passaggio di approvazione

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Passaggio di approvazione</td>
            <td>Passaggio di approvazione</td>
            <td>ARVSTP</td>
            <td>Fase di approvazione</td>
            <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPATHID</td>
             <td>FK</td>
             <td>APPROVALPATHS_CURRENT</td>
             <td>APPROVALPATHID</td>
        </tr>
        <tr>
             <td>APPROVALSTEPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Stato approvatore

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Stato approvatore</td>
            <td>Stato approvatore</td>
            <td>ARVSTS</td>
            <td>ApproverStatus</td>
            <td>APPROVERSTATUSES_CURRENT<br>APPROVERSTATUSES_DAILY_HISTORY<br>APPROVERSTATUSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERSTATUSID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>APPROVABILE</td>
             <td>FK</td>
             <td>Variabile basata su APPROVABLEOBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo APPROVABLEOBJCODE</td>
        </tr>
        <tr>
             <td>APPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>APPROVEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DELEGATEUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OVERRIDDENUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>STEPAPPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSYID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>CARATTERE JOLLY</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Assegnazione

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Assegnazione</td>
            <td>Assegnazione</td>
            <td>ASSGN</td>
            <td>Assegnazione</td>
            <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFICATORE_CORRENTE</td>
             <td>CLASSIFIERID</td>
        </tr>
      <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEAM ID</td>
             <td>FK</td>
             <td>TEAM_CURRENT</td>
             <td>TEAM ID</td>
        </tr>
    </tbody>
</table>

### In attesa di approvazioni

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>In attesa di approvazioni</td>
            <td>In attesa di approvazioni</td>
            <td>AWAPVL</td>
            <td>In attesa di approvazioni</td>
            <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSREQUESTID</td>
             <td>-</td>
             <td colspan="2">Tabella di richiesta di accesso non supportata al momento</td>
        </tr>
        <tr>
             <td>APPROVABILE</td>
             <td>FK</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>APPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>IN ATTESA DI APPROVAZIONE</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTVERSIONID</td>
             <td>FK</td>
             <td>DOCUMENTVERSIONS_CURRENT</td>
             <td>DOCUMENTVERSIONID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEAM ID</td>
             <td>FK</td>
             <td>TEAM_CURRENT</td>
             <td>TEAM ID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Linea di base

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Linea di base</td>
            <td>Linea di base</td>
            <td>CIECO</td>
            <td>Linea di base</td>
            <td>BASELINES_CURRENT<br>BASELINES_DAILY_HISTORY<br>BASELINES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BASELINEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Attività linea di base

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Attività linea di base</td>
            <td>Attività linea di base</td>
            <td>BSTSK</td>
            <td>Attività linea di base</td>
            <td>BASELINETASKS_CURRENT<br>BASELINETASKS_DAILY_HISTORY<br>BASELINETASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BASELINEID</td>
             <td>FK</td>
             <td>BASELINES_CURRENT</td>
             <td>BASELINEID</td>
        </tr>
        <tr>
             <td>BASELINETASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
    </tbody>
</table>

### Tariffa di fatturazione

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tariffa di fatturazione</td>
            <td>Tasso o tasso di sostituzione</td>
            <td>TARIFFA</td>
            <td>Tariffa di fatturazione</td>
            <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFICATORE_CORRENTE</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>FK</td>
             <td>NONLABORRESOURCES_CURRENT</td>
             <td>NONLABORRESOURCEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>RATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SOURCERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Record della fatturazione

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Record della fatturazione</td>
            <td>Record della fatturazione</td>
            <td>FATTURA</td>
            <td>Record della fatturazione</td>
            <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>INVOICEID</td>
             <td>-</td>
             <td colspan="2">Tabella fatture attualmente non supportata</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Prenotazione

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Prenotazione</td>
            <td>Prenotazione</td>
            <td>PRENOTAZIONE</td>
            <td>Prenotazione</td>
            <td>BOOKINGS_CURRENT<br>BOOKINGS_DAILY_HISTORY<br>BOOKINGS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BOOKINGID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>FK</td>
             <td>NONLABORRESOURCES_CURRENT</td>
             <td>NONLABORRESOURCEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATFORM</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATFORM</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variabile, basata su TOPOBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo TOPOBJCODE</td>
        </tr>
    </tbody>
</table>

### Profilo aziendale

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Profilo aziendale</td>
            <td>Profilo aziendale</td>
            <td>BSNPRF</td>
            <td>ProfiloBusiness</td>
            <td>BUSINESSPROFILE_CURRENT<br>BUSINESSPROFILE_DAILY_HISTORY<br>BUSINESSPROFILE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>FK</td>
             <td>ACCESSLEVELS_CURRENT</td>
             <td>ACCESSLEVELID</td>
        </tr>
        <tr>
             <td>BUSINESSPROFILEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Regola di business

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Regola di business</td>
            <td>Regola di business</td>
            <td>BSNRUL</td>
            <td>Regola di business</td>
            <td>BUSINESSRULE_CURRENT<br>BUSINESSRULE_DAILY_HISTORY<br>BUSINESSRULE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BUSINESSRULEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Categoria

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Categoria</td>
            <td>Modulo personalizzato</td>
            <td>CITTÀ</td>
            <td>Categoria</td>
            <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Parametro di Categoria

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Parametro di Categoria</td>
            <td>Campi modulo personalizzati</td>
            <td>CTGYPA</td>
            <td>Parametro di Categoria</td>
            <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORIESPARAMETERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>PARAMETERGROUPID</td>
             <td>FK</td>
             <td>PARAMETERGROUPS_CURRENT</td>
             <td>PARAMETERGROUPID</td>
        </tr>
        <tr>
             <td>PARAMETERID</td>
             <td>FK</td>
             <td>PARAMETERS_CURRENT</td>
             <td>PARAMETERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Classificatore

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Classificatore</td>
            <td>Posizione</td>
            <td>CLSF</td>
            <td>Posizione</td>
            <td>CLASSIFICATORE_CORRENTE<br>CLASSIFICATORE_CRONOLOGIA_GIORNALIERA<br>CLASSIFICATORE_EVENTO</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CLASSIFIERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>CLASSIFICATORE_CORRENTE</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Azienda

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Azienda</td>
            <td>Azienda</td>
            <td>CMPY</td>
            <td>Azienda</td>
            <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Trimestre personalizzato

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Trimestre personalizzato</td>
            <td>Trimestre personalizzato</td>
            <td>CSTQR</td>
            <td>Trimestre personalizzato</td>
            <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CUSTOMQUARTERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Enum personalizzata

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>EnumPersonalizzata</td>
            <td>Condizione, Priorità, Gravità, Stato</td>
            <td>CSTEM</td>
            <td>Enum personalizzata</td>
            <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CUSTOMENUMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

>[!NOTE]
>
>Tipo di record identificato tramite la proprietà `enumClass`. I tipi previsti sono:<br>
><ul><li>CONDITION_OPTASK</li>
>&gt;<li>CONDITION_PROJ</li>
>&gt;<li>CONDITION_TASK</li>
>&gt;<li>PRIORITY_OPTASK</li>
>&gt;<li>PRIORITY_PROJ</li>
>&gt;<li>TASK_PRIORITARIO</li>
>&gt;<li>GRAVITY_OPTASK</li>
>&gt;<li>STATUS_OPTASK</li>
>&gt;<li>STATUS_PROJ</li>
>&gt;<li>TASK_STATO</li></ul>


### Documento

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Documento</td>
            <td>Documento</td>
            <td>DOCU</td>
            <td>Documento</td>
            <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CHECKEDOUTBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTREQUESTID</td>
             <td>-</td>
             <td colspan="2">Tabella di richiesta documento non supportata al momento</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIO_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMI_CORRENTI</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RELEASEVERSIONID</td>
             <td>-</td>
             <td colspan="2">Tabella delle versioni di rilascio attualmente non supportata</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATFORM</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATFORM</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variabile, basata su TOPOBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo TOPOBJCODE</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Approvazione documento

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Approvazione documento</td>
            <td>Approvazione documento</td>
            <td>DOCAPL</td>
            <td>Approvazione documento</td>
            <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DOCAPPROVALID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>REQUESTORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Approvazione documento (NUOVO)

Disponibilità limitata dei clienti

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Approvazione documento</td>
            <td>Approvazione</td>
            <td>N/D</td>
            <td>N/D</td>
            <td>APPROVAL_CURRENT<br>APPROVAL_DAILY_HISTORY<br>APPROVAL_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">APPROVABILE</td>
             <td>PK</td>
             <td>-</td>
             <td>NOTA: questo è anche l'ID dell'oggetto DOCUMENTVERSION a cui è associata l'approvazione.</td>
        </tr>
        <tr>
             <td class="key">ASSETID</td>
             <td>FK</td>
             <td>Variabile, basata su ASSETTYPE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo ASSETTYPE</td>
        </tr>
        <tr>
             <td class="key">CREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">EAUTHTENANTID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td class="key">PRODUCTID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td class="key">REALCREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Fase di approvazione documento (NUOVO)

Disponibilità limitata dei clienti

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Fase di approvazione documento</td>
            <td>Fase di approvazione</td>
            <td>N/D</td>
            <td>N/D</td>
            <td>APPROVAL_STAGE_CURRENT<br>APPROVAL_STAGE_DAILY_HISTORY<br>APPROVAL_STAGE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">APPROVABILE</td>
             <td>FK</td>
             <td>APPROVAZIONE_CORRENTE</td>
             <td>APPROVABILE</td>
        </tr>
        <tr>
             <td class="key">APPROVALSTAGEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td class="key">CREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">OBJID</td>
             <td class="type">FK</td>
             <td class="relatedtable">Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
    </tbody>
</table>

### Partecipanti fase approvazione documento (NUOVO)

Disponibilità limitata dei clienti

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Partecipante alla fase di approvazione documento</td>
            <td>Decisioni di approvazione</td>
            <td>N/D</td>
            <td>N/D</td>
            <td>APPROVAL_STAGE_PARTICIPANT_CURRENT<br>APPROVAL_STAGE_PARTICIPANT_DAILY_HISTORY<br>APPROVAL_STAGE_PARTICIPANT_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">APPROVABILE</td>
             <td>FK</td>
             <td>APPROVAZIONE_CORRENTE</td>
             <td>APPROVABILE</td>
        </tr>
        <tr>
             <td class="key">APPROVALSTAGEPARTICIPANTID/td&gt;
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td class="key">ASSETID</td>
             <td>FK</td>
             <td>Variabile, basata su ASSETTYPE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo ASSETTYPE</td>
        </tr>
        <tr>
             <td class="key">DECISIONUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">OBJID</td>
             <td class="type">FK</td>
             <td class="relatedtable">Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td class="key">PARTICIPANTID</td>
             <td>FK</td>
             <td class="relatedtable">Variabile, basata su PARTICIPANTTYPE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo PARTICIPANTTYPE</td>
        </tr>
        <tr>
             <td class="key">REALREQUESTORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">REALUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">REQUESTORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">STAGEID</td>
             <td>FK</td>
             <td>APPROVAL_STAGE_CURRENT</td>
             <td>STAGEID</td>
        </tr>
    </tbody>
</table>

### Cartella documenti

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Cartella documenti</td>
            <td>Cartella documenti</td>
            <td>DOCFLD</td>
            <td>DocsFolders</td>
            <td>DOCFOLDERS_CURRENT<br>DOCFOLDERS_DAILY_HISTORY<br>DOCFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ID ISSUE</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>LINKEDFOLDERID</td>
             <td>FK</td>
             <td>LINKEDFOLDERS_CURRENT</td>
             <td>LINKEDFOLDERID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>DOCFOLDERS_CURRENT</td>
             <td>DOCFOLDERID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIO_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMI_CORRENTI</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATFORM</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATFORM</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Metadati provider documenti

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Metadati provider documenti</td>
            <td>Metadati provider documenti</td>
            <td>DOCMET</td>
            <td>DocumentProviderMetadata</td>
            <td>DOCPROVIDERMETA_CURRENT<br>DOCPROVIDERMETA_DAILY_HISTORY<br>DOCPROVIDERMETA_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERMETAID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Provider documento

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Provider documento</td>
            <td>Provider documento</td>
            <td>DOCPRO</td>
            <td>Provider documento</td>
            <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERCONFIGID</td>
             <td>FK</td>
             <td>DOCPROVIDERCONFIG_CURRENT</td>
             <td>DOCPROVIDERCONFIGID</td>
        </tr>
        <tr>
             <td>DOCPROVIDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Configurazione provider documenti

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Configurazione provider documenti</td>
            <td>Configurazione provider documenti</td>
            <td>DOCCFG</td>
            <td>DocumentProviderConfig</td>
            <td>DOCPROVIDERCONFIG_CURRENT<br>DOCPROVIDERCONFIG_DAILY_HISTORY<br>DOCPROVIDERCONFIG_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERCONFIGID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Versione documento

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Versione documento</td>
            <td>Versione documento</td>
            <td>DOCV</td>
            <td>Versione documento</td>
            <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTPROVIDERID</td>
             <td>FK</td>
             <td>DOCPROVIDERS_CURRENT</td>
             <td>DOCUMENTPROVIDERID</td>
        </tr>
        <tr>
             <td>DOCUMENTVERSIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXTERNALSTORAGEID</td>
             <td>-</td>
             <td colspan="2">ID esterno nel sistema di storage esterno</td>
        </tr>
        <tr>
             <td>PROOFAPPROVALSTATUSID</td>
             <td>-</td>
             <td colspan="2">Tabella dello stato di approvazione della bozza non supportata al momento</td>
        </tr>
        <tr>
             <td>PROOFEDBYUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROOFID</td>
             <td>-</td>
             <td colspan="2">Tabella bozza non supportata al momento</td>
        </tr>
        <tr>
             <td>PROOFOWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROOFSTAGEID</td>
             <td>FK</td>
             <td>-</td>
             <td colspan="2">Tabella fase bozza non supportata al momento</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Tasso di cambio

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tasso di cambio</td>
            <td>Tasso di cambio</td>
            <td>ESAURIRE</td>
            <td>Tasso di cambio</td>
            <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Spesa

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Spesa</td>
            <td>Spesa</td>
            <td>EXPNS</td>
            <td>Spesa</td>
            <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>SPESA ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXPENSETYPEID</td>
             <td>FK</td>
             <td>EXPENSETYPES_CURRENT</td>
             <td>EXPENSETYPEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATFORM</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATFORM</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variabile, basata su TOPBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo TOPBJCODE</td>
        </tr>
    </tbody>
</table>

### Tipo di spesa

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tipo di spesa</td>
            <td>Tipo di spesa</td>
            <td>EXPTYP</td>
            <td>Tipo di spesa</td>
            <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>EXPENSETYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Gruppo

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gruppo</td>
            <td>Gruppo</td>
            <td>GRUPPO</td>
            <td>Gruppo</td>
            <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ID AZIENDA</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>ROOTID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Ora

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Ora</td>
            <td>Ora</td>
            <td>HOUR</td>
            <td>Ora</td>
            <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFICATORE_CORRENTE</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>DUPIDO</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>EXTERNALTIMESHEETID</td>
             <td>-</td>
             <td colspan="2">Relazione non Workfront; utilizzato per l'integrazione con sistemi esterni
Autonomo</td>
        </tr>
        <tr>
             <td>HOURID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>HOURTYPEID</td>
             <td>FK</td>
             <td>HOURTYPES_CURRENT</td>
             <td>HOURTYPEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTOVERHEADID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
    </tbody>
</table>

### Tipo di ora

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tipo di ora</td>
            <td>Tipo di ora</td>
            <td>ORA</td>
            <td>Tipo di ora</td>
            <td>HOURTYPES_CURRENT<br>HOURTYPES_DAILY_HISTORY<br>HOURTYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>HOURTYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Iterazione

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Iterazione</td>
            <td>Iterazione</td>
            <td>ITRN</td>
            <td>Iterazione</td>
            <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TEAM ID</td>
             <td>FK</td>
             <td>TEAM_CURRENT</td>
             <td>TEAM ID</td>
        </tr>
    </tbody>
</table>

### Voce diario

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Voce diario</td>
            <td>Voce diario</td>
            <td>GERGO</td>
            <td>Voce diario</td>
            <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERSTATUSID</td>
             <td>FK</td>
             <td>APPROVERSTATUSES_CURRENT</td>
             <td>APPROVERSTATUSID</td>
        </tr>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>AUDITRECORDID</td>
             <td>-</td>
             <td colspan="2">Tabella record di controllo non supportata al momento</td>
        </tr>
        <tr>
             <td>BASELINEID</td>
             <td>FK</td>
             <td>BASELINES_CURRENT</td>
             <td>BASELINEID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTSHAREID</td>
             <td>-</td>
             <td colspan="2">Tabella Condivisione documento non supportata al momento</td>
        </tr>
        <tr>
             <td>EDITEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SPESA ID</td>
             <td>FK</td>
             <td>EXPENSES_CURRENT</td>
             <td>SPESA ID</td>
        </tr>
        <tr>
             <td>HOURID</td>
             <td>FK</td>
             <td>HOURS_CURRENT</td>
             <td>HOURID</td>
        </tr>
        <tr>
             <td>INITIATIVEID</td>
             <td>-</td>
             <td colspan="2">Tabella di iniziativa non supportata al momento</td>
        </tr>
        <tr>
             <td>JOURNALENTRIESID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIO_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMI_CORRENTI</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SUBOBJID</td>
             <td>FK</td>
             <td>Variabile, basata su SUBOBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo SUBOBJCODE</td>
        </tr>
        <tr>
             <td>SUBSCRIBEID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variabile, basata su TOPOBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo TOPOBJCODE</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Cartella collegata

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Cartella collegata</td>
            <td>Cartella collegata</td>
            <td>LNKFDR</td>
            <td>LinkedFolder</td>
            <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCUMENTPROVIDERID</td>
             <td>FK</td>
             <td>DOCPROVIDERS_CURRENT</td>
             <td>DOCUMENTPROVIDERID</td>
        </tr>
        <tr>
             <td>EXTERNALSTORAGEID</td>
             <td>-</td>
             <td colspan="2">ID esterno nel sistema di storage esterno</td>
        </tr>
        <tr>
             <td>FOLDERID</td>
             <td>FK</td>
             <td>DOCFOLDERS_CURRENT</td>
             <td>FOLDERID</td>
        </tr>
        <tr>
             <td>LINKEDBY</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LINKEDFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Milestone

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Milestone</td>
            <td>Milestone</td>
            <td>MIGLIA</td>
            <td>Milestone</td>
            <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>MILESTONEPATHID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATHID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Percorso milestone

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Percorso milestone</td>
            <td>Percorso milestone</td>
            <td>MPATH</td>
            <td>Percorso milestone</td>
            <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATHID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Risorsa non di manodopera

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Risorsa non di manodopera</td>
            <td>Risorsa non di manodopera</td>
            <td>NLBR</td>
            <td>Risorsa non di manodopera</td>
            <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCECATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Categoria risorsa non manodopera

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Categoria risorsa non manodopera</td>
            <td>Categoria risorsa non manodopera</td>
            <td>NLBRCY</td>
            <td>Categoria risorse non di manodopera</td>
            <td>NLBRCATEGORIES_CURRENT<br>NLBRCATEGORIES_DAILY_HISTORY<br>NLBRCATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Giorno non feriale

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Giorno non feriale</td>
            <td>Eccezione Schedule</td>
            <td>NON WKD</td>
            <td>Giorno non feriale</td>
            <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>NONWORKDAYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Nota

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Nota</td>
            <td>Nota</td>
            <td>NOTA</td>
            <td>Nota</td>
            <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ATTACHDOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>ATTACHOBJID</td>
             <td>FK</td>
             <td>Variabile basata su ATTACHOBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato in OBJCODE ATTACHOBJCODE</td>
        </tr>
        <tr>
             <td>ATTACHOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>ATTACHWORKID</td>
             <td>FK</td>
             <td>WORKITEMS_CURRENT</td>
             <td>WORKITEMID</td>
        </tr>
        <tr>
             <td>ATTACHWORKUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>AUDITRECORDID</td>
             <td>-</td>
             <td colspan="2">Tabella record di controllo non supportata al momento</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>EXTERNALSERVICEID</td>
             <td>-</td>
             <td colspan="2">Relazione non Workfront; utilizzato per l'integrazione con sistemi esterni</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile basata su NOTEOBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo NOTEOBJCODE</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARENTENDORSEMENTID</td>
             <td>-</td>
             <td colspan="2">Tabella di valutazione positiva attualmente non supportata</td>
        </tr>
        <tr>
             <td>PARENTJOURNALENTRYID</td>
             <td>FK</td>
             <td>JOURNALENTRIES_CURRENT</td>
             <td>JOURNALENTRYID</td>
        </tr>
        <tr>
             <td>PARENTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIO_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMI_CORRENTI</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROOFACTIONID</td>
             <td>-</td>
             <td colspan="2">Tabella azione bozza non supportata al momento</td>
        </tr>
        <tr>
             <td>PROOFID</td>
             <td>-</td>
             <td colspan="2">Tabella bozza non supportata al momento</td>
        </tr>
        <tr>
             <td>RICHTEXTNOTEID</td>
             <td>FK</td>
             <td>RESERVEDTEXTNOTES_CURRENT</td>
             <td>RICHTEXTNOTEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATFORM</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATFORM</td>
        </tr>
        <tr>
             <td>THREADID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>Variabile, basata su TOPOBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo TOPOBJCODE</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>


</table>

### Integrazione degli oggetti

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Integrazione degli oggetti</td>
            <td>Integrazione degli oggetti</td>
            <td>OGGETTO</td>
            <td>IntegrazioneOggetti</td>
            <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LINKEDOBJECTID</td>
             <td>FK</td>
             <td>Variabile basata su LINKEDOBJECTCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo LINKEDOBJECTCODE</td>
        </tr>
        <tr>
             <td>OBJECTINTEGRATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>

</table>

### Categoria oggetti

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Categoria oggetti</td>
            <td>Categorie di oggetti</td>
            <td>OBJCAT</td>
            <td>Categoria oggetto</td>
            <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>OBJECTSCATEGORYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Attività/problema operativo

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>OpTask</td>
            <td>Problema, richiesta</td>
            <td>OPTASK</td>
            <td>Problema</td>
            <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>KANBANBOARDID</td>
             <td>-</td>
             <td colspan="2">Tabella Kanban Board non supportata al momento</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">Tabella di definizione della coda attualmente non supportata</td>
        </tr>
        <tr>
             <td>QUEUETOPICID</td>
             <td>-</td>
             <td colspan="2">Tabella Argomento coda non supportata al momento</td>
        </tr>
        <tr>
             <td>RESOLVEOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESOLVEPROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RESOLVETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>RESOLVINGOBJID</td>
             <td>FK</td>
             <td>Variabile, basata su RESOLVINGOBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo RESOLVINGOBJCODE</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SOURCEOBJID</td>
             <td>FK</td>
             <td>Variabile basata su SOURCEOBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo SOURCEOBJCODE</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TEAM ID</td>
             <td>FK</td>
             <td>TEAM_CURRENT</td>
             <td>TEAM ID</td>
        </tr>
    </tbody>
</table>

### Parametro

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Parametro</td>
            <td>Campo personalizzato</td>
            <td>PARAM</td>
            <td>Parametro</td>
            <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY<br>PARAMETERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARAMETERFILTERID</td>
             <td>-</td>
             <td colspan="2">Tabella Filtro parametri non supportata al momento</td>
        </tr>
        <tr>
             <td>PARAMETERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Gruppo di parametri

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gruppo di parametri</td>
            <td>Sezione modulo</td>
            <td>PARAM</td>
            <td>Gruppo di parametri</td>
            <td>PARAMETERGROUPS_CURRENT<br>PARAMETERGROUPS_DAILY_HISTORY<br>PARAMETERGROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARAMETERGROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Opzione Parametro

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Opzione Parametro</td>
            <td>Opzione Parametro</td>
            <td>POPT</td>
            <td>Opzione Parametro</td>
            <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PARAMETERID</td>
             <td>FK</td>
             <td>PARAMETERS_CURRENT</td>
             <td>PARAMETERID</td>
        </tr>
        <tr>
             <td>PARAMETEROPTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Sezione portale/Report

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Sezione portale</td>
            <td>Rapporto</td>
            <td>PTLSEC</td>
            <td>Rapporto</td>
            <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>FILTERID</td>
             <td>FK</td>
             <td>UIFILTERS_CURRENT</td>
             <td>FILTERID</td>
        </tr>
        <tr>
             <td>GROUPBYID</td>
             <td>FK</td>
             <td>UIGROUPBYS_CURRENT</td>
             <td>GROUPBYID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTVIEWEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>PORTALSECTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>PUBLICRUNASUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>REPORTFOLDERID</td>
             <td>FK</td>
             <td>REPORTFOLDERS_CURRENT</td>
             <td>REPORTFOLDERID</td>
        </tr>
        <tr>
             <td>RUNASUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SCHEDULEDREPORTID</td>
             <td>-</td>
             <td colspan="2">La tabella dei rapporti pianificati non è al momento supportata</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>VIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>VIEWID</td>
        </tr>
    </tbody>
</table>

### Scheda portale/dashboard

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Scheda Portale</td>
            <td>Dashboard</td>
            <td>PTLTAB</td>
            <td>Dashboard</td>
            <td>PORTALTABS_CURRENT<br>PORTALTABS_DAILY_HISTORY<br>PORTALTABS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTALPROFILEID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>PORTALTABID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### La Sezione della Liguetta Portale

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>La Sezione della Liguetta Portale</td>
            <td>Sezione Cruscotto</td>
            <td>PRTBSC</td>
            <td>La Sezione della Liguetta Portale</td>
            <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CALENDARPORTALSECTIONID</td>
             <td>-</td>
             <td colspan="2">Sezione portale calendari non supportata al momento</td>
        </tr>
        <tr>
             <td>EXTERNALSECTIONID</td>
             <td>-</td>
             <td colspan="2">Tabella delle sezioni esterne non supportata al momento</td>
        </tr>
        <tr>
             <td>INTERNALSECTIONID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>PORTALSECTIONID</td>
        </tr>
        <tr>
             <td>PORTALSECTIONOBJID</td>
             <td>FK</td>
             <td>Variabile basata su PORTALSECTIONOBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo PORTALSECTIONOBJCODE</td>
        </tr>
        <tr>
             <td>PORTALTABID</td>
             <td>FK</td>
             <td>PORTALTABS_CURRENT</td>
             <td>PORTALTABID</td>
        </tr>
        <tr>
             <td>PORTALTABSECTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Ultimo visualizzatore sezione portale

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>PortalSectionLastViewer</td>
            <td>Ultimi visualizzatori report</td>
            <td>PLSLSV</td>
            <td>PortalSectionLastViewer</td>
            <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>REPORTID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>REPORTID</td>
        </tr>
        <tr>
             <td>REPORTLASTVIEWERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>VIEWERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Portfolio

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Portfolio</td>
            <td>Portfolio</td>
            <td>PORT</td>
            <td>Portfolio</td>
            <td>PORTFOLIOS_CURRENT<br>PORTFOLIOS_DAILY_HISTORY<br>PORTFOLIOS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ALIGNMENTSCORECARDID</td>
             <td>-</td>
             <td colspan="2">Tabella di scorecard non supportata al momento</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Preferenza

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Preferenza</td>
            <td>Visualizzazione, filtro, raggruppamento, definizione report</td>
            <td>PROSET</td>
            <td>Preferenza</td>
            <td>PREFERENCES_CURRENT<br>PREFERENCES_DAILY_HISTORY<br>PREFERENCES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Programma

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Programma</td>
            <td>Programma</td>
            <td>PRGM</td>
            <td>Programma</td>
            <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIO_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Progetto

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Progetto</td>
            <td>Progetto</td>
            <td>PROJ</td>
            <td>Progetto</td>
            <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>AEMNATIVEFOLDERTREESREFID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>ALIGNMENTSCORECARDID</td>
             <td>-</td>
             <td colspan="2">Tabella di scorecard non supportata al momento</td>
        </tr>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ATTACHEDRATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKORIGINATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>DELIVERABLESCORECARDID</td>
             <td>-</td>
             <td colspan="2">Tabella di scorecard non supportata al momento</td>
        </tr>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATHID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATHID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>POPACCOUNTID</td>
             <td>-</td>
             <td colspan="2">Tabella Account POP non supportata al momento</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIO_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMI_CORRENTI</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">Tabella di definizione della coda attualmente non supportata</td>
        </tr>
        <tr>
             <td>REJECTIONISSUEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>FK</td>
             <td>RESOURCEPOOLS_CURRENT</td>
             <td>RESOURCEPOOLID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SPONSORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TEAM ID</td>
             <td>FK</td>
             <td>TEAM_CURRENT</td>
             <td>TEAM ID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Utente team progetto

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Utente team progetto</td>
            <td>Utente team progetto</td>
            <td>PRTU</td>
            <td>Utente progetto</td>
            <td>PROJECTSUSERS_CURRENT<br>PROJECTSUSERS_DAILY_HISTORY<br>PROJECTSUSERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTSUSERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TMPUSERID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Ruolo utente team progetto

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Ruolo utente team progetto</td>
            <td>Ruolo utente team progetto</td>
            <td>PTEAM</td>
            <td>RuoloUtenteProgetto</td>
            <td>PROJECTSUSERSROLES_CURRENT<br>PROJECTSUSERSROLES_DAILY_HISTORY<br>PROJECTSUSERSROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTSUSERSROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Scheda tariffa

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Scheda tariffa</td>
            <td>Scheda tariffa</td>
            <td>RTCRD</td>
            <td>Scheda tariffa</td>
            <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>RATECARDID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SECURITYROOTID</td>
             <td>FK</td>
             <td>Variabile, basata su SECURITYOBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo SECURITYOBJCODE</td>
        </tr>
        <tr>
             <td>SOURCEID</td>
             <td>FK</td>
             <td>Variabile basata su SOURCEOBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo SOURCEOBJCODE</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>

</table>

### Cartella Report

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Cartella Report</td>
            <td>Cartella Report</td>
            <td>RPTFDR</td>
            <td>Cartella Report</td>
            <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>REPORTFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Conteggio delle statistiche della vista rapporto

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Conteggio delle statistiche della vista rapporto</td>
            <td>Conteggio delle statistiche della vista rapporto</td>
            <td>PLSVST</td>
            <td>PortalSectionStatisticInfo</td>
            <td>REPORTVIEWSTATISTICCOUNTS_CURRENT<br>REPORTVIEWSTATISTICCOUNTS_DAILY_HISTORY<br>REPORTVIEWSTATISTICCOUNTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>REPORTID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>PORTALSECTIONID</td>
        </tr>
        <tr>
             <td>REPORTVIEWSTATISTICCOUNTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Ore preventivate da segnalare

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Ore preventivate da segnalare</td>
            <td>Ore preventivate da segnalare</td>
            <td>RPBGHR</td>
            <td>Ore preventivate</td>
            <td>REPORTABLEBUDGETEDHOURS_CURRENT<br>REPORTABLEBUDGETEDHOURS_DAILY_HISTORY<br>REPORTABLEBUDGETEDHOURS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>REPORTABLEBUDGETEDHOURID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Tempo riservato/PTO

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tempo riservato</td>
            <td>Indisponibilità (personale)</td>
            <td>RESVT</td>
            <td>Indisponibilità</td>
            <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RESERVEDTIMEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Responsabile risorse

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Responsabile risorse</td>
            <td>Responsabile risorse</td>
            <td>RESMGR</td>
            <td>Responsabile risorse</td>
            <td>RESOURCEMANAGERS_CURRENT<br>RESOURCEMANAGERS_DAILY_HISTORY<br>RESOURCEMANAGERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RESOURCEMANAGERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Gruppo di risorse

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gruppo di risorse</td>
            <td>Gruppo di risorse</td>
            <td>RSPL</td>
            <td>Gruppo di risorse</td>
            <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Nota Rich Text

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Nota Rich Text</td>
            <td>Nota Rich Text</td>
            <td>RHNOTE</td>
            <td>Nota Rich Text</td>
            <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RICHTEXTNOTEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Valore parametro Rich Text

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Valore parametro Rich Text</td>
            <td>Valore parametro Rich Text</td>
            <td>RCHVAL</td>
            <td>RichTextParameterValue</td>
            <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PARAMETERVALUEID</td>
             <td>-</td>
             <td colspan="2">Tabella dei valori dei parametri non supportata al momento</td>
        </tr>
        <tr>
             <td>RICHTEXTPARAMETERVALUEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Rischio

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Rischio</td>
            <td>Rischio</td>
            <td>RISCHIO</td>
            <td>Rischio</td>
            <td>RISKS_CURRENT<br>RISKS_DAILY_HISTORY<br>RISKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RISKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>RISKTYPEID</td>
             <td>FK</td>
             <td>RISKTYPES_CURRENT</td>
             <td>RISKTYPEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Tipo di rischio

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Tipo di rischio</td>
            <td>Tipo di rischio</td>
            <td>RSKTYP</td>
            <td>Tipo di rischio</td>
            <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RISKTYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Ruolo

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Ruolo</td>
            <td>Mansione</td>
            <td>RUOLO</td>
            <td>Mansione</td>
            <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">La tabella del modello di layout non sarà supportata</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### Pianificazione

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Pianificazione</td>
            <td>Pianificazione</td>
            <td>SCHED</td>
            <td>Pianificazione</td>
            <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Piano per gestione del personale

Disponibilità limitata dei clienti

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Piano per gestione del personale</td>
            <td>Piano per gestione del personale</td>
            <td>STAFFP</td>
            <td>Piano per gestione del personale</td>
            <td>STAFFING_PLAN_CURRENT<br>STAFFING_PLAN_DAILY_HISTORY<br>STAFFING_PLAN_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ATTACHEDRATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT </td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>        
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>        
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>        
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>       
         <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID
</td>
        </tr>        
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID
</td>
        </tr>        
        <tr>
             <td>STAFFINGPLANID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Risorse del piano per gestione del personale

Disponibilità limitata dei clienti

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Risorse del piano per gestione del personale</td>
            <td>Risorse del piano per gestione del personale</td>
            <td>STAFFR</td>
            <td>Risorse del piano per gestione del personale</td>
            <td>STAFFING_PLAN_RESOURCE_CURRENT<br>STAFFING_PLAN_RESOURCE_DAILY_HISTORY<br>STAFFING_PLAN_RESOURCE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>        
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>        
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>        
        <tr>
             <td>STAFFINGPLANID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>       
         <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>        
    </tbody>
</table>

### Approvatore passaggio

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Approvatore passaggio</td>
            <td>Approvatore passaggio</td>
            <td>SPAPVR</td>
            <td>Approvatore fase</td>
            <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>STEPAPPROVERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TEAM ID</td>
             <td>FK</td>
             <td>TEAM_CURRENT</td>
             <td>TEAM ID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Attività

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Attività</td>
            <td>Attività</td>
            <td>ATTIVITÀ</td>
            <td>Attività</td>
            <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKORIGINATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>KANBANBOARDID</td>
             <td>-</td>
             <td colspan="2">Tabella Kanban Board non supportata al momento</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>FK</td>
             <td>MILESTONES_CURRENT</td>
             <td>MILESTONEID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RECURRENCERULEID</td>
             <td>-</td>
             <td colspan="2">Tabella delle regole di ricorrenza non supportata al momento</td>
        </tr>
        <tr>
             <td>REJECTIONISSUEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESERVEDTIMEID</td>
             <td>FK</td>
             <td>RESERVEDTIMES_CURRENT</td>
             <td>RESERVEDTIMEID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>SUBMITTEDBYID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>TEAM ID</td>
             <td>FK</td>
             <td>TEAM_CURRENT</td>
             <td>TEAM ID</td>
        </tr>
        <tr>
             <td>TEMPLATFORM</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATFORM</td>
        </tr>
    </tbody>
</table>

### Predecessore attività

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Predecessore attività</td>
            <td>Predecessore</td>
            <td>PRED</td>
            <td>Predecessore</td>
            <td>PREDECESSORS_CURRENT<br>PREDECESSORS_DAILY_HISTORY<br>PREDECESSORS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PREDECESSORID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SUCCESSORID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Team

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Team</td>
            <td>Team</td>
            <td>TEAMOB</td>
            <td>Team</td>
            <td>TEAM_CURRENT<br>TEAM_DAILY_HISTORY<br>TEAM_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">La tabella del modello di layout non sarà supportata</td>
        </tr>
        <tr>
             <td>MYWORKVIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>UIVIEWID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>REQUESTSVIEWID</td>
             <td>FK</td>
             <td>UIVIEWS_CURRENT</td>
             <td>UIVIEWID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>TEAM ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

>[!NOTE]
>
>Nelle tabelle degli oggetti Team sono archiviati 3 tipi di team: PROJECT, TEMPLATE e ADHOC. <br>
>Ciascuno di questi tipi di team è rappresentato insieme nelle visualizzazioni del data lake di Data Connect. Per isolare il tipo specifico di team da restituire, è necessario filtrare in base alla colonna `teamtype`. Ad esempio, se desideri solo i team tradizionali che fanno parte delle strutture organizzative, configurate nell’area Team dell’applicazione, potresti avere una query simile alla seguente: <code>seleziona * da teams_current dove teamtype = &quot;ADHOC&quot;;</code>

### Membro team

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Membro team</td>
            <td>Altri team, membro del team</td>
            <td>TEAM</td>
            <td>Membro team</td>
            <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TEAM ID</td>
             <td>FK</td>
             <td>TEAM_CURRENT</td>
             <td>TEAM ID</td>
        </tr>
        <tr>
             <td>TEAMMEMBERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Mansione membro team

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Mansione membro team</td>
            <td>Mansione membro team</td>
            <td>TEAMMR</td>
            <td>Mansione membro team</td>
            <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TEAM ID</td>
             <td>FK</td>
             <td>TEAM_CURRENT</td>
             <td>TEAM ID</td>
        </tr>
        <tr>
             <td>TEAMMEMBERROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Modello

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Modello</td>
            <td>Modello, Modello di progetto</td>
            <td>TMPL</td>
            <td>Modello</td>
            <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DELIVERABLESCORECARDID</td>
             <td>-</td>
             <td colspan="2">Tabella di Scorecard del deliverable non supportata al momento</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATHID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATHID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMI_CORRENTI</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">Tabella di definizione della coda attualmente non supportata</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TEAM ID</td>
             <td>FK</td>
             <td>TEAM_CURRENT</td>
             <td>TEAM ID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Assegnazione attività modello

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Assegnazione attività modello</td>
            <td>Assegnazione Modello</td>
            <td>ATTIVITÀ</td>
            <td>Assegnazione Modello</td>
            <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TEAM ID</td>
             <td>FK</td>
             <td>TEAM_CURRENT</td>
             <td>TEAM ID</td>
        </tr>
        <tr>
             <td>TEAMTIMELINEABLEID</td>
             <td>-</td>
             <td colspan="2">Tabella Timeline Team non supportata al momento</td>
        </tr>
        <tr>
             <td>TEMPLATEASSIGNMENTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>TEMPLATFORM</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATFORM</td>
        </tr>
    </tbody>
</table>

### Attività modello

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Attività modello</td>
            <td>Attività modello</td>
            <td>TTSK</td>
            <td>Attività modello</td>
            <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ASSIGNEDTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>FK</td>
             <td>MILESTONES_CURRENT</td>
             <td>MILESTONEID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATFORM</td>
        </tr>
        <tr>
             <td>RECURRENCERULEID</td>
             <td>-</td>
             <td colspan="2">Tabella delle regole di ricorrenza non supportata al momento</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TEAM ID</td>
             <td>FK</td>
             <td>TEAM_CURRENT</td>
             <td>TEAM ID</td>
        </tr>
        <tr>
             <td>TEAMTIMELINEABLEID</td>
             <td>-</td>
             <td colspan="2">Tabella Timeline Team non supportata al momento</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATFORM</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Predecessore attività modello

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Predecessore attività modello</td>
            <td>Predecessore modello</td>
            <td>TPRED</td>
            <td>Predecessore</td>
            <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PREDECESSORID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATFORM</td>
        </tr>
        <tr>
             <td>SUCCESSORID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATFORM</td>
        </tr>
        <tr>
             <td>PREDECESSORID MODELLO</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### KPI rapportati alla scala cronologica combinati

Disponibilità limitata dei clienti

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>KPI rapportati alla scala cronologica combinati</td>
            <td>KPI a fasi temporali</td>
            <td>TMPH</td>
            <td>KPIaseTempo</td>
            <td>TIMEPHASED_COMBINED_CURRENT<br>TIMEPHASED_COMBINED_DAILY_HISTORY<br>TIMEPHASED_COMBINED_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
                <tr>
             <td>EVENT_ID    </td>
             <td>PK</td>
             <td>Chiave naturale per la voce KPI rapportata alla tempificazione</td>
             <td>-</td>
        </tr>
                        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
                        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFICATORE_CORRENTE</td>
             <td>CLASSIFIERID</td>
        </tr>
                        <tr>
             <td>METADATAID</td>
             <td>FK</td>
             <td>Tabella METADATI non fornita</td>
             <td>-</td>
        </tr>
                        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
                        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIO_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
                        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMI_CORRENTI</td>
             <td>PROGRAMID</td>
        </tr>
                        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
                        <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE
</td>
        </tr>
                        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
                        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>Tabella SCHEMA non specificata. Il valore di questa tabella viene fornito nella colonna SCHEMANAME. SCHEMANAME identifica l'indicatore KPI (ad esempio, plannedHours, estimatedHours e actualHours) a cui è connesso il record.</td>
             <td>-</td>
        </tr>
                                <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                                <tr>
             <td>STAFFINGPLANID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>
                                <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_RESOURCE_CURRENT</td>
             <td>STAFFINGPLANRESOURCEID</td>
        </tr>
                                <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                                <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Valuta indicatore KPI rapportato alla scala cronologica

Disponibilità limitata dei clienti

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Valuta indicatore KPI rapportato alla scala cronologica</td>
            <td>KPI a fasi temporali</td>
            <td>TMPH</td>
            <td>KPIaseTempo</td>
            <td>TIMEPHASED_CURRENCY_CURRENT<br>TIMEPHASED_CURRENCY_DAILY_HISTORY<br>TIMEPHASED_CURRENCY_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFICATORE_CORRENTE</td>
             <td>CLASSIFIERID</td>
        </tr>
                <tr>
             <td>METADATAID</td>
             <td>FK</td>
             <td>Tabella METADATI non fornita</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIO_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMI_CORRENTI</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>Tabella SCHEMA non specificata. Il valore di questa tabella viene fornito nella colonna SCHEMANAME. SCHEMANAME identifica l'indicatore KPI (ad esempio, plannedRevenueRate, plannedCostRate, actualRevenue, ecc.) che il record è connesso a.</td>
             <td>SCHEMAID</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                <tr>
             <td>STAFFINGPLANID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>
          <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_RESOURCE_CURRENT</td>
             <td>STAFFINGPLANRESOURCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMEPHASEDCURRENCYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Durata KPI rapportata alla tempificazione

Disponibilità limitata dei clienti

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Durata KPI rapportata alla tempificazione</td>
            <td>KPI a fasi temporali</td>
            <td>TMPH</td>
            <td>KPIaseTempo</td>
            <td>TIMEPHASED_DURATION_CURRENT<br>TIMEPHASED_DURATION_DAILY_HISTORY<br>TIMEPHASED_DURATION_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFICATORE_CORRENTE</td>
             <td>CLASSIFIERID</td>
        </tr>
                <tr>
             <td>METADATAID</td>
             <td>FK</td>
             <td>Tabella METADATI non fornita</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIO_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMI_CORRENTI</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>Tabella SCHEMA non specificata. Il valore di questa tabella viene fornito nella colonna SCHEMANAME. SCHEMANAME identifica l'indicatore KPI (ad esempio, plannedHours, estimatedHours e actualHours) a cui è connesso il record.</td>
             <td>SCHEMAID</td>
        </tr>
        <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                <tr>
             <td>STAFFINGPLANID </td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>
           <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_RESOURCE_CURRENT</td>
             <td>STAFFINGPLANRESOURCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMEPHASEDDURATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Numeri KPI rapportati alla scala cronologica

Disponibilità limitata dei clienti

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Numeri KPI rapportati alla scala cronologica</td>
            <td>KPI a fasi temporali</td>
            <td>TMPH</td>
            <td>KPIaseTempo</td>
            <td>TIMEPHASED_NUMBERS_CURRENT<br>TIMEPHASED_NUMBERS_DAILY_HISTORY<br>TIMEPHASED_NUMBERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>EVENT_ID</td>
             <td>PK</td>
             <td>Chiave naturale per la voce KPI rapportata alla tempificazione</td>
             <td>-</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFICATORE_CORRENTE</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>METADATAID</td>
             <td>FK</td>
             <td>Tabella METADATI non fornita</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PORTFOLIOID</td>
             <td>FK</td>
             <td>PORTFOLIO_CURRENT</td>
             <td>PORTFOLIOID</td>
        </tr>
                <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMMI_CORRENTI</td>
             <td>PROGRAMID</td>
        </tr>
                <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
                <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
                <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
                <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>Tabella SCHEMA non specificata. Il valore di questa tabella viene fornito nella colonna SCHEMANAME. SCHEMANAME identifica l'indicatore KPI (ad esempio, plannedHours, estimatedHours e actualHours) a cui è connesso il record.</td>
             <td>-</td>
        </tr>
                <tr>
             <td>SOURCETASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                <tr>
             <td>STAFFINGPLANID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_CURRENT</td>
             <td>STAFFINGPLANID</td>
        </tr>
                <tr>
             <td>STAFFINGPLANRESOURCEID</td>
             <td>FK</td>
             <td>STAFFING_PLAN_RESOURCE_CURRENT</td>
             <td>STAFFINGPLANRESOURCEID</td>
        </tr>
                <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
                <tr>
             <td>TIMEPHASEDNUMBERSID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
                <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Scheda orario

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Scheda orario</td>
            <td>Scheda orario</td>
            <td>TSHET</td>
            <td>Scheda orario</td>
            <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>FK</td>
             <td>TIMESHEETPROFILES_CURRENT</td>
             <td>TIMESHEETPROFILEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Profilo scheda orario

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Profilo scheda orario</td>
            <td>Profilo scheda orario</td>
            <td>TSPRO</td>
            <td>Profilo scheda orario</td>
            <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Filtro interfaccia utente

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Filtro interfaccia utente</td>
            <td>Filtro</td>
            <td>UIFT</td>
            <td>Filtro</td>
            <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>UIFILTERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Raggruppa per interfaccia utente

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Raggruppa per interfaccia utente</td>
            <td>Raggruppamento</td>
            <td>UIGB</td>
            <td>Raggruppamento</td>
            <td>UIGROUPBYS_CURRENT<br>UIGROUPBYS_DAILY_HISTORY<br>UIGROUPBYS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>UIGROUPBYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Modello interfaccia utente

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Modello interfaccia utente</td>
            <td>Modello layout</td>
            <td>UITMPL</td>
            <td>Modello layout</td>
            <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Visualizzazione interfaccia utente

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Visualizzazione interfaccia utente</td>
            <td>Visualizzazione</td>
            <td>UIVIEW</td>
            <td>Visualizzazione</td>
            <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>UIVIEWID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Utente

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Utente</td>
            <td>Utente</td>
            <td>UTENTE</td>
            <td>Utente</td>
            <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>FK</td>
             <td>ACCESSLEVELS_CURRENT</td>
             <td>ACCESSLEVELID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DEFAULTHOURTYPEID</td>
             <td>FK</td>
             <td>HOURTYPES_CURRENT</td>
             <td>HOURTYPEID</td>
        </tr>
        <tr>
             <td>DELEGATIONTOID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EAUTHUSERID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>HOMETEAMID</td>
             <td>FK</td>
             <td>TEAM_CURRENT</td>
             <td>TEAM ID</td>
        </tr>
        <tr>
             <td>LASTENTEREDNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LATESTUPDATENOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">La tabella del modello di layout non sarà supportata</td>
        </tr>
        <tr>
             <td>MANAGERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTALPROFILEID</td>
             <td>-</td>
             <td colspan="2">La tabella Portal Profile non sarà supportata</td>
        </tr>
        <tr>
             <td>PREFUIID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>FK</td>
             <td>RESOURCEPOOLS_CURRENT</td>
             <td>RESOURCEPOOLID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>FK</td>
             <td>TIMESHEETPROFILES_CURRENT</td>
             <td>TIMESHEETPROFILEID</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>UUMUSERID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
    </tbody>
</table>

### Delega utente

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Delega utente</td>
            <td>Delega utente</td>
            <td>USRDEL</td>
            <td>Delega utente</td>
            <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>FROMUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TOUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERDELEGATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Gruppo di utenti

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Gruppo di utenti</td>
            <td>Altre Gruppi</td>
            <td>USRGPS</td>
            <td>Gruppo di utenti</td>
            <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERSGROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Posizione utente

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Posizione utente</td>
            <td>Posizione utente</td>
            <td>USRLOC</td>
            <td>UserLocation</td>
            <td>USERLOCATIONS_CURRENT<br>USERLOCATIONS_DAILY_HISTORY<br>USERLOCATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFICATORE_CORRENTE</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERLOCATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Mansione utente

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Mansione utente</td>
            <td>Altre mansioni</td>
            <td>USRROL</td>
            <td>Mansione utente</td>
            <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERROLESETID</td>
             <td>FK</td>
             <td>USERROLESET_CURRENT</td>
             <td>USERROLESETID</td>
        </tr>
        <tr>
             <td>USERLOCATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Valore Preferenze Utente

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Valore Pref Utente</td>
            <td>Preferenze utente</td>
            <td>USERPF</td>
            <td>Preferenze utente</td>
            <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERPREFVALUEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Set di ruoli utente

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UserRoleSet</td>
            <td>Set di ruoli utente</td>
            <td>URSET</td>
            <td>UserRoleSet</td>
            <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PRIMARYROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERROLESETID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### Decisioni degli utenti

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UsersDecisions</td>
            <td>Decisioni degli utenti</td>
            <td>USRDEC</td>
            <td>Decisioni degli utenti</td>
            <td>USERSDECISIONS_CURRENT<br>USERSDECISIONS_DAILY_HISTORY<br>USERSDECISIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>USERDECISIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### Elemento di lavoro

<table>
    <thead>
        <tr>
            <th>Nome entità Workfront</th>
            <th>Riferimenti interfaccia</th>
            <th>Riferimento API</th>
            <th>Etichetta API</th>
            <th>Visualizzazioni Data Lake</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>WorkItem</td>
            <td>Elemento di lavoro</td>
            <td>WRKITM</td>
            <td>WorkItem</td>
            <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>Chiave primaria/esterna</th>
            <th>Tipo</th>
            <th>Tabella correlata</th>
            <th>Campo correlato</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>Variabile, basata su OBJCODE</td>
             <td>Chiave/ID primario dell'oggetto identificato nel campo OBJCODE</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>PROJECTS_CURRENT</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">Non una relazione; utilizzato per scopi interni all’applicazione</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>TASKS_CURRENT</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>WORKITEMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

## Descrizioni e relazioni della vista Pianificazione

Le tabelle seguenti descrivono le visualizzazioni dati disponibili nello schema Planning in Data Connect. A differenza delle visualizzazioni dati del flusso di lavoro, le visualizzazioni dati di Planning includono una descrizione completa colonna per colonna per ogni visualizzazione.

I dati di Planning sono disponibili nelle seguenti viste:

* **FIELD\_CURRENT**: le definizioni correnti di tutti i campi configurati nei tipi di record di Planning.
* **FIELD\_DAILY\_HISTORY** — Istantanea giornaliera delle definizioni dei campi, utile per tenere traccia delle modifiche alla configurazione dei campi nel tempo.
* **FIELD\_EVENT** — Registro delle modifiche di ogni evento che modifica la definizione di un campo.
* **PLANNINGRECORD\_CURRENT**: lo stato corrente di tutti i record di Planning in tutte le aree di lavoro e i tipi di record.
* **PLANNINGRECORD\_DAILY\_HISTORY**: snapshot giornaliero dello stato del record di Planning, utile per l&#39;analisi delle tendenze.
* **PLANNINGRECORD\_EVENT** — Un registro delle modifiche di ogni evento che modifica un record di Planning, utile per confronti point-in-time.
* **RECORDTYPE\_CURRENT**: le definizioni correnti di tutti i tipi di record configurati nelle aree di lavoro di Planning.
* **RECORDTYPE\_DAILY\_HISTORY**: snapshot giornaliero delle definizioni dei tipi di record, utile per tenere traccia delle modifiche di configurazione dei tipi di record nel tempo.
* **RECORDTYPE\_EVENT**: registro delle modifiche di ogni evento che modifica una definizione di tipo di record.
* **REFERENCE\_CURRENT** — Lo stato corrente di tutte le connessioni di riferimento tra oggetti diversi tra i record di Planning e gli oggetti Workfront (o altri oggetti esterni).
* **WORKSPACE\_CURRENT**: le definizioni correnti di tutte le aree di lavoro di Planning.
* **WORKSPACE\_DAILY\_HISTORY**: snapshot giornaliero delle definizioni dell&#39;area di lavoro, utile per tenere traccia delle modifiche alla configurazione dell&#39;area di lavoro nel tempo.
* **WORKSPACE\_EVENT**: registro delle modifiche di ogni evento che modifica una definizione dell&#39;area di lavoro.



>[!NOTE]
>
>Le viste seguenti sono disponibili nello schema di Planning, ma non sono descritte in dettaglio. Seguono gli stessi pattern di colonne delle visualizzazioni CORRENTI corrispondenti, con l’aggiunta di campi di audit degli eventi e della cronologia standard.
>
>Le visualizzazioni sono:
>
>* VISTE DAILY\_HISTORY
>
>* VISUALIZZAZIONI EVENTO (CAMPO\_DAILY\_HISTORY, CAMPO\_EVENT, PLANNINGRECORD\_DAILY\_HISTORY, PLANNINGRECORD\_EVENT, RECORDTYPE\_DAILY\_HISTORY, RECORDTYPE\_EVENT, WORKSPACE\_DAILY\_HISTORY e WORKSPACE\_EVENT)


### CAMPO\_CURRENT

Contiene le definizioni correnti di tutti i campi configurati nei tipi di record di Workfront Planning. Ogni riga rappresenta un campo, inclusi il nome visualizzato, il tipo e la configurazione specifica per il tipo, memorizzati in colonne Variante strutturata (JSON). Utilizzare questa visualizzazione per risolvere gli ID di campo da PLANNINGRECORD\_CURRENT in nomi di campo e metadati leggibili dall&#39;utente.

<table>
    <tr>
        <td>Nome colonna</td>
        <td>Tipo</td>
        <td>Descrizione</td>
        <td>Tabella correlata</td>
        <td>Campo correlato</td>
    </tr>
    <tr>
        <td>"ID"</td>
        <td>Varchar</td>
        <td>Identificatore univoco per la definizione del campo. Chiave primaria per questa visualizzazione.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>'RECORDTYPEID'</td>
        <td>Varchar</td>
        <td>Identificatore univoco del tipo di record a cui appartiene questo campo. Utilizzare con RECORDTYPE\_CURRENT per cercare i dettagli del tipo di record.</td>
        <td>RECORDTYPE\_CURRENT</td>
        <td>ID</td>
    </tr>
    <tr>
        <td>"DISPLAYNAME"</td>
        <td>Varchar</td>
        <td>Il nome visualizzato del campo come mostrato nell'interfaccia di Planning.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"ALIASNAME"</td>
        <td>Varchar</td>
        <td>Una versione URL-safe, in minuscolo, del nome visualizzato del campo, utilizzata per l’identificazione a livello di sistema e l’accesso API (ad esempio, "End Date" diventa "end_date", "Percent Complete" diventa "percent_complete").</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"DESCRIPTION"</td>
        <td>Varchar</td>
        <td>Descrizione fornita dall'utente dello scopo del campo.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"FIELDTYPE"</td>
        <td>Varchar</td>
        <td>Tipo di dati o categoria di campi. I valori possibili includono: "text", "long-text", "number", "percentage", "currency", "date", "boolean", "single-select", "multi-select", "reference", "lookup", "formula", "user", "created-at" e "created-by".</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"HASERROR"</td>
        <td>Varchar</td>
        <td>Indica se il campo presenta attualmente un errore di configurazione o sincronizzazione. I valori sono le stringhe "true" o "false". Il valore "true" indica che il campo si trova in uno stato di errore e potrebbe non restituire correttamente i dati.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>'LINKEDFIELD'</td>
        <td>Variante</td>
        <td>Oggetto JSON contenente la definizione completa del campo di origine a cui è collegato questo campo. Presente per tipi di campo "reference" e "lookup"; include proprietà come "alias", "displayName", "fieldType" e "createdAt". Null per i campi non collegati.</td>
        <td>CAMPO\_CURRENT</td>
        <td>ID</td>
    </tr>
    <tr>
        <td>"OPTIONS"</td>
        <td>Variante</td>
        <td>Un array JSON di oggetti di scelta per i campi "single-select" e "multi-select". Ogni oggetto di scelta contiene "color" (un’etichetta di colore denominata), "displayName" (l’etichetta mostrata nell’interfaccia utente) e "name" (il nome API interno). Null per i tipi di campo non selezionati.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"DATEOPTIONS"</td>
        <td>Variante</td>
        <td>Un oggetto JSON contenente la configurazione di visualizzazione specifica per data per i campi "date". Include "dateFormat" (ad es., "locale") e "timeFormat" (null se non viene visualizzata l’ora). Null per i tipi di campo non di data.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"FORMULAOPTIONS"</td>
        <td>Variante</td>
        <td>Un oggetto JSON contenente la configurazione della formula per i campi "formula". Include "formula" (l’espressione della formula leggibile dall’uomo), "returnType" (ad esempio, "PERCENTAGE", "NUMBER"), "numberOptions" (precisione, visualizzazione) e "dateOptions". Nullo per i campi non formula.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"REFERENCEOPTIONS"</td>
        <td>Variante</td>
        <td>Un oggetto JSON contenente la configurazione della connessione per i campi "reference" che si collegano ad altri tipi di record di Planning. Include "backField" (la definizione del campo di riferimento inverso sul tipo di record connesso) e "linkedRecordTypeId". Null per i campi non di riferimento.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"LOOKUPOPTIONS"</td>
        <td>Variante</td>
        <td>Un oggetto JSON contenente la configurazione di ricerca per campi "lookup" che richiamano valori da un tipo di record connesso. Include "referenceFieldId" (l’ID del campo di riferimento che guida la ricerca), "rollup" (metodo di aggregazione o null per nessuna aggregazione) e "sourceField" (un oggetto con il "id" del campo che viene cercato). Null per i campi non di ricerca.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"NUMBEROPTIONS"</td>
        <td>Variante</td>
        <td>Un oggetto JSON contenente opzioni di formattazione numerica per i campi "number", "percentage" e "currency". Include "allowNegatives" (booleano), "currency" (codice valuta o nullo), "precision" (posizioni decimali) e "visualizationType" (stile di visualizzazione o null per il testo normale). Null per i tipi di campo non numerici.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>`EXTERNALOPTIONS`</td>
        <td>Variante</td>
        <td>Oggetto JSON contenente la configurazione dei campi collegati a sistemi esterni al di fuori di Planning. In genere null per i campi creati in modo nativo; popolato per i campi su tipi di record connessi esternamente.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"CREATEDAT"</td>
        <td>Timestamp\_NTZ</td>
        <td>La marca temporale (nessun fuso orario) di quando è stato creato questo campo.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"CREATEDBY"</td>
        <td>Varchar</td>
        <td>Identificatore dell'utente che ha creato il campo.</td>
        <td>WF.USERS\_CORRENTE</td>
        <td>EAUTHUSERID</td>
    </tr>
    <tr>
        <td>"UPDATEDAT"</td>
        <td>Timestamp\_NTZ</td>
        <td>La marca temporale (nessun fuso orario) dell’ultimo aggiornamento di questo campo.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"UPDATEDBY"</td>
        <td>Varchar</td>
        <td>Identificatore dell'ultimo utente che ha aggiornato questo campo.</td>
        <td>WF.USERS\_CORRENTE</td>
        <td>EAUTHUSERID</td>
    </tr>
    <tr>
        <td>'USERID'</td>
        <td>Varchar</td>
        <td>L’identificatore dell’utente associato a questo campo, in genere il proprietario del campo.</td>
        <td>WF.USERS\_CORRENTE</td>
        <td>EAUTHUSERID</td>
    </tr>
    <tr>
        <td>"CREATED"</td>
        <td>Numero</td>
        <td>Flag che indica l'ultimo tipo di operazione che ha interessato il record di campo. Il valore 1 indica che il record è stato creato nel ciclo di aggiornamento dati più recente, mentre il valore 0 indica che non lo è stato. Consulta CREATEDAT per la marca temporale della creazione effettiva.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"UPDATED"</td>
        <td>Numero</td>
        <td>Flag che indica l'ultimo tipo di operazione che ha interessato il record di campo. Il valore 1 indica che il record è stato aggiornato nel ciclo di aggiornamento dei dati più recente; 0 indica che non lo era. Per la marca temporale effettiva dell’ultimo aggiornamento, consulta UPDATEDAT.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"DELETED"</td>
        <td>Numero</td>
        <td>Flag che indica se il campo è stato eliminato temporaneamente. Il valore 1 indica eliminato, 0 indica attivo.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"RESTORED"</td>
        <td>Numero</td>
        <td>Flag che indica se il campo è stato ripristinato dopo l’eliminazione temporanea.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"TRIGGEREDBYSERVICE"</td>
        <td>Varchar</td>
        <td>Il nome del servizio o dell’integrazione che ha attivato l’ultima modifica a questo record di campo. Il valore "Unknown" indica che non è stato possibile determinare il servizio di origine.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>`ISFUSION`</td>
        <td>Booleano</td>
        <td>Flag che indica se il campo è stato creato o gestito tramite un’integrazione di Workfront Fusion. Il valore "true" indica la gestione di Fusion; "false" o un valore vuoto indica che si tratta di un campo creato in modo nativo.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"DL_LOAD_TIMESTAMP"</td>
        <td>Timestamp\_NTZ</td>
        <td>La marca temporale del processo di aggiornamento dati che ha caricato per ultimo questo record di campo nel data lake. Aggiornato dopo ogni ciclo di aggiornamento dei dati riuscito.</td>
        <td>—</td>
        <td>—</td>
    </tr>
</table>

### PLANNINGRECORD\_CURRENT

Contiene lo stato corrente di tutti i record creati in Workfront Planning, in tutte le aree di lavoro e in tutti i tipi di record. Ogni riga rappresenta un record Planning, con valori di campo memorizzati in colonne Variante strutturata (JSON) che riflettono la natura dinamica e flessibile dello schema dei dati Planning.

<table>
    <tr>
        <td>Nome colonna</td>
        <td>Tipo</td>
        <td>Descrizione</td>
        <td>Tabella correlata</td>
        <td>Campo correlato</td>
    </tr>
    <tr>
        <td>`RECORDID`</td>
        <td>Varchar</td>
        <td>Identificatore univoco del record di Planning. Chiave primaria per questa visualizzazione.</td>
        <td>WF.PLANNINGRECORDS\_CORRENTE</td>
        <td>RECORDID</td>
    </tr>
    <tr>
        <td>"WORKSPACEID"</td>
        <td>Varchar</td>
        <td>Identificatore univoco dell'area di lavoro di Planning che contiene il record.</td>
        <td>WORKSPACE\_CURRENT</td>
        <td>ID</td>
    </tr>
    <tr>
        <td>"WORKSPACENAME"</td>
        <td>Varchar</td>
        <td>Nome visualizzato dell'area di lavoro di Planning che contiene questo record.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>'RECORDTYPEID'</td>
        <td>Varchar</td>
        <td>Identificatore univoco del tipo di record (ad esempio, Campagna, Iniziativa) a cui appartiene il record.</td>
        <td>RECORDTYPE\_CURRENT</td>
        <td>ID</td>
    </tr>
    <tr>
        <td>'RECORDTYPENAME'</td>
        <td>Varchar</td>
        <td>Nome visualizzato del tipo di record a cui appartiene il record.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"FIELD_IDS"</td>
        <td>Variante</td>
        <td>Un oggetto JSON che mappa il nome visualizzato di ciascun campo al relativo ID campo (ad esempio, `{"Status": "F69bc...", "End Date": "F69bc..."}`). Usate questa funzione per mappare i nomi dei campi leggibili dall'utente agli ID utilizzati in FIELDID\_VALUES e FIELDID\_VALUES\_RAW.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"FIELD_VALUES_RAW"</td>
        <td>Variante</td>
        <td>Oggetto JSON che mappa il nome visualizzato di ciascun campo sul relativo valore non formattato. Per i campi di riferimento, il valore è una matrice di oggetti record connessi; per i campi numerici e per i campi formula, è un valore numerico semplice; per i campi di testo lungo, è un oggetto contenuto in formato Rich Text. Chiave in base al nome visualizzato del campo, campo corrispondente\_IDS.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"FIELD_VALUES"</td>
        <td>Variante</td>
        <td>Oggetto JSON che mappa il nome visualizzato di ciascun campo al relativo valore stringa in formato di visualizzazione. Chiave in base al nome visualizzato del campo, campo corrispondente\_IDS.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"FIELD_TYPES"</td>
        <td>Variante</td>
        <td>Un oggetto JSON che mappa il nome visualizzato di ciascun campo alla relativa stringa del tipo di campo (ad esempio, "text", "number", "date", "single-select", "reference", "formula"). Chiave in base al nome visualizzato del campo, campo corrispondente\_IDS.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>`FIELDID_VALUES`</td>
        <td>Variante</td>
        <td>Oggetto JSON che mappa ogni ID campo sul relativo valore in formato di visualizzazione. Per i tipi di campo semplici il valore è una stringa o un numero; per i campi di testo lungo è un oggetto contenente sia le proprietà "content" (testo normale) che le proprietà "contentHTML" (formattato in HTML). Utilizzare FIELD\_IDS per cercare il nome visualizzato per ciascun ID campo.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>`FIELDID_VALUES_RAW`</td>
        <td>Variante</td>
        <td>Oggetto JSON che mappa ogni ID campo al relativo valore non formattato. Per la maggior parte dei tipi di campo, i valori sono stringhe semplici, numeri o marche temporali millisecondi epoca. I campi a testo lungo restituiscono il contenuto di testo normale come stringa. Utilizzare FIELD\_IDS per cercare il nome visualizzato per ciascun ID campo.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>`FIELDID_FIELDID`</td>
        <td>Variante</td>
        <td>Oggetto JSON che elenca tutti gli ID di campo presenti in questo record come mappatura automatica (ogni ID di campo viene mappato su se stesso). Usare questa funzione per enumerare i campi compilati in un determinato record o per fare riferimento incrociato con FIELD\_CURRENT.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"REFERENCE_IDS"</td>
        <td>Variante</td>
        <td>Un oggetto JSON che mappa il nome visualizzato di ciascun campo di riferimento all’ID del record di connessione (ad esempio, `{"Project": "Ref8b471aa..."}`). Utilizzare in combinazione con REFERENCE\_CURRENT per risolvere gli oggetti esterni collegati per questo record.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"CREATED"</td>
        <td>Numero</td>
        <td>Flag che indica l'ultimo tipo di operazione che ha interessato il record. Il valore 1 indica che il record è stato creato nel ciclo di aggiornamento dati più recente, mentre il valore 0 indica che non lo è stato. Consulta CREATEDAT per la marca temporale della creazione effettiva.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"UPDATED"</td>
        <td>Numero</td>
        <td>Flag che indica l'ultimo tipo di operazione che ha interessato il record. Il valore 1 indica che il record è stato aggiornato nel ciclo di aggiornamento dei dati più recente; 0 indica che non lo era. Per la marca temporale effettiva dell’ultimo aggiornamento, consulta UPDATEDAT.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"DELETED"</td>
        <td>Numero</td>
        <td>Flag che indica se il record è stato eliminato in modo non permanente. Il valore 1 indica che il record è stato eliminato, mentre il valore 0 indica che è attivo.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"CREATEDAT"</td>
        <td>Timestamp\_NTZ</td>
        <td>La marca temporale (nessun fuso orario) di quando è stato creato questo record.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"CREATEDBY"</td>
        <td>Varchar</td>
        <td>Identificatore dell'utente che ha creato il record.</td>
        <td>WF.USERS\_CORRENTE</td>
        <td>EAUTHUSERID</td>
    </tr>
    <tr>
        <td>"UPDATEDAT"</td>
        <td>Timestamp\_NTZ</td>
        <td>La marca temporale (nessun fuso orario) dell’ultimo aggiornamento di questo record.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"UPDATEDBY"</td>
        <td>Varchar</td>
        <td>Identificatore dell'ultimo utente che ha aggiornato il record.</td>
        <td>WF.USERS\_CORRENTE</td>
        <td>EAUTHUSERID</td>
    </tr>
    <tr>
        <td>"DL_LOAD_TIMESTAMP"</td>
        <td>Timestamp\_NTZ</td>
        <td>La marca temporale del processo di aggiornamento dati che ha caricato per ultimo questo record nel data lake. Aggiornato dopo ogni ciclo di aggiornamento dei dati riuscito.</td>
        <td>—</td>
        <td>—</td>
    </tr>
</table>

### RECORDTYPE\_CURRENT

Contiene le definizioni correnti di tutti i tipi di record configurati nelle aree di lavoro di Workfront Planning. Ogni riga rappresenta un tipo di record, inclusi il nome visualizzato, l&#39;associazione all&#39;area di lavoro, il campo primario e i metadati di configurazione. Utilizzare questa visualizzazione per risolvere gli ID dei tipi di record da PLANNINGRECORD\_CURRENT e FIELD\_CURRENT in nomi leggibili dall&#39;utente.

<table>
    <tr>
        <td>Nome colonna</td>
        <td>Tipo</td>
        <td>Descrizione</td>
        <td>Tabella correlata</td>
        <td>Campo correlato</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"ID"</td>
        <td>Varchar</td>
        <td>Identificatore univoco per il tipo di record. Chiave primaria per questa visualizzazione.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"CREATED"</td>
        <td>Numero</td>
        <td>Flag che indica l'ultimo tipo di operazione che ha interessato questo tipo di record. Il valore 1 indica che il tipo di record è stato creato nel ciclo di aggiornamento dati più recente, mentre il valore 0 indica che non lo è stato. Consulta CREATEDAT per la marca temporale della creazione effettiva.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"UPDATED"</td>
        <td>Numero</td>
        <td>Flag che indica l'ultimo tipo di operazione che ha interessato questo tipo di record. Il valore 1 indica che il tipo di record è stato aggiornato nel ciclo di aggiornamento dei dati più recente, mentre il valore 0 indica che non lo era. Per la marca temporale effettiva dell’ultimo aggiornamento, consulta UPDATEDAT.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"DELETED"</td>
        <td>Numero</td>
        <td>Flag che indica se il tipo di record è stato eliminato in modo non permanente. Il valore 1 indica eliminato, 0 indica attivo.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"DL_LOAD_TIMESTAMP"</td>
        <td>Timestamp\_NTZ</td>
        <td>La marca temporale del processo di aggiornamento dati che ha caricato per ultimo questo tipo di record nel data lake. Aggiornato dopo ogni ciclo di aggiornamento dei dati riuscito.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"CREATEDBY"</td>
        <td>Varchar</td>
        <td>Identificatore dell'utente che ha creato questo tipo di record.</td>
        <td>WF.USERS\_CORRENTE</td>
        <td>EAUTHUSERID</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"CREATEDAT"</td>
        <td>Timestamp\_NTZ</td>
        <td>La marca temporale (senza fuso orario) di quando è stato creato questo tipo di record.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"UPDATEDBY"</td>
        <td>Varchar</td>
        <td>Identificatore dell'ultimo utente che ha aggiornato questo tipo di record.</td>
        <td>WF.USERS\_CORRENTE</td>
        <td>EAUTHUSERID</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"UPDATEDAT"</td>
        <td>Timestamp\_NTZ</td>
        <td>La marca temporale (nessun fuso orario) dell’ultimo aggiornamento di questo tipo di record.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>'USERID'</td>
        <td>Varchar</td>
        <td>Identificatore dell'utente associato a questo tipo di record, in genere il proprietario.</td>
        <td>WF.USERS\_CORRENTE</td>
        <td>EAUTHUSERID</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"WORKSPACEID"</td>
        <td>Varchar</td>
        <td>Identificatore univoco dell'area di lavoro a cui appartiene questo tipo di record. Usare con WORKSPACE\_CURRENT per cercare i dettagli del workspace.</td>
        <td>WORKSPACE\_CURRENT</td>
        <td>ID</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"DISPLAYNAME"</td>
        <td>Varchar</td>
        <td>Il nome visualizzato del tipo di record come mostrato nell'interfaccia di Planning (ad esempio, "Campaign", "Initiative").</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"DESCRIPTION"</td>
        <td>Varchar</td>
        <td>Descrizione fornita dall'utente dello scopo del tipo di record.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"COLOR"</td>
        <td>Varchar</td>
        <td>Un’etichetta a colori con nome associata a questo tipo di record nell’interfaccia di Planning (ad esempio, "blue", "green", "purple", "magenta", "chartreuse", "dark-gray"). Non è un codice esadecimale.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"PERMISSION"</td>
        <td>Varchar</td>
        <td>Il livello di autorizzazione configurato per l’accesso a questo tipo di record (ad esempio, "VIEW", "CONTRIBUTE", "MANAGE"). Può essere vuoto se non è impostata alcuna autorizzazione personalizzata.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>`PRIMARYFIELDID`</td>
        <td>Varchar</td>
        <td>Identificatore del campo designato come campo principale (titolo) per questo tipo di record. Chiave esterna a FIELD\_CURRENT.ID.</td>
        <td>CAMPO\_CURRENT</td>
        <td>ID</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"ISTAXONOMY"</td>
        <td>Varchar</td>
        <td>Indica se questo tipo di record è classificato come tipo di tassonomia, utilizzato per organizzare e classificare altri record. Il valore "true" indica un tipo di tassonomia. Può essere vuoto per i tipi di record non di tassonomia.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"PERMISSION"</td>
        <td>Varchar</td>
        <td>Il livello di autorizzazione configurato per l’accesso a questo tipo di record (ad esempio, "VIEW", "CONTRIBUTE", "MANAGE"). Può essere vuoto se non è impostata alcuna autorizzazione personalizzata.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td>`PRIMARYFIELDID`</td>
        <td>Varchar</td>
        <td>Identificatore del campo designato come campo principale (titolo) per questo tipo di record. Chiave esterna a FIELD\_CURRENT.ID.</td>
        <td>CAMPO\_CURRENT</td>
        <td>ID</td>
    </tr>
    <tr>
        <td>"ISTAXONOMY"</td>
        <td>Varchar</td>
        <td>Indica se questo tipo di record è classificato come tipo di tassonomia, utilizzato per organizzare e classificare altri record. Il valore "true" indica un tipo di tassonomia. Può essere vuoto per i tipi di record non di tassonomia.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>`INTERNO`</td>
        <td>Booleano</td>
        <td>Flag che indica se questo tipo di record rappresenta un tipo di oggetto connesso esternamente anziché un record di Planning nativo.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>`EXTERNALOPTIONS`</td>
        <td>Variante</td>
        <td>Oggetto JSON contenente i dettagli di configurazione per i tipi di record connessi a sistemi esterni. Include "connectionName" (ad esempio, "workfront"), "objectName" (il codice oggetto API di Workfront, ad esempio, "PROJ") e "fields" (una mappa degli alias di campo standard sugli ID campo di Planning per i campi sincronizzati). Null per i tipi di record creati in modo nativo.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"RESTORED"</td>
        <td>Numero</td>
        <td>Flag che indica se il tipo di record è stato ripristinato dopo l'eliminazione temporanea.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"ALIAS"</td>
        <td>Varchar</td>
        <td>Alias interno per il tipo di record, utilizzato per l’identificazione a livello di sistema e l’accesso API. Può essere vuoto per i tipi di record a cui non è stato assegnato un alias.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"TRIGGEREDBYSERVICE"</td>
        <td>Varchar</td>
        <td>Nome del servizio o dell'integrazione che ha attivato l'ultima modifica a questo tipo di record. Il valore "Unknown" indica che non è stato possibile determinare il servizio di origine.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>`ISFUSION`</td>
        <td>Booleano</td>
        <td>Flag che indica se questo tipo di record è stato creato o gestito tramite un’integrazione di Workfront Fusion. Il valore "true" indica la gestione di Fusion; "false" o un valore vuoto indica che si tratta di un tipo di record creato in modo nativo.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"CREATEDAT"</td>
        <td>Timestamp\_NTZ</td>
        <td>La marca temporale (senza fuso orario) di quando è stato creato questo tipo di record.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"CREATEDBY"</td>
        <td>Varchar</td>
        <td>Identificatore dell'utente che ha creato questo tipo di record.</td>
        <td>WF.USERS\_CORRENTE</td>
        <td>EAUTHUSERID</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"UPDATEDAT"</td>
        <td>Timestamp\_NTZ</td>
        <td>La marca temporale (nessun fuso orario) dell’ultimo aggiornamento di questo tipo di record.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"UPDATEDBY"</td>
        <td>Varchar</td>
        <td>Identificatore dell'ultimo utente che ha aggiornato questo tipo di record.</td>
        <td>WF.USERS\_CORRENTE</td>
        <td>EAUTHUSERID</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>'USERID'</td>
        <td>Varchar</td>
        <td>Identificatore dell'utente associato a questo tipo di record, in genere il proprietario.</td>
        <td>WF.USERS\_CORRENTE</td>
        <td>EAUTHUSERID</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>`TO_RECORDID`</td>
        <td>Varchar</td>
        <td>Identificatore univoco del record di Planning a cui appartiene questa connessione di riferimento. Chiave esterna di PLANNINGRECORD\_CURRENT.RECORDID.</td>
        <td>PLANNINGRECORD\_CURRENT</td>
        <td>RECORDID</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>'TO_EXTERNALID'</td>
        <td>Varchar</td>
        <td>Identificatore univoco dell'oggetto esterno a cui si fa riferimento (ad esempio, un ID progetto Workfront, un ID attività o un altro ID oggetto connesso).</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>'TO_EXTERNALCONNECTIONNAME'</td>
        <td>Varchar</td>
        <td>Il nome della connessione esterna attraverso la quale è connesso l'oggetto di riferimento (ad esempio, il nome della connessione Workfront configurata in Planning).</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>'TO_EXTERNALOBJECTNAME'</td>
        <td>Varchar</td>
        <td>Il codice oggetto API di Workfront per il tipo di oggetto esterno a cui si fa riferimento (ad esempio, "PROJ" per Progetto, "TASK" per Attività, "PORT" per Portfolio). Utilizzare questa opzione per determinare quale tabella Workfront unire quando si cerca l'oggetto di riferimento.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>'RECORDTYPEID'</td>
        <td>Varchar</td>
        <td>Identificatore univoco del tipo di record di Planning associato al record a cui appartiene questo riferimento. Chiave esterna di PLANNINGRECORD\_CURRENT.RECORDTYPEID.</td>
        <td>RECORDTYPE\_CURRENT</td>
        <td>ID</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"REFERENCEVALUE"</td>
        <td>Varchar</td>
        <td>Il nome visualizzato dell’oggetto esterno di riferimento all’ultimo aggiornamento dei dati (ad esempio, un nome di progetto Workfront come "Beta" o "Progetto dashboard Canvas"). Questo valore riflette il nome dell'oggetto al momento dell'aggiornamento e può diventare obsoleto se l'oggetto viene rinominato.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"CREATED"</td>
        <td>Numero</td>
        <td>Flag che indica l'ultimo tipo di operazione che ha interessato il record di riferimento. Il valore 1 indica che il riferimento è stato creato nel ciclo di aggiornamento dei dati più recente, mentre il valore 0 indica che non lo era.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"UPDATED"</td>
        <td>Numero</td>
        <td>Flag che indica l'ultimo tipo di operazione che ha interessato il record di riferimento. Il valore 1 indica che il riferimento è stato aggiornato nel ciclo di aggiornamento dei dati più recente; 0 indica che non lo era.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"DELETED"</td>
        <td>Numero</td>
        <td>Flag che indica se la connessione di riferimento è stata eliminata temporaneamente. Il valore 1 indica che il riferimento è stato eliminato, mentre 0 indica che è attivo.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>"DL_LOAD_TIMESTAMP"</td>
        <td>Timestamp\_NTZ</td>
        <td>La marca temporale del processo di aggiornamento dati che ha caricato per ultimo questo record di riferimento nel data lake. Aggiornato dopo ogni ciclo di aggiornamento dei dati riuscito.</td>
        <td>—</td>
        <td>—</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
</table>

### WORKSPACE\_CURRENT

Contiene le definizioni correnti di tutte le aree di lavoro di Workfront Planning. Ogni riga rappresenta un&#39;area di lavoro, inclusi il nome, la gerarchia e i metadati di proprietà. Utilizzare questa visualizzazione per risolvere gli ID del workspace da PLANNINGRECORD\_CURRENT e RECORDTYPE\_CURRENT in nomi di workspace leggibili dall&#39;utente.

<table>
    <tr>
        <td>Nome colonna</td>
        <td>Tipo</td>
        <td>Descrizione</td>
        <td>Tabella correlata</td>
        <td>Campo correlato</td>
    </tr>
    <tr>
        <td>"ID"</td>
        <td>Varchar</td>
        <td>Identificatore univoco per l'area di lavoro di Planning. Chiave primaria per questa visualizzazione.</td>
        <td>WF.WORKSPACES\_CURRENT</td>
        <td>ID</td>
    </tr>
    <tr>
        <td>"CREATED"</td>
        <td>Numero</td>
        <td>Flag che indica l'ultimo tipo di operazione che ha interessato il record dell'area di lavoro. Il valore 1 indica che l'area di lavoro è stata creata nel ciclo di aggiornamento dati più recente, mentre il valore 0 indica che non lo è stata. Consulta CREATEDAT per la marca temporale della creazione effettiva.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"UPDATED"</td>
        <td>Numero</td>
        <td>Flag che indica l'ultimo tipo di operazione che ha interessato il record dell'area di lavoro. Il valore 1 indica che l'area di lavoro è stata aggiornata nel ciclo di aggiornamento dati più recente, mentre il valore 0 indica che non lo era. Per la marca temporale effettiva dell’ultimo aggiornamento, consulta UPDATEDAT.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"DELETED"</td>
        <td>Numero</td>
        <td>Flag che indica se l'area di lavoro è stata eliminata temporaneamente. Il valore 1 indica eliminato, 0 indica attivo.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"DL_LOAD_TIMESTAMP"</td>
        <td>Timestamp\_NTZ</td>
        <td>La marca temporale del processo di aggiornamento dati che ha caricato per ultimo questo record dell’area di lavoro nel data lake. Aggiornato dopo ogni ciclo di aggiornamento dei dati riuscito.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"CREATEDBY"</td>
        <td>Varchar</td>
        <td>Identificatore dell'utente che ha creato l'area di lavoro.</td>
        <td>WF.USERS\_CORRENTE</td>
        <td>EAUTHUSERID</td>
    </tr>
    <tr>
        <td>"CREATEDAT"</td>
        <td>Timestamp\_NTZ</td>
        <td>La marca temporale (nessun fuso orario) di quando è stata creata l’area di lavoro.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"UPDATEDBY"</td>
        <td>Varchar</td>
        <td>Identificatore dell'ultimo utente che ha aggiornato l'area di lavoro.</td>
        <td>WF.USERS\_CORRENTE</td>
        <td>EAUTHUSERID</td>
    </tr>
    <tr>
        <td>"UPDATEDAT"</td>
        <td>Timestamp\_NTZ</td>
        <td>La marca temporale (nessun fuso orario) dell’ultimo aggiornamento di questa area di lavoro.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>'USERID'</td>
        <td>Varchar</td>
        <td>Identificatore dell'utente associato a questa area di lavoro, in genere il proprietario dell'area di lavoro.</td>
        <td>WF.USERS\_CORRENTE</td>
        <td>EAUTHUSERID</td>
    </tr>
    <tr>
        <td>"NAME"</td>
        <td>Varchar</td>
        <td>Il nome visualizzato dell'area di lavoro, come mostrato nell'interfaccia di Planning.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>'PARENTID'</td>
        <td>Varchar</td>
        <td>Identificatore dell'area di lavoro padre se quest'ultima è nidificata all'interno di una gerarchia di aree di lavoro. Vuoto se l'area di lavoro non ha un elemento padre (ad esempio, è un'area di lavoro di livello superiore).</td>
        <td>WORKSPACE\_CURRENT</td>
        <td>ID</td>
    </tr>
    <tr>
        <td>"RESTORED"</td>
        <td>Numero</td>
        <td>Flag che indica se l'area di lavoro è stata ripristinata dopo l'eliminazione temporanea.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>"TRIGGEREDBYSERVICE"</td>
        <td>Varchar</td>
        <td>Il nome del servizio o dell’integrazione che ha attivato l’ultima modifica a questo record dell’area di lavoro. Il valore "Unknown" indica che non è stato possibile determinare il servizio di origine.</td>
        <td>—</td>
        <td>—</td>
    </tr>
    <tr>
        <td>`ISFUSION`</td>
        <td>Booleano</td>
        <td>Flag che indica se l'area di lavoro è stata creata o gestita tramite un'integrazione di Workfront Fusion. Il valore "true" indica la gestione di Fusion; "false" o un valore vuoto indica che si tratta di un’area di lavoro creata in modo nativo.</td>
        <td>—</td>
        <td>—</td>
    </tr>
</table>
