---
title: Sostituzione di strumenti basati su Flash in Adobe Workfront
description: Sostituzione di strumenti basati su Flash in Adobe Workfront
author: Luke
draft: Probably
feature: Product Announcements
exl-id: a0ca824d-aab8-4da2-97ed-0913a7f76d55
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '2705'
ht-degree: 1%

---

# Sostituzione di strumenti basati su Flash in Adobe Workfront

Abbiamo rimosso tutti gli strumenti basati su Flash da Adobe Workfront Classic.

Gli strumenti di sostituzione basati sugli standard correnti sono ora disponibili in Workfront. Queste modifiche sono in linea con la fine del supporto per i prodotti di Flash, come annunciato da Adobe.

## Date importanti

Le date seguenti sono importanti per il processo di rimozione di tutti gli strumenti basati su Flash in Workfront:

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>July 1, 2020</strong>: All Flash-based tools will be removed from all Workfront products for those customers who are not using them currently. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">All customers who are currently using the Flash-based tools will continue to have access after this date. If you are still using these products, report all blocking issues or concerns that you see which prevent you from fully transitioning all your users to the new replacement tools by this date. Work with your account manager or our support team to report these concerns. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about contacting our support team, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>. </p>
  -->

* **19 novembre 2020**: Tutti gli strumenti basati su Flash sono stati rimossi da tutti i prodotti Workfront.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  We recommend that you start using the new tools and retire the Flash tools before then, to increase the security of your instance. We will also gradually disable the tools that have not been used for at least 3 months. If you would like us to disable the Flash tools before November, you can contact
  <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.
  </MadCap:conditionalText>
  -->

## Strumenti legacy basati su Flash

Gli strumenti elencati nelle sezioni seguenti sono stati rimossi dal sistema Workfront e sostituiti con nuove soluzioni.

