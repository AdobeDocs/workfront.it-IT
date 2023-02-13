---
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: Visualizza Ore disponibili, pianificate e effettive o FTE nel planner risorse quando si utilizza la visualizzazione Utente
description: Visualizza le ore disponibili, pianificate e effettive o FTE nel Planner risorse quando si utilizza la pianificazione della visualizzazione utente nel RP" - ad esempio "risorse di budget nel RP" o "Gestione delle risorse nel RP". ecc.. - o potrebbe essere necessario riproporre da un altro POV?!)"
author: Alina
feature: Resource Management
exl-id: 6b532aa2-435f-4fda-b7ce-abe0a785638f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1738'
ht-degree: 1%

---

# Visualizza Ore disponibili, pianificate e effettive o FTE nel planner risorse quando si utilizza la visualizzazione Utente

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Consider renaming this article (probably split already) to something other than "Planning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)</p>
-->

Oltre alle risorse di budget nelle visualizzazioni Progetto e Ruolo, è possibile utilizzare la visualizzazione utente del planner risorse di Adobe Workfront per visualizzare informazioni sui valori Orario pianificato, Disponibile e Effettivo o FTE per progetti e risorse.

## Panoramica della visualizzazione utente nel planner risorse

Quando si visualizzano le informazioni Ore o FTE nel Planner risorse, tenere presente quanto segue:

* È possibile visualizzare le informazioni Orari disponibili e pianificate o FTE per gli utenti, i ruoli di lavoro e i progetti in tutte le visualizzazioni del Planner risorse.
* È possibile visualizzare le seguenti informazioni solo nella visualizzazione utente:

   * La differenza tra la quantità di ore pianificate o FTE e la quantità di ore disponibili o FTE. Puoi quindi eseguire il budget dell’allocazione degli utenti in base a questa differenza nelle visualizzazioni Progetto e Ruolo .
   * Le ore effettive o FTE.

