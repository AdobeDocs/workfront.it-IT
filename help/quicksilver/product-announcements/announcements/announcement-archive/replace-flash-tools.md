---
title: Sostituzione degli strumenti basati su Flash in Adobe Workfront
description: Sostituzione degli strumenti basati su Flash in Adobe Workfront
author: Luke
draft: Probably
feature: Product Announcements
exl-id: a0ca824d-aab8-4da2-97ed-0913a7f76d55
source-git-commit: c80d9b0b7eb2a638af9e0a11ca3038ed99ecf1ee
workflow-type: tm+mt
source-wordcount: '2701'
ht-degree: 0%

---

# Sostituzione degli strumenti basati su Flash in Adobe Workfront

Abbiamo rimosso tutti gli strumenti basati su Flash da Adobe Workfront Classic.

Gli strumenti di sostituzione basati sugli standard attuali sono ora disponibili in Workfront. Queste modifiche sono in linea con la fine del supporto per i prodotti di Flash, come annunciato da Adobe.

## Date importanti

Le seguenti date sono importanti per il processo di rimozione di tutti gli strumenti basati sul Flash in Workfront:

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>July 1, 2020</strong>: All Flash-based tools will be removed from all Workfront products for those customers who are not using them currently. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">All customers who are currently using the Flash-based tools will continue to have access after this date. If you are still using these products, report all blocking issues or concerns that you see which prevent you from fully transitioning all your users to the new replacement tools by this date. Work with your account manager or our support team to report these concerns. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about contacting our support team, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>. </p>
  -->

* **19 novembre 2020**: tutti gli strumenti basati su Flash sono stati rimossi da tutti i prodotti Workfront.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  We recommend that you start using the new tools and retire the Flash tools before then, to increase the security of your instance. We will also gradually disable the tools that have not been used for at least 3 months. If you would like us to disable the Flash tools before November, you can contact
  <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.
  </MadCap:conditionalText>
  -->

## Strumenti basati su Flash legacy

Gli strumenti elencati nelle sezioni seguenti sono stati rimossi dal sistema Workfront e sostituiti con nuove soluzioni.

