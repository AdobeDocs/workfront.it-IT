---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: Costi di tracciamento
description: In Adobe Workfront puoi tenere traccia dei costi per progetti, attività e problemi.
author: Alina
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: 7e78ca8c8ea7f037b55b06e7452ac5c562b99eca
workflow-type: tm+mt
source-wordcount: '2418'
ht-degree: 1%

---

# Costi di tracciamento

In Adobe Workfront puoi tenere traccia dei costi per progetti, attività e problemi.

## Modalità di calcolo dei costi in Workfront

Per tenere traccia dei costi, è necessario associare utenti e ruoli di lavoro ai tassi di costo orari.

I tassi di costo orari sono importi di costi per unità di lavoro associati a ruoli di lavoro o utenti. Moltiplicare i tassi per le ore di lavoro genera costi per i progetti, le attività o i problemi.

Esistono i seguenti scenari:

* Se il tipo di costo delle attività è Orario utente, la tariffa oraria dell&#39;utente calcola i costi di attività e progetto.

   Per informazioni sull&#39;associazione degli utenti ai tassi di costo, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Se il tipo di costo delle attività è impostato su Ruolo orario, la frequenza oraria del ruolo dell&#39;OdL calcola i costi dell&#39;attività e del progetto.

   Per informazioni sull&#39;associazione dei ruoli di lavoro ai tassi di costo, vedere [Creare e gestire ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront calcola solo il costo effettivo per i problemi e i problemi privi di un tipo di costo. Per ulteriori informazioni, consulta la sezione . [Come Workfront tiene traccia dei costi per i problemi](#how-workfront-tracks-costs-for-issues) in questo articolo.

>[!TIP]
>
>Non è possibile sostituire i tassi di costo per i progetti. Una volta stabilito il tasso di costo per ora su un ruolo utente o lavoro, tale tasso calcola tutti i costi nel sistema.

## Indice delle prestazioni dei costi Workfront

Workfront calcola una serie di indici delle prestazioni dei costi per i progetti, in modo che i progetti possano essere monitorati in modo da garantire l’efficienza in termini di costi.\
Per ulteriori informazioni sul calcolo degli indici costi-prestazioni, consulta:

* [Calcola indice di prestazione dei costi (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [Calcola indice prestazioni pianificazione costi (CSI)](../../../manage-work/projects/project-finances/calculate-csi.md)
* [Calcola indice delle prestazioni della pianificazione (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)

## Come Workfront tiene traccia dei costi per attività e progetti

* [Come Workfront tiene traccia dei costi](#how-workfront-tracks-costs)
* [Modalità di calcolo dei costi pianificati, preventivati e effettivi da parte di Workfront](#how-workfront-calculates-planned-budgeted-and-actual-costs)
* [Modalità di calcolo dei tipi di costo per le attività in Workfront](#how-workfront-calculates-cost-types-for-tasks)

### Come Workfront tiene traccia dei costi  {#how-workfront-tracks-costs}

È possibile tenere traccia di diversi tipi di costi per attività e progetti in Workfront. I costi globali sono calcolati con la seguente formula:

```
Costs = Labor Costs + Expense Costs
```

* **Costi del lavoro** sono associati alle ore relative a attività e progetti e ai tassi di costo per ora delle risorse associate alle attività. In genere, Workfront calcola i seguenti costi di manodopera:

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Costi pianificati del lavoro</td> 
     <td> <p>Vengono calcolati con la seguente formula:</p><pre>Costi del lavoro pianificati = ore programmate * Costo per ora</pre> </td> 
    </tr> 
    <tr> 
     <td>Costi del lavoro a budget</td> 
     <td> <p>Vengono calcolati con la seguente formula:</p><pre>Costi manodopera a budget = ore a budget * Costo per ora</pre> </td> 
    </tr> 
    <tr> 
     <td>Costi effettivi del lavoro</td> 
     <td> <p>Vengono calcolati con la seguente formula:</p><pre>Costi effettivi del lavoro = ore effettive * Costo per ora</pre> </td> 
    </tr> 
   </tbody> 
  </table>

   Per ulteriori informazioni, consulta la sezione [Modalità di calcolo dei costi pianificati, preventivati e effettivi da parte di Workfront](#how-workfront-calculates-planned-budgeted-and-actual-costs) in questo articolo.

* **Costi di spesa** sono associati a spese relative a progetti e attività.\
   Quando crei un progetto, puoi impostare le spese pianificate per l’intero progetto. È inoltre possibile associare le spese a attività nuove o esistenti. Per informazioni, consulta [Gestione delle spese di progetto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **Costi fissi** sono definiti come un importo fisso di costo per un progetto. Questo fa parte del Costo pianificato del progetto, che rappresenta l’importo necessario per completare il progetto.

   >[!TIP]
   >
   >Quando si allega un modello a un progetto, il costo fisso di un modello viene aggiunto al costo fisso del progetto. Per informazioni, consulta [Panoramica sull’associazione di un modello a un progetto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### Modalità di calcolo dei costi pianificati, preventivati e effettivi da parte di Workfront {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront calcola il costo pianificato e il costo effettivo per ogni singola attività di un progetto. Workfront utilizza questi calcoli per le singole attività per calcolare il costo pianificato e il costo effettivo per il progetto.

* [Costo Pianificato](#planned-cost)
* [Bdg prv](#budgeted-cost)
* [Costo Reale](#actual-cost)

#### Costo Pianificato {#planned-cost}

Il costo pianificato di un progetto è il costo associato al lavoro pianificato (ore pianificate) relativo al progetto.

Il costo pianificato di un progetto viene calcolato con la seguente formula:

```
Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project
```

Ad esempio, nella scheda Spese di un&#39;attività sono disponibili le seguenti spese: una spesa di marketing da 100 dollari e una spesa amministrativa da 50 dollari. Nella scheda Finanza selezionare il tipo di costo orario utente. Un utente viene assegnato all&#39;attività e la tariffa oraria dell&#39;utente è di $ 15. L&#39;utente viene assegnato a lavorare 5 ore su questa attività. Nella scheda Spese del progetto è disponibile un costo pianificato di $100 per una spesa denominata Consulting. Hai anche un costo fisso di $ 200 per il progetto.

Il costo pianificato del progetto viene calcolato come segue:

```
$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525
```

#### Bdg prv {#budgeted-cost}

Il costo preventivato di un progetto è il costo associato al lavoro a budget (ore a budget) relativo al progetto.

Il costo preventivato del progetto è uguale al costo pianificato del progetto se sono soddisfatte le due condizioni seguenti:

* Le ore pianificate delle attività del progetto corrispondono alle ore previste (nel Planner risorse)
* Il tipo di fatturazione dell&#39;attività è Ruolo orario.

Il costo preventivato del progetto viene calcolato utilizzando la formula seguente se sono soddisfatte le seguenti condizioni:

* Le ore pianificate delle attività del progetto non corrispondono alle ore previste (nel planner risorse)
* Il tipo di fatturazione delle attività è Ruolo orario.

Quando vengono soddisfatte le condizioni di cui sopra, Workfront calcola il costo preventivato del progetto utilizzando la seguente formula:
<pre>Costo progetto a budget = Costo manodopera a budget + Costo spesa a budget di tutte le attività + Costo spesa a budget del progetto</pre>

#### Costo Reale {#actual-cost}

Il costo effettivo di un progetto è il costo associato al lavoro effettivo (ore registrate) sul progetto.

Il costo effettivo viene calcolato utilizzando la formula seguente:

```
Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project
```

Ad esempio, nella scheda Spese di un&#39;attività sono disponibili le seguenti spese: una spesa di marketing con un costo effettivo di $ 110 e una spesa amministrativa con un costo effettivo di $ 40. Selezionare il tipo di costo Orario ruolo e assegnare il ruolo di lavoro Consulente all&#39;attività. Il tasso del ruolo di consulente è di $15 all&#39;ora, e ci sono 6 ore registrate sull&#39;attività per il ruolo di lavoro di Consultant. È presente una spesa di consulenza associata al progetto (nella scheda Spese ), con un costo effettivo di $ 100 e un utente con un tasso di costo per ora di $ 20 nel proprio profilo utente registra 10 ore sul progetto. Hai anche un costo fisso di $ 200 per il progetto.

Il costo effettivo del progetto viene calcolato come segue:

```
$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740
```

>[!NOTE]
>
>Il costo effettivo del progetto viene calcolato come segue:
>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>Questi costi non vengono duplicati nel calcolo del costo effettivo. Ad esempio, se un costo fisso fa parte del costo effettivo del progetto, non viene aggiunto separatamente al costo effettivo.

>[!NOTE]
>
>Quando si registra il tempo in un progetto, quando si calcola il costo effettivo del lavoro per il progetto sono disponibili i seguenti scenari:
>
>* Per impostazione predefinita, Workfront utilizza il tasso di costo per ora dell’utente per calcolare il costo effettivo del lavoro.
>* Se l’utente che registra il tempo non è associato ad alcun costo, Workfront utilizza il tasso di costo per ora del ruolo principale dell’utente.
>* Se l’amministratore di Workfront ha abilitato la **Assegnare manualmente i ruoli del processo alle voci orarie** nell’area Preferenze fogli orari e ore e il tempo di registrazione dell’utente sul progetto seleziona un ruolo diverso da associare a questo momento, il costo effettivo del progetto viene calcolato in base al ruolo specificato al momento della registrazione delle ore. Per informazioni sull’abilitazione del tempo di registrazione per un ruolo di lavoro specifico, consulta l’articolo [Configurare le preferenze relative a schede attività e ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).


### Modalità di calcolo dei tipi di costo per le attività in Workfront {#how-workfront-calculates-cost-types-for-tasks}

Il costo pianificato e effettivo delle attività e i relativi costi manodopera sono determinati dal tipo di costo di ciascuna attività.

È possibile configurare il tipo di costo per le singole attività all&#39;interno del progetto. Ciascun tipo di costo influisce sui valori Costo pianificato e Costo effettivo.

Per informazioni su come modificare il tipo di costo di un&#39;attività, vedere [Aggiorna tipo di costo attività](../../../manage-work/tasks/task-information/update-task-cost-type.md).

Nella tabella seguente sono descritti i tipi di costo dell&#39;attività disponibili in Workfront:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tipo di costo attività</strong> </p> </th> 
   <th> <p><strong>Descrizione</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Ore Utente</p> </td> 
   <td> <p>Questo è il tipo di costo predefinito quando si crea un'attività.</p> <p><strong>Costo pianificato</strong> è calcolato con la seguente formula: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Se il costo del lavoro pianificato è calcolato da:<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>Nota:   <p>Considera i seguenti impatti derivanti dall’utilizzo del tipo di costo orario utente e dal calcolo del costo pianificato:</p> 
     <ul> 
      <li>Se si assegnano più risorse a un'attività, Workfront adegua i calcoli relativi al costo pianificato in base alla percentuale dell'attività assegnata a ciascuna risorsa.</li> 
      <li>Il valore del campo Costo pianificato può variare a seconda che il costo pianificato venga visualizzato dall'attività stessa o dal rapporto Utilizzo.<br><strong>Quando si visualizza Costo pianificato dall'attività stessa:</strong> Il campo Costo pianificato prende in considerazione il campo Costo/ora impostato a livello di Ruolo lavoro (quando il campo Costo/ora non è stato impostato a livello di utente).<br><strong>Quando si visualizza Costo pianificato dal rapporto Utilizzo relativo al progetto:</strong> Il campo Costo pianificato non tiene conto del campo Costo/ora impostato a livello di Ruolo lavoro. Se invece si desidera che il rapporto Utilizzo tenga conto del campo Costo/ora impostato a livello di Ruolo lavoro, è necessario impostare il tipo di costo per l'attività su Ruolo orario. </li> 
     </ul> </p> <p><strong>Costo effettivo</strong> è calcolato con la seguente formula: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Se il costo effettivo del lavoro è calcolato da:</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>Ad esempio, un utente ha un tasso di costo per ora di $ 20 nel suo profilo. Quando si registrano 5 ore per un'attività, il costo effettivo del lavoro è di 100 $ per tale attività. Se all'utente non è associato un tasso di costo per ora, il costo effettivo viene calcolato in base al tasso di costo per ora del ruolo di lavoro principale. Se non dispongono di un ruolo di lavoro o il tasso di costo per ora del ruolo di lavoro non è definito, il costo effettivo dell'attività è zero. </p> <p>Nota: I costi effettivi vengono calcolati in base al tasso di costo per ora per l'utente che registra il tempo, indipendentemente da chi è assegnato all'attività. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ore Ruolo</p> </td> 
   <td> <p><strong>Costo pianificato</strong> è calcolato con la seguente formula: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>Se il costo del lavoro pianificato dell'attività viene calcolato da:</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Nota: Se si assegnano più risorse a un'attività, Workfront adegua i calcoli relativi alle ore pianificate in base alla percentuale dell'attività assegnata a ciascuna risorsa.</p> <p><strong>Costo effettivo</strong> è calcolato con la seguente formula: </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Se il costo effettivo del lavoro dell'attività è calcolato da:</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Ad esempio, un'attività viene assegnata a un ruolo di lavoro o a un utente con un ruolo di lavoro per il quale il tasso di costo per ora è di $20. Quando un utente registra 5 ore per un'attività, il costo effettivo del lavoro è di $100 per tale attività. Se l'utente assegnato all'attività non dispone di un ruolo di lavoro associato all'attività, il costo effettivo viene calcolato in base al tasso di costo per ora del ruolo di lavoro principale. Se non dispongono di un ruolo di lavoro o il tasso di costo per ora del ruolo di lavoro non è definito, il costo effettivo dell'attività è zero. </p> <p>Nota:   <p> Le ore effettive di un'attività Orario ruolo vengono calcolate in base ai ruoli del lavoro degli utenti associati all'attività, non in base ai ruoli associati all'utente che registra l'ora.</p> <p>Se l’amministratore di Workfront ha abilitato la <strong>Assegnare manualmente i ruoli del processo alle voci orarie</strong> nell'area Preferenze fogli orari e ore e il tempo di registrazione dell'utente sull'attività seleziona un ruolo diverso da associare a questo momento, il costo effettivo di un'attività Orario ruolo viene calcolato in base al ruolo specificato al momento della registrazione delle ore. Per informazioni sull’abilitazione del tempo di registrazione per un ruolo di lavoro specifico, consulta l’articolo <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configurare le preferenze relative a schede attività e ora</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ore Fisse</p> </td> 
   <td> <p><strong>Costo pianificato</strong> è calcolato con la seguente formula:</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Se il costo del lavoro dell'attività viene calcolato da:</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>Costo effettivo</strong> è calcolato con la seguente formula: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>Se il costo manodopera attività effettiva è calcolato da:</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>Questo tipo di costo non tiene conto dei singoli utenti o ruoli di lavoro.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nessun Costo</p> </td> 
   <td> <p>Questo tipo di costo non influisce sui costi. Se un'attività padre dispone di questo tipo di costo, le sottoattività con un altro tipo di costo vengono calcolate in base ai singoli tipi di costo e il costo dell'attività padre viene influenzato di conseguenza. </p> <p>Quando un utente senza accesso ai dati finanziari o senza autorizzazioni finanziarie in un modello crea un progetto a partire da tale modello, si tratta del tipo di costo predefinito per le attività del progetto.</p> <p>Per informazioni sull'accesso ai dati finanziari, vedere l'articolo <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Concedere l’accesso ai dati finanziari</a>.</p> <p>Per informazioni sulle autorizzazioni finanziarie per gli oggetti, consulta l’articolo <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Condividere le autorizzazioni finanziarie su un oggetto</a>.</p> <p>Per informazioni sulla creazione di progetti da modelli, consulta l’articolo <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Creare un progetto utilizzando un modello</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because this was moved to its own how-to article linked above. Could be removed after some time.) </p>
<p>To configure the Cost Type of an individual task:</p>
<ol>
<li value="1">Go to the task where you want to configure the Cost Type. </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then expand the <strong>Finance</strong> area. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Double click <strong>Cost Type</strong> and select the cost type that you want to apply to the task. </p> </li>
<li value="4">Click <strong>Save.</strong></li>
</ol>
</div>
-->

## Come Workfront tiene traccia dei costi per i problemi {#how-workfront-tracks-costs-for-issues}

I problemi non hanno e non influiscono sui seguenti tipi di costi di un progetto:

* Costo Pianificato
* Bdg prv

I problemi possono tuttavia avere un **Costo effettivo** che influisce anche sul costo effettivo del progetto.

Nella tabella seguente viene illustrato come viene calcolato il costo effettivo per i problemi, a seconda del tipo di assegnazione relativa al problema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th colspan="4">Costo effettivo del problema</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Assegnazione utente</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Costo effettivo</strong> è calcolato con la seguente formula:</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Il tasso di costo per ora dell’utente che registra il tempo viene preso in considerazione qui, indipendentemente da chi è assegnato al problema. </p> <p>Se l'utente che registra il tempo non ha un tasso di costo per ora nel proprio profilo, il tasso di costo per ora del ruolo di lavoro principale calcola il costo effettivo del problema. Se l'utente che registra l'ora non ha alcun ruolo nel proprio profilo o nessun tasso associato, le ore effettive vengono calcolate utilizzando il tasso Costo per ora del ruolo principale dell'assegnatario principale sul problema. Se il ruolo non ha un tasso definito, il costo effettivo del problema è zero. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Assegnazione ruolo</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Costo effettivo</strong> è calcolato con la seguente formula:</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>Il tasso di costo per ora dell’utente che registra il tempo sul problema viene preso in considerazione qui, indipendentemente dal ruolo assegnato al problema. </p> <p>Se l'utente che registra l'ora non ha un tasso di costo per ora associato, il tasso di costo per ora del ruolo principale calcola il costo effettivo del problema.<br>Se l'utente che registra l'ora non ha alcun ruolo nel proprio profilo o nessun tasso associato, il costo effettivo del problema è zero. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nessuna assegnazione</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Costo effettivo</strong> è calcolato con la seguente formula:</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Se l'utente che registra l'ora non ha un tasso di costo per ora associato al proprio profilo, il tasso di costo per ora del ruolo di lavoro principale calcola il costo effettivo del problema. </p> <p>Se l'utente che registra l'ora non ha un ruolo di lavoro associato al proprio profilo o il ruolo di lavoro principale non ha un tasso di costo per ora definito, il costo effettivo del problema è zero. </p> </td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td colspan="4"> 
    <div> <MadCap:conditionalText data-mc-conditions="">
       If your Workfront administrator enabled the 
      <strong>Assign Job Roles to hour entries manually</strong> setting in the Timesheets &amp; Hours Preferences area, and the user logging time on the issue selects a different role to associate with this time, the Actual Cost of the issue calculates based on the role specified when the hours were logged. For information about enabling logging time for a specific job role, see the article 
      <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configure timesheet and hour preferences</a>. 
     </MadCap:conditionalText> 
    </div> </td> 
  </tr> 
  -->
 </tbody> 
</table>
