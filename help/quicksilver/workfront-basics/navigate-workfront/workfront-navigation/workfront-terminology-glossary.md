---
content-type: reference
navigation-topic: workfront-navigation
title: Glossario di [!DNL Adobe Workfront] terminologia
description: Il [!DNL Adobe Workfront] il glossario elenca i termini più comunemente utilizzati in Adobe Workfront.
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '19720'
ht-degree: 0%

---

# Glossario di [!DNL Adobe Workfront] terminologia

>[!IMPORTANT]
>
>Questo articolo deve essere utilizzato come riferimento per comprendere i termini che è possibile incontrare nel [!DNL Adobe Workfront] applicazione, nella [!DNL Workfront] o quando si parla in generale di pianificazione e gestione del lavoro. Stiamo aggiornando queste informazioni e di conseguenza questa tabella potrebbe non essere completa. La dichiarazione di non responsabilità verrà rimossa quando considereremo esaustive tali informazioni.

La tabella seguente è un elenco dei termini comunemente utilizzati in Adobe Workfront:

## A - C

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nome Oggetto</strong></th> 
   <th><strong>Descrizione</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Livello d'Accesso]</td> 
   <td>Profilo utente che determina il modo in cui un utente può interagire con diversi oggetti e strumenti all’interno di Workfront.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività Attiva]</td> 
   <td>Un'attività incompleta in un progetto corrente che non è impedita da un'attività predecessore e che non ha un vincolo attività con una data di inizio pianificata futura. In altre parole, si può lavorare oggi.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Activity]</td> 
   <td>In entrata [!DNL Workfront Goals], un’attività è un indicatore di avanzamento per un obiettivo. Può trattarsi di una barra di avanzamento che aggiorni manualmente o di un progetto associato all’obiettivo. Non è possibile visualizzare le attività in un rapporto e non è possibile accedervi tramite [!DNL Workfront] API. Per informazioni sulle attività, consulta <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Introduzione ai risultati e alle attività in Obiettivi di Adobe Workfront</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo Reale]</td> 
   <td> <p>Per attività e problemi, si tratta del costo associato alle ore effettive registrate in relazione alla tariffa oraria del costo della risorsa assegnata all'attività o al problema. Per i progetti, questo valore rappresenta un totale di tutti i [!UICONTROL Costi effettivi] relativi alle attività e ai problemi del progetto. Per informazioni, consulta <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tracciare i costi</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo Spesa Reale]</td> 
   <td> <p>Somma degli [!UICONTROL Importi effettivi] per tutte le spese registrate per un progetto o un'attività.</p> <b>ESEMPIO </b>
   <p>Se si crea una spesa per l'attività 1 e si immettono 600,00 $ nel campo [!UICONTROL Importo effettivo], il costo effettivo dell'attività [!UICONTROL Costo spesa effettivo] è 600,00 $. </p> 
   <p>Per un progetto, [!DNL Workfront] utilizza la formula seguente per calcolare [!UICONTROL Costo spesa effettivo]:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ore effettive]</td> 
   <td> <p>In un report di progetto, attività o problema, [!UICONTROL Ore effettive] sono la somma di tutte le ore registrate nel progetto, attività o problema.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span> Se dalla scheda [!UICONTROL Aggiornamenti] per l'attività 1 si fa clic su "Tempo di log" e si immettono 25 ore, le ore effettive dell'attività 1 = 25 ore. </p> <p>[!DNL Workfront] calcola [!UICONTROL Ore effettive] per le attività o i progetti padre utilizzando le formule seguenti:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo effettivo manodopera]</td> 
   <td> <p>Il [!UICONTROL Costo effettivo] associato alla manodopera investita in un'attività o in un progetto. </p> <p>Per un’attività, [!DNL Workfront] calcola il [!UICONTROL Costo effettivo manodopera] utilizzando la formula seguente:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Se l'attività ha un tipo di costo [!UICONTROL] di [!UICONTROL User Hourly], [!DNL Workfront] utilizza il tasso di utenti. Se l'attività ha un tipo di costo [!UICONTROL] di [!UICONTROL Ore Ruolo], [!DNL Workfront] utilizza il tasso di ruolo per calcolare [!UICONTROL Costo effettivo manodopera]. </p> <p>Per un progetto, [!DNL Workfront] utilizza la formula seguente per calcolare il [!UICONTROL Costo effettivo manodopera]:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tracciare i costi</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Ad esempio, se un utente registra 5 ore per un'attività con un [!UICONTROL User Hourly] [!UICONTROL Cost Type] e la tariffa oraria è di $100, il [!UICONTROL Actual Labor Cost] è di $500.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ricavi effettivi] </td> 
   <td> <p>Il ricavo effettivo di un progetto o di un'attività è la quantità di denaro associata alle [!UICONTROL Ore effettive] del progetto o dell'attività. </p> <p>Per informazioni sul tracciamento dei ricavi in [!DNL Workfront], vedi <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica su fatturazione e ricavi</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL inizio effettivo]</td> 
   <td>La marca temporale quando un utente modifica un oggetto in esecuzione sul lavoro assegnato.</td> 
  </tr> 
  <!--<tr> 
 <td>A type of work process that is unplanned.</td> 
 -->
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Additional Schedules</td> 
    <td>An additional preset to be used for a new user group.</td> 
   </tr>
  --> 
  <tr> 
   <td>Metodologia [!UICONTROL Agile]</td> 
   <td>Un tipo di metodologia basata sull’evoluzione collaborativa delle esigenze e delle soluzioni con team interfunzionali. Incoraggia la flessibilità e i cambiamenti sulla base di un calendario fisso.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Team Agile]</td> 
   <td>Si differenzia dal team tradizionale perché prende il lavoro potenziale da un backlog e lavoraci entro un periodo di tempo definito denominato [!UICONTROL Iteration].</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tutti I Miei Team]</td> 
   <td> <p>Quando si fa riferimento a questo in [!UICONTROL filters], in questo campo vengono visualizzati gli utenti che appartengono a uno qualsiasi dei team a cui appartiene l'utente connesso o gli elementi di lavoro assegnati a uno qualsiasi dei team a cui appartiene l'utente connesso. </p> <p>È consigliabile utilizzare questo campo in un filtro per rendere i rapporti più generici quando vengono condivisi con altri utenti. In questo modo, puoi creare un solo rapporto che visualizzerà informazioni diverse a seconda di chi effettua l’accesso per visualizzarle, poiché queste sono sempre personalizzate per l’utente connesso. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Allocation Date]</td> 
   <td> <p>Questo campo è disponibile nei seguenti tipi di rapporti:</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Project] (Dati Finanziari)</li> 
     <li>[!UICONTROL Ora Preventivata]</li> 
    </ul> <p>Per un<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->Rapporto [!UICONTROL Project (Financial Data)]: </p> 
    <ul> 
     <li>Genera questo rapporto quando cerchi di comprendere <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> la quantità di [!UICONTROL Lavoro Necessario] assegnata alle risorse.</li> 
     <li> <p>La [!UICONTROL Allocation Date] è il primo giorno (domenica) della settimana in cui inizia l'allocazione di una mansione [!UICONTROL] a un'attività. Una risorsa ([!UICONTROL Job Role]) può avere un numero di [!UICONTROL Allocation Dates] pari alle settimane durante il [!UICONTROL Duration] delle attività a cui è assegnata. Se le attività si estendono su più mesi, il primo giorno di un mese può anche diventare un [!UICONTROL Allocation Date], se rientra nella [!UICONTROL Duration] dell'attività.</p> <p>Ad esempio, puoi assegnare un [!UICONTROL Job Role] a un'attività che dura più di 3 settimane e ha 90 [!UICONTROL Planned Hours]. Queste ore vengono distribuite uniformemente durante la durata dell'attività, in modo che ogni giorno assegni 6 [!UICONTROL Lavoro Necessario] al tuo ruolo:</p> <p><em> [!UICONTROL Ore pianificate giornaliere] = [!UICONTROL Ore pianificate totali]/ Numero di [!UICONTROL Giorni lavorativi] durante la [!UICONTROL Durata] dell'attività </em> </p> <p>Di conseguenza, durante il periodo di [!UICONTROL Duration] dell'attività esistono tre [!UICONTROL Allocation Dates], una per ogni domenica di ogni settimana, a cui è associato un determinato numero di [!UICONTROL Planned Hours].<br>Se l'attività inizia a metà dell'ultima settimana di un mese e termina due settimane dopo l'inizio di un nuovo mese, l'attività avrà quattro [!UICONTROL Allocation Dates]: una per ogni domenica di ogni settimana durante la [!UICONTROL Duration] dell'attività e una per il primo giorno del nuovo mese.</p> <p>Per utilizzare al meglio queste informazioni, ti consigliamo di creare una <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> Crea un report (Dati finanziari) per il progetto e aggiungi un raggruppamento di matrici per [!UICONTROL Allocation Date], quindi raggruppa i risultati settimanalmente, mensilmente, trimestralmente o annualmente per ottenere i dati più accurati.<br>Per informazioni sulla creazione di un raggruppamento di matrici, vedere l'articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Creare un rapporto matrice</a>.</p> </li> 
    </ul> <p>Le informazioni finanziarie vengono inserite nei rapporti di [!UICONTROL Project (Financial Data)] solo quando i dati ad esse associati hanno meno di 5 anni. Ad esempio, se una mansione è stata allocata a un'attività nel gennaio 2015 e oggi è settembre 2021, un campo finanziario come [!UICONTROL Allocation Date] per la mansione non si popola nel rapporto [!UICONTROL Project (Financial Data)]. </p> 
    <div> 
     <p>Per un rapporto di [!UICONTROL Budgeted Hour]:</p> 
     <ul> 
      <li>Crea questo rapporto quando tenti di comprendere la quantità di [!UICONTROL Ore Preventivate] allocata alle risorse o ai progetti nella Programmazione delle risorse.</li> 
      <li> <p>La [!UICONTROL Allocation Date] è il primo giorno (una domenica) della settimana per la quale sono state preventivate le ore nel [!UICONTROL Resource Planner]. </p> <p>Suggerimento   <p>Se una settimana dura due mesi, verranno generate due righe nel rapporto: una corrispondente al primo giorno della settimana (domenica della prima settimana che cade durante il primo mese) e la seconda riga visualizza il primo giorno del secondo mese. </p> <p>Ad esempio, se preventivi 8 ore per un utente per la settimana dal 30 giugno (domenica) al 6 luglio (sabato), le due righe mostrano una [!UICONTROL Allocation Date] del 30 giugno e del 1 luglio. </p> </p> <p>Per informazioni sulla definizione del budget delle risorse, vedere [!DNL Resource Planner], vedi l’articolo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Risorse di budget nel [!DNL Resource Planner] utilizzo delle visualizzazioni [!UICONTROL Project] e [!UICONTROL Role]</a>.</p> <p>Per informazioni sulla creazione di un report [!UICONTROL Budgeted Hour], vedere <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Ore preventivate</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Announcements]</td> 
   <td> <p>Un modo per comunicare agli utenti informazioni all’interno del sistema. Queste informazioni spesso provengono da [!DNL Workfront] all'amministratore o dall'amministratore all'utente. </p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Inviare annunci</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL - Integrazione app]</td> 
   <td>Un’app rappresenta più comunemente un connettore per un’applicazione software, ma può anche rappresentare funzioni speciali che manipolano i dati.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Decisione approvatore]</td> 
   <td> <p>Nel rapporto [!UICONTROL Proof Approval] (Approvazione bozza) questo campo visualizza le decisioni di approvazione delle bozze per le bozze che non sono più attive.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fase approvatore]</td> 
   <td>Nel rapporto [!UICONTROL Proof Approval] (Approvazione bozza), questo campo visualizza informazioni su una fase corrente delle bozze.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval]</td> 
   <td> <p>Per un determinato elemento di lavoro, ad esempio un'attività, un documento o una scheda orario, può essere necessario che un supervisore o un altro utente approvi l'elemento di lavoro. Questo processo di approvazione è denominato approvazione. </p> <p>Per ulteriori informazioni, consulta <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Panoramica del processo di approvazione</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di approvazione]</td> 
   <td>Nel rapporto [!UICONTROL Proof Approval] (Approvazione bozza), questo campo visualizza la data di approvazione di una bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver]</td> 
   <td>Un utente o una mansione che deve approvare un dato elemento di lavoro o l'utente che approva le ore inserite nelle schede orario.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assegnato A]</td> 
   <td> <p>In un report [!UICONTROL Attività o Problema] questo campo visualizza il Proprietario dell'attività o del problema o l'assegnatario principale [!UICONTROL]. Puoi anche filtrare o raggruppare in base a questo campo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment]</td> 
   <td>Un utente, una mansione o un team assegnato a un problema o a un’attività. I progetti, i portfolio o i programmi non possono avere assegnazioni.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assegnazioni]</td> 
   <td> <p>In un rapporto di [!UICONTROL Attività] o [!UICONTROL Problema], questo campo visualizza un elenco di tutte le entità (utenti, ruoli, team) assegnate all'attività o al problema. È possibile filtrare in base a questo campo utilizzando i campi [!UICONTROL Assignment Users] e [!UICONTROL Assignment Roles]. Puoi filtrare in base al team assegnato all’attività o al problema utilizzando il campo Team. Impossibile raggruppare un report in base a questo campo.</p> <p>Gli elementi di lavoro posizionati nel Cestino [!UICONTROL] continueranno a essere visualizzati in alcuni report che fanno riferimento all'oggetto [!UICONTROL Assignment] in cui [!DNL OR] viene utilizzato un modificatore di filtro.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ruoli di assegnazione]</td> 
   <td>
   <p>In un report [!UICONTROL Attività] o [!UICONTROL Problema], questo campo visualizza informazioni sulle mansioni assegnate alle attività o ai problemi. In questo campo vengono visualizzati [!UICONTROL Proprietari primari] e altri ruoli assegnati ad attività o problemi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stato assegnazione]</td> 
   <td> <p>In un report di assegnazioni, attività o problemi, in [!UICONTROL Assignment Status] viene visualizzato se gli utenti assegnati a un elemento di lavoro hanno fatto clic sul pulsante [!UICONTROL Work On It] o [!UICONTROL Done] per accettare o completare il lavoro. Sono presenti i seguenti stati di [!UICONTROL Assignment Status]:</p> 
    <ul> 
     <li><b>[!UICONTROL Richiesto]</b>: l’utente è stato assegnato all’attività o al problema, ma non ha ancora fatto clic sul pulsante [!UICONTROL Lavoraci] per iniziare a lavorarci.</li> 
     <li><b>[!UICONTROL Funzionante]</b>: l'utente ha fatto clic sul pulsante [!UICONTROL Lavoraci] e sta attualmente lavorando sull'elemento. </li> 
     <li><b>[!UICONTROL completato]</b>: l'utente ha fatto clic sul pulsante [!UICONTROL Done] e ha completato il lavoro sull'elemento. </li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">Cenni preliminari sul pulsante [!UICONTROL Work On It] e [!UICONTROL Done]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Teams]</td> 
   <td>
   <p>In un rapporto di [!UICONTROL attività] o [!UICONTROL problema], questo campo visualizza informazioni sui team assegnati alle attività o ai problemi. Nel campo vengono visualizzati [!UICONTROL Proprietari principali] e gli altri team assegnati ad attività o problemi. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utenti assegnazione]</td> 
   <td>
   <p>In un report [!UICONTROL Attività] o [!UICONTROL Problema], questo campo visualizza informazioni sugli utenti assegnati alle attività o ai problemi. In questo campo vengono visualizzati [!UICONTROL Proprietari principali] e altri utenti assegnati ad attività o problemi. </p></td> 
  </tr> 
  <tr> 
   <td>Attributo [!UICONTROL]</td> 
   <td>Un attributo è una caratteristica di un [!DNL Workfront] oggetto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Area Di Audit]</td> 
   <td> <p>I controlli di audit sono messaggi di sistema che registrano un’azione eseguita in Workfront. Vengono registrati i seguenti tipi di controllo:</p> 
    <ul> 
     <li>[!UICONTROL Modifica ambito]</li> 
     <li>[!UICONTROL Attachment Action]</li> 
     <li>[!UICONTROL - Modifica generale]</li> 
     <li>[!UICONTROL - Modifica stato]</li> 
     <li>[!UICONTROL Note]</li> 
     <li>[!UICONTROL Voce Combinata]</li> 
     <li>[!UICONTROL Voce Di Errore]</li> 
     <li>[!UICONTROL - Modifica stato]</li> 
     <li>[!UICONTROL Modifica sottoscrizione]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Trail]</td> 
   <td>La raccolta di note generate automaticamente dagli eventi che vengono tracciati attraverso le Modifiche registrate ([!UICONTROL Aree di controllo]). Ogni nota registra chi ha fatto l'azione, cosa ha fatto e quando l'ha fatto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automatico E In Modifica]</td> 
   <td> <p>Uno dei tipi [!UICONTROL Project Update]. Le sequenze temporali Previsto e Pianificato del Progetto verranno ricalcolate quando viene eseguito il processo di ricalcolo notturno e quando viene effettuato un aggiornamento al Progetto o alle Attività all’interno del Progetto. </p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleziona il tipo di aggiornamento del progetto </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Disponibilità</p></td> 
   <td> <p>Questo termine viene utilizzato in relazione alla "disponibilità dell'utente" o alla "disponibilità delle risorse" e indica la quantità di tempo in cui la risorsa (utente o mansione) è disponibile per lavorare. </p> 
   <p>Workfront calcola la disponibilità dell'utente utilizzando diversi campi e in base alle impostazioni delle preferenze di Gestione risorse del sistema. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurare le preferenze di Gestione risorse</a>. </p>
   <p>Per ulteriori informazioni sulla disponibilità delle risorse, consulta <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Introduzione alla gestione delle risorse</a></p>
   In alternativa, "capacità" viene utilizzato anche per fare riferimento alla disponibilità delle risorse. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Solo Automatico]</td> 
   <td> <p>Uno dei tipi [!UICONTROL Project Update]. In questo modo verranno ricalcolati i timeline Previsti e Pianificati quando viene eseguito il processo di ricalcolo notturno.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleziona il tipo di aggiornamento del progetto</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>Il lavoro "business as usual" che contribuisce a raggiungere gli obiettivi aziendali principali quotidiani.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Backlog]</td> 
   <td>L’area in un ambiente agile in cui vengono mantenute le nuove questioni fino a quando non sono pronte per essere elaborate.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Baseline]</td> 
   <td>Origine di dati su cui misurare le iterazioni in un ambiente agile.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Fatturazione]</td> 
   <td> <p>Registra i ricavi, le ore o le spese che possono essere fatturati. Queste informazioni possono essere utilizzate per creare fatture in un sistema contabile esterno.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Crea record fatturazione</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>Stato record fatturazione</td> 
   <td> <p>In un rapporto Fatturazione o Ora, lo Stato di una fattura indica se la fattura è stata Fatturata o Non Fatturata. Non puoi eliminare un progetto o modificare l’ora associata a un record di fatturazione Fatturata. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Crea record fatturazione</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Branding]</td> 
   <td><p>Il processo di personalizzazione [!DNL Workfront] per dare all'interfaccia un aspetto che rispecchia la società utilizzando i colori e i loghi.</p><p><strong>NOTA</strong><br>Se per la tua organizzazione è stato eseguito l’onboarding in [!DNL Adobe Experience Cloud], branding non disponibile.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Breadcrumb]</td> 
   <td> <p>L’area nella parte superiore della pagina che mostra la posizione gerarchica della posizione in cui si trova l’utente nell’applicazione.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Per ulteriori informazioni, consulta <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Panoramica delle breadcrumb</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stato budget]</td> 
   <td> <p>Questo è un campo obsoleto. Qualsiasi informazione visualizzata in questo campo è correlata a una funzione [!DNL Workfront] è stato rimosso e non è possibile aggiornare il campo. </p> <p>Questo campo mostra se il progetto è stato aggiunto al [!UICONTROL Capacity Planner] e se il relativo calcolo del budget è stato completato. Il [!UICONTROL Capacity Planner] è stato rimosso da [!DNL Workfront]. </p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;not added to the capacity planner, its value is <i>Not Included</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;added to the Capacity Planner but is excluded from the budget calculation,&nbsp;the value is <i>Included but not Calculated</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is&nbsp;added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgeted Completion Date]</td> 
   <td> <p>Questo è un campo obsoleto. Qualsiasi informazione visualizzata in questo campo è correlata a una funzione [!DNL Workfront] ha rimosso. Impossibile aggiornare questo campo. </p>
   <p> Questo campo è ancora visibile nei report e negli elenchi [!UICONTROL project] e [!UICONTROL tasks].</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo Preventivato]</td>

