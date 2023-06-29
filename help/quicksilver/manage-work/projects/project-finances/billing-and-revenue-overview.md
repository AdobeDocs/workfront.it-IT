---
content-type: overview
product-area: projects
navigation-topic: financials
title: Panoramica su fatturazione e ricavi
description: In qualità di project manager, puoi utilizzare le tariffe di fatturazione per acquisire i ricavi dai tuoi progetti.
author: Alina, Lisa
feature: Work Management
exl-id: 400abcde-e368-4a70-89a9-05027900ab81
source-git-commit: d2b62f2ec2f52c54129b342d68c336c782601242
workflow-type: tm+mt
source-wordcount: '3706'
ht-degree: 0%

---

# Panoramica su fatturazione e ricavi

{{highlighted-preview}}

In qualità di project manager, puoi utilizzare le tariffe di fatturazione per acquisire i ricavi dai tuoi progetti.

Questo articolo descrive come tenere traccia dei ricavi per i progetti. I ricavi vengono calcolati in modo diverso nel rapporto Utilizzo. Per informazioni sui calcoli dei ricavi nel rapporto Utilizzo, vedere [Visualizza informazioni sull&#39;utilizzo delle risorse](../../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Panoramica delle tariffe di fatturazione

Quando si lavora con le tariffe di fatturazione, considera quanto segue:

* Per gestire le tariffe di fatturazione è necessaria una licenza Pianificazione con accesso Modifica ai dati finanziari.\
  Per ulteriori informazioni sulla concessione dell&#39;accesso ai dati finanziari, vedere [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Le tariffe di fatturazione sono quantità di ricavi per unità di lavoro associate a mansioni o utenti.

  Moltiplicando i tassi per le ore lavorative si generano ricavi per i progetti.

* Dopo aver stabilito le tariffe di fatturazione, puoi tenere traccia delle entrate creando record di fatturazione per registrare ciò che è stato o non è stato fatturato.

  >[!TIP]
  >
  >Quando si contrassegna un record fatturazione come fatturato, non è possibile modificarlo. Questo è importante quando le tariffe variano e si desidera bloccare le informazioni su ricavi e spese sul progetto. Aggiungendolo a un record di fatturazione e contrassegnandolo come Fatturato, si impedisce che venga aggiornato quando le tariffe vengono aggiornate nel sistema.

  Per ulteriori informazioni sulla creazione di record di fatturazione, consulta l’articolo [Crea record fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md).

* È possibile creare tariffe di fatturazione per utenti, mansioni o una tariffa di fatturazione occasionale per un progetto o un&#39;attività.

>[!IMPORTANT]
>
>I tassi che calcolano i ricavi appartengono all’utente che registra l’ora o alle sue mansioni.

* [Tariffe di fatturazione utente](#user-billing-rates)
* [Tariffe di fatturazione mansione](#job-role-billing-rates)
* [Tariffe di fatturazione fisse per progetti o attività](#fixed-billing-rates-for-projects-or-tasks)
* [Sostituisci tariffe di fatturazione](#override-billing-rates)

### Tariffe di fatturazione utente {#user-billing-rates}

In qualità di amministratore utente, quando crei un utente, puoi associarlo a una tariffa di fatturazione specificando un valore per il campo Fatturazione all’ora nel suo profilo.

Per ulteriori informazioni sulla creazione di utenti, consulta l’articolo [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

![](assets/qs-user-edit-ui-with-rp-and-billing-per-hour-field-1-350x152.png)

<div class="preview">

Nell&#39;ambiente di anteprima è possibile associare l&#39;utente alle tariffe di fatturazione effettive della data specificando i valori per i campi Fatturazione ad ore e le date per le tariffe.

![Modifica costo utente e tariffe di fatturazione](assets/edit-user-cost-billing-rate-1.png)

</div>

### Tariffe di fatturazione mansione {#job-role-billing-rates}

In qualità di amministratore di Adobe Workfront, quando crei una mansione, puoi associarla a una tariffa di fatturazione specificando un valore per il campo Fatturazione/Ora.

È possibile definire il valore di un tasso di fatturazione di una mansione utilizzando la valuta di base del sistema Workfront o un&#39;altra valuta personalizzata.

Per ulteriori informazioni sulla creazione di mansioni e sulla sostituzione della relativa valuta, consulta l’articolo [Creare e gestire le mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

![](assets/billing-rate-for-role-1-350x294.png)

<div class="preview">

Nell&#39;ambiente di anteprima è possibile associare la mansione alle tariffe di fatturazione effettive della data specificando i valori per i campi Fatturazione ad ore e le date per le tariffe.

![Modifica costi mansione e tariffe di fatturazione](assets/edit-job-role-multiple-billing-rates.png)

</div>

### Tariffe di fatturazione fisse per progetti o attività {#fixed-billing-rates-for-projects-or-tasks}

Oltre alle tariffe orarie dell&#39;utente e della mansione, è possibile avere anche le seguenti tariffe di fatturazione fisse:

* Importo fisso per tipo di retribuzione oraria fissa
* Importo fisso per tipo di reddito Reddito Fisso

Per ulteriori informazioni sulle modalità di utilizzo delle tariffe di fatturazione fisse per calcolare i ricavi, consulta [Panoramica sui tipi di retribuzione delle attività](#overview-of-task-revenue-types).

### Sostituisci tariffe di fatturazione {#override-billing-rates}

>[!IMPORTANT]
>
>Puoi sovrascrivere le tariffe di fatturazione associate alle mansioni. Non è possibile sostituire le tariffe di fatturazione o le tariffe fisse dell&#39;utente.

È possibile sostituire le tariffe di fatturazione dei ruoli per:

* Un’azienda specifica

  Per ulteriori informazioni sulla creazione di tariffe di fatturazione per mansioni specifiche per un’azienda, consulta [Creare e modificare le società](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Un progetto specifico

  Per ulteriori informazioni sulla creazione di tariffe di fatturazione dei ruoli specifiche per un progetto, consulta l’articolo [Panoramica sulla sostituzione delle tariffe di fatturazione dei ruoli e sul calcolo dei ricavi per un progetto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Tracciare gli importi dei ricavi

Workfront può tenere traccia automaticamente della Retribuzione pianificata quando le attività vengono create in base alle Ore pianificate delle attività.

Può anche tenere traccia automaticamente della Retribuzione effettiva quando vengono registrate le ore effettive sulle attività, sui problemi e sul progetto.

La tabella seguente mostra i tipi di ricavi associati ad attività, problemi e progetti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Reddito Pianificato</td> 
   <td> <p>Per le attività, si tratta delle entrate associate alle ore pianificate delle attività. Le ore pianificate da tutte le attività vengono riportate alle ore pianificate del progetto per contribuire al calcolo delle ore pianificate del progetto. </p> <p>Per ulteriori informazioni sulle ore pianificate in Workfront, consulta <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Panoramica sulle ore pianificate</a>. </p> <p>Workfront calcola la Retribuzione pianificata per le attività utilizzando la formula seguente:</p>
   <p><code>Task Planned Revenue = Planned Hours * Billing hourly rate</code><p> <p><span class="preview"><strong>NOTA</strong></br> La tariffa oraria di fatturazione nella formula considera eventuali modifiche effettive alla data della tariffa.</span></p> <p>Workfront calcola la Retribuzione pianificata per i progetti utilizzando la formula seguente:</p> <p><code>Project Planned Revenue = SUM (All tasks Planned Revenue) + Fixed Revenue</code></p>
   <p><b>NOTA</b>

<p>Il campo Retribuzione pianificata del progetto visualizzato nell'area Dettagli progetto e nei rapporti del progetto è diverso dal campo Retribuzione pianificata visualizzato nel rapporto Utilizzo. </p> <p>La Retribuzione pianificata nell'area Dettagli progetto riflette le entrate dell'attività associate all'attività Lavoro pianificato e alla Retribuzione fissa del progetto. Nel rapporto Utilizzo, la Retribuzione pianificata mostra la Retribuzione pianificata associata solo alle Ore pianificate delle assegnazioni delle attività del progetto. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p>Se il progetto ha 1 attività con 10 ore, assegnata a un consulente con una tariffa oraria di 20 $ e il progetto ha un reddito fisso di 100 $, il rapporto Utilizzo visualizza 200 $ per il reddito pianificato (il reddito pianificato associato alle ore dell'attività). La sezione Dettagli progetto visualizza $ 300 (la Retribuzione pianificata dall'attività e la Retribuzione fissa per il progetto). </p> 
     </div> </p> <p>La Retribuzione pianificata dell'attività viene calcolata utilizzando le tariffe orarie di fatturazione degli utenti o delle mansioni assegnate alle attività. Il tipo di retribuzione delle attività influisce sul tasso (utente o ruolo) utilizzato per calcolare la retribuzione pianificata. Per ulteriori informazioni, vedere le sezioni seguenti in questo articolo:</p> 
    <ul> 
     <li> <p><a href="#overview-of-task-revenue-types" class="MCXref xref">Panoramica sui tipi di retribuzione delle attività</a> </p> </li> 
     <li> <p><a href="#revenue-calculations-for-tasks-based-on-user-and-role-assignments" class="MCXref xref">Calcolo dei ricavi per le attività in base alle assegnazioni di utenti e ruoli</a> </p> </li> 
    </ul> <p>Per informazioni sui calcoli dei ricavi pianificati nel rapporto Utilizzo, vedere <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Visualizza informazioni sull'utilizzo delle risorse </a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reddito Reale*</td> 
   <td> <p>Associato alle ore effettive di attività, problemi e progetti. </p> <p>In genere, Workfront calcola i ricavi effettivi utilizzando questa formula:</p> <p><code>Actual Revenue = Actual Hours * Billing rate</code> </p> <p><span class="preview"><strong>NOTA</strong></br> La tariffa oraria di fatturazione nella formula considera eventuali modifiche effettive alla data della tariffa.</span></p> <p>Per informazioni sui calcoli dei ricavi effettivi nel rapporto Utilizzo, vedere <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Visualizza informazioni sull'utilizzo delle risorse </a>. </p> <p><b>SUGGERIMENTO</b>

Non è possibile visualizzare la Retribuzione effettiva a livello di problema, ma i ricavi associati alle Ore effettive sui problemi contribuiscono alla Retribuzione effettiva del progetto. </p> </td>
</tr> 
 </tbody> 
</table>

*Per le ore effettive, le tariffe dell’utente si riferiscono sempre all’utente che registra le ore o alle tariffe delle sue mansioni. Per informazioni su quando Workfront utilizza le tariffe dell’utente e quando utilizza le tariffe delle sue mansioni, vedi [Calcoli dei ricavi](#revenue-calculations) in questo articolo.

<!--Note from the table for Planned Revenue line: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    -->

Ad esempio, se un&#39;attività con Tipo di retribuzione oraria utente è pianificata in modo da richiedere 2 ore e l&#39;utente a essa assegnato ha una tariffa oraria di $ 30 all&#39;ora, la retribuzione pianificata dell&#39;attività è di $ 60. Al termine dell’attività, se l’utente registra solo 1,5 ore come tempo effettivo trascorso per terminarla, l’importo del Ricavo effettivo è pari a $ 45. Se un altro utente non assegnato all’attività registra l’ora, la Retribuzione effettiva viene calcolata in base alle tariffe di fatturazione dell’utente.

È possibile registrare i ricavi nei modi seguenti:

* Definendo il tipo di retribuzione delle attività e associando gli utenti o i ruoli assegnati agli elementi di lavoro alle tariffe di fatturazione. In questo modo i ricavi vengono calcolati in base alla quantità di ore pianificate o effettive sulle voci di lavoro. È possibile impostare un limite all&#39;importo massimo addebitato per le tariffe orarie o meno.\
  Per ulteriori informazioni su come specificare il tipo di retribuzione di un&#39;attività, vedere l&#39;articolo [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

* Fatturazione di un tasso fisso di retribuzione forfettaria per attività o progetti.\
  Se si dispone di attività con Reddito Fisso, l&#39;importo Reddito Fisso verrà aggiunto come Reddito Pianificato di un&#39;attività o di un progetto e la Retribuzione Pianificata di un&#39;attività sarà disponibile per essere aggiunta a un record Fatturazione come Reddito Fisso.
* Impostando una fatturazione forfettaria a tasso fisso per un progetto, quindi impostando tassi orari per le attività all&#39;interno del progetto. Workfront aggiunge le tariffe orarie per le attività alla tariffa fissa del progetto.\
  Ad esempio, un meccanico che utilizza Workfront potrebbe immettere un costo per le parti come ricavo fisso per il progetto, quindi fatturare un&#39;ora per il tempo impiegato per riparare un&#39;auto. Il reddito fisso per i progetti o le attività viene quindi realizzato al completamento.

È inoltre possibile contrassegnare le attività come &quot;Non fatturabili&quot;, nel qual caso non sono associate entrate pianificate o effettive.

## Panoramica sui tipi di retribuzione delle attività {#overview-of-task-revenue-types}

Per impostazione predefinita, il Tipo di retribuzione di tutte le nuove attività viene impostato in base alle Preferenze attività e problemi specificate dall&#39;amministratore del Workfront o del gruppo.\
Per ulteriori informazioni sulla definizione delle preferenze per attività e problemi per l’istanza di Workfront, consulta l’articolo [Configurare le preferenze per attività e problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Il proprietario del progetto può modificare il tipo di retribuzione delle attività e il tipo di retribuzione fissa per i progetti.\
Per ulteriori informazioni su come specificare i Redditi Fissi di un progetto, consulta l’articolo [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).\
Per ulteriori informazioni su come specificare il tipo di retribuzione di un&#39;attività, vedere l&#39;articolo [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

È possibile applicare i tipi di retribuzione seguenti alle attività o ai progetti:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tipo di Reddito</strong> </p> </th> 
   <th> <p><strong>Descrizione</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Reddito Fisso</p> </td> 
   <td> <p>Questo tipo può essere utilizzato con progetti e attività. </p> <p>Quando si allega un modello a un progetto, i Ricavi fissi del modello vengono aggiunti ai Ricavi fissi del progetto. Per informazioni, consulta <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Panoramica dell’associazione di un modello a un progetto</a>. </p> <p>Per le attività, indipendentemente dalle assegnazioni delle attività, i ricavi vengono sempre calcolati utilizzando l'importo fisso specificato per l'attività. </p> <p>Le attività Reddito Fisso da figli vengono aggregate ai Ricavi dell'attività padre e quindi ai ricavi del progetto. Se sull'attività padre e/o sul progetto è definito un importo fisso, tale importo viene aggiunto ai ricavi pianificati aggregati da qualsiasi attività figlio.</p> <p>L'importo dei ricavi fissi sulle attività può essere incluso in una Fatturazione del progetto.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ore Utente</p> </td> 
   <td> <p>Questo tipo può essere utilizzato solo per le attività. </p> <p>La tariffa di fatturazione impostata per un utente specifico moltiplicata per il numero di ore pianificate per l'attività diventa la quantità di retribuzione pianificata dell'attività. La tariffa di fatturazione impostata per un utente specifico moltiplicata per il numero di ore registrate dall'utente per l'attività corrisponde alla somma dei ricavi effettivi dell'attività. <br>Ad esempio, quando si crea un utente e si imposta $20 per il campo Fatturazione ad ora, se l'utente invia 5 ore per un'attività nella scheda orario, l'importo di Fatturazione effettiva dell'attività è $100.</p>
   <p><span class="preview">Un profilo utente può contenere più tariffe di fatturazione con date di validità. Ad esempio, la prima tariffa di fatturazione utente di 20 $ termina il 30 aprile 2023 e la seconda tariffa di fatturazione utente di 25 $ inizia il 1° maggio 2023. Se l’utente invia 2 ore il 28 aprile e 3 ore il 2 maggio per un’attività, l’importo di fatturazione effettiva dell’attività è pari a $ 40 + $ 75 = $ 115.</span></p>
   <p><b>SUGGERIMENTO</b>

Questo è il Tipo di Reddito predefinito quando si crea un&#39;attività.</p> </td>
</tr> 
  <tr> 
   <td> <p>Ore Ruolo</p> </td> 
   <td> <p>Questo tipo può essere utilizzato solo per le attività.</p> <p>Questo tipo è simile a Ore utente, ma utilizza tassi di ruolo anziché tassi utente.</p> <p><span class="preview"><strong>NOTA</strong><br>Una mansione può anche avere più tariffe di fatturazione con date di validità.</span></p></td> 
  </tr> 
  <tr> 
   <td> <p>Ore utente con limite</p> </td> 
   <td> <p>Questo tipo può essere utilizzato solo per le attività.</p> <p>Le attività vengono fatturate su base oraria come in Ore utente, ma hanno un massimale che puoi specificare. <br>Ad esempio, se la tariffa di fatturazione di un utente è di $ 25, ma l'importo limite per l'attività è di $ 20 e l'utente registra un'ora, la retribuzione effettiva per l'attività è di $ 20. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ore Ruolo con Limite</p> </td> 
   <td> <p>Questo tipo può essere utilizzato solo per le attività.</p> <p>Questo tipo è simile a Ore utente con limite, ma utilizza tassi di ruolo anziché tassi utente. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ore Utente più Fisso</p> </td> 
   <td> <p>Questo tipo può essere utilizzato solo per le attività. </p> <p>Le attività vengono fatturate ogni ora come in Ore utente, ma hanno un importo fisso che puoi aggiungere alla tariffa utente. L'importo fisso specificato per l'attività può essere incluso nei record di fatturazione per il progetto. L'importo fisso non viene moltiplicato per le ore dell'attività. Solo la tariffa di fatturazione dell’utente lo fa. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ore Ruolo più Fisso</p> </td> 
   <td> <p>Questo tipo può essere utilizzato solo per le attività. </p> <p>Le attività vengono fatturate ogni ora come in Ore Ruolo, ma dispongono di un importo fisso aggiuntivo che è possibile aggiungere alla tariffa del ruolo. L'importo fisso specificato per l'attività può essere incluso nei record di fatturazione per il progetto. L'importo fisso non viene moltiplicato per le ore dell'attività. Solo la tariffa di fatturazione della mansione lo fa. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ore Fisse</p> </td> 
   <td> <p>Questo tipo può essere utilizzato solo per le attività.</p> <p>L'importo massimo o fisso impostato per l'attività moltiplicato per il numero di ore immesse per l'attività (indipendentemente dall'utente o dalle mansioni) corrisponde all'importo di fatturazione.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Non Fatturabile</p> </td> 
   <td> <p>Questo tipo può essere utilizzato solo per le attività.</p> <p>Questo Tipo di Reddito non ha alcun effetto sui ricavi. </p> <p>Se un oggetto padre dispone di questa impostazione, le attività figlio con un tipo di fatturazione verranno comunque applicate normalmente.</p> <p>Quando un utente senza accesso ai dati finanziari o senza autorizzazioni finanziarie su un modello crea un progetto da tale modello, questo è il tipo di retribuzione predefinito per le attività sul progetto.</p> <p>Per informazioni sull'accesso ai dati finanziari, vedere l'articolo <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Concedere l’accesso ai dati finanziari</a>.<br>Per informazioni sulle autorizzazioni finanziarie per gli oggetti, vedere l'articolo <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Panoramica delle autorizzazioni di condivisione sugli oggetti</a>.<br>Per informazioni sulla creazione di progetti a partire da modelli, consulta l’articolo <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Creare un progetto utilizzando un modello</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Panoramica ricavi per attività padre

Se si modifica un&#39;attività autonoma contenente informazioni di fatturazione in un padre, la nuova attività padre conserva tutte le informazioni di fatturazione precedentemente applicate, insieme alle ore applicate in precedenza. Tutte le informazioni di fatturazione provenienti dalle ore registrate per le attività figlio verranno riportate come Ricavi effettivi nella nuova attività padre.

Anche la Retribuzione pianificata dalle attività figlio viene aggregata all&#39;attività padre.

## Panoramica dei ricavi per problemi

Le Issues non hanno un reddito Reale o Pianificato ma possono avere un Costo Reale.

Se si registrano le ore per un problema e si utilizza un tipo di ora contrassegnato come &quot;Conta come retribuzione&quot;, Workfront calcola un importo del costo effettivo in base alla tariffa dell&#39;utente che esegue l&#39;accesso all&#39;ora. Questo numero viene aggiunto al costo effettivo del progetto. Le ore possono essere incluse anche in una fatturazione.

Per ulteriori informazioni sul tracciamento dei costi, consulta l’articolo [Tracciare i costi](../../../manage-work/projects/project-finances/track-costs.md).

Per ulteriori informazioni sui tipi di ora, consulta l’articolo [Gestire i tipi di lavoro](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Calcoli dei ricavi

* [Calcolo dei ricavi per le attività in base alle assegnazioni di utenti e ruoli](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)

### Calcolo dei ricavi per le attività in base alle assegnazioni di utenti e ruoli {#revenue-calculations-for-tasks-based-on-user-and-role-assignments}

Quando si calcolano i ricavi per un&#39;attività, tenere presente quanto segue:

* Se un utente o una mansione visualizza un tasso di $0,00, Workfront lo legge come importo valido e lo moltiplica per il numero di ore sull’attività per calcolare i ricavi. Se non desideri visualizzare ricavi per le attività, accertati che il campo della tariffa di fatturazione per l’utente o la mansione sia vuoto.
* Quando vengono applicate le tariffe di fatturazione dei ruoli, Workfront utilizza la tariffa di sostituzione a livello di progetto, invece della tariffa di fatturazione per quel ruolo definita a livello di sistema ogni volta che è presente una tariffa di sostituzione sul progetto.
* <span class="preview">Per il ricavo effettivo, se l&#39;utente o la mansione dispone di più tariffe di fatturazione con date di validità, il ricavo dell&#39;attività è la somma dei ricavi di ogni periodo di tempo in cui l&#39;utente ha registrato il tempo. Il reddito pianificato si basa sulle ore pianificate per i periodi di tempo.</span>
* In caso di più assegnatari sulle attività, gli scenari descritti di seguito si applicano a ciascun assegnatario.

Esiste una gerarchia del tasso utilizzato nei calcoli dei ricavi in base alle assegnazioni delle attività.

Se l&#39;amministratore di Workfront ha abilitato **Assegna mansioni alle ore manualmente** Se si imposta l&#39;opzione nella sezione Preferenze schede orario e ore e l&#39;ora di accesso dell&#39;utente al progetto seleziona un ruolo diverso da associare a questo orario, la retribuzione effettiva dell&#39;attività o del progetto viene sempre calcolata in base al ruolo associato all&#39;immissione di ore. Per informazioni sull’abilitazione dell’ora di registrazione per una mansione specifica, consulta l’articolo [Preferenze Ore e Timesheet](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Esistono i seguenti scenari quando si calcolano i ricavi delle attività in base al tipo di ricavi e alla natura dell&#39;assegnazione delle attività:

* **Il tipo di retribuzione dell&#39;attività è Ore utente**

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Tariffa di fatturazione oraria</td> 
     <td>Nessuna assegnazione</td> 
     <td>Assegnazione utente</td> 
     <td>Assegnazione ruolo</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Tariffa oraria di fatturazione per la retribuzione pianificata</td> 
     <td>$0.00</td> 
     <td> Se un utente ha una tariffa di fatturazione nel suo profilo, questa viene utilizzata per calcolare la Retribuzione Pianificata. In caso contrario, viene utilizzata la tariffa di fatturazione del sistema per la mansione principale. <br><p><b>NOTA</b>  L’utente può essere assegnato all’attività con una delle sue mansioni secondarie, ma in questa posizione viene utilizzato il tasso della mansione principale.</p><p><span class="preview">Se il ruolo dell'utente è stato modificato durante l'assegnazione, al ricalcolo dei dati finanziari del progetto vengono applicati i tassi corretti.</span></p></td> 
     <td><p><span class="preview">Se al progetto è allegata una scheda tariffa, la Retribuzione pianificata viene calcolata in base alla mansione dalla scheda tariffa.</span></p> <p><span class="preview">Le tariffe di fatturazione possono essere sostituite a livello di progetto.</span></p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Tariffa oraria fatturazione per retribuzione effettiva</td> 
     <td>Se l’utente che registra le ore ha una tariffa di fatturazione nel suo profilo, viene utilizzata tale tariffa. 
     <br><span class="preview">Quando si registra l'ora per un utente o un ruolo che dispone di un'assegnazione specifica della posizione nelle assegnazioni avanzate, viene utilizzata la tariffa della posizione.</span>
     <br>In caso contrario, viene utilizzata la tariffa di fatturazione della mansione principale. Se all'utente o al suo ruolo principale non è associata alcuna tariffa di fatturazione, il Ricavo effettivo è pari a $0,00. <br><p><b>NOTA</b>

  Ai fini del calcolo, vengono prese in considerazione solo le tariffe associate all&#39;utente che registra l&#39;ora, anche quando un altro utente è assegnato all&#39;attività.</p></td>
  <td>Se l’utente che registra le ore ha una tariffa di fatturazione nel suo profilo, viene utilizzata tale tariffa. <br><span class="preview">Quando si registra l'ora per un utente o un ruolo che dispone di un'assegnazione specifica della posizione nelle assegnazioni avanzate, viene utilizzata la tariffa della posizione.</span><br>In caso contrario, viene utilizzata la tariffa di fatturazione della mansione principale. Se all'utente o al suo ruolo principale non è associata alcuna tariffa di fatturazione, il Ricavo effettivo è pari a $0,00. <br><p><b>NOTA</b>

  Ai fini del calcolo, vengono prese in considerazione solo le tariffe associate all&#39;utente che registra l&#39;ora, anche quando un altro utente è assegnato all&#39;attività.</p></td>
  <td>Se l’utente che registra le ore ha una tariffa di fatturazione nel suo profilo, viene utilizzata tale tariffa. In caso contrario, viene utilizzata la tariffa di fatturazione della mansione principale.<br><p><b>NOTA</b>

  Se al tempo di registrazione dell&#39;utente non è associata alcuna tariffa di fatturazione e l&#39;utente non dispone di una mansione o di una tariffa di fatturazione per la mansione, viene utilizzata la tariffa della mansione associata all&#39;attività. Se non esiste una tariffa di fatturazione per questa mansione, il ricavo è pari a $ 0,00</p></td>
  </tr> 
   </tbody> 
  </table>

* **Il Tipo di Reddito dell&#39;attività è Ore Ruolo**

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Tariffa di fatturazione oraria</td> 
     <td>Nessuna assegnazione</td> 
     <td>Assegnazione utente</td> 
     <td>Assegnazione ruolo</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Tariffa oraria di fatturazione per la retribuzione pianificata</td> 
     <td>$0.00</td> 
     <td><p>Workfront esamina il ruolo che l’utente svolge nell’attività per calcolare la Retribuzione Pianificata. <br>Se l'utente non è associato ad alcun ruolo nell'attività, il ricavo è $0,00.</p> <p><span class="preview"><strong>NOTA</strong><br>Se il ruolo dell'utente è stato modificato durante l'assegnazione, al ricalcolo dei dati finanziari del progetto vengono applicati i tassi corretti.</span></p> </td> 
     <td><p><span class="preview">Se al progetto è allegata una scheda tariffa, la Retribuzione pianificata viene calcolata in base alla mansione dalla scheda tariffa.</span></p> <p><span class="preview">Le tariffe di fatturazione possono essere sostituite a livello di progetto.</span></p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Tariffa oraria fatturazione per retribuzione effettiva</td> 
     <td>Workfront utilizza la tariffa di fatturazione della mansione principale dell’utente che registra l’ora. <br><span class="preview">Quando si registra l'ora per un utente o un ruolo che dispone di un'assegnazione specifica della posizione nelle assegnazioni avanzate, viene utilizzata la tariffa della posizione.</span> <br>Se l’utente che registra l’ora non ha una mansione associata o se la mansione principale non ha una tariffa di fatturazione, il Ricavo effettivo è pari a $ 0,00. </td> 
     <td> Se l'utente che registra l'ora è assegnato all'attività, la tariffa di fatturazione della mansione associata all'utente sull'attività viene utilizzata per calcolare la Retribuzione effettiva. <br><span class="preview">Quando si registra l'ora per un utente o un ruolo che dispone di un'assegnazione specifica della posizione nelle assegnazioni avanzate, viene utilizzata la tariffa della posizione.</span> <br>In caso contrario, viene utilizzata la tariffa di fatturazione della mansione principale. Se l'utente non ha una mansione principale o se la mansione principale non ha una tariffa di fatturazione, il reddito effettivo è pari a $0,00. </td> 
     <td>Se una delle mansioni dell’utente che registra l’ora è assegnata all’attività, viene utilizzata la frequenza di tali mansioni. Se la mansione assegnata all'attività non è associata all'utente che registra l'ora, per calcolare la Retribuzione effettiva viene utilizzata la tariffa di fatturazione del ruolo principale dell'utente. Se l'utente non dispone di una mansione o non è presente alcuna tariffa associata alla mansione principale, viene utilizzata la tariffa della mansione assegnata all'attività. </td> 
    </tr> 
   </tbody> 
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Ideal table but does not come across Markdown</p>
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
<td colspan="3">Revenue Type = User Hourly</td>
<td colspan="4">Revenue Type = Role Hourly</td>
</tr>
<tr>
<td> <p> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Planned Revenue</strong> </p> </td>
<td> <p>$0.00</p> </td>
<td> <p> If a user has a billing rate in their profile, then that rate is used to calculate Planned Revenue. Otherwise, the system billing rate of their primary job role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> </td>
<td> <p> The system billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> </td>
<td> <p>$0.00</p> </td>
<td> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Revenue. <br>If the user is not associated with any role on the task, the Revenue is $0.00. </p> </td>
<td> <p>The billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Actual Revenue</strong> </p> </td>
<td colspan="2"> <p>If the user logging the hours has a billing rate in their profile, that rate is used. <br>Otherwise, the billing rate of their primary job role is used. If there is no billing rate associated with the user or their primary role, the Actual Revenue is $0.00. <br><note type="note">
Only the rates associated with the user logging the time are taken into account for the calculation, even when another user is assigned to the task.
</note></p> </td>
<td> If the user logging the hours has a billing rate in their profile, that rate is used. Otherwise, the billing rate of their primary job role is used.<br><note type="note">
If the user logging time has no billing rate associated with them, and they do not have a job role or a billing rate for their job role, then the rate from the job role associated with the task is used. If there is no billing rate for this role, the revenue is $0.00
</note></td>
<td> <p>Workfront uses the billing rate of the primary job role of the user logging the time. <br>If the user logging the time has no job role associated with them, or if the primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p> If the user logging the time is assigned to the task, the billing rate of the job role associated with the user on the task is used to calculate the Actual Revenue. Otherwise, the billing rate of their primary job role is used. If the user has no primary job role or if their primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p>If one of the job roles of the user logging the time is assigned to the task, that job role rate is used. If the job role assigned to the task is not associated with the user logging the time, then the billing rate of the primary role of the user is used to calculate the Actual Revenue. If the user does not have a job role or there is no rate associated with their primary job role, then the rate of the job role assigned to the task is used. </p> </td>
</tr>
</tbody>
</table>
</div>
-->

### Calcolo ricavi per progetti

Puoi tenere traccia dei seguenti tipi di ricavi per i progetti:

* La Retribuzione Pianificata per un progetto viene calcolata con la seguente formula:

  ```
  Project Planned Revenue = SUM(Task Planned Revenue)+ Fixed Revenue
  ```

  Per informazioni sul calcolo della Retribuzione pianificata dell&#39;attività, vedere [Calcolo dei ricavi per le attività in base alle assegnazioni di utenti e ruoli](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) in questo articolo.

* Il reddito effettivo di un progetto viene calcolato con la formula seguente:

  ```
  Project Actual Revenue = SUM (Task Actual Revenue) + (Hours logged for the project x User Billing per Hour Rate) + SUM (Hours logged for the issues x User Billing per Hour rate)
  ```

Per informazioni sulla modalità di calcolo del reddito effettivo dell&#39;attività, vedere [Calcolo dei ricavi per le attività in base alle assegnazioni di utenti e ruoli](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) in questo articolo.

Per la Retribuzione effettiva associata alle ore registrate direttamente nel progetto o ai problemi, Workfront utilizza la Tariffa di fatturazione dell’utente che registra il tempo sul progetto. Se all&#39;utente non è associata alcuna tariffa di fatturazione con il profilo, Workfront utilizza la tariffa di fatturazione della mansione principale. Se entrambi i tassi sono pari a zero, la Retribuzione effettiva associata alle ore registrate nel progetto o ai problemi è pari a zero.
