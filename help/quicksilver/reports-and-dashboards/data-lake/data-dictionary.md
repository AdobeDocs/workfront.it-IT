---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Dizionario dati Data Lake
description: Questa pagina contiene informazioni sulla struttura e il contenuto dei dati nel data lake di Workfront.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 81f8477dd26b828c4255c678b36d98789cd81ff8
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 5%

---

# dizionario dati del data lake di Workfront

Questa pagina contiene informazioni sulla struttura e il contenuto dei dati nel data lake di Workfront.

>[!NOTE]
>
>I dati nel data lake di Workfront vengono aggiornati ogni quattro ore, pertanto le modifiche recenti potrebbero non essere applicate immediatamente.

## Tipi di tabella

Esistono diversi tipi di tabelle che è possibile utilizzare per visualizzare i dati di Workfront in modo da fornire la maggior parte delle informazioni.

* **Tabella corrente**

  La tabella Current riflette i dati in modo simile a come esistono in Workfront, in ogni oggetto e nel relativo stato corrente. Tuttavia, può essere navigato con una latenza molto più bassa rispetto a Workfront.

* **Tabella eventi**

  La tabella Evento tiene traccia di ogni record di modifica in Workfront, ovvero ogni volta che un oggetto cambia stato, viene creato un record che mostra quando è avvenuta la modifica, chi ha apportato la modifica e cosa è stato modificato. Pertanto, questa tabella è utile per i confronti point-in-time. Questa tabella include solo i record degli ultimi tre anni.

* **Tabella cronologia giornaliera**

  La tabella Cronologia giornaliera offre una versione abbreviata della tabella Evento, in quanto mostra lo stato di ciascun oggetto su base giornaliera anziché nel momento in cui si è verificato ogni singolo evento. Pertanto, questa tabella è utile per l’analisi delle tendenze.

<!-- Custom table -->

## Diagramma relazioni entità

Gli oggetti in Workfront (e, pertanto, nel data lake) sono definiti non solo dai singoli valori, ma anche dalle relazioni con altri oggetti. Il diagramma delle relazioni tra entità riportato di seguito fornisce una mappatura di alto livello delle relazioni tra oggetti nel data lake di Workfront. Il diagramma può essere visualizzato e scaricato utilizzando il seguente collegamento:

[Diagramma delle relazioni delle entità del data lake di Workfront](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>Il diagramma delle relazioni tra entità è un work in progress, in quanto tale, è solo a scopo di riferimento ed è soggetto a modifiche.

## Tipi di date

Esistono diversi oggetti data che forniscono informazioni su quando si verificano eventi specifici.

* `DL_LOAD_TIMESTAMP`: questa data viene utilizzata come riferimento interno e viene visualizzata quando i dati sono stati caricati nella tabella Cronologia corrente, evento o giornaliera. Questa data non deve essere utilizzata per l’analisi dei dati e deve essere rimossa durante la fase beta del data lake di Workfront.
* `CALENDAR_DATE`: data presente solo nella tabella Cronologia giornaliera. Questa tabella fornisce una registrazione dell’aspetto dei dati alle 11:59 UTC per ogni data specificata in `CALENDAR_DATE`.
* `BEGIN_EFFECTIVE_TIMESTAMP`: questa data è presente nelle tabelle Evento e Cronologia giornaliera e registra esattamente quando un record viene modificato _a_ il valore presente nella riga corrente.
* `END_EFFECTIVE_TIMESTAMP`: questa data è presente nelle tabelle Evento e Cronologia giornaliera e registra esattamente quando un record viene modificato _da_ il valore nella riga corrente a un valore in una riga diversa. Per consentire l’esecuzione di query tra `BEGIN_EFFECTIVE_TIMESTAMP` e `END_EFFECTIVE_TIMESTAMP` questo è un valore che non è mai nullo, anche se non esiste un nuovo valore. Nel caso in cui un record sia ancora valido (ossia il valore non sia stato modificato), `END_EFFECTIVE_TIMESTAMP` avrà un valore di 2300-01-01.

## Tabella terminologica

La tabella seguente mette in correlazione i nomi degli oggetti in Workfront (così come i loro nomi nell’interfaccia e nell’API) con i loro nomi equivalenti nel data lake.

<table>
<thead>
  <tr>
    <th>Nome entità Workfront</th>
    <th>Riferimenti interfaccia</th>
    <th>Riferimento API | Etichetta</th>
    <th>Tabelle Data Lake</th>
    <th>Note</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Assegnazione</td>
    <td>Assegnazione</td>
    <td>ASSEGNA | Assegnazione</td>
    <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>EnumPersonalizzata</td>
    <td>Condizione, Priorità, Gravità, Stato</td>
    <td>CSTEM | Enum personalizzata</td>
    <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
    <td>Il tipo di record è identificato tramite la proprietà "enumClass". Di seguito sono riportati i tipi previsti:<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>TASK_PRIORITARIO<br>GRAVITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>TASK_STATO</td>
  </tr>
  <tr>
    <td>Documento</td>
    <td>Documento</td>
    <td>DOCU | Documento</td>
    <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br><br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>DocumentVersion</td>
    <td>Versione documento</td>
    <td>DOCV | Versione documento</td>
    <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Gruppo</td>
    <td>Gruppo</td>
    <td>GRUPPO | Gruppo</td>
    <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Ora</td>
    <td>Ora</td>
    <td>ORA | Hour</td>
    <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Tipo di ora</td>
    <td>Tipo di ora</td>
    <td>ORA | Tipo di Ora</td>
    <td>HOURTYPES_CURRENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Milestone</td>
    <td>Milestone</td>
    <td>MIGLIA | Milestone</td>
    <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>PercorsoMilestone</td>
    <td>Percorso milestone</td>
    <td>MPATH | Percorso milestone</td>
    <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Nota</td>
    <td>Nota</td>
    <td>NOTA | Nota</td>
    <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>OpTask</td>
    <td>Problema, richiesta</td>
    <td>OPTASK | Problema</td>
    <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br><br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Portfolio</td>
    <td>Portfolio</td>
    <td>PORTA | Portfolio</td>
    <td>PORTFOLI_CORRENTE<br>PORTFOLI_CRONOLOGIA_GIORNALIERA<br>PORTFOLI_EVENT<br><br>PORTFOLI_CUSTOM_VALUE_CURRENT<br>PORTFOLI_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLI_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Programma</td>
    <td>Programma</td>
    <td>PRGM | Programma</td>
    <td>PROGRAMMI_CORRENTI<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br><br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Progetto</td>
    <td>Progetto</td>
    <td>PROJ | Progetto</td>
    <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br><br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Ruolo</td>
    <td>Ruolo</td>
    <td>RUOLO | Ruolo</td>
    <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Pianificazione</td>
    <td>Pianificazione</td>
    <td>SCHED | Pianificazione</td>
    <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Attività</td>
    <td>Attività</td>
    <td>ATTIVITÀ | Attività</td>
    <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br><br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Team</td>
    <td>Team</td>
    <td>TEAMOB | Team</td>
    <td>TEAM_CURRENT<br>TEAM_DAILY_HISTORY<br>TEAMS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Scheda orario</td>
    <td>Scheda orario</td>
    <td>SCHEDA | Scheda orario</td>
    <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Utente</td>
    <td>Utente</td>
    <td>UTENTE | Utente</td>
    <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br><br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
</tbody>
</table>
