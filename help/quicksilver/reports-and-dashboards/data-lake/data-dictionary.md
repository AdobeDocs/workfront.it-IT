---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Dizionario dati Workfront Data Connect
description: Questa pagina contiene informazioni sulla struttura e sul contenuto dei dati in Workfront Data Connect.
author: Nolan
feature: Reports and Dashboards
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '4294'
ht-degree: 4%

---

# Dizionario dati Workfront Data Connect

Questa pagina contiene informazioni sulla struttura e sul contenuto dei dati in Workfront Data Connect.

>[!NOTE]
>
>I dati in Data Connect vengono aggiornati ogni quattro ore, pertanto le modifiche recenti potrebbero non essere applicate immediatamente.

## Tipi di tabella

Esistono diversi tipi di tabelle che è possibile utilizzare in Data Connect per visualizzare i dati di Workfront in modo da fornire la maggior parte delle informazioni.

* **Tabella corrente**

  La tabella Current riflette i dati in modo simile a come esistono in Workfront, in ogni oggetto e nel relativo stato corrente. Tuttavia, può essere navigato con una latenza molto più bassa rispetto a Workfront.

* **Tabella eventi**

  La tabella Evento tiene traccia di ogni record di modifica in Workfront, ovvero ogni volta che un oggetto cambia stato, viene creato un record che mostra quando è avvenuta la modifica, chi ha apportato la modifica e cosa è stato modificato. Pertanto, questa tabella è utile per i confronti point-in-time. Questa tabella include solo i record degli ultimi tre anni.

* **Tabella cronologia giornaliera**

  La tabella Cronologia giornaliera offre una versione abbreviata della tabella Evento, in quanto mostra lo stato di ciascun oggetto su base giornaliera anziché nel momento in cui si è verificato ogni singolo evento. Pertanto, questa tabella è utile per l’analisi delle tendenze.

<!-- Custom table -->

## Diagramma relazioni entità

Gli oggetti in Workfront (e, pertanto, nel data lake di Data Connect) sono definiti non solo dai singoli valori, ma anche dalle relazioni con altri oggetti. Il diagramma delle relazioni tra entità riportato di seguito fornisce una mappatura di alto livello delle relazioni tra oggetti in Data Connect. Il diagramma può essere visualizzato e scaricato utilizzando il seguente collegamento:

[Diagramma delle relazioni tra entità di Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>Il diagramma delle relazioni tra entità è un work in progress, in quanto tale, è solo a scopo di riferimento ed è soggetto a modifiche.

## Tipi di date

Esistono diversi oggetti data che forniscono informazioni su quando si verificano eventi specifici.

* `DL_LOAD_TIMESTAMP`: questa data viene utilizzata come riferimento interno e indica quando i dati sono stati caricati nella tabella Cronologia corrente, evento o giornaliera. Questa data non deve essere utilizzata per l’analisi dei dati e deve essere rimossa durante la fase beta del data lake di Workfront.
* `CALENDAR_DATE`: data presente solo nella tabella Cronologia giornaliera. Questa tabella fornisce un record dell&#39;aspetto dei dati alle 11:59 UTC per ogni data specificata in `CALENDAR_DATE`.
* `BEGIN_EFFECTIVE_TIMESTAMP`: questa data è presente nelle tabelle Event e Daily History e registra esattamente quando un record ha cambiato _in_ il valore presente nella riga corrente.
* `END_EFFECTIVE_TIMESTAMP`: questa data è presente nelle tabelle Event e Daily History e registra esattamente quando un record ha cambiato _da_ il valore nella riga corrente a un valore in un&#39;altra riga. Per consentire l&#39;esecuzione di query tra `BEGIN_EFFECTIVE_TIMESTAMP` e `END_EFFECTIVE_TIMESTAMP`, questo valore non è mai nullo, anche se non è presente un nuovo valore. Se un record è ancora valido (ovvero se il valore non è stato modificato), `END_EFFECTIVE_TIMESTAMP` avrà il valore 2300-01-01.

## Tabella terminologica

La tabella seguente mette in correlazione i nomi degli oggetti in Workfront (nonché i relativi nomi nell’interfaccia e nell’API) con i nomi equivalenti in Data Connect.

<table>
  <thead>
    <tr>
        <th>Nome entità Workfront</th>
        <th>Riferimenti interfaccia</th>
        <th>Riferimento API | Etichetta</th>
        <th>Tabelle Data Lake</th>
        <th>Campo Relazioni</th>
        <th>Tabella relazioni e campo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td>Livello di accesso</td>
        <td>Livello di accesso</td>
        <td>ACSLVL | Livello d'Accesso</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        <td>ACCESSLEVELID (self)<br>APPGLOBALID<br>LASTUPDATEDBYID<br>LEGACYACCESSLEVELID<br>OBJID<br>SYSID</td>
        <td>Self<br>Non è una relazione; utilizzato per scopi interni dell'applicazione<br>USER_CURRENT | USERID<br>Non è una relazione; utilizzato per scopi interni all'applicazione<br>L'ID dell'oggetto identificato nel campo OBJCODE<br>Non è una relazione; utilizzato per scopi interni all'applicazione</td>
    </tr>
    <tr>
        <td>Regola di accesso</td>
        <td>Condividi</td>
        <td>ACSRUL | Condividi</td>
        <td>ACCESSRULES_CURRENT<br>ACCESSRULES_DAILY_HISTORY<br>ACCESSRULES_EVENT</td>
        <td>ACCESSORID <br>ACCESSRULEID (self) <br>ANCESTORID <br>LASTUPDATEDBYID <br>SECURITYOBJID <br>SYSID</td>
        <td>ID dell'oggetto identificato nel campo ACCESSOROBJCODE<br>Self<br>ID dell'oggetto identificato nel campo ANCESTOROBJCODE<br>USERS_CURRENT | USERID<br>L'ID dell'oggetto identificato nel campo SECURITYOBJCODE<br>Non è una relazione; viene utilizzato per scopi interni all'applicazione</td>
    </tr>
    <tr>
        <td>Percorso di approvazione</td>
        <td>Percorso di approvazione</td>
        <td>ARVPTH | Approvazione</td>
        <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        <td>APPROVALPATHID (self) <br>APPROVALPROCESSID <br>ENTEREDBYID <br>GLOBALPATHID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>Self<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>Non è una relazione; utilizzato per scopi interni all'applicazione<br>USERS_CURRENT | USERID<br>Non è una relazione; utilizzato per scopi interni all'applicazione</td>
    </tr>
    <tr>
        <td>Processo di approvazione</td>
        <td>Processo di approvazione</td>
        <td>ARVPRC | Processo di approvazione</td>
        <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        <td>APPROVALPROCESSID (self) <br>ENTEREDBYID <br>LASTUPDATEDBYID<br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>Non è una relazione; utilizzato per scopi interni all'applicazione</td>
    </tr>
    <tr>
        <td>Passaggio di approvazione</td>
        <td>Passaggio di approvazione</td>
        <td>ARVSTP | Fase di approvazione</td>
        <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        <td>APPROVALPATHID <br>APPROVALSTEPID (self) <br>SYSID</td>
        <td>APPROVALPATHS_CURRENT | APPROVALPATHID<br>Self<br>Non è una relazione; viene utilizzato per scopi interni all'applicazione</td>
    </tr>
    <tr>
        <td>ApproverStatus</td>
        <td>Stato approvatore</td>
        <td>ARVSTS | ApproverStatus</td>
        <td>APPROVERSTATUSES_CURRENT<br>APPROVERSTATUSES_DAILY_HISTORY<br>APPROVERSTATUSES_EVENT</td>
        <td>APPROVERSTATUSID (self)<br>APPROVABLEOBJID<br>APPROVALSTEPID<br>APPROVEDBYID <br>DELEGATEUSERID<br>LASTUPDATEDBYID <br>OPTASKID<br>OVERRIDDENUSERID<br>PROJECTID<br>STEPAPPROVERID<br>SYSID<br>TASKID<br>WILDCARDUSERID</td>
        <td>Self<br>ID dell'oggetto identificato nel campo APPROVABLEOBJCODE<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USERS_CURRENT | ID UTENTE <br>UTENTI_CORRENTE | USERID<br>USERS_CURRENT | ID UTENTE <br>OPTASKS_CURRENT | OPTASKID<br>USERS_CURRENT | USERID<br>PROJECTS_CURRENT | PROJECTID<br>USERS_CURRENT | USERID<br>Non è una relazione; utilizzato per scopi interni all'applicazione<br>TASKS_CURRENT | TASKID<br>UTENTI_CORRENTE | USERID</td>
    </tr>
    <tr>
        <td>Assegnazione</td>
        <td>Assegnazione</td>
        <td>ASSEGNA | Assegnazione</td>
        <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDBYID<br>ASSIGNEDTOID<br>ASSIGNMENTID (self)<br>CATEGORYID<br>CLASSIFIERID<br>OPTASKID<br>PRIVATERATECARDID<br>PROJECTID<br>ROLEID<br>TASKID<br>TEAMID</td>
        <td>USER_CURRENT | USERID<br>UTENTE_CORRENTE | USERID<br>Self<br>CATEGORIES_CURRENT | CATEGORYID<br>Tabella classificatore non supportata al momento<br>OPTASK_CURRENT | OPTASKID<br>RATECARD_CURRENT | RATECARDID<br>PROJECT_CURRENT | PROJECTID<br>ROLE_CURRENT | ID RUOLO<br>ATTIVITÀ_CORRENTE | TASKID<br>TEAM_CURRENT | TEAM ID</td>
    </tr>
    <tr>
        <td>In attesa di approvazioni</td>
        <td>In attesa di approvazioni</td>
        <td>AWAPVL | In attesa di approvazione</td>
        <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        <td>ACCESSREQUESTID<br>APPROVABLEID <br>APPROVERID <br>AWAITINGAPPROVALID (self) <br>DOCUMENTID <br>DOCUMENTVERSIONID<br>OPTASKID <br>PROJECTID <br>ROLEID <br>SUBMITTEDBYID <br>SYSID<br>TASKID <br>TEAMID <br>TIMESHEETID<br>USERID</td>
        <td>La tabella delle richieste di accesso non è attualmente supportata<br>Non è una relazione; viene utilizzata per scopi interni all'applicazione<br>USERS_CURRENT | USERID<br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>DOCUMENTVERSIONS_CURRENT | DOCUMENTVERSIONID<br>OPTASKS_CURRENT | OPTASKID<br>PROJECTS_CURRENT | PROJECTID<br>ROLES_CURRENT | ID RUOLO<br>UTENTI_CORRENTE | USERID<br>Non è una relazione; utilizzato per scopi interni all'applicazione<br>TASKS_CURRENT | TASKID<br>TEAM_CORRENTE | TEAMID<br>SCHEDE ORARIO_CORRENTE | TIMESHEETID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Linea di base</td>
        <td>Linea di base</td>
        <td>CIECO | Linea di base</td>
        <td>BASELINES_CURRENT<br>BASELINES_DAILY_HISTORY<br>BASELINES_EVENT</td>
        <td>BASELINEID (self)<br>EXCHANGERATEID <br>PROJECTID <br>SYSID</td>
        <td>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>Non è una relazione; utilizzato per scopi interni all'applicazione</td>
    </tr>
    <tr>
        <td>Attività linea di base</td>
        <td>Attività linea di base</td>
        <td>BSTSK | Attività linea di base</td>
        <td>BASELINETASKS_CURRENT<br>BASELINETASKS_DAILY_HISTORY<br>BASELINETASKS_EVENT</td>
        <td>BASELINEID<br>BASELINETASKID (self) <br>EXCHANGERATEID <br>PROJECTID <br>SYSID<br>TASKID</td>
        <td>BASELINES_CURRENT | BASELINEID<br>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>Non è una relazione; utilizzato per scopi interni all'applicazione<br>TASKS_CURRENT | TASKID</td>
    </tr>
    <tr>
        <td>Tariffa di fatturazione</td>
        <td>Tasso o tasso di sostituzione</td>
        <td>TARIFFA | Tariffa di fatturazione</td>
        <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        <td>ASSIGNMENTID<br>CLASSIFIERID<br>EXCHANGERATEID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID <br>RATECARDID<br>RATEID (self)<br>ROLEID <br>SOURCERATECARDID <br>SYSID <br>TEMPLATEID<br>USERID</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>Tabella classificatore non supportata al momento<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>Tabella delle categorie di risorse non manodopera attualmente non supportata<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>ID dell'oggetto identificato nel campo OBJCODE<br>PROJECTS_CURRENT | PROJECTID <br>RATECARD_CURRENT | RATECARDID<br>Self<br>ROLES_CURRENT | ID RUOLO <br>RATECARD_CURRENT | RATECARDID <br>Non è una relazione. Utilizzato per applicazioni interne <br>TEMPLATES_CURRNT | TEMPLATEID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Fatturazione</td>
        <td>Fatturazione</td>
        <td>FATTURA | Fatturazione</td>
        <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        <td>BILLINGRECORDID (self)<br>IDCATEGORIA<br>EXCHANGERATEID <br>IDFATTURA <br>IDAGGIORNAMENTOATTIVITÀBYID <br>IDPROGETTO <br>SID</td>
        <td>Self<br>CATEGORIES_CURRENT | CATEGORYID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>Tabella fatture non supportata attualmente <br>USERS_CURRENT | ID UTENTE <br>PROGETTI_CORRENTE | PROJECTID   <br>Nessuna relazione; utilizzato per scopi interni all'applicazione</td>
    </tr>
    <tr>
        <td>Prenotazione</td>
        <td>Prenotazione</td>
        <td>PRENOTAZIONE | Prenotazione</td>
        <td>BOOKINGS_CURRENT<br>BOOKINGS_DAILY_HISTORY<br>BOOKINGS_EVENT</td>
        <td>BOOKINGID (self)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>Tabella categorie risorse non manodopera non supportata al momento<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>ID dell'oggetto identificato nel campo OBJOBJCODE<br>PROJECTS_CURRENT | PROJECTID <br>Non è una relazione; viene utilizzato per scopi interni all'applicazione<br>TASKS_CURRENT | TASKID     <br>MODELLI_CORRENTI | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>ID dell'oggetto identificato nel campo TOPOBJCODE.</td>
    </tr>
    <tr>
        <td>Categoria</td>
        <td>Modulo personalizzato</td>
        <td>CITTÀ | Categoria</td>
        <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        <td>CATEGORYID (self)<br>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID <br>UTENTI_CORRENTE | USERID <br>Non è una relazione; utilizzato per scopi interni all'applicazione</td>
    </tr>
    <tr>
        <td>Parametro di Categoria</td>
        <td>Campi modulo personalizzati</td>
        <td>CTGYPA | Parametro di Categoria</td>
        <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        <td>CATEGORIESPARAMETERID (self)<br>CATEGORYID<br>PARAMETERGROUPID<br>PARAMETERID    <br>SYSID</td>
        <td>Self<br>CATEGORIES_CURRENT | CATEGORYID<br>Tabella di gruppi di parametri non supportata al momento<br>PARAMETERS_CURRENT | PARAMETERID    <br>Nessuna relazione; utilizzato per scopi interni all'applicazione</td>
    </tr>
    <tr>
        <td>Azienda</td>
        <td>Azienda</td>
        <td>AZIENDA | Azienda</td>
        <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        <td>CATEGORYID<br>COMPANYID (self)<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>PRIVATERATECARDID<br>SYSID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | ID UTENTE <br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | ID UTENTE <br>RATECARD_CURRENT | RATECARDID<br>Non è una relazione; utilizzato per scopi interni all'applicazione</td>
    </tr>
    <tr>
        <td>Trimestre personalizzato</td>
        <td>Trimestre personalizzato</td>
        <td>CSTQR | Trimestre personalizzato</td>
        <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        <td>CUSTOMQUARTERID (self) <br>SYSID</td>
        <td>Self<br>Non è una relazione; utilizzato per scopi interni dell'applicazione</td>
    </tr>
    <tr>
        <td>EnumPersonalizzata</td>
        <td>Condizione, Priorità, Gravità, Stato</td>
        <td>CSTEM | Enum personalizzata</td>
        <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT<br>* Il tipo di record è identificato tramite la proprietà `enumClass`. I tipi previsti sono:<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
        <td>ENTEREDBYID<br>GROUPID</td>
        <td>USER_CURRENT | USERID<br>GRUPPO_CORRENTE | GROUPID</td>
    </tr>
    <tr>
        <td>Documento</td>
        <td>Documento</td>
        <td>DOCU | Documento</td>
        <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>CHECKEDOUTBYID<br>DOCUMENTID<br>DOCUMENTREQUESTID<br>EXCHANGERATEID<br>ITERATIONID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>RELEASEVERSIONID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID 18}TOPOBJID<br>USERID<br></td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>UTENTE_CORRENTE | USERID<br>Self<br>Tabella richieste documenti non supportata al momento<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>NOTE_CURRENT | NOTEID<br>UTENTE_CORRENTE | USERID<br>NOTE_CURRENT | NOTEID<br>Variabile a seconda del valore DOCOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>UTENTE_CORRENTE | USERID<br>PORTFOLIO_CORRENTE | PORTFOLIOID<br>PROGRAMMA_CORRENTE | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Tabella delle versioni di rilascio non supportata al momento<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>Variabile a seconda del valore TOPOBJCODE<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Approvazione documento</td>
        <td>Approvazione documento</td>
        <td>DOCAPL | Approvazione documento</td>
        <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        <td>APPROVERID<br>DOCAPPROVALID (self)<br>DOCUMENTID<br>NOTEID<br>REQUESTORID<br>SYSID</td>
        <td>USERS_CURRENT | ID UTENTE <br>Autonomo<br>DOCUMENTI_CORRENTE | DOCUMENTID<br>NOTES_CURRENT | NOTEID<br>UTENTI_CORRENTE | USERID <br>Non è una relazione; utilizzato per scopi interni all'applicazione</td>
    </tr>
    <tr>
        <td>Cartella documenti</td>
        <td>Cartella documenti</td>
        <td>DOCFLD | DocsFolders</td>
        <td>DOCFOLDERS_CURRENT<br>DOCFOLDERS_DAILY_HISTORY<br>DOCFOLDERS_EVENT</td>
        <td>DOCFOLDERID (self)<br>ENTEREDBYID<br>ISSUEID<br>ITERATIONID    <br>LINKEDFOLDERID<br>PARENTID<br>PORTFOLIOID <br>PROGRAMID    <br>PROJECTID<br>SYSID<br>TASKID     <br>TEMPLATEID<br>TEMPLATETASKID<br>USERID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>OPTASKS_CURRENT | OPTASKID<br>ITERATIONS_CURRENT | ITERATIONID<br>LINKEDFOLDERS_CURRENT | LINKEDFOLDERID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>PORTFOLIO_CORRENTE | PORTFOLIOID <br>PROGRAMMA_CORRENTE | PROGRAMID    <br>PROGETTI_ATTUALI | PROJECTID <br>Non è una relazione; viene utilizzato per scopi interni all'applicazione<br>TASKS_CURRENT | TASKID     <br>MODELLI_CORRENTI | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>DocumentProvideMetadata</td>
        <td>Fornisci metadati documento</td>
        <td>DOCMET | DocumentProviderMetadata</td>
        <td>DOCPROVIDERMETA_CURRENT<br>DOCPROVIDERMETA_DAILY_HISTORY<br>DOCPROVIDERMETA_EVENT</td>
        <td>DOCPROVIDERMETAID (self) <br>SYSID</td>
        <td>Self<br>Non è una relazione; utilizzato per scopi interni dell'applicazione</td>
    </tr>
    <tr>
        <td>DocumentProvider</td>
        <td>Provider documento</td>
        <td>DOCPRO | Provider documento</td>
        <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        <td>DOCPROVIDERCONFIGID<br>DOCPROVIDERID (self)<br>OWNERID    <br>SYSID</td>
        <td>DOCPROVIDERCONFIG_CURRENT | DOCPROVIDERCONFIGID<br>Self<br>USERS_CURRENT | USERID    <br>Nessuna relazione; utilizzato per scopi interni all'applicazione</td>
    </tr>
    <tr>
        <td>DocumentProviderConfig</td>
        <td>Configurazione provider documenti</td>
        <td>DOCCFG | DocumentProviderConfig</td>
        <td>DOCPROVIDERCONFIG_CURRENT<br>DOCPROVIDERCONFIG_DAILY_HISTORY<br>DOCPROVIDERCONFIG_EVENT</td>
        <td>DOCPROVIDERCONFIGID (self)<br>SYSID</td>
        <td>Self<br>Non è una relazione; utilizzato per scopi interni dell'applicazione</td>
    </tr>
    <tr>
        <td>DocumentVersion</td>
        <td>Versione documento</td>
        <td>DOCV | Versione documento</td>
        <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        <td>DOCUMENTID<br>DOCUMENTPROVIDERID<br>DOCUMENTVERSIONID<br>ENTEREDBYID<br>EXTERNALSTORAGEID<br>PROOFAPPROVALSTATUSID<br>PROOFEDBYUSERID<br>PROOFID<br>PROOFOWNERID<br>PROOFSTAGEID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>DOCPROVIDERS_CURRENT | DOCUMENTPROVIDERID<br>Self<br>USER_CURRENT | USERID<br>ID esterno<br>Tabella dello stato di approvazione della bozza non supportata al momento<br>USER_CURRENT | USERID<br>Tabella bozza non supportata al momento<br>USER_CURRENT | USERID<br>Tabella fase bozza non supportata al momento</td>
    </tr>
    <tr>
        <td>Tasso di cambio</td>
        <td>Tasso di cambio</td>
        <td>ESAURIRE | Tasso di cambio</td>
        <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        <td>EXCHANGERATEID (self)<br>PROJECTID<br>SYSID <br>TEMPLATEID  </td>
        <td>Self<br>PROJECTS_CURRENT | PROJECTID <br>Non è una relazione; utilizzato per scopi interni dell'applicazione <br>TEMPLATES_CURRENT | TEMPLATEID  </td>
    </tr>
    <tr>
        <td>Spesa</td>
        <td>Spesa</td>
        <td>EXPNS | Spesa</td>
        <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        <td>BILLINGRECORDID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID <br>EXPENSEID (self) <br>EXPENSETYPEID <br>LASTUPDATEDBYID <br>OBJID <br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>Self <br>EXPENSETYPES_CURRENT | EXPENSETYPEID <br>UTENTI_CORRENTE | ID UTENTE <br>ID dell'oggetto identificato nel campo OBJCODE <br>PROJECTS_CURRENT | PROJECTID <br>Non è una relazione; viene utilizzato per scopi interni all'applicazione<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>ID dell'oggetto identificato nel campo TOPOBJCODE</td>
    </tr>
    <tr>
        <td>Tipo di spesa</td>
        <td>Tipo di spesa</td>
        <td>EXPTYP | Tipo di Spesa</td>
        <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        <td>APPGLOBALID<br>EXPENSETYPEID (self)<br>OBJID <br>SYSID  </td>
        <td>Non una relazione; utilizzato per scopi interni all'applicazione<br>Self<br>L'ID dell'oggetto identificato nel campo OBJCODE <br>Not a relationship; utilizzato per scopi interni all'applicazione  </td>
    </tr>
    <tr>
        <td>Gruppo</td>
        <td>Gruppo</td>
        <td>GRUPPO | Gruppo</td>
        <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        <td>BUSINESSLEADERID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>PARENTID<br>ROOTID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>UTENTE_CORRENTE | USERID<br>Self<br>Layout Template Table non supportato<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>UITEMPLATES_CURRENT | UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Ora</td>
        <td>Ora</td>
        <td>ORA | Hour</td>
        <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        <td>APPROVEDBYID<br>BILLINGRECORDID<br>CATEGORYID<br>CLASSIFIERID<br>DUPID<br>EXCHANGERATEID<br>EXTERNALTIMESHEETID<br>HOURID<br>HOURTYPEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>PROJECTOVERHEADID<br>ROLEID<br>TASKID<br>TIMESHEETID</td>
        <td>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>Tabella classificatore non supportata al momento<br>Nessuna relazione; utilizzata per scopi interni dell'applicazione<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>Non è una relazione Workfront; utilizzato per l'integrazione con sistemi esterni<br>Self<br>HOURTYPE_CURRENT | HOURTYPEID<br>UTENTE_CORRENTE | USERID<br>OPTASK_CURRENT | OPTASKID<br>UTENTE_CORRENTE | USERID<br>PROJECT_CURRENT | PROJECTID<br>Non è una relazione; viene utilizzato per scopi interni all'applicazione<br>ROLE_CURRENT | ROLEID<br>ATTIVITÀ_CORRENTE | TASKID<br>TIMESHEET_CURRENT | TIMESHEETID</td>
    </tr>
    <tr>
        <td>Tipo di ora</td>
        <td>Tipo di ora</td>
        <td>ORA | Tipo di Ora</td>
        <td>HOURTYPES_CURRENT</td>
        <td>APPGLOBALID<br>HOURTYPEID<br>OBJID</td>
        <td>Non una relazione; utilizzato per scopi interni dell'applicazione<br>Autonomo<br>Non una relazione; utilizzato per scopi interni dell'applicazione</td>
    </tr>
    <tr>
        <td>Iterazione</td>
        <td>Iterazione</td>
        <td>ITRN | Iterazione</td>
        <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>ITERATIONID (self)<br>LASTUPDATEDBYID<br>OWNERID<br>SYSID<br>TEAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | ID UTENTE <br>Self<br>USERS_CURRENT | ID UTENTE <br>UTENTI_CORRENTE | USERID <br>Non è una relazione; utilizzato per scopi interni all'applicazione<br>TEAMS_CURRENT | TEAM ID</td>
    </tr>
    <tr>
        <td>Voce del diario</td>
        <td>Voce del diario</td>
        <td>GERGO | Voce diario</td>
        <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        <td>APPROVERSTATUSID<br>ASSIGNMENTID<br>AUDITRECORDID<br>BASELINEID <br>BILLINGRECORDID<br>COMPANYID <br>DOCUMENTID <br>DOCUMENTSHAREID <br>EDITEDBYID<br>EXPENSEID<br>HOURID<br>INITIATIVEID<br>JOURNALENTRIEID (self)<br>OBJID<br>OPTASKID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>SUBOBJID<br>SUBSCRIPTID ID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TIMESHEETID<br>TOPOBJID<br>USERID</td>
        <td>APPROVERSTATUSES_CURRENT | APPROVERSTATUSID<br>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>Tabella record di controllo non supportata al momento<br>BASELINES_CURRENT | BASELINEID <br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENTI_CORRENTI | La tabella di condivisione documenti <br>ID documento non è attualmente supportata <br>USERS_CURRENT | ID UTENTE<br>SPESE_CORRENTE | EXPENSEID<br>HOURS_CURRENT | HOURID<br>Tabella iniziativa non supportata al momento<br>Self<br>ID dell'oggetto identificato nel campo OBJCODE<br>OPTASKS_CURRENT | OPTASKID<br>PORTFOLIO_CORRENTE | PORTFOLIOID<br>PROGRAMMA_CORRENTE | PROGRAMID<br>PROJECTS_CURRENT | PROJECTID <br>L'ID dell'oggetto identificato nel campo SUBOBJCODE<br>Tabella di sottoscrizione non supportata al momento<br>Nessuna relazione. Utilizzato per applicazioni interne<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>ID dell'oggetto identificato nel campo TOPOBJCODE<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>LinkedFolder</td>
        <td>LinkedFolder</td>
        <td>LNKFDR | LinkedFolder</td>
        <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        <td>DOCUMENTPROVIDERID<br>EXTERNALSTORAGEID<br>FOLDERID<br>LINKEDBYID<br>LINKEDFOLDERID (self)<br>SYSID</td>
        <td>DOCPROVIDERS_CURRENT | DOCPROVIDERID<br>ID esterno<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>USERS_CURRENT | USERID <br>Autonomo<br>Non è una relazione; viene utilizzato per scopi interni all'applicazione  </td>
    </tr>
    <tr>
        <td>Milestone</td>
        <td>Milestone</td>
        <td>MIGLIA | Milestone</td>
        <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
        <td>LASTUPDATEDBYID<br>MILESTONEID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>Self<br>MILESTONEPATH_CURRENT | MILESTONEID</td>
    </tr>
    <tr>
        <td>PercorsoMilestone</td>
        <td>Percorso milestone</td>
        <td>MPATH | Percorso milestone</td>
        <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>UTENTE_CORRENTE | USERID<br>Self</td>
    </tr>
    <tr>
        <td>NonLaborResource</td>
        <td>Risorsa non di manodopera</td>
        <td>NLBR | Risorsa non manodopera</td>
        <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        <td>CATEGORYID<br>NONLABORRESOURCEID (self)<br>ENTEREDBYID<br>HOMEGROUPID<br>LASTUPDATEDBYID<br>NONLABORRESOURCECATEGORYID <br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | ID UTENTE <br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID <br>Tabella delle categorie di risorse non manodopera non supportata al momento <br>Nessuna relazione. Utilizzata per applicazioni interne    </td>
    </tr>
    <tr>
        <td>Giorno non feriale</td>
        <td>Eccezione Schedule</td>
        <td>NON WKD | Giorno non feriale</td>
        <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        <td>NONWORKDAYID (self)<br>OBJID <br>SCHEDULEID <br>SYSID <br>USERID  </td>
        <td>Self<br>ID dell'oggetto identificato nel campo OBJCODE <br>SCHEDULES_CURRENT | SCHEDULEID <br>Non è una relazione; utilizzato per scopi interni dell'applicazione <br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Nota</td>
        <td>Nota</td>
        <td>NOTA | Nota</td>
        <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        <td>ATTACHDOCUMENTID<br>ATTACHOBJID<br>ATTACHOPTASKID<br>ATTACHWORKID<br>ATTACHWORKUSERID<br>AUDITRECORDID<br>COMPANYID<br>DOCUMENTID<br>EXTERNALSERVICEID<br>ITERATIONID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PARENTENDORSEMENTID<br>PARENTJOURNALENTRYID<br>PARENTNOTEID<br>PORTAFOGLIO{17 PROGRAMID<br>PROJECTID<br>PROOFACTIONID<br>PROOFID<br>RICHTEXTNOTEID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>THREADID<br>TIMESHEETID<br>TOPOBJID<br>USERID<br></td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>Variabile a seconda di ATTACHOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>ELEMENTI DI LAVORO_CORRENTE<br>UTENTE_CORRENTE | USERID<br>Tabella record di controllo non supportata al momento<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENTO_CORRENTE | DOCUMENTID<br>Relazione non Workfront; utilizzato per l'integrazione con sistemi esterni<br>ITERATIONS_CURRENT | ITERATIONID<br>Self<br>Variabile a seconda di NOTEOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>UTENTE_CORRENTE | USERID<br>Tabella di verifica non supportata al momento<br>JOURNALENTRIES_CURRENT | JOURNALENTRYID<br>NOTE_CURRENT | NOTEID<br>PORTFOLIO_CORRENTE | PORTFOLIOID<br>PROGRAMMA_CORRENTE | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Tabella azione bozza non supportata al momento<br>Tabella bozza non supportata al momento<br>RESERVEDTEXTNOTES_CURRENT | RICHTEXTNOTEID<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>NOTA_CORRENTE | NOTEID<br>TIMESHEET_CURRENT | TIMESHEETID<br>Variabile che dipende da TOPOBJCODE<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Integrazione degli oggetti</td>
        <td>Integrazione degli oggetti</td>
        <td>OGGETTO | IntegrazioneOggetti</td>
        <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        <td>LINKEDOBJECTID<br>OBJECTINTEGRATIONID   (self)<br>OBJID <br>SYSID  </td>
        <td>L'ID dell'oggetto identificato nel campo LINKEDOBJECTCODE <br>Self<br>L'ID dell'oggetto identificato nel campo OBJCODE <br>Not a relationship; utilizzato per scopi interni all'applicazione  </td>
    </tr>
    <tr>
        <td>Categoria oggetti</td>
        <td>Categorie di oggetti</td>
        <td>OBJCAT | Categoria oggetto</td>
        <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        <td>CATEGORYID<br>OBJECTSCATEGORYID (self)<br>OBJID <br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>L'ID dell'oggetto identificato nel campo OBJCODE <br>Non è una relazione; viene utilizzato per scopi interni all'applicazione  </td>
    </tr>
    <tr>
        <td>OpTask</td>
        <td>Problema, richiesta</td>
        <td>OPTASK | Problema</td>
        <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>QUEUEDEFID<br>QUEUETOPICID<br>RESOLVEOPTASKID 16}RESOLVEPROJECTID<br>RESOLVETASKID<br>RESOLVINGOBJID<br>ROLEID<br>SOURCEOBJID<br>SOURCETASKID<br>SUBMITTEDBYID<br>TEAMID<br></td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>UTENTE_CORRENTE | USERID<br>CATEGORIES_CURRENT | IDCATEGORIA<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>UTENTE_CORRENTE | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>Tabella Kanban Board non supportata al momento<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>UTENTE_CORRENTE | USERID<br>Self<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>Tabella di definizione coda non supportata al momento<br>Tabella di argomenti coda non supportata al momento<br>OPTASK_CURRENT | OPTASKID<br>PROJECT_CURRENT | PROJECTID<br>TASK_CURRENT | TASKID<br>Variabile a seconda di RESOLVINGOBJCODE<br>ROLE_CURRENT | ROLEID<br>Variabile a seconda di SOURCEOBJCODE<br>TASK_CURRENT | TASKID<br>UTENTE_CORRENTE | USERID<br>TEAM_CURRENT | TEAM ID</td>
    </tr>
    <tr>
        <td>Parametro</td>
        <td>Campo personalizzato</td>
        <td>PARAM | Parametro</td>
        <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY<br>PARAMETERS_EVENT</td>
        <td>LASTUPDATEDBYID<br>PARAMETERFILTERID<br>PARAMETERID (self)<br>SYSID  </td>
        <td>USERS_CURRENT | USERID<br>La tabella dei filtri dei parametri non è attualmente supportata<br>Self<br>Not a relationship; utilizzata per scopi interni all'applicazione  </td>
    </tr>
    <tr>
        <td>Opzione Parametro</td>
        <td>Opzione Parametro</td>
        <td>POPT | Opzione Parametro</td>
        <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        <td>PARAMETERID<br>PARAMETEROPTIONID (self) <br>SYSID  </td>
        <td>PARAMETERS_CURRENT | PARAMETERID <br>Self <br>Non è una relazione; utilizzato per scopi interni dell'applicazione  </td>
    </tr>
    <tr>
        <td>Sezione portale</td>
        <td>Rapporto</td>
        <td>PTLSEC | Report</td>
        <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID<br>FILTERID<br>GROUPBYID<br>LASTUPDATEDBYID<br>LASTVIEWEDBYID<br>OBJID<br>PORTALSECTIONID (self)<br>PREFERENCEID<br>PUBLICRUNASUSERID<br>REPORTFOLDERID<br>RUNASUSERID<br>SCHEDULEDREPORTID<br>SYSID<br>VIEWID</td>
        <td>Non è una relazione; utilizzato per scopi interni all'applicazione <br>USERS_CURRENT | ID UTENTE <br>UIFILTERS_CURRENT | FILTERID<br>UIGROUPBYS_CURRENT | GROUPBYID<br>USERS_CURRENT | ID UTENTE <br>UTENTI_CORRENTE | ID UTENTE <br>ID dell'oggetto identificato nel campo OBJOBJCODE<br>Self<br>PREFERENCES_CURRENT | PREFERENCEID<br>USERS_CURRENT | ID UTENTE <br>REPORTFOLDERS_CURRENT | REPORTFOLDERID<br>USERS_CURRENT | USERID <br>Tabella dei report pianificati non supportata al momento<br>Nessuna relazione; utilizzata per applicazioni interne <br>UIVIEWS_CURRENT | VIEWID</td>
    </tr>
    <tr>
        <td>Scheda Portale</td>
        <td>Dashboard</td>
        <td>PTLTAB | Dashboard</td>
        <td>PORTALTABS_CURRENT<br>PORTALTABS_DAILY_HISTORY<br>PORTALTABS_EVENT</td>
        <td>DOCID<br>LASTUPDATEDBYID<br>PORTALPROFILEID<br>PORTALTABID (self)<br>SYSID<br>USERID</td>
        <td>Non è una relazione; utilizzato per scopi interni all'applicazione <br>USERS_CURRENT | USERID <br>La tabella Portal Profile non sarà supportata <br>Self<br>Not a relationship; utilizzata per scopi interni all'applicazione <br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>La Sezione della Liguetta Portale</td>
        <td>Sezione Cruscotto</td>
        <td>PRTBSC | Sezione scheda portale</td>
        <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        <td>CALENDARPORTALSECTIONID<br>EXTERNALSECTIONID<br>INTERNALSECTIONID <br>PORTALSECTIONOBJID <br>PORTALTABID<br>PORTALTABSECTIONID (self)<br>SYSID</td>
        <td>Sezione portale calendari non supportata al momento<br>Tabella sezioni esterne non supportata al momento<br>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>ID dell'oggetto identificato nel campo PORTALSECTIONOBJCODE<br>PORTALTABS_CURRENT | PORTALTABID<br>Autonomo<br>Nessuna relazione; utilizzato per scopi interni all'applicazione</td>
    </tr>
    <tr>
        <td>PortalSectionLastViewer</td>
        <td>Ultimi visualizzatori report</td>
        <td>PLSLSV | PortalSectionLastViewer</td>
        <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        <td>REPORTID<br>REPORTLASTVIEWERID (self)<br>SYSID<br>VIEWERID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>REPORTLASTVIEWERID (self)<br>Nessuna relazione; utilizzato a scopo di applicazione interna<br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Portfolio</td>
        <td>Portfolio</td>
        <td>PORTA | Portfolio</td>
        <td>PORTFOLI_CORRENTI<br>PORTFOLI_CRONOLOGIA_GIORNALIERA<br>PORTFOLI_EVENTI<br>PORTFOLI_VALORE_PERSONALIZZATO_CORRENTE<br>PORTFOLI_VALORE_PERSONALIZZATO_CRONOLOGIA_GIORNALIERA<br>PORTFOLI_VALORE_PERSONALIZZATO_EVENTO</td>
        <td>ALIGNMENTSCORECARDID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID</td>
        <td>Tabella scorecard non supportata al momento<br>CATEGORIES_CURRENT | CATEGORYID<br>UTENTE_CORRENTE | USERID<br>GROUP_CURRENT | GROUPID<br>UTENTE_CORRENTE | USERID<br>UTENTE_CORRENTE | USERID<br>Self</td>
    </tr>
    <tr>
        <td>Preferenza</td>
        <td>Visualizzazione, filtro, raggruppamento, definizione report</td>
        <td>PROSET | Preferenza</td>
        <td>PREFERENCES_CURRENT<br>PREFERENCES_DAILY_HISTORY<br>PREFERENCES_EVENT</td>
        <td>APPGLOBALID<br>PREFERENCEID (self) <br>SYSID  </td>
        <td>Non una relazione; utilizzato per scopi interni all'applicazione<br>Autonomo <br>Non una relazione; utilizzato per scopi interni all'applicazione  </td>
    </tr>
    <tr>
        <td>Programma</td>
        <td>Programma</td>
        <td>PRGM | Programma</td>
        <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>UTENTE_CORRENTE | USERID<br>GROUP_CURRENT | GROUPID<br>UTENTE_CORRENTE | USERID<br>UTENTE_CORRENTE | USERID<br>PORTFOLIO_CORRENTE | PORTFOLIOID<br>Self</td>
    </tr>
    <tr>
        <td>Progetto</td>
        <td>Progetto</td>
        <td>PROJ | Progetto</td>
        <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
        <td>AEMNATIVEFOLDERTREESREFID<br>ALIGNMENTSCORECARDID<br>APPROVALPROCESSID<br>ATTACHEDRATECARDID<br>CATEGORYID<br>COMPANYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>DELIVERABLESCORECARDID<br>ENTEREDBYID<br>GROUPID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>ESTONEPATHID<br>OWNERID<br>POPACCOUNTID<br>PORTFOLIOID<br>PRIVATERATECARDID<br>PROGRAMID<br>PROJECTID<br>QUEUEDEFID<br>REJECTIONISSUEID<br>RESOURCEPOOLID<br>SCHEDULEID<br>SPONSORID<br>SUBMITTEDBYID<br>TEAMID<br>TEMPLATEID</td>
        <td>Relazione non Workfront; utilizzata per l'integrazione con sistemi esterni<br>La tabella delle scorecard non è attualmente supportata<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>RATECARD_CURRENT | RATECARDID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>OPTASK_CURRENT | OPTASKID<br>UTENTE_CORRENTE | ID UTENTE<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>Tabella scorecard non supportata al momento<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>UTENTE_CORRENTE | ID UTENTE<br>MILESTONEPATH_CURRENT | MILESTONEPATHID<br>UTENTE_CORRENTE | USERID<br>Tabella account POP non supportata al momento<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | PROGRAMID<br>Self<br>Tabella di definizione coda non supportata al momento<br>OPTASK_CURRENT | OPTASKID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>SCHEDULE_CURRENT | SCHEDULEID<br>UTENTE_CORRENTE | ID UTENTE<br>UTENTE_CORRENTE | USERID<br>TEAM_CURRENT | TEAMID<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>RateCard</td>
        <td>Scheda tariffa</td>
        <td>RTCRD |Biglietto tariffa</td>
        <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>LASTUPDATEDBYID <br>RATECARDID (self) <br>SECURITYROOTID <br>SOURCEID<br>SYSID</td>
        <td>CATEGORYID<br>USERS_CURRENT | ID UTENTE <br>UTENTI_CORRENTE | USERID    <br>Autonomo<br>ID dell'oggetto identificato nel campo SECURITYOBJCODE <br>ID dell'oggetto identificato nel campo SOURCEOBJCODE<br>Nessuna relazione, utilizzato per scopi interni all'applicazione  </td>
    </tr>
    <tr>
        <td>Cartella Report</td>
        <td>Cartella Report</td>
        <td>RPTFDR | Cartella report</td>
        <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        <td>REPORTFOLDERID (self) <br>SYSID  </td>
        <td>Autonomo <br>Non è una relazione; utilizzato per scopi interni all'applicazione  </td>
    </tr>
    <tr>
        <td>Tempo riservato</td>
        <td>Indisponibilità (personale)</td>
        <td>RESVT | Indisponibilità</td>
        <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        <td>RESERVEDTIMEID (self) <br>SYSID<br>TASKID<br>USERID  </td>
        <td>Self<br>Non è una relazione; utilizzato per scopi interni dell'applicazione<br>TASKS_CURRENT | TASKID<br>UTENTI_CORRENTE | USERID  </td>
    </tr>
    <tr>
        <td>Gruppo di risorse</td>
        <td>Gruppo di risorse</td>
        <td>RSPL | Pool di Risorse</td>
        <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID <br>RESOURCEPOOLID (self)<br>SYSID  </td>
        <td>USERS_CURRENT | ID UTENTE <br>UTENTI_CORRENTE | USERID <br>Self<br>Non è una relazione; viene utilizzato per scopi interni all'applicazione  </td>
    </tr>
    <tr>
        <td>Nota Rich Text</td>
        <td>Nota Rich Text</td>
        <td>RHNOTE | Nota Rich Text</td>
        <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        <td>RICHTEXTNOTEID (self) <br>SYSID  </td>
        <td>Autonomo <br>Non è una relazione; utilizzato per scopi interni all'applicazione  </td>
    </tr>
    <tr>
        <td>Valore parametro Rich Text</td>
        <td>Valore parametro Rich Text</td>
        <td>RCHVAL | RichTextParameterValue</td>
        <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        <td>PARAMETERVALUEID<br>RICHTEXTPARAMETERVALUEID (self) <br>SYSID  </td>
        <td>La tabella dei valori dei parametri non è supportata al momento<br>Self <br>Not a relationship; utilizzata per scopi interni all'applicazione  </td>
    </tr>
    <tr>
        <td>Rischio</td>
        <td>Rischio</td>
        <td>RISCHIO | Rischio</td>
        <td>RISKS_CURRENT<br>RISKS_DAILY_HISTORY<br>RISKS_EVENT</td>
        <td>ENTEREDBYID<br>EXCHANGERATEID<br>LASTUPDATEDBYID <br>PROJECTID <br>RISKID (self)<br>RISKTYPEID<br>SYSID<br>TEMPLATEID</td>
        <td>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>USERS_CURRENT | ID UTENTE <br>PROGETTI_CORRENTE | PROJECTID   <br>Self<br>RISKTYPES_CURRENT | RISKTYPEID<br>Non è una relazione; utilizzato per scopi interni dell'applicazione<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>Tipo Rischio</td>
        <td>Tipo Rischio</td>
        <td>RSKTYP | Tipo di rischio</td>
        <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        <td>RISKTYPEID<br>SYSID</td>
        <td>Self<br>Non è una relazione; utilizzato per scopi interni dell'applicazione</td>
    </tr>
    <tr>
        <td>Ruolo</td>
        <td>Ruolo</td>
        <td>RUOLO | Ruolo</td>
        <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        <td>ENTEREDBYID<br>LAYOUTTEMPLATEID<br>PRIVATERATECARDID<br>ROLEID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>La tabella dei modelli di layout non sarà supportata<br>RATECARD_CURRENT | RATECARDID<br>SELF<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Pianificazione</td>
        <td>Pianificazione</td>
        <td>SCHED | Pianificazione</td>
        <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID<br>HOMEGROUPID<br>SCHEDULEID</td>
        <td>USER_CURRENT | USERID<br>GRUPPO_CORRENTE | GROUPID<br>CORRENTE_GRUPPO | GROUPID<br>Self</td>
    </tr>
    <tr>
        <td>Approvatore passaggio</td>
        <td>Approvatore passaggio</td>
        <td>SPAPVR | Approvatore fase</td>
        <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        <td>APPROVALSTEPID<br>ROLEID<br>STEPAPPROVERID (self)<br>SYSID <br>TEAMID<br>USERID</td>
        <td>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>ROLES_CURRENT | ROLEID<br>Self<br>Non è una relazione; utilizzato per scopi interni dell'applicazione <br>TEAMS_CURRENT | TEAMID<br>UTENTI_CORRENTE | USERID</td>
    </tr>
    <tr>
        <td>Attività</td>
        <td>Attività</td>
        <td>ATTIVITÀ | Attività</td>
        <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>BILLINGRECORDID<br>IDCATEGORIA<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>GROUPID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID{15 PARENTID<br>PROJECTID<br>RECURRENULEID<br>REJECTIONISSUEID<br>RESERVEDTIMEID<br>ROLEID<br>SUBMITTEDBYID<br>TASKID<br>TEAMID<br>TEMPLATETASKID<br></td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>UTENTE_CORRENTE | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | IDCATEGORIA<br>OPTASK_CURRENT | OPTASKID<br>UTENTE_CORRENTE | ID UTENTE<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>UTENTE_CORRENTE | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>GROUP_CURRENT | GROUPID<br>ITERATIONS_CURRENT | ITERATIONID<br>Tabella Kanban Board non supportata al momento<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>UTENTE_CORRENTE | ID UTENTE<br>MILESTONE_CURRENT | MILESTONEID<br>ATTIVITÀ_CORRENTE | TASKID<br>PROJECT_CURRENT | PROJECTID<br>Tabella regole di ricorrenza non supportata al momento<br>OPTASK_CURRENT | OPTASKID<br>RESERVEDTIMES_CURRENT | RESERVEDTIMEID<br>ROLE_CURRENT | ID RUOLO<br>UTENTE_CORRENTE | USERID<br>Self<br>TEAM_CURRENT | TEAMID<br>TEMPLATETASKS_CURRENT | TEMPLATFORM</td>
    </tr>
    <tr>
        <td>Predecessore attività</td>
        <td>Predecessore</td>
        <td>PRED | Predecessore</td>
        <td>PREDECESSORS_CURRENT<br>PREDECESSORS_DAILY_HISTORY<br>PREDECESSORS_EVENT</td>
        <td>ID (self)<br>PREDECESSORID<br>SUCCESSORID <br>SYSID</td>
        <td>Self<br>ATTIVITÀ_CORRENTE | TASKID<br>ATTIVITÀ_CORRENTE | TASKID <br>Non è una relazione; viene utilizzato per scopi interni all'applicazione</td>
    </tr>
    <tr>
        <td>Team</td>
        <td>Team</td>
        <td>TEAMOB | Team</td>
        <td>TEAM_CURRENT<br>TEAM_DAILY_HISTORY<br>TEAM_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>MYWORKVIEWID<br>OWNERID<br>REQUESTSVIEWID<br>SCHEDULEID<br>TEAMID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>GRUPPO_CORRENTE | GROUPID<br>La tabella del modello di layout non sarà supportata<br>UIVIEWS_CURRENT | UIVIEWID<br>UTENTE_CORRENTE | ID UTENTE<br>UIVIEWS_CURRENT | UIVIEWID<br>SCHEDULE_CURRENT | SCHEDULEID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Membro team</td>
        <td>Altri team, membro del team</td>
        <td>TEAM | Membro team</td>
        <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        <td>SYSID <br>IDTEAM<br>IDMEMBRO TEAM (self)<br>IDUTENTE</td>
        <td>Non è una relazione; utilizzato per scopi interni all'applicazione <br>TEAMS_CURRENT | TEAMID<br>Self<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>RuoloMembroTeam</td>
        <td>Mansione membro team</td>
        <td>TEAMMR | Ruolo membro team</td>
        <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        <td>ID RUOLO <br>ID TEAM<br>IDMEMBRO TEAM (self)<br>ID UTENTE</td>
        <td>ROLES_CURRENT | ID RUOLO <br>TEAM_CORRENTE | TEAMID<br>Self<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Modello</td>
        <td>Modello</td>
        <td>TMPL | Modello</td>
        <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        <td>APPROVALPROCESSID<br>CATEGORYID<br>COMPANYID <br>DELIVERABLESCORECARDID <br>ENTEREDBYID<br>GROUPID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID <br>OWNERID <br>PRIVATERATECARDID<br>PROGRAMID<br>QUEUEDEFID<br>SCHEDULEID <br>SYSID <br>TEAMID<br>TEMPLATEID (self)</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID   <br>DELIVERABLESCORECARDID <br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>NOTES_CURRENT | NOTEID<br>UTENTI_CORRENTE | ID UTENTE<br>MILESTONEPATH_CURRENT | MILESTONEPATHID <br>USERS_CURRENT | ID UTENTE <br>RATECARD_CURRENT | RATECARDID<br>PROGRAMMA_CORRENTE | PROGRAMID<br>Tabella di definizione coda non supportata al momento<br>SCHEDULES_CURRENT | SCHEDULEID <br>Non è una relazione; utilizzato per scopi interni dell'applicazione <br>TEAMS_CURRENT | TEAMID<br>Self</td>
    </tr>
    <tr>
        <td>Assegnazione Modello</td>
        <td>Assegnazione Modello</td>
        <td>ATTIVITÀ | Assegnazione modello</td>
        <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDTOID<br>CATEGORYID<br>LASTUPDATEDBYID<br>OBJID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEASSIGNMENTID (self)<br>TEMPLATETASKID</td>
        <td>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>ID dell'oggetto identificato nel campo OBJCODE<br>ROLES_CURRENT | ROLEID<br>Non è una relazione; utilizzato per scopi interni all'applicazione<br>TEAMS_CURRENT | TEAMID<br>Tabella Timeline Team non supportata al momento<br>Self<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>Attività modello</td>
        <td>Attività modello</td>
        <td>TTSK | Attività modello</td>
        <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>RECURRENCERULEID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEID<br>TEMPLATETASKID (self)</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>NOTES_CURRENT | NOTEID<br>UTENTI_CORRENTE | ID UTENTE<br>MILESTONE_CURRENT | MILESTONEID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>Tabella delle regole di ricorrenza non supportata al momento<br>ROLES_CURRENT | ROLEID<br>Non è una relazione; utilizzato per scopi interni dell'applicazione<br>TEAMS_CURRENT | TEAMID<br>Tabella Timeline Team non supportata al momento<br>TEMPLATES_CURRENT | TEMPLATEID<br>Self</td>
    </tr>
    <tr>
        <td>Predecessore attività modello</td>
        <td>Predecessore modello</td>
        <td>TPRED | Predecessore</td>
        <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        <td>PREDECESSORID<br>SUCCESSORID <br>TEMPLATEPREDECESSORID (self)<br>SYSID</td>
        <td>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID <br>Autonomo<br>Nessuna relazione; utilizzato per scopi interni all'applicazione</td>
    </tr>
    <tr>
        <td>Scheda orario</td>
        <td>Scheda orario</td>
        <td>SCHEDA | Scheda orario</td>
        <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
        <td>APPROVERID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>TIMESHEETID<br>TIMESHEETPROFILEID<br>USERID</td>
        <td>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>UTENTE_CORRENTE | USERID<br>Self<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>UTENTE_CORRENTE | USERID</td>
    </tr>
    <tr>
        <td>Profilo scheda orario</td>
        <td>Profilo scheda orario</td>
        <td>TSPRO | Timesheet Ricorrente</td>
        <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        <td>APPROVERID<br>ENTEREDBYID <br>GROUPID<br>SYSID<br>TIMESHEETPROFILEID (self)</td>
        <td>USERS_CURRENT | USERID<br>USERS_CURRENT | ID UTENTE <br>GROUPS_CURRENT | GROUPID<br>Non è una relazione; utilizzato per scopi interni dell'applicazione<br>Self</td>
    </tr>
    <tr>
        <td>Filtro interfaccia utente</td>
        <td>Filtro</td>
        <td>UIFT | Filtro</td>
        <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIFILTERID (self)</td>
        <td>Non è una relazione; utilizzato per scopi interni all'applicazione<br>USERS_CURRENT | ID UTENTE <br>UTENTI_CORRENTE | ID UTENTE <br>ID dell'oggetto identificato nel campo OBJCODE<br>PREFERENCES_CURRENT | PREFERENCEID<br>Non è una relazione; utilizzato per scopi interni dell'applicazione <br>Self</td>
    </tr>
    <tr>
        <td>Raggruppa per interfaccia utente</td>
        <td>Raggruppamento</td>
        <td>UIGB | Raggruppamento</td>
        <td>UIGROUPBYS_CURRENT<br>UIGROUPBYS_DAILY_HISTORY<br>UIGROUPBYS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID <br>UITEMPLATEID (self)</td>
        <td>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID <br>UTENTI_CORRENTE | USERID <br>Non è una relazione; utilizzato per scopi interni dell'applicazione <br>Autonomo</td>
    </tr>
    <tr>
        <td>Modello interfaccia utente</td>
        <td>Modello layout</td>
        <td>UITMPL | Modello di layout</td>
        <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIGROUPBYID (self)</td>
        <td>Non è una relazione; utilizzato per scopi interni all'applicazione<br>USERS_CURRENT | ID UTENTE <br>UTENTI_CORRENTE | ID UTENTE <br>ID dell'oggetto identificato nel campo OBJCODE<br>PREFERENCES_CURRENT | PREFERENCEID<br>Non è una relazione; utilizzato per scopi interni dell'applicazione <br>Self</td>
    </tr>
    <tr>
        <td>Visualizzazione interfaccia utente</td>
        <td>Visualizza</td>
        <td>UIVIEW | Visualizza</td>
        <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIVIEWID (self)</td>
        <td>Non è una relazione; utilizzato per scopi interni all'applicazione<br>USERS_CURRENT | ID UTENTE <br>UTENTI_CORRENTE | ID UTENTE <br>ID dell'oggetto identificato nel campo OBJCODE<br>PREFERENCES_CURRENT | PREFERENCEID<br>Non è una relazione; utilizzato per scopi interni dell'applicazione <br>Self</td>
    </tr>
    <tr>
        <td>Utente</td>
        <td>Utente</td>
        <td>UTENTE | Utente</td>
        <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
        <td>ACCESSLEVELID<br>CATEGORYID<br>COMPANYID<br>DEFAULTHOURTYPEID<br>DELEGATIONTOID<br>EAUTHUSERID<br>ENTEREDBYID<br>HOMEGROUPID<br>HOMETEAMID<br>LASTENTEREDNOTEID<br>LASTUPDATEDBYID<br>LATESTUPDATENOTEID<br>LAYOUTTEMPLATEID<br>MANAGERID<br>PORTALPROFILEID<br>PREFUIID<br>PRIVATERATECARDID <br>RESOURCEPOOLID<br>ROLEID<br>SCHEDULEID<br>TIMESHEETPROFILEID<br>UITEMPLATEID<br>USERID<br>UUMUSERID</td>
        <td>ACCESSLEVELS_CURRENT |ACCESSLEVELID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>HOURTYPE_CURRENT | HOURTYPEID<br>UTENTE_CORRENTE | USERID<br>Non è una relazione; utilizzato per scopi interni all'applicazione<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>TEAM_CURRENT | TEAMID<br>NOTE_CURRENT | NOTEID<br>UTENTE_CORRENTE | USERID<br>NOTE_CURRENT | NOTEID<br>La tabella dei modelli di layout non sarà supportata<br>USER_CURRENT | USERID<br>La tabella Portal Profile non sarà supportata<br>Nessuna relazione; utilizzata per scopi interni all'applicazione<br>RATECARD_CURRENT | RATECARDID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>ROLE_CURRENT | ID RUOLO<br>PIANIFICAZIONE_CORRENTE | SCHEDULEID<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>UITEMPLATES_CURRENT |UITEMPLATEID<br>Self<br>Non è una relazione; viene utilizzato a scopo di applicazione interna</td>
    </tr>
    <tr>
        <td>Delega utente</td>
        <td>Delega utente</td>
        <td>USRDEL | Delega utente</td>
        <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        <td>FROMUSERID<br>SYSID <br>TOUSERID <br>USERDELEGATIONID (self)</td>
        <td>USERS_CURRENT | USERID<br>Non è una relazione; utilizzato per scopi interni dell'applicazione <br>USERS_CURRENT | ID UTENTE <br>Autonomo</td>
    </tr>
    <tr>
        <td>Gruppo di utenti</td>
        <td>Altre Gruppi</td>
        <td>USRGPS | Gruppo utenti</td>
        <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        <td>GROUPID <br>SYSID<br>ID UTENTE <br>USERSGROUPID (self)</td>
        <td>GROUPS_CURRENT | GROUPID <br>Non è una relazione; utilizzato per scopi interni dell'applicazione<br>USERS_CURRENT | ID UTENTE <br>Autonomo</td>
    </tr>
    <tr>
        <td>Mansione utente</td>
        <td>Altre mansioni</td>
        <td>USRROL | Ruolo utente</td>
        <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        <td>ID RUOLO <br>SYSID<br>ID UTENTE    <br>USERROLESETID<br>USERSROLEID (self)</td>
        <td>ROLES_CURRENT | ROLEID <br>Non è una relazione; utilizzato per scopi interni all'applicazione<br>USERS_CURRENT | USERID    <br>USERROLESET_CURRENT | USERROLESETID<br>Self</td>
    </tr>
    <tr>
        <td>UserPrefValue</td>
        <td>UserPrefValue</td>
        <td>USERPF | Preferenza utente</td>
        <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        <td>SYSID    <br>USERID <br>USERPREFVALUEID (self)</td>
        <td>Non è una relazione; utilizzato per scopi interni all'applicazione<br>USERS_CURRENT | USERID    <br>Autonomo</td>
    </tr>
    <tr>
        <td>UserRoleSet</td>
        <td>UserRoleSet</td>
        <td>URSET | UserRoleSet</td>
        <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        <td>PRIMARYROLEID <br>SYSID<br>USERID    <br>USERROLESETID (self)</td>
        <td>ROLES_CURRENT | ROLEID <br>Non è una relazione; utilizzato per scopi interni all'applicazione<br>USERS_CURRENT | ID UTENTE <br>Autonomo</td>
    </tr>
    <tr>
        <td>UsersDecisions</td>
        <td>Decisioni degli utenti</td>
        <td>USRDEC | Decisioni degli utenti</td>
        <td>USERSDECISIONS_CURRENT<br>USERSDECISIONS_DAILY_HISTORY<br>USERSDECISIONS_EVENT</td>
        <td>USERDECISIONID (self)<br>SYSID <br>USERID  </td>
        <td>Self<br>Non è una relazione; utilizzato per scopi interni dell'applicazione <br>USERS_CURRENT | USERID </td>
    </tr>
    <tr>
        <td>WorkItem</td>
        <td>Elemento di lavoro</td>
        <td>WRKITM | WorkItem</td>
        <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        <td>ASSIGNMENTID <br>OBJID<br>OPTASKID    <br>PROJECTID <br>SYSID<br>TASKID    <br>USERID <br>WORKITEMID (self)</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID <br>ID dell'oggetto identificato nel campo OBJOBJCODE<br>OPTASK_CURRENT | OPTASKID    <br>PROGETTI_ATTUALI | PROJECTID <br>Non è una relazione; viene utilizzato per scopi interni all'applicazione<br>TASKS_CURRENT | TASKID    <br>UTENTI_CORRENTI | USERID    <br>Autonomo </td>
    </tr>
  </tbody>
</table>
