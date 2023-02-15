---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Panoramica delle informazioni su ore, FTE e costi nelle visualizzazioni Progetto e Ruolo del Planner risorse
description: Panoramica delle informazioni su ore, FTE e costi nelle visualizzazioni Progetto e Ruolo del Planner risorse
author: Alina
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2973'
ht-degree: 0%

---

# Panoramica delle informazioni su ore, FTE e costi nelle visualizzazioni Progetto e Ruolo del Planner risorse

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

La funzione principale di Resource Planner consiste nell’assegnare un budget alle risorse per il lavoro che devono eseguire su un progetto. È possibile visualizzare il tempo disponibile delle risorse e assegnare il relativo tempo ai progetti in cui sono assegnate.

Per informazioni sulle risorse di budget nel Planner risorse, vedere [Risorse di budget nel planner risorse utilizzando le visualizzazioni Progetto e Ruolo](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

Questo articolo descrive alcuni dei concetti chiave che è necessario conoscere prima di iniziare a eseguire il budget delle risorse nel Planner risorse.

## Panoramica sulle risorse di budget

Quando si inseriscono risorse in budget utilizzando il planner risorse, tenere presente quanto segue:

* È possibile allocare le risorse in budget specificando un importo di ore, FTE o Costo che le risorse possono utilizzare per completare il lavoro sui progetti. Quando si esegue il budget di tempo o costo per una risorsa, le ore disponibili, le FTE o il costo per la risorsa diminuiscono dell&#39;importo preventivato. Di conseguenza, gli importi Ore disponibili, FTE o Costo per i progetti che seguono il progetto per il quale si sta preventivando il budget diminuiscono per gli utenti e i ruoli per tali progetti.

   >[!IMPORTANT]
   >
   >È possibile eseguire il budget delle risorse per un periodo di 15 anni. Se si finanziano risorse per un progetto con una durata superiore a 15 anni, le informazioni di budget potrebbero non essere precise.

* È possibile assegnare un budget a Ore, FTE o Costo per le risorse per qualsiasi intervallo di tempo visualizzato nel Planner risorse, indipendentemente dalla timeline del progetto. Ad esempio, se desideri indicare che le risorse potrebbero non essere disponibili durante la cronologia del progetto (dove sono associate all’orario pianificato), ma potrebbero essere disponibili in un altro momento, puoi farlo inserendole nel budget per i frame di tempo in cui l’ora pianificata è zero, se questo è il momento in cui diventano disponibili per il lavoro. Puoi modificare manualmente la timeline del progetto in modo che corrisponda alla disponibilità della risorsa in seguito a questa operazione.

   >[!NOTE]
   >
   >È consigliabile eseguire manualmente il budget di ore, FTE o Costo per i ruoli di lavoro o per gli utenti. È possibile utilizzare le opzioni automatiche per calcolare il tempo di budget per i progetti e le risorse solo se si è certi che la quantità di ore pianificate, FTE o Costo deve sempre corrispondere alle ore previste, FTE o Costo.\
   >Per informazioni sull&#39;utilizzo delle opzioni automatiche per l&#39;impostazione del budget nel Planner risorse, vedere la sezione &quot;Progetto di budget e ruoli automaticamente&quot; nell&#39;articolo [Verifica la disponibilità e l’allocazione delle risorse utilizzando Adobe Workfront Resource Planner](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

* FTE o costi di budget è identico alle ore di budget, dove Adobe Workfront utilizza i valori FTE e di costo invece delle ore per le risorse budget.

   Per ulteriori informazioni su come vengono calcolati i costi nel Planner risorse, vedere [Calcolare i costi nel planner risorse](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

* Le allocazioni a budget per le risorse nel Planner risorse vengono eseguite nei seguenti modi:

   * Manualmente

      Oppure

   * Automaticamente, utilizzando le opzioni del progetto e del ruolo nel **Visualizza per progetto** e **Visualizza per ruolo** visualizzazioni.
   Per ulteriori informazioni, consulta [Risorse di budget nel planner risorse utilizzando le visualizzazioni Progetto e Ruolo](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

* Quando un utente modifica i ruoli di lavoro, viene eliminato, disattivato o rimosso da un pool di risorse, le ore previste nel budget per il ruolo non cambiano e vengono ridistribuite agli utenti rimanenti nel ruolo. Se nessun utente è più associato al ruolo del lavoro, le ore previste per il ruolo diventano zero.

Per ulteriori informazioni sulle opzioni di progetto e ruolo, consulta la sezione . [Comprendere i valori di Ore, FTE e Costo nel Planner risorse](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner) in questo articolo.

## Comprendere i valori di Ore, FTE e Costo nel Planner risorse {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

Prima di includere nel budget le risorse e aggiornare le informazioni sulle ore previste nel Planner risorse, è necessario avere familiarità con i seguenti concetti

* **Ore, FTE o Costo pianificati**: Il lavoro che deve essere svolto come definito su attività e problemi.
* **Ore disponibili, FTE o Costo**: Il tempo a disposizione degli utenti o dei ruoli di lavoro, in base alle pianificazioni associate agli utenti.

Queste informazioni vengono visualizzate nel Planner risorse per ogni risorsa (utente o ruolo) e per ogni progetto.

Per informazioni su ciò che viene visualizzato nelle visualizzazioni Progetto e Ruolo del progetto, consulta l’articolo [Panoramica sulla navigazione in planner risorse](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Per informazioni su come vengono calcolati i costi nel Planner risorse, vedere l&#39;articolo [Calcolare i costi nel planner risorse](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

>[!NOTE]
>
>L&#39;impostazione del budget per costo è identica all&#39;impostazione del budget per ore o FTE, ma è necessario comprendere in che modo Workfront calcola il costo per il planner risorse.
>
>Per informazioni sul calcolo dei costi nel Planner risorse, vedere l&#39;articolo [Calcolare i costi nel planner risorse](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

Le tabelle seguenti mostrano le informazioni di allocazione e disponibilità visualizzate nel Planner risorse quando si applica la visualizzazione Progetto o Ruolo. Puoi visualizzare queste informazioni per ore, FTE o Costo:

* [Colonna AVL (disponibile)](#the-avl-available-column)
* [Colonna PLN (pianificata)](#the-pln-planned-column)
* [Colonna BDG (a budget)](#the-bdg-budgeted-column)
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
   <td> <p>Totale di ore, FTE o Costo per i quali tutti gli utenti del progetto possono lavorare in base alla propria pianificazione, per l’intervallo di tempo selezionato. </p> </td> 
  </tr> 
  <tr> 
   <td>Qual</td> 
   <td> <p>Totale di ore, FTE o Costo per i quali tutti gli utenti associati a questo ruolo sono disponibili per lavorare in base alla loro pianificazione e al loro costo <strong>Percentuale di disponibilità FTE</strong> per quel ruolo specifico, per l'intervallo di tempo selezionato. </p> <p>Considera quanto segue: </p> 
    <ul> 
     <li>Se nessun utente è associato a un ruolo di lavoro, il valore per le ore disponibili per il ruolo di lavoro è zero. </li> 
     <li>Se un utente è associato a un ruolo di lavoro principale, ma la <strong>Percentuale di disponibilità FTE</strong> per il ruolo è 0%, il valore del ruolo Ore disponibili è zero.</li> 
     <li>Se l’utente è associato ad Altri ruoli e al <strong>Percentuale di disponibilità FTE</strong> per i ruoli è pari a 0%, gli altri ruoli non sono elencati nel Planner risorse e l'utente viene visualizzato solo sotto il relativo Ruolo principale.</li> 
    </ul> <p>Per ulteriori informazioni sulla <strong>Percentuale di disponibilità FTE</strong> per un ruolo di lavoro, consulta l’articolo <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente</a>.</p> <p>Per ulteriori informazioni su come viene calcolata la disponibilità del ruolo di lavoro nel Planner risorse, vedere la sezione "Calcolare le ore disponibili e l’ETP per un ruolo di lavoro nel Planner risorse" nell’articolo <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Panoramica del calcolo delle ore e degli FTE per utenti e ruoli nel Planner risorse</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td> <p>Ore, FTE o Costo che l’utente è disponibile per lavorare, in base alla propria pianificazione, per l’intervallo di tempo selezionato. Questo numero sottrae le ore associate ai seguenti elementi:</p> 
    <ul> 
     <li>eccezioni di programmazione</li> 
     <li>tempo di inattività dell'utente</li> 
     <li>ore previste per altri progetti. </li> 
    </ul> <p>Le ore disponibili, le FTE o il costo di un cambiamento utente in base alle seguenti modalità: </p> 
    <ul> 
     <li>come vengono calcolati la pianificazione e l’ETP in base alle preferenze di gestione delle risorse a livello di sistema.<br><p>Per ulteriori informazioni sul calcolo della disponibilità dei ruoli di lavoro e utente, consulta l’articolo <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Panoramica del calcolo delle ore e degli FTE per utenti e ruoli nel Planner risorse</a>.</p>
     Per ulteriori informazioni sulla configurazione delle preferenze di gestione delle risorse in Workfront, consulta <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurare le preferenze di Gestione risorse</a></li> 
    </ul> 
    <ul> 
     <li>la <strong>Priorità di pianificazione del progetto</strong>, se l’utente è iscritto in budget per il lavoro.<br>Per ulteriori informazioni sull'effetto della priorità di pianificazione del progetto sulle ore disponibili di un utente, vedere <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Panoramica sulla navigazione in planner risorse </a>. </li> 
    </ul> <p>Se l’utente è pianificato per la disattivazione, le ore disponibili, le FTE o il costo per i giorni successivi alla data di disattivazione sono pari a zero. <br>Per ulteriori informazioni sulla disattivazione degli utenti, consulta l’articolo <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Disattivare o riattivare un utente</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Colonna PLN (pianificata) {#the-pln-planned-column}

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
   <td> <p>Totale delle ore pianificate, delle FTE o del costo per tutti i ruoli di lavoro o gli utenti elencati nel progetto, incluso nel <strong>Nessun ruolo</strong> o <strong>Nessun utente</strong> sezioni, per l’intervallo di tempo selezionato e come visualizzato nella scheda Dettagli progetto del progetto. </p> <p><b>NOTA</b>

Gli aggiustamenti manuali delle allocazioni giornaliere degli utenti possono modificare il valore settimanale, mensile o trimestrale dell&#39;orario pianificato nel Planner risorse. È possibile regolare manualmente le allocazioni giornaliere degli utenti per le attività e i problemi utilizzando il servizio di bilanciamento del carico di lavoro. Per ulteriori informazioni, consulta <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gestire le allocazioni di utenti nel load balancer</a>.</p> </td>
</tr> 
  <tr> 
   <td>Qual</td> 
   <td> <p>Totale delle ore pianificate di tutte le attività assegnate al ruolo, durante l'intervallo di tempo selezionato. </p> <p>La <strong>Nessun ruolo</strong> La sezione mostra le ore pianificate associate alle attività non assegnate, assegnate ai team (le cui ore sono elencate nella <strong>Nessun utente</strong> (sezione) o assegnato a utenti che non sono associati a un ruolo di lavoro. </p> </td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td> <p>Orario pianificato per tutte le attività assegnate all’utente in un ruolo specifico, durante l’intervallo di tempo selezionato. </p> <p>La <strong>Nessun utente</strong> Viene visualizzata la sezione Orari pianificati associata alle attività non assegnate o assegnate ai team. </p> </td> 
  </tr> 
 </tbody> 
</table>

Quando si visualizzano le ore pianificate, tenere presente quanto segue:

* Sebbene non sia possibile visualizzare informazioni sulle allocazioni di attività nel Planner risorse nelle visualizzazioni Progetto e Ruolo, la quantità di ore pianificate proviene dalle ore pianificate sulle attività nei progetti.
* Le ore pianificate vengono distribuite in modo uniforme a ogni giorno entro la durata delle attività, per ogni risorsa assegnata loro. La durata dell&#39;attività si basa sulle date di inizio e di completamento pianificate e include ogni giorno di calendario entro tale periodo di tempo.\
   Workfront tiene conto della pianificazione dell’utente o del progetto quando distribuisce gli orari pianificati a utenti o progetti. In questo caso, le ore pianificate vengono distribuite in modo uniforme a ogni giorno entro la durata delle attività, esclusi i fine settimana, i giorni di timeout e le eccezioni di pianificazione.\
   Se, ad esempio, si visualizza il Planner risorse per settimana e si dispone di attività che si estendono per più settimane sui progetti, il numero di ore pianificate per settimana dipende dal numero di giorni all&#39;interno di tale settimana che fanno parte dell&#39;attività Durata. Questo funziona in modo simile quando si visualizza il Planner risorse per mese o trimestre e quando le attività si estendono su più mesi o trimestri.\
   I giorni di fine settimana, le eccezioni di pianificazione e i giorni di timeout sono esclusi da questa distribuzione.
* Le seguenti categorie di attività sono incluse nel calcolo delle ore pianificate per ogni risorsa:

   * attività assegnate agli utenti in pool di risorse, ruoli o team del progetto\
      Se le attività vengono assegnate ai team, la relativa allocazione verrà visualizzata in **Nessun ruolo** e **Nessun utente** sezioni. È possibile visualizzare le ore pianificate associate ai team, ma non è possibile eseguire il budget delle ore, perché non sono associati ruoli e utenti alle attività.

   * attività non assegnate

* Le ore pianificate nel planner risorse non includono le ore pianificate associate ai seguenti elementi:

   * attività principali
   * attività assegnate a utenti senza pool di risorse
   * quando **Includi ore da problemi** è disabilitata.

* Le ore pianificate non vengono visualizzate nel planner risorse se la durata dell&#39;attività è pari a zero.
* Le ore pianificate associate agli utenti disattivati non vengono visualizzate.

### Colonna BDG (a budget) {#the-bdg-budgeted-column}

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
   <td> <p>Inserimento manuale per stimare il numero di ore, FTE o Costo preventivati per un progetto per un intervallo di tempo selezionato. </p> <p>Nella vista Progetto, le ore di budget del progetto vengono distribuite ai ruoli di lavoro elencati nel progetto. La quantità di ore pianificate per ogni ruolo determina la distribuzione delle ore previste nei ruoli. Le ore previste vengono distribuite ai ruoli con valori orari pianificati più elevati. </p> <p>Nella vista Ruolo , le ore di budget per il progetto non vengono distribuite ai ruoli o agli utenti del progetto. </p> </td> 
  </tr> 
  <tr> 
   <td>Qual</td> 
   <td> <p>Una voce manuale per stimare quante ore budget si prevede per un ruolo, per un intervallo di tempo selezionato. </p> <p>Se nessun utente è associato al ruolo del lavoro, non è possibile stimare gli orari previsti per il ruolo del lavoro. </p> <p>Nella vista Ruolo , le ore di budget per il ruolo vengono distribuite ai progetti elencati sotto il ruolo . La quantità di ore pianificate per ogni progetto determina la distribuzione delle ore previste nei progetti. Le ore previste vengono distribuite ai progetti con valori orari pianificati più elevati.</p> <p>Nella vista Progetto, le ore di budget per il ruolo non vengono distribuite ai progetti o agli utenti associati al ruolo. </p> </td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td> <p>Una voce manuale per stimare quante ore budget si prevede per un utente per un intervallo di tempo selezionato. </p> <p> <p><b>NOTA</b>   È possibile stimare gli orari previsti per gli utenti che non sono assegnati alle attività, ma sono associati a un pool di risorse in un progetto, perché questi utenti vengono visualizzati anche nel Planner risorse. Tuttavia, se non sono assegnati a attività, l’orario pianificato deve essere zero. </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Quando si lavora con le ore a budget, tenere presente quanto segue:

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(Duplicated below ??)
</MadCap:conditionalText>
-->

* È possibile assegnare il budget alle risorse solo quando si dispone dell&#39;accesso Modifica alle autorizzazioni Gestione risorse e Dati finanziari e Gestione finanziaria per i progetti.

   Per informazioni sull&#39;accesso necessario per le risorse di budget, consulta l&#39;articolo [Accesso necessario alle risorse di budget in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Per impostazione predefinita, le ore previste nel Planner risorse sono pari a zero per tutte le risorse e per tutti i progetti.
* È possibile stimare manualmente le ore previste per utenti e ruoli oppure utilizzare uno dei collegamenti nel ruolo Progetto o Processo **Altro** menu per aggiornarli in base al numero di ore pianificate.\
   Per ulteriori informazioni sulle opzioni di progetto e ruolo, consulta la sezione . [Panoramica delle informazioni su ore, FTE e costi nelle visualizzazioni Progetto e Ruolo del Planner risorse](#Budget) in questo articolo.

* Il periodo di tempo più piccolo per il quale è possibile eseguire il budget di ore, FTE o Costo è una settimana. Non è possibile impostare il budget per ore, FTE o Costo per un giorno.
* Le ore previste vengono distribuite in modo uniforme a ogni giorno entro la durata delle attività, per ogni risorsa assegnata. La durata dell&#39;attività si basa sulle date di inizio e di completamento pianificate e include ogni giorno di calendario entro tale periodo di tempo.\
   Workfront prende in considerazione la pianificazione dell’utente o del progetto quando distribuisce gli orari a budget a utenti o progetti. In questo caso, le ore previste in budget vengono distribuite in modo uniforme a ogni giorno entro la durata delle attività, esclusi i fine settimana, ma includendo le eccezioni di orario e di programmazione.\
   Se, ad esempio, si visualizza il Planner risorse per settimana e si dispone di attività che si estendono su più settimane, il numero di ore previste per settimana dipende dal numero di giorni all&#39;interno di tale settimana che fanno parte dell&#39;attività Durata. I giorni di fine settimana sono esclusi da questa distribuzione. Questo funziona in modo simile quando si visualizza il Planner risorse per mese o trimestre e quando le attività si estendono su più mesi o trimestri.

* È possibile creare rapporti sulle ore previste, selezionando Ora a budget come oggetto di rapporto per un nuovo rapporto.\
   Per informazioni sugli oggetti su cui è possibile creare rapporti in Workfront, consulta la sezione &quot;Rapporto sugli oggetti&quot; nell’articolo [Comprendere gli oggetti in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
   Per informazioni sulla creazione di un rapporto sull&#39;ora a budget, consulta l&#39;articolo [Rapporto: Ora budget](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

* Le ore in precedenza preventivate per gli utenti successivamente disattivati non vengono visualizzate.

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
   <td> <p>L’ora, l’FTE o la varianza dei costi indica se il progetto dispone di ore a budget sufficienti per completare tutte le ore pianificate per il progetto. </p> <p>L'ora, l'FTE o lo scostamento del costo del progetto viene calcolato con la seguente formula:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Qual</td> 
   <td> <p>L'ora, l'FTE o lo scostamento dei costi mostra se il ruolo ha un numero sufficiente di ore a budget, FTE o Costo per completare le ore pianificate assegnate. </p> <p>L’ora del ruolo, l’FTE o l’varianza dei costi viene calcolata utilizzando la seguente formula:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Utente</td> 
   <td> <p>L'ora, l'FTE o la varianza dei costi mostra se l'utente dispone di un numero sufficiente di ore a budget per completare le ore pianificate assegnate. </p> <p>La formula Ore utente, FTE o Varianza costo viene calcolata utilizzando la seguente formula:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Quando le ore, le FTE o le Varianze di costo vengono visualizzate in rosso, è stato stimato un numero inferiore di ore previste rispetto alle ore previste del lavoro effettivo che deve essere completato. In questo caso, le ore previste potrebbero non essere sufficienti per completare il lavoro.

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
     <p>Il progetto Orari netti, FTE o Costo può mostrare uno dei seguenti elementi: </p> 
     <ul> 
      <li> <p>Differenza tra il tempo o il costo disponibili e il tempo o il costo preventivati per il progetto:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>La differenza tra l'ora o il costo disponibili e l'ora o il costo pianificati per il progetto, quando i valori Use Planned (PLN) nell'impostazione di calcolo NET sono abilitati: </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>SUGGERIMENTO</b></p>        
  <p>Questa opzione viene applicata solo quando si personalizza la visualizzazione nella sezione Visualizza elementi selezionati .</p>
  <p>Per ulteriori informazioni, consulta <a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >Verifica la disponibilità e l’allocazione delle risorse utilizzando Adobe Workfront Resource Planner</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>Qual</td> 
   <td> 
    <div> 
     <p>Il ruolo Orari netti, FTE o Costo può mostrare uno dei seguenti elementi: </p> 
     <ul> 
      <li> <p>La differenza tra il tempo o il costo disponibili e il tempo o il costo preventivati per il ruolo:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>La differenza tra l'ora o il costo disponibili e l'ora o il costo pianificati per il ruolo, quando i valori Use Planned (PLN) nell'impostazione di calcolo NET sono abilitati:</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>SUGGERIMENTO</b> <span>

Questa opzione viene applicata solo quando si personalizza la visualizzazione nella sezione Visualizza elementi selezionati .</span> </p> <p><span>Per ulteriori informazioni, consulta </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Verifica la disponibilità e l’allocazione delle risorse utilizzando Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>Utente</td> 
   <td> 
    <div> 
     <p>L'utente Orari netti, FTE o Costo può mostrare una delle seguenti opzioni: </p> 
     <ul> 
      <li> <p>La differenza tra il tempo o il costo disponibili e il tempo o il costo preventivati per l'utente:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>La differenza tra l'ora o il costo disponibili e l'ora o il costo pianificati per l'utente quando i valori Use Planned (PLN) nell'impostazione di calcolo NET sono abilitati:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>SUGGERIMENTO</b> <span>

Questa opzione viene applicata solo quando si personalizza la visualizzazione nella sezione Visualizza elementi selezionati .</span> </p> <p><span>Per ulteriori informazioni, consulta </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Verifica la disponibilità e l’allocazione delle risorse utilizzando Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Quando le ore, gli FTE o i costi NETTI vengono visualizzati in rosso, il tempo o il budget disponibili non sono sufficienti per coprire il budget** o l&#39;orario o il costo pianificati associati all&#39;opera. In questo caso, le risorse sono sovrassegnate.

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