<td> <p>Si tratta del costo associato alle risorse di definizione del budget per un progetto. </p>
   <p>Il campo viene visualizzato nelle seguenti aree di [!DNL Workfront] sotto i seguenti nomi:</p>
   <ul>
   <li><strong>[!UICONTROL Costo Preventivato]</strong>: nel pannello [!UICONTROL Business Case Summary]</li>
   <li><strong>[!UICONTROL Costo]</strong>: nelle aree [!UICONTROL Utilization] quando si visualizzano le informazioni per [!UICONTROL Cost]</li>
   <li><strong>[!UICONTROL Costo preventivato progetto]</strong>: in elenchi e report</li>
   </ul>   
    <p>Il costo preventivato di [!UICONTROL] per il progetto viene calcolato con la seguente formula:</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Per ulteriori informazioni sul calcolo di [!UICONTROL Costo preventivato] e per comprendere i vari nomi di questo concetto in [!DNL Workfront], vedi <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calcola costo preventivato progetto</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ore Preventivate]</td> 
   <td> <p>Le ore preventivate per le risorse per il lavoro da completare sui progetti. Questo campo si riferisce alle ore preventivate nell'area [!UICONTROL Resource Budgeting] del business case [!UICONTROL] (o nel Resource Planner [!UICONTROL]) per il progetto o per le risorse del progetto.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Informazioni su [!UICONTROL Budgeted Labor Cost] e [!UICONTROL Budgeted Hours] per i progetti</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Per informazioni sulla definizione del budget degli utenti in [!DNL Resource Planner], vedi l’articolo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Risorse di budget nel [!DNL Resource Planner] utilizzo delle visualizzazioni [!UICONTROL Project] e [!UICONTROL Role]</a>. </p> 
    <p>Le ore preventivate nell'area [!UICONTROL Resource Budgeting] del Business Case [!UICONTROL] o del Resource Planner [!UICONTROL] vengono visualizzate nelle seguenti aree di [!DNL Workfront] e sotto i seguenti nomi:</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>Nome visualizzato di [!UICONTROL Ore preventivate]</strong></td> 
        <td><strong>Aree di [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Hours]</td> 
        <td>Area [!UICONTROL Resource Budgeting] del Business Case [!UICONTROL]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Resource Planner] visualizzato da [!UICONTROL Hours]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Ore Preventivate]</td> 
        <td> <p>Visualizzazione report di utilizzo [!UICONTROL Hours]</p> <p>Per ulteriori informazioni sul rapporto Utilizzo di [!UICONTROL], vedi l'articolo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Panoramica del rapporto Utilizzo risorse [!UICONTROL]</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. Ore]</td> 
        <td> <p>Rapporto [!UICONTROL Ore preventivate]</p><p>L'oggetto [!UICONTROL Budgeted Hour] nel report Ore preventivate fa riferimento a informazioni relative a uno strumento di gestione delle risorse obsoleto. Solo il "[!UICONTROL Bud. Il campo Ore]" in questo report si riferisce alle ore preventivate nell'area [!UICONTROL Resource Planner] o [!UICONTROL Resource Budgeting] del progetto [!UICONTROL Business Case]. </p> <p>Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un rapporto personalizzato</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Ore preventivate di programmazione risorse] </td> 
        <td> <p>Trovato nei seguenti rapporti:</p>
        <ul>
        <li>Report [!UICONTROL Project]
        <li>Rapporto Progetto [!UICONTROL (dati finanziari)]
        <li>Report [!UICONTROL Task]
        <li>Report [!UICONTROL Issue]
        <li>Rapporto [!UICONTROL Ore preventivate]</li>
        </ul>
         <p>Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un rapporto personalizzato</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Qualsiasi altra indicazione di [!UICONTROL Ore Preventivate] in [!DNL Adobe Workfront] si riferisce alle ore preventivate utilizzando funzioni obsolete che sono state rimosse da Workfront. Si tratta di campi di sola visualizzazione che non vengono aggiornati con le informazioni correnti quando si utilizzano gli strumenti di budgeting delle risorse correnti. </p>
    <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the&nbsp;Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy&nbsp;Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy&nbsp;Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial&nbsp;Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul> --> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo manodopera preventivato]</td> 
   <td> <p>Questo è il costo associato alle ore che il Responsabile risorse deve preventivare per le mansioni per il lavoro da completare nei progetti. </p> <p>Il [!UICONTROL Budgeted Labor Cost] in un report di progetto viene calcolato utilizzando la seguente formula:</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Questo campo può fare riferimento a quanto segue:</p> 
    <ul> 
     <li> <p>I costi della manodopera visualizzati nell'area [!UICONTROL Resource Budgeting] del Business Case di [!UICONTROL] o nel Resource Planner di [!UICONTROL] associati al costo delle mansioni in un progetto. Per informazioni sul calcolo di [!UICONTROL Costo manodopera preventivato], vedere l'articolo <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Comprendere il costo della manodopera preventivato] e [!UICONTROL Ore preventivate] per i progetti</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>I costi della manodopera visualizzati nell'area [!UICONTROL Resource Budgeting] del Business Case [!UICONTROL] che riflettono i [!UICONTROL People Costs] stimati in un'iniziativa collegata al progetto da [!DNL Scenario Planner] quando si utilizza la Pianificazione scenario per preventivare le risorse del progetto. Per informazioni sulle iniziative, consulta <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Panoramica delle iniziative nella Pianificazione scenario</a>. </p> <p>Il [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Il [!DNL Scenario Planner] panoramica</a>. </p> </li> 
     <p>Viene visualizzato nelle seguenti aree di sotto i seguenti nomi:</p>
   <ul>
   <li><strong>[!UICONTROL Costo manodopera preventivato]</strong>: nell’area [!UICONTROL Resource Budgeting] del Business Case di [!UICONTROL].
   <li><strong>[!UICONTROL Costo Preventivato]</strong>: nella visualizzazione [!UICONTROL Utilization] del report [!UICONTROL Cost]
   <p>Per ulteriori informazioni, consulta <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Visualizza informazioni sull'utilizzo delle risorse </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: nel [!DNL Resource Planner] Progetto o [!DNL Role] visualizzazioni, quando si visualizza per costo
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: nei seguenti rapporti: 
   <ul>
    <li>Report [!UICONTROL Project]</li>
    <li>Rapporto Progetto [!UICONTROL (dati finanziari)]</li>
    <li>Report [!UICONTROL Task]</li>
    <li>Report [!UICONTROL Issue]</li>
    <li>Rapporto [!UICONTROL Ore preventivate]</li> 
    </ul>
    <p>Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un rapporto personalizzato</a>.</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in&nbsp;Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;.&nbsp;</p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Budgeted Start Date]</td> 
  <td> <p>Questo è un campo obsoleto. Qualsiasi informazione visualizzata in questo campo è correlata a una funzione [!DNL Workfront] ha rimosso. Impossibile aggiornare questo campo.</p>
  <p>Queste aree sono state rimosse da [!DNL Workfront]. </p> 
  <p>Il campo è ancora visibile nei report e negli elenchi di [!UICONTROL project] e [!UICONTROL task].</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Grafico Burndown [!UICONTROL]</td> 
   <td>Grafico a linee che fornisce una rappresentazione visiva del lavoro completato e rimanente.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case]</td> 
   <td> <p>Strumento utilizzato per valutare se un progetto deve essere spostato in avanti dallo stato [!UICONTROL Idea] allo stato [!UICONTROL Planning]. In altre parole, un business case [!UICONTROL] aiuta l'organizzazione a decidere se sia utile avviare e completare il progetto o meno, soprattutto quando si confrontano i progetti con altri in un portfolio.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Creare un business case [!UICONTROL] per un progetto </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ore preventivate caso di business]</td> 
   <td> <p>Questo è un campo obsoleto. Qualsiasi informazione visualizzata in questo campo è correlata a una funzione [!DNL Workfront] ha rimosso. Impossibile aggiornare questo campo.</p> <p>Questo campo è ancora visibile negli elenchi e nei report di progetti e attività [!UICONTROL]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assegnazione Calcolata]</td> 
   <td> <p>Uno dei tipi di attività [!UICONTROL Duration]. In questo modo verrà calcolata la percentuale di un giorno lavorativo di 8 ore che l'utente assegnato all'attività verrà allocato all'attività, in base alla [!UICONTROL Duration] dell'attività e al [!UICONTROL Work Required].</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica dell'attività [!UICONTROL Duration] e [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lavoro Calcolato]</td> 
   <td> <p>Uno dei tipi di durata dell'attività [!UICONTROL]. In questo modo verrà calcolato il lavoro [!UICONTROL Work Required] per un'attività, date le percentuali di [!UICONTROL Duration] e di [!UICONTROL Assignment] utente (basate su un giorno lavorativo di 8 ore).</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica dell'attività [!UICONTROL Duration] e [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar]</td> 
   <td> <p>Esistono due tipi di calendari in [!DNL Workfront]: i report Calendario predefinito e calendario di [!UICONTROL].</p> <p>Il [!UICONTROL Home Calendar] è un calendario personale che consente a un utente di gestire il proprio carico di lavoro rispetto alle ore disponibili in [!DNL Workfront]. L'utente può anche integrare il proprio [!UICONTROL Home Calendar] con [!DNL Outlook] ([!DNL Google] e [!DNL Microsoft] l'integrazione). </p> <p>Per ulteriori informazioni sul Calendario predefinito di [!UICONTROL], vedere <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">Visualizzazione Calendario predefinito di [!UICONTROL]</a>.</p> <p>Un report calendario è un report dinamico in cui gli utenti possono visualizzare la data e altri dettagli importanti di un evento, tra cui la data di scadenza, lo stato del lavoro e l'utente a cui l'evento è assegnato.</p> <p> Per ulteriori informazioni sui report calendario, vedere <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Panoramica dei rapporti sul calendario</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Può Iniziare]</td> 
   <td> <p>Questo campo indica se un'attività è pronta per essere lavorata. Se l'inizio è pronto per essere elaborato sul campo [!UICONTROL Può iniziare] dell'attività è impostato su [!UICONTROL True]. </p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">Panoramica di "[!UICONTROL Può iniziare]" per le attività</a>.</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    --> <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.&nbsp;</li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.&nbsp;</li> 
     </ul>
    --> 
    <!--
     <p>For information about task predecessors, see <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p>
    --> <!--
     <p>Tip: If the Dependency Type between a task and its predecessors is Start-Start, the predecessor must start before the predecessor relationship is considered resolved and the successor tasks can start. For information about dependency types, see <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>. </p>
    --> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Capacity</td> 
    <td>The total availability (measure in either hours or FTE) of a designated user, resource pool, team, rob role, or company.</td> 
   </tr>
  -->

<tr> 
   <td> <p>Capacità</p> </td> 
   <td> <p>Il tempo disponibile di una risorsa quando può essere allocata al lavoro. Consulta "Disponibilità". </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Categoria]</p> </td> 
   <td> <p>Una categoria è un modulo personalizzato. È possibile creare report per questo oggetto e visualizzarlo anche in altri report oggetto. Non tutti gli oggetti possono avere un modulo o una categoria personalizzata. I seguenti oggetti possono avere un modulo personalizzato: <br></p> 
    <ul> 
     <li>Progetto [!UICONTROL]</li> 
     <li>[!UICONTROL Attività]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Portfoli]</li> 
     <li>[!UICONTROL Documento]</li> 
     <li>[!UICONTROL Spesa]</li> 
     <li>[!UICONTROL Program]</li> 
     <li>[!UICONTROL Utente]</li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iterazione]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome Categoria]</td> 
   <td> <p>Quando viene aggiunta come colonna alla visualizzazione di uno dei seguenti oggetti, viene visualizzato un elenco di tutti i moduli personalizzati associati a tali oggetti:</p> 
    <ul> 
     <li>Progetto [!UICONTROL]</li> 
     <li>[!UICONTROL Attività]<br></li> 
     <li>[!UICONTROL Issue]<br></li> 
     <li>[!UICONTROL Portfoli]<br></li> 
     <li>[!UICONTROL Documento]<br></li> 
     <li>[!UICONTROL Spesa]<br></li> 
     <li>[!UICONTROL Program]<br></li> 
     <li>[!UICONTROL Utente]<br></li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iterazione]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Gestione modifiche]</td> 
   <td>Un'area di esercitazione incentrata sulla definizione, la comprensione e l'adattamento del lavoro pianificato ai cambiamenti di ambito, pianificazione, costi e fattori delle risorse.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Order]</td> 
   <td>Tipo di problema sollevato in relazione a un progetto che illustra una richiesta di modifica dell’ambito concordato.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Solo Modifica]</td> 
   <td>Uno dei tipi di aggiornamento del progetto [!UICONTROL]. Aggiorna le timeline di [!UICONTROL Project Projected] (Progetto previsto) e [!UICONTROL Planned] (Pianificato) solo quando vengono apportati aggiornamenti alle attività o alle modifiche al progetto o alle attività.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Order]</td> 
   <td> <p>Uno dei tipi di problema [!UICONTROL], che in genere indica che è necessario eseguire una quantità di lavoro non pianificata prima di completare il progetto.</p> <p>Per ulteriori informazioni sui tipi di [!UICONTROL Issue], consulta la sezione "Default issue types" nell'articolo <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Personalizzare i tipi di problemi predefiniti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL attività figlio]</td> 
   <td>Un'attività che è una [!UICONTROL Subtask] di un' [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL elementi figlio]</td> 
   <td>L'insieme di [!UICONTROL Subtasks] in un'attività padre [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] e [!UICONTROL Training]</td> 
   <td>Moduli di apprendimento, certificazioni, standard o una community di professionisti.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit]</td> 
   <td>Strumento di comunicazione che consente agli utenti di impostare le aspettative relative ai risultati finali delle attività.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit Date]</td> 
   <td>Strumento di comunicazione che consente all’utente di impostare le aspettative relative ai risultati finali delle attività.</td> 
  </tr> 
  <tr> 
   <td>Comunicazione [!UICONTROL] e reporting [!UICONTROL]</td> 
   <td>Standard per la verifica delle eccezioni e dello stato di un progetto, programma o portfolio</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Company]</td> 
   <td> <p>Una [!UICONTROL Company] è un'unità organizzativa in [!DNL Workfront]. </p> 
   <p> È possibile associare un utente o un progetto a una società. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Creare e modificare le società</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di completamento]</td> 
   <td> <p>La data in cui un progetto, un’attività o un problema è impostato per essere completato. Esistono diversi tipi di [!UICONTROL Completion Date] in [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL Data di completamento effettiva]. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Panoramica del progetto [!UICONTROL Data di completamento effettiva] </a>.</li> 
     <li>[!UICONTROL Data di completamento Pianificata]. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Imposta il progetto [!UICONTROL Planned Completion Date]</a> e <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Panoramica dell'attività [!UICONTROL Data di completamento pianificata]</a>.</li> 
     <li>[!UICONTROL Data di completamento Prevista]. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Panoramica di [!UICONTROL Data di completamento prevista] per progetti, attività e problemi</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Day]</td> 
   <td>Il giorno, relativo all'inizio del [!UICONTROL Template], in cui deve essere completata un'[!UICONTROL Template Task] o un [!UICONTROL Template].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modalità di completamento]</td> 
   <td> <p>Indica come verrà contrassegnato un progetto come [!UICONTROL Complete]. Può avere due valori:</p> 
    <ul> 
     <li>[!UICONTROL Manual]: un utente deve modificare lo stato del progetto in [!UICONTROL Complete].</li> 
     <li>[!UICONTROL Automatic]: lo stato del progetto passa automaticamente a [!UICONTROL Complete] quando tutte le attività del progetto sono completate al 100% e tutti i problemi sono chiusi.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Condizione [!UICONTROL]</td> 
   <td> <p>Si tratta di una rappresentazione visiva dell’avanzamento di un’attività, un problema o un progetto.</p> <p>Per i progetti, la condizione può essere impostata manualmente dal proprietario del progetto oppure automaticamente da [!DNL Workfront], in base allo stato di avanzamento del progetto. </p> <p>I valori possibili per la condizione del progetto sono:</p> 
    <ul> 
     <li>[!UICONTROL Su Target]</li> 
     <li>[!UICONTROL A Rischio]</li> 
     <li>[!UICONTROL Nei Problemi]</li> 
    </ul> <p>Per ulteriori informazioni sulla condizione del progetto, consulta l’articolo <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Panoramica della condizione del progetto [!UICONTROL] e del tipo di condizione [!UICONTROL]</a>.</p>
     <p>È possibile associare le condizioni di attività e problemi a un numero che può essere visualizzato nei rapporti. Negli elenchi seguenti vengono visualizzati i nomi e i numeri predefiniti per le condizioni di attività e problemi. L’amministratore di sistema può aggiornare i nomi delle condizioni e aggiungere nuove condizioni con numeri diversi. Quando un numero è associato a una condizione, non può essere modificato.  </p> 
     <p>Per le attività, la condizione viene impostata manualmente dal proprietario dell'attività. I valori possibili per la condizione di attività sono:</p> 
    <ul> 
     <li>[!UICONTROL Senza Problemi] (0)<br></li> 
     <li> [!UICONTROL Alcuni problemi] (1)<br></li> 
     <li>[!UICONTROL Principali Elementi Di Blocco] (2)</li> 
    </ul> <p>Per ulteriori informazioni sulla condizione dell'attività, vedere l'articolo <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Aggiorna condizione [!UICONTROL] per attività e problemi</a>.</p> <p>Per i problemi, la condizione viene impostata manualmente dal proprietario del problema. I valori possibili per la condizione di problema sono:<br></p> 
    <ul> 
     <li>[!UICONTROL Senza Problemi] (0)<br></li> 
     <li>[!UICONTROL Alcuni problemi] (1)<br></li> 
     <li>[!UICONTROL Principali Elementi Di Blocco] (2)</li> 
    </ul> 
   <p><b>NOTA</b></p>
    <p>Quando il campo Condizione [!UICONTROL] viene tracciato nei report [!UICONTROL Voce diario], nei report [!UICONTROL Nuovi] e [!UICONTROL Vecchi valori numerici] viene visualizzato il numero associato alla condizione anziché il nome. Se per un'attività o un problema non è stata originariamente definita una condizione e successivamente viene aggiornata, la voce del journal che acquisisce l'aggiornamento visualizzerà il valore [!UICONTROL Old Number Value] del campo [!UICONTROL Condition] come -2.147.483.648. Vedi anche "[!UICONTROL New Number Value]", "[!UICONTROL Old Number Value]" e "[!UICONTROL Journal Entry]" in questo articolo. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition Update]</td> 
   <td> <p>Questo campo mostra la condizione corrente delle attività, dei progetti o dei problemi. Questa opzione mostra gli aggiornamenti più recenti forniti dai proprietari di attività, progetti o problemi nel campo [!UICONTROL Update Status] (Stato aggiornamento), insieme alla nuova condizione.</p> <p>I commenti aggiunti agli aggiornamenti delle condizioni non vengono visualizzati nella colonna [!UICONTROL Condition Update], ma solo nell'aggiornamento principale.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data Vincolata]</td> 
   <td> <p>Se si utilizza un [!UICONTROL Vincolo attività] associato a una data specifica, ad esempio [!UICONTROL Deve iniziare il], tale data specifica diventerà il [!UICONTROL Vincolo data] dell'attività.</p> <p>I seguenti vincoli di attività aggiornano il campo [!UICONTROL Constraint Date]:</p> 
    <ul> 
     <li>[!UICONTROL Deve Iniziare Il]</li> 
     <li>[!UICONTROL Deve Finire Il]</li> 
     <li>[!UICONTROL Inizia Non Più Tardi]</li> 
     <li>[!UICONTROL Iniziare Non Prima Di]</li> 
    </ul> <p>Suggerimento   
     <ul> 
      <li> <p>Un'attività con [!UICONTROL Constraint] di [!UICONTROL Fixed Dates] non ha [!UICONTROL Constraint Date]. </p> </li> 
      <li> <p> [!UICONTROL Data vincolo] è visualizzabile solo in un report o in una visualizzazione personalizzata.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vincolo Giorno]</td> 
   <td> <p>Se si utilizza un vincolo attività in un'attività modello associata a un giorno specifico, ad esempio Deve iniziare il, tale giorno specifico diventa il giorno vincolo dell'attività modello.</p> <p>I seguenti vincoli di attività aggiornano il campo [!UICONTROL Constraint Day]:</p> 
    <ul> 
     <li>[!UICONTROL Deve Iniziare Il]</li> 
     <li>[!UICONTROL Deve Finire Il]</li> 
     <li>[!UICONTROL Inizia Non Più Tardi]</li> 
     <li>[!UICONTROL Iniziare Non Prima Di]</li> 
    </ul> <p>Suggerimento: [!UICONTROL Constraint Day] è visualizzabile solo in un report o in una visualizzazione personalizzata. </p> </td> 
  </tr> 
  <tr> 
   <td>Tipo di vincolo [!UICONTROL]</td> 
   <td> <p>Tendenza di programmazione di un'attività. Ad esempio, [!UICONTROL Appena possibile] pianifica l'inizio di un'attività il prima possibile e [!UICONTROL Fine non oltre] pianifica il completamento di un'attività entro il [!UICONTROL Data vincolo] e non oltre.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica di [!UICONTROL Task Constraint]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Menu contestuale di [!UICONTROL]</td> 
   <td>Un menu, situato sul lato sinistro dello schermo, in cui le voci vengono modificate in modo da essere correlate al contenuto attivo. Ad esempio, quando un utente visualizza un progetto, nel menu contestuale di [!UICONTROL] verranno visualizzati collegamenti a informazioni e strumenti relativi al progetto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converted Issue Originator]</td> 
   <td>Campo in un report di progetti o attività che visualizza informazioni sull'utente che è il [!UICONTROL Contatto principale] di un problema quando il problema viene convertito in un progetto o in un'attività. Il campo viene visualizzato anche nella sezione [!UICONTROL Project Details] (Dettagli progetto) in cui viene visualizzato il nome del [!UICONTROL Primary Contact] del problema convertito. Vedi anche "[!UICONTROL Contatto principale]" in questo articolo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Costo]</td> 
   <td> <p>Importo monetario da spendere per il completamento di un progetto, attività o problema. </p> <p>È possibile tenere traccia di vari tipi di costi per manodopera, spese e rischi correlati al progetto.Per informazioni sulla registrazione dei costi in [!DNL Workfront] vedi <a href="../../../manage-work/projects/project-finances/track-costs.md">Tracciare i costi</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di costo]</td> 
   <td>Per un'attività, il [!UICONTROL Tipo di costo] determina il modo in cui l'attività accantonerà i costi. Alcuni esempi includono [!UICONTROL Ore Fisse], [!UICONTROL Ore Utente] e [!UICONTROL Ore Utente più Fisse]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dipendenze tra progetti]</td> 
   <td> <p>Un'attività di un progetto dipende da un'attività di un progetto diverso.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Creare predecessori per più progetti</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Dati Personalizzati]</td> 
   <td> <p>Dati univoci di un’organizzazione. Le organizzazioni possono personalizzare [!DNL Workfront] creazione di moduli personalizzati e campi personalizzati. Queste informazioni personalizzate possono stimolare il reporting per KPI, auditing e demand mix. </p> <p>[!UICONTROL Custom Data] può essere collegato a:</p> 
    <ul> 
     <li>[!UICONTROL Progetti]</li> 
     <li>[!UICONTROL Attività]</li> 
     <li>[!UICONTROL Utenti]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documenti]</li> 
     <li>[!UICONTROL Spese]</li> 
     <li>[!UICONTROL Portfoli]</li> 
     <li>[!UICONTROL Programmi]</li> 
     <li>[!UICONTROL Iterazioni]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Data Type]</td> 
   <td>Opzione che consente di specificare se un campo [!UICONTROL Custom Data] è memorizzato nel database come testo, data, numero o valuta.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Display Type]</td> 
   <td>Tipo di visualizzazione di un campo personalizzato. Gli esempi includono [!UICONTROL Elenco a discesa], [!UICONTROL Campo di testo], [!UICONTROL Area di testo], [!UICONTROL Pulsanti di scelta], ecc.</td> 
  </tr> 
  <tr> 
   <td>Campo personalizzato [!UICONTROL]</td> 
   <td>Per i dati personalizzati che consentono all’utente di selezionare tra diverse opzioni, questi sono i valori da cui un utente può selezionare. Le opzioni personalizzate sono valide solo in [!UICONTROL Elenco a discesa], [!UICONTROL Elenchi a discesa a selezione multipla], [!UICONTROL Pulsanti di opzione] e [!UICONTROL Caselle di controllo].</td> 
  </tr> 
  <tr> 
   <td>Etichetta modulo personalizzato [!UICONTROL]</td> 
   <td>Quando si utilizza un tipo di visualizzazione personalizzato con opzioni personalizzate, si tratta del testo dell’interfaccia utente che verrà visualizzato nel menu a discesa, nelle caselle di controllo o nei pulsanti di scelta per tale opzione personalizzata.</td> 
  </tr> 
  <tr> 
   <td>Valore personalizzato [!UICONTROL]</td> 
   <td>Quando si utilizza un campo personalizzato con opzioni personalizzate, questo è il valore che verrà memorizzato nel database per una particolare opzione.</td> 
  </tr> 
  <tr> 
   <td>Visualizzazione personalizzata [!UICONTROL]</td> 
   <td>Definizione dei campi o delle colonne di dati visualizzati per ogni oggetto di un elenco.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cliente]</td> 
   <td>Organizzazione che utilizza un'istanza di Workfront.</td> 
  </tr> 
 </tbody> 
