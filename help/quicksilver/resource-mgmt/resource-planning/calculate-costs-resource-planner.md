---
product-area: resource-management
navigation-topic: resource-planning
title: Calcolare i costi nel planner risorse
description: '''(Alina: ***Collegato alla pianificazione nell''articolo Planner risorse, Informazioni sulle aree del planner risorse. - non spostare/modificare/eliminare.)"'
author: Alina
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '1373'
ht-degree: 0%

---

# Calcolare i costi nel planner risorse

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

È possibile eseguire il budget delle risorse in Adobe Workfront Resource Planner utilizzando i valori Cost anziché i valori Hours o FTE. I valori di costo non sono disponibili per il **Visualizza per utente** nel planner risorse.

>[!IMPORTANT]
>
>Per visualizzare le informazioni sui costi nel planner risorse, è necessario associare utenti e ruoli di lavoro ai tassi di costo per ora.\
>Per ulteriori informazioni sull&#39;associazione dei tassi di costo per ora con i ruoli di lavoro, vedere [Creare e gestire ruoli di lavoro](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
>Per ulteriori informazioni sull&#39;associazione delle tariffe di costo per ora con gli utenti, consulta [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Prima di includere nel budget le risorse, assicurati di avere una buona comprensione di ciò che occorre fare (ore pianificate, FTE o Costo) e di quando gli utenti sono aperti al lavoro (ore disponibili, FTE o Costo).\
Per ulteriori informazioni su come comprendere le informazioni nel Planner risorse quando si esegue il budget per ore o FTE, vedere [Panoramica delle informazioni su ore, FTE e costi nelle visualizzazioni Progetto e Ruolo del Planner risorse](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro e superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l'accesso a Gestione risorse che include l'accesso a Modifica priorità e ore di budget nel Planner risorse</p> <p>Modificare l’accesso a Dati finanziari, Progetti e Utenti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Consente di gestire le autorizzazioni per i progetti per i quali si desidera assegnare il budget alle informazioni con la possibilità di gestire le finanze</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Visualizza le informazioni nel planner risorse per costo

Per impostazione predefinita, le informazioni sulla disponibilità e sull&#39;allocazione vengono visualizzate in ore nel Planner risorse.

Per visualizzare le informazioni disponibili, pianificate e a budget in base al costo nel planner risorse:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Risorsa**.
1. Vai a .
1. (Condizionale) Seleziona **Visualizza per progetto** o **Visualizza per ruolo**.\
   Per impostazione predefinita **Visualizza per progetto** è selezionato.\
   Le informazioni sull’allocazione e sulla disponibilità vengono visualizzate in ore.

1. Da **Ore** menu a discesa, seleziona **Costo**.

   Se non hai accesso ai dati finanziari nel tuo livello di accesso, questa opzione non è disponibile.\
   Se i progetti hanno una valuta diversa da quella di sistema, il costo per questi progetti viene visualizzato nel Planner risorse convertito nella valuta del sistema. L&#39;amministratore di sistema definisce la valuta di sistema.\
   Per ulteriori informazioni sulla configurazione della valuta del sistema in Workfront e sui tassi di conversione, vedi [Imposta i tassi di cambio](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).\
   ![cost_in_the_planner_with_no_budgeting.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## Calcola costo disponibile nel planner risorse

Per visualizzare i valori dei costi disponibili nel Planner risorse, è necessario disporre dei seguenti elementi:

* Tariffe orarie per utenti e ruoli
* Informazioni sulla disponibilità degli utenti.

   L’ottenimento di informazioni sulla disponibilità degli utenti dipende dal modo in cui l’amministratore di Workfront configura le Preferenze di gestione delle risorse.\
   Per ulteriori informazioni sul calcolo della disponibilità degli utenti e sull&#39;impostazione delle preferenze di gestione delle risorse, vedere [Configurare le preferenze di Gestione risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Nella tabella seguente viene illustrato come viene calcolato il costo disponibile nel planner risorse:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Costo disponibile</strong> </th> 
   <th><strong>Calcolo</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Costo disponibile utente</td> 
   <td> <p>Il costo disponibile per utente viene calcolato utilizzando la seguente formula:</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>NOTA</b>

Se nel profilo dell&#39;utente non è presente un tasso di costo per ora, nel calcolo viene utilizzato il tasso di costo per ora del ruolo di lavoro in cui sono elencati. Se l&#39;utente non ha alcun ruolo associato a tali ruoli, il costo utente disponibile è $0. </p> </td>
</tr> 
  <tr> 
   <td>Costo disponibile ruolo</td> 
   <td> <p>Il costo disponibile per ruolo viene calcolato utilizzando la seguente formula:</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>NOTA</b>

Se il ruolo non dispone di un tasso di costo per ora, il costo del ruolo disponibile è $0.</p> </td>
</tr> 
  <tr> 
   <td>Costo disponibile progetto</td> 
   <td> <p>Il costo disponibile per progetto viene calcolato utilizzando la seguente formula:</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Calcola costo pianificato nel planner risorse

Sebbene non sia possibile visualizzare le informazioni sulle attività nel Planner risorse, i costi pianificati per gli utenti, i ruoli e i progetti vengono calcolati tenendo conto delle seguenti informazioni sulle attività:

* Tipo di assegnazione dell&#39;attività.\
   È possibile lasciare un&#39;attività non assegnata o assegnare le seguenti entità a un&#39;attività:

   * Un utente (con o senza un ruolo di lavoro)
   * Un ruolo
   * Un team\
      Un&#39;attività assegnata a un team viene considerata non assegnata, dal punto di vista del Planner risorse.

* La **Tipo di costo** dei compiti del progetto.\
   Per ulteriori informazioni sul tipo di costo di un&#39;attività, vedere [Costi di tracciamento](../../manage-work/projects/project-finances/track-costs.md).

>[!NOTE]
>
>I costi pianificati dall&#39;utente non influiscono sul costo pianificato del progetto. Solo i costi pianificati per il ruolo influiscono sui costi pianificati del progetto, nel Planner risorse.

Esistono i seguenti scenari durante il calcolo del costo pianificato per utenti, ruoli e progetto:

* Quando il **Tipo di costo** è **Utente ogni ora **ed è presente **nessuna assegnazione** sull&#39;attività:

   * **Ruolo e costo pianificato utente**:

      I costi pianificati per Ruolo e Utente sono pari a $ 0,00.

   * **Costo pianificato progetto**:

      Il costo pianificato del progetto è $0,00.

* Quando il **Tipo di costo** è **Utente orario** e c&#39;è un **assegnazione utente** sull&#39;attività:

   * **Ruolo e costo pianificato utente**:

      Il costo pianificato dall&#39;utente viene calcolato utilizzando la seguente formula:



      ```
      User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate
      ```

      Se un utente ha un tasso di costo nel proprio profilo, tale tasso viene utilizzato per calcolare il costo pianificato. In caso contrario, viene utilizzato il tasso di costo per ora a livello di sistema del ruolo principale.

      >[!NOTE]
      >
      >L’utente può essere assegnato all’attività con uno dei propri ruoli di lavoro secondari, ma in questo caso viene utilizzato il tasso del ruolo di lavoro principale.

      Il costo pianificato per il ruolo viene calcolato utilizzando la seguente formula:

      ```
      Role Planned Cost = SUM(User Planned Cost)
      ```

   * **Costo pianificato progetto**:

      Il costo pianificato del progetto è $0,00.

* Quando il **Tipo di costo** è **Utente orario** e c&#39;è un **assegnazione ruolo** sull&#39;attività:

   * **Ruolo e costo pianificato utente**:

      Il costo pianificato dall&#39;utente è $0,00.

      Il costo pianificato per il ruolo viene calcolato utilizzando la seguente formula:

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      Il tasso di costo per ora a livello di sistema del ruolo di lavoro assegnato all&#39;attività viene utilizzato per calcolare il costo pianificato.

   * **Costo pianificato progetto**:

      Il costo pianificato del progetto è $0,00.

* Quando il **Tipo di costo** è **Ruolo orario** e **nessuna assegnazione** sull&#39;attività:

   * **Ruolo e costo pianificato utente**:

      I costi pianificati per Ruolo e Utente sono pari a $ 0,00.

   * **Costo pianificato progetto**:

      Il costo pianificato del progetto è $0,00.

* Quando il **Tipo di costo** è **Ruolo orario** e c&#39;è un **assegnazione utente** sull&#39;attività:

   * **Ruolo e costo pianificato utente**:

      Il costo pianificato dall&#39;utente è $0,00.

      Il costo pianificato per il ruolo viene calcolato dalla seguente formula:

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      Per calcolare il costo pianificato per il ruolo, Workfront esamina il ruolo dell’utente che esegue l’attività.

      Se l&#39;utente non è associato ad alcun ruolo sull&#39;attività, il costo pianificato è di $0,00.

   * **Costo pianificato progetto**:

      Il costo pianificato del progetto viene calcolato utilizzando la seguente formula:

      ```
      Project Planned Cost = SUM(Role Planned Costs)
      ```

* Quando il **Tipo di costo** è **Ruolo orario** e c&#39;è un **assegnazione ruolo** sull&#39;attività:

   * **Ruolo e costo pianificato utente**:

      Il costo pianificato dall&#39;utente è $0,00.

      Il costo pianificato per il ruolo viene calcolato dalla seguente formula:

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      Per calcolare il costo pianificato per il ruolo, Workfront esamina il ruolo dell’utente che esegue l’attività.

   * **Costo pianificato progetto**:

      Il costo pianificato del progetto viene calcolato utilizzando la seguente formula:

      ```
      Project Planned Cost = SUM(Role Planned Costs)
      ```

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(table below ideal but drafted because it does not display correctly in Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td rowspan="2">&nbsp;</td>
<td colspan="3"> <p><strong>Cost Type = User Hourly</strong> </p><strong>User Planned Cost</strong> </td>
<td colspan="3"> <p><strong>Cost Type = Role Hourly</strong> </p><strong>Role Planned Cost</strong> </td>
</tr>
<tr>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>User and Role Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is calculated using the following formula: </p> <p><code> User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate </code> </p> <p> If a user has a cost rate in their profile, then that rate is used to calculate Planned Cost. Otherwise, the system-level Cost per Hour rate of their Primary Role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code>Role Planned Cost = SUM(User Planned Cost)</code> </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code> Role Planned Cost = Role Planned Hours * Role Cost per Hours </code> </p> <p> The system-level Cost per Hour rate of the job role assigned to the task is used to calculate Planned Cost. </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> If the user is not associated with any role on the task, the Planned Cost is $0.00. </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td rowspan="2"> <p><strong>Project Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td colspan="2"> <p> The Project Planned Cost is calculated using the following formula: </p> <p><code> Project Planned Cost = SUM(Role Planned Costs) </code> </p> <p> </p> </td>
</tr>
<tr>
<td colspan="6"> <note type="note">
User Planned Costs do not influence the Project Planned Cost. Only the Role Planned costs affect the Project Planned Costs, in the Resource Planner.
</note> </td>
</tr>
</tbody>
</table>
-->

## Calcola costo preventivato nel planner risorse

Per visualizzare i valori dei costi a budget nel Planner risorse, è necessario disporre dei seguenti elementi:

* Ore previste per ruoli, utenti e progetti.
* Tariffe orarie per utenti e ruoli.

>[!NOTE]
>
>Le ore previste per i progetti vengono calcolate in base alle ore previste per i ruoli e non a quelle degli utenti.

Nella tabella seguente viene illustrato come viene calcolato il costo preventivato nel planner risorse:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Bdg prv</strong> </th> 
   <th><strong>Calcolo</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Costo a budget utente</td> 
   <td> <p>Il costo a budget per utente viene calcolato utilizzando la seguente formula:</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>NOTA</b>

Se nel profilo dell&#39;utente non è presente un tasso di costo per ora, il costo per l&#39;utente in budget è $0,00.</p> </p> </td>
</tr> 
  <tr> 
   <td>Costo preventivato ruolo</td> 
   <td> <p>Il costo preventivato ruolo viene calcolato utilizzando la seguente formula:</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>NOTA</b>

Se il ruolo non dispone di un tasso di costo per ora, il costo del ruolo a budget è $0,00.</p> </p> </td>
</tr> 
  <tr> 
   <td>Costo preventivato progetto</td> 
   <td> <p>Il costo preventivato per progetto viene calcolato utilizzando la seguente formula:</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
