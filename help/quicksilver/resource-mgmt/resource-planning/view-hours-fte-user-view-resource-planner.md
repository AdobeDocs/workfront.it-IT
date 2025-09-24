---
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: Visualizzare le ore disponibili, pianificate ed effettive o l'FTE nella Programmazione delle risorse quando si utilizza la Vista utente
description: Visualizzare le ore disponibili, pianificate ed effettive o FTE nella pianificazione risorse quando si utilizza la vista UtentePianificazione nell'RP, ad esempio "budgeting delle risorse nell'RP" o "Gestione delle risorse nell'RP". ecc... - o potrebbe essere necessario riutilizzarlo da un altro POV?!)
author: LIsa
feature: Resource Management
exl-id: 6b532aa2-435f-4fda-b7ce-abe0a785638f
source-git-commit: 13621c29f32a514af46489fb58397f3e96f640ce
workflow-type: tm+mt
source-wordcount: '1739'
ht-degree: 1%

---

# Visualizzare le ore disponibili, pianificate ed effettive o FTE nella Programmazione delle risorse quando si utilizza la vista Utente

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Consider renaming this article (probably split already) to something other than "Planning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)</p>
-->

Oltre alle risorse preventivate nelle viste Progetto e Ruolo, è possibile utilizzare la Vista utente di Adobe Workfront Resource Planner per visualizzare informazioni sui valori delle ore o FTE pianificate, disponibili e effettive per i progetti e le risorse.

## Panoramica della visualizzazione utente nella Programmazione delle risorse

Quando visualizzi le informazioni sulle ore o sull&#39;FTE nella Programmazione risorse, considera quanto segue:

* È possibile visualizzare le ore disponibili e pianificate o le informazioni FTE per gli utenti, le mansioni e i progetti in tutte le visualizzazioni di Programmazione delle risorse.
* È possibile visualizzare le seguenti informazioni solo nella Vista utente:

   * Differenza tra la quantità di ore pianificate o FTE e la quantità di ore disponibili o FTE. Puoi quindi preventivare l’allocazione degli utenti in base a questa differenza nelle viste Progetto e Ruolo.
   * Le ore effettive o FTE.