</table>

## D - F

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome Oggetto</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Dashboards]</td> 
   <td> <p> È possibile aggiungere questo campo in un report o in un elenco dell'oggetto report per visualizzare i dashboard in cui il report è elencato. </p> <p> Puoi utilizzare questo campo per filtrare anche i rapporti elencati in un dashboard specifico. </p> <p> Per ulteriori informazioni sull'inclusione delle informazioni del dashboard nei report sugli oggetti report, vedere la sezione "Informazioni sui report elencati nei dashboard" nell'articolo <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Accedere e organizzare i rapporti</a></p> </td> 
  </tr> 
  <tr> 
   <td>Tipo di dati [!UICONTROL]</td> 
   <td>Consulta "[!UICONTROL Custom Data Type]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Days Late]</td> 
   <td> <p>Questo campo mostra una differenza di data tra [!UICONTROL Planned Start] e [!UICONTROL Today] se manca la [!UICONTROL Actual Completion Date].</p> <p>Mostra anche una differenza di data tra [!UICONTROL Completamento effettivo] e [!UICONTROL Completamento pianificato], quando è presente una [!UICONTROL Data di completamento effettiva].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Default Schedule]</td> 
   <td> <p>Le ore di lavoro predefinite personalizzabili da assegnare a utenti e progetti all’interno di un’organizzazione. </p> <p>Le pianificazioni vengono utilizzate per calcolare le date pianificate, di inizio e di completamento delle attività assegnate agli utenti.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Deliverable]</td> 
   <td>Beni o servizi quantificabili che devono essere forniti al completamento di un progetto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Demand Management]</td> 
   <td>Punteggio e definizione delle priorità dei processi di assunzione.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Obiettivi Reparto]</td> 
   <td>Obiettivi specifici per un reparto specifico che si concentrano sul miglioramento delle metriche operative all’interno del reparto.</td> 
  </tr> 
  <tr> 
   <td>Dipendenza [!UICONTROL]</td> 
   <td>Anche il collegamento tra due attività che richiedono la modifica dello stato di un'attività prima che l'altra possa cambiare stato.</td> 
  </tr> 
  <tr> 
   <td>Tipo di dipendenza [!UICONTROL]</td> 
   <td> <p>Tipo di relazione di programmazione tra un'attività e i suoi predecessori. Un esempio è [!UICONTROL Finish-Start], che richiede che la prima attività debba terminare prima che la seconda possa iniziare.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Panoramica dei tipi di relazione tra attività</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Documento]</td> 
   <td>Qualsiasi file allegato a un oggetto all'interno di [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL versione documento]</td> 
   <td> <p>Ogni volta che lo stesso documento viene caricato nello stesso oggetto, gli viene assegnato un numero di versione. Gli utenti possono visualizzare e modificare diverse opzioni per una versione precedente di un documento.</p> <p>Per ulteriori informazioni, consulta <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Gestire le versioni dei documenti</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration]</td> 
   <td> <p>Intervallo di tempo allocato per il completamento di un problema o progetto di attività (come determinato dal numero di giorni tra l'inizio pianificato [!UICONTROL] e il completamento pianificato).</p> 
    <ul> 
     <li>Per le attività, la Durata è un campo modificabile se il Tipo di Durata dell'attività non è Semplice. Se il Tipo di durata dell'attività è Semplice o se il Vincolo attività è Date fisse, la Durata è un calcolo eseguito da Workfront.</li> 
     <li>Per i problemi, il campo Durata è sempre modificabile e deve rappresentare una stima di un numero di giorni che richiederebbero la risoluzione del problema.</li> 
     <li>Per i progetti, la Durata è un calcolo eseguito da [!DNL Workfront] e rappresenta la differenza in giorni tra l'inizio pianificato della prima attività e il [!UICONTROL Planned Completion] dell'ultima attività del progetto.</li> 
    </ul> <p>Per ulteriori informazioni sulla differenza tra [!UICONTROL Duration] e [!UICONTROL Planned Duration] per le attività, vedi l'articolo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Differenza tra [!UICONTROL Planned Duration] e [!UICONTROL Duration] per le attività</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Durata in minuti]</td> 
   <td>Questo campo visualizza le stesse informazioni del campo [!UICONTROL Duration] in minuti anziché in giorni. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Durata per Occorrenza]</td> 
   <td> <p>Questa operazione viene visualizzata nelle caselle [!UICONTROL Dettagli attività] e [!UICONTROL Modifica attività] di un elemento padre di attività ricorrenti. Viene visualizzata la durata di ogni attività ricorrente. Per informazioni sulla creazione di attività ricorrenti, vedere <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Creare attività ricorrenti</a>. </p> <p> <span>Le durate modificate in singole attività ricorrenti non visualizzano il valore indicato in questo campo.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Tipo di durata [!UICONTROL]</td> 
   <td> <p>Campo dell'attività che indica il modo in cui il lavoro necessario per completare l'attività viene allocato agli assegnatari per tutta la durata dell'attività. Rappresenta la relazione tra la [!UICONTROL Duration] dell'attività, il lavoro [!UICONTROL Work Required] e la quantità di tempo, o allocazione [!UICONTROL Allocation], che le risorse assegnate devono dedicare all'attività per completarla. </p> <p>Questo campo viene visualizzato nella scheda [!UICONTROL Details] di un'attività. </p> <p>Le opzioni sono:</p> 
    <ul> 
     <li>[!UICONTROL Assegnazione calcolata]</li> 
     <li>[!UICONTROL Lavoro Calcolato]</li> 
     <li>[!UICONTROL Basato Sullo Sforzo]</li> 
     <li>[!UICONTROL semplice]</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica dell'attività [!UICONTROL Duration] e [!UICONTROL Duration Type]</a>.</p> 
    —&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Unità di Durata]</td> 
   <td>Unità utilizzata per misurare il tempo in una ricerca di risparmio energia.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Basato Sullo Sforzo]</td> 
   <td>La relazione tra il numero di utenti e il tempo necessario al completamento dell'attività. Quando si aggiungono più utenti, il tempo totale pianificato per il completamento dell'attività diminuisce, ma la durata dell'attività rimane invariata. Ad esempio, se un'attività sta svuotando un barile di noccioline, l'aggiunta di più persone diminuirà il tempo pianificato, ma la durata in giorni-persona rimarrà la stessa.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo Trascorso]</td> 
   <td> <p>[!UICONTROL Tempo trascorso] è un'unità di tempo per [!UICONTROL Durata] di un'attività. È l'intervallo di tempo compreso tra [!UICONTROL Planned Start Date] (Data di inizio pianificata) e [!UICONTROL Planned Completion Date] (Data di completamento pianificata) di un'attività che include ferie, fine settimana e ferie. In altre parole, il tempo trascorso è il trascorrere dei giorni di calendario. </p> <p>[!DNL Workfront] supporta le seguenti unità di tempo trascorse per la durata dell'attività:</p> 
    <ul> 
     <li> <p>[!UICONTROL Minuti Trascorsi]</p> </li> 
     <li> <p>[!UICONTROL Ore Trascorsi]</p> </li> 
     <li> <p>[!UICONTROL Giorni Trascorsi]</p> </li> 
     <li> <p>[!UICONTROL Settimane Trascorsi]</p> </li> 
     <li> <p>[!UICONTROL Mesi Trascorsi]</p> </li> 
    </ul> <p>Per ulteriori informazioni sulla durata dell'attività, incluso il tempo trascorso, vedere <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica dell'attività [!UICONTROL Duration] e [!UICONTROL Duration Type]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di fine]</td> 
   <td> <p> In un report [!UICONTROL Rate], indica la data di fine di una nuova tariffa di fatturazione per una mansione a livello di progetto. Le ore associate al progetto precedenti a questa data vengono moltiplicate per questa tariffa di fatturazione per calcolare i ricavi sul progetto. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Engagement]</td> 
   <td>[!UICONTROL Work Performance Indicator] (WPI) che indica quando l'impegno e la fiducia nell'attività, nel progetto, nel team o nell'organizzazione stanno diminuendo. Questo indica che devi agire per far rivivere quella convinzione e quell'impegno. WPI si misurava facendo le semplici domande: "Hai capito cosa ci si aspettava da te? Il lavoro che ti è stato assegnato ha cambiato l’organizzazione? Hai fatto un ottimo lavoro?"</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Enterprise Goals]</td> 
   <td>Obiettivi interfunzionali che contribuiscono alle metriche degli obiettivi aziendali.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event]</td> 
   <td>Qualsiasi modifica apportata a un progetto o a un'attività.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event Handler]</td> 
   <td>Attività automatizzate che si verificano quando si verificano gli eventi. Un esempio comune è una notifica e-mail automatizzata.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notifica evento]</td> 
   <td>E-mail generata da un gestore eventi.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Spese]</td> 
   <td>Costo non manodopera per attività o progetti.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Esterno]</td> 
   <td> <p>In genere, un tipo di licenza, o un utente con tale licenza, che ha solo la possibilità di rivedere le informazioni nel sistema.</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] panoramica sulle licenze</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External System]</td> 
   <td>Qualsiasi servizio o software memorizzato e gestito al di fuori del sistema di registrazione designato.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Field]</td> 
   <td><p>Qualsiasi oggetto Workfront o le informazioni ad esso associate, così come sono visualizzate nel database. </p>
   <p>Ad esempio, "progetto", "utente", "ora" sono sia oggetti di Workfront che campi. "Nome", "stato", "proprietario", "data di inizio" sono campi di Workfront associati agli oggetti di cui sopra. </p>

<p>Quando si fa riferimento a un oggetto, i termini "oggetti" e "campi" possono essere utilizzati in modo intercambiabile.</p>
   <p>Nell’ambito del reporting, i "campi" si riferiscono agli oggetti o alle informazioni sull’oggetto che desideri acquisire nel report.</p>

<p><b>NOTA</b></p>

<p>Nei rapporti di tipo testo-altro, i campi fanno riferimento agli oggetti o alle relative informazioni così come vengono visualizzati nel database.</p>
   <p>A volte il nome visualizzato nell’interfaccia utente è diverso dal nome del campo nel database. Ad esempio, "problema" è il nome dell’oggetto nell’interfaccia di Workfront, ma "opTask" è il nome dell’oggetto (o del campo) nel database di Workfront. </p> 
   <p> È importante utilizzare il campo così come viene visualizzato nel database quando si scrive un report in modalità testo, si visualizza, si filtra o si crea un campo calcolato.</p>

<p>Per ulteriori informazioni, consulta <a href="../../../wf-api/general/api-explorer.md">API Explorer</a> e <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">Panoramica sulla modalità testo</a>.</p>

<p>Per impostazione predefinita, Workfront include un set di campi che definiscono sia gli oggetti che le relative informazioni. È inoltre possibile creare campi personalizzati per definire gli oggetti, ma non è possibile creare oggetti personalizzati.</p> 
   </td> 
  </tr>

<tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filtro]</td> 
   <td> <p>Uno dei principali blocchi predefiniti di un rapporto o di un elemento elenco che definisce quali informazioni visualizzare sullo schermo. Per ulteriori informazioni sugli elementi di reporting, consulta <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementi di reporting: filtri, viste e raggruppamenti</a>.</p> <p>Il filtro determina i risultati visualizzati in un report o in un [!DNL Workfront] elenco di pannelli, ad esempio progetti, attività o problemi.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Gestione lavoro finanziario]</td> 
   <td>Processo per gestire i dati su costi della manodopera, spese e ricavi in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo Fisso]</td> 
   <td>È possibile definire un importo fisso di costo per un progetto. Questo fa parte del [!UICONTROL Planned Cost] del progetto che rappresenta la quantità di denaro necessaria per completare il progetto. Per informazioni sui costi, consulta <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tracciare i costi</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reddito Fisso]</td> 
   <td>È possibile definire un importo fisso di ricavi per un progetto. Fa parte del [!UICONTROL Planned Revenue] del progetto che rappresenta la quantità di denaro che potresti ottenere se completi il progetto. Per informazioni sui ricavi, consulta <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica su fatturazione e ricavi</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Flags]</td> 
   <td> <p> Questo campo è uguale a [!UICONTROL Status Icons], ma è disponibile solo per le visualizzazioni seguenti: </p> 
    <ul> 
     <li> [!UICONTROL Modelli] </li> 
     <li> [!UICONTROL Spese] </li> 
    </ul> <p> Per ulteriori informazioni, consulta l’articolo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Icone di stato incorporate nelle visualizzazioni</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>Le cartelle vengono utilizzate per organizzare documenti o report associati a un oggetto.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (Equivalente tempo pieno)</td> 
   <td>Equivalente tempo pieno che indica il tempo di disponibilità di una risorsa per il lavoro. 
   Il campo [!UICONTROL FTE] viene visualizzato nelle seguenti aree: 
  <ul>
   <li> Profilo dell’utente, durante la modifica o la creazione dell’utente </li>
   <li> [!UICONTROL Pianificazione risorse] </li>
   <li> [!UICONTROL Scenario Planner] (richiede una licenza aggiuntiva per Workfront Scenario Planner) </li>
   <li> Elenchi di utenti e report </li> </ul>

<p>Il valore di [!UICONTROL FTE] deve essere un numero decimale massimo di 1 e non può essere 0. </p>
   <p> Un [!UICONTROL FTE] pari a 1 (impostazione predefinita per il campo [!UICONTROL FTE] di un utente, come definito nel relativo profilo) indica che una risorsa (utente o ruolo) funziona per l'intero numero di ore, in base alla pianificazione che ne calcola la disponibilità. </p>
   <p>L'amministratore di Workfront determina la pianificazione da utilizzare per determinare la disponibilità dell'utente.  </p>
   <ul>
   <li> Quando si utilizza la pianificazione predefinita di [!UICONTROL], Workfront utilizza l'FTE [!UICONTROL] dell'utente trovato nel proprio profilo per calcolare la disponibilità. </li>
   <li> Quando si utilizza la pianificazione dell'utente, Workfront utilizza il tempo libero dell'utente, il valore dell'orario di lavoro [!UICONTROL] e le ore della pianificazione predefinita [!UICONTROL] per calcolare l'FTE dell'utente. </li> </ul>

<p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurare le preferenze di Gestione risorse</a>.  </p>
   <p>Per ulteriori informazioni sulla creazione di pianificazioni in [!DNL Workfront], vedi <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Creare una pianificazione</a>. </p>

<p><b>NOTA</b></p>
   <p>Per tutti i calcoli in [!UICONTROL Scenario Planner], Workfront utilizza il valore seguente: 1 [!UICONTROL FTE] = 8 ore.</p>
   <p>Per ulteriori informazioni, consulta <a href="../../../scenario-planner/get-started-with-scenario-planning.md">Introduzione a [!UICONTROL Scenario Planner]</a>. </p>
   </td> </tr> 
   </tbody> 
   </table>

<!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Task field used by the planner to set how the work required is allocated to the assignees across the duration.</p>
<!--
FTE
The designated full time equivalency for users. A full-time user should have 100% FTE and part-time user should have a percentage that equals their working hours. 
-->

