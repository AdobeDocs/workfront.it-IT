---
content-type: overview
product-area: projects
navigation-topic: financials
title: Panoramica di fatturazione e ricavi
description: In qualità di project manager, puoi utilizzare le tariffe di fatturazione per acquisire i ricavi relativi ai tuoi progetti.
author: Alina
feature: Work Management
exl-id: 400abcde-e368-4a70-89a9-05027900ab81
source-git-commit: 518a552845598a30fd547d432aa9d22dfef6ec8e
workflow-type: tm+mt
source-wordcount: '3313'
ht-degree: 0%

---

# Panoramica di fatturazione e ricavi

In qualità di project manager, puoi utilizzare le tariffe di fatturazione per acquisire i ricavi relativi ai tuoi progetti.

Questo articolo descrive il tracciamento dei ricavi per i progetti. I ricavi vengono calcolati in modo diverso nel rapporto Utilizzo. Per informazioni sui calcoli dei ricavi nel rapporto Utilizzo, vedi [Visualizza informazioni sull’utilizzo delle risorse](../../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Panoramica dei tassi di fatturazione

Quando si lavora con le tariffe di fatturazione, considera quanto segue:

* Per gestire le tariffe di fatturazione è necessaria una licenza di piano con accesso Modifica ai dati finanziari.\
   Per ulteriori informazioni sulla concessione dell&#39;accesso ai dati finanziari, vedere [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* I tassi di fatturazione sono importi di ricavi per unità di lavoro associati a ruoli di lavoro o utenti.

   Moltiplicare i tassi per le ore dedicate al lavoro genera ricavi per i tuoi progetti.

* Dopo aver stabilito le tariffe di fatturazione, puoi quindi tenere traccia dei ricavi creando dei record di fatturazione per registrare ciò che è stato fatturato e ciò che non è stato fatturato.

   >[!TIP]
   >
   >Quando si contrassegna un record di fatturazione come Fatturato, questo non può mai essere modificato. Questo è importante quando le tariffe variano e si desidera bloccare le informazioni su ricavi e spese sul progetto. Aggiungendolo a un record di fatturazione e contrassegnandolo come Fatturato, non viene aggiornato quando le tariffe vengono aggiornate nel sistema.

   Per ulteriori informazioni sulla creazione di record di fatturazione, consulta l’articolo [Creazione di record di fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md).

* È possibile creare tariffe di fatturazione per utenti, ruoli o un tasso di fatturazione una tantum per un progetto o un&#39;attività.

>[!IMPORTANT]
>
>Le percentuali che calcolano i ricavi appartengono all’utente che registra l’ora o ai relativi ruoli di lavoro.

* [Tassi di fatturazione utente](#user-billing-rates)
* [Tassi di fatturazione del ruolo di lavoro](#job-role-billing-rates)
* [Tassi di fatturazione fissi per progetti o attività](#fixed-billing-rates-for-projects-or-tasks)
* [Override tassi di fatturazione](#override-billing-rates)

### Tassi di fatturazione utente {#user-billing-rates}

In qualità di amministratore utente, quando crei un utente, puoi associarlo a un tasso di fatturazione specificando un valore per il campo Fatturazione per ora nel relativo profilo.\
Per ulteriori informazioni sulla creazione di utenti, consulta l’articolo [Aggiungi utenti](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)

![](assets/qs-user-edit-ui-with-rp-and-billing-per-hour-field-1-350x152.png)

### Tassi di fatturazione del ruolo di lavoro {#job-role-billing-rates}

In qualità di amministratore di Adobe Workfront, quando si crea un ruolo di lavoro, è possibile associarlo a un tasso di fatturazione specificando un valore per il campo Fatturazione/ora.

È possibile definire il valore di un tasso di fatturazione dei ruoli di lavoro utilizzando la valuta di base del sistema Workfront o un&#39;altra valuta personalizzata.

Per ulteriori informazioni sulla creazione di ruoli di lavoro e sull&#39;override della relativa valuta, consulta l&#39;articolo [Creare e gestire ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

![](assets/billing-rate-for-role-1-350x294.png)

### Tassi di fatturazione fissi per progetti o attività {#fixed-billing-rates-for-projects-or-tasks}

Oltre alle tariffe orarie per i ruoli utente e lavoro, puoi anche avere i seguenti tassi fissi di fatturazione:

* Importo fisso per tipo di ricavi orari fissi
* Importo fisso per tipo di ricavi fissi

Per ulteriori informazioni sull&#39;utilizzo dei tassi di fatturazione fissi per calcolare i ricavi, vedi [Panoramica dei tipi di ricavi delle attività](#overview-of-task-revenue-types).

### Override tassi di fatturazione {#override-billing-rates}

>[!IMPORTANT]
>
>È possibile sovrascrivere i tassi di fatturazione associati ai ruoli di lavoro. Non è possibile ignorare i tassi di fatturazione utente o i tassi fissi.

È possibile sostituire le percentuali di fatturazione dei ruoli di lavoro per:

* Un&#39;azienda specifica

   Per ulteriori informazioni sulla creazione di tassi di fatturazione dei ruoli di lavoro specifici per un&#39;azienda, consulta [Creare e modificare aziende](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Un progetto specifico

   Per ulteriori informazioni sulla creazione di tassi di fatturazione dei ruoli di lavoro specifici per un progetto, consulta l’articolo [Panoramica sulla priorità dei tassi di fatturazione dei ruoli di lavoro e sul calcolo dei ricavi per un progetto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Tracciare gli importi dei ricavi

Workfront può tenere traccia automaticamente dei ricavi pianificati quando le attività vengono create in base all&#39;ora pianificata delle attività.

Inoltre, può tenere traccia automaticamente dei ricavi effettivi quando le ore effettive sono registrate sulle attività, sui problemi e sul progetto.

Nella tabella seguente sono illustrati i tipi di ricavi associati a attività, problemi e progetti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Reddito Pianificato</td> 
   <td> <p>Per le attività, si tratta dei ricavi associati all'orario pianificato delle attività. Le ore pianificate di tutte le attività si estendono fino alle ore pianificate del progetto per contribuire al calcolo delle ore pianificate del progetto. </p> <p>Per ulteriori informazioni sulle ore pianificate in Workfront, vedi <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Panoramica sull’orario pianificato</a>. </p> <p>Workfront calcola i ricavi pianificati per attività e progetti utilizzando le seguenti formule:</p> <p><code>Task Planned Revenue = Planned Hours * Billing hourly rate</code> </p> <p><code>Project Planned Revenue = SUM (All tasks Planned Revenue) +&nbsp;Fixed Revenue</code> </p> 
   <p><b>NOTA</b>

<p>I ricavi pianificati del progetto visualizzati nell'area Dettagli progetto e nei rapporti sul progetto sono diversi dai ricavi pianificati visualizzati nel rapporto Utilizzo. </p> <p>I ricavi pianificati nell'area Dettagli progetto riflettono i ricavi delle attività associati all'attività Ore pianificate e i ricavi fissi del progetto. Nel rapporto Utilizzo dei ricavi pianificati vengono visualizzati i ricavi pianificati associati solo alle ore pianificate delle assegnazioni delle attività nel progetto. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p>Se il progetto dispone di 1 attività con 10 ore, assegnata a un Consulente con una tariffa oraria di $ 20 e il progetto ha un Ricavo fisso di $ 100, il rapporto Utilizzo visualizza $ 200 per Ricavi pianificati (i Ricavi pianificati associati alle ore dell'attività). Nella sezione Dettagli progetto viene visualizzato $300 (Ricavi pianificati dall'attività e Ricavi fissi per il progetto). </p> 
     </div> </p> <p>I ricavi pianificati attività vengono calcolati utilizzando la frequenza oraria di fatturazione degli utenti o dei ruoli di lavoro assegnati alle attività. Il tipo di ricavi delle attività influenza la percentuale (utente o ruolo) utilizzata per il calcolo dei ricavi pianificati. Per ulteriori informazioni, consulta le sezioni seguenti in questo articolo:</p> 
    <ul> 
     <li> <p><a href="#overview-of-task-revenue-types" class="MCXref xref">Panoramica dei tipi di ricavi delle attività</a> </p> </li> 
     <li> <p><a href="#revenue-calculations-for-tasks-based-on-user-and-role-assignments" class="MCXref xref">Calcoli dei ricavi per le attività basate su assegnazioni utente e ruolo</a> </p> </li> 
    </ul> <p>Per informazioni sui calcoli dei ricavi pianificati nel rapporto Utilizzo, vedi <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Visualizza informazioni sull’utilizzo delle risorse </a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reddito Reale*</td> 
   <td> <p>Associato all'orario effettivo di attività, problemi e progetti. </p> <p>In genere, Workfront calcola i ricavi effettivi utilizzando questa formula:</p> <p><code>Planned Revenue = Planned Hours * Billing rate</code> </p> <p>Per informazioni sui calcoli dei ricavi effettivi nel rapporto Utilizzo, vedi <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Visualizza informazioni sull’utilizzo delle risorse </a>. </p> <p><b>SUGGERIMENTO</b>

Non è possibile visualizzare i ricavi effettivi a livello di problema, ma i ricavi associati alle ore effettive sui problemi contribuiscono ai ricavi effettivi del progetto. </p> </td>
</tr> 
 </tbody> 
</table>

*Per le ore effettive, le tariffe dell&#39;utente si riferiscono sempre all&#39;utente che registra le ore o ai tassi dei propri ruoli. Per informazioni su quando Workfront utilizza le percentuali di utilizzo dei ruoli utente e quando utilizza le percentuali di tali ruoli, consulta la sezione [Calcoli dei ricavi](#revenue-calculations) in questo articolo.

<!--Note from the table for Planned Revenue line: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    -->

Ad esempio, se un&#39;attività con Tipo di ricavo orario utente è pianificata per 2 ore e l&#39;utente a cui è assegnato ha una tariffa oraria di 30 $ all&#39;ora, il Ricavo pianificato dell&#39;attività è di 60 $. Una volta completata l&#39;attività, se l&#39;utente registra solo 1,5 ore come tempo effettivo impiegato per completare l&#39;attività, l&#39;importo delle entrate effettive è pari a 45 $. Se un altro utente non assegnato all&#39;attività registra il tempo, i Ricavi effettivi vengono calcolati in base ai Tassi di fatturazione dell&#39;utente.

Puoi registrare i ricavi nei seguenti modi:

* Definendo il tipo di ricavi delle attività e associando utenti o ruoli assegnati a elementi di lavoro con i tassi di fatturazione. In questo modo i ricavi vengono calcolati in base alla quantità di ore pianificate o effettive sugli elementi di lavoro. È possibile impostare un limite all&#39;importo massimo addebitato per le tariffe orarie o meno.\
   Per ulteriori informazioni sulla specifica del tipo di ricavi di un&#39;attività, consulta l&#39;articolo [Modifica delle attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

* Fatturazione di un&#39;aliquota fissa dei ricavi per attività o progetti.\
   Se si dispone di attività con ricavi fissi, l&#39;importo Ricavo fisso verrà aggiunto come Ricavo pianificato di un&#39;attività o di un progetto e i Ricavi pianificati di un&#39;attività saranno disponibili per essere aggiunti a un Record di fatturazione come Ricavi fissi.
* Impostando una fatturazione piatta Fisso Ricavo per un progetto, quindi impostando tassi orari per le attività all&#39;interno del progetto. Workfront aggiunge le tariffe orarie per le attività al tasso fisso del progetto.\
   Ad esempio, un meccanico che utilizza Workfront potrebbe inserire un costo per le parti come entrate fisse per il progetto, quindi fatturare ogni ora per il tempo impiegato a riparare un&#39;auto. Ricavi fissi su progetti o attività vengono quindi realizzati al termine.

È inoltre possibile contrassegnare le attività come &quot;Non fatturabile&quot;, nel qual caso non sono associati ricavi pianificati o effettivi.

## Panoramica dei tipi di ricavi delle attività {#overview-of-task-revenue-types}

Per impostazione predefinita, il Tipo di ricavi di tutte le nuove attività viene impostato in base alle Preferenze attività e problemi specificate dal tuo amministratore di Workfront o di gruppo.\
Per ulteriori informazioni sulla definizione dell&#39;attività e sulle preferenze del problema per l&#39;istanza Workfront, consulta l&#39;articolo [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Il proprietario del progetto può modificare il tipo di ricavi delle attività e i ricavi fissi dei progetti.\
Per ulteriori informazioni sulla specifica dei ricavi fissi di un progetto, consulta l’articolo [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).\
Per ulteriori informazioni sulla specifica del tipo di ricavi di un&#39;attività, consulta l&#39;articolo [Modifica delle attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Puoi applicare i seguenti tipi di ricavi alle attività o ai progetti:

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
   <td> <p>Questo tipo può essere utilizzato con progetti e attività. </p> <p>Quando si allega un modello a un progetto, i Ricavi fissi del modello vengono aggiunti ai Ricavi fissi del progetto. Per informazioni, consulta <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Panoramica sull’associazione di un modello a un progetto</a>. </p> <p>Per le attività, indipendentemente dalle assegnazioni delle attività, i ricavi relativi all'attività vengono sempre calcolati utilizzando l'Importo fisso specificato nell'attività. </p> <p>I ricavi fissi delle attività figlio vengono aggregati ai ricavi dell'attività padre e quindi ai ricavi del progetto. Se viene definito un importo fisso sull'attività padre e/o sul progetto, l'importo viene aggiunto ai ricavi pianificati aggregati da qualsiasi attività figlio.</p> <p>L'importo dei ricavi fissi sulle attività può essere incluso in un record di fatturazione sul progetto.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ore Utente</p> </td> 
   <td> <p>Questo tipo può essere utilizzato solo per le attività. </p> <p>Il tasso di fatturazione impostato per un utente specifico moltiplicato per il numero di ore pianificate per l'attività diventa l'importo dei ricavi pianificati dell'attività. Il tasso di fatturazione impostato per un utente specifico moltiplicato per il numero di ore di accesso dell'utente all'attività è l'importo effettivo dei ricavi dell'attività. <br>Ad esempio, quando si crea un utente e si imposta $20 per il campo Fatturazione all'ora, se l'utente invia 5 ore per un'attività sulla scheda attività, l'importo Fatturazione effettiva dell'attività sarà $100.</p> <p><b>SUGGERIMENTO</b>

Questo è il tipo di ricavi predefinito quando crei un&#39;attività.</p> </td>
</tr> 
  <tr> 
   <td> <p>Ore Ruolo</p> </td> 
   <td> <p>Questo tipo può essere utilizzato solo per le attività.</p> <p>Questo tipo è simile a User Hourly ma utilizza le percentuali dei ruoli di lavoro anziché le tariffe utente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utente ogni ora con cap</p> </td> 
   <td> <p>Questo tipo può essere utilizzato solo per le attività.</p> <p>Le attività vengono fatturate ogni ora come nell’orario utente, ma dispongono di un importo massimo di sollecito che è possibile specificare. <br>Ad esempio, se il tasso di fatturazione di un utente è di $25, ma l'importo massimo sull'attività è di $20 e l'utente registra un'ora, il ricavo effettivo sull'attività è di $20. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ruolo ogni ora con cap</p> </td> 
   <td> <p>Questo tipo può essere utilizzato solo per le attività.</p> <p>Questo tipo è simile a User Hourly con Cap ma utilizza le percentuali dei ruoli di lavoro anziché le tariffe utente. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ore Utente più Fisso</p> </td> 
   <td> <p>Questo tipo può essere utilizzato solo per le attività. </p> <p>Le attività vengono fatturate ogni ora come nell'orario utente, ma dispongono di un Importo fisso che è possibile aggiungere alla tariffa utente. L'importo fisso specificato nell'attività può essere incluso nei record di fatturazione per il progetto. L'importo fisso non viene moltiplicato per le ore dell'attività. Solo il tasso di fatturazione dell'utente lo fa. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ore Ruolo più Fisso</p> </td> 
   <td> <p>Questo tipo può essere utilizzato solo per le attività. </p> <p>Le attività vengono fatturate ogni ora come in Ruolo orario, ma dispongono di un importo fisso aggiuntivo che è possibile aggiungere alla percentuale di ruolo. L'importo fisso specificato nell'attività può essere incluso nei record di fatturazione per il progetto. L'importo fisso non viene moltiplicato per le ore dell'attività. Solo il tasso di fatturazione del ruolo del lavoro lo fa. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ore Fisse</p> </td> 
   <td> <p>Questo tipo può essere utilizzato solo per le attività.</p> <p>L'importo di fatturazione è l'importo dell'importo fisso o dell'importo dell'importo fisso impostato per l'attività moltiplicato per il numero di ore immesse per l'attività (indipendentemente dall'utente o dai relativi ruoli di lavoro).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Non Fatturabile</p> </td> 
   <td> <p>Questo tipo può essere utilizzato solo per le attività.</p> <p>Questo tipo di ricavi non ha alcun effetto sui ricavi. </p> <p>Se un oggetto principale dispone di questa impostazione, le attività secondarie con un tipo di fatturazione continueranno ad essere applicate normalmente.</p> <p>Quando un utente senza accesso ai dati finanziari o senza autorizzazioni finanziarie in un modello crea un progetto da quel modello, si tratta del tipo di ricavi predefinito per le attività del progetto.</p> <p>Per informazioni sull'accesso ai dati finanziari, vedere l'articolo <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Concedere l’accesso ai dati finanziari</a>.<br>Per informazioni sulle autorizzazioni finanziarie per gli oggetti, consulta l’articolo <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Panoramica della condivisione delle autorizzazioni sugli oggetti</a>.<br>Per informazioni sulla creazione di progetti da modelli, consulta l’articolo <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Creare un progetto utilizzando un modello</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Panoramica dei ricavi per le attività principali

Se si modifica un&#39;attività autonoma con le relative informazioni di fatturazione in un&#39;attività padre, la nuova attività padre conserva tutte le informazioni di fatturazione precedentemente applicate, insieme alle ore precedentemente applicate. Tutte le informazioni di fatturazione provenienti dalle ore registrate nelle attività figlio verranno raggruppate come Entrate effettive nella nuova attività padre.

Anche i ricavi pianificati delle attività figlio vengono aggregati all&#39;attività padre.

## Panoramica dei ricavi per i problemi

I problemi non hanno importi di ricavi pianificati o effettivi, ma possono avere costi effettivi.

Se si registrano le ore per un problema e si utilizza un tipo di ora contrassegnato come &quot;Conteggio come ricavi&quot;, Workfront calcola un importo del costo effettivo in base al tasso dell&#39;utente che registra nel tempo. Questo numero viene aggiunto al costo effettivo del progetto. Le ore possono anche essere incluse in un record di fatturazione.

Per ulteriori informazioni sui costi di tracciamento, consulta l’articolo [Costi di tracciamento](../../../manage-work/projects/project-finances/track-costs.md).

Per ulteriori informazioni sui tipi di ora, consulta l’articolo [Gestione dei tipi di ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Calcoli dei ricavi

* [Calcoli dei ricavi per le attività basate su assegnazioni utente e ruolo](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)

### Calcoli dei ricavi per le attività basate su assegnazioni utente e ruolo {#revenue-calculations-for-tasks-based-on-user-and-role-assignments}

Quando si calcolano i ricavi per un&#39;attività, tenere presente quanto segue:

* Se un utente o un ruolo di lavoro mostra un tasso di $ 0,00, Workfront lo legge come un importo valido e lo moltiplicherà per il numero di ore sull&#39;attività per calcolare i ricavi. Se non si desidera visualizzare alcun ricavo per le attività, assicurarsi che il campo relativo al tasso di fatturazione per il ruolo utente o processo sia vuoto.
* Quando si applicano le tariffe di fatturazione dei ruoli di lavoro, Workfront utilizza la percentuale di sostituzione a livello di progetto, invece del tasso di fatturazione per quel ruolo definito a livello di sistema ogni volta che si verifica un tasso di sostituzione sul progetto.
* Nel caso di più assegnatari sulle attività, per ciascun assegnatario si applicano gli scenari descritti di seguito.

Esiste una gerarchia di cui viene utilizzato il tasso nei calcoli dei ricavi in base alle assegnazioni delle attività.

Se l’amministratore di Workfront ha abilitato la **Assegnare manualmente i ruoli del processo alle voci orarie** nell’area Preferenze fogli orari e ore e il tempo di registrazione dell’utente sul progetto seleziona un ruolo diverso da associare a questo momento, il Ricavo effettivo dell’attività o del progetto calcola sempre in base al ruolo associato all’immissione dell’ora. Per informazioni sull’abilitazione del tempo di registrazione per un ruolo di lavoro specifico, consulta l’articolo [Preferenze scheda attività e ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Esistono i seguenti scenari quando si calcolano i ricavi dell&#39;attività in base al tipo di ricavi e alla natura dell&#39;assegnazione dell&#39;attività:

* **Il tipo di ricavi dell’attività è Orario utente**

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Fatturazione per ora</td> 
     <td>Nessuna assegnazione</td> 
     <td>Assegnazione utente</td> 
     <td>Assegnazione ruolo lavoro</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Fatturazione per ora per ricavi pianificati</td> 
     <td>$0.00</td> 
     <td> Se un utente ha un tasso di fatturazione nel proprio profilo, tale tasso viene utilizzato per calcolare i ricavi pianificati. In caso contrario, viene utilizzato il tasso di fatturazione del sistema relativo al ruolo di lavoro principale. <br><p><b>NOTA</b>  L’utente può essere assegnato all’attività con uno dei propri ruoli di lavoro secondari, ma in questo caso viene utilizzato il tasso del ruolo di lavoro principale.</p></td> 
     <td>Il tasso di fatturazione del sistema del ruolo di lavoro assegnato all'attività viene utilizzato per calcolare i ricavi pianificati. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Fatturazione per ora per i ricavi effettivi</td> 
     <td>Se l’utente che registra le ore ha un tasso di fatturazione nel proprio profilo, tale tasso viene utilizzato. <br>In caso contrario, viene utilizzato il tasso di fatturazione del ruolo principale del lavoro. Se non esiste un tasso di fatturazione associato all'utente o al suo ruolo principale, il ricavo effettivo è di $0,00. <br><p><b>NOTA</b>

   Per il calcolo vengono prese in considerazione solo le percentuali associate all’utente che registra l’ora, anche quando un altro utente viene assegnato all’attività.</p></td>
   <td>Se l’utente che registra le ore ha un tasso di fatturazione nel proprio profilo, tale tasso viene utilizzato. <br>In caso contrario, viene utilizzato il tasso di fatturazione del ruolo principale del lavoro. Se non esiste un tasso di fatturazione associato all'utente o al suo ruolo principale, il ricavo effettivo è di $0,00. <br><p><b>NOTA</b>

   Per il calcolo vengono prese in considerazione solo le percentuali associate all’utente che registra l’ora, anche quando un altro utente viene assegnato all’attività.</p></td>
   <td>Se l’utente che registra le ore ha un tasso di fatturazione nel proprio profilo, tale tasso viene utilizzato. In caso contrario, viene utilizzato il tasso di fatturazione del ruolo principale del lavoro.<br><p><b>NOTA</b>

   Se il tempo di registrazione dell&#39;utente non ha un tasso di fatturazione associato a tale periodo e non dispone di un ruolo o di un tasso di fatturazione per il ruolo di lavoro, viene utilizzato il tasso del ruolo di lavoro associato all&#39;attività. Se non esiste un tasso di fatturazione per questo ruolo, il ricavo è $0,00</p></td>
   </tr> 
   </tbody> 
  </table>

* **Il tipo di ricavi dell’attività è Ruolo orario**

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Fatturazione per ora</td> 
     <td>Nessuna assegnazione</td> 
     <td>Assegnazione utente</td> 
     <td>Assegnazione ruolo lavoro</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Fatturazione per ora per ricavi pianificati</td> 
     <td>$0.00</td> 
     <td>Workfront esamina il ruolo del lavoro svolto dall’utente sull’attività per calcolare i ricavi pianificati. <br>Se l'utente non è associato ad alcun ruolo sull'attività, il Ricavo è $0,00. </td> 
     <td>Il tasso di fatturazione del ruolo di lavoro assegnato all'attività viene utilizzato per calcolare i ricavi pianificati.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Fatturazione per ora per i ricavi effettivi</td> 
     <td>Workfront utilizza il tasso di fatturazione del ruolo principale del lavoro dell'utente che registra l'ora. <br>Se l'utente che registra l'ora non ha un ruolo di lavoro associato a loro, o se il ruolo di lavoro principale non ha un tasso di fatturazione, le entrate effettive sono $0,00. </td> 
     <td> Se l'utente che registra l'ora è assegnato all'attività, il tasso di fatturazione del ruolo di processo associato all'utente sull'attività viene utilizzato per calcolare i ricavi effettivi. In caso contrario, viene utilizzato il tasso di fatturazione del ruolo principale del lavoro. Se l'utente non ha un ruolo di lavoro principale o se il suo ruolo di lavoro principale non ha un tasso di fatturazione, il Ricavo effettivo è di $0,00. </td> 
     <td>Se uno dei ruoli dell'utente che registra il tempo viene assegnato all'attività, viene utilizzata la percentuale di ruolo del processo. Se il ruolo di lavoro assegnato all'attività non è associato all'utente che registra l'ora, il tasso di fatturazione del ruolo principale dell'utente viene utilizzato per calcolare i ricavi effettivi. Se l'utente non dispone di un ruolo o non esiste un tasso associato al ruolo di lavoro principale, viene utilizzato il tasso del ruolo di lavoro assegnato all'attività. </td> 
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

### Calcolo dei ricavi per i progetti

Puoi tenere traccia dei seguenti tipi di ricavi per i progetti:

* I ricavi pianificati per un progetto vengono calcolati con la seguente formula:

   ```
   Project Planned Revenue = SUM(Task Planned Revenue)+ Fixed Revenue
   ```

   Per informazioni sul calcolo dei ricavi pianificati dell&#39;attività, consulta la sezione [Calcoli dei ricavi per le attività basate su assegnazioni utente e ruolo](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) in questo articolo.

* I ricavi effettivi per un progetto vengono calcolati con la seguente formula:

   ```
   Project Actual Revenue = SUM (Task Actual Revenue) + (Hours logged for the project x User Billing per Hour Rate) + SUM (Hours logged for the issues x User Billing per Hour rate)
   ```

Per informazioni sul calcolo dei ricavi effettivi dell&#39;attività, vedere la sezione [Calcoli dei ricavi per le attività basate su assegnazioni utente e ruolo](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) in questo articolo.

Per i ricavi effettivi associati alle ore registrate direttamente nel progetto o ai problemi, Workfront utilizza il Billing Rate (Tasso di fatturazione) dell’utente che accede al progetto. Se all’utente non è associato alcun tasso di fatturazione al suo profilo, Workfront utilizza il tasso di fatturazione del ruolo di lavoro principale. Se entrambi i tassi sono pari a zero, i ricavi effettivi associati alle ore registrate nel progetto o i problemi sono pari a zero.