Per informazioni sugli strumenti di sostituzione, vedere [Strumenti basati su Flash legacy e loro sostituti](#legacy-flash-based-tools-and-their-replacements) in questo articolo.

### Gestione risorse

* La scheda Pianificazione risorse legacy nell&#39;area Persone e tutti gli strumenti contenuti nella scheda, che include quanto segue:

   * Gestore Budget Risorse
   * Pianificazione capacità
   * Stime delle Risorse
   * Tabella delle Risorse\
     Per ulteriori informazioni, consulta [Pianificazione risorse: indice articolo](../../../resource-mgmt/resource-planning/resource-planning-overview.md).

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

* Scheda secondaria Tabella risorse nella scheda Gestione del personale di un progetto
* L&#39;opzione Usa nuova area di pianificazione nella scheda secondaria Pianificazione della scheda Gestione del personale di un progetto che rimuove l&#39;area di pianificazione legacy o Team Builder. In questo caso, la timeline Pianificazione ora viene visualizzata per impostazione predefinita.
* Scheda Allocazione nel profilo utente

### Report

Le seguenti funzioni di reporting sono state rimosse:

* Funzioni di reporting rimosse:

   * Opzione Tabella risorse in un report utente
   * Opzione Gantt legacy in un progetto o in un report attività\
     Per ulteriori informazioni, consulta [Visualizzare le informazioni nel diagramma di Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

* Rapporti rimossi:

   * Rapporto Pool di risorse legacy
   * Rapporto Stime risorse

  >[!NOTE]
  >
  >Tutti i campi legacy a cui si accede tramite i rapporti o tramite l’API (gruppo di risorse legacy, costo preventivato legacy, costo preventivato legacy, ore preventivate legacy, costo preventivato legacy della manodopera, ecc.) vengono visualizzati in vari rapporti, ma non vengono compilati con le nuove informazioni.

### Gantt legacy

* Tutte le viste Gantt legacy dagli elenchi di progetti e attività, nonché le opzioni per report e reporting
* Schede secondarie Gantt legacy in Portfoli e programmi
* Scheda secondaria Gantt legacy in un elenco di attività modello su un modello, visualizzazione Gantt legacy nella scheda Attività secondarie di un&#39;attività modello e in un report attività modello

### Verifica

Il visualizzatore di bozze legacy è stato sostituito con il nuovo visualizzatore di bozze web e il nuovo visualizzatore di bozze desktop per la maggior parte dei clienti ed è stato rimosso per tutti i clienti a novembre 2020.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">With the 2018.2 release, the Legacy proofing viewer was removed as the default viewer.</p>
-->

Per ulteriori informazioni, consulta le risorse seguenti:

* [Esaminare le bozze nel visualizzatore bozze web](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proofs-in-wpv.md)
* [Esaminare le bozze nel Visualizzatore bozze desktop](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/review-proofs-in-desktop-proofing-viewer.md)

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

## Strumenti basati su Flash legacy e loro sostituti {#legacy-flash-based-tools-and-their-replacements}

Salvo diversa indicazione, tutte le feature legacy sono state sostituite da nuove, come illustrato nella tabella seguente.

>[!CAUTION]
>
>Gli strumenti legacy basati su Flash sono stati rimossi da tutti gli ambienti.

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
   <td> <p><strong>Gruppi di risorse esistenti</strong> </p> <p>I Pool di Risorse legacy erano gruppi o raccolte di Ruoli necessari contemporaneamente per il completamento di un progetto. I gruppi di risorse esistenti presentavano una serie di carenze:</p> 
    <ul> 
     <li> È possibile associare un utente a un gruppo di risorse esistente, ma questo è stato utilizzato solo a scopo di reporting. Poiché i pool di risorse legacy funzionavano con entità ruolo astratte, non sono state prese in considerazione le eccezioni di pianificazione e il tempo libero degli utenti, con conseguente imprecisione dei dati sulla disponibilità delle risorse. </li> 
    </ul> 
    <ul> 
     <li>È possibile specificare un solo pool di risorse legacy per progetto, il che si traduce in più pool di risorse legacy che supportano solo il flusso di gruppi separati che lavorano indipendentemente l’uno dall’altro e non condividono mai le risorse. In tutti gli altri casi, è stato consigliato di mantenere un gruppo di risorse esistente che includesse tutte le risorse nel sistema, il che ha causato problemi di prestazioni con grandi quantità di progetti e dati.</li> 
    </ul> </td> 
   <td> <p><strong>Pool di Risorse</strong> </p> <p>I nuovi gruppi di risorse sono una raccolta di utenti necessari contemporaneamente per il completamento del progetto. Workfront si rende inoltre conto che in alcuni casi è necessario assegnare il lavoro separatamente agli utenti specializzati. Per questo motivo, ora puoi assegnare un budget agli utenti invece che alle mansioni. </p> I vantaggi del gruppo di risorse rispetto ai gruppi di risorse legacy includono: 
    <ul>
     <li>Poiché i pool di risorse sono basati sugli utenti, le eccezioni di indisponibilità e pianificazione vengono già prese in considerazione per i calcoli sulla disponibilità di utenti e ruoli. Ciò consente di ottenere dati precisi e aggiornati, che consentono di prendere decisioni di budget corrette e di ridurre al minimo la probabilità di cambiamenti quando il progetto è in corso.</li>
     <li>Poiché ora è disponibile un maggiore controllo sulla disponibilità delle risorse e sulla precisione dei dati, Workfront consente di associare più gruppi di risorse a un progetto. Un utente può anche appartenere a più gruppi di risorse, nel caso in cui abbia più competenze che potrebbero essere utilizzate in più progetti contemporaneamente. </li>
    </ul><p>Con tale controllo sui dati, non è più necessario disporre di un gruppo di risorse che includa tutte le risorse per la distribuzione del budget disponibile. In effetti, non lo consigliamo. Consigliamo invece di diversificare i Pool di Risorse e di associare solo i Pool di Risorse pertinenti ai progetti.</p><p> Per ulteriori informazioni sui gruppi di risorse, consulta <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Panoramica sui pool di risorse </a></p></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Responsabile budget risorse</strong> </p> <p>È possibile utilizzare Gestione budget risorse per specificare la disponibilità delle risorse dei ruoli in più gruppi di risorse. Tuttavia, a causa delle carenze del Pool di Risorse legacy, questa funzionalità è stata utilizzata raramente. Quando è stato utilizzato, ha costretto gli utenti a inserire manualmente la disponibilità delle mansioni per rendere più accurata la definizione del budget. Le eccezioni alla pianificazione e il tempo libero degli utenti non sono stati presi in considerazione.</p> </td> 
   <td> <p>Con il calcolo automatico della disponibilità basato sugli utenti nei gruppi di risorse, Gestione budget risorse non è più necessario. Lo strumento è stato eliminato, insieme a tutto il lavoro manuale per calcolare la disponibilità.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Stime di Risorse</strong> </p> <p>La scheda Stime risorse in ogni gruppo di risorse esistente ha lo stesso scopo di Responsabile del budget risorse, solo nel contesto di un gruppo di risorse esistente. Questo strumento presenta le stesse limitazioni di Gestione budget risorse e dei Pool di risorse legacy: dati imprecisi e immissione manuale della disponibilità. </p> </td> 
   <td> <p>Con il calcolo automatico della disponibilità utente, le Stime di Risorse sono diventate obsolete e sono state rimosse.</p> <p>Lo strumento viene eliminato nei gruppi di risorse legacy e nelle Stime di risorse legacy nel caso aziendale di un progetto. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The Legacy Resource Estimates area on the Business Case of the project remains there in View-only mode at this time. 
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Capacity Planner</strong> </p> <p>Il Capacity Planner era uno strumento di Workfront per la definizione del budget delle risorse e l'assegnazione delle priorità ai progetti all'interno di un Pool di Risorse Legacy, in base alla disponibilità delle risorse. Data l'incompletezza dei dati delle stime delle risorse e del responsabile del budget risorse che ha fornito le informazioni per il Capacity Planner, è stato necessario verificare la priorità del progetto in base alla disponibilità degli utenti.</p> <p>L'utilizzo di un singolo pool di risorse legacy che includeva tutti i ruoli nel sistema è stato lo scenario più comune, che ha causato problemi di prestazioni con il Capacity Planner che ha tentato di caricare un gran numero di progetti.</p> </td> 
   <td> <p><strong>Vista progetto della Programmazione delle risorse</strong> </p> <p>Nella visualizzazione basata sul progetto della Programmazione delle risorse, è possibile preventivare le risorse e assegnare priorità ai progetti in modo analogo a come si faceva nella Programmazione delle capacità legacy. A differenza dello strumento legacy, ora sono supportati più dati e le informazioni disponibili sono più precise, tenendo conto sia del tempo libero degli utenti che delle eccezioni di pianificazione.</p> <p>Le informazioni disponibili, pianificate e preventivate sono immediatamente visibili in modo che i responsabili delle risorse possano verificare se il numero di persone necessarie per eseguire il lavoro è sufficiente e se i piani di progetto superano le stime di budget iniziali.</p> <p> Per informazioni sull'utilizzo della Vista progetto nella Programmazione delle risorse, vedere <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Panoramica di Programmazione delle risorse</a></p> <p><strong>Pianificazione scenario</strong> </p> <p>Per la pianificazione a lungo termine della capacità, la modellazione di scenari what-if e la definizione delle priorità, abbiamo anche introdotto Workfront Scenario Planner . </p> <p>La Pianificazione scenario è disponibile solo nella nuova esperienza Adobe Workfront e richiede una licenza aggiuntiva. Per informazioni su Workfront Scenario Planner, consulta <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Panoramica sulla pianificazione degli scenari</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Stime risorse legacy (caso aziendale)</strong> </p> <p>È possibile utilizzare l'area Stime risorse legacy del Business Case per preventivare una determinata quantità di ore e costi di manodopera nell'ambito della pianificazione del progetto e della richiesta di risorse. Questa visualizzazione non forniva alcuna visibilità sulla disponibilità delle risorse, il che risultava in richieste approssimative di risorse e una maggiore possibilità di rifiutare il lavoro di progetto.</p> </td> 
   <td> <p><strong>Budget di risorse (Business Case)</strong> </p> <p>La sezione Resource Budgeting nel Business Case include le funzionalità di pianificazione delle risorse nel Business Case, fornendo visibilità sulla disponibilità di utenti e ruoli e sulla possibilità di definire un budget a livello di utente. </p> <p> Per informazioni sull'area Budget risorse del Business Case, vedere <a href="../../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">Panoramica delle aree del Business Case</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Rapporti Stima Risorse</strong> </p> <p>Quando si utilizzano gli strumenti legacy per la gestione delle risorse, è possibile creare rapporti sulle ore pianificate e pianificate dal Business Case. Questo consentiva di creare report matrice che mostravano il lavoro totale preventivato e pianificato per ogni mansione in un intervallo di tempo specifico. Il report non era modificabile e non è stato possibile apportare modifiche al budget delle risorse in base ai risultati del report. </p> </td> 
   <td> <p><strong>Rapporto utilizzo</strong> </p> <p>Il rapporto Uso predefinito visualizza affiancati Ore pianificate, Preventivate e Ore effettive, Costo e Ricavi. </p> <p>Per informazioni sull'utilizzo del rapporto Utilizzo, vedere <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Visualizza informazioni sull'utilizzo delle risorse </a>. </p> 
    <div> 
     <p><strong>Ore preventivate da segnalare</strong> </p> 
     <p>Creare un rapporto relativo alle ore preventivate per esaminare le ore preventivate nella Programmazione risorse in una maschera di rapporto. </p> 
     <p>Per informazioni sulle ore preventivate, consulta <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glossario della terminologia di Adobe Workfront</a>.</p> 
     <p>Per informazioni sulla creazione di un rapporto, consulta <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un rapporto personalizzato</a>.</p> 
    </div> <p><strong>Visualizzazione Ruolo della Programmazione delle risorse</strong> </p> <p>Le ore preventivate e pianificate del caso aziendale negli strumenti legacy di gestione delle risorse sono ora disponibili in una nuova vista nativa, la vista basata sul ruolo della pianificazione delle risorse. Questa vista fornisce informazioni sulle ore disponibili, pianificate e preventivate in breve tempo e consente di controllare e modificare il budget nello stesso luogo. Ciò garantisce un processo decisionale migliore durante la pianificazione dei ruoli di alto livello. </p> <p> Per informazioni sull'impostazione del budget delle risorse nella visualizzazione Ruolo della Programmazione risorse, vedere <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using2" class="MCXref xref">Utilizzare le visualizzazioni Progetto e Ruolo per preventivare le risorse </a> sezione in <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Panoramica di Programmazione delle risorse</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Griglia risorse</strong> </p> <p>La griglia delle risorse fornisce visibilità sull’allocazione di utenti specifici man mano che un progetto progredisce verso il completamento. </p> <p>Ad esempio, puoi facilmente vedere quando qualcuno nel team di progetto ha completato il lavoro in anticipo, quando qualcuno è rimasto indietro e se è stato sovrassegnato o sottoassegnato per un intervallo di tempo specifico. </p> <p>Sfortunatamente, non è stato possibile agire in base alle informazioni nella stessa visualizzazione. Per risolvere i problemi di sovrassegnazione era necessario passare ai progetti e regolare manualmente le informazioni senza visualizzare il risultato delle azioni.</p> </td> 
   <td> <p>La griglia delle risorse è stata sostituita da due nuovi strumenti. Puoi utilizzare i seguenti strumenti, a seconda della fase di pianificazione delle risorse in cui ti trovi:</p> 
    <ul> 
     <li> <p><strong>Per la fase analitica:</strong> </p> 
      <ul> 
       <li> <p><strong>Il Bilanciatore dei carichi di lavoro</strong>: utilizza il Bilanciatore dei carichi di lavoro per visualizzare il carico di lavoro degli utenti a un livello più granulare. Quando si utilizza il Bilanciatore dei carichi di lavoro, è possibile visualizzare gli utenti che dispongono di disponibilità nel carico di lavoro per completare l'attività in tempo. Questo include i dettagli relativi alle ferie e alle eccezioni alla pianificazione. </p> <p>Per informazioni sul Bilanciatore dei carichi di lavoro, consulta <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Panoramica del Bilanciatore dei carichi di lavoro</a>.</p> </li> 
       <li> <p><strong>Visualizzazione utente della Programmazione delle risorse</strong><strong>:</strong> Quando cerchi di capire a un livello più alto a quali progetti sono assegnati gli utenti, utilizza la Vista utente della Programmazione delle risorse. Questo consente di vedere su cosa stanno lavorando gli utenti e le loro sovrassegnazioni e sottoassegnazioni per un intervallo di tempo specifico. La Programmazione delle risorse fornisce anche una visualizzazione dell’allocazione complessiva degli utenti nel suo insieme, nonché la visibilità sulle Ore effettive registrate, utile per analizzare l’avanzamento del lavoro svolto. </p> <p>Per informazioni sull'utilizzo della Vista utente nella Programmazione delle risorse, vedere <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using" class="MCXref xref">Utilizza la Vista utente per visualizzare le Ore disponibili, pianificate ed effettive o FTE </a> sezione in <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Panoramica di Programmazione delle risorse</a></p> </li> 
      </ul> </li> 
     <li><strong>Per la fase tattica:</strong> 
      <ul> 
       <li><strong>Il Bilanciatore dei carichi di lavoro</strong> Puoi eseguire le seguenti operazioni utilizzando il Bilanciatore dei carichi di lavoro: 
        <ul>
         <li>Assegna lavoro agli utenti.</li>
         <li>Gestire le allocazioni degli utenti agli elementi di lavoro. </li>
         <li>Condividi il Bilanciatore dei carichi di lavoro con altri utenti che potrebbero non avere visibilità nell’area Persone. Utilizza la funzionalità di collegamento condivisibile per condividere un collegamento al Bilanciatore dei carichi di lavoro e incorporarlo in dashboard personalizzati. Tutti gli utenti con accesso a Visualizza utenti possono visualizzare queste dashboard quando vengono condivise.</li>
        </ul><p>Il Bilanciatore dei carichi di lavoro è disponibile nell’area Persone. </p><p>Per informazioni sul Bilanciatore dei carichi di lavoro, consulta <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Panoramica del Bilanciatore dei carichi di lavoro</a>.</p></li> 
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
   <td> <p><strong>Grafico di Gantt legacy, elenco attività</strong> </p> <p> Il Grafico di Gantt legacy presente nell'elenco delle attività consente agli utenti di visualizzare visivamente la timeline del progetto e di eseguire la pianificazione dello scenario what-if senza apportare modifiche al database. Il grafico Gantt legacy si basava sulla tecnologia di Flash, che presentava rischi per la sicurezza. </p> </td> 
   <td> <p><strong>Diagramma di Gantt,</strong> <strong>Elenco attività</strong></p> <p> Il nuovo Diagramma di Gantt basato su HTML ha lo stesso scopo del Gantt legacy. Gli utenti possono visualizzare la timeline del progetto ed eseguire la pianificazione dello scenario what-if senza apportare modifiche al database passando all’opzione Salvataggio manuale dalla barra degli strumenti dell’elenco di attività. </p> <p>Il nuovo Diagramma di Gantt è interattivo quando si utilizza l’opzione Salvataggio automatico, che è possibile utilizzare quando si desidera salvare automaticamente le modifiche nel momento in cui si verificano. </p> <p>Il nuovo Diagramma di Gantt dell’elenco delle attività si basa sulla tecnologia più recente ed è affidabile. Questo nuovo diagramma di Gantt si trova direttamente nell'elenco delle attività ed è facilmente accessibile quando si lavora sull'elenco delle attività senza cambiare scheda o senza modificare la visualizzazione. </p> <p>Sebbene il nuovo diagramma di Gantt offra le stesse funzionalità del grafico precedente, vi sono alcune differenze nelle caratteristiche rispetto al diagramma precedente. </p> <p> La scheda secondaria Gantt legacy in un elenco di attività modello su un modello, la vista Gantt legacy nella scheda Attività secondarie di un'attività modello e il grafico Gantt legacy in un report Attività modello sono stati sostituiti anche con il grafico Gantt basato su HTML. </p> <p>Se si utilizza il Grafico di Gantt legacy principalmente per la visualizzazione semplice e le modifiche rapide e non si utilizza il grafico effettivo, la nuova opzione Pianificazione sequenza temporale consente di apportare modifiche rapide ai campi di pianificazione chiave. Dalla barra degli strumenti dell'elenco di task è possibile selezionare Pianificazione sequenza temporale anziché Salvataggio automatico.</p> <p>Per ulteriori informazioni sul salvataggio di un elenco di task mediante l'opzione Pianificazione sequenza temporale, vedere la sezione "Salvare manualmente le modifiche in un elenco di task quando si seleziona l'opzione Pianificazione sequenza temporale" nell'articolo <a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Modificare le attività in un elenco</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Grafico di Gantt legacy per un elenco di progetti</strong> </p> <p>Il Grafico di Gantt legacy nell’elenco dei progetti consentiva agli utenti di visualizzare i progetti e le relative attività in un’unica schermata. Senza uscire dal contesto dell’elenco dei progetti, gli utenti potevano visualizzare i dettagli delle attività di un progetto e le dipendenze tra i progetti. Il grafico Gantt legacy nell’elenco dei progetti si basava sulla tecnologia di Flash, che presentava rischi per la sicurezza. </p> </td> 
   <td> <p><strong>Diagramma di Gantt, elenco progetti</strong> </p> <p>Il grafico di Gantt basato su HTML ha lo stesso scopo del grafico Gantt legacy. Gli utenti possono visualizzare i progetti e le relative attività in un’unica visualizzazione per identificare visivamente le dipendenze tra progetti e attività. Il diagramma di Gantt dell’elenco dei progetti si trova direttamente nell’elenco dei progetti. Il nuovo grafico Gantt ha un'interfaccia moderna ed è basato sulla tecnologia più recente.</p> <p>Per informazioni sull'elenco dei progetti Diagramma di Gantt, vedere <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Visualizzare le informazioni nel diagramma di Gantt </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Finestre di dialogo di condivisione per report, calendari e documenti</strong> </p> <p>Quando si condividevano report, calendari e documenti, le finestre di dialogo utilizzate erano basate sulla tecnologia di Flash.</p> </td> 
   <td> <p>L'esperienza di condivisione di report, calendari e documenti in Workfront non è cambiata. Tuttavia, l’esperienza non si basa più sul Flash.</p> <p>Per ulteriori informazioni sulla condivisione di questi elementi, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Panoramica delle autorizzazioni di condivisione sugli oggetti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Visualizzatore di bozze legacy</strong> </p> <p>Il visualizzatore di bozze legacy era un visualizzatore di bozze basato su web che forniva funzionalità di bozza per bozze statiche, video e interattive.</p> </td> 
   <td> <p><strong>Visualizzatore bozze Web e visualizzatore bozze desktop</strong> </p> <p>Il visualizzatore bozze web fornisce funzionalità di bozza per bozze statiche e video.</p> <p>Il Visualizzatore bozze desktop fornisce funzionalità di bozza per le bozze interattive, oltre a fornire supporto completo per le bozze statiche e video.</p> <p>Il formato di file SWF non è più supportato da nessuno dei principali provider ed è stato sostituito con i banner HTML5 per la verifica. </p> <p>Per informazioni più dettagliate sulle differenze tra i visualizzatori di bozze disponibili, vedere <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Panoramica sulle differenze tra il visualizzatore bozze web e il visualizzatore bozze desktop</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