## G - I

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome Oggetto</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Grafico di Gantt [!UICONTROL]</td> 
   <td> <p>Una sequenza temporale visiva delle date del progetto in una visualizzazione calendario basata sulle date pianificate o previste in quanto le attività del progetto sono attualmente pianificate.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal]</td> 
   <td><p>Esistono due concetti di obiettivi in [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>Obiettivi del progetto</b>: una serie di obiettivi aziendali concordati dalle parti interessate di un progetto. Gli obiettivi del progetto fanno parte del Business Case di un progetto. </p> <p>Non è possibile visualizzare gli obiettivi del progetto in elenchi o rapporti, ma è possibile accedervi tramite l’API. </p> <p>Per informazioni sugli obiettivi del progetto di caso di business, consulta <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Creare obiettivi di business case </a>. </p> </li> 
     <li> <p><b>Obiettivi strategici</b>: un obiettivo strategico è un obiettivo che puoi creare per pianificare la tua strategia di lavoro per un periodo di tempo specifico. Puoi creare questi tipi di obiettivi utilizzando [!DNL Workfront Goals]. La tua organizzazione deve acquistare una licenza aggiuntiva e devi avere accesso a questa funzione per poter creare obiettivi strategici. [!DNL Workfront Goals] sono disponibili solo con una licenza aggiuntiva.</p> 
     <p>Per ulteriori informazioni, consulta <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] panoramica </a>. </p> 
     <p>Puoi visualizzare gli obiettivi strategici in un rapporto di obiettivo o progetto e accedervi tramite l’API. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Gerarchia obiettivi]</td> 
   <td> <p>Nei rapporti [!UICONTROL Obiettivo] e [!UICONTROL Progetto], questo è un campo di raccolta che visualizza gli obiettivi nella gerarchia a cui appartiene un obiettivo strategico quando è allineato ad altri obiettivi. Gli obiettivi sono separati da un delimitatore ▸. </p> <p>In questo campo vengono visualizzati solo i padri dell’obiettivo e l’obiettivo. Gli obiettivi secondari non vengono visualizzati. </p> <p>Per informazioni sull’allineamento degli obiettivi in [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Panoramica sull’allineamento degli obiettivi in [!DNL Workfront Goals]</a>. </p> 
   <p>Questo campo è visibile solo se l’organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sulla gestione degli obiettivi strategici tramite [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] panoramica </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Punteggio di successo obiettivo]</td> 
   <td> In un report di [!UICONTROL Project] questo campo faceva riferimento agli obiettivi a livello di progetto associati al caso [!UICONTROL Business]. Attualmente, si tratta di un campo obsoleto e non è associato ad alcuna funzionalità.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Goals] </td> 
   <td> <p>In un report [!UICONTROL Project], questo è un campo di raccolta che visualizza tutti gli obiettivi strategici associati a un progetto. Gli obiettivi sono separati da virgole.</p> <p>Questo campo è visibile solo se l’organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sulla gestione degli obiettivi strategici tramite [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] panoramica</a>. Per ulteriori informazioni sugli obiettivi strategici e sugli obiettivi del progetto in [!DNL Workfront], vedi "[!UICONTROL Goal]" in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global Interface Preferences]</td> 
   <td>Impostazioni di interfaccia che interessano tutti gli utenti. Le [!UICONTROL Global Interface Preferences] possono essere sovrascritte da [!UICONTROL User Interface Preferences].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Group]</td> 
   <td> <p>Un insieme di utenti (possibilmente dello stesso reparto o business unit) che hanno accesso agli stessi oggetti. Oltre agli utenti, i gruppi possono essere associati a portfolio, programmi, progetti,<span> modelli di progetto,</span> società, team, pianificazioni, modelli di layout e profili di schede orario.</p> <p>È inoltre possibile concedere autorizzazioni agli oggetti per gruppo. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Panoramica sui gruppi</a>.</p> <p>In un elenco o in un report di oggetti di uno dei tipi seguenti è possibile utilizzare il campo [!UICONTROL Group] per elencare gli oggetti di quel tipo associati a un determinato gruppo: utente, portfolio, programma, progetto, <span>modello di progetto</span>, società, team, pianificazione, modello di layout o profilo scheda orario.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Group Administrator]</td> 
   <td> <p>Utenti che gestiscono gli oggetti, l’accesso e gli utenti di gruppi di utenti designati.</p> <p> In un report [!UICONTROL Group], questo campo visualizza i nomi degli utenti designati come [!UICONTROL Group Administrators] nel gruppo. Per ulteriori informazioni sugli amministratori di gruppi, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppi</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group con accesso amministratore]</td> 
   <td> <p> In un [!UICONTROL Layout Template], [!UICONTROL Timesheet Profile] o [!UICONTROL Schedule Report] questo campo visualizza i gruppi i cui amministratori di gruppi hanno accesso per modificare il modello. Puoi anche filtrare il rapporto in base a questo campo. </p> <p> Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creare e gestire modelli di layout</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Raggruppamento]</td> 
   <td> <p>Elemento di reporting utilizzato per categorizzare le informazioni in un elenco in base a un criterio comune.</p> <p>Per ulteriori informazioni, consulta la sezione "[!UICONTROL Groupings]" nell’articolo <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementi di reporting: filtri, viste e raggruppamenti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Handoff Date]</td> 
   <td> <p>Data in cui un'attività diventa disponibile per il lavoro. La [!UICONTROL Handoff Date] è un calcolo e non può essere impostata manualmente. <br>Per ulteriori informazioni su [!UICONTROL Handoff Date], vedi l'articolo <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">Panoramica di [!UICONTROL Task Handoff Date]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help Desk]</td> 
   <td>La porzione di [!DNL Workfront] che contiene tutte le code di problemi. L'[!UICONTROL Help Desk] può essere utilizzato per elaborare ticket di assistenza clienti, richieste di progetto, ticket di help desk, ecc. Corrisponde all'area [!UICONTROL Requests].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proprietario]</td> 
   <td>In un report di [!UICONTROL Hour], l'utente a cui sono attribuite le ore è [!UICONTROL Owner]. È diverso dall’utente che registra effettivamente l’ora. Queste due entità possono a volte essere due utenti diversi. <br>Per ulteriori informazioni sull’ora di registrazione per un altro utente, consulta l’articolo <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Tempo di connessione</a>.</td> 
  </tr>

<tr> 
   <td>Stato delle Ore</td> 
   <td> <p>Attributo impostato da Workfront per le ore effettive registrate dagli utenti per attività, problemi o progetti. </p>

Le ore possono avere uno dei seguenti stati in Workfront:
<ul>
   <li><b>Inviato</b>: le ore sono state registrate per un progetto, un’attività o un problema. Fanno parte di una fatturazione o non sono ancora stati aggiunti a una fatturazione.</li>
   <li><b>Approvato</b>: le ore sono state registrate e approvate dal proprietario del progetto. Fanno parte di una fatturazione o non sono ancora stati aggiunti a una fatturazione.</li> 
   <li><b>Non Approvato</b>: le ore sono state registrate e rifiutate dal proprietario del progetto. Fanno parte di una fatturazione o non sono ancora stati aggiunti a una fatturazione.</li>
   <li><b>Fatturato</b>: le ore sono state registrate, aggiunte a una fatturazione e lo stato della fatturazione è stato contrassegnato come Fatturato. Non era necessario che fossero approvati dal proprietario del progetto.</li>
   <li><b>Fatturato e Approvato</b>: le ore sono state registrate, approvate dal proprietario del progetto, e lo stato del record di fatturazione è stato contrassegnato come Fatturato.</li>
   </ul>


<p>Quando le ore fanno parte di una fatturazione, lo Stato Ore indica se le ore sono state approvate o se la Fatturazione a cui appartengono è stata fatturata. Lo stato di un'ora è visibile solo in un elenco o report di ore. </p>

<p>Per ulteriori informazioni sull’aggiunta di ore ai record di fatturazione, consulta la sezione "Aggiungere ore ai record di fatturazione" nell’articolo <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Crea record fatturazione</a>.</p>

<p>Per ulteriori informazioni sull'approvazione del tempo sui progetti, vedi <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Richiede l'approvazione del tempo per un progetto</a>.</p>

<p><b>SUGGERIMENTO</b></p>

<p>Le ore generali non registrate direttamente sugli elementi di lavoro non visualizzano uno Stato delle ore. </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Hour Type]</td> 
   <td> <p>Attributo che può essere impostato per le ore effettive registrate per attività, problemi o progetti. Questo è anche un attributo per le ore registrate che non sono collegate direttamente all'attività, ad esempio [!UICONTROL Vacation] e [!UICONTROL Time Off].</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Gestire i tipi di lavoro</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>L’ID è un indicatore alfanumerico associato a ogni oggetto in [!DNL Workfront]. Identifica in modo univoco ogni oggetto nel [!DNL Workfront] database. Puoi visualizzare l’ID di qualsiasi oggetto in un rapporto o un elenco per ogni oggetto. </p> <p>Suggerimento   <p>Puoi anche visualizzare l’ID nell’URL della pagina dell’oggetto. Ad esempio, l'ID di un progetto potrebbe avere un aspetto simile al numero indicato nel seguente URL, quando si accede alla pagina [!UICONTROL Dettagli progetto]:</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Singoli Obiettivi]</td> 
   <td>Singoli obiettivi che contribuiscono alle metriche degli obiettivi del team, ma non relativi allo sviluppo personale o della carriera.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Accesso ereditato di [!UICONTROL]</td> 
   <td>Funzione di condivisione che consente l'accesso per la propagazione da un oggetto a un altro. Ad esempio, l’accesso in eredità dell’utente del progetto definito nei record del programma e del portfolio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>In [!DNL Workfront Scenario Planner], è possibile suddividere un piano in più iniziative per facilitarne la gestione. <span>È possibile generare un report [!UICONTROL Initiative] e accedere alle informazioni [!UICONTROL Initiative] in un report [!UICONTROL Project].</span></p> <p>Il [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Il [!DNL Scenario Planner] panoramica</a>. </p> <p>Il [!DNL Initiative] non è visibile nel tuo [!DNL Workfront] a meno che la tua azienda non abbia acquistato un [!DNL Workfront Scenario Planner] licenza. Non è possibile accedere a [!UICONTROL Initiatives] tramite l'API.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role]</span> </td> 
   <td> <p><span>Il tipo di report [!UICONTROL Initiative Job Role] visualizza informazioni sulle mansioni associate a un'iniziativa del piano in [!DNL Workfront Scenario Planner].</span> </p> <p>Il [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md">Il [!DNL Scenario Planner] panoramica</a>. </p> <p><span>Questo tipo di rapporto non è visibile nel tuo [!DNL Workfront] a meno che la tua azienda non abbia acquistato un [!DNL Workfront Scenario Planner] licenza.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Hours]</span> </td> 
   <td> <p><span> In un report [!UICONTROL Initiative Job Role] (Ruolo iniziativa), questo mostra il numero di ore associate a una mansione in un'iniziativa.</span> </p> <p>Il [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md">Il [!DNL Scenario Planner] panoramica</a>. </p> <p>Questo campo e il tipo di report [!UICONTROL Initiative Job Role] non sono visibili nel [!DNL Workfront] a meno che la tua azienda non abbia acquistato un [!DNL Workfront Scenario Planner] licenza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Count]</td> 
   <td> <p>In un report [!UICONTROL Initiative Job Role] (Ruolo iniziativa), viene visualizzato il numero di una mansione specifica associata a un'iniziativa.</p> <p>Il [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md">Il [!DNL Scenario Planner] panoramica</a>. </p> <p>Questo campo e il tipo di report [!UICONTROL Initiative Job Role] non sono visibili nel [!DNL Workfront] a meno che la tua azienda non abbia acquistato un [!DNL Workfront Scenario Planner] licenza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Last Published Date]</td> 
   <td> <p>Un campo in un report [!UICONTROL Initiative], [!UICONTROL Initiative Job Role] e [!UICONTROL Project] visualizza la data dell'ultima pubblicazione di un'iniziativa di piano in un progetto. Puoi pubblicare iniziative per creare progetti o aggiornare progetti collegati alle iniziative.</p> <p>Il [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md">Il [!DNL Scenario Planner] panoramica</a>. </p> <p><span>Per informazioni sulle iniziative di pubblicazione, consulta</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Pubblicare scenari per creare e aggiornare i progetti in [!DNL Workfront Scenario Planner]</a>. Questo campo non è visibile nel [!DNL Workfront] a meno che la tua azienda non abbia acquistato un [!DNL Workfront Scenario Planner] licenza.</p> </td> 
  </tr> 
  <tr> 
   <td>Ricerca in linea in [!UICONTROL]</td> 
   <td>Ricerca eseguita durante la compilazione di un modulo per trovare le voci possibili per un campo specifico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interface Setup]</td> 
   <td>Area dell'applicazione che consente di definire visualizzazioni personalizzate, filtri, raggruppamenti, controlli elenco e così via.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL È L'Obiettivo Aziendale]</p></td> 
   <td> <p>In entrata [!DNL goal reports], visualizza un valore "[!UICONTROL True]/ [!UICONTROL False]" per ogni obiettivo strategico per indicare se l'organizzazione è assegnata all'obiettivo come proprietario. </p> 
   <p>Questo campo è visibile solo se l’organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sulla gestione degli obiettivi strategici tramite [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] panoramica </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue]</td> 
   <td> <p>Elemento di lavoro non pianificato che in genere indica che esiste un problema che impedisce il completamento di un'attività o di un progetto. Viene valutata e valutata per un ulteriore esame dell'impegno di lavoro</p> <p>Un [!UICONTROL Issue] può anche essere una richiesta [!UICONTROL Help Desk]. [!UICONTROL Change Orders], [!UICONTROL Requests] e [!UICONTROL Bugs] sono anche [!UICONTROL Issues].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Gestione problemi]</td> 
   <td> <p>Il processo e le regole che disciplinano la definizione dei tipi di problema e il processo di instradamento, valutazione o traffico associato a ciascun tipo.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Proprietario problema]</td> 
   <td>Il team o gli utenti responsabili della valutazione e del completamento di un problema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iterazione]</td> 
   <td>Periodo di tempo in cui un team produce un set predefinito di risultati finali.</td> 
  </tr> 
 </tbody> 
</table>

## J - L

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome Oggetto</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Ruolo]</td> 
   <td> <p>Utilizzato per identificare le funzioni lavorative e le responsabilità quotidiane di un utente. I ruoli possono essere assegnati agli elementi di lavoro per identificare l'abilità necessaria per completare un processo di lavoro senza assegnarla a un utente specifico. </p> <p>Un utente può avere più ruoli. Alcuni esempi includono Graphic Designer o Consultant.</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire le mansioni</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Voce Diario]</p> </td> 
   <td> <p>Oggetto segnalabile che fornisce informazioni sugli aggiornamenti di sistema per i campi tracciati visualizzati nell'area [!UICONTROL Aggiornamenti] di progetti, attività, problemi e altri oggetti.</p> <p>Per ulteriori informazioni, consulta <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Report sull'area [!UICONTROL Aggiornamenti]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Flag Kanban]</td> 
   <td> <p>In un report [!UICONTROL Attività] o in un report [!UICONTROL Problema], il campo [!UICONTROL Flag Kanban] visualizza lo stato del flag impostato sul brano nel [!UICONTROL Kanban Board]. I valori possibili sono [!UICONTROL On Track], [!UICONTROL Ready to Pull] e [!UICONTROL Is Blocked].</p> <p>Per ulteriori informazioni sull'impostazione dello stato del contrassegno per le storie sulla bacheca delle storie [!UICONTROL Kanban], vedere l'articolo <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Utilizza i flag nelle storie sulla bacheca [!UICONTROL Kanban]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI</td> 
   <td>Valore misurabile che dimostra l'efficacia con cui un'azienda raggiunge gli obiettivi aziendali chiave.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>Quantità di tempo che deve trascorrere dopo che l'attività predecessore [!UICONTROL Planned Completion Date] (Data di completamento pianificata) è passata fino a quando l'attività dipendente non può iniziare.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipi di Lag]</td> 
   <td> <p>Il metodo di calcolo del [!UICONTROL Lag]. Può essere:</p> 
    <ul> 
     <li>[!UICONTROL Days] (giorni lavorativi)</li> 
     <li>[!UICONTROL Calendar Days] (ignora festività)</li> 
     <li>[!UICONTROL Percent]</li> 
     <li>[!UICONTROL Day of Week]</li> 
    </ul> <p>Per ulteriori informazioni, consulta la sezione "[!UICONTROL Lag Types overview]" in <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Panoramica sui tipi di ritardo</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Miniatura Grande]</td> 
   <td> <p> In un elenco o report di [!UICONTROL Document] viene visualizzata un'anteprima del documento in una miniatura. </p> <p>Seleziona <strong>[!UICONTROL Miniatura Grande]</strong> per visualizzare una miniatura di 400 pixel nel rapporto.</p> <p>Le dimensioni della miniatura vengono regolate quando si modifica la larghezza della colonna in un elenco o in un report.</p> <p>Vedi anche "[!UICONTROL Thumbnail]" in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ultimi 10 Visualizzatori]</td> 
   <td> <p>In un elenco di rapporti, questo campo visualizza i nomi di un massimo di 10 utenti che hanno visualizzato il rapporto più di recente.<br>Per ulteriori informazioni sulle informazioni di utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizza utilizzo report</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Nota ultima condizione [!UICONTROL]</td> 
   <td> <p>In questo campo viene visualizzato l'ultimo aggiornamento immesso su un oggetto dal proprietario dell'oggetto. Si tratta dell'attività o dell'interazione più recente del proprietario su un oggetto.</p> <p>Il [!DNL Last Condition Note] Se il testo della nota dell'ultima nota di un oggetto è stato eliminato, la colonna è vuota. Una nuova nota immessa sull'oggetto diventa l'ultima nota e viene nuovamente visualizzata nella colonna. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ultima Data Aggiornamento Finanza]</td> 
   <td>In un report di [!UICONTROL project], questo campo acquisisce la data e l'ora dell'ultimo calcolo e aggiornamento dei dati finanziari del progetto. Per informazioni sulla situazione finanziaria dei progetti, consulta <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Panoramica sulle finanze dei progetti</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Note]</td> 
   <td> <p>In questo campo viene visualizzato l'ultimo aggiornamento immesso su un oggetto da qualsiasi utente. Questa è l’attività o interazione più recente su un oggetto.</p> <p>La colonna [!UICONTROL Ultima nota] è vuota se il testo dell'ultima nota di un oggetto è stato eliminato. Una nuova nota immessa sull'oggetto diventa l'ultima nota e viene nuovamente visualizzata nella colonna.</p>
   <p>Quando questo campo viene aggiunto a un report [!UICONTROL Task], vengono mantenuti tutti gli aggiornamenti sugli oggetti figlio, ad esempio problemi, sottoattività, documenti e così via. — dell'attività non viene visualizzato in questa colonna.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ultimo Visualizzato Da]</td> 
   <td> <p>In un elenco di rapporti, questo campo visualizza informazioni sull’ultimo utente che ha visualizzato il rapporto.<br>Per ulteriori informazioni sulle informazioni di utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizza utilizzo report</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ultima data di visualizzazione]</td> 
   <td> <p>In un elenco di report, questo campo visualizza la data dell'ultima visualizzazione del report.<br>Per ulteriori informazioni sulle informazioni di utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizza utilizzo report</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Modello di layout]</td> 
   <td>Definito dall’amministratore di sistema o dall’amministratore di gruppo per identificare le schede e i rapporti visualizzati nell’area di lavoro di un determinato utente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di layout]</td> 
   <td>Insieme alle visualizzazioni personalizzate di [!UICONTROL], il tipo di layout [!UICONTROL] specifica il tipo di visualizzazione personalizzata [!UICONTROL]. Attualmente, è disponibile solo l’elenco. In futuro, [!UICONTROL Detail] (la visualizzazione [!UICONTROL Detail] di un oggetto) potrebbe diventare disponibile.</td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Cost</i>. </p> </td> 
  </tr>
  --> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Hours</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Hours</i>. </p> <p>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        This field shows the number of hours budgeted for the project in the Legacy Resource Estimates area of the Business Case or in the Capacity Planner. 
       <br>If there&nbsp;are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.&nbsp; 
     </p> </td> </tr> -->
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.&nbsp;</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;&nbsp;</p>
    --> </td> 
  </tr> 
  <tr> 
   <!-- <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection&nbsp;of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività Library]</td> 
   <td>Modello per una singola attività utilizzato per fornire una denominazione coerente delle attività [!UICONTROL Tasks] e [!UICONTROL Template Tasks] nell'applicazione.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Type]</td> 
   <td>Tipo di licenza allocata a un [!UICONTROL Access Level]. È [!UICONTROL Full User], [!UICONTROL Limited User] o [!UICONTROL Requester].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Plan]</td> 
   <td> <p>In una visualizzazione o in un report di [!UICONTROL Group], questo campo mostra il numero massimo di licenze [!UICONTROL Plan] che possono essere assegnate agli utenti che hanno il rispettivo gruppo designato come proprio [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Work]</td> 
   <td> <p>In una visualizzazione o in un report di [!UICONTROL Group], questo campo mostra il numero massimo di licenze [!UICONTROL Work] che possono essere assegnate agli utenti che hanno il rispettivo gruppo designato come proprio [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limited User]</td> 
   <td>Un tipo di licenza che consente la creazione di un [!DNL Access Level] che contiene privilegi di sola visualizzazione, con la possibilità di inviare problemi, immettere note e caricare documenti.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL List Controls]</td> 
   <td> <p>Parte di [!UICONTROL Interface Setup] che consente di collegare filtri, viste e raggruppamenti personalizzati a singoli utenti o a livello globale a tutti gli utenti.</p> </td> 
  </tr> 
 </tbody> 
</table>

