---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: Tracciare i costi
description: Puoi tenere traccia dei costi per progetti, attività e problemi in Adobe Workfront.
author: Alina, Lisa
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '2472'
ht-degree: 1%

---

# Tracciare i costi

Puoi tenere traccia dei costi per progetti, attività e problemi in Adobe Workfront.

## Calcolo dei costi in Workfront

Per tenere traccia dei costi, è necessario associare utenti e mansioni alle tariffe orarie.

Le tariffe orarie rappresentano gli importi dei costi per unità di lavoro associati alle mansioni o agli utenti. Moltiplicando le tariffe per le ore lavorative si generano costi per progetti, attività o problemi.

Esistono i seguenti scenari:

* Se il tipo di costo delle attività è Ore utente, la tariffa oraria utente calcola i costi dell&#39;attività e del progetto.

  Per informazioni sull&#39;associazione degli utenti alle tariffe, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Se il tipo di costo delle attività è Ore mansione, la tariffa oraria della mansione calcola i costi dell&#39;attività e del progetto.

  Per informazioni sull&#39;associazione delle mansioni alle tariffe, vedere [Creare e gestire le mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront calcola solo il costo effettivo per i problemi e i problemi non hanno un tipo di costo. Per ulteriori informazioni, consulta la sezione [Come Workfront tiene traccia dei costi per i problemi](#how-workfront-tracks-costs-for-issues) in questo articolo.

>[!TIP]
>
>Non è possibile sostituire i tassi di costo per i progetti. Una volta stabilita la tariffa oraria per un utente o una mansione, tale tariffa calcola tutti i costi nel sistema.

## Indici prestazioni costi Workfront

Workfront calcola una serie di indici di prestazioni dei costi per i progetti in modo che sia possibile tenere traccia dei progetti in modo da ottimizzare i costi.\
Per ulteriori informazioni sul calcolo degli indici di prestazioni dei costi, vedere:

* [Calcola indice prestazioni costi (IPC)](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [Calcola indice prestazioni programma costi (CSI)](../../../manage-work/projects/project-finances/calculate-csi.md)
* [Calcola indice prestazioni Schedule (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)

## Come Workfront tiene traccia dei costi per attività e progetti

* [Tracciamento dei costi in Workfront](#how-workfront-tracks-costs)
* [Calcolo dei costi pianificati, preventivati ed effettivi in Workfront](#how-workfront-calculates-planned-budgeted-and-actual-costs)
* [Modalità di calcolo dei tipi di costo per le attività in Workfront](#how-workfront-calculates-cost-types-for-tasks)

### Tracciamento dei costi in Workfront  {#how-workfront-tracks-costs}

In Workfront è possibile tenere traccia di diversi tipi di costi per attività e progetti. I costi complessivi sono calcolati con la seguente formula:

`Costs = Labor Costs + Expense Costs`

* **Costi manodopera** sono associati alle ore per attività e progetti e alle tariffe Costo orario delle risorse associate alle attività. In genere, Workfront calcola i seguenti costi di manodopera:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Costi manodopera pianificati</td> 
     <td> <p>Sono calcolati con la seguente formula:</p><code>Planned Labor Costs = Planned Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Costi manodopera preventivati</td> 
     <td> <p>Sono calcolati con la seguente formula:</p><code>Budgeted Labor Costs = Budgeted Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>Costi effettivi manodopera</td> 
     <td> <p>Sono calcolati con la seguente formula:</p><code>Actual Labor Costs = Actual Hours * Cost per Hour rate</code> </td> 
    </tr> 
   </tbody> 
  </table>

  Per ulteriori informazioni, vedere [Calcolo dei costi pianificati, preventivati ed effettivi in Workfront](#how-workfront-calculates-planned-budgeted-and-actual-costs) in questo articolo.

* **Costi spese** sono associate a Spese per progetti e attività.\
  Quando si crea un progetto, è possibile impostare le spese pianificate per l&#39;intero progetto. È inoltre possibile associare le spese ad attività nuove o esistenti. Per informazioni, consulta [Gestisci spese progetto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **Costi fissi** sono definiti come importo fisso di costo per un progetto. Questa parte del Costo pianificato del progetto rappresenta la quantità di denaro necessaria per completare il progetto.

  >[!TIP]
  >
  >Quando si allega un modello a un progetto, il Costo fisso di un modello viene aggiunto al Costo fisso del progetto. Per informazioni, consulta [Panoramica dell’associazione di un modello a un progetto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### Calcolo dei costi pianificati, preventivati ed effettivi in Workfront {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront calcola il Costo pianificato e il Costo effettivo per ogni singola attività di un progetto. Workfront utilizza questi calcoli per le singole attività per calcolare il Costo pianificato e il Costo effettivo del progetto.

* [Costo Pianificato](#planned-cost)
* [Bdg prv](#budgeted-cost)
* [Costo Reale](#actual-cost)

#### Costo Pianificato {#planned-cost}

Il costo pianificato di un progetto è il costo associato al lavoro pianificato (ore pianificate) del progetto.

Il costo pianificato di un progetto viene calcolato con la formula seguente:

`Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project`

Ad esempio, nella scheda Spese di un&#39;attività sono presenti le seguenti spese: una spesa di marketing di $ 100 e una spesa amministrativa di $ 50. Nella scheda Finanza selezionare il tipo di costo Orario utente. Un utente viene assegnato all&#39;attività e la tariffa oraria dell&#39;utente è pari a $ 15. L’utente è assegnato a lavorare 5 ore su questa attività. Nella scheda Spese del progetto, si dispone di un costo pianificato di 100 $ per una spesa denominata Consulenza. Hai anche un Costo Fisso di 200 $ per il progetto.

Il costo pianificato del progetto viene calcolato come segue:

`$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525`

La tariffa oraria nella formula considera eventuali modifiche effettive alla data della tariffa.

#### Bdg prv {#budgeted-cost}

Il costo preventivato di un progetto è il costo associato al lavoro preventivato (ore preventivate) del progetto.

Il costo preventivato del progetto è uguale al costo pianificato del progetto se sono soddisfatte le due condizioni seguenti:

* Le ore pianificate delle attività del progetto corrispondono alle ore pianificate (nella Programmazione delle risorse)
* Il tipo di fatturazione dell&#39;attività è Ore ruolo.

Il costo preventivato del progetto viene calcolato utilizzando la formula seguente se vengono soddisfatte le seguenti condizioni:

* Le ore pianificate delle attività del progetto non corrispondono alle ore pianificate (nella pianificazione risorse)
* Il tipo di fatturazione delle attività è Ore ruolo.

Quando le condizioni di cui sopra sono soddisfatte, Workfront calcola il costo preventivato del progetto utilizzando la seguente formula:

`Budgeted Project Cost = Budgeted Labor Cost + Budgeted Expense Cost of all tasks + Budgeted Expense Cost of the project`

#### Costo Reale {#actual-cost}

Il costo effettivo di un progetto è il costo associato al lavoro effettivo (ore registrate) del progetto.

Il costo effettivo viene calcolato utilizzando la formula seguente:

`Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project`

Ad esempio, nella scheda Spese di un&#39;attività sono presenti le spese seguenti: una spesa di marketing con un costo effettivo di 110 dollari e una spesa amministrativa con un costo effettivo di 40 dollari. Selezionare il tipo di costo Orario ruolo e assegnare il ruolo Consulente all&#39;attività. La tariffa del ruolo di consulente è di $ 15 all&#39;ora e sono disponibili 6 ore di accesso all&#39;attività per il ruolo di consulente. Esiste una spesa di consulenza associata al progetto (nella scheda Spese), con un costo effettivo di $ 100 e un utente con una tariffa Costo all’ora di $ 20 nei registri del profilo utente 10 ore sul progetto. Hai anche un Costo Fisso di 200 $ per il progetto.

Il costo effettivo del progetto viene calcolato nel modo seguente:

`$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740`

La tariffa oraria nella formula considera eventuali modifiche effettive alla data della tariffa.

>[!NOTE]
>
>Il Costo di Spesa Reale del progetto viene calcolato come segue:
>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>Questi costi non vengono duplicati nel calcolo del costo effettivo. Ad esempio, se un Costo Fisso fa parte del Costo Spesa Reale del progetto, non viene aggiunto separatamente al Costo Reale.

>[!NOTE]
>
>Quando si registra il tempo di un progetto, esistono i seguenti scenari per il calcolo del costo effettivo della manodopera per il progetto:
>
>* Per impostazione predefinita, Workfront utilizza la tariffa Costo orario dell&#39;utente per calcolare il Costo effettivo della manodopera.
>* Se l&#39;utente che registra l&#39;ora non è associato ad alcun costo, Workfront utilizza la tariffa Costo all&#39;ora del ruolo principale dell&#39;utente.
>* Se l&#39;amministratore di Workfront ha abilitato **Assegna mansioni alle ore manualmente** Se si imposta l&#39;opzione nella sezione Preferenze schede orario e ore e l&#39;utente registra il progetto seleziona un ruolo diverso da associare a questo orario, il costo effettivo del progetto viene calcolato in base al ruolo specificato al momento della registrazione delle ore. Per informazioni sull’abilitazione dell’ora di registrazione per una mansione specifica, consulta l’articolo [Configurare le preferenze di orario e scheda orario](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

### Modalità di calcolo dei tipi di costo per le attività in Workfront {#how-workfront-calculates-cost-types-for-tasks}

Il Costo pianificato e il Costo effettivo delle attività e i relativi Costi manodopera sono determinati dal Tipo di costo di ogni attività.

È possibile configurare il tipo di costo per le singole attività all&#39;interno del progetto. Ogni tipo di costo influisce sui valori Costo pianificato e Costo effettivo.

Per informazioni sulla modifica del tipo di costo di un&#39;attività, vedere [Aggiorna tipo di costo attività](../../../manage-work/tasks/task-information/update-task-cost-type.md).

Nella tabella seguente vengono descritti i tipi di costo dei task disponibili in Workfront:

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
   <td> <p>Questo è il tipo di costo predefinito quando si crea un'attività.</p> <p><strong>Costo Pianificato</strong> è calcolato con la seguente formula: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Dove il costo della manodopera pianificata è calcolato da:<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>Nota: <p>Considera i seguenti impatti dell’utilizzo del tipo di costo orario utente e del calcolo del costo pianificato:</p> 
     <ul> 
      <li>Se si assegnano più risorse a un'attività, Workfront adegua i calcoli per il Costo pianificato in base alla percentuale dell'attività assegnata a ciascuna risorsa.</li>
      <li>Per i tassi di costo effettivi per data, il costo manodopera pianificata è la somma dei costi pianificati di ogni periodo di tempo coperto dall'attività.</li>
      <li>Il valore del campo Costo pianificato può variare a seconda che il Costo pianificato venga visualizzato dall'attività stessa o dal rapporto Utilizzo.<br><strong>Quando si visualizza Costo pianificato dall'attività stessa:</strong> Il campo Costo pianificato prende in considerazione il campo Costo/ora impostato a livello di mansione (quando il campo Costo/ora non è stato impostato a livello di utente).<br><strong>Quando si visualizza Costo pianificato dal rapporto Utilizzo del progetto:</strong> Il campo Costo pianificato non prende in considerazione il campo Costo/ora impostato a livello di mansione. Se invece si desidera che il rapporto Utilizzo prenda in considerazione il campo Costo/Ora impostato a livello Mansione, è necessario impostare il tipo di costo dell'attività su Ore mansione. </li> 
     </ul> </p> <p><strong>Costo Reale</strong> è calcolato con la seguente formula: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Se il costo effettivo della manodopera è calcolato in base a:</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>Ad esempio, un utente nel suo profilo ha una tariffa Costo orario di 20 $. Quando si registrano 5 ore per un'attività, il costo effettivo della manodopera per tale attività è pari a $ 100. Se all'utente non è associata una tariffa Costo orario, il Costo effettivo viene calcolato in base alla tariffa Costo orario della mansione principale. Se non hanno una mansione o la tariffa Costo orario della loro mansione non è definita, il Costo effettivo dell'attività è pari a zero. </p> <p>Nota: i costi effettivi vengono calcolati in base alla tariffa Costo orario per l'utente che registra l'ora, indipendentemente da chi è assegnato all'attività. Inoltre, la tariffa oraria di fatturazione nella formula considera qualsiasi modifica effettiva della data della tariffa.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ore Ruolo</p> </td>
   <td> <p><strong>Costo Pianificato</strong> è calcolato con la seguente formula: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>Dove il costo manodopera pianificata dell'attività viene calcolato in base a:</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Nota: se si assegnano più risorse a un'attività, Workfront adegua i calcoli per le ore pianificate in base alla percentuale dell'attività assegnata a ciascuna risorsa. Inoltre, la tariffa oraria nella formula considera qualsiasi modifica effettiva della data della tariffa.</p> <p><strong>Costo Reale</strong> è calcolato con la seguente formula: </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Dove il costo effettivo manodopera task viene calcolato in base a:</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Ad esempio, un'attività viene assegnata a una mansione o a un utente con una mansione per la quale la tariffa oraria è di 20 $. Quando un utente registra 5 ore per un’attività, il costo effettivo della manodopera per tale attività è pari a $ 100. Se all'utente assegnato all'attività non è associata alcuna mansione, il costo effettivo viene calcolato in base alla tariffa oraria del relativo Ruolo principale. Se non hanno una mansione o la tariffa Costo orario della loro mansione non è definita, il Costo effettivo dell'attività è pari a zero. </p> <p>Nota:   <p> Le ore effettive di un'attività oraria ruolo vengono calcolate in base ai ruoli degli utenti associati all'attività e non ai ruoli associati all'utente che registra l'ora. Inoltre, la tariffa oraria di fatturazione nella formula considera qualsiasi modifica effettiva della data della tariffa.</p> <p>Se l'amministratore di Workfront ha abilitato <strong>Assegna mansioni alle ore manualmente</strong> Se si imposta l'impostazione nella sezione Preferenze schede orario e ore e l'utente registra l'ora per l'attività seleziona un ruolo diverso da associare a questo orario, il costo effettivo di un'attività oraria ruolo viene calcolato in base al ruolo specificato al momento della registrazione delle ore. Per informazioni sull’abilitazione dell’ora di registrazione per una mansione specifica, consulta l’articolo <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configurare le preferenze di orario e scheda orario</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ore Fisse</p> </td> 
   <td> <p><strong>Costo Pianificato</strong> è calcolato con la seguente formula:</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Dove il costo manodopera task viene calcolato in base a:</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>Costo Reale</strong> è calcolato con la seguente formula: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>Dove il costo effettivo manodopera task viene calcolato in base a:</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>Questo tipo di costo non prende in considerazione singoli utenti o mansioni.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nessun Costo</p> </td> 
   <td> <p>Questo tipo di costo non influisce sui costi. Se un task padre ha questo tipo di costo, i task secondari con un altro tipo di costo calcolano in base ai singoli tipi di costo e il costo del task padre viene influenzato di conseguenza. </p> <p>Quando un utente senza accesso ai dati finanziari o senza autorizzazioni finanziarie su un modello crea un progetto da tale modello, questo è il tipo di costo predefinito per le attività del progetto.</p> <p>Per informazioni sull'accesso ai dati finanziari, vedere l'articolo <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Concedere l’accesso ai dati finanziari</a>.</p> <p>Per informazioni sulle autorizzazioni finanziarie per gli oggetti, vedere l'articolo <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Condividere le autorizzazioni finanziarie su un oggetto</a>.</p> <p>Per informazioni sulla creazione di progetti a partire da modelli, consulta l’articolo <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Creare un progetto utilizzando un modello</a>.</p> </td> 
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

Problemi, tuttavia, possono avere un **Costo Reale** che influisce anche sul costo effettivo del progetto.

Nella tabella seguente viene illustrato come viene calcolato il costo effettivo per i problemi, in base al tipo di assegnazione per il problema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th colspan="4">Costo effettivo problema</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Assegnazione utente</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Costo Reale</strong> è calcolato con la seguente formula:</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>La tariffa Costo orario dell’utente che registra l’ora viene presa in considerazione qui, indipendentemente da chi è assegnato al problema. </p> <p>Se l'utente che registra l'ora non dispone di una tariffa Costo orario nel proprio profilo, la tariffa Costo orario della mansione principale calcola il Costo effettivo del problema. Se l'utente che registra l'ora non ha alcun ruolo nel proprio profilo o nessuna tariffa ad esso associata, le ore effettive vengono calcolate utilizzando la tariffa Costo per ora della mansione principale dell'assegnatario principale per il problema. Se per tale ruolo non è stato definito alcun tasso, il costo effettivo del problema è pari a zero. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Assegnazione Ruolo</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Costo Reale</strong> è calcolato con la seguente formula:</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>In questo caso, viene preso in considerazione il tasso di costo orario dell’utente che registra l’ora sul problema, indipendentemente dal ruolo assegnato al problema. </p> <p>Se l’utente che registra l’ora non ha una tariffa Costo orario associata, la tariffa Costo orario del suo ruolo principale calcola il Costo effettivo del problema.<br>Se l’utente che registra l’ora non ha alcun ruolo nel profilo o nessuna tariffa associata, il costo effettivo del problema è zero. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nessuna assegnazione</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Costo Reale</strong> è calcolato con la seguente formula:</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Se l'utente che registra l'ora non ha una tariffa Costo orario associata al proprio profilo, la tariffa Costo orario della sua mansione principale calcola il Costo effettivo del problema. </p> <p>Se l'utente che registra l'ora non ha una mansione associata al suo profilo o la sua mansione principale non ha una tariffa Costo per Ora definita, il Costo Reale del problema è zero. </p> </td> 
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
