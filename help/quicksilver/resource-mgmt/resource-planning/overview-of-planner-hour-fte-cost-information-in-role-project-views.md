---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Panoramica su ore, FTE e informazioni sui costi nelle visualizzazioni Progetto e Ruolo della Programmazione delle risorse
description: Panoramica di ore, FTE e informazioni sui costi nelle visualizzazioni Progetto e Ruolo della Programmazione delle risorse
author: Lisa
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '2977'
ht-degree: 0%

---

# Panoramica di ore, FTE e informazioni sui costi nelle visualizzazioni Progetto e Ruolo della Programmazione delle risorse

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

La pianificazione delle risorse è la funzione principale delle risorse per il lavoro da eseguire in un progetto. Puoi visualizzare il tempo disponibile delle risorse e assegnarlo ai progetti a cui sono assegnate.

Per informazioni sull&#39;impostazione del budget delle risorse nella Programmazione delle risorse, vedere [Risorse preventivate nella Programmazione delle risorse utilizzando le visualizzazioni Progetto e Ruolo](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

In questo articolo vengono descritti alcuni concetti chiave che è necessario conoscere prima di iniziare a pianificare le risorse in Pianificazione risorse.

## Panoramica risorse budget

Quando si definiscono i budget per le risorse utilizzando la Programmazione risorse, tenere presente quanto segue:

* È possibile preventivare l&#39;allocazione delle risorse specificando una quantità di ore, FTE o Costo che le risorse possono utilizzare per completare il lavoro sui progetti. Quando si calcola il tempo o il costo per una risorsa, le ore disponibili, l&#39;FTE o il costo per la risorsa diminuiscono in base all&#39;importo preventivato. Di conseguenza, gli importi di Ore, FTE o Costo disponibili per i progetti che seguono il progetto per il quale si sta definendo il budget diminuiscono per gli utenti e i ruoli di tali progetti.

  >[!IMPORTANT]
  >
  >È possibile preventivare le risorse per un periodo di 15 anni. Se si preventivano le risorse per un progetto con una durata superiore a 15 anni, le informazioni di definizione del budget potrebbero non essere accurate.

* È possibile preventivare ore, FTE o Costo per le risorse per qualsiasi intervallo di tempo visualizzato nella Programmazione delle risorse, indipendentemente dalla sequenza temporale del progetto. Ad esempio, se vuoi indicare che le risorse potrebbero non essere disponibili durante la timeline del progetto (dove sono associate alle ore pianificate), ma potrebbero essere disponibili in un altro momento, puoi preventivarle per intervalli di tempo in cui le ore pianificate sono zero, se questo è il momento in cui diventano disponibili per lavorare. Dopo aver eseguito questa operazione, puoi modificare manualmente la timeline del progetto in modo che corrisponda alla disponibilità della risorsa.

  >[!NOTE]
  >
  >È consigliabile preventivare manualmente ore, FTE o Costo per le mansioni o per gli utenti. È possibile utilizzare le opzioni automatiche per preventivare il tempo per i progetti e le risorse solo quando si è certi che la quantità di ore pianificate, FTE o Costo debba sempre corrispondere alle ore preventivate, FTE o Costo.\
  >Per informazioni sull&#39;utilizzo delle opzioni automatiche per l&#39;impostazione del budget nella Programmazione risorse, vedere la sezione &quot;Progetti e ruoli di budget automaticamente&quot; nell&#39;articolo [Verificare la disponibilità e l&#39;allocazione delle risorse mediante la Programmazione risorse di Adobe Workfront](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