## M - O

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome Oggetto</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Solo Manuale]</td> 
   <td> <p>Uno dei [!UICONTROL Tipi di aggiornamento] di un progetto [!UICONTROL]. Questa impostazione consente di aggiornare le timeline di [!UICONTROL Project Projected] e [!UICONTROL Planned] solo quando si fa clic su "[!UICONTROL Recalculated Timelines]". I progetti impostati in questo modo verranno ignorati durante il processo di ricalcolo leggero e quando il progetto o l'attività nel progetto vengono aggiornati.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleziona il progetto [!UICONTROL Update Type] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>Si riferisce all’utente attualmente connesso. </p> <p>È consigliabile utilizzare questo campo in un filtro per rendere i rapporti più generici quando vengono condivisi con altri utenti. In questo modo, puoi creare un solo rapporto che visualizzerà informazioni diverse a seconda di chi effettua l’accesso per visualizzarle, poiché queste sono sempre personalizzate per l’utente connesso. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Max Utenti]</td> 
   <td> <p>Questo è un campo obsoleto. Qualsiasi informazione visualizzata in questo campo è correlata a una funzione [!DNL Workfront] è stato rimosso e non è possibile aggiornare il campo. </p> <p>Nelle versioni precedenti di [!DNL Workfront], è possibile aggiornare questo campo durante la creazione o la modifica di una mansione. Viene visualizzato il numero totale di utenti che possono essere associati a un ruolo in ciascun progetto. Un valore pari a zero è consentito per un numero illimitato di utenti che possono essere assegnati a un progetto. </p>Il campo rimane visibile in alcuni report ed elenchi, ma non è possibile aggiornare le informazioni visualizzate. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone]</td> 
   <td> <p>Indicatore che è possibile associare a un'attività per indicare che un punto chiave del progetto è stato raggiunto al completamento dell'attività. In genere, è possibile utilizzare le milestone per mostrare un evento significativo, ad esempio il completamento di una fase del progetto o di una serie di attività critiche. Le [!UICONTROL Milestones] sono in genere associate alle attività padre. È necessario creare le milestone prima di allegarle alle attività. Per informazioni sulle milestone, vedi <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Creare un percorso milestone</a> e <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Associa attività cardine ad attività</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percorso Milestone]</td> 
   <td>Una raccolta di [!UICONTROL milestones]. I [!UICONTROL Milestone Paths] (Percorsi milestone) vengono utilizzati nei progetti per distinguere i progetti con determinati tipi di [!UICONTROL Milestones] dai progetti con un diverso set di [!UICONTROL Milestones].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Attività Milestone]</td> 
   <td>Attività contrassegnata per indicare un evento da segnalare da misurare.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Module]</td> 
   <td>Un singolo passaggio in uno scenario in [!DNL Workfront Fusion] che esegue alcune funzioni in base all’app associata.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Il Mio Ruolo Principale]</td> 
   <td> <p>Nei filtri viene fatto riferimento a questo elemento. Vengono visualizzati gli utenti che hanno lo stesso [!UICONTROL Primary Role] dell'utente connesso o gli elementi di lavoro assegnati al [!UICONTROL Primary Role] dell'utente connesso.</p> <p>È consigliabile utilizzare questo campo in un filtro per rendere i rapporti più generici quando vengono condivisi con altri utenti. In questo modo, puoi creare un solo rapporto che visualizzerà informazioni diverse a seconda di chi effettua l’accesso per visualizzarle, poiché queste sono sempre personalizzate per l’utente connesso. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Il Mio Team Predefinito]</td> 
   <td> <p>Nei filtri viene fatto riferimento a questo campo per visualizzare gli utenti che appartengono al [!UICONTROL Home Team] dell'utente connesso o gli elementi di lavoro assegnati al [!UICONTROL Home Team] dell'utente connesso. </p> <p>È consigliabile utilizzare questo campo in un filtro per rendere i rapporti più generici quando vengono condivisi con altri utenti. In questo modo, puoi creare un solo rapporto che visualizzerà informazioni diverse a seconda di chi effettua l’accesso per visualizzarle, poiché queste sono sempre personalizzate per l’utente connesso. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Convenzione di denominazione]</td> 
   <td>Un insieme di regole a livello di organizzazione che utilizza i dati per creare nomi di progetti, attività e risultati finali.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Integrazione Nativa]</td> 
   <td>Un’integrazione che non richiede alcuna codifica manuale o configurazione API. Definita anche integrazione "predefinita".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Menu Di Navigazione]</td> 
   <td>Pannello superiore centrale dell'applicazione che include collegamenti alle aree principali di [!UICONTROL Workfront].</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL Valore Nuovo Numero]</td> 
   <td>In un report [!UICONTROL Voce diario] viene visualizzato il valore aggiornato di un campo che sostituisce il [!UICONTROL Vecchio valore numerico].
   Per ulteriori informazioni, consulta "[!UICONTROL Old Number Value]" in questo articolo.</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Giorno Non Feriale]</td> 
   <td>Giorno non assegnato al completamento di alcuna assegnazione. Di solito si tratta di un giorno di vacanza, di una vacanza o di un weekend.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note]</td> 
   <td>Un commento o un aggiornamento effettuato su [!DNL Workfront] oggetto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testo Nota]</td> 
   <td> <p>In questo modo viene visualizzato il testo di un aggiornamento immesso da un utente su qualsiasi oggetto. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Numero di obiettivi collegati]</td> 
   <td> <p>In un report [!UICONTROL Project] indica il numero di obiettivi strategici associati al progetto. Per informazioni sull’associazione dei progetti agli obiettivi strategici, consulta <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Aggiungere progetti agli obiettivi in  [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>Per informazioni sugli obiettivi strategici, consulta anche "[!UICONTROL Goal]" in questo articolo.</p> 
   <p>Questo campo è visibile solo se l’organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sulla gestione degli obiettivi strategici tramite [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Aggiungere progetti agli obiettivi in [!UICONTROL Obiettivi Adobe Workfront]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object]</td> 
   <td> <p>Informazioni visualizzate in [!DNL Adobe Workfront] è rappresentato da oggetti archiviati in [!DNL Workfront] database. Gli oggetti sono ciò che guida le informazioni in Workfront. Alcuni esempi di oggetti sono:</p> 
    <ul> 
     <li>[!UICONTROL Portfoli]</li> 
     <li>[!UICONTROL Programmi]</li> 
     <li>[!UICONTROL Progetti]</li> 
     <li>[!UICONTROL Attività]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documenti]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>Rapporti di [!UICONTROL]</li> 
     <li>[!UICONTROL Groups]</li> 
     <li>[!UICONTROL Teams]</li> 
     <li>[!UICONTROL Utenti]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Moduli personalizzati]</li>
     <li>[!UICONTROL Campi personalizzati]</li>  
     <li>[!UICONTROL Hours]</li> 
     <li>[!UICONTROL Tariffe di fatturazione]</li> 
     <li>[!UICONTROL Modelli]</li> 
     <li>[!UICONTROL Attività modello]</li>

<p><b>NOTA</b></p>
  <p>Non si tratta di un elenco completo. </p>