* È possibile visualizzare la differenza tra l’Utente disponibile e la quantità di Ore pianificate o FTE sotto forma di numero o come valore percentuale nella visualizzazione Utente.
* Non è possibile visualizzare le informazioni nella visualizzazione Utente in base al costo.
* Adobe Workfront compila gli orari disponibili o gli orari FTE in base all’orario di lavoro associato agli utenti nelle loro pianificazioni.\
   Gli utenti non associati a una pianificazione mostrano la disponibilità in base alla pianificazione predefinita.\
   Per informazioni sulla pianificazione predefinita, consulta [Creare una pianificazione](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Workfront compila le ore pianificate o FTE dalle informazioni sulle ore pianificate relative alle attività e ai problemi relativi ai progetti.
* Workfront compila le ore effettive con il tempo effettivamente registrato per le attività e i problemi degli utenti a cui sono assegnati. Questo include il tempo di accesso a un progetto.
* Nella visualizzazione Utente è possibile effettuare le seguenti operazioni:

   * Espandi ogni utente per visualizzare un elenco di progetti a cui è assegnato l’utente.

      >[!NOTE]
      >
      >Puoi espandere solo gli utenti associati ai progetti inclusi nei filtri.

   * Espandi ogni progetto per visualizzare un elenco di ruoli di lavoro che l’utente può eseguire su tali progetti.
   * Espandi ogni ruolo per visualizzare un elenco delle attività a cui è assegnato l’utente in quel ruolo.

   Se gli utenti non dispongono di ruoli di lavoro associati, le opzioni Disponibili, Pianificate e Ore effettive o FTE sono elencate in **Nessun ruolo** sezione .\
   Per informazioni sui campi e gli elementi visualizzati quando si applica la visualizzazione Utente al planner risorse, vedere la sezione &quot;Progetto/Ruolo/Selezione visualizzazione utente&quot; in [Panoramica sulla navigazione in planner risorse](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Panoramica dei campi visibili nella Visualizzazione utente del planner risorse

Fare riferimento alle tabelle seguenti per comprendere le informazioni visualizzate nella visualizzazione Utente del Planner risorse. Le informazioni vengono visualizzate in ore o valori FTE.

* [Colonna AVL (disponibile)](#the-avl-available-column)
* [Colonna PLN (pianificata)](#the-pln-planned-column)
* [Colonna ACT (effettivo)](#The%C2%A0ACT)
* [Colonna DIF (Differenza)](#the-dif-difference-column)
* [Colonna % (Percentuale allocazione ore pianificate)](#the-planned-hours-allocation-percentage-column)

### Colonna AVL (disponibile) {#the-avl-available-column}

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
   <td>Il totale di ore disponibili o FTE per l’utente in base alla loro pianificazione. </td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td>Queste informazioni non sono disponibili per il progetto quando si applica la visualizzazione Utente al Planner risorse. </td> 
  </tr> 
  <tr> 
   <td>Qual</td> 
   <td> <p>Totale di ore disponibili o FTE per il ruolo in base alla pianificazione dell’utente e del <strong>Percentuale di disponibilità FTE</strong> del ruolo.</p> </td> 
  </tr> 
  <tr> 
   <td>Attività o problema</td> 
   <td>Informazioni non disponibili per l'attività o il problema. </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni sul calcolo della disponibilità di utenti e ruoli in base alla pianificazione dell’utente e alla percentuale di disponibilità FTE del ruolo, consulta [Panoramica del calcolo delle ore e degli FTE per utenti e ruoli nel Planner risorse](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

### Colonna PLN (pianificata) {#the-pln-planned-column}

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
   <td> Totale ore pianificate o FTE da tutte le attività o problemi assegnati all’utente su tutti i progetti.<br><p>Ciò include le attività e i problemi assegnati all'utente ma non associati ad alcun ruolo di lavoro e attività o problemi che non si verificano nei progetti a cui hai accesso per la gestione.</p><p>Quando l'allocazione utente per ore è stata modificata utilizzando il servizio di bilanciamento del carico di lavoro, i dati nel planner risorse possono essere interessati se le date selezionate contengono solo una parte di un'attività o di un problema. Per informazioni sulla modifica delle allocazioni per gli utenti, consulta <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gestire le allocazioni di utenti nel load balancer</a> . </p></td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td> Totale di ore pianificate o FTE da tutte le attività e i problemi assegnati a un utente specifico del progetto.<br><p>Nota: Non sono incluse le ore pianificate o le FTE da attività o problemi non assegnati ad alcun utente. </p></td> 
  </tr> 
  <tr> 
   <td>Qual</td> 
   <td> <p>Totale di ore pianificate o FTE da tutte le attività e i problemi assegnati all’utente in questo ruolo sul progetto.</p> <p> <p>Nota: Questo non include le ore pianificate o FTE da attività o problemi assegnati a questo ruolo ma non a questo utente in questo ruolo. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Attività o problema</td> 
   <td>Orari pianificati o FTE associati all’attività o al problema relativo al progetto.</td> 
  </tr> 
 </tbody> 
</table>

Quando si visualizzano le ore pianificate, tenere presente quanto segue:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view)</p>
-->

* Le ore pianificate vengono distribuite in modo uniforme a ogni giorno entro la durata delle attività e dei problemi , per ogni risorsa loro assegnata. La durata dell&#39;attività o del problema si basa sulle rispettive date di inizio e di completamento pianificate e include ogni giorno di calendario entro tale periodo di tempo.\
   Workfront tiene conto della pianificazione dell’utente o del progetto quando distribuisce gli orari pianificati a utenti o progetti. In questo caso, le ore pianificate vengono distribuite in modo uniforme a ogni giorno entro la Durata delle attività o dei problemi, esclusi i fine settimana, i giorni di timeout e le eccezioni di pianificazione.

   Se, ad esempio, si visualizza il Planner risorse per settimana e si dispone di attività che si estendono per più settimane sui progetti, il numero di ore pianificate per settimana dipende dal numero di giorni all&#39;interno di tale settimana che fanno parte dell&#39;attività Durata. Questo funziona in modo simile quando si visualizza il Planner risorse per mese o trimestre e quando le attività si estendono su più mesi o trimestri.\
   I giorni di fine settimana, le eccezioni di pianificazione e i giorni di timeout sono esclusi da questa distribuzione.

* Le seguenti categorie di attività sono incluse nel calcolo delle ore pianificate per ogni risorsa:

   * attività assegnate agli utenti in pool di risorse, ruoli di lavoro o team del progetto.

      >[!TIP]
      >
      >Se le attività vengono assegnate ai team, la relativa allocazione verrà visualizzata in **Nessun ruolo** e **Nessun utente** sezioni. È possibile visualizzare le ore pianificate associate ai team, ma non è possibile eseguire il budget delle ore, perché non sono associati ruoli e utenti alle attività.

* Le ore pianificate nel planner risorse non includono le ore pianificate associate ai seguenti elementi:

   * attività principali
   * attività non assegnate
   * quando **Includi ore da problemi** è disabilitata.

* Le ore pianificate non vengono visualizzate nel planner risorse se la durata dell&#39;attività o del problema è pari a zero.
* Le ore pianificate associate agli utenti disattivati non vengono visualizzate.

Per ulteriori informazioni su Orari pianificati e FTE nel Planner risorse, vedi [Panoramica delle informazioni su ore, FTE e costi nelle visualizzazioni Progetto e Ruolo del Planner risorse](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

### Colonna ACT (effettivo)

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
   <td> <p>Il tempo registrato dall'utente su tutte le attività o i problemi assegnati.</p> <p>Ciò include i seguenti elementi:</p> 
    <ul> 
     <li>Attività e problemi assegnati all'utente ma non associati ad alcun ruolo di lavoro.</li> 
     <li>Attività e problemi che non si trovano in progetti per i quali hai accesso a Gestisci. </li> 
    </ul> <p>Ciò include il tempo di accesso al progetto solo quando l’utente viene assegnato alle attività o ai problemi relativi a quel progetto.  </p> </td> 
  </tr> 
  <tr> 
   <td>Progetto </td> 
   <td> <p>Tempo registrato dall’utente su tutte le attività e i problemi assegnati al progetto.</p> <p>Ciò include ogni volta che hanno effettuato l’accesso direttamente al progetto.</p> <p>Ciò non include quanto segue:</p> 
    <ul> 
     <li> <p>Attività registrate al momento e problemi non assegnati ad alcun utente. </p> </li> 
     <li> <p>Tempo connesso alle attività principali. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Qual</td> 
   <td> <p>L'ora ha effettuato l'accesso a tutte le attività o i problemi assegnati all'utente in questo ruolo. </p> <p>Ciò non include quanto segue:</p> 
    <ul> 
     <li>Attività e problemi registrati nel tempo assegnati a questo ruolo ma non a questo utente in questo ruolo.</li> 
     <li>Registrato direttamente sul progetto o sulle attività principali. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Attività o problema </td> 
   <td> <p>L'ora di accesso alle attività e ai problemi da parte dell'utente che è anche assegnato a loro. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>L’intervallo di tempo registrato viene visualizzato nell’intervallo temporale corrispondente alla data di ingresso dell’ora, indipendentemente dall’intervallo temporale dell’attività, del problema o del progetto in cui vengono registrate le ore.

Per ulteriori informazioni sugli orari effettivi, vedi [Visualizza ore effettive](../../manage-work/tasks/task-information/actual-hours.md).

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
   <td> <p>La differenza tra le ore disponibili e pianificate o FTE dell’utente. </p> <p>La differenza Ora o FTE viene calcolata utilizzando la seguente formula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>Nota: Se il valore viene visualizzato in numeri rossi negativi, l’utente viene sovrapassegnato. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td>Queste informazioni non sono disponibili per il progetto. </td> 
  </tr> 
  <tr> 
   <td>Qual</td> 
   <td> <p>La differenza tra le ore disponibili e pianificate o FTE del ruolo di lavoro. </p> <p>La differenza Ora o FTE viene calcolata utilizzando la seguente formula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>Nota: Se il valore viene visualizzato in numeri rossi negativi, il ruolo viene sovrassegnato. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Attività o problema</td> 
   <td>Queste informazioni non sono disponibili per l'attività, il problema o il progetto. </td> 
  </tr> 
 </tbody> 
</table>

### Colonna % (Percentuale allocazione ore pianificate) {#the-planned-hours-allocation-percentage-column}

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
   <td> <p>L’assegnazione delle ore pianificate o degli ETP in percentuale delle ore disponibili. La percentuale dell'allocazione oraria pianificata viene calcolata utilizzando la seguente formula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>Lo stesso calcolo viene utilizzato per i valori FTE. </p> </td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td>Queste informazioni non sono disponibili per il progetto quando si applica il <strong>Visualizza per utente</strong> visualizzare il planner risorse.</td> 
  </tr> 
  <tr> 
   <td>Qual</td> 
   <td> L’assegnazione delle ore pianificate o degli ETP in percentuale delle ore disponibili. <p>La percentuale dell'allocazione oraria pianificata viene calcolata utilizzando la seguente formula:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>Lo stesso calcolo viene utilizzato per i valori FTE.</p></td> 
  </tr> 
  <tr> 
   <td>Attività o problema</td> 
   <td>Queste informazioni non sono disponibili per l'attività, il problema o il progetto. </td> 
  </tr> 
 </tbody> 
</table>

Se il valore dell’ora pianificata o dell’FTE è zero, l’allocazione percentuale è pari a 0%. Se il valore di Ore disponibili o FTE è zero, non è possibile calcolare l’Allocazione percentuale.

Per ulteriori informazioni su Orari pianificati e FTE e su come vengono visualizzati nel Planner risorse, vedi [Risorse di budget nel planner risorse utilizzando le visualizzazioni Progetto e Ruolo](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

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