* È possibile visualizzare la differenza tra l&#39;utente disponibile e la quantità di ore pianificate o FTE come numero o come valore percentuale nella vista Utente.
* Non è possibile visualizzare le informazioni nella vista Utente in base al costo.
* Adobe Workfront compila le ore disponibili o FTE in base all’orario di lavoro associato agli utenti nelle loro pianificazioni.\
  Gli utenti non associati a una pianificazione mostrano la disponibilità in base alla pianificazione predefinita.\
  Per informazioni sulla pianificazione predefinita, vedere [Creare una pianificazione](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Workfront compila le ore pianificate o FTE dalle informazioni sulle ore pianificate relative alle attività e ai problemi dei progetti.
* Workfront compila le ore effettive con il tempo effettivamente registrato per le attività e i problemi dagli utenti assegnati. Questo include il tempo di connessione a un progetto.
* Nella vista Utente, è possibile effettuare le seguenti operazioni:

   * Espandi ogni utente per visualizzare un elenco di progetti a cui è assegnato l’utente.

     >[!NOTE]
     >
     >È possibile espandere solo gli utenti associati ai progetti inclusi nei filtri.

   * Espandi ogni progetto per visualizzare un elenco di mansioni che l’utente può svolgere su tali progetti.
   * Espandere ogni ruolo per visualizzare un elenco di attività a cui l&#39;utente in tale ruolo è assegnato.

  Se agli utenti non sono associati ruoli, le ore disponibili, pianificate e effettive o FTE sono elencate nella sezione **Nessun ruolo**.\
  Per informazioni sui campi e sugli elementi visualizzati quando si applica la visualizzazione Utente alla Programmazione delle risorse, vedere la sezione &quot;Selezione progetto/ruolo/visualizzazione utente&quot; nella [Panoramica sulla navigazione di Programmazione delle risorse](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Panoramica dei campi visibili nella Visualizzazione utente della Programmazione delle risorse

Per informazioni sulle informazioni visualizzate nella visualizzazione Utente della Programmazione delle risorse, fare riferimento alle tabelle seguenti. Le informazioni vengono visualizzate in Ore o valori FTE.

* [Colonna AVL (disponibile)](#the-avl-available-column)
* [Colonna PLN (pianificato)](#the-pln-planned-column)
* [Colonna ACT (Effettivo)](#The%C2%A0ACT)
* [Colonna DIF (Differenza)](#the-dif-difference-column)
* [Colonna % (percentuale allocazione ore pianificate)](#the-planned-hours-allocation-percentage-column)

### Colonna AVL (Disponibile) {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visualizzato da</strong> </td> 
   <td> <p><strong>Descrizione</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td>Totale delle ore disponibili o FTE per l'utente in base alla pianificazione. </td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td>Queste informazioni non sono disponibili per il progetto quando si applica la vista Utente alla pianificazione risorse. </td> 
  </tr> 
  <tr> 
   <td>Ruolo</td> 
   <td> <p>Totale delle ore disponibili o FTE per il ruolo in base alla pianificazione dell'utente e alla <strong>percentuale di disponibilità FTE</strong> del ruolo.</p> </td> 
  </tr> 
  <tr> 
   <td>Attività o problema</td> 
   <td>Queste informazioni non sono disponibili per l’Attività o il Problema. </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni sul modo in cui la disponibilità di utenti e ruoli viene calcolata in base alla pianificazione dell&#39;utente e alla percentuale di disponibilità FTE del ruolo, vedere [Panoramica sul calcolo delle ore e FTE per utenti e ruoli nella programmazione delle risorse](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

### Colonna PLN (Pianificato) {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visualizzato da</strong> </td> 
   <td> <p><strong>Descrizione</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td> Il totale delle ore pianificate o FTE da tutte le attività o i problemi assegnati all’utente su tutti i progetti.<br><p>Ciò include le attività e i problemi assegnati all’utente ma non associati ad alcuna mansione e le attività o i problemi che non si trovano nei progetti a cui hai accesso per la gestione.</p><p>Quando l’allocazione utente per le ore è stata modificata utilizzando il Bilanciatore dei carichi di lavoro, i dati nella Programmazione delle risorse possono essere interessati se le date selezionate contengono solo una parte di un’attività o di un problema. Per informazioni sulla modifica delle allocazioni per gli utenti, vedere <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gestione delle allocazioni utente nel Bilanciatore dei carichi di lavoro</a> . </p></td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td> Il totale delle ore pianificate o FTE da tutte le attività e i problemi assegnati a un utente specifico sul progetto.<br><p>Nota: non sono incluse le ore pianificate o l’FTE da attività o problemi non assegnati ad alcun utente. </p></td> 
  </tr> 
  <tr> 
   <td>Ruolo</td> 
   <td> <p>Il totale delle ore pianificate o FTE da tutte le attività e i problemi assegnati all'utente con questo ruolo sul progetto.</p> <p> <p>Nota: non sono incluse le ore pianificate o l’FTE da attività o problemi assegnati a questo ruolo ma non a questo utente in questo ruolo. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Attività o problema</td> 
   <td>Le ore pianificate o l'FTE associato all'attività o al problema nel progetto.</td> 
  </tr> 
 </tbody> 
</table>

Quando visualizzi le ore pianificate, tieni presente quanto segue:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view)</p>
-->

* Le ore pianificate vengono distribuite in modo uniforme a ogni giorno entro la Durata delle attività e dei problemi , per ogni risorsa a loro assegnata. La durata dell’attività o del problema è basata sulle date di inizio e completamento pianificate e include ogni giorno di calendario entro tale periodo di tempo.\
  Workfront prende in considerazione la pianificazione dell’utente o del progetto al momento della distribuzione delle ore pianificate agli utenti o ai progetti. In questo caso, le ore pianificate vengono distribuite in modo uniforme a ogni giorno entro la Durata delle attività o dei problemi, esclusi i fine settimana, i giorni di ferie e le eccezioni alla pianificazione.

  Se ad esempio si visualizza la Pianificazione risorse per settimana e si dispone di attività che si estendono su più settimane nei progetti, il numero di ore pianificate alla settimana dipende dal numero di giorni della settimana che fanno parte della Durata dell&#39;attività. Questa funzione funziona in modo simile quando si visualizza la Programmazione delle risorse per mese o trimestre e quando le attività si estendono su più mesi o trimestri.\
  I giorni di fine settimana, le eccezioni alla programmazione e i giorni di ferie sono esclusi da questa distribuzione.

* Le seguenti categorie di attività sono incluse nel calcolo delle ore pianificate per ciascuna risorsa:

   * le attività assegnate agli utenti nei Pool di Risorse, le mansioni o i team del progetto.

     >[!TIP]
     >
     >Se le attività sono assegnate ai team, la loro allocazione verrà visualizzata nelle sezioni **Nessun ruolo** e **Nessun utente**. Puoi visualizzare le ore pianificate associate ai team, ma non puoi preventivarle, perché alle attività non sono associati ruoli né utenti.

* Le ore pianificate nella pianificazione risorse non includono le ore pianificate associate ai seguenti elementi:

   * attività padre
   * attività non assegnate
   * problemi, quando l&#39;impostazione **Includi ore da problemi** è disabilitata.

* Le ore pianificate non vengono visualizzate nella Programmazione delle risorse se l&#39;attività o la Durata del problema è zero.
* Le ore pianificate associate agli utenti disattivati non vengono visualizzate.

Per ulteriori informazioni sulle ore pianificate e sull&#39;FTE nella Programmazione delle risorse, vedere [Panoramica sulle ore, sull&#39;FTE e sui costi nelle visualizzazioni Progetto e Ruolo della Programmazione delle risorse](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

### Colonna ACT (Effettivo)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visualizzato da</strong> </td> 
   <td> <p><strong>Descrizione</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Utente </td> 
   <td> <p>L’ora registrata dall’utente su tutte le attività o i problemi ad esso assegnati.</p> <p>Ciò include quanto segue:</p> 
    <ul> 
     <li>Attività e problemi assegnati all'utente ma non associati ad alcuna mansione.</li> 
     <li>Attività e problemi che non si trovano in progetti per i quali hai accesso a Gestisci. </li> 
    </ul> <p>Questo include il tempo registrato sul progetto solo quando l'utente è assegnato ad attività o problemi su quel progetto.  </p> </td> 
  </tr> 
  <tr> 
   <td>Progetto </td> 
   <td> <p>L’ora registrata dall’utente su tutte le attività e i problemi ad esso assegnati sul progetto.</p> <p>Ciò include tutte le volte in cui hanno effettuato l’accesso diretto al progetto.</p> <p>Non sono compresi i seguenti elementi:</p> 
    <ul> 
     <li> <p>Attività e problemi connessi all'ora non assegnati ad alcun utente. </p> </li> 
     <li> <p>Tempo di connessione delle attività padre. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Ruolo</td> 
   <td> <p>L'ora di accesso a tutte le attività o i problemi assegnati all'utente con questo ruolo. </p> <p>Non sono compresi i seguenti elementi:</p> 
    <ul> 
     <li>Le attività e i problemi connessi all'ora assegnati a questo ruolo ma non a questo utente in questo ruolo.</li> 
     <li>Tempo registrato direttamente sul progetto o sulle attività padre. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Attività o problema </td> 
   <td> <p>L'ora di accesso alle attività e ai problemi da parte dell'utente a cui vengono assegnati. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>L’ora registrata viene visualizzata nell’intervallo di tempo corrispondente alla data di immissione dell’ora, indipendentemente dall’intervallo di tempo dell’attività, del problema o del progetto in cui sono registrate le ore.

Per ulteriori informazioni sulle ore effettive, vedere [Visualizza ore effettive](../../manage-work/tasks/task-information/actual-hours.md).

### Colonna DIF (Differenza) {#the-dif-difference-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visualizzato da</strong> </td> 
   <td> <p><strong>Descrizione</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td> <p>Differenza tra le ore disponibili e pianificate o FTE dell’utente. </p> <p>La differenza di ore o FTE viene calcolata utilizzando la seguente formula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>Nota: se il valore è visualizzato in numeri rossi negativi, l'utente è sovrassegnato. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td>Queste informazioni non sono disponibili per il progetto. </td> 
  </tr> 
  <tr> 
   <td>Ruolo</td> 
   <td> <p>Differenza tra le ore disponibili e pianificate o FTE del ruolo. </p> <p>La differenza di ore o FTE viene calcolata utilizzando la seguente formula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>Nota: se il valore viene visualizzato in numeri rossi negativi, il ruolo è sovrassegnato. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Attività o problema</td> 
   <td>Queste informazioni non sono disponibili per l'Attività, la Issue o il Progetto. </td> 
  </tr> 
 </tbody> 
</table>

### Colonna % (percentuale allocazione ore pianificate) {#the-planned-hours-allocation-percentage-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visualizzato da</strong> </td> 
   <td> <p><strong>Descrizione</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td> <p>L’allocazione delle ore pianificate o FTE come percentuale delle ore disponibili. La percentuale dell'allocazione ore pianificate viene calcolata utilizzando la formula seguente:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>Lo stesso calcolo viene utilizzato per i valori FTE. </p> </td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td>Queste informazioni non sono disponibili per il progetto quando si applica la visualizzazione <strong>Visualizza per utente</strong> alla pianificazione risorse.</td> 
  </tr> 
  <tr> 
   <td>Ruolo</td> 
   <td> L’allocazione delle ore pianificate o FTE come percentuale delle ore disponibili. <p>La percentuale dell'allocazione ore pianificate viene calcolata utilizzando la formula seguente:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>Lo stesso calcolo viene utilizzato per i valori FTE.</p></td> 
  </tr> 
  <tr> 
   <td>Attività o problema</td> 
   <td>Queste informazioni non sono disponibili per l'Attività, la Issue o il Progetto. </td> 
  </tr> 
 </tbody> 
</table>

Se il valore delle ore pianificate o dell&#39;FTE è zero, la percentuale di allocazione sarà 0%. Se il valore di Ore disponibili o FTE è zero, non è possibile calcolare la percentuale di allocazione.

Per ulteriori informazioni sulle ore pianificate e sull&#39;FTE e su come vengono visualizzate nella Programmazione delle risorse, vedere [Risorse preventivate nella Programmazione delle risorse utilizzando le visualizzazioni Progetto e Ruolo](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this table is ideal but it does not render in Markdown) </p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours or FTE)</strong> </td>
<td><strong>Displayed By</strong> </td>
<td> <p><strong>Description</strong> </p> </td>
</tr>
<tr>
<td rowspan="5">AVL <br>(Available Hours or FTE)</td>
<td>User</td>
<td>The total of Available Hours or FTE for the user according to their schedule. </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the User view to the Resource Planner. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Available Hours or FTE for the role according to the schedule of the user and the <strong>Percentage of FTE Availability</strong> of the role.</p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project.</td>
</tr>
<tr>
<td colspan="2"> <p colspan="2">For more information about how user and role availability is calculated based on the schedule of the user and the Percentage of FTE Availability of the role, see <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">PLN <br>(Planned Hours or FTE)</td>
<td>User</td>
<td> The total of Planned Hours or FTE from all the tasks or issues assigned to the user on all the projects.<br><p>This includes tasks and issues that are assigned to the user but not associated with any job role and tasks or issues that are not on projects that you have access to Manage.</p><p>When the user allocation for hours has been modified using the Workload Balancer, the data in the Resource Planner can be affected if the dates selected contain only a portion of a task or issue. For information about modifying allocations for users, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a> . </p></td>
</tr>
<tr>
<td>Project</td>
<td> The total of Planned Hours or FTE from all the tasks and issues assigned to a specific user on the project.<br><note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are not assigned to any users.
</note></td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Planned Hours or FTE from all the tasks and issues assigned to the user in this role on the project.</p> <p> <note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are assigned to this role but not to this user in this role.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>The Planned Hours or FTE associated with the task or the issue on the project.</td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view))</p>
<ul>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks and issues , for each resource assigned to them. The task or issue Duration is based on their Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks or issues excluding weekends, time-off days, and schedule exceptions.</p> <p>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> <p>The following categories of tasks are included in calculating the Planned Hours for each resource: </p>
<ul>
<li> <p> tasks assigned to users in Resource Pools, job roles, or teams on the project.</p> <note type="tip">
If tasks are assigned to teams, their allocation will appear under
<strong>No Role</strong> and
<strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks.
</note> </li>
</ul> </li>
</ul>
<ul>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>unassigned tasks</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task or issue Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> <p>For more information about Planned Hours and FTE in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">ACT<br>(Actual Hours or FTE) </td>
<td>User </td>
<td> <p>The time logged by the user on all the tasks or issues assigned to them.</p> <p>This includes the following:</p>
<ul>
<li>Tasks and issues that are assigned to the user but not associated with any job role.</li>
<li>Tasks and issues that are not on projects for which you have access to Manage.. </li>
</ul> <p>This does not include time logged directly on the project or on parent tasks. </p> </td>
</tr>
<tr>
<td>Project </td>
<td> <p>The time logged by the user on all the tasks and issues assigned to them on the project.</p> <p>This includes any time that they logged directly on the project.</p> <p>This does not include the following:</p>
<ul>
<li> <p>Time logged on tasks and issues that are not assigned to any users. </p> </li>
<li> <p>Time logged on parent tasks. </p> </li>
</ul> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The time logged on all the tasks or issues assigned to the user in this role. </p> <p>This does not include the following:</p>
<ul>
<li>Time logged on tasks and issues assigned to this role but not to this user in this role.<em> </em></li>
<li>Time logged directly on the project or parent tasks. </li>
</ul> </td>
</tr>
<tr>
<td>Task or Issue </td>
<td> <p>The time logged on tasks and issues by the user who is also assigned to them. </p> </td>
</tr>
<tr>
<td colspan="2"> <p> <note type="important">
The time logged is displayed in the timeframe corresponding to the Entry Date of the hour entry, regardless of the timeframe of the task, issue, or project where the hours are logged.
</note> </p> <p>For more information about Actual Hours, see <a href="../../manage-work/tasks/task-information/actual-hours.md" class="MCXref xref">View Actual Hours</a></p> </td>
</tr>
<tr>
<td rowspan="4">DIF <br>(Hour or FTE Difference) <br><br></td>
<td>User</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the user. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <note type="note">
If the value displays in negative red numbers, the user is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the job role. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <note type="note">
If the value is displayed in negative red numbers, the role is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td rowspan="5">Planned Hours or FTE Allocation Percentage (%)</td>
<td>User</td>
<td> <p>The allocation of the Planned Hours or FTE as a percentage of the Available Hours. The percentage of the Planned Hours Allocation is calculated using the following formula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>The same calculation is used for FTE values. </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the <strong>View by User</strong> view to the Resource Planner.</td>
</tr>
<tr>
<td>Role</td>
<td> The allocation of the Planned Hours or FTE as a percentage of the Available Hours. <p>The percentage of the Planned Hours Allocation is calculated using the following formula:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>The same calculation is used for FTE values.</p></td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td colspan="2"> <p> If the value of the Planned Hours or FTE is zero, the Percentage Allocation is 0%. If the value of the Available Hours or FTE is zero, the Percentage Allocation cannot be calculated. </p> <p>For more information about Planned Hours and FTE and how they are displayed in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> </td>
</tr>
</tbody>
</table>
-->