Per informazioni sugli strumenti di sostituzione, consulta [Strumenti legacy basati su Flash e loro sostituzioni](#legacy-flash-based-tools-and-their-replacements) in questo articolo.

### Gestione risorse

* La scheda Pianificazione risorse legacy nell&#39;area Persone e tutti gli strumenti contenuti nella scheda, che include quanto segue:

   * Gestore Budget Risorse
   * Pianificazione capacità
   * Stime delle Risorse
   * Tabella delle Risorse\
      Per ulteriori informazioni, consulta [Pianificazione delle risorse in Adobe Workfront](../../../resource-mgmt/resource-planning/resource-planning-overview.md).

* Area Stime risorse legacy nel caso aziendale di un progetto

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  is displayed in view-only mode
  </MadCap:conditionalText>
  -->

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  For more information, see
  <a href="../../../resource-mgmt/resource-mgmt-overview/migrate-resource-estimates-to-budgeting.md" class="MCXref xref">Migrate from Legacy Resource Estimates to Resource Budgeting </a>
  </MadCap:conditionalText>
  -->

   .

* Scheda secondaria Griglia risorse nella scheda Gestione risorse di un progetto
* L&#39;opzione Usa nuova area di programmazione nella scheda secondaria Pianificazione della scheda Gestione risorse di un progetto che rimuove l&#39;area di programmazione precedente o il Generatore di team. In questo caso, la timeline di pianificazione ora viene visualizzata per impostazione predefinita.
* Scheda Allocazione nel profilo utente

### Report

Le seguenti funzioni di reporting e rapporti sono stati rimossi:

* Funzioni di reporting rimosse:

   * Opzione Griglia risorse in un rapporto utente
   * Opzione Gantt legacy in un progetto o in un rapporto attività\
      Per ulteriori informazioni, consulta [Visualizzazione delle informazioni nel diagramma di Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

* Rapporti rimossi:

   * Rapporto Pool di risorse legacy
   * Rapporto Stime risorse

   >[!NOTE]
   >
   >Tutti i campi legacy accessibili tramite i rapporti o tramite l’API (pool di risorse legacy, costo con budget legacy, costo legacy, ore con budget legacy, costo del lavoro con budget legacy, ecc.) vengono visualizzati in vari rapporti, ma non vengono compilati con nuove informazioni.

### Gantt legacy

* Tutte le visualizzazioni Gantt legacy dagli elenchi dei progetti e delle attività, nonché i rapporti e le opzioni di reporting
* Schede secondarie Gantt legacy in Portfoli e programmi
* Scheda secondaria Gantt legacy in un elenco di task modello in un modello, nella visualizzazione Gantt legacy nella scheda Sottoattività di un task modello e in un rapporto task modello

### Verifica

Il visualizzatore di correzione legacy è stato sostituito con il nuovo visualizzatore per correzione web e il visualizzatore per correzione desktop per la maggior parte dei clienti ed è stato rimosso per tutti i clienti a novembre 2020.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">With the 2018.2 release, the Legacy proofing viewer was removed as the default viewer.</p>
-->

Per ulteriori informazioni, consulta le risorse seguenti:

* [Revisione delle bozze nel visualizzatore per correzione web](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proofs-in-wpv.md)
* [Revisione delle bozze nel visualizzatore di correzione desktop](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/review-proofs-in-desktop-proofing-viewer.md)

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-proof/wp-work-proofsfiles/review-proofs-lpv/lpv-removed-2018.md" class="MCXref xref">Legacy proofing viewer removed in 2018.3</a> </li>
  -->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Additional features to be removed</h3>
<ul>
<li>The Legacy Portfolio Optimizer<br>For more information, see <a href="../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md" class="MCXref xref">Portfolio Optimizer overview</a>.<br></li>
<li>The Legacy financial fields in the Business Case of the project and the Portfolio Optimizer</li>
<li>The dialog boxes used when sharing reports, calendars, and documents no longer rely on Flash-based technology</li>
</ul>
</div>
-->

## Strumenti legacy basati su Flash e loro sostituzioni {#legacy-flash-based-tools-and-their-replacements}

Salvo diversa indicazione, tutte le funzioni legacy sono state sostituite da nuove, come illustrato nella tabella seguente.

>[!CAUTION]
>
>Gli strumenti legacy basati sul Flash sono stati rimossi da tutti gli ambienti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Strumenti legacy</strong> </p> </th> 
   <th> <p><strong>Nuovi strumenti</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Gruppi di risorse esistenti</strong> </p> <p>I pool di risorse legacy erano gruppi o raccolte di ruoli di lavoro necessari allo stesso tempo per il completamento di un progetto. I pool di risorse legacy presentavano una serie di carenze:</p> 
    <ul> 
     <li> È possibile associare un utente a un pool di risorse legacy, ma questo è stato utilizzato solo a scopo di reporting. Poiché i pool di risorse legacy funzionavano con entità ruolo di lavoro astratte, non sono state prese in considerazione alcuna delle eccezioni di pianificazione e del tempo di inattività degli utenti, risultando in dati imprecisi sulla disponibilità delle risorse. </li> 
    </ul> 
    <ul> 
     <li>È possibile specificare un solo pool di risorse legacy per progetto, il che ha comportato il supporto di più pool di risorse legacy solo per il flusso di gruppi separati che operano indipendentemente l’uno dall’altro e non condividono mai le risorse. In tutti gli altri casi, è stato consigliato di mantenere un pool di risorse legacy che includeva tutte le risorse nel sistema, il che ha causato problemi di prestazioni con grandi quantità di progetti e dati.</li> 
    </ul> </td> 
   <td> <p><strong>Gruppo di risorse</strong> </p> <p>I nuovi pool di risorse sono una raccolta di utenti necessari allo stesso tempo per il completamento del progetto. Workfront si rende anche conto che ci sono casi in cui gli utenti specializzati devono avere il lavoro assegnato loro separatamente. Per questo motivo, ora è possibile generare il budget degli utenti invece dei ruoli di lavoro. </p> I vantaggi del pool di risorse rispetto ai pool di risorse legacy includono: 
    <ul>
     <li>Poiché i pool di risorse sono basati sugli utenti, il loro tempo di inattività e le eccezioni di pianificazione sono già prese in considerazione per i calcoli di disponibilità dell’utente e del ruolo. Ciò consente di ottenere dati precisi e aggiornati, consentendo decisioni di budget corrette e riducendo al minimo la probabilità di cambiamenti quando il progetto è in volo.</li>
     <li>Poiché ora è disponibile un maggiore controllo sulla disponibilità di risorse e sulla precisione dei dati, Workfront consente di associare più pool di risorse a un progetto. Un utente può anche appartenere a più pool di risorse, nel caso in cui disponga di più competenze che potrebbero essere utilizzate contemporaneamente in più progetti. </li>
    </ul><p>Con tale controllo sui dati, non è più necessario disporre di un pool di risorse che includa tutte le risorse per la distribuzione del budget disponibile. Infatti, non lo consigliamo. Consigliamo invece di diversificare i pool di risorse e di associare solo i pool di risorse pertinenti ai progetti.</p><p> Per ulteriori informazioni sui pool di risorse, consulta <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Panoramica dei pool di risorse </a></p></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Gestore Budget Risorse</strong> </p> <p>È possibile utilizzare Gestione budget risorse per specificare la disponibilità delle risorse dei ruoli di lavoro in più pool di risorse. Tuttavia, a causa delle carenze del pool di risorse legacy, questa funzionalità è stata utilizzata raramente. Quando è stato utilizzato, ha costretto gli utenti a inserire manualmente la disponibilità dei ruoli di lavoro per rendere il budget più preciso. Non sono state prese in considerazione le eccezioni di pianificazione e il tempo di inattività degli utenti.</p> </td> 
   <td> <p>Con il calcolo automatico della disponibilità basato sugli utenti nei pool di risorse, Gestione budget risorse non è più necessario. Lo strumento è stato eliminato, insieme a tutto il lavoro manuale per il calcolo della disponibilità.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Stime delle Risorse</strong> </p> <p>La scheda Stime risorse in ciascun pool di risorse legacy ha avuto lo stesso scopo di Gestione budget risorse, solo nel contesto di un pool di risorse legacy. Questo strumento presentava le stesse limitazioni di Gestione budget risorse e dei pool di risorse legacy: dati imprecisi e input manuale della disponibilità. </p> </td> 
   <td> <p>Con il calcolo automatico della disponibilità degli utenti, le stime delle risorse sono diventate obsolete e sono state rimosse.</p> <p>Lo strumento viene eliminato dai pool di risorse legacy e dalle stime delle risorse legacy nel caso aziendale di un progetto. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The Legacy Resource Estimates area on the Business Case of the project remains there in View-only mode at this time. 
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Pianificazione capacità</strong> </p> <p>Il Planner capacità era uno strumento Workfront per l’impostazione del budget delle risorse e la definizione della priorità dei progetti all’interno di un pool di risorse legacy, in base alla disponibilità delle risorse. Data l'incompletezza dei dati provenienti da stime delle risorse e dal responsabile del budget delle risorse che ha fornito le informazioni per il planner della capacità, la priorità del progetto doveva essere controllata due volte in base alla disponibilità degli utenti.</p> <p>L'utilizzo di un singolo pool di risorse legacy che includeva tutti i ruoli di lavoro nel sistema era lo scenario più comune, il che causava problemi di prestazioni con il planner capacità che tentava di caricare un gran numero di progetti.</p> </td> 
   <td> <p><strong>Visualizzazione del progetto del planner risorse</strong> </p> <p>Nella visualizzazione basata su progetto del Planner risorse è possibile assegnare un budget alle risorse e assegnare priorità ai progetti in modo simile a come lo si faceva in Pianificazione capacità legacy. A differenza dello strumento legacy, ora sono supportati più dati, con informazioni più precise tenendo conto sia del tempo di inattività degli utenti che delle eccezioni di pianificazione.</p> <p>Le informazioni disponibili, pianificate e a budget sono visibili immediatamente, in modo che i responsabili delle risorse possano vedere se ci sono abbastanza persone per eseguire il lavoro e se i piani del progetto superano le stime di budget iniziali.</p> <p> Per informazioni sull'utilizzo della visualizzazione Progetto nel planner risorse, vedere <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Panoramica di Resource Planner</a></p> <p><strong>La pianificazione dello scenario</strong> </p> <p>Per la pianificazione della capacità a lungo termine, la modellazione e la definizione delle priorità degli scenari, è stato inoltre introdotto lo Scenario Planner di Workfront . </p> <p>Il planner scenario è disponibile solo nella nuova esperienza Adobe Workfront e richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, vedi <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Panoramica di Scenario Planner</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Stime risorsa legacy (caso aziendale)</strong> </p> <p>È possibile utilizzare l'area Stime risorse legacy del Business Case per eseguire il budget di una certa quantità di ore e costi di manodopera nell'ambito della pianificazione del progetto e della richiesta di risorse. Questa visualizzazione non ha fornito alcuna visibilità sulla disponibilità delle risorse, dando luogo a richieste approssimative di risorse e a una maggiore possibilità di lavoro rifiutato per il progetto.</p> </td> 
   <td> <p><strong>Budget risorse (Business Case)</strong> </p> <p>La sezione Resource Budgeting nel caso aziendale include le funzionalità Resource Planner nel caso Business, fornendo visibilità sulla disponibilità di utenti e ruoli e sulla capacità di eseguire il budget a livello di utente. </p> <p> Per informazioni sull'area Resource Budgeting del Business Case, vedere <a href="../../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">Panoramica delle aree del Business Case</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Rapporti sulla stima delle risorse</strong> </p> <p>Quando si utilizzano gli strumenti legacy per la gestione delle risorse, è possibile creare rapporti sulle ore previste e previste dal Business Case. Ciò consente di creare rapporti a matrice che mostrano il lavoro totale previsto e pianificato per ogni ruolo di lavoro in un intervallo di tempo specifico. Questo rapporto non è stato modificabile e non è stato possibile apportare alcuna modifica al budget delle risorse in base ai risultati del rapporto. </p> </td> 
   <td> <p><strong>Rapporto sull'utilizzo</strong> </p> <p>Il rapporto Utilizzazione integrato visualizza le ore, i costi e i ricavi pianificati, preventivati e effettivi affiancati. </p> <p>Per informazioni sull'utilizzo del rapporto Utilizzo, vedere <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Visualizza informazioni sull’utilizzo delle risorse </a>. </p> 
    <div> 
     <p><strong>Ore di budget segnalabili</strong> </p> 
     <p>Creare un report per le ore previste per esaminare le ore previste nel budget nel Planner risorse in un modulo di report. </p> 
     <p>Per informazioni sull'orario previsto, vedi <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glossario della terminologia di Adobe Workfront</a>.</p> 
     <p>Per informazioni sulla creazione di un rapporto, vedi <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un rapporto personalizzato</a>.</p> 
    </div> <p><strong>Visualizzazione del ruolo del planner risorse</strong> </p> <p>Le ore pianificate e in budget dal caso Business negli strumenti di gestione delle risorse legacy sono ora disponibili in una nuova vista nativa, la vista basata sul ruolo del Planner risorse. Questa visualizzazione fornisce immediatamente informazioni su Orari disponibili, Pianificati e Preventivi e consente di controllare e modificare il budget nella stessa posizione. Ciò garantisce un migliore processo decisionale durante la pianificazione dei ruoli di lavoro ad alto livello. </p> <p> Per informazioni sulle risorse di budget nella Vista ruolo del planner risorse, vedere la <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using2" class="MCXref xref">Utilizzare le visualizzazioni Progetto e Ruolo per preventivare le risorse </a> sezione <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Panoramica di Resource Planner</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Tabella delle Risorse</strong> </p> <p>La griglia delle risorse ti ha dato visibilità sull’allocazione di utenti specifici mentre un progetto progredisce verso il completamento. </p> <p>Ad esempio, è possibile vedere facilmente quando un membro del team di progetto ha lavorato in anticipo e quando un utente è rimasto indietro, nonché se è stato allocato o non assegnato per un intervallo di tempo specifico. </p> <p>Purtroppo non è stato possibile agire sulla base delle informazioni nella stessa visualizzazione. Per risolvere i problemi di sovrallocazione è stato necessario passare ai progetti e regolare manualmente le informazioni senza alcuna visibilità sul risultato delle azioni.</p> </td> 
   <td> <p>La griglia delle risorse è stata sostituita da due nuovi strumenti. Puoi utilizzare i seguenti strumenti, a seconda della fase di pianificazione delle risorse in cui ti trovi:</p> 
    <ul> 
     <li> <p><strong>Per la fase analitica:</strong> </p> 
      <ul> 
       <li> <p><strong>Il servizio di bilanciamento del carico di lavoro</strong>: Utilizza il servizio di bilanciamento del carico di lavoro per visualizzare il carico di lavoro degli utenti a un livello più granulare. Quando si utilizza il servizio di bilanciamento del carico di lavoro, è possibile visualizzare gli utenti disponibili nel carico di lavoro per completare l'attività in tempo. Questo include i dettagli delle eccezioni di orario e pianificazione. </p> <p>Per informazioni sul bilanciamento del carico di lavoro, vedi <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Panoramica del servizio di bilanciamento del carico di lavoro</a>.</p> </li> 
       <li> <p><strong>Visualizzazione utente del planner risorse</strong><strong>:</strong> Quando si tenta di comprendere a un livello più alto a quali progetti sono assegnati gli utenti, utilizzare la visualizzazione utente del planner risorse. Questo ti consente di vedere su cosa stanno lavorando gli utenti e la loro sovrallocazione e sottoallocazione per un intervallo di tempo specifico. Il Resource Planner fornisce anche la visualizzazione dell’allocazione complessiva degli utenti nel suo complesso, nonché la visibilità nelle ore effettive registrate, utile per analizzare l’avanzamento del lavoro svolto. </p> <p>Per informazioni sull'utilizzo della visualizzazione utente nel planner risorse, vedere la <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using" class="MCXref xref">Utilizza la visualizzazione utente per visualizzare le ore disponibili, pianificate e effettive o FTE </a> sezione <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Panoramica di Resource Planner</a></p> </li> 
      </ul> </li> 
     <li><strong>Per la fase tattica:</strong> 
      <ul> 
       <li><strong>Il servizio di bilanciamento del carico di lavoro</strong> Utilizzando il servizio di bilanciamento del carico di lavoro puoi effettuare le seguenti operazioni: 
        <ul>
         <li>Assegna il lavoro agli utenti.</li>
         <li>Gestisci le allocazioni degli utenti per gli elementi di lavoro. </li>
         <li>Condividi il servizio di bilanciamento del carico di lavoro con altri utenti che potrebbero non avere visibilità nell’area Persone. Utilizza la funzionalità di collegamento condivisibile per condividere un collegamento al servizio di bilanciamento del carico di lavoro e incorporarlo nei dashboard personalizzati. Tutti gli utenti con accesso a Visualizza utenti possono visualizzare queste dashboard quando le condividi.</li>
        </ul><p>Il servizio di bilanciamento del carico di lavoro è disponibile nell’area Persone. </p><p>Per informazioni sul bilanciamento del carico di lavoro, vedi <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Panoramica del servizio di bilanciamento del carico di lavoro</a>.</p></li> 
      </ul> <!--
       <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
        <li><strong>The Resource Scheduling Areas</strong><strong>:</strong> When assigning your resources to the actual work that must be completed, use the Resource Scheduling areas in the People or Team areas, or at the project level. These areas allow you to visualize and manage the users' workload by day and rectify any problems from one view using the following actions: 
         <ul>
          <li> manual dragging and dropping of tasks to the correct assignee </li>
          <li> automatic assigning of tasks </li>
          <li> bulk swapping assignments </li>
          <li><p>adjusting Planned Hours according to the true availability of users. </p></li>
         </ul><p>These actions provide even more control over managing workload. </p><p> For information about managing user assignments and allocations in the Resource Scheduling areas, see <a href="../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md" class="MCXref xref">Get started with Resource Scheduling</a>.</p><p>With this new functionality, the Resource Grid is replaced by the User View of the Resource Planner and the Resource Scheduling areas in the following areas of the application: </p>
         <ul>
          <li>People - the Resource Grid is eliminated along with the Legacy Resource Planning tab.</li>
          <li>Project - the Scheduling area under the Staffing tab of the project is available to Work and Plan license users. They do not have to have Manage access to the project to view this area. </li>
          <li>Reporting - the ability to view User reports in the Resource Grid view is removed. Instead, there is an option to share a URL for the User View of the Resource Planner and embed it in custom dashboards, providing visibility into user utilization to virtually anyone in the system. Any users with access to View users are able to view these dashboards when you share them. </li>
          <li>User - the Allocation tab is eliminated as the same information can be accessed in the User View of the Resource Planner.</li>
         </ul></li> 
       </ul>
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Diagramma di Gantt legacy, Elenco attività</strong> </p> <p> Il diagramma di Gantt legacy nell’elenco delle attività consente agli utenti di visualizzare visivamente la cronologia del progetto ed eseguire una pianificazione dello scenario What-if senza apportare modifiche al database. Il diagramma di Gantt legacy era basato sulla tecnologia di Flash, che presentava rischi per la sicurezza. </p> </td> 
   <td> <p><strong>Diagramma di Gantt,</strong> <strong>Elenco attività</strong></p> <p> Il nuovo Diagramma di Gantt basato su HTML ha lo stesso scopo del Gantt legacy. Gli utenti possono visualizzare la timeline del progetto ed eseguire la pianificazione dello scenario What-if senza apportare modifiche al database modificando l’opzione Salva manuale nella barra degli strumenti dell’elenco delle attività. </p> <p>Il nuovo Diagramma di Gantt è interattivo quando si utilizza l'opzione Salvataggio automatico che è possibile utilizzare quando si desidera salvare automaticamente le modifiche man mano che si verificano. </p> <p>Il nuovo Diagramma di Gantt elenco task è basato sulla tecnologia più recente ed è affidabile. Questo nuovo diagramma di Gantt si trova direttamente nell'elenco delle attività ed è facilmente accessibile quando si lavora sull'elenco delle attività senza cambiare scheda o cambiare visualizzazione. </p> <p>Anche se il nuovo diagramma di Gantt offre le stesse funzionalità del grafico precedente, esistono alcune differenze nelle funzioni rispetto al Gantt legacy. </p> <p> La sottoscheda Gantt legacy in un elenco di attività modello in un modello, la visualizzazione Gantt legacy nella scheda Sottoattività di un task modello e il diagramma di Gantt legacy in un rapporto task modello sono stati sostituiti anche con il diagramma di Gantt basato su HTML. </p> <p>Se si utilizza il Diagramma di Gantt legacy principalmente per la visualizzazione semplice e per le modifiche rapide e non si utilizza il grafico effettivo, la nuova opzione Pianificazione timeline consente di apportare modifiche rapide ai campi di pianificazione chiave. È possibile selezionare Pianificazione timeline invece di Salvataggio automatico dalla barra degli strumenti dell'elenco delle attività.</p> <p>Per ulteriori informazioni sul salvataggio di un elenco di task utilizzando l'opzione Pianificazione timeline, vedere la sezione "Salvare manualmente le modifiche in un elenco di task quando si seleziona l'opzione Pianificazione timeline" nell'articolo <a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Modificare le attività in un elenco</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Diagramma di Gantt legacy per un elenco di progetti</strong> </p> <p>Il diagramma di Gantt legacy nell’elenco dei progetti consente agli utenti di visualizzare i progetti e le relative attività in un’unica visualizzazione. Senza uscire dall’elenco dei progetti, gli utenti potevano visualizzare i dettagli relativi alle attività di un progetto e alle dipendenze tra i progetti. Il diagramma di Gantt legacy nell’elenco dei progetti si basa sulla tecnologia dei Flash, che presentava rischi per la sicurezza. </p> </td> 
   <td> <p><strong>Diagramma di Gantt, Elenco progetti</strong> </p> <p>Il diagramma di Gantt basato su HTML ha lo stesso scopo del diagramma di Gantt legacy. Gli utenti possono visualizzare i progetti e le loro attività in un’unica visualizzazione per identificare visivamente le dipendenze tra progetti e attività. Il diagramma di Gantt Elenco progetti si trova direttamente nell’elenco dei progetti. Il nuovo diagramma di Gantt è dotato di un'interfaccia moderna e si basa sulla tecnologia più recente.</p> <p>Per informazioni sull'elenco dei progetti Diagramma di Gantt, vedere <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Visualizzazione delle informazioni nel diagramma di Gantt </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Condivisione di finestre di dialogo per report, calendari e documenti</strong> </p> <p>Quando si condividono rapporti, calendari e documenti, le finestre di dialogo utilizzate si basavano sulla tecnologia di Flash.</p> </td> 
   <td> <p>L’esperienza durante la condivisione di rapporti, calendari e documenti in Workfront non è cambiata. Tuttavia, l’esperienza non si basa più sul Flash.</p> <p>Per ulteriori informazioni sulla condivisione di questi elementi, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Panoramica della condivisione delle autorizzazioni sugli oggetti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Visualizzatore di correzione legacy</strong> </p> <p>Il visualizzatore di correzione legacy era un visualizzatore di correzione basato su web che forniva funzionalità di correzione per bozze statiche, video e interattive.</p> </td> 
   <td> <p><strong>Visualizzatore per correzione web e visualizzatore per correzione desktop</strong> </p> <p>Il visualizzatore per correzione web fornisce funzionalità di correzione per le bozze statiche e video.</p> <p>Il visualizzatore per correzione desktop fornisce funzionalità di correzione per le bozze interattive, oltre a fornire supporto completo per le bozze statiche e video.</p> <p>Il formato di file SWF non è più supportato da nessuno dei provider principali ed è stato sostituito con banner HTML5 per la correzione. </p> <p>Per informazioni più dettagliate sulle differenze tra i visualizzatori di correzione disponibili, vedi <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Panoramica sulle differenze tra il visualizzatore per correzione web e il visualizzatore per correzione desktop</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