* La definizione del budget per FTE o costi è identica alla definizione del budget per le ore, in cui Adobe Workfront utilizza i valori FTE e costo invece delle ore per le risorse preventivate.

  Per ulteriori informazioni sul calcolo dei costi nella Programmazione delle risorse, vedere [Calcolare i costi nella Programmazione delle risorse](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

* Le allocazioni di budget per le risorse nella Programmazione risorse vengono eseguite nei modi seguenti:

   * Manualmente

     Oppure

   * Automaticamente, utilizzando le opzioni di progetto e ruolo nelle visualizzazioni **Visualizza per progetto** e **Visualizza per ruolo**.

  Per ulteriori informazioni, vedere [Risorse preventivate nella Programmazione delle risorse utilizzando le visualizzazioni Progetto e Ruolo](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

* Quando un utente cambia i ruoli, viene eliminato, disattivato o rimosso da un Pool di Risorse, le ore preventivate per il ruolo non cambiano e vengono ridistribuite agli altri utenti del ruolo. Se nessun utente è più associato alla mansione, le ore preventivate per la mansione diventano pari a zero.

Per ulteriori informazioni sulle opzioni di progetto e ruolo, vedere la sezione [Comprendere i valori di Ore, FTE e Costo nella Programmazione delle risorse](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner) in questo articolo.

## Comprendere i valori di Ore, FTE e Costo nella Programmazione delle risorse {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

Prima di definire il budget delle risorse e aggiornare le informazioni sulle ore preventivate nella Programmazione delle risorse, è necessario conoscere i concetti seguenti

* **Ore pianificate, FTE o Costo**: il lavoro da eseguire come definito per attività e problemi.
* **Ore disponibili, FTE o Costo**: la quantità di tempo in cui gli utenti o le mansioni sono disponibili a lavorare, in base alle pianificazioni associate agli utenti.

Queste informazioni vengono visualizzate nella Programmazione delle risorse per ogni risorsa (utente o ruolo) e per ogni progetto.

Per informazioni sulle visualizzazioni del progetto e dei ruoli, vedere l&#39;articolo [Panoramica sulla navigazione di Programmazione delle risorse](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Per informazioni sul calcolo dei costi nella Programmazione delle risorse, vedere l&#39;articolo [Calcolare i costi nella Programmazione delle risorse](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

>[!NOTE]
>
>La definizione del budget per costo è identica alla definizione del budget per ore o FTE, ma è necessario comprendere in che modo Workfront calcola il costo per la programmazione delle risorse.
>
>Per informazioni sul metodo di calcolo dei costi in Pianificazione risorse, vedere l&#39;articolo [Calcolare i costi in Pianificazione risorse](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

Le tabelle seguenti mostrano le informazioni relative all&#39;allocazione e alla disponibilità visualizzate nella Programmazione delle risorse quando si applica la vista Progetto o Ruolo. È possibile visualizzare queste informazioni per ore, FTE o Costo:

* [Colonna AVL (disponibile)](#the-avl-available-column)
* [Colonna PLN (pianificato)](#the-pln-planned-column)
* [Colonna BDG (preventivato)](#the-bdg-budgeted-column)
* [Colonna VAR (Varianza)](#the-var-variance-column)
* [Colonna NET](#the-net-column)

### Colonna AVL (disponibile) {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visualizzato da</strong> </td> 
   <td><strong>Descrizione</strong> </td> 
  </tr> 
  <tr> 
   <td>Progetto </td> 
   <td> <p>Totale di ore, FTE o Costo per cui tutti gli utenti del progetto sono disponibili a lavorare in base alla programmazione, per l'intervallo di tempo selezionato. </p> </td> 
  </tr> 
  <tr> 
   <td>Ruolo</td> 
   <td> <p>Il totale di ore, FTE o Costo per cui tutti gli utenti associati a questo ruolo sono disponibili a lavorare in base alla loro pianificazione e alla loro <strong>Percentuale di disponibilità FTE</strong> per quel ruolo specifico, per l'intervallo di tempo selezionato. </p> <p>Considera quanto segue: </p> 
    <ul> 
     <li>Se nessun utente è associato a una mansione, il valore di Ore disponibili per la mansione è zero. </li> 
     <li>Se un utente è associato a un Ruolo principale, ma la <strong>Percentuale di disponibilità FTE</strong> per il ruolo è 0%, il valore Ore disponibili per il ruolo è zero.</li> 
     <li>Se l'utente è associato ad Altri ruoli e la <strong>Percentuale di disponibilità FTE</strong> per i ruoli è 0%, gli altri ruoli non sono elencati nella Programmazione delle risorse e l'utente viene visualizzato solo sotto il proprio Ruolo principale.</li> 
    </ul> <p>Per ulteriori informazioni sulla <strong>Percentuale di disponibilità FTE</strong> per una mansione, vedere l'articolo <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente</a>.</p> <p>Per ulteriori informazioni sul calcolo della disponibilità dei ruoli nella Programmazione delle risorse, vedere la sezione "Calcolare le ore e l'FTE disponibili per un ruolo nella Programmazione delle risorse" nell'articolo <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Panoramica sul calcolo delle ore e dell'FTE per utenti e ruoli nella Programmazione delle risorse</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td> <p>Ore, FTE o Costo che l’utente è disponibile a lavorare, in base alla propria pianificazione, per l’intervallo di tempo selezionato. Questo numero sottrae le ore associate ai seguenti elementi:</p> 
    <ul> 
     <li>eccezioni di pianificazione</li> 
     <li>indisponibilità dell'utente</li> 
     <li>ore preventivate per altri progetti. </li> 
    </ul> <p>Le ore, FTE o Costo disponibili per un utente cambiano in base a quanto segue: </p> 
    <ul> 
     <li>modalità di calcolo della programmazione e dell'FTE in base alle preferenze di gestione delle risorse a livello di sistema.<br><p>Per ulteriori informazioni sul calcolo della disponibilità di utenti e ruoli, vedere l'articolo <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Panoramica sul calcolo delle ore e dell'FTE per utenti e ruoli nella pianificazione delle risorse</a>.</p>
     Per ulteriori informazioni sulla configurazione delle preferenze di Gestione risorse in Workfront, vedere <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurare le preferenze di Gestione risorse</a></li> 
    </ul> 
    <ul> 
     <li>la <strong>Priorità pianificazione progetto</strong>, se l'utente è preventivato per il lavoro.<br>Per ulteriori informazioni su come la priorità di pianificazione del progetto influisce sulle ore disponibili di un utente, vedere <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Panoramica sulla navigazione di Programmazione delle risorse </a>. </li> 
    </ul> <p>Se l'utente è programmato per la disattivazione, le ore disponibili, FTE o Costo per i giorni successivi alla data di disattivazione sono pari a zero. <br>Per ulteriori informazioni sulla disattivazione degli utenti, vedere l'articolo <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Disattivare o riattivare un utente</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Colonna PLN (Pianificato) {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visualizzato da</strong> </td> 
   <td><strong>Descrizione</strong> </td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td> <p>Totale delle ore pianificate, FTE o Costo di tutti i ruoli o utenti elencati nel progetto, incluso nelle sezioni <strong>Nessun ruolo</strong> o <strong>Nessun utente</strong>, per l'intervallo di tempo selezionato e come visualizzato nella scheda Dettagli progetto del progetto. </p> <p><b>NOTA</b>

Gli adeguamenti manuali delle allocazioni utente giornaliere potrebbero modificare il valore delle ore pianificate settimanali, mensili o trimestrali nella pianificazione risorse. Puoi regolare manualmente le allocazioni giornaliere degli utenti per attività e problemi utilizzando il Bilanciatore dei carichi di lavoro. Per ulteriori informazioni, consulta <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gestire le allocazioni utente nel Bilanciatore dei carichi di lavoro</a>.</p> </td>
</tr> 
  <tr> 
   <td>Ruolo</td> 
   <td> <p>Totale delle ore pianificate da tutte le attività assegnate al ruolo durante l'intervallo di tempo selezionato. </p> <p>Nella sezione <strong>Nessun ruolo</strong> verranno visualizzate le ore pianificate associate alle attività non assegnate, assegnate ai team (le cui ore sono elencate nella sezione <strong>Nessun utente</strong>) o assegnate a utenti non associati a una mansione. </p> </td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td> <p>Le ore pianificate da tutte le attività assegnate all'utente in un ruolo specifico, durante l'intervallo di tempo selezionato. </p> <p>Nella sezione <strong>Nessun utente</strong> verranno visualizzate le ore pianificate associate alle attività non assegnate o assegnate ai team. </p> </td> 
  </tr> 
 </tbody> 
</table>

Quando visualizzi le ore pianificate, tieni presente quanto segue:

* Sebbene non sia possibile visualizzare informazioni sulle allocazioni delle attività nella Programmazione delle risorse nelle visualizzazioni Progetto e Ruolo, la quantità di ore pianificate deriva dalle ore pianificate per le attività nei progetti.
* Le ore pianificate vengono distribuite in modo uniforme a ogni giorno entro la Durata delle attività, per ogni risorsa ad esse assegnata. La durata dell&#39;attività è basata sulle date pianificate di inizio e completamento dell&#39;attività e include ogni giorno di calendario compreso in tale periodo di tempo.\
  Workfront prende in considerazione la pianificazione dell’utente o del progetto al momento della distribuzione delle ore pianificate agli utenti o ai progetti. In questo caso, le ore pianificate vengono distribuite in modo uniforme a ogni giorno entro la durata delle attività, esclusi i fine settimana, i giorni di ferie e le eccezioni alla pianificazione.\
  Se ad esempio si visualizza la Pianificazione risorse per settimana e si dispone di attività che si estendono su più settimane nei progetti, il numero di ore pianificate alla settimana dipende dal numero di giorni della settimana che fanno parte della Durata dell&#39;attività. Questa funzione funziona in modo simile quando si visualizza la Programmazione delle risorse per mese o trimestre e quando le attività si estendono su più mesi o trimestri.\
  I giorni di fine settimana, le eccezioni alla programmazione e i giorni di ferie sono esclusi da questa distribuzione.
* Le seguenti categorie di attività sono incluse nel calcolo delle ore pianificate per ciascuna risorsa:

   * le attività assegnate agli utenti nei Pool di Risorse, le mansioni o i team nel progetto\
     Se le attività sono assegnate ai team, la loro allocazione verrà visualizzata nelle sezioni **Nessun ruolo** e **Nessun utente**. Puoi visualizzare le ore pianificate associate ai team, ma non puoi preventivarle, perché alle attività non sono associati ruoli né utenti.

   * attività non assegnate

* Le ore pianificate nella pianificazione risorse non includono le ore pianificate associate ai seguenti elementi:

   * attività padre
   * attività assegnate a utenti senza gruppi di risorse
   * problemi, quando l&#39;impostazione **Includi ore da problemi** è disabilitata.

* Le ore pianificate non vengono visualizzate nella Programmazione delle risorse se la Durata dell&#39;attività è zero.
* Le ore pianificate associate agli utenti disattivati non vengono visualizzate.

### Colonna BDG (Preventivato) {#the-bdg-budgeted-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visualizzato da</strong> </td> 
   <td><strong>Descrizione</strong> </td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td> <p>Inserimento manuale per stimare il numero di ore, FTE o Costo preventivato per un progetto per un intervallo di tempo selezionato. </p> <p>Nella vista Progetto, le ore preventivate per il progetto vengono distribuite alle mansioni elencate nel progetto. La quantità di ore pianificate per ciascun ruolo determina il modo in cui le ore pianificate vengono distribuite ai ruoli. Le ore preventivate vengono distribuite ai ruoli con valori Ore pianificate più elevati. </p> <p>Nella vista Ruolo, le ore preventivate per il progetto non vengono distribuite ai ruoli o agli utenti del progetto. </p> </td> 
  </tr> 
  <tr> 
   <td>Ruolo</td> 
   <td> <p>Inserimento manuale per stimare il numero di ore preventivate per un ruolo per un intervallo di tempo selezionato. </p> <p>Se nessun utente è associato alla mansione, non è possibile stimare le ore preventivate per la mansione. </p> <p>Nella vista Ruolo, le ore preventivate per il ruolo vengono distribuite ai progetti elencati sotto il ruolo. La quantità di ore pianificate per ciascun progetto determina il modo in cui le ore pianificate vengono distribuite ai progetti. Le ore preventivate vengono distribuite ai progetti con valori Ore pianificate più elevati.</p> <p>Nella vista Progetto, le ore preventivate per il ruolo non vengono distribuite ai progetti o agli utenti associati al ruolo. </p> </td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td> <p>Inserimento manuale per stimare il numero di ore preventivate per un utente per un intervallo di tempo selezionato. </p> <p> <p><b>NOTA</b>   È possibile stimare le ore preventivate per gli utenti che non sono assegnati ad attività, ma sono associati a un Pool di Risorse in un progetto perché questi utenti vengono visualizzati anche nella Programmazione risorse. Le ore pianificate devono essere zero, tuttavia, se non sono assegnate ad attività. </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Quando si lavora con le ore preventivate, considera quanto segue:

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(Duplicated below ??)
</MadCap:conditionalText>
-->

* È possibile preventivare le risorse solo se si dispone dell&#39;accesso Modifica a Gestione risorse e dati finanziari e delle autorizzazioni Gestisci dati finanziari per i progetti.

  Per informazioni sull&#39;accesso necessario per l&#39;impostazione del budget delle risorse, vedere l&#39;articolo [Accesso necessario per il preventivo delle risorse in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Per impostazione predefinita, le ore preventivate nella pianificazione risorse sono pari a zero per tutte le risorse e per tutti i progetti.
* Puoi stimare manualmente le ore preventivate per utenti e ruoli, oppure puoi utilizzare uno dei collegamenti nei menu Progetto o Ruolo **Altro** per aggiornarli in base al numero di ore pianificate.\
  Per ulteriori informazioni sulle opzioni di progetto e ruolo, vedere la sezione [Panoramica su ore, FTE e informazioni sui costi nelle visualizzazioni Progetto e Ruolo della Programmazione delle risorse](#Budget) in questo articolo.

* Il periodo di tempo più piccolo per il quale è possibile preventivare ore, FTE o Costo è una settimana. Impossibile preventivare ore, FTE o Costo per un giorno.
* Le ore preventivate vengono equamente distribuite a ogni giorno entro la Durata delle attività, per ogni risorsa ad esse assegnata. La durata dell&#39;attività è basata sulle date pianificate di inizio e completamento dell&#39;attività e include ogni giorno di calendario compreso in tale periodo di tempo.\
  Workfront tiene conto della pianificazione dell’utente o del progetto al momento della distribuzione delle ore preventivate agli utenti o ai progetti. In questo caso, le ore preventivate vengono distribuite in modo uniforme a ogni giorno entro la durata delle attività, esclusi i fine settimana, ma incluse le eccezioni di indisponibilità e di programmazione.\
  Se ad esempio si visualizza la Programmazione delle risorse per settimana e si dispone di attività che si estendono su più settimane, il numero di ore preventivate per settimana dipende dal numero di giorni della settimana che fanno parte della Durata dell&#39;attività. I giorni di fine settimana sono esclusi da questa distribuzione. Questa funzione funziona in modo simile quando si visualizza la Programmazione delle risorse per mese o trimestre e quando le attività si estendono su più mesi o trimestri.

* Puoi generare rapporti sulle ore preventivate selezionando Ore preventivate come oggetto del rapporto per un nuovo rapporto.\
  Per informazioni sugli oggetti su cui è possibile creare rapporti in Workfront, vedere la sezione &quot;Report sugli oggetti&quot; nell&#39;articolo [Comprendere gli oggetti in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
  Per informazioni sulla creazione di un report Ore preventivate, vedere l&#39;articolo [Report: Ore preventivate](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

* Le ore preventivate in precedenza per gli utenti che sono stati successivamente disattivati non vengono visualizzate.

### Colonna VAR (Varianza) {#the-var-variance-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visualizzato da</strong> </td> 
   <td><strong>Descrizione</strong> </td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td> <p>Il valore Ora, FTE o Variazione costo indica se il numero di ore preventivate è sufficiente per il progetto per completare tutte le ore pianificate per il progetto. </p> <p>L'Ora progetto, FTE o Variazione costo viene calcolata utilizzando la formula seguente:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Ruolo</td> 
   <td> <p>Nel campo Ore, FTE o Variazione costo viene indicato se il numero di ore preventivate, FTE o Costo del ruolo è sufficiente per completare le ore pianificate assegnate al ruolo. </p> <p>L'Ora del ruolo, l'FTE o lo Scostamento costo viene calcolato utilizzando la formula seguente:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td> <p>Le ore, il valore FTE o lo scostamento costo indicano se le ore preventivate sono sufficienti per consentire all'utente di eseguire le ore pianificate assegnate. </p> <p>Le ore utente, il valore FTE o lo scostamento costo vengono calcolati utilizzando la formula seguente:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Quando le ore, il valore FTE o lo scostamento costi sono visualizzati in rosso, è stato stimato un numero di ore preventivate inferiore alle ore pianificate del lavoro effettivo da completare. In questo caso, le ore preventivate potrebbero non essere sufficienti per completare il lavoro.

### Colonna NET  {#the-net-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Visualizzato da</strong> </td> 
   <td><strong>Descrizione</strong> </td> 
  </tr> 
  <tr> 
   <td>Progetto</td> 
   <td> 
    <div> 
     <p>Nel progetto Ore nette, FTE o Costo può essere visualizzato uno dei seguenti elementi: </p> 
     <ul> 
      <li> <p>Differenza tra il tempo o costo disponibile e il tempo o costo preventivato per il progetto:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>Differenza tra il tempo o costo disponibile e il tempo o costo pianificato per il progetto, quando l'impostazione Usa valori pianificati (PLN) nei calcoli NETTI è abilitata: </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>SUGGERIMENTO</b></p>        
  <p>Questa opzione viene applicata solo quando si personalizza la vista nella sezione Visualizza elementi selezionati.</p>
  <p>Per ulteriori informazioni, vedere <a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >Verificare la disponibilità e l'allocazione delle risorse tramite Adobe Workfront Resource Planner</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>Ruolo</td> 
   <td> 
    <div> 
     <p>Il ruolo Ore nette, FTE o Costo può mostrare uno dei seguenti elementi: </p> 
     <ul> 
      <li> <p>Differenza tra il tempo o costo disponibile e il tempo o costo preventivato per il ruolo:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>Differenza tra il tempo o costo disponibile e il tempo o costo pianificato per il ruolo quando l'impostazione Usa valori pianificati (PLN) nei calcoli NET è abilitata:</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>SUGGERIMENTO</b> <span>

Questa opzione viene applicata solo quando si personalizza la visualizzazione nella sezione Visualizza elementi selezionati.</span> </p> <p><span>Per ulteriori informazioni, vedere </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Verificare la disponibilità e l&#39;allocazione delle risorse tramite Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>Utente</td> 
   <td> 
    <div> 
     <p>L'utente Net Hours, FTE o Cost può visualizzare uno dei seguenti elementi: </p> 
     <ul> 
      <li> <p>Differenza tra il tempo o costo disponibile e il tempo o costo preventivato per l'utente:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>Differenza tra il tempo o costo disponibile e il tempo o costo pianificato per l'utente quando l'impostazione Usa valori pianificati (PLN) nei calcoli NET è abilitata:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>SUGGERIMENTO</b> <span>

Questa opzione viene applicata solo quando si personalizza la visualizzazione nella sezione Visualizza elementi selezionati.</span> </p> <p><span>Per ulteriori informazioni, vedere </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Verificare la disponibilità e l&#39;allocazione delle risorse tramite Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Quando le ore NETTE, FTE o Costo sono visualizzati in rosso, il tempo disponibile o il budget non sono sufficienti per coprire il Budget** o il Tempo pianificato o il costo associato al lavoro. In questo caso, le risorse sono sovrassegnate.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the table below is ideal but it does not transfer to Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours, FTE, or Cost)</strong> </td>
<td><strong>Displayed by</strong> </td>
<td><strong>Description</strong> </td>
</tr>
<tr>
<td rowspan="3">AVL <br>(Available Hours, FTE, or Cost)</td>
<td>Project </td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users on the project are available to work according to their schedule, for the time frame selected. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users associated with this role are available to work according to their schedule and their <strong>Percentage of FTE Availability</strong> for that specific role, for the time frame selected. </p> <p>Consider the following: </p>
<ul>
<li>If no user is associated with a job role, then the value for the Available Hours for the job role is zero. </li>
<li>If a user is associated with a Primary Job Role, but the <strong>Percentage of FTE Availability</strong> for the role is 0%, the job role Available Hours value is zero.</li>
<li>If the user is associated with Other Roles and the <strong>Percentage of FTE Availability</strong> for the roles is 0%, the Other Roles are not listed in the Resource Planner and the user displays only under their Primary Role.</li>
</ul> <p>For more information about the <strong>Percentage of FTE Availability</strong> for a job role, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> <p>For more information about how the job role availability is calculated in the Resource Planner, see the section "Calculate the Available Hours and FTE for a job role in the Resource Planner" in the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>Hours, FTEs, or Cost that the user is available to work, according to their schedule, for the time frame selected. This number subtracts the hours associated with the following:</p>
<ul>
<li>schedule exceptions</li>
<li>time off of the user</li>
<li>hours budgeted for other projects. </li>
</ul> <p>The Available Hours, FTEs, or Cost for a user change according the following: </p>
<ul>
<li>how their schedule and FTE are calculated based on the Resource Management Preferences at the system level.<br>For more information about calculating user and job role availability, see the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</li>
</ul>
<ul>
<li>the <strong>Project Planning Priority</strong>, if the user is budgeted for work.<br>For more information about how Project Planning Priority affects the Available Hours of a user, see <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Resource Planner navigation overview </a>. </li>
</ul> <p>If the user is scheduled for deactivation, the Available Hours, FTEs, or Cost for the days after the deactivation date are zero. <br>For more information about deactivating users, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</p> </td>
</tr>
<tr>
<td rowspan="4">PLN <br>(Planned Hours, FTE, or Cost)</td>
<td>Project</td>
<td> <p>The total of the Planned Hours, FTEs, or Cost from all the job roles or users listed under the project, including in the <strong>No Role</strong> or <strong>No User</strong> sections, for the time frame selected, and as displayed in the Project Details tab of the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of the Planned Hours from all the tasks assigned to the role, during the time frame selected. </p> <p>The <strong>No Role</strong> section will show the Planned Hours associated with tasks that are either unassigned, assigned to teams (whose hours are listed in the <strong>No User</strong> section), or assigned to users who are not associated with a job role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Planned Hours from all the tasks assigned to the user in a specific role, during the time frame selected. </p> <p>The <strong>No User</strong> section will show the Planned Hours associated with tasks that are either unassigned or assigned to teams. </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<ul>
<li>Although you cannot see information about task allocations in the Resource Planner in the Project and Role views, the amount of Planned Hours comes from the Planned Hours on the tasks in the projects. </li>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks excluding weekends, time-off days, and schedule exceptions.<br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> The following categories of tasks are included in calculating the Planned Hours for each resource:
<ul>
<li> tasks assigned to users in Resource Pools, job roles, or teams on the project<br>If tasks are assigned to teams, their allocation will appear under <strong>No Role</strong> and <strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks. </li>
<li> unassigned tasks </li>
</ul></li>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>tasks assigned to users with no Resource Pools</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> </td>
</tr>
<tr>
<td rowspan="4"> BDG <br>(BudgetedHours, FTE, or Cost) </td>
<td>Project</td>
<td> <p>A manual entry to estimate how many hours, FTE, or Cost you budget for a project, for a selected time frame. </p> <p>In the Project view, the hours you budget for the project are distributed to the job roles listed under the project. The amount of Planned Hours for each role determines how the Budgeted Hours are distributed to the roles. The Budgeted Hours are distributed to the roles with higher Planned Hours values. </p> <p>In the Role view, the hours you budget for the project are not distributed to the roles or the users on the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>A manual entry to estimate how many hours you budget for a role, for a selected time frame. </p> <p>If no user is associated with the job role, you cannot estimate the Budgeted Hours for the job role. </p> <p>In the Role view, the hours you budget for the role are distributed to the projects listed under the role. The amount of Planned Hours for each project determines how the Budgeted Hours are distributed to the projects. The Budgeted Hours are distributed to the projects with higher Planned Hours values.</p> <p>In the Project view, the hours you budget for the role are not distributed to the projects or the users associated with the role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>A manual entry to estimate how many hours you budget for a user, for a selected time frame. </p> <p> <note type="note">  You can estimate the Budgeted Hours for users who are not assigned to tasks, but are associated with a Resource Pool on a project because these users also appear in the Resource Planner. Their Planned Hours should be zero, however, if they are not assigned to tasks.
</note> </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when working with Budgeted Hours:</p> <li>
<ul>
<li> <p>You can budget resources only when you have Edit access to Resource Management and Financial Data and Manage Finance permissions on the projects.</p> <p>For information about the access needed for budgeting resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this bullet: Duplicated below)</p>
</li>
</ul> </li>
<ul>
<li>By default, the Budgeted Hours in the Resource Planner are zero for all resources and for all the projects.</li>
<li>You can manually estimate the Budgeted Hours for users and roles, or you can use one of the links in the Project or Job Role <strong>More</strong> menus to update them according to the number of Planned Hours.<br>For more information about project and role options, see the section <a href="#Budget" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a> in this article.</li>
<li> The smallest period of time you can budget hours, FTE, or Cost for is a week. You cannot budget hours, FTE, or Cost for a day. </li>
<li> Budgeted Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time. <br>Workfront takes into account the schedule of the user or of the project when distributing Budgeted Hours to users or projects. In this case, Budgeted Hours are equally distributed to each day within the Duration of tasks excluding weekends, but including time-off and schedule exceptions. <br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks, the number of Budgeted Hours per week depends on how many days within that week are part of the task Duration. Weekend days are excluded from this distribution. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters. </li>
<li>You can report on Budgeted Hours, by selecting Budgeted Hour as your report object for a new report.<br>For information about what objects you can report on in Workfront, see the section "Report on objects" in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. <br>For information about building a Budgeted Hour report, see the article <a href="../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Budgeted Hour</a>.</li>
<li>Hours previously budgeted for users who were later deactivated do not display. <br></li>
</ul> </td>
</tr>
<tr>
<td rowspan="4">VAR <br>(Hour, FTE, or ,Cost Variance)</td>
<td>Project</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the project to accomplish all the Planned Hours for the project. </p> <p>The Project Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours, FTE, or Cost for the role to accomplish the Planned Hours assigned to it. </p> <p>The Role Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Hours, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the user to accomplish the Planned Hours assigned to them. </p> <p>The User Hours, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
When the Hours, FTE, or Cost Variance displays in red, you have estimated less Budgeted Hours than the Planned Hours of the actual work that needs to be completed. In this case, the Budgeted Hours might not be enough to complete the work.
</note> </td>
</tr>
<tr>
<td rowspan="4"> NET <br>(Net Hours, FTEs, or Cost) </td>
<td>Project</td>
<td>
<div>
<p>The project Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the project:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the project, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>Role</td>
<td>
<div>
<p>The role Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the role:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the role, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span class="preview"><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>User</td>
<td>
<div>
<p>The user Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the user:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the user, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
<span>When the NET Hours,&nbsp;FTE, or Cost display in red, there is not enough Available time or budget to cover either the Budgeted</span> or the Planned time or cost associated with the work. In this case, the resources are overallocated.
</note> </td>
</tr>
</tbody>
</table>
-->