</ul> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Comprendere gli oggetti in [!UICONTROL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipi di oggetto]</td> 
   <td>Se si crea un report o un elenco contenente tutti i moduli personalizzati, è possibile utilizzare questo campo come visualizzazione o filtro per visualizzare i tipi di oggetto associati a ogni modulo. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Vecchio Valore Numerico]</td> 
   <td>In un report [!UICONTROL Voce diario] viene visualizzato il valore originale di un campo prima che sia stato aggiornato. Una volta aggiornato, il valore di un campo viene visualizzato come [!UICONTROL Nuovo valore numerico] in un report [!UICONTROL Voce diario]. Per ulteriori informazioni, vedere anche "[!UICONTROL Nuovo valore numerico]".</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Solo Su Modifica]</td> 
   <td> <p>Uno dei tipi [!UICONTROL Project Update]. Quando questa opzione è selezionata, le timeline [!UICONTROL Project Projected] (Progetto previsto) e [!UICONTROL Planned] (Pianificato) vengono aggiornate solo quando viene effettuato un aggiornamento o una modifica al progetto o a un'attività all'interno del progetto. Non aggiorna il progetto ogni notte.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleziona il tipo di aggiornamento del progetto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Operazione]</td> 
   <td> <p>Il nome di [!UICONTROL Issue] nel [!DNL Workfront] database, utilizzato nei report in modalità testo o nei dati personalizzati calcolati.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL aperto]</td> 
   <td>Un problema o un'attività che non è stata completata ma su cui si sta lavorando.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organigramma]</td> 
   <td>Abbreviazione di Organizational Chart (Grafico organizzativo). Questo è un grafico che mostra la gerarchia di un’organizzazione. Si trova anche nella scheda della schermata di dettaglio [!UICONTROL User] che visualizza e consente di impostare le relazioni [!UICONTROL Company] e [!UICONTROL Reporting] dell'utente [!UICONTROL User].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Impostazione organizzazione]</td> 
   <td>Definisce [!UICONTROL Companies], [!UICONTROL Groups] e [!UICONTROL Security Profiles] per la tua organizzazione.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Altri Gruppi]</td> 
   <td> <p>In un report o in una visualizzazione che elenca gli utenti, questo campo visualizza tutti i gruppi di cui ogni utente è membro. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Sovrascrivi valuta]</span> </td> 
   <td> 
    <div> 
     <p>In un report [!UICONTROL Ruolo], questa è la valuta associata a una mansione. Si tratta di un override di [!UICONTROL Base Currency] come stabilito nell'area [!UICONTROL Setup] da [!DNL Workfront] amministratore. </p> 
     <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire le mansioni</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Sostituisci valuta fatturazione/ora]</span> </td> 
   <td> 
    <div> 
     <p>In un rapporto di [!UICONTROL Ruolo], corrisponde alla tariffa oraria di fatturazione della mansione che utilizza la [!UICONTROL Override Currency] selezionata della mansione.</p> 
     <p> Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire le mansioni</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Sostituisci Costo valuta/Ora]</span> </td> 
   <td> 
    <div> 
     <p>In un report [!UICONTROL Ruolo], indica la tariffa oraria del costo della mansione che utilizza la [!UICONTROL Override Currency] selezionata della mansione. </p> 
     <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire le mansioni</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Proprietario]</td> 
   <td>Utente responsabile del completamento dell'oggetto designato.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Tipo proprietario]</span> </td> 
   <td> 
    <div> 
     <p>In un report [!UICONTROL Goal] viene visualizzato il tipo di proprietario assegnato a un obiettivo strategico. Di seguito sono riportati i tipi di proprietario dell'obiettivo:</p> 
     <ul> 
      <li> <p>[!UICONTROL Utente]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL Group]</p> </li> 
     </ul> 
     <p>In questo campo non viene visualizzato alcun valore se il proprietario dell’obiettivo è la tua organizzazione. </p> 
     <p>È necessaria una licenza aggiuntiva. Per informazioni su [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] panoramica</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## P - R

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome Oggetto</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Parameter]</td> 
   <td> <p>Un parametro [!UICONTROL] è un campo personalizzato. Puoi creare un rapporto per tutti i parametri o campi personalizzati nel tuo sistema. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL padre]</td> 
   <td>In un report, questo campo mostra informazioni sull'elemento padre dell'oggetto. In un report [!UICONTROL issue], ad esempio, è possibile che vengano visualizzate informazioni sull'attività o sul progetto in cui è registrato il problema. In un report attività è possibile che vengano visualizzate informazioni sull'attività padre diretta o sul progetto. Per ulteriori informazioni sugli oggetti con elementi padre in [!DNL Workfront], vedere la sezione "Interdipendenza e gerarchia degli oggetti" nell'articolo <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Comprendere gli oggetti in [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag Genitore]</td> 
   <td>Il tempo che deve trascorrere tra l'inizio dell'attività padre [!UICONTROL] e l'inizio dell'attività secondaria [!UICONTROL].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività Padre]</td> 
   <td>Nota anche come attività di riepilogo [!UICONTROL]. Si tratta di un'attività con sottoattività (dette anche [!UICONTROL Children Tasks]). La [!UICONTROL Duration], [!UICONTROL Work Required] e [!UICONTROL Percent Complete] dell'attività padre viene calcolata a partire dalle sottoattività.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Risorse Part-Time]</td> 
   <td>Utente concesso in licenza con capacità inferiore alla pianificazione predefinita definita nel sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percent Complete]</td> 
   <td> <p>Campo relativo a un progetto, un'attività o un problema che mostra la percentuale di completamento del lavoro associato all'attività, al progetto o al problema.</p> <p>È possibile aggiornare questo campo manualmente per problemi e attività di lavoro. </p> <p>Per i progetti e le attività padre, questo campo è un riepilogo di tutte le attività in esecuzione e non è possibile aggiornarlo manualmente. </p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Panoramica del progetto [!UICONTROL Percent Complete]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permission]</td> 
   <td> <p>Diritti concessi a un utente su un oggetto, in genere assegnati in modo che possa completare il lavoro sull'elemento o visualizzarlo. Puoi concedere autorizzazioni a:</p> 
    <ul> 
     <li>[!UICONTROL Progetti]</li> 
     <li>[!UICONTROL Attività]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Portfoli]</li> 
     <li>[!UICONTROL Programmi]</li> 
     <li>Rapporti di [!UICONTROL]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Documenti]</li> 
     <li>[!UICONTROL Custom Forms]</li> 
     <li>Visualizzazioni di [!UICONTROL]</li> 
     <li>[!UICONTROL Filters]</li> 
     <li>[!UICONTROL Raggruppamenti]</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Panoramica delle autorizzazioni di condivisione sugli oggetti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]</td> 
   <td> <p>Si tratta di un tipo di licenza completo nel [!DNL Workfront] di rete. Gli utenti devono disporre di questo per accedere a tutte le funzioni in [!DNL Workfront].</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] panoramica sulle licenze</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan] (nel [!DNL Scenario Planner])</td> 
   <td> <p>Un piano è l'oggetto principale quando si lavora con [!DNL Workfront] Pianificazione scenario. Puoi delineare la strategia per il futuro a breve e lungo termine della tua azienda, identificare ogni risultato di alto livello e aggiungerlo come piano alla [!DNL Workfront] Pianificazione scenario. </p> <p>Impossibile visualizzare [!DNL Scenario Planner] piani in un rapporto e non è possibile accedervi tramite il [!DNL Workfront] API. </p> <p>Il [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md">Il [!DNL Scenario Planner] panoramica</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pianificato]</td> 
   <td> <p>L’intervallo di tempo entro il quale è pianificato un evento. Quando crei progetti, attività o problemi in [!DNL Workfront], stabilisci le date di inizio e fine pianificate, nonché l’arco temporale pianificato durante il quale si verificano. Questi valori rappresentano l'intenzione originale o la stima del tempo necessario per il completamento di un elemento. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Benefit]</td> 
   <td>Si tratta di un inserimento manuale che consente al project manager di valutare se il completamento di un progetto comporterebbe un beneficio monetario per l'organizzazione. La specifica di questo valore può essere utile per creare un [!UICONTROL Business Case] per il progetto. Per aggiornare questo valore è necessario disporre delle autorizzazioni [!UICONTROL Manage] per il progetto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Ore Preventivate]</td> 
   <td> <p>In un rapporto di [!UICONTROL Ore preventivate] viene visualizzata la quantità di ore preventivate per i progetti o [!UICONTROL Ruoli] in [!UICONTROL Resource Planner]. </p> <p>Per informazioni sulla definizione del budget di progetti o ruoli in [!UICONTROL Resource Planner], vedere l'articolo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Preventivare le risorse in [!UICONTROL Resource Planner] utilizzando le viste [!UICONTROL Project] e [!UICONTROL Role]</a>. Per informazioni sul report [!UICONTROL Ore preventivate], vedi l'articolo <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Ore preventivate</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di completamento Pianificata]</td> 
   <td> <p>È possibile impostare manualmente [!UICONTROL Planned Completion Date] (Data di completamento pianificata) a una data a scelta. Se non imposti [!UICONTROL Planned Completion Date] (Data di completamento pianificata), [!DNL Workfront] la imposta automaticamente. Se impostata automaticamente, la [!UICONTROL Planned Completion Date] è: [!UICONTROL Planned Start Date] + [!UICONTROL Duration]</p> <p>Per ulteriori informazioni, consulta i seguenti articoli:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Panoramica dell'attività [!UICONTROL Data di completamento pianificata]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Imposta il progetto [!UICONTROL Planned Completion Date]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo Pianificato]</td> 
   <td> <p>Un totale di [!UICONTROL Planned Labor Cost] e [!UICONTROL Planned Expense Cost] del progetto. Questo valore non include [!UICONTROL Planned Risk Cost] nel progetto.  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration]</td> 
   <td> <p>La [!UICONTROL Planned Duration] di un'attività corrisponde in genere alla [!UICONTROL Planned Duration] dell'attività. Rappresenta la differenza in giorni tra il [!UICONTROL Planned Start] (Inizio pianificato) e il [!UICONTROL Planned Completion Dates] (Date di completamento pianificate) dell'attività. </p> <p>Quando l'attività ha un tipo [!UICONTROL Duration] di [!UICONTROL Effort Driven], la [!UICONTROL Planned Duration] può differire dalla [!UICONTROL Duration] dell'attività, in base al numero di risorse assegnate all'attività. </p> <p>Ad esempio, se un'attività con un tipo [!UICONTROL Duration] di [!UICONTROL Effort Driven] ha una [!UICONTROL Duration] di 3 giorni e si assegna all'attività una risorsa con una pianificazione a tempo pieno, anche la [!UICONTROL Planned Duration] sarà di 3 giorni. Se si assegnano tre risorse con una pianificazione a tempo pieno alla stessa attività, la [!UICONTROL Durata] rimane 3 giorni, ma la [!UICONTROL Durata pianificata] diventa 1 giorno. Con [!UICONTROL Planned Duration] (Durata pianificata) vengono modificate anche le date di [!UICONTROL Planned Start] (Inizio pianificato) e [!UICONTROL Planned Completion] (Completamento pianificato) dell'attività, in modo da riflettere la nuova [!UICONTROL Planned Duration] (Durata pianificata). Di conseguenza, anche la timeline del progetto ne risente. </p> <p>Per ulteriori informazioni sulla differenza tra [!UICONTROL Duration] e [!UICONTROL Planned Duration] per le attività, vedi l'articolo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Differenza tra [!UICONTROL Planned Duration] e [!UICONTROL Duration] per le attività</a>.</p> <p>I progetti e i problemi non hanno una [!UICONTROL Planned Duration]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Minuti di Durata Pianificati]</td> 
   <td> <p>La [!UICONTROL Planned Duration Minutes] di un progetto o di un problema è la [!UICONTROL Duration] del progetto o del problema in minuti. </p> <p>Le attività non hanno un campo [!UICONTROL Planned Duration Minutes] (Minuti di durata pianificati). </p> <p>Le attività modello di [!UICONTROL] hanno un campo [!UICONTROL Planned Duration Minutes] che visualizza il campo [!UICONTROL Planned Duration] dell'attività in minuti. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo Spesa Pianificato]</td> 
   <td> <p>Somma degli [!UICONTROL Planned Amount] per tutte le spese registrate per un progetto o un'attività.</p> <p><b>ESEMPIO</b></p>
   <p>Se si crea una spesa per l'attività 1 e si immettono 600,00 $ nel campo [!UICONTROL Importo pianificato], il costo [!UICONTROL Costo spese pianificato] per questa attività è 600,00 $. </p> 
   <p>Per un progetto, [!DNL Workfront] utilizza la formula seguente per calcolare [!UICONTROL Planned Expense Cost]:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lavoro Necessario]</td> 
   <td> <p>Questo campo viene visualizzato nelle aree [!UICONTROL progetti], [!UICONTROL attività] e problemi, nei report per progetti, attività o problemi e negli strumenti di gestione delle risorse come [!UICONTROL Resource Planner], [!UICONTROL Workload Balancer] e il report [!UICONTROL Utilization]. </p> <p>Mostra il numero di ore che, secondo le stime del Proprietario del progetto, devono essere necessarie per completare ogni attività o problema. Per i progetti, si tratta in genere di un riepilogo delle [!UICONTROL Lavoro Necessario] delle attività del progetto. </p> <p>Nel campo [!UICONTROL Planned Hours] (Ore pianificate) possono essere visualizzate informazioni diverse a seconda dell'origine di visualizzazione. Per informazioni sulle ore pianificate, vedi <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Panoramica sulle ore pianificate</a>.</p> <p>Le ore pianificate vengono memorizzate in minuti nel [!DNL Workfront] database. Quando scrivi calcoli utilizzando questo campo, assicurati di tenere conto del fatto che le ore vengono visualizzate in minuti.<br></p> <p>Per impostazione predefinita, le ore pianificate vengono distribuite in modo uniforme a tutti i giorni all'interno della durata di un elemento di lavoro e anche in modo uniforme per tutte le risorse assegnate all'attività. Gli utenti possono aggiornare la quantità giornaliera di ore pianificate per un elemento di lavoro o le singole ore pianificate per ciascun assegnatario.</p> <p>L’aggiornamento di questo campo è diverso per progetti, attività e problemi: </p> 
    <ul> 
     <li> <p>Per i problemi, puoi aggiornare manualmente questo campo. Le ore pianificate del problema non vengono aggiunte alle ore pianificate del progetto. </p> <p>Suggerimento: in un report sui problemi, uno dei campi [!UICONTROL Lavoro pianificato] viene sostituito dal campo [!UICONTROL Lavoro]. Nel campo viene visualizzato il numero di ore pianificate per il problema. Per ulteriori informazioni, vedere i campi "lavoro" o "[!UICONTROL Lavoro]" in questa tabella. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>Per le attività, è possibile aggiornare manualmente questo campo quando il [!UICONTROL Tipo di Durata] dell'attività è [!UICONTROL Assegnazione Calcolata] o [!UICONTROL Semplice]. Questo campo viene calcolato da [!DNL Workfront] quando il tipo di durata [!UICONTROL] dell'attività è [!UICONTROL Lavoro calcolato] o [!UICONTROL Impegno guidato].<br>Per informazioni su [!UICONTROL Task Duration], vedere l'articolo <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica dell'attività [!UICONTROL Duration] e [!UICONTROL Duration Type]</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Per i progetti: [!DNL Workfront] calcola le ore pianificate aggiungendo tutte le ore pianificate da tutte le attività del progetto. </p> </li> 
    </ul> <p><b>SUGGERIMENTO</b></p> <p>È possibile visualizzare [!UICONTROL Planned Hours] nei report [!UICONTROL project], [!UICONTROL task] o [!UICONTROL issues] anche utilizzando la modalità testo e facendo riferimento a campi aggiuntivi. Per ulteriori informazioni, consulta la sezione "<code>work</code>", "[!UICONTROL Work]" e "<code>workRequiredExpression</code>" in questa tabella. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo Lavoro Pianificato]</td> 
   <td> 
    <p>Per un'attività, la tariffa oraria dell'utente o del ruolo moltiplicata per il numero di ore assegnate all'utente o al ruolo.</p> <p>Per un progetto, rappresenta un totale di tutti [!UICONTROL Costi manodopera pianificata] di tutte le attività.</p> <p>L'utilizzo della tariffa dell'utente o del ruolo dipende dal tipo di costo selezionato per l'attività specificata. </p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/track-costs.md">Tracciare i costi</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reddito Pianificato]</td> 
   <td> <p>Nelle attività e nei progetti è possibile visualizzare un valore per [!UICONTROL Planned Revenue] (Ricavi pianificati) in [!DNL Workfront]. [!UICONTROL Planned Revenue] rappresenta la quantità di denaro associata alle [!UICONTROL Planned Hours] delle attività sul progetto. Per i progetti, può anche includere il [!UICONTROL Fixed Revenue] del progetto. </p> <p>Per le attività, si tratta dei ricavi associati alle [!UICONTROL Lavoro Necessario] delle attività. Le ore pianificate da tutte le attività vengono riportate alle ore pianificate del progetto per contribuire al calcolo del progetto [!UICONTROL Lavoro pianificato]. </p> 
   <p>[!DNL Workfront] calcola il ricavo pianificato di [!UICONTROL] per le attività e i progetti utilizzando le formule seguenti:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>Il progetto [!UICONTROL Planned Revenue] (Ricavi pianificati) visualizzato nell'area [!UICONTROL Project Details] (Dettagli progetto) e nei report del progetto è diverso dal progetto Planned Revenue (Ricavi pianificati) visualizzato nel report [!UICONTROL Utilization] (Utilizzo). </p> <p>Il campo [!UICONTROL Planned Revenue] (Ricavi pianificati) nell'area [!UICONTROL Project Details] (Dettagli progetto) riflette i ricavi dell'attività e quelli fissi del progetto. Nel rapporto Utilizzo di [!UICONTROL Planned Revenue] (Ricavi pianificati) di [!UICONTROL Planned Revenue] (Ricavi pianificati) viene visualizzato [!UICONTROL Planned Revenue] (Ricavi pianificati) associato solo alle attività del progetto. </p> 
     <p><b>ESEMPIO</b></p>  
      <p>Se il progetto ha 1 attività con 10 ore, assegnata a un consulente con una tariffa oraria di $ 20 e il progetto ha un importo di $ 100 [!UICONTROL Fixed Revenue], il rapporto Utilizzo [!UICONTROL] visualizza $ 200 per il ricavo pianificato [!UICONTROL Planned Revenue] (il ricavo pianificato [!UICONTROL] associato alle ore dell'attività). La sezione [!UICONTROL Dettagli progetto] visualizza $ 300 (il [!UICONTROL Ricavi pianificati] dall'attività e il Ricavo fisso per il progetto). </p> 
    <p>Per informazioni sul tracciamento dei ricavi in [!DNL Workfront] vedi <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Panoramica su fatturazione e ricavi</a>. </p> 
    <p>Per informazioni sui calcoli di [!UICONTROL Planned Revenue] nel report sull'utilizzo di [!UICONTROL], vedere <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Visualizza informazioni sull'utilizzo delle risorse </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo Rischio Pianificato]</td> 
   <td> <p>Totale del [!UICONTROL Costo Potenziale] di tutti i rischi sul progetto, tenendo conto della loro Probabilità che si verifichi. Questo importo non è incluso nel [!UICONTROL Planned Cost] del progetto.</p> <p>Il [!UICONTROL Planned Risk Cost] di un progetto viene calcolato con la seguente formula:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Profile]</td> 
   <td>Un insieme di schede e sezioni portale definito dall'amministratore che viene visualizzato sul [!DNL Workfront] Applicazione [!UICONTROL Home] e altre dashboard.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Section]</td> 
   <td>Un componente di una scheda su una dashboard o pagina portale. Di solito un singolo report, grafico, calendario o elenco di informazioni chiave.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Tab]</td> 
   <td>Scheda di un portale o di un dashboard contenente fino a tre sezioni portale.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfoli]</td> 
   <td> <p>Una raccolta di progetti che hanno caratteristiche unificanti. Questi progetti in genere competono per le stesse risorse, budget o fasce orarie. È possibile suddividere i Portfoli in Programmi e associare i progetti ai Programmi prima che vengano aggiunti a un Portfolio.</p> <p>Per ulteriori informazioni sui portfolio, consulta <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Panoramica del Portfolio in [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Gestione Portfoli]</td> 
   <td>Un’area pratica incentrata sulla gestione di una raccolta o di programmi correlati e sulle attività di progetto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfoli Optimizer]</td> 
   <td>A [!DNL Workfront] strumento di assistenza nella valutazione e nella definizione delle priorità dei progetti all’interno di un portfolio.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Proprietario Portfolio]</td> 
   <td>Il soggetto interessato responsabile della definizione delle priorità e del budget per un portfolio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Costo Rischio Potenziale]</td> 
   <td>Questo è un campo del progetto che è possibile individuare in elenchi e report. Mostra il costo potenziale per i rischi associati al progetto, qualora si verifichino. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcola costo rischio potenziale </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Predecessore]</td> 
   <td> <p>Attività che deve essere completata prima del completamento di un'attività dipendente. È anche un'attività contrassegnata come dipendenza [!UICONTROL] per un'altra attività. I predecessori consentono al planner di impostare la logica di dipendenza dalla sequenza, ad esempio di avviare un'attività al termine di un'altra attività.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Panoramica dei predecessori delle attività</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL società principale]</td> 
   <td>L’azienda a cui appartiene l’utente indicata nelle impostazioni utente. Le aziende possono anche essere associate ai progetti.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contatto primario]</td> 
   <td><p>Il [!UICONTROL Contatto principale] è l'autore di un problema ed è automaticamente designato da [!DNL Workfront] quando l'utente crea il problema. Puoi aggiornare manualmente questo campo se [!DNL Manage] autorizzazioni per il problema. Un problema può avere un solo contatto principale.</p> 
   <p>Se modifichi il contatto principale, l’utente originariamente designato come contatto principale disporrà ancora dell’accesso [!UICONTROL Manage] al problema.</p>
   <p>Quando si converte un problema in un'attività o in un progetto, l'utente designato come [!UICONTROL Contatto principale] di diventa il [!UICONTROL Converted Issue Originator] del progetto o dell'attività. Se il [!UICONTROL Contatto primario] del problema viene aggiornato dopo la conversione del problema, il [!UICONTROL Convertted Issue Originator] verrà mantenuto come [!UICONTROL Contatto primario] del problema nel momento in cui si è verificata la conversione. Vedi anche "[!UICONTROL Converted Issue Originator]" in questo articolo.</p> 
   </td> 
  </tr>
  <tr> 
   <td>Priorità [!UICONTROL]</td> 
   <td>Valore che può essere assegnato a un'attività, una questione o un progetto per specificarne l'importanza. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Privato]</td> 
   <td>In un [!UICONTROL Note] o in un [!UICONTROL Document], questa opzione rende l'oggetto nascosto alla maggior parte dei visualizzatori. Per una coda di helpdesk privata, solo gli utenti del team di coda possono inviare i problemi a tale coda tramite l'area [!UICONTROL Help Desk].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profile]</td> 
   <td>Tutte le informazioni su un account utente.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Program]</td> 
   <td> <p>Un sottogruppo all’interno di un portfolio, in cui progetti simili possono essere raggruppati per ottenere un beneficio ben definito.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Management]</td> 
   <td>Gestione delle dipendenze, dei rischi, dei problemi, dei requisiti e delle soluzioni tra progetti per mantenere sano il programma e ottenere i vantaggi definiti dal programma.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Proprietario del programma]</td> 
   <td>Le parti interessate responsabili della supervisione e dell’organizzazione delle attività per garantire che gli obiettivi del progetto siano in linea con gli obiettivi aziendali.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Avanzamento]</span> </td> 
   <td> <p>In un rapporto di [!UICONTROL Goal] (Obiettivo), questa mostra la percentuale di completamento di un obiettivo strategico. La percentuale di avanzamento viene visualizzata sotto forma di numero. Per informazioni sugli obiettivi strategici, consulta anche "[!UICONTROL Goal]" in questa tabella.</p> <p>Questo campo è visibile solo se l’organizzazione ha acquistato [!DNL Workfront] Obiettivi. Per informazioni sulla gestione degli obiettivi strategici tramite [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> Aggiungere progetti agli obiettivi in [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>Stato di avanzamento di [!UICONTROL]</td> 
   <td> <p>In un report Progetto, Attività e Obiettivo questo campo visualizza lo Stato di avanzamento di progetti, attività o obiettivi strategici. Per ulteriori informazioni, consulta i seguenti articoli:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Panoramica sullo stato di avanzamento del progetto</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Panoramica sullo stato di avanzamento dell’attività</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Panoramica dell’avanzamento e della condizione dell’obiettivo in [!DNL Adobe Workfront Goals]</a> </p>
     <p>Il rapporto [!UICONTROL Goal] e lo stato di avanzamento [!UICONTROL] per [!DNL goals] sono visibili solo se l'organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sugli obiettivi strategici in [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] panoramica</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>Progetto [!UICONTROL]</td> 
   <td> <p>Una grande quantità di lavoro che deve essere completata in un arco temporale specifico e deve utilizzare un budget specifico e un numero specifico di risorse. Per renderlo gestibile, il progetto viene suddiviso in una serie di attività. Il completamento di tutte le attività comporta il completamento del progetto. Per informazioni sulla pianificazione di un progetto, consulta <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Pianificare una panoramica del progetto</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ore pianificate assegnazione progetto]</td> 
   <td> <p>In un report [!UICONTROL Initiative Job Role] (Ruolo iniziativa) viene visualizzato il numero di [!UICONTROL Planned Hours] (Ore pianificate) associato a una mansione assegnata ad attività o problemi nel progetto. Questo campo e il tipo di report [!UICONTROL Initiative Job Role] non vengono visualizzati nel [!DNL Workfront] a meno che la tua azienda non abbia acquistato un [!DNL Workfront Scenario Planner] licenza. Per informazioni su [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md">Il [!DNL Workfront Scenario Planner] panoramica</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dettagli progetto]</td> 
   <td>Dettagli dello stato corrente di un progetto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo preventivato progetto]</td> 
   <td> <p> Questo è il [!UICONTROL Budgeted Cost] di un progetto visualizzato in elenchi e report.</p><p>Vedi anche "[!UICONTROL Costo preventivato]" in questo articolo.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Project Management]</td> 
   <td>Un insieme di criteri che definisce le soglie per la creazione, la categorizzazione e la denominazione dei progetti.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Spese Fisse Del Progetto]</td> 
   <td>In un report [!UICONTROL Hour], questo campo è riservato alle informazioni finanziarie associate alle ore registrate con il tipo di ora [!UICONTROL Project Time]. I progetti possono avere proprie tariffe di fatturazione e se un’ora viene registrata direttamente su un progetto, tali tariffe verranno utilizzate nei calcoli. In base alle impostazioni del progetto, i progetti possono anche avere valute diverse ed è possibile effettuare una conversione di valuta per tali ore. L'oggetto [!UICONTROL Project Overhead] consente [!DNL Workfront] per ottenere quelle informazioni.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proprietario Progetto]</td> 
   <td>Utente responsabile della gestione dell'ambito, della sequenza temporale e delle assegnazioni di un progetto. Autorizzatore predefinito per gli ordini di modifica, le modifiche finanziarie e i deliverable.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pianificazione progetto]</td> 
   <td>Processi per sviluppare e gestire la pianificazione del progetto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sponsor Progetto]</td> 
   <td>Un profilo di parti interessate a cui ciascuno degli utenti deve riferirsi. In entrata [!DNL Workfront], questi sono designati come [!UICONTROL Access Levels]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team di progetto]</td> 
   <td> <p>Insieme di utenti o ruoli assegnati a un progetto</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Panoramica del team del progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tracciamento progetto]</td> 
   <td>Dati utilizzati per misurare lo stato e l'ambito di un progetto</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Previsto]</td> 
   <td> <p>Stima della marca temporale del completamento del lavoro in base alle ore pianificate e alla percentuale di completamento di un'attività, un problema o un progetto.</p> <p>Si riferisce alle date o alla [!UICONTROL Duration] di attività, problemi o progetti. In genere, vengono indicate date e durate più adatte alla vita degli elementi di lavoro, dopo che un lavoro è già stato completato o dopo che è trascorso un certo periodo di tempo. </p> <p>Ad esempio, [!UICONTROL Data di completamento prevista] di un'attività è la data in cui [!DNL Workfront] stima il completamento dell'attività in base alla quantità di lavoro svolto, al numero di persone assegnate e al tempo trascorso dalla data di inizio.</p> </td> 
  </tr> 
  <tr> 
   <td>Scadenza bozza [!UICONTROL]</td> 
   <td> <p>Nei report che contengono l'oggetto [!UICONTROL Document Version], ad esempio un report [!UICONTROL Document Version] e un report [!UICONTROL Proof Approval], questo campo visualizza il giorno della settimana, la data, l'ora del giorno e l'anno della scadenza della bozza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Decision]</td> 
   <td> <p>Nei report che contengono l'oggetto [!UICONTROL Document Version], ad esempio i report [!UICONTROL Document Version] e [!UICONTROL Proof Approval], questo campo visualizza lo stato di decisione della bozza (in sospeso, modifiche necessarie o approvate)</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome bozza]</td> 
   <td> <p>Nei report che contengono l'oggetto [!UICONTROL Document Version], ad esempio un report [!UICONTROL Document Version] e un report [!UICONTROL Proof Approval], questo campo visualizza il nome della bozza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL - Pagine bozza]</td> 
   <td> <p>Nei report che contengono l'oggetto [!UICONTROL Document Version], ad esempio i report [!UICONTROL Document Version] e [!UICONTROL Proof Approval], questo campo visualizza il numero di pagine incluse nella bozza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stato bozza]</td> 
   <td> <p>Nei report che contengono l'oggetto [!UICONTROL Document Version], ad esempio un report [!UICONTROL Document Version] e un report [!UICONTROL Proof Approval], visualizza lo stato di avanzamento della bozza ([!UICONTROL Sent], [!UICONTROL Opened], [!UICONTROL Commented], [!UICONTROL Decision Made]).</p> <p>Per ulteriori informazioni, consulta <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Panoramica sull’avanzamento della bozza</a> in <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Panoramica sullo stato e sull’avanzamento della bozza</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Strumenti di correzione]</td> 
   <td>Un processo di revisione in cui uno o più utenti contrassegnano e commentano il contenuto da modificare in un’immagine, un documento di testo, un video o un contenuto web interattivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>In un [!UICONTROL Note] o in un [!UICONTROL Document], questa opzione rende l'oggetto accessibile ad altri utenti o anche a persone esterne [!DNL Workfront]. Per una [!UICONTROL Help Desk Queue], [!UICONTROL Public] significa che tutti gli utenti che possono inviare problemi possono inviarli tramite l'area [!UICONTROL Help Desk].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Quality]</td> 
   <td>La percezione della qualità del lavoro all’interno dell’organizzazione.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue]</td> 
   <td>Chiamata anche [!UICONTROL Help Desk Queue]. Questo progetto è stato pubblicato nell'area [!UICONTROL Help Desk] per consentire agli utenti di inviare problemi. Di solito vengono create code per argomenti particolari, come bug, richieste di progetto, ecc.</td> 
  </tr> 
  <tr> 
   <td>Proprietà coda [!UICONTROL]</td> 
   <td>Queste impostazioni definiscono le regole di invio dei problemi per un progetto che viene pubblicato nell'Help Desk di [!UICONTROL].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Argomento Coda]</td> 
   <td> <p>Proprietà di una [!UICONTROL Help Desk Queue] che consente agli utenti che inviano un problema di selezionare un argomento. Gli argomenti possono:</p> 
    <ul> 
     <li>Essere associato a un form dati personalizzato.</li> 
     <li>Assegna automaticamente il problema a un utente, un ruolo o un team tramite la regola di indirizzamento impostata sull'argomento selezionato.</li> 
     <li>Sposta il problema in un progetto o in una coda diversa tramite la regola di instradamento impostata sull'argomento selezionato.</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Crea argomenti coda</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rank]</td> 
   <td> <p>In un report [!UICONTROL Livello di accesso] è possibile indicare manualmente un [!UICONTROL Livello di accesso] di [!UICONTROL Livello di accesso]. Questo ti aiuta, in quanto [!DNL Workfront] per identificare visivamente il livello di complessità associato a ciascun livello di accesso. Ad esempio, è possibile assegnare numeri più bassi per livelli di accesso più complessi ([!UICONTROL Plan]) e numeri più alti per livelli di accesso meno complessi ([!UICONTROL Requester]). Impossibile classificare i livelli di accesso standard. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pronto]</td> 
   <td> <p>Questo campo in un report attività indica se un'attività [!UICONTROL Agile] è stata contrassegnata come [!UICONTROL Ready] nel backlog. Questo flag si applica solo alle attività [!UICONTROL Agile], che sono attività assegnate a un team [!UICONTROL Agile]. </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Frequenza Ricorrenza]</td> 
   <td> <p>Campo visualizzato nella casella [!UICONTROL Dettagli attività] o [!UICONTROL Modifica attività] di un elemento padre di attività ricorrenti. Frequenza con cui si verificano le attività nella ricorrenza. Per informazioni sulla creazione di attività ricorrenti, vedere <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Creare attività ricorrenti</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reference Number]</td> 
   <td> <p>I progetti, le attività e i problemi vengono associati automaticamente a un numero di riferimento univoco durante la creazione. È possibile visualizzare il numero di riferimento [!UICONTROL] nella pagina [!UICONTROL Details] dei progetti, delle attività o dei problemi oppure in un elenco o in un report. </p> <p><b>SUGGERIMENTO</b><p><br>È possibile fare riferimento ai numeri di riferimento quando due elementi hanno lo stesso nome, poiché i numeri di riferimento sono sempre univoci. </p> <p>[!DNL Workfront] genera automaticamente un numero di riferimento sequenziale a livello di sistema. A ogni progetto, attività o problema viene assegnato il successivo numero disponibile nella sequenza. <br></p> <p>Ad esempio, se l'Utente A crea un'attività, [!DNL Workfront] può assegnare automaticamente all'attività il numero di riferimento 100. Se l'utente B crea un problema subito dopo, [!DNL Workfront] assegna al problema il numero di riferimento 101. Non è possibile modificare manualmente i numeri di riferimento. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema rifiuto]</td> 
   <td>In un progetto o in un report attività, questo è il problema che viene creato quando l’approvazione per il progetto o l’attività viene rifiutata. Per informazioni sui problemi di rifiuto, vedi l’articolo <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Creare un processo di approvazione per gli elementi di lavoro</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo Rischio Rimanente]</td> 
   <td> <p>Campo del progetto che mostra la differenza tra il [!UICONTROL Planned Risk Cost] di un progetto e il totale di tutti i [!UICONTROL Actual Costs] di tutti i rischi del progetto. </p> <p>Il [!UICONTROL Costo rischio rimanente] per un progetto viene calcolato utilizzando la seguente formula:</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ripianificazione]</td> 
   <td>Modifica delle date di un progetto per risolvere o risolvere problemi. Ad esempio, un progetto che è rimasto in sospeso per diversi mesi dovrebbe essere ripianificato per riflettere date precise.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Report]</td> 
   <td>Un grafico o una tabella contenente informazioni su un dato [!DNL Workfront] oggetto e gli attributi correlati.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request]</td> 
   <td> <p>Un tipo di problema che viene esaminato in una singola coda centralizzata e non è correlato a un impegno di lavoro continuo.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request Queue]</td> 
   <td>Il backlog di problemi gestiti da un processo di traffico e valutazione.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Velocity richiesta]</td> 
   <td>Tempo totale del ciclo di lavoro da assumere e completare una richiesta.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requester]</td> 
   <td>In genere è un tipo di licenza. Un utente con una licenza Richiedente può inviare richieste per nuove operazioni nel sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ora Riservata]</td> 
   <td>Giorni specificati nell'Ora personale di un utente, che indicano che l'utente non sarà disponibile per il lavoro. Consulta "[!UICONTROL Non Work Days]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risolvi problema]</td> 
   <td> <p>In un rapporto sui problemi, utilizza questo campo nelle visualizzazioni o nei filtri per fare riferimento al problema che risolve il problema. </p> <p>Per informazioni sulla visualizzazione degli oggetti di risoluzione nei report, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Visualizzare informazioni sugli oggetti risolvibili e risolvibili in un report</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sugli oggetti risolvibili e risolvibili </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risolvi progetto]</td> 
   <td> <p>In un report sui problemi, utilizza questo campo nelle visualizzazioni o nei filtri per fare riferimento al progetto che risolve il problema. </p> <p>Per informazioni sulla visualizzazione degli oggetti di risoluzione nei report, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Visualizzare informazioni sugli oggetti risolvibili e risolvibili in un report</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sugli oggetti risolvibili e risolvibili </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risolvi attività]</td> 
   <td> <p>In un rapporto sui problemi, utilizza questo campo nelle visualizzazioni o nei filtri per fare riferimento all’attività che risolve il problema. </p> <p>Per informazioni sulla visualizzazione degli oggetti di risoluzione nei report, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Visualizzare informazioni sugli oggetti risolvibili e risolvibili in un report</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sugli oggetti risolvibili e risolvibili </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource]</td> 
   <td>Utente/i e/o Ruolo/i esistente/i nel sistema e assegnato/i a Team e attività di progetto.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Gestione risorse]</td> 
   <td> <p>[!UICONTROL Resource Management] è un insieme di strumenti dell'organizzazione che consente di prevedere con precisione l'utilizzo delle risorse in base alla loro disponibilità in modo che il lavoro da eseguire venga completato nei tempi e nel budget previsti. </p> <p>Con gli strumenti di gestione delle risorse è possibile pianificare le esigenze di capacità a lungo termine e di programmazione a breve termine per le risorse. </p> <p>Per informazioni sulla gestione delle risorse in [!DNL Workfront], vedi <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Introduzione alla gestione delle risorse</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID gestione risorse]</td> 
   <td><p>In un rapporto di progetto, puoi utilizzare questa opzione durante la creazione di un filtro per trovare un responsabile risorse specifico. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager]</td> 
   <td> <p>In un report di progetto o in una visualizzazione elenco, questo è un campo informativo che visualizza gli utenti designati per eseguire attività di gestione delle risorse sul progetto.  Quando si utilizza "[!UICONTROL Resource Manager]" in un report, viene visualizzato un elenco di gestori di risorse, con ogni gestore di risorse sul progetto separato da una virgola. Puoi designare fino a 30 responsabili delle risorse per un determinato progetto.</p> <p>Per ulteriori informazioni, consulta l’articolo <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Designare Responsabili risorse per un progetto o un modello </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Ore preventivate di programmazione risorse] </td> 
   <td>Le ore preventivate per il progetto e le risorse associate in [!UICONTROL Resource Planner]. Vedi anche "[!UICONTROL Ore Preventivate]" in questo articolo. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Pianificazione risorse] </td> 
   <td>Una versione avanzata [!DNL Workfront] strumento che consente di visualizzare e gestire le risorse tra progetti, ruoli o utenti. Per informazioni, consulta <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Panoramica di Programmazione delle risorse</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo manodopera preventivato per la pianificazione delle risorse]</td> 
   <td> <p>Si tratta del costo associato alle ore preventivate per le mansioni di progetto che utilizzano la pianificazione risorse. </p> <p>Vedere anche "Costo manodopera preventivato" in questo articolo. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Pool di Risorse]</td> 
   <td> <p>I Pool di Risorse sono insiemi di utenti che possono essere associati a un progetto. Gli utenti dello stesso Pool di Risorse appartengono in genere allo stesso reparto, hanno abilità simili o complementari o sono finanziati con lo stesso budget. È possibile associare più gruppi di risorse a un progetto o a un utente. Un pool di risorse può essere assegnato esclusivamente a un progetto o condiviso da più progetti.</p> 
   <p>Per ulteriori informazioni sui pool di risorse, consulta <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Panoramica sui pool di risorse </a>.</p> 
   <p>Nei report di progetto, i Pool di Risorse mostrano tutti i Pool associati a un Progetto. Questo oggetto non può essere utilizzato in un raggruppamento.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>Utilizzo risorse [!UICONTROL]</td> 
   <td>Un report che mostra il numero di ore disponibili durante un determinato periodo di tempo e il numero di ore pianificate per ogni utente nel report. Viene calcolato anche in [!UICONTROL Average Hours Per Day] e in una percentuale di allocazione.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Result]</td> 
   <td>In entrata [!DNL Workfront Goals], un risultato è un indicatore di avanzamento per un obiettivo. Può essere un numero, un valore percentuale o un importo di valuta aggiornato manualmente. Non è possibile visualizzare i risultati in un report e non è possibile accedervi tramite [!DNL Workfront] API. Per informazioni sulle attività, consulta <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Introduzione ai risultati e alle attività in Obiettivi di Adobe Workfront</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Revenue]</td> 
   <td>Importo fatturabile per l'attività o il progetto. L’importo può essere orario, fisso o una combinazione di entrambi.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di retribuzione]</td> 
   <td>Il tipo di retribuzione determina il modo in cui l'attività accantonerà i ricavi. Alcuni esempi includono [!UICONTROL Ore Fisse], [!UICONTROL Ore Ruolo] e [!UICONTROL Ore Ruolo w/Cap]. Per informazioni sul tracciamento dei ricavi in [!DNL Workfront] vedi <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica su fatturazione e ricavi</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>In genere è un tipo di licenza. Un utente con una licenza di [!UICONTROL Reviewer] può rivedere e approvare elementi di lavoro nel sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk]</td> 
   <td> <p>Questo può fare riferimento ai seguenti concetti in [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>Campo in un progetto che indica quanto può essere rischioso un progetto. Puoi assegnare la priorità all’esecuzione dei progetti in base al livello di rischio. I progetti possono presentare i seguenti livelli di rischio:</p> <p>- [!UICONTROL Molto Basso]</p> <p>- [!UICONTROL Min]</p> <p>- [!UICONTROL Medio]</p> <p>- [!UICONTROL Alto]</p> <p>- [!UICONTROL Molto Alto]</p> <p>I livelli di rischio indicati per un progetto non possono essere personalizzati. </p> <p> Per informazioni sull’aggiornamento del rischio di un progetto, consulta la sezione "Impostazioni progetto" dell’articolo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Modifica progetti</a>. Puoi visualizzare il campo dei rischi di un progetto nei rapporti. </p> </li> 
     <li> <p>Evento che può verificarsi durante il ciclo di vita di un progetto e che identifica un potenziale impatto sul costo, sull'ambito o sulla pianificazione del progetto. È possibile definire i rischi potenziali per un progetto e associarne la probabilità o un costo durante la creazione del Business Case del progetto. Per informazioni sull'aggiunta di rischi al Business Case del progetto, vedere "Creazione e modifica di rischi nei progetti". </p> <p>Non è possibile visualizzare nei rapporti i rischi definiti nel business case [!UICONTROL]. Nei rapporti e negli elenchi è possibile visualizzare solo diversi tipi di costi dei rischi. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Costo Rischio]</td> 
   <td> <p>Il costo associato ai rischi di un progetto. Di seguito sono riportati i costi dei rischi associati ai progetti che è possibile visualizzare nei rapporti:</p> 
    <ul> 
     <li> <p>[!UICONTROL Costo effettivo]: campo di un rischio che mostra il costo effettivo del rischio che si è verificato. Oltre ai report e agli elenchi, è possibile individuarli nella casella [!UICONTROL Modifica rischio] durante la modifica o la creazione di un rischio. </p> <p>Per i costi relativi a progetti, attività o problemi, consulta "[!UICONTROL Costo effettivo]" in questo articolo. </p> </li> 
     <li> <p>[!UICONTROL Planned Risk Cost]: campo del progetto che mostra un totale di tutti i [!UICONTROL Potential Risk Costs] per il progetto. Vedi anche "[!UICONTROL Planned Risk Cost]" in questo articolo. </p> <p>Per informazioni sul costo del rischio potenziale, vedere <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcola costo rischio potenziale </a>. </p> </li> 
     <li> <p>[!UICONTROL Costo rischio rimanente]: campo del progetto che visualizza la differenza tra il totale dei [!UICONTROL Costi effettivi] di tutti i rischi e il [!UICONTROL Costo rischio pianificato]. Vedere anche "Costo del rischio residuo" in questo articolo. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Gestione del rischio]</td> 
   <td>Processi per identificare, mitigare e monitorare i rischi.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td>Consulta "[!UICONTROL Ruolo]" in questo articolo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing]</td> 
   <td>Assegnazione o spostamento automatico di un problema, in genere a causa di un argomento della coda o per il fatto di essere il percorso predefinito (Regola di indirizzamento) per la coda.</td> 
  </tr> 
  <tr> 
   <td>Regola di routing [!UICONTROL]</td> 
   <td>Impostazione su progetti e code che assegna automaticamente un problema a un utente, a una mansione o a un team oppure che sposta il problema in un altro progetto o coda. Le regole di instradamento vengono generalmente utilizzate con le code dell'helpdesk per assegnare automaticamente i problemi in arrivo.</td> 
  </tr> 
 </tbody> 
