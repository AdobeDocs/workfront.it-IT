---
product-area: resource-management
navigation-topic: resource-planning
title: Calcola costi nella programmazione delle risorse
description: È possibile preventivare le risorse in Adobe Workfront Resource Planner utilizzando i valori Costo anziché i valori Ore o FTE. I valori dei costi non sono disponibili per la visualizzazione **Visualizza per utente** nella Programmazione risorse.
author: Lisa
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: 3c3175c347431b10aed1a6034df6c756056399b3
workflow-type: tm+mt
source-wordcount: '1421'
ht-degree: 0%

---

# Calcola i costi nella Programmazione delle risorse

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

<!--'(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)'-->

È possibile preventivare le risorse in Adobe Workfront Resource Planner utilizzando i valori Costo anziché i valori Ore o FTE. I valori di costo non sono disponibili per la visualizzazione **Visualizza per utente** nella Programmazione delle risorse.

>[!IMPORTANT]
>
>È necessario associare utenti e mansioni alle tariffe Costo orario per visualizzare le informazioni sul costo nella Programmazione delle risorse.\
>Per ulteriori informazioni sull&#39;associazione delle tariffe orarie con le mansioni, vedere [Creare e gestire le mansioni](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
>Per ulteriori informazioni sull&#39;associazione delle tariffe orarie con gli utenti, vedere [Modificare il profilo di un utente](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Prima di definire il budget delle risorse, accertati di avere una buona conoscenza del lavoro da eseguire (ore pianificate, FTE o costo) e degli orari in cui gli utenti sono aperti al lavoro (ore disponibili, FTE o costo).\
Per ulteriori informazioni sulla comprensione delle informazioni nella Programmazione delle risorse durante la definizione del budget per ore o FTE, vedere [Panoramica sulle ore, FTE e informazioni sui costi nelle visualizzazioni Progetto e Ruolo della Programmazione delle risorse](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
    <td><p>Nuovo: Qualsiasi</p>
       <p>oppure</p>
       <p>Corrente: Pro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>oppure</p>
       <p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso a Gestione risorse, incluso l'accesso a Modifica priorità e ore preventivate nella Programmazione risorse</p> <p>Modifica accesso a dati finanziari, progetti e utenti</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per i progetti per i quali si desidera preventivare le informazioni con la possibilità di gestire le finanze</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizza informazioni nella Programmazione risorse per costo

Per impostazione predefinita, le informazioni sulla disponibilità e sull&#39;allocazione vengono visualizzate in Ore nella Programmazione delle risorse.

Per visualizzare le informazioni Disponibili, Pianificate e Preventivate per Costo nella Programmazione risorse:

{{step1-to-resourcing}}

1. Vai alla Programmazione delle risorse.
1. (Condizionale) Selezionare **Visualizza per progetto** o **Visualizza per ruolo**.\
   Per impostazione predefinita è selezionata l&#39;opzione **Visualizza per progetto**.\
   Le informazioni sull&#39;allocazione e sulla disponibilità vengono visualizzate in Ore.

1. Dal menu a discesa **Ore**, selezionare **Costo**.

   Se non si dispone dell&#39;accesso ai dati finanziari nel proprio livello di accesso, questa opzione non è disponibile.\
   Se i progetti hanno una valuta diversa rispetto a quella di sistema, il Costo per questi progetti viene visualizzato in Pianificazione risorse convertito nella valuta del sistema. L&#39;amministratore di sistema definisce la valuta di sistema.\
   Per ulteriori informazioni sull&#39;impostazione della valuta di sistema in Workfront e sui tassi di conversione, vedere [Impostare i tassi di cambio](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).\
   ![cost_in_the_planner_with_no_budgeting.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## Calcola costo disponibile nella Programmazione delle risorse

Per visualizzare i valori di Costo disponibile nella Programmazione delle risorse, è necessario disporre dei seguenti elementi:

* Tariffe del costo orario per utenti e ruoli
* Informazioni sulla disponibilità degli utenti.

  L&#39;ottenimento di informazioni sulla disponibilità degli utenti dipende dal modo in cui l&#39;amministratore di Workfront configura le preferenze di gestione delle risorse.\
  Per ulteriori informazioni sul calcolo della disponibilità utente e sull&#39;impostazione delle preferenze di Gestione risorse, vedere [Configurare le preferenze di Gestione risorse](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Nella tabella seguente viene illustrato il calcolo del costo disponibile nella Programmazione delle risorse:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Costo Disponibile</strong> </th> 
   <th><strong>Calcolo</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Costo disponibile utente</td> 
   <td> <p>Il costo disponibile per utente viene calcolato utilizzando la formula seguente:</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>NOTA</b>

Se nel profilo dell&#39;utente non è presente una tariffa Costo orario, nel calcolo verrà utilizzata la tariffa Costo orario della mansione con cui è elencato l&#39;utente. Se all&#39;utente non è associato alcun ruolo, il costo utente disponibile è $0. </p> </td>
</tr> 
  <tr> 
   <td>Costo disponibile ruolo</td> 
   <td> <p>Il costo disponibile per ruolo viene calcolato utilizzando la formula seguente:</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>NOTA</b>

Se per il ruolo non è disponibile una tariffa Costo orario, il costo disponibile per il ruolo è pari a $0.</p> </td>
</tr> 
  <tr> 
   <td>Costo disponibile progetto</td> 
   <td> <p>Il costo disponibile per progetto viene calcolato utilizzando la seguente formula:</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Calcola costo pianificato nella Programmazione delle risorse

Sebbene non sia possibile visualizzare le informazioni sulle attività nella Programmazione delle risorse, i costi pianificati per utenti, ruoli e progetti vengono calcolati tenendo conto delle seguenti informazioni sulle attività:

* Tipo di assegnazione per l&#39;attività.\
  È possibile lasciare un&#39;attività non assegnata o assegnare le seguenti entità a un&#39;attività:

   * Un utente (con o senza una mansione)
   * Un Ruolo
   * Un team\
     Un&#39;attività assegnata a un team viene considerata non assegnata dal punto di vista della programmazione delle risorse.

* Il **Tipo di costo** delle attività nel progetto.\
  Per ulteriori informazioni sul tipo di costo di un&#39;attività, vedere [Tracciare i costi](../../manage-work/projects/project-finances/track-costs.md).

* Le date di validità dei tassi di costo per mansioni e utenti.

  Ad esempio, se il ruolo o l&#39;utente ha 10 ore pianificate in febbraio e 10 ore pianificate in marzo, ma il tasso di costo è cambiato da 12 a 20 dollari in marzo, il valore per il costo pianificato in febbraio è 120 dollari e in marzo è 200 dollari.

>[!NOTE]
>
>I costi pianificati dall&#39;utente non influiscono sul costo pianificato del progetto. Solo i costi pianificati per ruolo influiscono sui costi pianificati del progetto nella pianificazione risorse.

Per calcolare il costo pianificato per utenti, ruoli e progetto sono disponibili i seguenti scenari:

* Quando il **Tipo di costo** è **Ore utente **e non è presente **alcuna assegnazione** nell&#39;attività:

   * **Costo pianificato per ruolo e utente**:

     I costi pianificati per ruolo e utente sono pari a $ 0,00.

   * **Costo pianificato progetto**:

     Il costo pianificato del progetto è di $0,00.

* Quando il tipo di costo **Tipo di costo** è **Ore utente** ed è presente un&#39;assegnazione **utente** per l&#39;attività:

   * **Costo pianificato per ruolo e utente**:

     Il costo pianificato dall&#39;utente viene calcolato utilizzando la formula seguente:

     `User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate`

     Se nel profilo di un utente è presente una tariffa, questa viene utilizzata per calcolare il costo pianificato. In caso contrario, viene utilizzato il tasso di costo orario a livello di sistema per il ruolo principale.

     >[!NOTE]
     >
     >L’utente può essere assegnato all’attività con una delle sue mansioni secondarie, ma in questa posizione viene utilizzato il tasso della mansione principale.

     Il costo pianificato del ruolo viene calcolato utilizzando la formula seguente:

     `Role Planned Cost = SUM(User Planned Cost)`

   * **Costo pianificato progetto**:

     Il costo pianificato del progetto è di $0,00.

* Quando il tipo di costo **Tipo di costo** è **Ore utente** ed è presente un&#39;assegnazione di ruolo **** per l&#39;attività:

   * **Costo pianificato per ruolo e utente**:

     Il costo pianificato dell&#39;utente è di $0,00.

     Il costo pianificato del ruolo viene calcolato utilizzando la formula seguente:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     La tariffa oraria a livello di sistema per la mansione assegnata all&#39;attività viene utilizzata per calcolare il costo pianificato.

   * **Costo pianificato progetto**:

     Il costo pianificato del progetto è di $0,00.

* Quando il **Tipo di costo** è **Ore ruolo** e non è presente **alcuna assegnazione** sull&#39;attività:

   * **Costo pianificato per ruolo e utente**:

     I costi pianificati per ruolo e utente sono pari a $ 0,00.

   * **Costo pianificato progetto**:

     Il costo pianificato del progetto è di $0,00.

* Quando il **Tipo di costo** è **Ore ruolo** ed è presente un **assegnazione utente** sull&#39;attività:

   * **Costo pianificato per ruolo e utente**:

     Il costo pianificato dell&#39;utente è di $0,00.

     Il costo pianificato del ruolo viene calcolato con la formula seguente:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Per calcolare il costo pianificato per il ruolo, Workfront esamina il ruolo che l&#39;utente svolge nell&#39;attività.

     Se l&#39;utente non è associato ad alcun ruolo nell&#39;attività, il costo pianificato è $0,00.

   * **Costo pianificato progetto**:

     Il costo pianificato del progetto viene calcolato utilizzando la formula seguente:

     `Project Planned Cost = SUM(Role Planned Costs)`

* Quando il **Tipo di costo** è **Ore ruolo** ed è presente un **assegnazione mansione** sull&#39;attività:

   * **Costo pianificato per ruolo e utente**:

     Il costo pianificato dell&#39;utente è di $0,00.

     Il costo pianificato del ruolo viene calcolato con la formula seguente:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Per calcolare il costo pianificato per il ruolo, Workfront esamina il ruolo che l&#39;utente svolge nell&#39;attività.

   * **Costo pianificato progetto**:

     Il costo pianificato del progetto viene calcolato utilizzando la formula seguente:

     `Project Planned Cost = SUM(Role Planned Costs)`

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

## Calcola costo preventivato nella Programmazione delle risorse

Per visualizzare i valori di Costo preventivato nella Programmazione delle risorse, è necessario disporre dei seguenti elementi:

* Ore preventivate per ruoli, utenti e progetti.
* Tariffe del costo orario per utenti e ruoli.

>[!NOTE]
>
>Le ore preventivate per i progetti vengono calcolate in base alle ore preventivate per i ruoli, non a quelle degli utenti.

Nella tabella seguente viene illustrato come viene calcolato il Costo preventivato nella Programmazione risorse:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Costo preventivato</strong> </th> 
   <th><strong>Calcolo</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Costo preventivato utente</td> 
   <td> <p>Il costo preventivato per utente viene calcolato utilizzando la formula seguente:</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>NOTA</b>

Se l&#39;utente non ha una tariffa Costo all&#39;ora nel suo profilo, il Costo utente preventivato è $0,00.</p> </p> </td>
</tr> 
  <tr> 
   <td>Costo preventivato mansione</td> 
   <td> <p>Il costo preventivato ruolo viene calcolato utilizzando la formula seguente:</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>NOTA</b>

Se per il ruolo non è disponibile una tariffa Costo orario, il costo del ruolo preventivato è pari a $ 0,00.</p> </p> </td>
</tr> 
  <tr> 
   <td>Costo preventivato progetto</td> 
   <td> <p>Il Costo preventivato per progetto viene calcolato utilizzando la seguente formula:</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