</table>

## S - U

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome Oggetto</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Saved Search]</td> 
   <td>Una ricerca per la quale sono stati salvati i criteri di ricerca. Le Ricerche salvate semplificano l'esecuzione della stessa ricerca senza dover immettere nuovamente i criteri di ricerca.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Scenario] (in [!DNL Workfront Fusion]) </td> 
   <td> <p>Uno scenario è costituito da una serie di passaggi (moduli) che indicano come i dati devono essere trasferiti e trasformati tra app/servizi.</p> <p>Per informazioni sugli scenari in [!DNL Workfront Fusion], vedi <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] panoramica dello scenario</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scenario] (nel [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>In [!DNL Scenario Planner], uno scenario è una copia di un piano. </p> <p>Il [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Il [!DNL Scenario Planner] panoramica</a>. </p> <p>Per informazioni sulla creazione di scenari, consulta <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Creare e confrontare scenari di piano in [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule]</td> 
   <td>Il programma di lavoro settimanale, inclusi gli orari di lavoro, combinato con Giorni liberi (come festività) e giorni di eccezione (come un giorno lavorativo del sabato). Le pianificazioni possono essere applicate a progetti e utenti.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Esenzione pianificazione]</td> 
   <td>Anche noto come [!UICONTROL Modified Shift]. Giorni programmati in contrasto con gli orari di lavoro settimanali regolari come definiti dalla programmazione. Ad esempio, un sabato programmato per il lavoro, se la pianificazione è impostata su Lavora solo dal lunedì al venerdì, sarà un'esenzione dalla pianificazione [!UICONTROL].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Report Programmato]</td> 
   <td> <p>Quando si crea un report di report, è possibile visualizzare informazioni sulle pianificazioni del report, se la consegna è pianificata utilizzando il campo [!UICONTROL Scheduled Report]. Questo campo mostra più valori, uno per ogni pianificazione di ciascun rapporto, in un elenco puntato. Per ulteriori informazioni sulla pianificazione dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Panoramica sulla consegna dei rapporti</a>.</p> <p>Poiché questo campo mostra più valori, non può essere utilizzato in un raggruppamento. È possibile accedervi solo in un filtro o in una visualizzazione. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modifica ambito]</td> 
   <td>Un [!UICONTROL Audit Trail] che, se attivo, genera una nota ogni volta che viene apportata una modifica all'ambito di un progetto o di un'attività, ad esempio se una [!UICONTROL Task Duration] o [!UICONTROL Predecessors] vengono modificati.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section]</td> 
   <td>Un’area sullo schermo, con una propria intestazione, creata per organizzare i dati personalizzati a scopo di visualizzazione.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interruzione Di Sezione]</td> 
   <td>Distanza o bordo tra le sezioni.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Security]</td> 
   <td>Impostazioni che consentono a un utente di interagire con determinati oggetti nel sistema e non con altri. Consulta anche "[!UICONTROL Access Levels]" in questo articolo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Setup]</td> 
   <td>Area in cui gli amministratori possono impostare le configurazioni di sistema e le preferenze.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severity]</td> 
   <td> <p>[!UICONTROL Severity] indica la probabilità che un elemento influisca sul completamento del lavoro. Ad esempio, un problema con [!UICONTROL Severity] elevata può bloccare completamente il completamento di un'attività, ma un problema con [!UICONTROL Severity] bassa può essere puramente cosmetico.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> Aggiorna gravità problema</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severities]</td> 
   <td>Consulta "[!UICONTROL Severity]" in questo articolo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sharing]</td> 
   <td>Azione che consente ad altri utenti di visualizzare o modificare un elemento specifico in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data Slack]</td> 
   <td>In una visualizzazione o in un report attività, in [!UICONTROL Data Slack] viene visualizzata la data esatta in cui un'attività potrebbe influire in modo significativo sulla [!UICONTROL Data completamento] del progetto. Per informazioni sulla data di Slack di un'attività, vedere <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Panoramica sulla data di Slack attività</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assegnazioni Smart]</td> 
   <td> <p>Quando si assegnano attività o problemi agli utenti, [!DNL Workfront] formula raccomandazioni ([!UICONTROL Smart Assignments]) su chi sono gli utenti migliori per completare il lavoro, in base al tempo disponibile per completarlo e alla loro relazione con il progetto.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Panoramica delle assegnazioni intelligenti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>Indica l'oggetto padre di un altro oggetto. Ad esempio, un documento allegato a un'attività ha il nome dell'attività nel campo [!UICONTROL Source] di un report o di una visualizzazione [!UICONTROL Document]; un problema registrato in un progetto ha il nome del progetto nel campo [!UICONTROL Source] di un report o di una visualizzazione Problema. </p> 
   <p>Nei seguenti rapporti viene visualizzata una colonna Origine in cui è possibile visualizzare informazioni sull'oggetto padre:</p>
  <ul><li>Rapporti sui problemi</li>
    <li>Rapporti orari</li>
    <li>Report documenti </li>
    </ul>
   <p>Se gli utenti non dispongono delle autorizzazioni per l’oggetto principale di un problema, un’ora o un documento, la colonna Origine del rapporto risulta vuota, anche se il rapporto è configurato per la visualizzazione, o per essere consegnato con i diritti di accesso di un altro utente. </p>
   <p> Per visualizzare informazioni sull'oggetto padre nel report, è consigliabile aggiungere una colonna per l'oggetto padre in cui è possibile visualizzare il nome dell'oggetto padre. </p>
    <p>Ad esempio, è possibile aggiungere uno degli elementi seguenti a un report con una colonna Origine: </p>
    <ul><li>Le colonne Nome progetto, Nome attività o Nome problema in un documento o in una relazione sulle ore.</li>
    <li>Le colonne Nome progetto o Nome attività di un report sui problemi. </li> </ul>
    Per ulteriori informazioni, consulta <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">Eseguire e consegnare un report con i diritti di accesso di un altro utente</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data Inizio]</td> 
   <td> <p>La data in cui il lavoro su un elemento è impostato per l'inizio. In sono presenti diverse date di inizio [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL Pianificato]</li> 
     <li>[!UICONTROL Effettivo]</li> 
     <li>[!UICONTROL Previsto] </li> 
    </ul> <p>In un rapporto [!UICONTROL Rate], indica la data di inizio di una nuova tariffa di fatturazione per una mansione a livello di progetto. Le ore associate al progetto che sono successive a questa data vengono moltiplicate per questa tariffa di fatturazione per calcolare i ricavi sul progetto. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stato]</td> 
   <td> <p>Indicatore utilizzato per segnalare la posizione di un elemento di lavoro o di un obiettivo strategico nel flusso di lavoro.</p> <p>Per i progetti, [!UICONTROL Status] è un'impostazione del progetto che indica se il progetto è:</p> 
    <ul> 
     <li>[!UICONTROL corrente]</li> 
     <li>[!UICONTROL In Attesa] </li> 
     <li>[!UICONTROL Complete] </li> 
     <li>[!UICONTROL Dead]</li> 
    </ul> <p>Per ulteriori informazioni sullo stato del progetto, consulta <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Accedere all’elenco degli stati del progetto di sistema</a>.</p>
    <p>Per le attività, [!UICONTROL Status] è un'impostazione dell'attività che indica se l'attività è:</p> 
    <ul> 
     <li>[!UICONTROL Nuovo]</li> 
     <li>[!UICONTROL In Corso]</li> 
     <li>[!UICONTROL Complete]</li> 
    </ul> <p>Per ulteriori informazioni sullo stato delle attività, vedere <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Accedere all'elenco degli stati delle attività di sistema</a></p> <p>Per Issues, [!UICONTROL Status] è un'impostazione per Issue che indica se il Issue è:</p> 
    <ul> 
     <li>[!UICONTROL Nuovo]</li> 
     <li>[!UICONTROL In Corso]</li> 
     <li>[!UICONTROL in attesa di feedback]</li> 
     <li>[!UICONTROL In Attesa]</li> 
     <li>[!UICONTROL risolto]</li> 
     <li>[!UICONTROL non verrà risolto]</li> 
     <li>[!UICONTROL Non Può Essere Duplicato]</li> 
     <li>[!UICONTROL verificato completato]</li> 
     <li>[!UICONTROL Riaperto]</li> 
    </ul> <p>Per ulteriori informazioni sugli stati dei problemi, consulta <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Accedere all’elenco degli stati dei problemi di sistema</a>.</p> 
    <p>Per gli obiettivi strategici, [!UICONTROL Status] è un'impostazione sull'obiettivo che indica se l'obiettivo è:</p> 
     <ul> 
      <li>[!UICONTROL Attivo]</li> 
      <li>[!UICONTROL Bozza]</li> 
      <li>[!UICONTROL inattivo]</li> 
      <li>[!UICONTROL chiuso]</li> 
     </ul> 
     <p>Per ulteriori informazioni sugli obiettivi strategici, consulta anche "[!UICONTROL Goal]" o "[!UICONTROL Goals]" in questo articolo. </p> 
     <p>Per gli obiettivi strategici, questo campo è visibile solo se l’organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sulla gestione degli obiettivi strategici tramite [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] panoramica</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL - Modifica stato]</td> 
   <td>Un [!UICONTROL Audit Trail]. Viene generata una nota quando un Utente modifica lo Stato di un progetto, un’attività o un problema.</td> 
  </tr> 
  <tr> 
   <td>Le icone di Stato</td> 
   <td> <p>È possibile aggiungere il campo [!UICONTROL Status Icons] incorporato come colonna nelle visualizzazioni per migliorare la visibilità dei punti chiave relativi agli oggetti, ad esempio:</p> 
    <ul> 
     <li>A un oggetto sono allegati dei documenti</li> 
     <li>Un oggetto è associato a un processo di approvazione</li> 
     <li>A un oggetto sono associate delle note aggiuntive</li> 
     <li>Una spesa è fatturabile o rimborsabile </li> 
     <li>Un'attività si trova in un percorso critico</li> 
     <li>Un utente appartiene a un’azienda, a un team o si trova in un fuso orario diverso </li> 
    </ul> <p>È possibile aggiungere il campo [!UICONTROL Icone di stato] nelle visualizzazioni dei seguenti oggetti: </p> 
    <ul> 
     <li>[!UICONTROL Attività]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Progetti]</li> 
     <li>Attività modello [!UICONTROL]</li> 
     <li>[!UICONTROL Modelli]</li> 
     <li>[!UICONTROL Spese]</li> 
     <li>[!UICONTROL Documenti]</li> 
     <li>[!UICONTROL Utenti]</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Icone di stato incorporate nelle visualizzazioni</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL - Aggiornamento stato]</td> 
   <td> <p>Questo campo mostra l'aggiornamento di stato più recente fornito dagli utenti nel campo '[!UICONTROL Update Status]'. I commenti aggiunti agli aggiornamenti dello stato non vengono visualizzati nella colonna [!UICONTROL Status Update] (Aggiornamento dello stato).</p> <p>Per visualizzare gli stati '[!UICONTROL New],' '[!UICONTROL In Process],' e '[!UICONTROL Complete]', utilizzare la colonna [!UICONTROL Status].</p> <p>I commenti aggiunti agli aggiornamenti dello stato non vengono visualizzati nella colonna [!UICONTROL Status Update] (Aggiornamento dello stato).</p> <p>Per ulteriori informazioni sugli stati, consulta l’articolo <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Aggiorna stato attività</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Stati [!UICONTROL]</td> 
   <td>Consulta "[!UICONTROL Status]" in questo articolo.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>Un grafico che rappresenta lo stato delle storie (attività nella metodologia agile) e il loro avanzamento verso il completamento.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Ore storia]</td> 
   <td>Una metrica utilizzata per misurare la difficoltà o la complessità di una storia. I team agili possono scegliere se utilizzare le ore o i punti.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Punti storia]</td> 
   <td>Una metrica utilizzata per misurare la difficoltà o la complessità di una storia. I team agili possono scegliere se utilizzare le ore o i punti.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL strategico]</td> 
   <td>Lavoro a lungo termine che modifica l’organizzazione o il suo funzionamento.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Allineamento strategico]</td> 
   <td>Misurazione e allineamento degli obiettivi aziendali tra portfolio e programmi.</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>Viene utilizzato nelle colonne del rapporto quando si utilizza l’interfaccia in modalità testo. </p>
   <p>Il <code>[!UICONTROL stretch]</code> viene utilizzato per identificare le colonne che occupano spazio aggiuntivo non necessario per la visualizzazione. La larghezza dell’interfaccia utente dell’area di lavoro per un utente tipico è di circa 850 pixel. Ciò significa che se disponi di una vista con quattro colonne (150 pixel ciascuna), la vista occupa 600 di 850 pixel. Nell’interfaccia utente sono presenti 250 pixel aggiuntivi che verranno aggiunti alle colonne per le quali è fornita una percentuale di estensione. </p>
   <p>L'estensione di una colonna viene applicata quando si utilizza la riga di codice aggiuntiva: <code>[!UICONTROL usewidths=true]</code> per almeno una delle colonne della visualizzazione. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Subscribers]</td> 
   <td> <p>Utenti abbonati a progetti, attività o problemi.</p> <p>Quando utilizzi questo campo in un rapporto, viene visualizzato un elenco di abbonati, separati da una virgola.</p> <p>Per ulteriori informazioni, consulta l’articolo <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Iscriviti agli elementi in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività di riepilogo]</td> 
   <td>Vedi "[!UICONTROL Attività padre]" in questo articolo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sottoattività]</td> 
   <td>Un'attività figlio, che si trova sotto un'attività padre.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Governance del sistema]</td> 
   <td>Un insieme di criteri che regolano le modifiche e la manutenzione di un sistema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL System Integration]</td> 
   <td>Il processo di collegamento fisico o funzionale tra diversi sistemi informatici e applicazioni software per agire come un insieme coordinato.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Attività]</td> 
   <td> <p>Un’attività che deve essere eseguita come un passaggio verso il raggiungimento di un obiettivo finale (completamento del progetto).</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Panoramica delle attività</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Attributo attività [!UICONTROL]</td> 
   <td>Altri campi o oggetti associati a un oggetto Task e che indicano determinati dettagli sull'oggetto Task. Alcuni esempi sono [!UICONTROL Data di completamento pianificata] e [!UICONTROL Stato].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vincolo Attività]</td> 
   <td>Consulta "[!UICONTROL Tipo di vincolo]" e "[!UICONTROL Data vincolo]".</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Gestione attività]</td> 
   <td>Un insieme di criteri che definisce le soglie per la creazione, l'assegnazione, la chiusura e la visibilità delle attività.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Proprietario attività]</td> 
   <td>Il team o l’utente responsabile della stima dello sforzo e del completamento dell’attività</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Team]</td> 
   <td> <p>Una raccolta di utenti che lavorano per obiettivi aziendali o obiettivi di business simili. Questi utenti possono essere collettivamente assegnati a un elemento di lavoro assegnando il team all’elemento di lavoro.</p> <p>Per ulteriori informazioni sui team, consulta <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Panoramica sui team</a>.</p> <p>I progetti possono avere un [!UICONTROL Project Team] che contiene tutti gli utenti o i ruoli associati al lavoro sul progetto.</p> <p>Per ulteriori informazioni sui team di progetto, consulta <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Panoramica del team del progetto</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>Modello [!UICONTROL]</td> 
   <td> <p>I modelli di progetto sono contorni generici dei progetti più ripetibili. Quando si crea un modello di progetto, è possibile definire attività, argomenti della coda, moduli personalizzati, allegare documenti o approvazioni per risparmiare tempo quando è necessario creare un nuovo progetto. </p> <p>È possibile allegare modelli ai progetti esistenti o utilizzarli per creare nuovi progetti. Tutte le informazioni specificate nel modello vengono trasferite ai progetti creati utilizzando tale modello. </p> <p>Per ulteriori informazioni sui modelli, consulta <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Panoramica sui modelli di progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività Modello]</td> 
   <td>Un'attività che fa parte di un modello. Le Attività modello diventano Attività nel progetto creato mediante il Modello.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>Una [!UICONTROL Note] e la relativa raccolta di risposte relative a un argomento specifico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thumbnail]</td> 
   <td> <p> In un elenco o report di [!UICONTROL Document] viene visualizzata un'anteprima del documento in una miniatura. </p> <p> Seleziona <strong>[!UICONTROL Thumbnail]</strong>  per visualizzare una miniatura di 33-66 pixel nel rapporto. </p> <p>Le dimensioni della miniatura vengono regolate quando si modifica la larghezza della colonna in un elenco o in un report.</p> <p>Vedi anche "[!UICONTROL Large Thumbnail]" in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time Off]</td> 
   <td>È possibile generare un report [!UICONTROL Time Off] (Ferie) per visualizzare quando gli utenti hanno indicato un'indisponibilità nel loro profilo. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet]</td> 
   <td> <p>Un foglio ore che consente agli utenti di immettere le ore effettive trascorse lavorando su progetti, attività o problemi, oppure le ore trascorse per altre attività non correlate al lavoro, come riunioni o formazione. Oltre a specificare la quantità di tempo impiegata, è possibile indicare anche se il tempo è correlato al lavoro o equivale a un tempo di lavoro comune utilizzando i Tipi di lavoro per definire le immissioni di tempo. Per informazioni sulle schede orario, consulta <a href="../../../timesheets/timesheets/timesheets-overview.md">Panoramica schede orario</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet Ricorrente]</td> 
   <td> <p>Un [!UICONTROL Timesheet Profile] è un modello che [!DNL Workfront] utilizza per creare automaticamente le schede orario per gli utenti ad esse associati. </p> <p>Puoi configurare diverse impostazioni da applicare a ogni scheda orario durante la creazione. Alcune di queste impostazioni sono: la frequenza con cui la scheda orario deve essere creata (settimanalmente, ogni due settimane, due volte al mese o mensilmente), il giorno di inizio della scheda orario, gli approvatori della scheda orario, i [!UICONTROL Hour Types] disponibili che gli utenti possono associare alle ore registrate.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL ID padre principale] </td> 
   <td> <p>Questo campo consente di identificare e filtrare i dati relativi a un gruppo di primo livello e ai relativi sottogruppi in un elenco o in un report.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome padre principale] </td> 
   <td> <p>Questo campo consente di identificare i dati di un gruppo di primo livello e dei relativi sottogruppi in una visualizzazione [!UICONTROL] per un elenco o un report.</p> <p>Puoi eseguire questa operazione anche utilizzando il campo [!UICONTROL Top Parent ID].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ore Totali]</td> 
   <td> <p>In un report di progetto [!UICONTROL], questo campo visualizza la somma arrotondata di tutte le ore del progetto, l'ultima volta che sono stati calcolati i dati finanziari del progetto. Le ore effettive di [!UICONTROL] riflettono le ore esatte registrate nel progetto. In genere, le [!UICONTROL Ore effettive] devono corrispondere alle [!UICONTROL Ore totali]. Se il campo [!UICONTROL Ore totali] è significativamente diverso dal campo [!UICONTROL Ore effettive], è necessario ricalcolare i dati finanziari sul progetto.</p> <p>Per ulteriori informazioni sul ricalcolo dei dati finanziari del progetto, vedere l'articolo <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Ricalcolare i dati finanziari del progetto</a>.</p> <p>In una visualizzazione Scheda orario [!UICONTROL Standard], questo campo si riferisce al totale delle ore registrate per gli elementi per le date visualizzate in una scheda orario. Il campo [!UICONTROL Ore totali] per le schede orario in questa visualizzazione incorporata fa riferimento al campo "[!UICONTROL hoursDuration]" che calcola dinamicamente la differenza di ore tra le date di inizio e fine della scheda orario. Viene utilizzato per visualizzare la colonna [!UICONTROL Total Hours] (Ore totali) in rosso se l’utente registra più tempo delle ore disponibili nell’intervallo di tempo della scheda orario. Per ulteriori informazioni, consulta <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">Visualizza le ore totali sulla scheda orario</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modalità Tracciamento]</td> 
   <td> <p>Attributo di un'attività. Questo ha determinato come e quindi le timeline previste verranno aggiornate per un’attività. Ad esempio:</p> 
    <ul> 
     <li>[!UICONTROL User Must Update] richiede l'aggiornamento manuale di un'attività. In caso contrario, diventerà [!UICONTROL Behind Schedule], quindi [!UICONTROL Late].</li> 
     <li>[!UICONTROL Completamento automatico] completerà automaticamente un'attività quando la data di scadenza, o [!UICONTROL Data di completamento pianificata], è stata superata.</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Panoramica sulla modalità di monitoraggio attività</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Trigger]</td> 
   <td>Un evento che avvia uno scenario.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività con problemi]</td> 
   <td>Attività incompleta con una condizione di [!UICONTROL Late], [!UICONTROL Behind Schedule] o [!UICONTROL At Risk].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività non assegnata]</td> 
   <td>Un'attività che non è assegnata ad alcun Utente, Ruolo o Team.</td> 
  </tr> 
  <tr> 
   <td>Tipo di aggiornamento [!UICONTROL]</td> 
   <td> <p>Impostazione del progetto che determina quando verrà ricalcolata la sequenza temporale prevista del progetto. Le opzioni sono:</p> 
    <ul> 
     <li>[!UICONTROL Automatic and On Change]</li> 
     <li>[!UICONTROL Solo Automatico]</li> 
     <li>[!UICONTROL Solo Manuale] </li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleziona il tipo di aggiornamento del progetto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utente]</td> 
   <td>Un account creato in [!DNL Workfront] per consentire a una persona di accedere al sistema e interagire con esso.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL - Delega utente]</p> </td> 
   <td> <p>Oggetto segnalabile che indica:</p> 
    <ul> 
     <li>Quali utenti hanno delegato le approvazioni di attività, problemi e progetti</li> 
     <li>Quali utenti hanno ricevuto le approvazioni di attività, problemi e progetti delegate</li> 
     <li>Quando queste deleghe iniziano e terminano</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Creare un rapporto di delega utente</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interfaccia Utente]</td> 
   <td>Tutti gli aspetti visivi e interattivi della [!DNL Workfront] applicazione.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL - Preferenze interfaccia utente]</td> 
   <td>[!UICONTROL User Interface Setup]. [!DNL Workfront] gli amministratori possono modificare queste impostazioni per personalizzare alcuni aspetti dell’interfaccia utente.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>Utilizzo di [!UICONTROL]</td> 
   <td>La disponibilità per un utente o un ruolo in base alla pianificazione assegnata, alla PTO e al carico di lavoro corrente.</td> 
  </tr> 
  <tr> 
   <td>Utilizzo utente di [!UICONTROL]</td> 
   <td> <p>Una ricerca combinata con un rapporto che mostra come gli Utenti (Risorse) sono allocati o sovrassegnati. Consulta "[!UICONTROL Resource Utilization]" in questo articolo.</p> </td> 
  </tr> 
 </tbody> 
</table>

## V - Z

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome Oggetto</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Velocity]</td> 
   <td>Misura della durata totale del ciclo di lavoro (tempo necessario per completare un lavoro) e la frequenza con cui il lavoro viene eseguito nel tempo impegnato originariamente (rapporto lavoro su impegno).</td> 
   </tr> 
  <tr> 
   <td>Visualizzazione [!UICONTROL]</td> 
   <td> <p>Le visualizzazioni possono essere utilizzate per modificare le colonne di un report o di un elenco di progetti, attività o problemi oppure per indicare il diritto di un utente di visualizzare solo le informazioni a un livello di accesso o a un livello di condivisione delle autorizzazioni.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Icone Vista]</td> 
   <td> <p> Questo campo è uguale a quello delle icone di stato, ma è disponibile solo per le visualizzazioni seguenti: </p> 
    <ul> 
     <li> [!UICONTROL Documenti] </li> 
    </ul> <p> Per ulteriori informazioni, consulta l’articolo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Icone di stato incorporate nelle visualizzazioni</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni Mese Scorso]</td> 
   <td> <p>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato durante l’ultimo mese.<br>Per ulteriori informazioni sulle informazioni di utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizza utilizzo report</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni ultimo trimestre]</td> 
   <td>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato durante l’ultimo trimestre.<br>Per ulteriori informazioni sulle informazioni di utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >Visualizza utilizzo report</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni ultimo anno]</td> 
   <td>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato durante l’ultimo anno.<br>Per ulteriori informazioni sulle informazioni di utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizza utilizzo report</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni Questo Mese]</td> 
   <td> <p>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato nel corso del mese corrente.<br>Per ulteriori informazioni sulle informazioni di utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizza utilizzo report</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni Questo Trimestre]</td> 
   <td>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato durante questo trimestre.<br>Per ulteriori informazioni sulle informazioni di utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizza utilizzo report</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni Quest'Anno]</td> 
   <td>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato durante l'anno corrente.<br>Per ulteriori informazioni sulle informazioni di utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">Visualizza utilizzo report</a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> In un report, quando si utilizza l'interfaccia [!UICONTROL Text Mode], la riga di codice in cui è possibile specificare la larghezza di ogni colonna in pixel. Workfront fornisce una larghezza consigliata per ogni campo, anche se a seconda del tipo di campo e del formato, potrebbe essere necessario apportare delle modifiche.
È necessario utilizzare il pulsante aggiuntivo <code>[!UICONTROL usewidths=true]</code> riga di codice per applicare la larghezza specificata per la colonna. 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>In un rapporto di progetto, attività o problema, l’istruzione che segue in modalità testo mostra le Ore pianificate del progetto, dell’attività o del problema:</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>Per informazioni sull'utilizzo della modalità testo, vedere <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Panoramica sulla sintassi della modalità testo</a>. </p> 
   <p><b>SUGGERIMENTO</b> 
   <p>In un report sui problemi, l’aggiunta di uno dei campi [!UICONTROL Planned Hours] (Ore pianificate) aggiunge <code>work </code>al report. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lavoro]</td> 
   <td> <p>Uno dei due tipi di licenza principali. L'accesso è inferiore a [!UICONTROL Plan], ma è possibile creare e aggiornare il sistema. Sono disponibili più capacità rispetto ai tipi di licenza [!UICONTROL External], [!UICONTROL Reviewer] o [!UICONTROL Requester].</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] panoramica sulle licenze</a>.</p> <p>Il lavoro può fare riferimento al numero di [!UICONTROL Lavoro Necessario] per un progetto, un'attività o un problema. Per ulteriori informazioni, vedere il campo "[!UICONTROL work]" in questa tabella. </p> <p>Suggerimento: in un rapporto sui problemi, l’aggiunta di uno dei campi [!UICONTROL Planned Hours] (Ore pianificate) aggiunge <code>work </code>al report. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Breakdown Structure]</td> 
   <td>Struttura gerarchica delle attività che devono essere eseguite dal team di progetto in base alla relazione padre/figlio.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Impegno di lavoro] </td> 
   <td> 
    <p>Un project manager potrebbe decidere di utilizzare questo campo anziché [!UICONTROL Lavoro Necessario] per stimare lo sforzo necessario per completare un'attività. Questo campo è visibile solo quando sono soddisfatte le seguenti condizioni:</p> 
     <ul> 
      <li> <p>L'attività ha un [!UICONTROL Simple Duration Type]. </p> <p>Suggerimento: se si aggiorna l'attività [!UICONTROL Duration Type] a un altro tipo, questo campo viene nascosto. </p> </li> 
      <li>Il project manager ha abilitato il campo [!UICONTROL Use Work Effort] per calcolare automaticamente l'attività [!UICONTROL Planned Hours] nel progetto. </li> 
     </ul> 
     <p>Per informazioni sull'utilizzo di [!UICONTROL Impegno di lavoro] invece di [!UICONTROL Ore pianificate] per stimare l'impegno di attività, vedere <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Panoramica sull’impegno di lavoro</a>. </p> 
     <p>È possibile visualizzare questo campo nei report attività e negli elenchi.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Elemento Di Lavoro]</td> 
   <td> <p>Questo campo si riferisce alle attività o ai problemi in [!DNL Workfront]. </p> <p>Il rapporto [!UICONTROL Work Item] (Elemento di lavoro) visualizza informazioni sia per le attività che per i problemi. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Mix]</td> 
   <td>Un [!UICONTROL Work Performance Indicator] (WPI) della proporzione di lavoro allocata per l'esecuzione dell'azienda rispetto a una modifica dell'azienda. L’interfaccia WPI di tipo Mix consente di comprendere, a livello organizzativo, se alla strategia è applicata un’allocazione effettiva del lavoro.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risorsa gestione lavoro]</td> 
   <td>Designazione di un utente tipo nel sistema che è idoneo a ricevere lavoro o tempo di registrazione.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ruolo e responsabilità di gestione del lavoro]</td> 
   <td>Definizione dei proprietari e delle parti interessate per la gestione dell'ambito, dell'esecuzione e delle approvazioni del problema, del task, del progetto, del programma o del portfolio designato.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL SLA gestione lavoro]</td> 
   <td>Una metrica quantificabile concordata da tutte le parti interessate.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interessato alla gestione del lavoro]</td> 
   <td>Una raccolta di utenti con un interesse acquisito nei risultati di una richiesta di lavoro.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Punti di contatto per la gestione del lavoro]</td> 
   <td>Record digitalizzati di comunicazione tra le parti interessate.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indicatori prestazioni lavoro] </td> 
   <td> <p>Rapporto di mix, capacità, velocità, qualità e coinvolgimento.</p> <p>WPI è un acronimo comune per [!UICONTROL Work Performance Indicator].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Process] (Processo di lavoro)</td> 
   <td> <p>Il metodo in cui il lavoro viene ricevuto, prioritizzato ed eseguito. Il modo in cui si esegue il lavoro è in genere denominato "flusso di lavoro" o "piano di progetto" (un elenco di attività con date, relazioni predecessore e così via). </p> <p>Esempi di un processo di lavoro possono essere la produzione di una singola risorsa o la consegna di una campagna con più risorse. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modello flusso di lavoro]</td> 
   <td>Nel rapporto [!UICONTROL Proof Approval] (Approvazione bozza) questo campo visualizza tutti i modelli di flusso di lavoro allegati a una bozza. Se non sono presenti modelli allegati, la colonna è vuota.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Orario Di Lavoro]</td> 
   <td>

<p>Rappresenta la percentuale di tempo equivalente a tempo pieno ([!UICONTROL FTE]) per cui l'utente è disponibile per il lavoro effettivo, esclusi i costi comuni. [!UICONTROL Work Time] deve essere un numero decimale massimo di 1 e non può essere 0. Ad esempio, una disponibilità del 20% per il lavoro effettivo sarebbe 0,2.</p>
   </p>Il valore predefinito del campo è 1, che indica che un utente spende l’intero [!UICONTROL FTE] per il lavoro effettivo relativo al progetto.  </p>
   <p>Il sistema utilizza questo numero per calcolare la disponibilità dell'utente per il lavoro effettivo correlato al progetto. </p>
   <p> Eccezioni alla pianificazione e indisponibilità potrebbero influire anche sulla capacità dell'utente. </p>
   <p>Per ulteriori informazioni sulla creazione di pianificazioni in Workfront, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Creare una pianificazione</a>. </p>
    <p>Workfront calcola la disponibilità di un utente in base alle preferenze di Gestione risorse nell'area [!UICONTROL Setup]. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Configurare le preferenze di Gestione risorse</a>. </p> 
   <p>È possibile aggiornare l'[!UICONTROL Work Time] di un utente quando lo si modifica o lo si crea. Per informazioni, consulta <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Modificare il profilo di un utente</a></p> 
   <b>SUGGERIMENTO</b> 
   <p>Imposta il valore [!UICONTROL Work Time] (Tempo di lavoro) su 1 per indicare che l'utente è disponibile per il lavoro correlato al progetto per l'intero equivalente a tempo pieno.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Orario di lavoro]</td> 
   <td>Nella documentazione di Workfront, questo termine viene utilizzato per descrivere il tempo assegnato al lavoro, in base a una pianificazione.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>In un report di progetto, attività o problema, utilizzando l’istruzione seguente in modalità testo viene visualizzato il numero di ore pianificate del progetto, attività o problema seguito dalla parola "ore":</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>Per informazioni sull'utilizzo della modalità testo, vedere <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Panoramica sulla sintassi della modalità testo</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
