---
content-type: reference
navigation-topic: workfront-navigation
title: 'Glossario della terminologia di  [!DNL Adobe Workfront] '
description: Il glossario di  [!DNL Adobe Workfront]  elenca i termini comunemente usati nell’interfaccia di  [!DNL Adobe Workfront]. You can use the glossary when you want to find the definition of concepts you see in the [!UICONTROL Workfront] , nei rapporti o quando provi a capire il significato di concetti di  [!DNL Workfront]  definiti nella documentazione di  [!DNL Workfront] .
author: Alina
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 087589f3d7a3fbb1611045b921e804aec3db9a74
workflow-type: tm+mt
source-wordcount: '21621'
ht-degree: 99%

---


# Glossario della terminologia di [!DNL Adobe Workfront]

<!--Audited: 12/2023-->

>[!IMPORTANT]
>
>Questo articolo deve essere utilizzato come riferimento per comprendere i termini che puoi incontrare nell’applicazione [!DNL Adobe Workfront], nella documentazione di [!DNL Workfront] o quando si parla in generale di pianificazione e gestione del lavoro. Queste informazioni sono in fase di aggiornamento e di conseguenza questa tabella potrebbe non essere completa. Quando tali informazioni saranno considerate esaustive, la dichiarazione di non responsabilità verrà rimossa.

La tabella seguente è un elenco dei termini comunemente utilizzati in Adobe Workfront:

## A - C

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nome oggetto</strong></th> 
   <th><strong>Descrizione</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Livello di accesso]</td> 
   <td>Profilo utente che determina il modo in cui un utente può interagire con diversi oggetti e strumenti all’interno di Workfront.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività attiva]</td> 
   <td>Attività incompleta in un progetto corrente che non è impedita da un’attività predecessore e che non ha un vincolo attività con una data di inizio pianificata futura. In altre parole, ci si può lavorare già oggi.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Attività]</td> 
   <td>In [!DNL Workfront Goals] un’attività è un indicatore di avanzamento per un obiettivo. Può trattarsi di una barra di avanzamento che aggiorni manualmente o di un progetto associato all’obiettivo. Non puoi visualizzare le attività in un rapporto e accedervi tramite l’API [!DNL Workfront]. Per informazioni sulle attività, consulta <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Introduzione ai risultati e alle attività negli obiettivi di Adobe Workfront</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo effettivo]</td> 
   <td> <p>Per attività e problemi, questo rappresenta il costo associato alle ore effettive registrate in relazione alla tariffa oraria del costo della risorsa assegnata all’attività o al problema. Per i progetti, questo rappresenta il valore totale di tutti i [!UICONTROL Costi effettivi] relativi alle attività e ai problemi del progetto. Per informazioni, consulta <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tenere traccia dei costi</a>.</p>

<p>I calcoli del [!UICONTROL Costo effettivo] prendono in considerazione le [!UICONTROL Ore effettive precedenti]. Per informazioni, consulta “[!UICONTROL Ore effettive]” o “[!UICONTROL Ore effettive precedenti]” in questa tabella. </p>   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo spesa effettivo]</td> 
   <td> <p>La somma degli [!UICONTROL Importi effettivi] per tutte le spese registrate per un progetto o un’attività.</p> <b>ESEMPIO </b>
   <p>Se crei una spesa per l’attività 1 e inserisci 600,00 $ nel campo [!UICONTROL Importo effettivo], il costo effettivo per questa attività [!UICONTROL Costo spesa effettivo] è di 600,00 $. </p> 
   <p>Per un progetto, [!DNL Workfront] utilizza la formula seguente per calcolare le [!UICONTROL Spese effettive]:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ore effettive]</td> 
   <td> <p>In un rapporto di progetto, attività o problema, [!UICONTROL Ore effettive] corrispondono alla somma di tutte le ore registrate sul progetto, sull’attività o sul problema dopo maggio 2021.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span> se dalla scheda [!UICONTROL Aggiornamenti] per l’attività 1, fai clic su “Registra ore” e inserisci 25 ore, le ore effettive dell’attività 1 = 25 ore. </p> <p>[!DNL Workfront] Calcola le [!UICONTROL Ore effettive] per le attività o i progetti principali utilizzando le formule seguenti:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project + [!UICONTROL Actual Hours] logged on issues in the project</code>  </p> </li> 
    </ul> 
   <p>Consulta anche <strong>[!UICONTROL Ore effettive precedenti]</strong>.
    <p>Per ulteriori informazioni, consulta <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md">Visualizzare le ore effettive</a>.</p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo effettivo della manodopera]</td> 
   <td> <p>Il [!UICONTROL Costo effettivo] associato alla manodopera investita in un’attività o in un progetto. </p> <p>Per un’attività, [!DNL Workfront] calcola il [!UICONTROL Costo effettivo della manodopera] utilizzando la formula seguente:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Se l’attività ha un [!UICONTROL Tipo di costo] di [!UICONTROL Ore per utente], [!DNL Workfront] utilizza la tariffa utente. Se l’attività ha un [!UICONTROL Tipo di costo] di [!UICONTROL Ore per ruolo], [!DNL Workfront] utilizza la tariffa della mansione per calcolare il [!UICONTROL Costo effettivo della manodopera]. </p> <p>Per un progetto, [!DNL Workfront] utilizza la formula seguente per calcolare il [!UICONTROL Costo effettivo della manodopera]:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tenere traccia dei costi</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>ad esempio, se un utente registra 5 ore per un’attività con un [!UICONTROL Tipo di costo] [!UICONTROL Ore per utente] e la tariffa oraria è di 100 $, il [!UICONTROL Costo effettivo della manodopera] è di 500 $.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Entrate effettive] </td> 
   <td> <p>Le [!UICONTROL Entrate effettive] di un progetto o di un’attività rappresentano la quantità di denaro associata alle [!UICONTROL Ore effettive] del progetto o dell’attività. </p> <p>Per informazioni sul tracciamento delle entrate in [!DNL Workfront], consulta <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica della fatturazione e delle entrate</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Inizio effettivo]</td> 
   <td>La marca temporale quando un utente modifica un oggetto di lavoro assegnato.</td> 
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
   <td>Un tipo di metodologia basata sull’evoluzione collaborativa delle esigenze e delle soluzioni con team interfunzionali. Incoraggia la flessibilità e il cambiamento sulla base di una timeline fissa.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Team Agile]</td> 
   <td>Si differenzia da un team tradizionale perché attinge il proprio lavoro potenziale da un backlog e ci lavora entro un periodo di tempo prestabilito denominato [!UICONTROL Iterazione].</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tutti i miei team]</td> 
   <td> <p>Quando si fa riferimento a questo nei [!UICONTROL filtri], questo campo mostra gli utenti che appartengono a uno dei team dell’utente connesso o gli elementi di lavoro assegnati a dei team a dell’utente connesso. </p> <p>È consigliabile utilizzare questo campo in un filtro per rendere i rapporti più generici quando vengono condivisi con altri utenti. In questo modo, puoi creare un unico rapporto che mostrerà informazioni diverse a seconda di chi effettua l’accesso per visualizzarlo, poiché queste sono sempre personalizzate per l’utente connesso. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di assegnazione]</td> 
   <td> <p>Puoi trovare questo campo nei seguenti tipi di rapporti:</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Progetto] (Dati finanziari)</li> 
     <li>[!UICONTROL Ora preventivata]</li> 
    </ul> <p>Per un rapporto di <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL Progetto (Dati finanziari)]: </p> 
    <ul> 
     <li>Genera questo rapporto quando tenti di comprendere <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> la quantità di [!UICONTROL Ore pianificate] assegnata alle risorse.</li> 
     <li> <p>La [!UICONTROL Data di assegnazione] è il primo giorno (domenica) della settimana in cui inizia l’allocazione di una [!UICONTROL Mansione] a un’attività. Una risorsa ([!UICONTROL Mansione]) può avere un numero di [!UICONTROL Date di assegnazione] pari alle settimane durante la [!UICONTROL Durata] delle attività a cui è assegnata. Se le attività si estendono su più mesi, anche il primo giorno di un mese può anche diventare una [!UICONTROL Data di assegnazione], se rientra nella [!UICONTROL Durata] dell’attività.</p> <p>Ad esempio, puoi assegnare una [!UICONTROL Mansione] a un’attività che si estende per più di 3 settimane e ha 90 [!UICONTROL Ore pianificate]. Queste ore vengono distribuite in modo uniforme durante la durata dell’attività, in modo che ciascun giorno assegni 6 [!UICONTROL Ore pianificate] alla tua mansione:</p> <p><em> [!UICONTROL Ore pianificate giornaliere] = [!UICONTROL Ore pianificate totali]/Numero di [!UICONTROL Giorni lavorativi] durante la [!UICONTROL Durata] dell’attività </em> </p> <p>Di conseguenza, durante il periodo di [!UICONTROL Durata] dell’attività esistono tre [!UICONTROL Date di assegnazione], una per ogni domenica di ciascuna settimana, a cui è associato un determinato numero di [!UICONTROL Ore pianificate].<br>Se l’attività inizia a metà dell’ultima settimana di un mese e termina due settimane dopo l’inizio di un nuovo mese, l’attività avrà quattro [!UICONTROL Date di assegnazione]: una per ogni domenica di ciascuna settimana durante la [!UICONTROL Durata] dell’attività e una per il primo giorno del nuovo mese.</p> <p>Per utilizzare al meglio queste informazioni, è consigliabile creare un rapporto <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> Progetto (Dati finanziari) e aggiungere un raggruppamento con matrice per [!UICONTROL Data di assegnazione], quindi raggruppare i risultati settimanalmente, mensilmente, trimestralmente o annualmente per ottenere i dati più accurati.<br>Per informazioni sulla creazione di un raggruppamento con matrice, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Creare un rapporto con matrice</a>.</p> </li> 
    </ul> <p>Le informazioni finanziarie vengono popolate nei rapporti del [!UICONTROL Progetto (Dati finanziari)] solo quando i dati a esse associati hanno meno di 5 anni. Ad esempio, se una mansione è stata allocata a un’attività nel gennaio 2015 e oggi è settembre 2021, un campo finanziario come la [!UICONTROL Data di assegnazione] relativo alla mansione non viene popolato nel rapporto [!UICONTROL Progetto (Dati finanziari)]. </p> 
    <div> 
     <p>Per un rapporto di [!UICONTROL Ora preventivata]:</p> 
     <ul> 
      <li>Crea questo rapporto quando tenti di comprendere la quantità di [!UICONTROL Ore preventivate] allocata alle risorse o ai progetti nella pianificazione risorse.</li> 
      <li> <p>La [!UICONTROL Data di assegnazione] è il primo giorno (una domenica) della settimana per la quale sono state preventivate le ore nella [!UICONTROL Pianificazione risorse]. </p> <p><b>SUGGERIMENTO</b></p> <p>Se una settimana si estende per due mesi, verranno generate due righe nel rapporto: una corrispondente al primo giorno della settimana (la domenica della prima settimana che cade nel primo mese) e la seconda riga mostrerà il primo giorno del secondo mese. </p> <p>Ad esempio, se preventivi 8 ore per un utente per la settimana dal 30 giugno (domenica) al 6 luglio (sabato), le due righe mostrano una [!UICONTROL Data di assegnazione] del 30 giugno e del 1 luglio. </p> </p> <p>Per informazioni sul budget delle risorse in [!DNL Resource Planner], consulta l’articolo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget per le risorse in [!DNL Resource Planner] utilizzando le viste [!UICONTROL Progetto] e [!UICONTROL Ruolo]</a>.</p> <p>Per informazioni sulla creazione di un rapporto [!UICONTROL Ora preventivata], consulta <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Rapporto: ora preventivata</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Annunci]</td> 
   <td> <p>Un modo per comunicare agli utenti informazioni all’interno del sistema. Queste informazioni vengono spesso fornite da [!DNL Workfront] all’amministratore o dall’amministratore all’utente. </p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Inviare annunci</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Integrazione di un’app]</td> 
   <td>Un’app rappresenta più comunemente un connettore per un’applicazione software, ma può anche rappresentare funzioni speciali che manipolano i dati.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Decisione dell’approvatore]</td> 
   <td> <p>Nel rapporto [!UICONTROL Approvazione bozza] questo campo mostra le decisioni di approvazione della bozza per le bozze che non sono più attive.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fase Approvatore]</td> 
   <td>Nel rapporto [!UICONTROL Rapporto approvazione bozza], questo campo mostra le informazioni su una fase corrente delle bozze.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approvazione]</td> 
   <td> <p>Per un determinato elemento di lavoro, ad esempio un’attività, un documento o una scheda orario, può essere necessario che un supervisore o un altro utente approvi l’elemento di lavoro. Questo processo è denominato approvazione. </p> <p>Per ulteriori informazioni, consulta <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Panoramica del processo di approvazione</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di approvazione]</td> 
   <td>Nel rapporto [!UICONTROL Approvazione bozza], questo campo mostra la data di approvazione di una bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approvatore]</td> 
   <td>Un utente o una mansione che deve approvare un dato elemento di lavoro o l’utente che approva le ore inserite nelle schede orario.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assegnato a]</td> 
   <td> <p>In un rapporto di [!UICONTROL Attività o Problema], questo campo mostra il proprietario dell’attività o del problema, oppure l’[!UICONTROL Assegnatario principale]. Puoi anche filtrare o raggruppare in base a questo campo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assegnazione]</td> 
   <td>Un utente, una mansione o un team assegnato a un problema o a un’attività. I progetti, i portfolio o i programmi non possono avere assegnazioni.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assegnazioni]</td> 
   <td> <p>In un rapporto [!UICONTROL Attività] o [!UICONTROL Problema], questo campo mostra un elenco di tutte le entità (utenti, mansioni, team) assegnate all’attività o al problema. Puoi filtrare in base a questo campo utilizzando i campi [!UICONTROL Assegnazioni Utenti] e [!UICONTROL Assegnazioni Ruoli]. Puoi filtrare in base al team assegnato all’attività o al problema utilizzando il campo Team. Non puoi raggruppare un rapporto in base a questo campo.</p> <p>Gli elementi di lavoro che sono stati spostati nel [!UICONTROL Cestino] continueranno a essere visualizzati in alcuni rapporti che fanno riferimento all’oggetto [!UICONTROL Assegnazione] in cui viene utilizzato un modificatore di filtro [!DNL OR].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assegnazioni Ruoli]</td> 
   <td>
   <p>In un rapporto [!UICONTROL Attività] o [!UICONTROL Problema], questo campo mostra informazioni sulle mansioni assegnate alle attività o ai problemi. In questo campo vengono visualizzati i [!UICONTROL Proprietari principali] e altre mansioni assegnati ad attività o problemi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stato dell’assegnazione]</td> 
   <td> <p>In un rapporto di assegnazione, attività o problema, lo [!UICONTROL Stato dell’assegnazione] mostra se gli utenti assegnati a un elemento di lavoro hanno fatto clic sul pulsante [!UICONTROL Lavoraci] o [!UICONTROL Fine] per accettare o completare il lavoro. Esistono i seguenti [!UICONTROL Stati di assegnazione]:</p> 
    <ul> 
     <li><b>[!UICONTROL Richiesto]</b>: l’utente è stato assegnato all’attività o al problema, ma non ha ancora fatto clic sul pulsante [!UICONTROL Lavoraci] per iniziare a lavorarci.</li> 
     <li><b>[!UICONTROL In elaborazione]</b>: l’utente ha fatto clic sul pulsante [!UICONTROL Lavoraci] e sta attualmente lavorando sull’elemento. </li> 
     <li><b>[!UICONTROL Fine]</b>: l’utente ha fatto clic sul pulsante [!UICONTROL Fine] e ha completato il lavoro sull’elemento. </li> 
    </ul> <p>Per ulteriori informazioni, consulta la Panoramica del pulsante <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[!UICONTROL Lavoraci] e [!UICONTROL Fine]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team di lavoro]</td> 
   <td>
   <p>In un rapporto di [!UICONTROL attività] o [!UICONTROL problema], questo campo mostra le informazioni sui team assegnati alle attività o ai problemi. Nel campo vengono visualizzati i [!UICONTROL Proprietari principali] e gli altri team assegnati ad attività o problemi. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assegnazione Utenti]</td> 
   <td>
   <p>In un rapporto di [!UICONTROL Attività] o [!UICONTROL Problema], questo campo mostra le informazioni sugli utenti assegnati alle attività o ai problemi. In questo campo vengono visualizzati i [!UICONTROL Proprietari principali] e altri utenti assegnati ad attività o problemi. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attributo]</td> 
   <td>Un attributo è una caratteristica di un oggetto di [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Area audit]</td> 
   <td> <p>Gli audit sono messaggi di sistema che registrano un’azione che si è verificata in Workfront. Vengono registrati i seguenti tipi di audit:</p> 
    <ul> 
     <li>[!UICONTROL Modifica ambito]</li> 
     <li>[!UICONTROL Azione allegato]</li> 
     <li>[!UICONTROL Modifica generale]</li> 
     <li>[!UICONTROL Modifica stato]</li> 
     <li>[!UICONTROL Nota]</li> 
     <li>[!UICONTROL Inserimento combinato]</li> 
     <li>[!UICONTROL Errore inserimento]</li> 
     <li>[!UICONTROL Modifica stato]</li> 
     <li>[!UICONTROL Modifica sottoscrizione]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit trail]</td> 
   <td>La raccolta di note generate automaticamente dagli eventi che vengono tracciati attraverso le Modifiche registrate ([!UICONTROL Aree audit]). Ciascuna nota registra chi ha eseguito l’azione, cosa ha fatto e quando l’ha fatta.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modifica automatica e attiva]</td> 
   <td> <p>Uno dei tipi di [!UICONTROL Aggiornamento del progetto]. Le timeline Prevista e Pianificata del Progetto verranno ricalcolate durante il processo di ricalcolo notturno e quando viene eseguito un aggiornamento al progetto o alle attività all’interno del Progetto. </p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selezionare il tipo di aggiornamento del progetto </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Disponibilità</p></td> 
   <td> <p>Questo termine viene utilizzato in relazione alla “disponibilità dell’utente” o alla “disponibilità delle risorse” e illustra la quantità di tempo in cui la risorsa (utente o mansione) è disponibile per lavorare. </p> 
   <p>Workfront calcola la disponibilità dell’utente utilizzando diversi campi e in base alle impostazioni delle preferenze di Gestione delle risorse nel sistema. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurare le preferenze di gestione delle risorse</a>. </p>
   <p>Per ulteriori informazioni sulla disponibilità delle risorse, consulta <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Introduzione alla gestione delle risorse</a></p>
   In alternativa, anche il termine “capacità” viene utilizzato per fare riferimento alla disponibilità delle risorse. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Solo automatico]</td> 
   <td> <p>Uno dei tipi di [!UICONTROL Aggiornamento del progetto]. In questo modo le timeline Prevista e Pianificata verranno ricalcolate durante l’esecuzione del ricalcolo notturno.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selezionare il tipo di aggiornamento del progetto</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>Il lavoro “business as usual” che contribuisce alla gestione degli obiettivi aziendali primari quotidiani.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Backlog]</td> 
   <td>L’area in un ambiente Agile in cui vengono mantenuti i nuovi problemi fino a quando non sono pronti per l’esecuzione.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Linea di base]</td> 
   <td>Un’origine di dati su cui misurare le iterazioni in un ambiente Agile.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Spesa Fatturabile]</td> 
   <td> <p>Spesa contrassegnata come fatturabile per il cliente. Questa può essere una spesa pianificata o una spesa effettiva.</p> <p>I campi Costo spesa pianificata fatturabile e Costo spesa fatturabile effettivo sono disponibili per essere aggiunti alle viste e ai rapporti. Non vengono visualizzati nelle pagine dei dettagli del progetto o dell’attività.</p>
   <p>Questi campi sono disponibili nei seguenti tipi di rapporti:</p>
   <ul>
   <li>Linea di base</li>
   <li>Modello</li>
   <li>Progetto (dati finanziari)</li>
   </ul>
   <p>Per ulteriori informazioni su come contrassegnare una spesa come fatturabile, consulta <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Gestire le spese del progetto</a>.</p>
   </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Record della fatturazione]</td> 
   <td> <p>Registra le entrate, le ore o le spese che possono essere fatturati. Queste informazioni possono essere utilizzate per creare fatture in un sistema contabile esterno.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Creare record di fatturazione</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>Stato record della fatturazione</td> 
   <td> <p>In un Record della fatturazione oppure rapporto Ora, lo Stato di un record della fatturazione indica se questo è stato Fatturato o Non fatturato. Non puoi eliminare un progetto o modificare l’ora associata a un record di fatturazione fatturato. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Creare record di fatturazione</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Branding]</td> 
   <td><p>Il processo di personalizzazione di [!DNL Workfront] per dare all’interfaccia un aspetto che riflette l’azienda utilizzandone i colori e i loghi.</p><p><strong>NOTA</strong><br>Se la tua organizzazione ha effettuato l’onboarding su [!DNL Adobe Experience Cloud], il branding non è disponibile.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Breadcrumb]</td> 
   <td> <p>L’area nella parte superiore della pagina che mostra la posizione gerarchica in cui si trova l’utente nell’applicazione.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Per ulteriori informazioni, consulta <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Panoramica dei breadcrumb</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stato budget]</td> 
   <td> <p>Questo campo è obsoleto. Qualsiasi informazione visualizzata in questo campo è correlata a una funzione rimossa da [!DNL Workfront] e non è possibile aggiornare il campo. </p> <p>Questo campo mostra se il progetto è stato aggiunto alla [!UICONTROL Pianificazione capacità] e se il relativo calcolo del budget è stato completato. [!UICONTROL Pianificazione capacità] è stato rimosso da [!DNL Workfront]. </p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is  not added to the capacity planner, its value is <i>Not Included</i>.  </li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is  added to the Capacity Planner but is excluded from the budget calculation,  the value is <i>Included but not Calculated</i>.  </li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is  added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Raggruppamento]</td> 
   <td> <p>Nella Pianificazione di Workfront puoi visualizzare i record connessi nella vista timeline di un record utilizzando la funzione Raggruppamento. </p>
   <p>Il raggruppamento dei record in base alle relative connessioni consente di visualizzare le timeline degli altri record connessi e di comprendere in che modo potrebbero interessare le prestazioni e le scadenze dei record. </p>
   <p>I record connessi vengono visualizzati nidificati sotto il rispettivo record. </p>
   <p>Per informazioni, consulta <a href="/help/quicksilver/planning/views/manage-the-timeline-view.md">Gestire la vista timeline</a>. </p>
   </td> 
    </tr>

<tr> 
   <td>[!UICONTROL Data di completamento preventivata]</td> 
   <td> <p>Questo campo è obsoleto. Qualsiasi informazione mostrata in questo campo è correlata a una funzione rimossa da [!DNL Workfront]. Questo campo non può essere aggiornato. </p>
   <p> Questo campo è ancora visibile nei rapporti e negli elenchi del [!UICONTROL progetto].</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo preventivato]</td>

<td> <p>Si tratta del costo associato al budget delle risorse del progetto. </p>
   <p>Il campo viene mostrato nelle seguenti aree di [!DNL Workfront] con i seguenti nomi:</p>
   <ul>
   <li><strong>[!UICONTROL Costo preventivato]</strong>: nel pannello [!UICONTROL Riepilogo caso di business]</li>
   <li><strong>[!UICONTROL Costo]</strong>: nelle aree [!UICONTROL Utilizzo] quando vengono visualizzate le informazioni per il [!UICONTROL Costo]</li>
   <li><strong>[!UICONTROL Costo preventivato progetto]</strong>: in elenchi e rapporti</li>
   </ul>   
    <p>Il [!UICONTROL Costo preventivato] del progetto viene calcolato con la formula seguente:</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Per ulteriori informazioni sul calcolo del [!UICONTROL Costo preventivato] e per comprendere i vari termini relativi a questo concetto in [!DNL Workfront], consulta <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calcolare il costo preventivato del progetto</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ore preventivate]</td> 
   <td> <p>Le ore preventivate per le risorse relative al lavoro da completare sui progetti. Questo campo si riferisce alle ore preventivate nell’area [!UICONTROL Budget risorse] del [!UICONTROL Caso di business] (o nella [!UICONTROL Pianificazione risorse]) per il progetto o per le risorse del progetto.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Informazioni sul [!UICONTROL Costo preventivato della manodopera] e [!UICONTROL Ore preventivate] dei progetti</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Per informazioni sul budget degli utenti nella [!DNL Resource Planner], consulta l’articolo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget per le risorse nella [!DNL Resource Planner] utilizzando le viste [!UICONTROL Progetto] e [!UICONTROL Ruolo]</a>. </p> 
    <p>Le ore preventivate nell’area [!UICONTROL Budget risorse] del [!UICONTROL Caso di business] o della [!UICONTROL Pianificazione risorse] vengono visualizzate nelle seguenti aree di [!DNL Workfront] e con i seguenti nomi:</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>Nome visualizzato per [!UICONTROL Ore preventivate]</strong></td> 
        <td><strong>Aree di [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Ore]</td> 
        <td>Area [!UICONTROL Budget risorse] del [!UICONTROL Caso di business]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Pianificazione risorse] visualizzata per [!UICONTROL Ore]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Ore preventivate]</td> 
        <td> <p>Vista rapporto di utilizzo [!UICONTROL Ore]</p> <p>Per ulteriori informazioni sul rapporto di [!UICONTROL Utilizzo], consulta l’articolo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Panoramica del rapporto [!UICONTROL Utilizzo risorse]</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Ore preventivate]</td> 
        <td> <p>Rapporto [!UICONTROL Ora preventivata]</p><p>L’oggetto [!UICONTROL Ora preventivata] nel rapporto Ore preventivate fa riferimento a informazioni correlate a uno strumento di gestione delle risorse obsoleto. In questo rapporto, solo il campo “[!UICONTROL Ore preventivate]” si riferisce alle ore preventivate nell’area [!UICONTROL Pianificazione risorse] o [!UICONTROL Budget risorse] del [!UICONTROL Caso di business] del progetto. </p> <p>Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un rapporto personalizzato</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Ore preventivate per pianificazione risorse] </td> 
        <td> <p>Disponibile nei seguenti rapporti:</p>
        <ul>
        <li>Rapporto [!UICONTROL Progetto]
        <li>Rapporto [!UICONTROL Progetto (Dati finanziari)]
        <li>Rapporto [!UICONTROL Attività]
        <li>Rapporto [!UICONTROL Problema]
        <li>Rapporto [!UICONTROL Ora preventivata]</li>
        </ul>
         <p>Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un rapporto personalizzato</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Qualsiasi altra menzione di [!UICONTROL Ore preventivate] in [!DNL Adobe Workfront] fa riferimento alle ore preventivate utilizzando funzioni obsolete che sono state rimosse da Workfront. Si tratta di campi di sola visualizzazione che non vengono aggiornati con le informazioni correnti durante l’utilizzo degli strumenti di budget delle risorse correnti. </p>
    <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the  Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy  Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy  Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial  Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task  report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul> --> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo manodopera preventivato]</td> 
   <td> <p>Questo è il costo associato alle ore che tu, in qualità di manager risorse, preventivi per le mansioni relative al lavoro da completare nei progetti. </p> <p>In un rapporto di progetto, il [!UICONTROL Costo manodopera preventivato] viene calcolato utilizzando la formula seguente:</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Questo campo può fare riferimento a quanto segue:</p> 
    <ul> 
     <li> <p>I costi della manodopera mostrati nell’area [!UICONTROL Budget risorse] del [!UICONTROL Caso di business] o nella [!UICONTROL Pianificazione risorse] associati al costo delle mansioni in un progetto. Per informazioni sul calcolo di [!UICONTROL Costo manodopera preventivato], consulta l’articolo <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Informazioni sul costo manodopera preventivato] e [!UICONTROL Ore preventivate] dei progetti</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>I costi della manodopera mostrati nell’area [!UICONTROL Budget risorse] del [!UICONTROL Business case] che riflettono i [!UICONTROL Costi personale] stimati in un’iniziativa collegata al progetto da [!DNL Scenario Planner] quando utilizzi Pianificazione scenari per prevntivare le risorse del progetto. Per informazioni sulle iniziative, consulta <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Panoramica delle iniziative in Pianificazione scenari</a>. </p> <p>[!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], consulta <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Panoramica di [!DNL Scenario Planner]</a>. </p> </li> 
     <p>Viene visualizzata nelle seguenti aree con i seguenti nomi:</p>
   <ul>
   <li><strong>[!UICONTROL Costo manodopera preventivato]</strong>: nell’area [!UICONTROL Budget risorse] del [!UICONTROL Caso di business].
   <li><strong>[!UICONTROL Costo preventivato]</strong>: nella vista [!UICONTROL Costo] del rapporto di [!UICONTROL Utilizzo]
   <p>Per ulteriori informazioni, consulta <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Visualizzare le informazioni sull’utilizzo delle risorse </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: nelle viste del progetto di [!DNL Resource Planner] o [!DNL Role], durante la visualizzazione per costo
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: nei seguenti rapporti: 
   <ul>
    <li>Rapporto [!UICONTROL progetto]</li>
    <li>Rapporto [!UICONTROL Progetto (Dati finanziari)]</li>
    <li>Rapporto [!UICONTROL Attività]</li>
    <li>Rapporto [!UICONTROL Problema]</li>
    <li>Rapporto [!UICONTROL Ora preventivata]</li> 
    </ul>
    <p>Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un rapporto personalizzato</a>.</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in  Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task  report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task  report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>  .  </p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Data di inizio preventivata]</td> 
  <td> <p>Questo campo è obsoleto. Qualsiasi informazione mostrata in questo campo è correlata a una funzione rimossa da [!DNL Workfront]. Questo campo non può essere aggiornato.</p>
  <p>Queste aree sono state rimosse da [!DNL Workfront]. </p> 
  <p>Il campo è ancora visibile nei rapporti e negli elenchi del [!UICONTROL progetto].</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Grafico lavoro]</td> 
   <td>Grafico a linee che fornisce una rappresentazione visiva del lavoro completato e rimanente.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Caso di business]</td> 
   <td> <p>Strumento utilizzato per valutare se un progetto deve essere spostato dallo stato [!UICONTROL Idea] allo stato successivo [!UICONTROL Pianificazione]. In altre parole, un [!UICONTROL caso di business] aiuta l’organizzazione a decidere se sia utile avviare e completare il progetto o meno, soprattutto quando vengono confrontati i progetti con altri presenti in un portfolio.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Creare un [!UICONTROL Caso di business] per un progetto </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ore preventivate caso di business]</td> 
   <td> <p>Questo campo è obsoleto. Qualsiasi informazione mostrata in questo campo è correlata a una funzione rimossa da [!DNL Workfront]. Questo campo non può essere aggiornato.</p> <p>Questo campo è ancora visibile negli elenchi e nei rapporti di progetti e [!UICONTROL attività]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assegnazione calcolata]</td> 
   <td> <p>Uno dei [!UICONTROL Tipi di durata]. In questo modo verrà calcolata la percentuale di un giorno lavorativo di 8 ore che verrà allocata all’utente assegnato all’attività per tale attività, in base alla [!UICONTROL Durata] dell’attività e al [!UICONTROL Lavoro richiesto].</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica della [!UICONTROL Durata] e del [!UICONTROL Tipo di durata] dell’attività</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lavoro calcolato]</td> 
   <td> <p>Uno dei [!UICONTROL Tipi di durata]. In questo modo verrà calcolato il [!UICONTROL Lavoro richiesto] di un’attività, date le percentuali di [!UICONTROL Durata] e di [!UICONTROL Assegnazione] utente (in base a un giorno lavorativo di 8 ore).</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica della [!UICONTROL Durata] e del [!UICONTROL Tipo di durata] dell’attività</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendario]</td> 
   <td> <p>In Workfront, un rapporto calendario è un rapporto dinamico in cui gli utenti possono visualizzare la data e altri dettagli importanti di un evento, tra cui la data di scadenza, lo stato del lavoro e l’utente a cui è assegnato l’evento.</p> <p> Per ulteriori informazioni sui rapporti del calendario, consulta <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Panoramica dei rapporti del calendario</a>.</p>
   <p> In Pianificazione di Workfront, una vista Calendario è un tipo di vista per un tipo di record che mostra i record in un calendario. Per accedere a Pianificazione di Workfront devi disporre di una licenza aggiuntiva. </p>
    </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Può iniziare]</td> 
   <td> <p>Questo campo indica se un’attività è pronta per iniziare a essere elaborata. Se l’inizio è pronto per essere elaborato, sul campo [!UICONTROL Può iniziare] sull’attività è impostato [!UICONTROL True]. </p> <p>Per ulteriori informazioni, consulta la panoramica del campo <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">“[!UICONTROL Può iniziare]” per le attività</a>.</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    --> <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.  </li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.  </li> 
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
   <td> <p>Il tempo disponibile di una risorsa per l’allocazione al lavoro. Consulta “Disponibilità”. </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Categoria]</p> </td> 
   <td> <p>Una categoria è un modulo personalizzato. Puoi generare rapporti per questo oggetto e visualizzarlo anche in altri rapporti dell’oggetto. Non tutti gli oggetti possono avere un modulo personalizzato o una categoria. I seguenti oggetti possono avere un modulo personalizzato: <br></p> 
    <ul> 
     <li>[!UICONTROL Progetto]</li> 
     <li>[!UICONTROL Attività]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Documento]</li> 
     <li>[!UICONTROL Spesa]</li> 
     <li>[!UICONTROL Programma]</li> 
     <li>[!UICONTROL Utente]</li> 
     <li>[!UICONTROL Azienda]</li> 
     <li>[!UICONTROL Iterazione]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome categoria]</td> 
   <td> <p>Quando vengono aggiunti come colonna alla vista di uno dei seguenti oggetti, viene visualizzato un elenco di tutti i moduli personalizzati associati a tali oggetti:</p> 
    <ul> 
     <li>[!UICONTROL Progetto]</li> 
     <li>[!UICONTROL Attività]<br></li> 
     <li>[!UICONTROL Problema]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL Documento]<br></li> 
     <li>[!UICONTROL Spesa]<br></li> 
     <li>[!UICONTROL Programma]<br></li> 
     <li>[!UICONTROL Utente]<br></li> 
     <li>[!UICONTROL Azienda]</li> 
     <li>[!UICONTROL Iterazione]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Gestione del cambiamento]</td> 
   <td>Un’area di pratica incentrata sulla definizione, la comprensione e l’adattamento del lavoro pianificato ai cambiamenti di ambito, pianificazione, costi e fattori delle risorse.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ordine di modifica]</td> 
   <td>Tipo di problema sollevato in relazione a un progetto che illustra una richiesta di cambiamento dell’ambito concordato.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Solo Modifica]</td> 
   <td>Uno dei [!UICONTROL Tipi di aggiornamento] del progetto. Aggiorna le timeline di [!UICONTROL Progetto previsto] e [!UICONTROL Pianificato] solo quando vengono effettuati aggiornamenti alle attività o apportate modifiche nel progetto o nelle attività.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordine di modifica]</td> 
   <td> <p>Uno dei tipi di [!UICONTROL Problema], che in genere indica la necessità di svolgere una quantità di lavoro non pianificata prima che il progetto possa essere completato.</p> <p>Per ulteriori informazioni sui tipi di [!UICONTROL Problema], consulta la sezione “Tipi di problemi predefiniti” nell’articolo <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Personalizzare i tipi di problemi predefiniti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività secondaria]</td> 
   <td>Un’attività che è una [!UICONTROL Attività secondaria] di un’[!UICONTROL Attività principale] ([!UICONTROL Attività di riepilogo]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Secondarie]</td> 
   <td>L’insieme di [!UICONTROL Attività secondarie] in un’[!UICONTROL Attività principale] ([!UICONTROL Attività di riepilogo]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] e [!UICONTROL Formazione]</td> 
   <td>Moduli di apprendimento, certificazioni, standard o una community di pratica.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Impegno]</td> 
   <td>Strumento di comunicazione che consente agli utenti di impostare le aspettative relative ai deliverable delle attività.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di impegno]</td> 
   <td>Strumento di comunicazione che consente agli utenti di impostare le aspettative relative ai deliverable delle attività.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comunicazione] e [!UICONTROL Reporting]</td> 
   <td>Standard per la revisione delle eccezioni e dello stato di un progetto, programma o portfolio</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Azienda]</td> 
   <td> <p>Una [!UICONTROL Azienda] è un’unità organizzativa in [!DNL Workfront]. </p> 
   <p> Puoi associare un utente o un progetto a un’azienda. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Creare e modificare le aziende</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di completamento]</td> 
   <td> <p>La data di completamento prevista per un progetto, un’attività o un problema. Esistono diversi tipi di [!UICONTROL Date di completamento] in [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL Data di completamento effettiva]. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Panoramica della [!UICONTROL Data di completamento effettiva] del progetto</a>.</li> 
     <li>[!UICONTROL Data di completamento pianificata]. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Impostare la [!UICONTROL Data di completamento pianificata] del progetto</a> e <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Panoramica della [!UICONTROL Data di completamento pianificata] dell’attività</a>.</li> 
     <li>[!UICONTROL Data di completamento prevista]. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Panoramica della [!UICONTROL Data di completamento prevista] per progetti, attività e problemi</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Giorno di completamento]</td> 
   <td>Il giorno relativo all’inizio del [!UICONTROL Modello], in cui deve essere completata un’[!UICONTROL Attività modello] o un [!UICONTROL Modello].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modalità di completamento]</td> 
   <td> <p>Indica in che modo un progetto verrà contrassegnato come [!UICONTROL Completato]. Può avere due valori:</p> 
    <ul> 
     <li>[!UICONTROL Manuale]: un utente deve cambiare lo stato del progetto in [!UICONTROL Completato].</li> 
     <li>[!UICONTROL Automatico]: lo stato del progetto viene cambiata automaticamente in [!UICONTROL Completato] quando tutte le attività del progetto sono state completate al 100% e tutti i problemi sono chiusi.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condizione]</td> 
   <td> <p>Si tratta di una rappresentazione visiva dell’avanzamento di un’attività, un problema o un progetto.</p> <p>Per i progetti, la condizione può essere impostata manualmente dal proprietario del progetto oppure automaticamente da [!DNL Workfront], in base allo stato di avanzamento del progetto. </p> <p>I valori possibili per la condizione del progetto sono:</p> 
    <ul> 
     <li>[!UICONTROL In linea]</li> 
     <li>[!UICONTROL A rischio]</li> 
     <li>[!UICONTROL In difficoltà]</li> 
    </ul> <p>Per ulteriori informazioni sulle condizioni del progetto, consulta l’articolo <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Panoramica della [!UICONTROL Condizione del progetto] e del [!UICONTROL Tipo di condizione]</a>.</p>
     <p>Puoi associare le condizioni di attività e problemi a un numero che può essere visualizzato nei rapporti. Negli elenchi seguenti vengono visualizzati i nomi e i numeri predefiniti per le condizioni di attività e problemi. L’amministratore di sistema può aggiornare i nomi delle condizioni e aggiungerne di nuove con numeri diversi. Quando un numero è associato a una condizione, non può essere modificato.  </p> 
     <p>Per le attività, la condizione viene impostata manualmente dal proprietario dell’attività. I valori possibili per la condizione di attività sono:</p> 
    <ul> 
     <li>[!UICONTROL Regolare] (0)<br></li> 
     <li> [!UICONTROL Piccole difficoltà] (1)<br></li> 
     <li>[!UICONTROL Ostacoli critici] (2)</li> 
    </ul> <p>Per ulteriori informazioni sulle condizioni dell’attività, consulta l’articolo <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Aggiornare la [!UICONTROL Condizione] per le attività e i problemi</a>.</p> <p>Per i problemi, la condizione viene impostata manualmente dal proprietario del problema. I valori possibili per la condizione di problema sono:<br></p> 
    <ul> 
     <li>[!UICONTROL Regolare] (0)<br></li> 
     <li>[!UICONTROL Piccole difficoltà] (1)<br></li> 
     <li>[!UICONTROL Ostacoli critici] (2)</li> 
    </ul> 
   <p><b>NOTA</b></p>
    <p>Quando il campo [!UICONTROL Condizione] viene tracciato nei rapporti di [!UICONTROL Voce diario], i [!UICONTROL Valori numerici precedenti] e i [!UICONTROL Nuovi] mostrano il numero associato alla condizione anziché il nome. Se per una condizione non è stata originariamente definita per un’attività o un problema e successivamente viene aggiornata, la voce diario che acquisisce l’aggiornamento mostrerà il [!UICONTROL Valore numerico precedente] del campo [!UICONTROL Condizione] come -2.147.483.648. Consulta anche “[!UICONTROL Nuovo valore numerico]”, “[!UICONTROL Valore numerico precedente]” e “[!UICONTROL Voce diario]” in questo articolo. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggiornamento condizione]</td> 
   <td> <p>Questo campo mostra la condizione corrente delle attività, dei progetti o dei problemi. Questa opzione mostra gli aggiornamenti più recenti forniti dai proprietari di attività, progetti o problemi nel campo [!UICONTROL Stato aggiornamento], insieme alla nuova condizione.</p> <p>I commenti aggiunti agli aggiornamenti delle condizioni non vengono visualizzati nella colonna [!UICONTROL Aggiornamento condizione], ma solo nell’aggiornamento principale.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Tipi di record collegati]</td> 
   <td> <p>In Pianificazione di Workfront puoi creare una connessione tra uno dei seguenti elementi: </p>
   <ul>
   <li>Due tipi di record</li>
   <li>Un tipo di record e un tipo di oggetto Workfront</li>
   <li>Un tipo di record e una risorsa Adobe Experience Manager</li></ul>
   <p>La connessione dei tipi di record consente di visualizzare le informazioni di un record o di un tipo di oggetto su un altro tipo di record.</p>
   <p>Per informazioni, consulta <a href="/help/quicksilver/planning/architecture/connect-record-types-overview.md">Panoramica dei tipi di record collegati</a>  </p>
  <p>Pianificazione di Workfront richiede una licenza aggiuntiva. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Record connessi]</td> 
   <td> <p>In Pianificazione di Workfront, dopo aver connesso due tipi di record, puoi collegare tra loro due singoli record di tali tipi.  </p>
   <p>La connessione dei record consente di visualizzare le informazioni di un record o di un oggetto di un’altra applicazione su un altro record.</p>
   <p>Per informazioni, consulta <a href="/help/quicksilver/planning/records/connected-records-overview.md">Panoramica dei record connessi</a>. </p>

<p>Pianificazione di Workfront richiede una licenza aggiuntiva. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Connessioni]</td> 
   <td> <p>In Pianificazione di Workfront le connessioni possono fare riferimento a tipi di record o a record connessi. Pianificazione di Workfront richiede una licenza aggiuntiva.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Data vincolo]</td> 
   <td> <p>Se utilizzi un [!UICONTROL Vincolo attività] associato a una data specifica, ad esempio [!UICONTROL Deve iniziare il], tale data specifica diventa la [!UICONTROL Data vincolo] dell’attività.</p> <p>I seguenti vincoli di attività aggiornano il campo [!UICONTROL Data vincolo]:</p> 
    <ul> 
     <li>[!UICONTROL Deve iniziare il]</li> 
     <li>[!UICONTROL Deve finire il]</li> 
     <li>[!UICONTROL Iniziare non oltre il]</li> 
     <li>[!UICONTROL Iniziare non prima del]</li> 
    </ul> <p><b>SUGGERIMENTO</b></p>   
     <ul> 
      <li> <p>Un’attività con [!UICONTROL Vincolo] di [!UICONTROL Date fisse] non ha una [!UICONTROL Data vincolo]. </p> </li> 
      <li> <p> La [!UICONTROL Data vincolo] è visualizzabile solo in un rapporto o in una vista personalizzata.</p> </li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Giorno vincolo]</td> 
   <td> <p>Se utilizzi un vincolo attività in un’attività modello associata a un giorno specifico, ad esempio Deve iniziare il, tale giorno specifico diventa il giorno vincolo dell’attività modello.</p> <p>I seguenti vincoli di attività aggiornano il campo [!UICONTROL Giorno vincolo]:</p> 
    <ul> 
     <li>[!UICONTROL Deve iniziare il]</li> 
     <li>[!UICONTROL Deve finire il]</li> 
     <li>[!UICONTROL Iniziare non oltre il]</li> 
     <li>[!UICONTROL Iniziare non prima del]</li> 
    </ul> <p><b>SUGGERIMENTO</b></p> <p>  Il [!UICONTROL Giorno vincolo] è visualizzabile solo in un rapporto o in una vista personalizzata. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di vincolo]</td> 
   <td> <p>La tendenza di programmazione di un’attività. Ad esempio, [!UICONTROL Il prima possibile] pianificherà un’attività in modo che inizi il prima possibile e [!UICONTROL Termina non oltre il] pianificherà un’attività in modo che venga completata entro la [!UICONTROL Data vincolo] e non oltre.</p> <p>Per ulteriori informazioni, consulta la <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">panoramica del [!UICONTROL Vincolo attività]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Menu contestuale]</td> 
   <td>Un menu, situato sul lato sinistro dello schermo, in cui le voci vengono modificate in modo da essere correlate ai contenuti attivi. Ad esempio, quando un utente visualizza un progetto, il [!UICONTROL Menu contestuale] mostrerà collegamenti a informazioni e strumenti relativi al progetto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Referente problema convertito]</td> 
   <td>Un campo in un rapporto di progetti o attività che mostra informazioni sull’utente che è il [!UICONTROL Contatto principale] di un problema quando questo viene convertito in un progetto o in un’attività. Il campo viene visualizzato anche nella sezione [!UICONTROL Dettagli progetto] in cui viene visualizzato il nome del [!UICONTROL Contatto principale] del problema convertito. Consulta anche “[!UICONTROL Contatto principale]” in questo articolo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Costo]</td> 
   <td> <p>Importo monetario da spendere per il completamento di un progetto, attività o problema. </p> <p>Puoi tenere traccia di vari tipi di costi per manodopera, spese e rischi correlati al progetto.Per informazioni sul tracciamento dei costi in [!DNL Workfront], consulta <a href="../../../manage-work/projects/project-finances/track-costs.md">Tracciare i costi</a>.</p> 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Indice prestazioni costi (CPI)]</td> 
   <td> <p>L’[!UICONTROL Indice prestazioni costi (CPI)] descrive la relazione a livello di progetto o attività tra il costo pianificato e il costo effettivo. Questa metrica viene utilizzata dai project manager per tracciare eventuali scostamenti al di sotto o al di sopra del costo rispetto a singole attività o progetti in un determinato momento. Il costo può essere misurato in ore o in valuta, a seconda del [!UICONTROL Metodo degli indici delle prestazioni (PIM)].</p> 
    <p> Per informazioni, consulta <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-cpi.md">Calcolare l’Indice delle prestazioni dei costi (CPI)</a>.</p>

</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Indice delle prestazioni di pianificazione dei costi (CSI)]</td> 
   <td> <p>L’[!UICONTROL Indice prestazioni di pianificazione dei costi (CSI)] è un calcolo automatico che combina l’[!UICONTROL Indice prestazioni dei costi (CPI)] e l’[!UICONTROL Indice prestazioni della pianificazione (SPI)] in un’unica metrica generale che bilancia costi e pianificazione. Moltiplicando insieme questi valori, una singola metrica può rappresentare una pianificazione prolungata con un budget inferiore o viceversa. I project manager possono utilizzarla per determinare lo stato generale del progetto o dell’attività quando il costo viene sacrificato per prouovere alla pianificazione di metà progetto.</p> 
    <p> Per informazioni, consulta <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-csi.md">Calcolare l’indice delle prestazioni della pianificazione dei costi</a>.</p>
    </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Tipo di costo]</td> 
   <td>Per un’attività, il [!UICONTROL Tipo di costo] determina la modalità di maturazione dei costi. Alcuni esempi includono [!UICONTROL Ora fissa], [!UICONTROL Ore per utente] e [!UICONTROL Ore per utente più Fisse]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dipendenze tra progetti]</td> 
   <td> <p>Un’attività di un progetto dipende da un’attività di un progetto diverso.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Creare predecessori tra progetti</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Dati personalizzati]</td> 
   <td> <p>I dati univoci di un’organizzazione. Le organizzazioni possono personalizzare l’applicazione [!DNL Workfront] creando moduli e campi personalizzati. Queste informazioni personalizzate possono promuovere il reporting per una combinazione di KPI, auditing e domanda. </p> <p>[!UICONTROL Dati personalizzati] può essere collegato a:</p> 
    <ul> 
     <li>[!UICONTROL Progetti]</li> 
     <li>[!UICONTROL Attività]</li> 
     <li>[!UICONTROL Utenti]</li> 
     <li>[!UICONTROL Aziende]</li> 
     <li>[!UICONTROL Problemi]</li> 
     <li>[!UICONTROL Documenti]</li> 
     <li>[!UICONTROL Spese]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Programmi]</li> 
     <li>[!UICONTROL Iterazioni]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di dati personalizzati]</td> 
   <td>Opzione per specificare se un campo [!UICONTROL Dati personalizzati] è archiviato nel database come testo, data, numero o valuta.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di visualizzazione personalizzata]</td> 
   <td>Il tipo di visualizzazione di un campo personalizzato. Gli esempi includono [!UICONTROL Menu a discesa], [!UICONTROL Campo di testo], [!UICONTROL Area di testo], [!UICONTROL Pulsanti di scelta], ecc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campo personalizzato]</td> 
   <td>Per i dati personalizzati che consentono all’utente di selezionare tra diverse opzioni, questi sono i valori da cui un utente può effettuare le selezioni. Le opzioni personalizzate sono valide solo in [!UICONTROL Menu a discesa], [!UICONTROL Menu a discesa a selezione multipla], [!UICONTROL Pulsanti di scelta] e [!UICONTROL Caselle di controllo].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Etichetta modulo personalizzato]</td> 
   <td>Quando utilizzi un tipo di visualizzazione personalizzata con opzioni personalizzate, questo è il testo dell’interfaccia utente che verrà visualizzato nel menu a discesa, nelle caselle di controllo o nei pulsanti di scelta relative a tale opzione personalizzata.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valore personalizzato]</td> 
   <td>Quando utilizzi un campo personalizzato con opzioni personalizzate, questo è il valore che verrà archivato nel database per una particolare opzione.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vista personalizzata]</td> 
   <td>La definizione dei campi dati o delle colonne visualizzate per ciascun oggetto di un elenco.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cliente]</td> 
   <td>Un’rganizzazione che utilizza un’istanza di Workfront.</td> 
  </tr> 
 </tbody> 
</table>

## D - F

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome oggetto</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Dashboard]</td> 
   <td> <p> Puoi aggiungere questo campo in un rapporto o in una vista dell’oggetto del rapporto per visualizzare le dashboard in cui il rapporto è riportato in un elenco. </p> <p> Puoi utilizzare questo campo anche per filtrare i rapporti elencati in una dashboard specifica. </p> <p> Per ulteriori informazioni sull’inclusione delle informazioni della dashboard nei rapporti sull’oggetto del rapporto, consulta la sezione “Informazioni sui rapporti elencati nelle dashboard” nell’articolo <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Accedere e organizzare i rapporti</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di dati]</td> 
   <td>Consulta “[!UICONTROL Tipo di dati personalizzati]”.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Giorni di ritardo]</td> 
   <td> <p>Questo campo mostra una differenza di data tra [!UICONTROL Inizio pianificato] e [!UICONTROL Oggi] se manca la [!UICONTROL Data di completamento effettiva].</p> <p>Mostra anche una differenza di data tra [!UICONTROL Completamento effettivo] e [!UICONTROL Completamento pianificato], quando è presente una [!UICONTROL Data di completamento effettiva].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Pianificazione predefinita]</td> 
   <td> <p>Le ore di lavoro predefinite personalizzabili da assegnare a utenti e progetti all’interno di un’organizzazione. </p> <p>Le pianificazioni vengono utilizzate per calcolare le date pianificate, di inizio e di completamento delle attività assegnate agli utenti.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Derivable]</td> 
   <td>Beni o servizi quantificabili che devono essere forniti al completamento di un progetto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Gestione della domanda]</td> 
   <td>Punteggio e assegnazione delle priorità dei processi di acquisizione.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Obiettivi del reparto]</td> 
   <td>Obiettivi univoci per un reparto specifico che si incencentrano sul miglioramento delle metriche operative all’interno del reparto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dipendenza]</td> 
   <td>Il collegamento tra due attività che richiedono la modifica dello stato della prima affinché anche la seconda possa cambiare il proprio.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di dipendenza]</td> 
   <td> <p>Tipo di relazione di pianificazione tra un’attività e i relativi predecessori. Un esempio è [!UICONTROL Fine-Inizio], che richiede che la prima attività debba essere completata prima che la seconda possa iniziare.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Panoramica dei tipi di dipendenza tra attività</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Documento]</td> 
   <td>Qualsiasi file associato a un oggetto in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Versione del documento]</td> 
   <td> <p>Ogni volta che lo stesso documento viene caricato nello stesso oggetto, gli viene assegnato un numero di versione. Gli utenti possono visualizzare e modificare diverse opzioni relative a una versione precedente di un documento.</p> <p>Per ulteriori informazioni, consulta <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Gestire le versioni dei documenti</a>.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Data di scadenza]</td> 
   <td> <p>La data in cui un’attività o un problema deve essere completato. La data di scadenza di un’attività o di un problema corrisponde alla stessa data di completamento pianificata.</p>
    <p>La data di scadenza dell’attività e del problema è visibile nei relativi  elenchi e rapporti.</p> 
    <p>Consulta anche la data di completamento pianificata in questa tabella. 
    </td> 
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Durata]</td> 
   <td> <p>La finestra temporale allocata per il completamento di un problema dell’attività o di un progetto (come determinato dal numero di giorni tra [!UICONTROL Inizio pianificato] e Completamento pianificato).</p> 
    <ul> 
     <li>Per le attività, la Durata è un campo modificabile se il Tipo di durata dell’attività non è Semplice. Se il Tipo di durata dell’attività è Semplice o se il Vincolo attività è Date fisse, la Durata è un calcolo eseguito da Workfront.</li> 
     <li>Per i problemi, il campo Durata è sempre modificabile e deve rappresentare una stima di un numero di giorni necessari per la risoluzione del problema.</li> 
     <li>Per i progetti, la Durata è un calcolo eseguito da [!DNL Workfront] e rappresenta la differenza in giorni tra l’Inizio pianificato della prima attività e il [!UICONTROL Completamento pianificato] dell’ultima attività sul progetto.</li> 
    </ul> <p>Per ulteriori informazioni sulla differenza tra [!UICONTROL Durata] e [!UICONTROL Durata pianificata] per le attività, consulta l’articolo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Differenza tra [!UICONTROL Durata pianificata] e [!UICONTROL Durata] per le attività</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Durata in minuti]</td> 
   <td>Questo campo mostra le stesse informazioni di quello [!UICONTROL Durata] in minuti anziché in giorni. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Durata per occorrenza]</td> 
   <td> <p>Questa viene visualizzata nelle caselle [!UICONTROL Dettagli attività] e [!UICONTROL Modifica attività] di un elemento principale di attività ricorrenti. Visualizza la durata di ciascuna attività ricorrente. Per informazioni sulla creazione di attività ricorrenti, consulta <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Creare attività ricorrenti</a>. </p> <p> <span>Le durate modificate in singole attività ricorrenti non mostrano il valore indicato in questo campo.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Tipo di durata]</td> 
   <td> <p>Un campo dell’attività che indica il modo in cui il lavoro necessario per completare l’attività viene allocato agli assegnatari per tutta la durata della stessa. Rappresenta la relazione tra la [!UICONTROL Durata] dell’attività, il [!UICONTROL Lavoro richiesto] e la quantità di tempo, o [!UICONTROL Allocazione], che le risorse assegnate devono dedicare all’attività per completarla. </p> <p>Questo campo viene visualizzato nella scheda [!UICONTROL Dettagli] di un’attività. </p> <p>Le opzioni per il Tipo di durata di un’attività sono:</p> 
    <ul> 
     <li>[!UICONTROL Assegnazione calcolata]</li> 
     <li>[!UICONTROL Lavoro calcolato]</li> 
     <li>[!UICONTROL In base all’impegno]</li> 
     <li>[!UICONTROL Semplice]</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica della [!UICONTROL Durata] e del [!UICONTROL Tipo di durata] dell’attività</a>.</p> 
    --&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Unità di durata]</td> 
   <td>L’unità utilizzata per misurare il tempo in una ricerca avanzata.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL In base all’impegno]</td> 
   <td>La relazione tra il numero di utenti e il tempo necessario per il completamento dell’attività. Man mano che aggiungi più utenti, il tempo totale pianificato per il completamento dell’attività diminuisce, ma la durata dell’attività rimane invariata. Ad esempio, se un’attività consiste nello sgusciare un barile di arachidi, l’aggiunta di più persone ridurrà il tempo pianificato, ma la durata in giorni-persona rimarrà la stessa.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo trascorso]</td> 
   <td> <p>Il [!UICONTROL Tempo trascorso] è un’unità di tempo per la [!UICONTROL Durata] di un’attività. È l’intervallo di tempo compreso tra [!UICONTROL Data di inizio pianificata] e [!UICONTROL Data di completamento pianificata] di un’attività che include festività, fine settimana e indisponibilità. In altre parole, il tempo trascorso indica il passaggio effettivo dei giorni solari. </p> <p>[!DNL Workfront] supporta le seguenti unità di tempo trascorso per la durata dell’attività:</p> 
    <ul> 
     <li> <p>[!UICONTROL Minuti trascorsi]</p> </li> 
     <li> <p>[!UICONTROL Ore trascorse]</p> </li> 
     <li> <p>[!UICONTROL Giorni trascorsi]</p> </li> 
     <li> <p>[!UICONTROL Settimane trascorse]</p> </li> 
     <li> <p>[!UICONTROL Mesi trascorsi]</p> </li> 
    </ul> <p>Per ulteriori informazioni sulla durata dell’attività, compreso il tempo trascorso, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica della [!UICONTROL Durata] e del [!UICONTROL Tipo di durata] dell’attività</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di fine]</td> 
   <td> <p> In un rapporto [!UICONTROL Tariffa], indica la data di fine di una nuova tariffa di fatturazione per una mansione a livello di progetto. Le ore associate al progetto precedenti a questa data vengono moltiplicate per questa tariffa di fatturazione per calcolare le entrate del progetto. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Coinvolgimento]</td> 
   <td>[!UICONTROL Indicatore prestazioni del lavoro] (WPI) che indica quando l’impegno e la fiducia nell’attività, nel progetto, nel team o nell’organizzazione stanno calando. ndica la necessità di intervenire per ripristinare la fiducia e l’impegno. Per misurare il WPI, basterebbe porre delle semplici domande: “Hai compreso cosa ci si aspetta da te? Il lavoro che ti è stato assegnato ha fatto la differenza per l’organizzazione? Hai fatto un ottimo lavoro?”</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Obiettivi aziendali]</td> 
   <td>Obiettivi interfunzionali che contribuiscono alle metriche degli obiettivi aziendali.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Stima al completamento]</td> 
   <td><p>Come metrica delle prestazioni di un progetto, la Stima al completamento (EAC) rappresenta il costo totale previsto del progetto o dell’attività al completamento.</p>
   <p>Come impostazione di progetto, ti consente di definire come deve essere calcolato il valore EAC.</p>
   <p>Per informazioni, consulta <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-eac.md">Calcolare la stima al completamento (EAC)</a>. </p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Data di scadenza stimata]</td> 
   <td>Nei rapporti relativi a progetti, attività e problemi, la data di scadenza stimata è la data entro la quale Workfront stima che l’elemento debba essere completato.</td> 
  </tr>


<tr> 
   <td>[!UICONTROL Evento]</td> 
   <td>Qualsiasi modifica apportata a un progetto o a un’attività.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Handler di eventi]</td> 
   <td>Attività automatizzate che si attivano quando si verificano gli Eventi. Un esempio comune è una notifica e-mail automatizzata.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notifica evento]</td> 
   <td>E-mail generata da un handler di eventi.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Spese]</td> 
   <td>Costo non di manodopera per attività o progetti.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Esterno]</td> 
   <td> <p>In genere, questo è un tipo di licenza o un utente in possesso di tale licenza. Un utente in possess di questo tipo di licenza può solo rivedere le informazioni contenute nel sistema. Non può partecipare attivamente al lavoro.</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront]Panoramica delle licenze</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sistema esterno]</td> 
   <td>Qualsiasi servizio o software archiviato e gestito al di fuori del sistema di record designato.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Campo]</td> 
   <td><p>Qualsiasi oggetto Workfront o le informazioni ad esso associate, così come sono visualizzate nel database. </p>
   <p>Ad esempio, “progetto”, “utente”, “ora” sono sia oggetti di Workfront che campi. “Nome”, “stato”, “proprietario”, “data di inizio” sono campi di Workfront associati agli oggetti precedenti. </p>

<p>Quando viene fatto riferimento a un oggetto, i termini “oggetti” e “campi” possono essere utilizzati in modo intercambiabile.</p>
   <p>Nell’ambito del reporting, i “campi” si riferiscono agli oggetti o alle informazioni sull’oggetto che desideri acquisire nel rapporto.</p>

<p><b>NOTA</b></p>

<p>Nel reporting in modalità testuale, i campi fanno riferimento agli oggetti o alle relative informazioni così come vengono visualizzati nel database.</p>
   <p>A volte il nome visualizzato nell’interfaccia utente è diverso dal nome del campo nel database. Ad esempio, “problema” è il nome dell’oggetto nell’interfaccia di Workfront, ma “opTask” è il nome dell’oggetto (o del campo) nel database di Workfront. </p> 
   <p> È importante utilizzare il campo così come viene visualizzato nel database durante la scrittura di un raggruppamento, un filtro, una vista o un rapporto in modalità testo o durante la creazione di un campo calcolato.</p>

<p>Per ulteriori informazioni, consulta <a href="../../../wf-api/general/api-explorer.md">API Explorer</a> e <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">Panoramica della modalità di testo</a>.</p>

<p>Per impostazione predefinita, Workfront include un set di campi che definiscono sia gli oggetti che le relative informazioni. Inoltre puoi creare campi personalizzati per definire gli oggetti, ma non puoi creare oggetti personalizzati.</p>

<p>In Pianificazione di Workfront puoi creare campi personalizzati per tutti i tipi di record. I tipi di record Workfront sono disponibili con un numero molto limitato di campi. Dovrai creare tutti i campi da zero e associarli ai tipi di record. Per informazioni, consulta <a href="/help/quicksilver/planning/fields/fields-overview.md">Panoramica del campo</a>. </p> <p>Pianificazione di Workfront richiede una licenza aggiuntiva. </p>   
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filtro]</td> 
   <td> <p>Uno dei principali blocchi predefiniti di un rapporto o di un elemento elenco che definisce quali informazioni visualizzare sullo schermo. Per ulteriori informazioni sugli elementi di reporting, consulta <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementi di reporting: filtri, viste e raggruppamenti</a>.</p> <p>Il filtro determina i risultati visualizzati in un rapporto o in un elenco di pannelli di [!DNL Workfront], ad esempio progetti, attività o problemi.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Gestione finanziaria del lavoro]</td> 
   <td>Processo per gestire i dati relativi a costi di manodopera, spese e le entrate in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo fisso]</td> 
   <td>Puoi definire un importo di costo fisso per un progetto. Questo fa parte del [!UICONTROL Costo pianificato] del progetto che rappresenta la quantità di denaro necessaria per completare il progetto. Per informazioni sui costi, consulta <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tenere traccia dei costi</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Entrate fisse]</td> 
   <td>Puoi definire un importo di entrate fisso per un progetto. Questo fa parte delle [!UICONTROL Entrate pianificate] del progetto che rappresentano la quantità di denaro che potresti ottenere se completi il progetto. Per informazioni sulle entrate, consulta <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica della fatturazione e delle entrate</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Flag]</td> 
   <td> <p> Questo campo è uguale a [!UICONTROL Icone di stato], ma è disponibile solo per le viste seguenti: </p> 
    <ul> 
     <li> [!UICONTROL Modelli] </li> 
     <li> [!UICONTROL Spese] </li> 
    </ul> <p> Per ulteriori informazioni, consulta l’articolo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Icone di stato incorporate nelle viste</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella]</td> 
   <td>Le cartelle vengono utilizzate per organizzare documenti o rapporti associati a un oggetto.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (Equivalente a tempo pieno)</td> 
   <td>Si tratta dell’Equivalente a tempo pieno, che indica la quantità di tempo che una risorsa ha a disposizione per il lavoro. 
Il campo [!UICONTROL FTE] viene visualizzato nelle seguenti aree: 
  <ul>
   <li> Profilo dell’utente, durante la modifica o la creazione dell’utente </li>
   <li> [!UICONTROL Pianificazione risorse] </li>
   <li> [!UICONTROL Pianificazione scenari] (richiede una licenza aggiuntiva per la Pianificazione scenari di Workfront) </li>
   <li> Elenchi di utenti e rapporti </li> </ul>

<p>Il campo [!UICONTROL FTE] deve essere un numero decimale con un valore massimo di 1, ma non può essere 0. </p>
   <p> Un [!UICONTROL FTE] pari a 1 (impostazione predefinita per il campo [!UICONTROL FTE] di un utente, come definito nel relativo profilo) indica che una risorsa (utente o ruolo) lavora per l’intero numero di ore, in base alla pianificazione che ne calcola la disponibilità. </p>
   <p>L’amministratore di Workfront decide la pianificazione da utilizzare determinando la disponibilità dell’utente.  </p>
   <ul>
   <li> Quando viene utilizzata la [!UICONTROL Pianificazione predefinita], Workfront utilizza l’[!UICONTROL FTE] dell’utente trovato nel rispettivo profilo per calcolare la disponibilità. </li>
   <li> Quando viene utilizzata la Pianificazione dell’utente, Workfront utilizza le indisponibilità dell’utente, il valore del [!UICONTROL Tempo di lavoro] e le ore della [!UICONTROL Pianificazione predefinita] per calcolare l’[!UICONTROL FTE] dell’utente. </li> </ul>

<p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurare le preferenze di gestione delle risorse</a>.  </p>
   <p>Per ulteriori informazioni sulla creazione di pianificazioni in [!DNL Workfront], consulta <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Creare una pianificazione</a>. </p>

<p><b>NOTA</b></p>
   <p>Per tutti i calcoli in [!UICONTROL Pianificazione scenari], Workfront utilizza il valore seguente: 1 [!UICONTROL FTE] = 8 ore.</p>
   <p>Per ulteriori informazioni, consulta <a href="../../../scenario-planner/get-started-with-scenario-planning.md">Introduzione alla [!UICONTROL Pianificazione scenari]</a>. </p>
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
   <th>Nome oggetto</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Grafico di Gantt]</td> 
   <td> <p>Una timeline visiva delle date del progetto in una vista calendario basata sulle date pianificate o previste, nel modo in cui le attività del progetto sono attualmente pianificate.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Obiettivo]</td> 
   <td><p>Sono presenti due concetti di obiettivi in [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>Obiettivi del progetto</b>: un set di obiettivi aziendali concordati dagli stakeholder di un progetto. Gli obiettivi del progetto fanno parte del caso di business di un progetto. </p> <p>Non puoi visualizzare gli obiettivi del progetto in elenchi o rapporti, ma puoi accedervi tramite l’API. </p> <p>Per informazioni sugli obiettivi del progetto del caso di business, consulta <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Creare gli obiettivi del caso di business</a>. </p> </li> 
     <li> <p><b>Obiettivi strategici</b>: un obiettivo strategico è un obiettivo che crei per pianificare la tua strategia di lavoro per un periodo di tempo specificato. Puoi creare questi tipi di obiettivi utilizzando [!DNL Workfront Goals]. Per poter creare obiettivi strategici, la tua organizzazione dovrà acquistare una licenza aggiuntiva e tu dovrai disporre dell’accesso a questa funzione. [!DNL Workfront Goals] sono disponibili solo con una licenza aggiuntiva.</p> 
     <p>Per maggiori informazioni, consulta Panoramica di <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] </a>. </p> 
     <p>Puoi visualizzare gli obiettivi strategici in un rapporto di obiettivo o progetto e accedervi tramite l’API. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Gerarchia obiettivi]</td> 
   <td> <p>Nei rapporti [!UICONTROL Obiettivo] e [!UICONTROL Progetto], questo è un campo di raccolta che mostra gli obiettivi nella gerarchia a cui appartiene un obiettivo strategico quando è allineato ad altri obiettivi. Gli obiettivi sono separati da un delimitatore ▸. </p> <p>In questo campo vengono mostrati solo l’obiettivo e i rispettivi elementi principali. Gli obiettivi secondari non vengono mostrati. </p> <p>Per informazioni sull’allineamento degli obiettivi in [!DNL Workfront Goals], consulta <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Panoramica dell’allineamento degli obiettivi in [!DNL Workfront Goals]</a>. </p> 
   <p>Questo campo è visibile solo se la tua organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sulla gestione degli obiettivi strategici tramite [!DNL Workfront Goals], consulta Panoramica di <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Punteggio di successo dell’obiettivo]</td> 
   <td> In un [!UICONTROL Rapporto di progetto] questo campo faceva riferimento agli obiettivi a livello di progetto associati al caso di [!UICONTROL Business]. Attualmente, si tratta di un campo obsoleto e non è associato ad alcuna funzionalità.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Obiettivi] </td> 
   <td> <p>In un rapporto di [!UICONTROL Progetto], questo è un campo di raccolta che mostra tutti gli obiettivi strategici associati a un progetto. Gli obiettivi sono separati da virgole.</p> <p>Questo campo è visibile solo se la tua organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sulla gestione degli obiettivi strategici tramite [!DNL Workfront Goals], consulta Panoramica di <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] </a>. Per ulteriori informazioni sugli obiettivi strategici e di progetto in [!DNL Workfront], consulta “[!UICONTROL Obiettivo]” in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Preferenze dell’interfaccia globale]</td> 
   <td>Impostazioni dell’interfaccia che interessano tutti gli utenti. Le [!UICONTROL Preferenze dell’interfaccia globale] possono essere sovrascritte dalle [!UICONTROL Preferenze dell’interfaccia utente].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Gruppo]</td> 
   <td> <p>Un insieme di utenti (possibilmente dello stesso reparto o unità di business) che hanno accesso agli stessi oggetti. Oltre agli utenti, i gruppi possono essere associati a portfolio, programmi, progetti, <span> modelli di progetto,</span> azienda, team, pianificazioni, modelli layout e profili schede orario.</p> <p>Inoltre, puoi concedere autorizzazioni agli oggetti per gruppo. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Panoramica dei gruppi</a>.</p> <p>In un elenco o in un rapporto di oggetti di uno dei tipi seguenti puoi utilizzare il campo [!UICONTROL Gruppo] per elencare gli oggetti di quel tipo associati a un gruppo specifico: utente, portfolio, programma, progetto, <span>modello di progetto</span>, azienda, team, pianificazione, modello layout o profilo scheda orario.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Amministratore gruppo]</td> 
   <td> <p>Utenti che gestiscono gli oggetti, l’accesso e utenti di gruppi di utenti designati.</p> <p> In un rapporto di [!UICONTROL Gruppo], questo campo mostra i nomi degli utenti designati come [!UICONTROL Amministratori di gruppo] del gruppo. Per ulteriori informazioni sugli amministratori di gruppo, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gruppo con accesso amministratore]</td> 
   <td> <p> In un [!UICONTROL Modello layout], [!UICONTROL Profilo scheda orario] o [!UICONTROL Rapporto pianificato] questo campo mostra i gruppi i cui amministratori di gruppo hanno accesso per modificare il modello. Puoi anche filtrare il rapporto in base a questo campo. </p> <p> Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creare e gestire modelli layout</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Raggruppamento]</td> 
   <td> <p>Un elemento di reporting utilizzato per categorizzare le informazioni di un elenco in base a un criterio comune.</p> <p>Per ulteriori informazioni, consulta la sezione “[!UICONTROL Raggruppamenti]” nell’articolo <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementi di reporting: filtri, viste e raggruppamenti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di handoff]</td> 
   <td> <p>La data in cui un’attività diventa disponibile per il lavoro. La [!UICONTROL Data di handoff] è un calcolo e non può essere impostata manualmente. <br>Per ulteriori informazioni su [!UICONTROL Data di handoff], consulta l’articolo <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">Panoramica della [!UICONTROL Data di handoff dell’attività]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help desk]</td> 
   <td>Nome alternativo per descrivere l’area [!UICONTROL Richieste] di [!DNL Workfront]. Puoi utilizzare l’area [!UICONTROL Richieste] per elaborare i ticket di assistenza clienti, le richieste di progetto, i ticket dell’help desk e così via.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proprietario]</td> 
   <td>In un Rapporto [!UICONTROL Ore], l’utente a cui sono attribuite le ore è il [!UICONTROL Proprietario]. Questo è diverso dall’utente che registra effettivamente l’ora. Queste due entità possono a volte essere due utenti diversi. <br>Per ulteriori informazioni sulla registrazione delle ore per un altro utente, consulta l’articolo <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Registrare le ore</a>.</td> 
  </tr>

<tr> 
   <td>Stato delle Ore</td> 
   <td> <p>Un attributo impostato da Workfront per le ore effettive registrate dagli utenti per attività, problemi o progetti. </p>

Le voci relative alle ore possono avere uno dei seguenti stati in Workfront:
<ul>
   <li><b>Inviate</b>: le ore sono state registrate in un progetto, attività o problema. Fanno parte di un record di fatturazione o non sono ancora state aggiunte a un record della fatturazione.</li>
   <li><b>Approvate</b>: le ore sono state registrate e sono state approvate dal proprietario del progetto. Fanno parte di un record di fatturazione o non sono ancora state aggiunte a un record della fatturazione.</li> 
   <li><b>Non approvate</b>: le ore sono state registrate e rifiutate dal proprietario del progetto. Fanno parte di un record di fatturazione o non sono ancora state aggiunte a un record della fatturazione.</li>
   <li><b>Fatturate</b>: le ore sono state registrate, aggiunte a un record della fatturazione e lo stato del record è stato contrassegnato come Fatturato. Per queste ore non è necessaria l’approvazione da parte del proprietario del progetto.</li>
   <li><b>Fatturate e approvate</b>: le ore sono state registrate, approvate dal proprietario del progetto e lo stato del record della fatturazione è stato contrassegnato come Fatturato.</li>
   </ul>

<p>Quando le ore fanno parte di un record della fatturazione, lo Stato ore indica se le ore sono state approvate o se il record della fatturazione a cui appartengono è stato fatturato. Lo stato di un’ora è visibile solo in un elenco o in un rapporto ore. </p>

<p>Per ulteriori informazioni sull’aggiunta di ore ai record di fatturazione, consulta la sezione “Aggiungere ore ai record della fatturazione” nell’articolo <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Creare record della fatturazione</a>.</p>

<p>Per ulteriori informazioni sull’approvazione del tempo per i progetti, consulta <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Richiedere l’approvazione del tempo per un progetto</a>.</p>

<p><b>SUGGERIMENTO</b></p>

<p>Le ore generali non registrate direttamente sugli elementi di lavoro non mostrano uno Stato delle ore. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Tipo di ora]</td> 
   <td> <p>Un attributo che può essere impostato per le ore effettive registrate dagli utenti per attività, problemi o progetti. Questo è anche un attributo delle ore registrate che non sono collegate direttamente all’attività, ad esempio [!UICONTROL Vacanza] e [!UICONTROL Indisponibilità].</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Gestire i tipi di ore</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>L’ID è un indicatore alfanumerico associato a ogni oggetto in [!DNL Workfront]. Identifica in modo univoco ciascun oggetto nel database [!DNL Workfront]. Puoi visualizzare l’ID di qualsiasi oggetto in un rapporto o elenco di ciascun oggetto. </p> <p><b>SUGGERIMENTO</b></p>   <p>Puoi anche visualizzare l’ID nell’URL della pagina dell’oggetto. Ad esempio, l’ID di un progetto potrebbe avere un aspetto simile al numero indicato nel seguente URL, quando accedi alla pagina [!UICONTROL Dettagli progetto]:</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL IMS]</td> 
   <td>Identity Management System. Adobe IMS richiede di accedere a Workfront tramite Adobe, anziché con il nome utente e la password di Workfront.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Obiettivi individuali]</td> 
   <td>Obiettivi individuali che contribuiscono alle metriche degli obiettivi del team, ma che non sono correlati allo sviluppo personale o della carriera.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Accesso ereditato]</td> 
   <td>Funzione di condivisione che consente l’accesso per la propagazione da un oggetto a un altro. Ad esempio, l’accesso ereditato dell’utente del progetto definito nei record del programma e del portfolio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Iniziativa]</td> 
   <td> <p>In [!DNL Workfront Scenario Planner] puoi suddividere un piano in più iniziative per semplificarne la gestione. <span>Puoi creare un rapporto [!UICONTROL Iniziativa] e accedere alle informazioni [!UICONTROL Iniziativa] in un rapporto [!UICONTROL Progetto].</span></p> <p>[!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], consulta <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Panoramica di [!DNL Scenario Planner]</a>. </p> <p>Il rapporto [!DNL Initiative] non è visibile nell’istanza di [!DNL Workfront], a meno che la tua azienda non abbia acquistato una licenza [!DNL Workfront Scenario Planner]. Non puoi accedere alle [!UICONTROL Iniziative] tramite l’API.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Mansione iniziativa]</span> </td> 
   <td> <p><span>Il tipo di rapporto [!UICONTROL Mansione iniziativa] mostra le informazioni sulle mansioni associate a un’iniziativa del piano in [!DNL Workfront Scenario Planner].</span> </p> <p>[!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], consulta <a href="../../../scenario-planner/scenario-planner-overview.md">Panoramica di [!DNL Scenario Planner]</a>. </p> <p><span>Questo tipo di rapporto non è visibile nell’istanza di [!DNL Workfront], a meno che la tua azienda non abbia acquistato una licenza [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Ore per mansione iniziativa]</span> </td> 
   <td> <p><span> In un rapporto [!UICONTROL Mansione iniziativa], questo mostra il numero di ore associate a una mansione in un’iniziativa.</span> </p> <p>[!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], consulta <a href="../../../scenario-planner/scenario-planner-overview.md">Panoramica di [!DNL Scenario Planner]</a>. </p> <p>Questo campo e il tipo di rapporto [!UICONTROL Mansione iniziativa] non sono visibili nell’istanza di [!DNL Workfront], a meno che la tua azienda non abbia acquistato una licenza [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Conteggio mansioni iniziativa]</td> 
   <td> <p>In un rapporto [!UICONTROL Mansione iniziativa], mostra il numero di mansioni specifiche associate a un’iniziativa.</p> <p>[!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], consulta <a href="../../../scenario-planner/scenario-planner-overview.md">Panoramica di [!DNL Scenario Planner]</a>. </p> <p>Questo campo e il tipo di rapporto [!UICONTROL Mansione iniziativa] non sono visibili nell’istanza di [!DNL Workfront], a meno che la tua azienda non abbia acquistato una licenza [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data ultima pubblicazione dell’iniziativa]</td> 
   <td> <p>Campo in un rapporto [!UICONTROL Iniziativa], [!UICONTROL Mansione iniziativa] e [!UICONTROL Progetto] che mostra la data dell’ultima pubblicazione di un’iniziativa di piano in un progetto. Puoi pubblicare iniziative per creare o aggiornare progetti collegati alle iniziative.</p> <p>[!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], consulta <a href="../../../scenario-planner/scenario-planner-overview.md">Panoramica di [!DNL Scenario Planner]</a>. </p> <p><span>Per informazioni sulle iniziative di pubblicazione, consulta</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Scenari di pubblicazione per creare e aggiornare progetti in [!DNL Workfront Scenario Planner]</a>. Questo campo non è visibile nell’istanza [!DNL Workfront] a meno che l’azienda non abbia acquistato una licenza [!DNL Workfront Scenario Planner].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ricerca in linea]</td> 
   <td>Ricerca eseguita durante la compilazione di un modulo per trovare le voci possibili per un campo specifico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Configurazione interfaccia]</td> 
   <td>Area dell’applicazione che consente di definire viste personalizzate, filtri, raggruppamenti, controlli elenco e così via.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL È obiettivo aziendale]</p></td> 
   <td> <p>In [!DNL goal reports], mostra un valore “[!UICONTROL Vero]/ [!UICONTROL Falso]” per ogni obiettivo strategico per indicare se l’organizzazione è assegnata all’obiettivo come proprietario. </p> 
   <p>Questo campo è visibile solo se la tua organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sulla gestione degli obiettivi strategici tramite [!DNL Workfront Goals], consulta la panoramica <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Problema]</td> 
   <td> <p>Elemento di lavoro non pianificato che di solito indica che esiste un problema che impedisce il completamento di un’attività o di un progetto. Viene analizzato e valutato per ulteriori considerazioni relative all’impegno di lavoro.</p> <p>Un [!UICONTROL Problema] può anche essere una richiesta dell’[!UICONTROL Help Desk]. [!UICONTROL Ordini di modifica], [!UICONTROL Richieste] e [!UICONTROL Bug] sono anche [!UICONTROL Problemi].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Gestione problemi]</td> 
   <td> <p>Il processo e le regole che disciplinano la definizione dei tipi di problema e il processo di instradamento, analisi o traffico associato a ciascun tipo.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Proprietario del problema]</td> 
   <td>Il team o gli utenti responsabili di analizzare e completare un problema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iterazione]</td> 
   <td>Periodo di tempo in cui un team produce un set predefinito di deliverable.</td> 
  </tr> 
 </tbody> 
</table>

## J - L

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome oggetto</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Mansione]</td> 
   <td> <p>Utilizzato per identificare le mansioni lavorative e le responsabilità quotidiane di un utente. Le mansioni possono essere assegnate agli elementi di lavoro per identificare l’abilità necessaria per completare un processo di lavoro senza assegnarlo a un utente specifico. </p> <p>Un utente può avere più di una mansione. Alcuni esempi includono Graphic Designer o Consulente.</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire mansioni</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Voce diario]</p> </td> 
   <td> <p>Oggetto segnalabile che fornisce informazioni sugli aggiornamenti di sistema per i campi tracciati mostrati nell’area [!UICONTROL Aggiornamenti] di progetti, attività, problemi e altri oggetti.</p> <p>Per ulteriori informazioni, consulta <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Rapporto sull’area Aggiornamenti con un rapporto sulle voci diario</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contrassegno kanban]</td> 
   <td> <p>In un rapporto [!UICONTROL Attività] o [!UICONTROL Problema], il campo [!UICONTROL Contrassegno kanban] mostra lo stato del contrassegno impostato sulla storia nella [!UICONTROL Bacheca kanban]. I valori possibili sono [!UICONTROL Sotto controllo], [!UICONTROL Pronto per la fase successiva] e [!UICONTROL È bloccato].</p> <p>Per ulteriori informazioni sull’impostazione dello stato del contrassegno per le storie sulla [!UICONTROL Bacheca delle storie kanban], consulta l’articolo <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Usare i contrassegni sulle storie sulla [!UICONTROL Bacheca kanban]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI</td> 
   <td>Valore misurabile che dimostra l’efficacia con cui un’azienda raggiunge gli obiettivi aziendali chiave.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attesa]</td> 
   <td>Quantità di tempo che deve trascorrere dopo che la [!UICONTROL Data di completamento pianificata] dell’attività del predecessore è passata fino a quando l’attività dipendente può iniziare.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipi di attesa]</td> 
   <td> <p>Il metodo di calcolo dell’[!UICONTROL Attesa]. Può essere:</p> 
    <ul> 
     <li>[!UICONTROL Giorni] (giorni lavorativi)</li> 
     <li>[!UICONTROL Giorni di calendario] (ignora festività)</li> 
     <li>[!UICONTROL Percentuale]</li> 
     <li>[!UICONTROL Giorno della settimana]</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Panoramica dei tipi di attesa</a>.</p> </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Miniatura grande]</td> 
   <td> <p> In un elenco o rapporto del [!UICONTROL Documento] viene visualizzata un’anteprima del documento in una miniatura. </p> <p>Seleziona <strong>[!UICONTROL Miniatura grande]</strong> per visualizzare una miniatura di 400 pixel nel rapporto.</p> <p>Le dimensioni della miniatura vengono regolate modificando la larghezza della colonna in un elenco o in un rapporto.</p> <p>Consulta anche “[!UICONTROL Miniatura]” in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ultimi 10 visualizzatori]</td> 
   <td> <p>In un elenco di rapporti, questo campo mostra i nomi di un massimo di 10 utenti che hanno visualizzato il rapporto più di recente.<br>Per ulteriori informazioni sull’utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizzare l’utilizzo del rapporto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mota ultima condizione]</td> 
   <td> <p>In questo campo viene visualizzato l’ultimo aggiornamento immesso su un oggetto dal relativo proprietario. Si tratta dell’attività o dell’interazione più recente del proprietario su un oggetto.</p> <p>La colonna [!DNL Last Condition Note] è vuota se il testo della nota dell’ultima nota di un oggetto è stato eliminato. Quando una nuova nota inserita sull’oggetto diventa l’ultima nota e viene nuovamente visualizzata nella colonna.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data ultimo aggiornamento finanza]</td> 
   <td>In un rapporto di [!UICONTROL progetto], questo campo acquisisce la data e l’ora dell’ultimo calcolo e aggiornamento delle finanze del progetto. Per informazioni sulle finanze del progetto, consulta <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Panoramica delle finanze del progetto</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ultima nota]</td> 
   <td> <p>Questo campo mostra l’ultimo aggiornamento inserito su un oggetto da qualsiasi utente. Questa è l’attività o interazione più recente su un oggetto.</p> <p>La colonna [!UICONTROL Ultima nota] è vuota se il testo dell’ultima nota di un oggetto è stato eliminato. Una nuova nota inserita sull’oggetto diventa l’ultima nota e viene nuovamente visualizzata nella colonna.</p>
   <p>Quando questo campo viene aggiunto a un report [!UICONTROL Task], gli eventuali aggiornamenti rimasti sugli oggetti figlio, ad esempio problemi, sottoattività o documenti, dell'attività non vengono visualizzati in questa colonna.</p> 
   <p><b>NOTA</p>
   <p>L’ultima nota aggiunta a un oggetto utilizzando l’API non viene visualizzata in un rapporto in Workfront. Il campo [!DNL Last Note] è vuoto se è stato aggiunto l'ultimo aggiornamento su un oggetto utilizzando l'API. </p>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ultima visualizzazione di]</td> 
   <td> <p>In un elenco di rapporti, questo campo visualizza informazioni sull’ultimo utente che ha visualizzato il rapporto.<br>Per ulteriori informazioni sull’utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizzare l’utilizzo dei rapporti</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data ultima visualizzazione]</td> 
   <td> <p>In un elenco di rapporti, questo campo mostra la data dell’ultima visualizzazione del rapporto.<br>Per ulteriori informazioni sull’utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizzare l’utilizzo dei rapporti</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Modello layout]</td> 
   <td>Definito dall’amministratore di sistema o dall’amministratore gruppo per identificare le schede e i rapporti visualizzati nell’area di lavoro di un determinato utente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di layout]</td> 
   <td>Insieme alle [!UICONTROL Viste personalizzate], il [!UICONTROL Typo di layout] specifica il tipo di [!UICONTROL Vista personalizzata]. Attualmente, è disponibile solo l’elenco. In futuro, [!UICONTROL Dettaglio] (la visualizzazione [!UICONTROL Dettaglio] di un oggetto) potrebbe diventare disponibile.</td> 
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
       <br>If there  are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.   
     </p> </td> </tr> -->
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.  </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>    </p>
    --> </td> 
  </tr> 
  <tr> 
   <!-- <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection  of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ore effettive precedenti]</td> 
   <td> <p>In un rapporto di progetto, attività o problema, le [!UICONTROL Ore effettive precedenti] rappresentano la somma di tutte le ore registrate sul progetto, attività o problema in qualsiasi momento, anche prima di maggio 2021.</p>  
   <p>Le ore effettive precedenti vengono visualizzate come Ore effettive nell’area Dettagli del progetto, dell’attività o del problema. </p>
   <p>Consulta anche <strong>Ore effettive</strong>.
    <p>Per ulteriori informazioni, consulta <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md">Visualizzare le ore effettive</a>.</p>
    </td> 
  </tr>  <tr> 
   <td>[!UICONTROL Tipo di licenza]</td> 
   <td>Tipo di licenza allocata a un [!UICONTROL Livello di accesso]. È [!UICONTROL Utente con licenza Full], [!UICONTROL Utente limitato] o [!UICONTROL Richiedente].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite piano licenze]</td> 
   <td> <p>In una visualizzazione o in un rapporto di [!UICONTROL Gruppo], questo campo mostra il numero massimo di licenze [!UICONTROL Piano] che possono essere assegnate agli utenti che hanno il rispettivo gruppo designato come proprio [!UICONTROL Gruppo predefinito].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite licenze operative]</td> 
   <td> <p>In una visualizzazione o in un rapporto di [!UICONTROL Gruppo], questo campo mostra il numero massimo di licenze [!UICONTROL Lavoro] che possono essere assegnate agli utenti che hanno il rispettivo gruppo designato come proprio [!UICONTROL Gruppo predefinito].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utente limitato]</td> 
   <td>Tipo di licenza che consente la creazione di un [!DNL Access Level] che contiene privilegi di sola visualizzazione, con la possibilità di inviare problemi, inserire note e caricare documenti.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Controlli elenco]</td> 
   <td> <p>Parte della [!UICONTROL Configurazione interfaccia] che consente di collegare filtri, viste e raggruppamenti personalizzati a singoli utenti o a livello globale a tutti gli utenti.</p> </td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Campi di ricerca]</td> 
   <td> <p>In Pianificazione di Workfront, dopo aver stabilito la connessione tra due tipi di record e aver collegato i singoli record, puoi fare riferimento ai campi dei record collegati nel record da cui stai effettuando la connessione.</p>
   <p>Se ad esempio colleghi un tipo di record Campagna a un tipo di oggetto Progetto Workfront, puoi visualizzare il campo Budget dei progetti collegati nei record della campagna. Il campo Budget del progetto è un campo di ricerca dei progetti di una campagna.</p> <p>I valori dei campi di ricerca vengono compilati automaticamente nei record da cui sono connessi.</p>
   <p>Per informazioni, consulta <a href="/help/quicksilver/planning/records/connected-records-overview.md">Panoramica dei record connessi</a>.</p>
   <p>Pianificazione di Workfront richiede una licenza aggiuntiva.</p>
    </td> 
  </tr> 
 </tbody> 
</table>

## M - O

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome oggetto</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Solo manuale]</td> 
   <td> <p>Uno dei [!UICONTROL Tipi di aggiornamento] di un [!UICONTROL Progetto]. Questa impostazione consente di aggiornare le timeline di [!UICONTROL Progetto previsto] e [!UICONTROL Pianificato] solo quando viene fatto clic su “[!UICONTROL Timeline ricalcolate]”. I progetti impostati in questo modo verranno ignorati durante il processo di ricalcolo notturno e quando il progetto o le attività al suo interno vengono aggiornati.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selezionare il [!UICONTROL Tipo di aggiornamento] del progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>Si riferisce all’utente attualmente connesso. </p> <p>È consigliabile utilizzare questo campo in un filtro per rendere i rapporti più generici quando vengono condivisi con altri utenti. In questo modo, puoi creare un unico rapporto che mostrerà informazioni diverse a seconda di chi effettua l’accesso per visualizzarlo, poiché queste sono sempre personalizzate per l’utente connesso. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Max utenti]</td> 
   <td> <p>Questo campo è obsoleto. Qualsiasi informazione visualizzata in questo campo è correlata a una funzione rimossa da [!DNL Workfront] e non è possibile aggiornare il campo. </p> <p>Nelle versioni precedenti di [!DNL Workfront], era possibile aggiornare questo campo durante la creazione o la modifica di una mansione. Mostrava il numero totale di utenti che possono essere associati a un ruolo in ciascun progetto. Un valore pari a zero consentiva un numero illimitato di utenti che potevano essere assegnati a un progetto. </p>Il campo rimane visibile in alcuni rapporti ed elenchi, ma non è possibile aggiornare le informazioni visualizzate. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone]</td> 
   <td> <p>Un indicatore che è possibile associare a un’attività per indicare che un punto chiave del progetto è stato raggiunto al completamento dell’attività. In genere, puoi utilizzare le milestone per mostrare un evento significativo, ad esempio il completamento di una fase del progetto o di una serie di attività critiche. Le [!UICONTROL Milestone] sono solitamente associate alle attività principali. Prima di poterle associare alle attività, è necessario crearle. Per informazioni sulle milestone, consulta <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Creare un percorso milestone</a> e <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Associare le milestone alle attività</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percorso milestone]</td> 
   <td>Una raccolta di [!UICONTROL milestones]. I [!UICONTROL Percorsi milestone] vengono utilizzati nei progetti per distinguere i progetti con determinati tipi di [!UICONTROL Milestone] dai progetti con un diverso set di [!UICONTROL Milestone].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Attività milestone]</td> 
   <td>Attività contrassegnata per indicare un evento segnalabile da misurare.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Modulo]</td> 
   <td>Un singolo passaggio all’interno di uno scenario in [!DNL Workfront Fusion] che esegue alcune funzioni in base all’app associata.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Il mio ruolo principale]</td> 
   <td> <p>Quando nei filtri viene fatto riferimento a questo elemento, sono visualizzati gli utenti che hanno lo stesso [!UICONTROL Ruolo principale] dell’utente connesso o gli elementi di lavoro assegnati al [!UICONTROL Ruolo principale] dell’utente connesso.</p> <p>È consigliabile utilizzare questo campo in un filtro per rendere i rapporti più generici quando vengono condivisi con altri utenti. In questo modo, puoi creare un unico rapporto che mostrerà informazioni diverse a seconda di chi effettua l’accesso per visualizzarlo, poiché queste sono sempre personalizzate per l’utente connesso. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Team Home]</td> 
   <td> <p>Quando nei filtri viene fatto riferimento a questo campo, sono visualizzati gli utenti che appartengono al [!UICONTROL Team Home] dell’utente connesso o gli elementi di lavoro assegnati al [!UICONTROL Team Home] dell’utente connesso. </p> <p>È consigliabile utilizzare questo campo in un filtro per rendere i rapporti più generici quando vengono condivisi con altri utenti. In questo modo, puoi creare un unico rapporto che mostrerà informazioni diverse a seconda di chi effettua l’accesso per visualizzarlo, poiché queste sono sempre personalizzate per l’utente connesso. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Convenzione di denominazione]</td> 
   <td>Un set di regole a livello di organizzazione che utilizzano i dati per creare nomi di progetti, attività e deliverables.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Integrazione nativa]</td> 
   <td>Un’integrazione che non richiede alcuna codifica manuale o configurazione API. Definita anche integrazione “predefinita”.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Menu di navigazione]</td> 
   <td>Il pannello nella parte superiore al centro dell’applicazione che dispone di collegamenti alle aree principali di [!UICONTROL Workfront].</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL Nuovo valore numerico]</td> 
   <td>In un rapporto [!UICONTROL Voce diario] viene visualizzato il valore aggiornato di un campo che sostituisce il [!UICONTROL Valore numerico precedente].
   Per ulteriori informazioni, consulta “[!UICONTROL Valore numerico precedente]” in questo articolo.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Spesa non fatturabile]</td> 
   <td> <p>Una spesa che non è contrassegnata come fatturabile per il cliente. Questa può essere una spesa pianificata o una spesa effettiva.</p> <p>I campi Costo spesa non fatturabile pianificato e Costo spesa non fatturabile effettivo sono disponibili per essere aggiunti alle visualizzazioni e ai rapporti. Non vengono visualizzati nelle pagine dei dettagli del progetto o dell’attività.</p>
   <p>Questi campi sono disponibili nei seguenti tipi di rapporti:</p>
   <ul>
   <li>Linea di base</li>
   <li>Modello</li>
   <li>Progetto (dati finanziari)</li>
   </ul>
   <p>Per ulteriori informazioni su come contrassegnare una spesa come fatturabile, consulta <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Gestire le spese del progetto</a>.</p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Giorno non feriale]</td> 
   <td>Giorno che non è allocato al completamento di alcuna assegnazione. Di solito si tratta di un giorno di vacanza, di una festività o di un fine settimana. Il termine viene visualizzato in API Explorer. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nota]</td> 
   <td>Commento o aggiornamento eseguito su un oggetto [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testo della Nota]</td> 
   <td> <p>Questo visualizza il testo di un aggiornamento immesso da un utente su qualsiasi oggetto. </p> </td> 
  </tr>

<tr data-mc-conditions="">

<td>[!UICONTROL Numero di obiettivi collegati]</td> 
   <td> <p>In un rapporto di [!UICONTROL Progetto], questo è il numero di obiettivi strategici associati al progetto. Per informazioni sull’associazione dei progetti agli obiettivi strategici, consulta <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Aggiungere progetti agli obiettivi in [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>Per informazioni sugli obiettivi strategici, consulta anche “[!UICONTROL Obiettivo]” in questo articolo.</p> 
   <p>Questo campo è visibile solo se la tua organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sulla gestione degli obiettivi strategici utilizzando [!DNL Workfront Goals], consulta <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Aggiungere progetti agli obiettivi in [!UICONTROL Obiettivi Adobe Workfront]</a>. </p> </td> 
  </tr>

<tr>

<td>[!UICONTROL Numero di elementi figlio]</td> 
   <td> <p>In un report [!UICONTROL Project] indica il numero di attività secondarie o secondarie di un'attività. 
   <p><b>SUGGERIMENTO</b></p>
   È possibile aggiungere il calcolo <code>{numberOfChildren}</code> a un campo personalizzato calcolato nel modulo personalizzato dell'attività per visualizzare in un campo personalizzato il numero di elementi figlio dell'attività. Per ulteriori informazioni, vedere <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md">Aggiungere un campo calcolato a un modulo</a>. 
    </td>


</tr> 
  <tr> 
   <td>[!UICONTROL Oggetto]</td> 
   <td> <p>Le informazioni visualizzate in [!DNL Adobe Workfront] sono rappresentate da oggetti archiviati nel database di [!DNL Workfront]. Gli oggetti sono ciò che guida le informazioni in Workfront. Alcuni esempi di oggetti sono:</p> 
    <ul> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Programmi]</li> 
     <li>[!UICONTROL Progetti]</li> 
     <li>[!UICONTROL Attività]</li> 
     <li>[!UICONTROL Problemi]</li> 
     <li>[!UICONTROL Documenti]</li> 
     <li>[!UICONTROL Dashboard]</li> 
     <li>[!UICONTROL Rapporti]</li> 
     <li>[!UICONTROL Gruppi]</li> 
     <li>[!UICONTROL Team]</li> 
     <li>[!UICONTROL Utenti]</li> 
     <li>[!UICONTROL Aziende]</li> 
     <li>[!UICONTROL Campi personalizzati]</li>
     <li>[!UICONTROL Campi personalizzati]</li>  
     <li>[!UICONTROL Ore]</li> 
     <li>[!UICONTROL Tariffe di fatturazione]</li> 
     <li>[!UICONTROL Modelli]</li> 
     <li>[!UICONTROL Attività del modello]</li>

<p><b>NOTA</b></p>
  <p>Questo elenco non è completo. </p>

</ul> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Informazioni sugli oggetti in [!UICONTROL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipi di oggetto]</td> 
   <td>Se crei un rapporto o un elenco contenente tutti i moduli personalizzati, puoi utilizzare questo campo come vista o filtro per visualizzare i tipi di oggetto associati a ciascun modulo. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Valore numerico precedente]</td> 
   <td>In un rapporto [!UICONTROL Voce diario], mostra il valore originale di un campo prima che questo venisse aggiornato. Una volta aggiornato, il valore del campo viene visualizzato come [!UICONTROL Nuovo valore numerico] in un rapporto [!UICONTROL Voce diario]. Per ulteriori informazioni, consulta anche “[!UICONTROL Nuovo valore numerico]”.</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Solo su modifica]</td> 
   <td> <p> Uno dei tipi di [!UICONTROL Aggiornamento del progetto]. Quando questa opzione è selezionata, le timeline del [!UICONTROL Progetto previsto] e [!UICONTROL Pianificato] vengono aggiornate solo quando viene effettuato un aggiornamento o una modifica al progetto o a un’attività all’interno del progetto. Non aggiorna il progetto ogni notte.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selezionare il tipo di aggiornamento del progetto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività operativa]</td> 
   <td> <p>Nome di [!UICONTROL Problema] nel database [!DNL Workfront], utilizzato nei rapporti in modalità testo o nei dati personalizzati calcolati.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aperto]</td> 
   <td>Un problema o un’attività non completati, ma su cui si sta lavorando.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organigramma]</td> 
   <td>Abbreviazione di Grafico organizzativo. Questo è un grafico che mostra la gerarchia di un’organizzazione. È presente anche nella scheda della schermata dei dettagli [!UICONTROL Utente] che mostra e consente di impostare le relazioni di [!UICONTROL Azienda] e [!UICONTROL Reporting] dell’[!UICONTROL Utente].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Configurazione organizzativa]</td> 
   <td>Definisce [!UICONTROL Aziende], [!UICONTROL Gruppi] e [!UICONTROL Profili di sicurezza] per la tua organizzazione.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Altri gruppi]</td> 
   <td> <p>In un rapporto o in una vista che elenca gli utenti, questo campo mostra tutti i gruppi di cui ciascun utente è membro. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Valuta di sostituzione]</span> </td> 
   <td> 
    <div> 
     <p>In un rapporto [!UICONTROL Mansione], questa è la valuta associata a una mansione. Si tratta di una sostituzione della [!UICONTROL Valuta di base], nel modo stabilito nell’area [!UICONTROL Configurazione] dall’amministratore di [!DNL Workfront]. </p> 
     <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire mansioni</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Valuta di sostituzione fatturazione/ora]</span> </td> 
   <td> 
    <div> 
     <p>In un rapporto di [!UICONTROL Mansione], corrisponde alla tariffa oraria di fatturazione della mansione che utilizza la [!UICONTROL Valuta di sostituzione] selezionata della mansione.</p> 
     <p> Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire le mansioni</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Valuta di sostituzione costo/ora]</span> </td> 
   <td> 
    <div> 
     <p>In un rapporto [!UICONTROL Mansione], indica la tariffa oraria del costo della mansione che utilizza la [!UICONTROL Valuta di sostituzione] selezionata della mansione. </p> 
     <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire le mansioni</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Proprietario]</td> 
   <td>Utente responsabile del completamento dell’oggetto designato.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Tipo di proprietario]</span> </td> 
   <td> 
    <div> 
     <p>In un rapporto [!UICONTROL Obiettivo] viene visualizzato il tipo di proprietario assegnato a un obiettivo strategico. Di seguito sono riportati i tipi di proprietario dell’obiettivo:</p> 
     <ul> 
      <li> <p>[!UICONTROL Utente]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL Gruppo]</p> </li> 
     </ul> 
     <p>In questo campo non viene mostrato alcun valore se il proprietario dell’obiettivo è la tua organizzazione. </p> 
     <p>È richiesta una licenza aggiuntiva. Per informazioni su [!DNL Workfront Goals], consulta la panoramica <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] </a>. </p> 
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
   <th>Nome oggetto</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Parametro]</td> 
   <td> <p>Un [!UICONTROL Parametro] è un campo personalizzato. Puoi creare un rapporto per tutti i parametri o campi personalizzati nel tuo sistema. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Padre]</td> 
   <td>In un rapporto, questo campo mostra informazioni sull’elemento padre dell’oggetto. In un rapporto [!UICONTROL problema], ad esempio, è possibile che vengano visualizzate informazioni sull’attività o sul progetto in cui è registrato il problema. In un rapporto attività è possibile che vengano mostrate informazioni sull’attività padre diretta o sul progetto. Per ulteriori informazioni sugli oggetti con elementi padre in [!DNL Workfront], consulta la sezione “Interdipendenza e gerarchia degli oggetti” nell’articolo <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Informazioni sugli oggetti in [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attesa attività padre]</td> 
   <td>La quantità di tempo che deve trascorrere tra l’inizio di [!UICONTROL Attività padre] e l’inizio di [!UICONTROL Attività secondaria].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività padre]</td> 
   <td>Nota anche come [!UICONTROL Attività di riepilogo]. Questa è un’attività con attività secondarie (dette anche [!UICONTROL Attività figlio]). La [!UICONTROL Durata], il [!UICONTROL Lavoro richiesto] e la [!UICONTROL Percentuale completata] dell’attività padre viene calcolata a partire dalle attività secondarie.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Risorse part-time]</td> 
   <td>Un utente con licenza che ha capacità inferiore rispetto alla pianificazione predefinita stabilita nel sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percentuale completata]</td> 
   <td> <p>Un campo relativo a un progetto, un’attività o un problema che mostra la percentuale completata di lavoro associata all’attività, al progetto o al problema.</p> <p>Puoi aggiornare questo campo manualmente per problemi e attività di lavoro. </p> <p>Per i progetti e le attività padre, questo campo è un riepilogo di tutte le attività di lavoro e non è possibile aggiornarlo manualmente. </p> <p>Per ulteriori informazioni, consulta la <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Panoramica [!UICONTROL Percentuale completata]</a>.</p> </td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Metodo indice prestazioni (PIM)]</td> 
   <td> <p>Il [!UICONTROL Metodo indice prestazioni (PIM)] per il progetto controlla il metodo utilizzato da Adobe Workfront per calcolare le metriche delle prestazioni del progetto, ad esempio l’Indice prestazioni costi (CPI), l’Indice prestazioni pianificazione costi (CSI), l’Indice prestazioni pianificazione (SPI) e la Stima al completamento (EAC)</p> 
   <p>Workfront calcola questi valori in base alle ore o al costo.</p>
   <p>Per informazioni, consulta <a href="/help/quicksilver/manage-work/projects/project-finances/set-pim.md">Impostare il Metodo indice di prestazioni (PIM)</a>.</p>
   </td> 
  </tr>
 <tr> 
   <td>[!UICONTROL Autorizzazione]</td> 
   <td> <p>Diritti concessi a un utente su un oggetto, in genere assegnati in modo che possa completare il lavoro sull’elemento o visualizzarlo. Puoi concedere autorizzazioni a:</p> 
    <ul> 
     <li>[!UICONTROL Progetti]</li> 
     <li>[!UICONTROL Attività]</li> 
     <li>[!UICONTROL Problemi]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Programmi]</li> 
     <li>[!UICONTROL Rapporti]</li> 
     <li>[!UICONTROL Dashboard]</li> 
     <li>[!UICONTROL Documenti]</li> 
     <li>[!UICONTROL Campi personalizzati]</li> 
     <li>[!UICONTROL Visualizzazioni]</li> 
     <li>[!UICONTROL Filtri]</li> 
     <li>[!UICONTROL Raggruppamenti]</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Panoramica delle autorizzazioni di condivisione sugli oggetti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Piano]</td> 
   <td> <p>Questo è di un tipo di licenza completa nel sistema [!DNL Workfront]. Gli utenti devono disporne per accedere a tutte le funzioni in [!DNL Workfront].</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront]Panoramica delle licenze</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Piano] (in [!DNL Scenario Planner])</td> 
   <td> <p>Un piano è l’oggetto principale quando lavori con la Pianificazione scenari [!DNL Workfront]. Puoi delineare la strategia per il futuro a breve e lungo termine della tua azienda, identificare ogni risultato di alto livello e aggiungerlo come piano alla Pianificazione scenari [!DNL Workfront]. </p> <p>Non puoi visualizzare piani [!DNL Scenario Planner] in un rapporto né accedervi tramite l’API [!DNL Workfront]. </p> <p>[!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], consulta <a href="../../../scenario-planner/scenario-planner-overview.md">La panoramica di [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pianificato]</td> 
   <td> <p>L’intervallo di tempo entro il quale è pianificato un evento. Quando crei progetti, attività o problemi in [!DNL Workfront], puoi stabilire le date di inizio e di fine pianificate, nonché l’arco temporale pianificato durante il quale si verificano. Questi valori rappresentano l’intenzione originale o la stima del tempo necessario per il completamento di un elemento. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vantaggio pianificato]</td> 
   <td>Questo è un inserimento manuale in modo che il project manager valuti se il completamento di un progetto porterebbe un beneficio monetario per l’organizzazione. La specifica di questo valore può essere utile per creare un [!UICONTROL Caso di business] per il progetto. Per aggiornare questo valore devi disporre delle autorizzazioni [!UICONTROL Gestisci] per il progetto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Ore a budget pianificate]</td> 
   <td> <p>In un rapporto di [!UICONTROL Ora preventivata] viene visualizzato il numero di ore preventivate per i progetti o [!UICONTROL Mansioni] in [!UICONTROL Pianificazione risorse]. </p> <p>Per informazioni sul budget di progetti o ruoli in [!UICONTROL Pianificazione risorse], consulta l’articolo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Risorse a budget in [!UICONTROL Pianificazione risorse] utilizzando le visualizzazioni [!UICONTROL Progetto] e [!UICONTROL Ruolo]</a>. Per informazioni sul rapporto [!UICONTROL Ore preventivate], consulta l’articolo <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Rapporto: Ore preventivate</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di completamento pianificata]</td> 
   <td> <p>Puoi impostare manualmente la [!UICONTROL Data di completamento pianificata] di un’attività, un progetto o un problema su una data a tua scelta. Se non imposti la [!UICONTROL Data di completamento pianificata], [!DNL Workfront] lo fa automaticamente. Quando viene impostata automaticamente, la [!UICONTROL Data di completamento pianificata] è: [!UICONTROL Data di inizio pianificata] + [!UICONTROL Durata]</p> <p>Per ulteriori informazioni, consulta i seguenti articoli:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Panoramica dell’attività [!UICONTROL Data di completamento pianificata]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Impostare il progetto [!UICONTROL Data di completamento pianificata]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo pianificato]</td> 
   <td> <p>Un totale di [!UICONTROL Costo manodopera pianificato] e [!UICONTROL Costo spese pianificate] del progetto. Questo non include il [!UICONTROL Costo del rischio pianificato] nel progetto.  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Allineamento date pianificate]</td> 
   <td> <p>Questo è un indicatore automatico che Workfront assegna progetti, attività e problemi per mostrare quando un elemento verrà completato in relazione alla sua Data di completamento pianificata. </p>
   <p>Di seguito sono riportati i valori possibili per l’indicatore Allineamento data pianificata. </p>
<ul>
<li>Verrà eseguito il giorno della data di completamento pianificata</li>
<li>Verrà eseguito prima della data di completamento pianificata</li>
<li>Verrà eseguito dopo la data di completamento pianificata</li></ul>
<p>L’Allineamento data pianificata è visibile negli elenchi e nei rapporti relativi a progetti, attività e problemi. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Durata pianificata]</td> 
   <td> <p>La [!UICONTROL Durata pianificata] di un’attività corrisponde in genere alla relativa [!UICONTROL Durata]. Rappresenta la differenza in giorni tra [!UICONTROL Inizio pianificato] e  [!UICONTROL Date di completamento pianificate] dell’attività. </p> <p>Quando l’attività ha un tipo [!UICONTROL Durata] [!UICONTROL In base all’impegno], la [!UICONTROL Durata pianificata] può differire dalla [!UICONTROL Durata] dell’attività, in base al numero di risorse assegnate all’attività. </p> <p>Ad esempio, se un’attività con un tipo di [!UICONTROL Durata] [!UICONTROL In base all’impegno] ha una [!UICONTROL Durata] di 3 giorni e assegni all’attività una risorsa con una pianificazione a tempo pieno, anche la [!UICONTROL Durata pianificata] sarà di 3 giorni. Se assegni tre risorse con una pianificazione a tempo pieno alla stessa attività, la [!UICONTROL Durata] rimane 3 giorni, ma la [!UICONTROL Durata pianificata] diventa 1 giorno. Con la [!UICONTROL Durata pianificata] vengono modificate anche le date di [!UICONTROL Inizio pianificato] e [!UICONTROL Completamento pianificato] dell’attività, in modo da riflettere la nuova [!UICONTROL Durata pianificata]. Di conseguenza, viene interessata anche la timeline del progetto. </p> <p>Per ulteriori informazioni sulla differenza tra [!UICONTROL Durata] e [!UICONTROL Durata pianificata] per le attività, consulta l’articolo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Differenza tra [!UICONTROL Durata pianificata] e [!UICONTROL Durata] per le attività</a>.</p> <p>I progetti e i problemi non hanno una [!UICONTROL Durata pianificata]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Minuti durata pianificata]</td> 
   <td> <p>La [!UICONTROL Minuti durata pianificata] di un progetto o di un problema è la [!UICONTROL Durata] del progetto o del problema in minuti. </p> <p>Le attività non hanno un campo [!UICONTROL Minuti durata pianificata]. </p> <p>Le [!UICONTROL Attività modello] hanno un campo [!UICONTROL Minuti durata pianificata] che mostrala [!UICONTROL Durata pianificata] dell’attività in minuti. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo spese pianificate]</td> 
   <td> <p>La somma degli [!UICONTROL Importi pianificati] per tutte le spese registrate per un progetto o un’attività.</p> <p><b>ESEMPIO</b></p>
   <p>Se crei una spesa per l’Attività 1 e inserisci 600.00 $ nel campo [!UICONTROL Importo pianificato], il [!UICONTROL Costo spese pianificate] per questa attività è 600.00 $. </p> 
   <p>Per un progetto, [!DNL Workfront] utilizza la formula seguente per calcolare il [!UICONTROL Costo spese pianificate]:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ore pianificate]</td> 
   <td> <p>Questo campo viene visualizzato nelle aree [!UICONTROL progetti], [!UICONTROL attività] e problemi, nei rapporti per progetti, attività o problemi e negli strumenti di gestione delle risorse come [!UICONTROL Pianificazione risorse], [!UICONTROL Bilanciamento carico di lavoro] e il rapporto [!UICONTROL Utilizzo]. </p> <p>Mostra il numero di ore che il proprietario del progetto stima debbano essere necessarie per completare ogni attività o problema. Per i progetti, questa è in genere l’aggregazione delle [!UICONTROL Ire pianificate] delle attività del progetto. </p> <p>Il campo [!UICONTROL Ore pianificate] potrebbe mostrare informazioni diverse in base a dove le visualizzi. Per informazioni sulle ore pianificate, consulta <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Panoramica sulle ore pianificate</a>.</p> <p>Le ore pianificate sono memorizzate in minuti nel database [!DNL Workfront]. Quando scrivi calcoli utilizzando questo campo, assicurati di tenere conto del fatto che le ore vengono visualizzate in minuti.<br></p> <p>Per impostazione predefinita, le ore pianificate vengono distribuite in modo uniforme su tutti i giorni all’interno della durata di un elemento di lavoro e anche in modo uniforme per tutte le risorse assegnate all’attività. Gli utenti possono aggiornare il numero giornaliero di ore pianificate per un elemento di lavoro o le singole ore pianificate per ciascun assegnatario.</p> <p>L’aggiornamento di questo campo è diverso per progetti, attività e problemi: </p> 
    <ul> 
     <li> <p>Per i problemi, puoi aggiornare manualmente questo campo. Le ore pianificate del problema non vengono aggiunte alle ore pianificate del progetto. </p> <p><b>SUGGERIMENTO</b></p> <p>In un rapporto sui problemi, uno dei campi [!UICONTROL Ore pianificate] viene sostituito dal campo [!UICONTROL Lavoro].Nel campo viene visualizzato il numero di ore pianificate per il problema. Per ulteriori informazioni, consulta i campi “lavoro” o “[!UICONTROL Lavoro]” in questa tabella. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>Per le attività, puoi aggiornare manualmente questo campo quando il [!UICONTROL Tipo di durata] dell’attività è [!UICONTROL Assegnazione calcolata] o [!UICONTROL Semplice]. Questo campo viene calcolato da [!DNL Workfront] quando il [!UICONTROL Tipo di durata] dell’attività è [!UICONTROL Lavoro calcolato] o [!UICONTROL In base all’impegno].<br>Per informazioni su [!UICONTROL Durata dell’attività], consulta l’articolo <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica della [!UICONTROL Durata] e [!UICONTROL Tipo di durata] dell’attività</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Per i progetti, [!DNL Workfront] calcola le ore pianificate aggiungendo tutte le ore pianificate da tutte le attività del progetto. </p> </li> 
    </ul> <p><b>SUGGERIMENTO</b></p> <p>Puoi visualizzare le [!UICONTROL Ore pianificate] nei rapporti [!UICONTROL progetto], [!UICONTROL attività] o [!UICONTROL problemi] anche utilizzando la modalità testo e facendo riferimento a campi aggiuntivi. Per ulteriori informazioni, consulta i campi “<code>work</code>”, “[!UICONTROL Lavoro]” e “<code>workRequiredExpression</code>” in questa tabella. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo manodopera pianificato]</td> 
   <td> 
    <p>Per un’attività, la tariffa oraria dell’utente o del ruolo moltiplicata per il numero di ore assegnate all’utente o al ruolo.</p> <p>Per un progetto, rappresenta un totale di tutti [!UICONTROL Costi manodopera pianificata] di tutte le attività.</p> <p>L’utilizzo della tariffa dell’utente o del ruolo dipende dal tipo di costo selezionato per l’attività specificata. </p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/track-costs.md">Tracciare i costi</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Entrate pianificate]</td> 
   <td> <p>Nelle attività e nei progetti è possibile visualizzare un valore per le [!UICONTROL Entrate pianificate] in [!DNL Workfront]. [!UICONTROL Entrate pianificate] rappresenta la quantità di denaro associata alle [!UICONTROL Ore pianificate] delle attività sul progetto. Per i progetti, può anche includere le [!UICONTROL Entrate fisse] del progetto. </p> <p>Per le attività, queste sono le entrate associate alle [!UICONTROL Ore pianificate] delle attività. Le ore pianificate da tutte le attività vengono aggregate a quelle del progetto per contribuire alle [!UICONTROL ore pianificate] del progetto. </p> 
   <p>[!DNL Workfront] calcola le [!UICONTROL Entrat pianificate] per le attività e i progetti utilizzando le formule seguenti:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>Le [!UICONTROL Entrate pianificate] del progetto che vengono visualizzate nell’area dei [!UICONTROL Dettagli del progetto] e nei relativi rapporti sono diverse dalle Entrate pianificate visualizzate nel rapporto [!UICONTROL Utilizzo]. </p> <p>Il campo [!UICONTROL Entrate pianificate] nell’area [!UICONTROL Dettagli progetto] riflette le entrate dell’attività e quelle fisse del progetto. Il campo [!UICONTROL Entrate pianificate] nel [!UICONTROL Rapporto di utilizzo] visualizza le [!UICONTROL Entrate pianificate] associate solo alle attività del progetto. </p> 
     <p><b>ESEMPIO</b></p>  
      <p>Se il progetto ha 1 attività con 10 ore, assegnata a un consulente con una tariffa oraria di 20$ e il progetto ha un importo di 100 $ di [!UICONTROL Entrate fisse], il rapporto di [!UICONTROL Utilizzo] visualizza 200 $ per le [!UICONTROL Entrate pianificate] ([!UICONTROL Entrate pianificate] associate alle ore dell’attività). La sezione [!UICONTROL Dettagli progetto] visualizza 300 $ ([!UICONTROL Entrate pianificate] dall’attività e Entrate fisse per il progetto). </p> 
    <p>Per informazioni sul tracciamento delle entrate in [!DNL Workfront], consulta <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Panoramica della fatturazione e delle entrate</a>. </p> 
    <p>Per informazioni sui calcoli delle [!UICONTROL Entrate pianificate] nel [!UICONTROL Rapporto di utilizzo], consulta <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Visualizzare le informazioni sull’utilizzo delle risorse </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo del rischio pianificato]</td> 
   <td> <p>Il totale del [!UICONTROL Costo potenziale] di tutti i rischi del progetto, tenendo conto della probabilità che si verifichino. Questo importo non è incluso nel [!UICONTROL Costo pianificato] del progetto.</p> <p>Il [!UICONTROL Costo del rischio pianificato] di un progetto viene calcolato con la seguente formula:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profilo del portale]</td> 
   <td>Raccolta di schede e sezioni definita dall’amministratore visualizzata in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sezione del portale]</td> 
   <td>Un componente di una scheda su una dashboard o pagina del portale. Di solito un singolo rapporto, grafico, calendario o elenco di informazioni chiave.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scheda del portale]</td> 
   <td>Scheda di un portale o di una dashboard contenente fino a tre sezioni del portale.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>Una raccolta di progetti che presentano caratteristiche comuni. Questi progetti in genere competono per le stesse risorse, budget o fasce orarie. Puoi suddividere i portfolio in programmi e associarvi i progetti, prima che vengano aggiunti a un portfolio.</p> <p>Per ulteriori informazioni sui portfolio, consulta <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Informazioni sulla metodologia dei portfolio</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Gestione del portfolio]</td> 
   <td>Un’area pratica incentrata sulla gestione di una raccolta o di programmi correlati e sulle attività di progetto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Ottimizzatore portfolio]</td> 
   <td>Uno strumento [!DNL Workfront] che aiuta a valutare e ad assegnare le priorità ai progetti all’interno di un portfolio.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Proprietario portfolio]</td> 
   <td>Stakeholder responsabile della definizione delle priorità e del budget per un portfolio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Costo del rischio potenziale]</td> 
   <td>Puoi individuare questo campo di progetto in elenchi e rapporti. Mostra il costo potenziale per i rischi associati al progetto, qualora si verifichino. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcolare il costo del rischio potenziale </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Predecessore]</td> 
   <td> <p>Un’attività che deve essere terminata prima del completamento di un’attività dipendente. È anche un’attività contrassegnata come [!UICONTROL Dipendenza] per un’altra attività. I predecessori consentono alla pianificazione di impostare la logica di dipendenza dalla sequenza, ad esempio di avviare un’attività al termine di un’altra attività.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Panoramica dei predecessori delle attività</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Azienda principale]</td> 
   <td>L’azienda a cui appartiene l’utente designata nelle impostazioni utente. Le aziende possono anche essere associate ai progetti.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contatto principale]</td> 
   <td><p>Il [!UICONTROL Contatto principale] è l’autore di un problema e viene automaticamente designato da [!DNL Workfront] quando qualcuno crea il problema. Puoi aggiornare manualmente questo campo se disponi di autorizzazioni di [!DNL Manage] per il problema. Un problema può avere un solo contatto principale.</p> 
   <p>Se modifichi il contatto principale, l’utente originariamente designato come contatto principale disporrà ancora dell’accesso in [!UICONTROL Gestione] al problema.</p>
   <p>Quando un problema viene convertito in un’attività o in un progetto, l’utente designato come [!UICONTROL Contatto principale] del problema diventa il [!UICONTROL Referente problema convertito] del progetto o dell’attività. Se il [!UICONTROL Contatto principale] del problema viene aggiornato dopo la conversione del problema, il [!UICONTROL Referente problema convertito] verrà mantenuto come [!UICONTROL Contatto principale] del problema nel momento in cui si è verificata la conversione. Consulta anche “[!UICONTROL Referente problema convertito]” in questo articolo.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Priorità]</td> 
   <td>Valore che può essere assegnato a un’attività, un problema o un progetto per specificarne l’importanza. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Privato]</td> 
   <td>In una [!UICONTROL Nota] o in un [!UICONTROL Documento], questa opzione rende l’oggetto nascosto alla maggior parte dei visualizzatori. Per una coda di richieste di aiuto privato, solo gli utenti del team di progetto possono inviare problemi a tale coda (o progetto) tramite l’area [!UICONTROL Richieste].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profilo]</td> 
   <td>Tutte le informazioni su un account utente.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Programma]</td> 
   <td> <p>Sottogruppo all’interno di un portfolio, in cui progetti simili possono essere raggruppati per ottenere un vantaggio ben definito.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Gestione programma]</td> 
   <td>Gestione delle dipendenze, dei rischi, dei problemi, dei requisiti e delle soluzioni tra progetti per mantenere il programma in buona salute e ottenere i vantaggi definiti.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Proprietario del programma]</td> 
   <td>La parte interessata responsabile della supervisione e dell’organizzazione delle attività per garantire che gli obiettivi del progetto siano in linea con quelli aziendali.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Avanzamento]</span> </td> 
   <td> <p>In un rapporto di [!UICONTROL Obiettivo], questo mostra la percentuale di completamento di un obiettivo strategico. La percentuale di avanzamento viene visualizzata sotto forma di numero. Per informazioni sugli obiettivi strategici, consulta anche “[!UICONTROL Obiettivo]” in questa tabella.</p> <p>Questo campo è visibile solo se l’organizzazione ha acquistato  obiettivi [!DNL Workfront]. Per informazioni sulla gestione degli obiettivi strategici tramite [!DNL Workfront Goals], consulta <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> Aggiungere progetti agli obiettivi in [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stato di avanzamento]</td> 
   <td> <p>In un rapporto di Progetto, Attività e Obiettivo questo campo mostra lo Stato di avanzamento di progetti, attività o obiettivi strategici. Per ulteriori informazioni, consulta i seguenti articoli:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Panoramica sullo stato di avanzamento del progetto</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Panoramica sullo stato di avanzamento dell’attività</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Panoramica dell’avanzamento e della condizione dell’obiettivo in [!DNL Adobe Workfront Goals]</a> </p>
     <p>Il rapporto [!UICONTROL Obiettivo] e lo [!UICONTROL Stato di avanzamento] per il campo [!DNL goals] sono visibili solo se l’organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sugli obiettivi strategici in [!DNL Workfront Goals], consulta la panoramica <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] </a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Progetto]</td> 
   <td> <p>Grande quantità di lavoro che deve essere completata in un arco temporale specifico e deve utilizzare uno specifico budget e numero di risorse. Per renderlo gestibile, il progetto viene suddiviso in una serie di attività. Il completamento di tutte le attività comporta il completamento del progetto. Per informazioni sulla pianificazione di un progetto, consulta <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Pianificare una panoramica del progetto</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ore pianificate assegnazione progetto]</td> 
   <td> <p>In un rapporto [!UICONTROL Mansione iniziativa] viene visualizzato il numero di [!UICONTROL Ore pianificate] associato a una mansione assegnata ad attività o problemi nel progetto. Questo campo e il tipo di rapporto [!UICONTROL Mansione iniziativa] non vengono visualizzati nell’istanza [!DNL Workfront] a meno che l’azienda non abbia acquistato una licenza [!DNL Workfront Scenario Planner]. Per informazioni su [!DNL Workfront Scenario Planner], consulta <a href="../../../scenario-planner/scenario-planner-overview.md">Panoramica di [!DNL Workfront Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dettagli progetto]</td> 
   <td>Dettagli dello stato corrente di un progetto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo preventivato progetto]</td> 
   <td> <p> Questo è il [!UICONTROL Costo preventivato] di un progetto visualizzato in elenchi e rapporti.</p><p>Consulta anche “[!UICONTROL Costo preventivato]” in questo articolo.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Project management]</td> 
   <td>Un insieme di criteri che definisce le soglie per la creazione, la categorizzazione e la denominazione dei progetti.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Spese del progetto]</td> 
   <td>In un rapporto [!UICONTROL Ora], questo campo è riservato alle informazioni finanziarie associate alle ore registrate con il tipo di ora del [!UICONTROL Tempo del progetto]. I progetti possono avere proprie tariffe di fatturazione e se un’ora viene registrata direttamente su un progetto, tali tariffe verranno utilizzate nei calcoli. In base alle impostazioni, i progetti possono anche avere valute diverse e potrebbe esserci una conversione di valuta per tali ore. L’oggetto [!UICONTROL Spese progetto] consente a [!DNL Workfront] di ottenere tali informazioni.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proprietario del progetto]</td> 
   <td>Utente responsabile della gestione dell’ambito, della timeline e delle assegnazioni di un progetto. Approvatore predefinito per gli ordini di modifica, le modifiche finanziarie e i deliverable.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pianificazione del progetto]</td> 
   <td>Processi per sviluppare e mantenere la pianificazione del progetto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sponsor del progetto]</td> 
   <td>Profilo di parti interessate designato a cui ciascuno degli utenti dovrebbe riferirsi. In [!DNL Workfront], questi sono designati come [!UICONTROL Livello di accessi]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team di progetto]</td> 
   <td> <p>La raccolta di utenti o ruoli assegnati a un progetto</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Panoramica del team di progetto</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tracciamento del progetto]</td> 
   <td>Dati utilizzati per misurare lo stato e l’ambito di un progetto</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Previsto]</td> 
   <td> <p>Stima della marca temporale del completamento del lavoro in base alle ore pianificate e alla percentuale di completamento di un’attività, un problema o un progetto.</p> <p>Questo fa riferimento alle date o alla [!UICONTROL Durata] di attività, problemi o progetti. Di solito, vengono indicate date e durate che sono più fedeli alla vita degli elementi di lavoro, dopo che una parte di questo è già stata completata o è trascorso un certo tempo. </p> <p>Ad esempio, la [!UICONTROL Data di completamento prevista] di un’attività è quella in cui [!DNL Workfront] stima che verrà completata, in base alla quantità di lavoro svolto fino a quel momento, al numero di persone assegnate e al tempo trascorso dalla data di inizio.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scadenza bozza]</td> 
   <td> <p>Nei rapporti che contengono l’oggetto [!UICONTROL Versione del documento], (ad esempio un rapporto [!UICONTROL Versione del documento] e [!UICONTROL Approvazione bozza]), questo campo mostra il giorno della settimana, la data, l’ora del giorno e l’anno della scadenza della bozza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Decisione della bozza]</td> 
   <td> <p>Nei rapporti che contengono l’oggetto [!UICONTROL Versione del documento], (ad esempio un rapporto [!UICONTROL Versione del documento] e [!UICONTROL Approvazione bozza]), questo campo mostra lo stato di decisione della bozza (in sospeso, modifiche necessarie o approvata)</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome della bozza]</td> 
   <td> <p>Nei rapporti che contengono l’oggetto [!UICONTROL Versione del documento], (ad esempio un rapporto [!UICONTROL Versione del documento] e [!UICONTROL Approvazione bozza]), questo campo mostra il nome della bozza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pagine bozza]</td> 
   <td> <p>Nei rapporti che contengono l’oggetto [!UICONTROL Versione del documento] (ad esempio il rapporto [!UICONTROL Versione del] e [!UICONTROL Approvazione bozza]), questo campo mostra il numero di pagine incluse nella bozza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Avanzamento bozza]</td> 
   <td> <p>Nei rapporti che contengono l’oggetto [!UICONTROL Versione del documento], (ad esempio un rapporto [!UICONTROL Version del documento] e [!UICONTROL Approvazione bozza]), mostra lo stato di avanzamento della bozza ([!UICONTROL Inviata], [!UICONTROL Aperta], [!UICONTROL Commentata], [!UICONTROL Decisione presa]).</p> <p>Per ulteriori informazioni, consulta <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Panoramica sull’avanzamento della bozza</a> in <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Panoramica sull’avanzamento e sullo stato della bozza</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Bozza]</td> 
   <td>Un processo di revisione in cui uno o più utenti contrassegnano e commentano il contenuto da modificare in un’immagine, un documento di testo, un video o un contenuto web interattivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pubblico]</td> 
   <td>In una [!UICONTROL Nota] o in un [!UICONTROL Documento], questa opzione rende l’oggetto accessibile ad altri utenti o anche a persone esterne a [!DNL Workfront]. Per una [!UICONTROL Coda di richieste di aiuto], [!UICONTROL Pubblico] significa che tutti gli utenti che possono inviare problemi a un progetto possono farlo tramite l’area [!UICONTROL Richieste].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Qualità]</td> 
   <td>La percezione della qualità del lavoro all’interno dell’organizzazione.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coda]</td> 
   <td>Chiamata anche Coda help desk o [!UICONTROL Coda di richieste di aiuto]. Questo progetto è stato pubblicato nell’area [!UICONTROL Richieste] per consentire agli utenti di inviarvi problemi. Di solito vengono create code per argomenti particolari, ad esempio [!UICONTROL Bug], [!UICONTROL Richieste progetto] e così via.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proprietà coda]</td> 
   <td>Queste impostazioni definiscono le regole di invio dei problemi per un progetto che viene pubblicato nell’area [!UICONTROL Richieste].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Argomento Coda]</td> 
   <td> <p>Proprietà su una [!UICONTROL Coda di richieste di aiuto] che consente agli utenti che inviano un problema di selezionare un argomento. Gli argomenti possono:</p> 
    <ul> 
     <li>Essere associato a un modulo di dati personalizzati.</li> 
     <li>Assegnare automaticamente il problema a un utente, un ruolo o un team tramite la Regola di instradamento impostata sull’argomento selezionato.</li> 
     <li>Spostare il problema in un progetto o in una coda diversi attraverso il set di regole di instradamento sull’argomento selezionato.</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Creare argomenti di coda</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ranking]</td> 
   <td> <p>In un rapporto [!UICONTROL Livello di accesso] puoi indicare manualmente un [!UICONTROL Ranking] del [!UICONTROL Livello di accesso]. Questo ti consente, in qualità di amministratore di [!DNL Workfront], di identificare visivamente il livello di complessità associato a ciascun livello di accesso. Ad esempio, puoi assegnare numeri più bassi per livelli di accesso più complessi ([!UICONTROL Piano]) e numeri più alti per livelli di accesso meno complessi ([!UICONTROL Richiedente]). Non puoi seguire il ranking dei livelli di accesso standard.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pronto]</td> 
   <td> <p>Questo campo in un rapporto attività indica se un’attività [!UICONTROL Agile] è stata contrassegnata come [!UICONTROL Pronta] nel backlog. Questo contrassegno si applica solo alle attività [!UICONTROL Agile], che sono assegnate a un team [!UICONTROL Agile]. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Record]</td> 
   <td> <p>In Pianificazione di Workfront, un record è un’istanza univoca di un tipo di record.</p>
<p>Dopo aver aggiunto un tipo di record a un’area di lavoro, puoi iniziare ad aggiungere record di tale tipo nella pagina del tipo di record.</p>
<p>Ad esempio, “Campagna” può essere un tipo di record e “Campagna estiva per l’area EMEA” è un record del tipo di record Campagna.</p>
<p>Per informazioni sulla creazione di record, Consulta <a href="/help/quicksilver/planning/records/create-records.md">Creare record</a>. </p> <p>Pianificazione di Workfront richiede una licenza aggiuntiva. </p></td> 
  </tr>


<tr> 
   <td>[!UICONTROL Tipo di record]</td> 
   <td> <p>Tipo di oggetto di Pianificazione di Workfront.</p>
<p>A differenza di Workfront, dove i tipi di oggetto sono predefiniti, in Pianificazione di Workfront puoi creare i tuoi tipi di oggetto. I tipi di oggetto di Panificazione di Workfront sono denominati tipi di record.</p>
<p>Ad esempio, in Workfront sono già stati creati i tipi di oggetto Programma, Portfolio, Progetto, Attività o Problema.</p>
<p>Nella Pianificazione di Workfront, puoi creare qualsiasi tipo di record che soddisfi i flussi di lavoro della tua organizzazione. Successivamente, puoi definire come i tipi di record si relazionano l’uno con l’altro o le dipendenze dei moduli.</p> Per informazioni sulla creazione di tipi di record, consulta <a href="/help/quicksilver/planning/architecture/create-record-types.md">Creare tipi di record</a>. </p> <p>Pianificazione di Workfront richiede una licenza aggiuntiva. </p></td> 
  </tr>

<tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Frequenza ricorrenza]</td> 
   <td> <p>Campo visualizzato nella casella [!UICONTROL Dettagli attività] o [!UICONTROL Modifica attività] di un elemento padre di attività ricorrenti. Frequenza con cui si verificano le attività nella ricorrenza. Per informazioni sulla creazione di attività ricorrenti, consulta <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Creare attività ricorrenti</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero di riferimento]</td> 
   <td> <p>I progetti, le attività e i problemi vengono associati automaticamente a un numero di riferimento univoco durante la creazione. Puoi visualizzare il [!UICONTROL Numero di riferimento] nella pagina [!UICONTROL Dettagli] dei progetti, delle attività o dei problemi oppure in un elenco o in un rapporto. </p> <p><b>SUGGERIMENTO</b><p><br>Puoi affidarti ai numeri di riferimento quando due elementi hanno lo stesso nome, poiché sono sempre univoci. </p> <p>[!DNL Workfront] genera automaticamente numeri di riferimento sequenziali a livello di sistema. A ogni progetto, attività o problema viene assegnato il numero disponibile successivo nella sequenza. <br></p> <p>Ad esempio, se l’utente A crea un’attività, [!DNL Workfront] potrebbe assegnare automaticamente a questa il numero di riferimento 100. Se l’utente B crea un problema subito dopo, [!DNL Workfront] gli assegna il numero di riferimento 101. Non puoi modificare manualmente i numeri di riferimento. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema rifiuto]</td> 
   <td>In un rapporto progetto o attività, questo è il problema che viene creato quando l’approvazione per il progetto o l’attività viene rifiutata. Per informazioni sui problemi di rifiuto, consulta l’articolo <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Creare un processo di approvazione per gli elementi di lavoro</a>. </td> 
  </tr>

<tr>
  <td>Tipi di relazione</td>
  <td><p>Gli oggetti Workfront sono sempre collegati tra loro utilizzando uno dei tipi di relazione seguenti:</p>

<ul><li> <b>Uno a molti</b>: in questa relazione un oggetto può essere collegato a diversi altri oggetti di tipi diversi. Ad esempio, un progetto può avere più attività. La relazione Progetto-Attività è di tipo uno-a-molti. Non puoi visualizzare questa relazione in un rapporto utilizzando l’interfaccia Standard. Devi utilizzare la modalità di reporting testo per visualizzare le relazioni uno a molti.</li>
  <li><b>Uno a uno</b>: in questa relazione un oggetto può essere collegato solo a un altro oggetto di tipo diverso. Ad esempio, un progetto può avere un solo Gruppo. La relazione Progetto-Gruppo è di tipo uno a uno. Puoi visualizzare una relazione uno a uno tra gli oggetti in un rapporto Standard.</li>
  <li><b>Molti a uno</b>: in questa relazione puoi collegare più oggetti a un solo altro oggetto di tipo diverso. Ad esempio, puoi collegare più attività allo stesso progetto. La relazione Attività-Progetto è di tipo molti-a-uno. In un rapporto Standard puoi visualizzare relazioni tra gli oggetti di tipo molti a uno. </li>
  <li><b>Molti a molti</b>: in questa relazione più oggetti dello stesso tipo possono essere collegati a più oggetti di un tipo diverso. Ad esempio, diversi utenti possono appartenere a più Altri team e i team possono appartenere a più utenti. Non puoi visualizzare questa relazione in un rapporto utilizzando l’interfaccia Standard. Devi utilizzare il reporting in modalità testo per visualizzare le relazioni di tipo molti a molti. </li> </ul>
  </td></tr>
<tr> 
   <td>[!UICONTROL Costo rischio rimanente]</td> 
   <td> <p>Campo del progetto che mostra la differenza tra il [!UICONTROL Costo rischio pianificato] di un progetto e il totale di tutti i [!UICONTROL Costi effettivi] di tutti i rischi del progetto. </p> <p>Il [!UICONTROL Costo rischio rimanente] per un progetto viene calcolato utilizzando la seguente formula:</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Ripianificazione]</td> 
   <td>Modifica delle date di un progetto per riparare o risolvere problemi. Ad esempio, un progetto che è rimasto in attesa per diversi mesi dovrebbe essere ripianificato per riflettere date precise. Questa è un’operazione manuale di adeguamento delle date del progetto o di quelle delle attività. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rapporto]</td> 
   <td>Grafico o tabella contenente informazioni su un oggetto [!DNL Workfront] specificato e i relativi attributi.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Richiesta]</td> 
   <td> <p>Un tipo di problema che viene analizzato in una singola coda centralizzata e non è correlato a un impegno di lavoro continuo.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Coda richieste]</td> 
   <td>Il backlog di problemi gestiti da un processo di traffico e analisi.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Velocità di richiesta]</td> 
   <td>Tempo totale del ciclo di lavoro per acquisire e completare una richiesta.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Richiedente]</td> 
   <td>In genere è un tipo di licenza. Un utente con una licenza Richiedente può inviare richieste di nuovi lavori da eseguire nel sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo riservato]</td> 
   <td>Giorni specificati nel tempo personale di un utente, che indicano che non sarà disponibile per il lavoro. Consulta “[!UICONTROL Giorni di non lavoro]”.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risolvi problema]</td> 
   <td> <p>In un rapporto sui problemi, utilizza questo campo nelle visualizzazioni o nei filtri per fare riferimento al problema che risolve il problema. </p> <p>Per informazioni sulla visualizzazione degli oggetti di risoluzione nei rapporti, consulta <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Visualizzare le informazioni sugli oggetti risolvibili e di risoluzione in un rapporto</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sugli oggetti in risoluzione e risolvibili </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risolvi progetto]</td> 
   <td> <p>In un rapporto sui problemi, utilizza questo campo nelle visualizzazioni o nei filtri per fare riferimento al progetto che risolve il problema. </p> <p>Per informazioni sulla visualizzazione degli oggetti di risoluzione nei rapporti, consulta <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Visualizzare le informazioni sugli oggetti risolvibili e di risoluzione in un rapporto</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica oggetti in risoluzione e risolvibili </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risolvi attività]</td> 
   <td> <p>In un rapporto sui problemi, utilizza questo campo nelle visualizzazioni o nei filtri per fare riferimento all’attività che risolve il problema. </p> <p>Per informazioni sulla visualizzazione degli oggetti di risoluzione nei rapporti, consulta <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Visualizzare le informazioni sugli oggetti risolvibili e di risoluzione in un rapporto</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica oggetti in risoluzione e risolvibili </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risorsa]</td> 
   <td>Utenti o ruoli esistenti in [!DNL Workfront] e assegnati a Team di progetto, attività e problemi. Sono responsabili del completamento del lavoro associato a progetti, attività o problemi. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in  Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Gestione delle risorse]</td> 
   <td> <p>[!UICONTROL Gestione delle risorse] è un insieme di strumenti Enterprise che consente di prevedere con precisione l’utilizzo delle risorse in base alla loro disponibilità in modo che il lavoro da eseguire venga completato puntualmente e con il buget previsto. </p> <p>Con gli strumenti di gestione delle risorse è possibile pianificare le esigenze di capacità a lungo termine e di programmazione a breve termine per le risorse. </p> <p>Per informazioni sulla gestione delle risorse in [!DNL Workfront], consulta <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Introduzione alla gestione delle risorse</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID Manager risorse]</td> 
   <td><p>In un rapporto di progetto, puoi utilizzare questa opzione durante la creazione di un filtro per trovare un manager risorse specifico. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Manager risorse]</td> 
   <td> <p>In un rapporto di progetto o in una vista elenco, questo è un campo informativo che mostra gli utenti designati per eseguire attività di gestione delle risorse sul progetto.  Quando utilizzi “[!UICONTROL Manager risorse]” in un rapporto, viene visualizzato un elenco di manager di risorse, con ognuno d questi sul progetto separato da una virgola. Puoi designare fino a 30 manager delle risorse per un progetto specificato.</p> <p>Per ulteriori informazioni, consulta l’articolo <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Designare manager delle risorse per un progetto o un modello </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Ore preventivate per pianificazione risorse] </td> 
   <td>Le ore preventivate per il progetto e le risorse associate a esso nella [!UICONTROL Pianificazione risorse]. Consulta anche “[!UICONTROL Ore preventivate]” in questo articolo. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Pianificazione risorse] </td> 
   <td>Uno strumento avanzato di [!DNL Workfront] che ti consente di visualizzare e gestire le risorse tra progetti, mansioni o utenti. Per informazioni, consulta <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Panoramica sulla pianificazione risorse</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo della manodopera preventivato per la pianificazione risorse]</td> 
   <td> <p>Si tratta del costo associato alle ore preventivate per le mansioni di progetto che utilizzano la pianificazione risorse. </p> <p>Consulta anche “Costo della manodopera preventivato” in questo articolo. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Pool di Risorse]</td> 
   <td> <p>I Pool di Risorse sono raccolte di utenti che possono essere associati a un progetto. Gli utenti dello stesso Pool di Risorse appartengono in genere allo stesso reparto, hanno competenze simili o complementari o sono finanziati con lo stesso budget. Puoi associare più Pool di Risorse a un progetto o a un utente. Un pool di risorse può essere assegnato esclusivamente a un progetto o condiviso da più progetti.</p> 
   <p>Per ulteriori informazioni sui pool di risorse, consulta <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Panoramica sui pool di risorse </a>.</p> 
   <p>Nei rapporti di progetto, i Pool di Risorse mostrano tutti i pool associati a un progetto. Questo oggetto non può essere utilizzato in un raggruppamento.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utilizzazione risorse]</td> 
   <td>Un rapporto che visualizza il numero di ore disponibili durante un determinato periodo di tempo e il numero di ore pianificate per ogni utente nel rapporto. Questo viene calcolato anche in [!UICONTROL Ore medie al giorno] e in una percentuale di allocazione.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Risultato]</td> 
   <td>In [!DNL Workfront Goals], un risultato è un indicatore di avanzamento per un obiettivo. Può essere un numero, un valore percentuale o un importo di valuta che aggiorni manualmente. Impossibile visualizzare i risultati in un rapporto e accedervi tramite l’API [!DNL Workfront]. Per informazioni sulle attività, consulta <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Introduzione ai risultati e alle attività negli Obiettivi di Adobe Workfront</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Entrate]</td> 
   <td>Importo fatturabile per l’attività o il progetto. L’importo può essere orario, fisso o una combinazione di entrambi.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di entrate]</td> 
   <td>Il tipo di entrate determina il modo in cui l’attività accumulerà le entrate. Alcuni esempi includono [!UICONTROL Ore fisse], [!UICONTROL Ore ruolo] e [!UICONTROL Ore ruolo con limite]. Per informazioni sul tracciamento delle entrate in [!DNL Workfront], consulta <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica su fatturazione ed entrate</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Revisore]</td> 
   <td>In genere è un tipo di licenza. Un utente con una licenza di [!UICONTROL Revisore] può rivedere e approvare gli elementi di lavoro nel sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Rischio]</td> 
   <td> <p>Questo può fare riferimento ai seguenti concetti in [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>Campo in un progetto che indica quanto può essere rischioso un progetto. Puoi assegnare la priorità all’esecuzione dei progetti in base al livello di rischio. I progetti possono presentare i seguenti livelli di rischio:</p> <p>- [!UICONTROL Bassissimo]</p> <p>- [!UICONTROL Basso]</p> <p>- [!UICONTROL Medio]</p> <p>- [!UICONTROL Alto]</p> <p>- [!UICONTROL Altissimo]</p> <p>I livelli di rischio indicati per un progetto non possono essere personalizzati. </p> <p> Per informazioni sull’aggiornamento del rischio di un progetto, consulta la sezione “Impostazioni progetto” dell’articolo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Modificare i progetti</a>. Puoi visualizzare il campo del rischio di un progetto nei rapporti. </p> </li> 
     <li> <p>Evento che può verificarsi durante il ciclo di vita di un progetto e che identifica un potenziale impatto sul costo, sull’ambito o sulla pianificazione del progetto. Puoi definire i rischi potenziali per un progetto e associarne la probabilità o un costo durante la creazione del Business case del progetto. Per informazioni sull’aggiunta di rischi al caso di business del progetto, consulta “Creare e modificare i rischi nei progetti”. </p> <p>Non è possibile visualizzare nei rapporti i rischi definiti nel [!UICONTROL Caso di business]. Nei rapporti e negli elenchi è possibile visualizzare solo diversi tipi di costi dei rischi. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Costo del rischio]</td> 
   <td> <p>Il costo associato ai rischi di un progetto. Di seguito sono riportati i costi dei rischi associati ai progetti che puoi visualizzare nei rapporti:</p> 
    <ul> 
     <li> <p>[!UICONTROL Costo effettivo]: campo di un rischio che mostra il costo effettivo del rischio che si è verificato. Oltre ai rapporti e agli elenchi, puoi individuarli nella casella [!UICONTROL Modifica rischio] durante la modifica o la creazione di un rischio. </p> <p>Per i costi relativi a progetti, attività o problemi, consulta “[!UICONTROL Costo effettivo]” in questo articolo. </p> </li> 
     <li> <p>[!UICONTROL Costo del rischio pianificato]: campo del progetto che mostra un totale di tutti i [!UICONTROL Costi dei rischi potenziali] del progetto. Consulta anche “[!UICONTROL Costo del rischio pianificato]” in questo articolo. </p> <p>Per informazioni sul costo del rischio potenziale, consulta <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcolare il costo del rischio potenziale </a>. </p> </li> 
     <li> <p>[!UICONTROL Costo del rischio rimanente]: campo del progetto che mostra la differenza tra il totale dei [!UICONTROL Costi effettivi] di tutti i rischi e il [!UICONTROL Costo del rischio pianificato]. Consulta anche “Costo del rischio rimanente” in questo articolo. </p> </li>
    </ul> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Gestione del rischio]</td> 
   <td>Processi per identificare, mitigare e monitorare i rischi.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ruolo]</td> 
   <td>Consulta “[!UICONTROL Ruolo]” in questo articolo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indirizzamento]</td> 
   <td>Assegnazione o spostamento automatico di un problema, in genere a causa di un argomento della coda oppure perché rappresenta il percorso predefinito (Regola di indirizzamento) della coda.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Regola di indirizzamento]</td> 
   <td>Un’impostazione su progetti e argomenti della coda che assegna automaticamente un problema a un utente, a un ruolo o a un team oppure lo sposta in un altro progetto o argomento della coda. Le regole di indirizzamento vengono generalmente utilizzate con le code di richieste di aiuto per assegnare automaticamente i problemi in ingresso.</td> 
  </tr> 
 </tbody> 
</table>

## S - U

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome oggetto</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Ricerca salvata]</td> 
   <td>Una ricerca per la quale sono stati salvati i criteri di ricerca. Le ricerche salvate semplificano l’esecuzione della stessa ricerca senza doverne immettere nuovamente i criteri.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Scenario] (in [!DNL Workfront Fusion]) </td> 
   <td> <p>Uno scenario è costituito da una serie di passaggi (moduli) che indicano come i dati devono essere trasferiti e trasformati tra app/servizi.</p> <p>Per informazioni sugli scenari in [!DNL Workfront Fusion], consulta <a href="https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/scenario-overview">[!DNL Adobe Workfront Fusion]Panoramica degli scenari</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scenario] (in [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>In [!DNL Scenario Planner], uno scenario è una copia di un piano. </p> <p>[!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Scenario Planner], consulta <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Panoramica di [!DNL Scenario Planner]</a>. </p> <p>Per informazioni sulla creazione di scenari, consulta <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Creare e confrontare scenari di piano in [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pianificazione]</td> 
   <td>La pianificazione del lavoro settimanale, inclusi gli orari di lavoro, combinata con giorni di ferie (come festività) e giorni di eccezione (come un giorno lavorativo del sabato). È possibile associare pianificazioni a progetti e utenti.</td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Indice prestazioni pianificazione (SPI)]</td> 
   <td><p>L’[!UICONTROL Indice prestazioni pianificazione (SPI)] descrive la relazione tra la pianificazione programmata e quella effettiva. Adobe Workfront calcola l’indice SPI ai livelli di progetto e di attività. Questa metrica viene tracciata dai project manager e le attività o i progetti sono attualmente in anticipo o in ritardo rispetto alla pianificazione.</p>
  <p>Per informazioni, consulta <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-spi.md">Calcolare l’indice delle prestazioni della pianificazione (SPI)</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Esenzione pianificazione]</td> 
   <td>Anche nota come [!UICONTROL Turno modificato]. Giorni programmati in deroga ai normali orari di lavoro settimanali definiti dalla pianificazione. Ad esempio, un sabato in cui è pianificato il lavoro, quando la pianificazione è impostata su Lavora solo dal lunedì al venerdì, sarà un’[!UICONTROL Esenzione pianificazione].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rapporto pianificato]</td> 
   <td> <p>Quando si genera un rapporto dei rapporti, puoi visualizzare informazioni sulle pianificazioni del rapporto, se questo è pianificato per la consegna utilizzando il campo [!UICONTROL Rapporto pianificato]. Questo campo mostra più valori, uno per ogni pianificazione di ciascun rapporto, in un elenco puntato. Per ulteriori informazioni sulla pianificazione dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Panoramica sulla consegna del rapporto</a>.</p> <p>Poiché questo campo mostra più valori, non può essere utilizzato in un raggruppamento. Puoi accedervi solo in un filtro o in una vista. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modifica ambito]</td> 
   <td>Un [!UICONTROL Audit trail] che, se attivo, genera una nota ogni volta che viene effettuata una modifica all’ambito di un progetto o di un’attività, ad esempio se una [!UICONTROL Durata attività] o i [!UICONTROL Predecessori] vengono modificati.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sezione]</td> 
   <td>Un’area sullo schermo, con una propria intestazione, creata per organizzare i dati personalizzati a scopo di visualizzazione.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interruzione di sezione]</td> 
   <td>Vuoto o bordo tra le sezioni.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sicurezza]</td> 
   <td>Le impostazioni che consentono a un utente di interagire con determinati oggetti nel sistema e non con altri. Consulta anche “[!UICONTROL Livelli di accesso]” in questo articolo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Configurazione]</td> 
   <td>L’area in cui gli amministratori possono impostare le configurazioni di sistema e le preferenze.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gravità]</td> 
   <td> <p>[!UICONTROL Gravità] indica la probabilità che un elemento influisca sul completamento del lavoro. Ad esempio, un problema con [!UICONTROL Gravità] alta può bloccare completamente il completamento di un’attività, ma un problema con [!UICONTROL Gravità] bassa può essere puramente cosmetico.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> Aggiornare la gravità del problema</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gravità]</td> 
   <td>Consulta “[!UICONTROL Gravità]” in questo articolo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condivisione]</td> 
   <td>L’azione che consente ad altri utenti di visualizzare o modificare un elemento specifico in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Slack Date]</td> 
   <td>In un rapporto o in una vista dell’attività, in [!UICONTROL Slack Date] viene visualizzata la data esatta in cui un’attività potrebbe influire in modo significativo sulla [!UICONTROL Data di completamento] del progetto. Per informazioni sulla [!UICONTROL Slack Date] di un’attività, consulta <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Panoramica sulla Slack Date dell’attività</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assegnazioni Smart]</td> 
   <td> <p>Quando si assegnano attività o problemi agli utenti, [!DNL Workfront] consiglia le ([!UICONTROL Assegnazioni Smart]) su chi sono gli utenti migliori per completare il lavoro, in base al tempo disponibile per completarlo e alla loro relazione con il progetto.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Panoramica sulle assegnazioni Smart</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Origine]</td> 
   <td> <p>Indica l’oggetto padre di un altro oggetto. Ad esempio, un documento allegato a un’attività ha il nome dell’attività nel campo [!UICONTROL Origine] di un rapporto o di una vista [!UICONTROL Documento]; un problema registrato in un progetto ha il nome del progetto nel campo [!UICONTROL Origine] di una vista o di un rapporto del problema. </p> 
   <p>Nei seguenti rapporti viene visualizzata una colonna Origine in cui puoi visualizzare informazioni sull’oggetto padre:</p>
  <ul><li>Rapporti problema</li>
    <li>Rapporti ora</li>
    <li>Rapporti documento </li>
    </ul>
   <p>Se gli utenti non dispongono delle autorizzazioni per l’oggetto padre di un problema, un’ora o un documento, la colonna Origine del rapporto risulta vuota, anche se il rapporto è configurato per la visualizzazione, o per essere consegnato con i diritti di accesso di un altro utente. </p>
   <p> Per visualizzare informazioni sull’oggetto padre nel rapporto, è consigliabile aggiungere una colonna per l’oggetto padre in cui è possibile visualizzare il nome del padre. </p>
    <p>Ad esempio, puoi aggiungere uno dei seguenti elementi a un rapporto con una colonna Origine: </p>
    <ul><li>Le colonne Nome progetto, Nome attività o Nome problema a un rapporto ora o documento.</li>
    <li>Le colonne Nome progetto o Nome attività a un rapporto problema. </li> </ul>
    Per ulteriori informazioni, consulta <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">Eseguire e consegnare un rapporto con i diritti di accesso di un altro utente</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di inizio]</td> 
   <td> <p>La data in cui il lavoro su un elemento è impostato per l’inizio. In [!DNL Workfront] sono presenti diverse date di inizio: </p> 
    <ul> 
     <li>[!UICONTROL Pianificato]</li> 
     <li>[!UICONTROL Effettivo]</li> 
     <li>[!UICONTROL Previsto] </li> 
    </ul> <p>In un [!UICONTROL Rapporto tariffa], indica la data di inizio di una nuova tariffa di fatturazione per una mansione a livello di progetto. Le ore associate al progetto che sono successive a questa data vengono moltiplicate per questa tariffa di fatturazione per calcolare le entrate sul progetto. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stato]</td> 
   <td> <p>Un indicatore utilizzato per segnalare la posizione di un elemento di lavoro o di un obiettivo strategico nel flusso di lavoro.</p> <p>Per i progetti, lo [!UICONTROL Stato] è un’impostazione del progetto che indica se il progetto è:</p> 
    <ul> 
     <li>[!UICONTROL Corrente]</li> 
     <li>[!UICONTROL In attesa] </li> 
     <li>[!UICONTROL Completato] </li> 
     <li>[!UICONTROL Inattivo]</li> 
    </ul> <p>Per ulteriori informazioni sullo stato di un progetto, consulta <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Accedere all’elenco degli stati del progetto di sistema</a>.</p>
    <p>Per le attività, lo [!UICONTROL Stato] è un’impostazione sull’attività che indica se l’attività è:</p> 
    <ul> 
     <li>[!UICONTROL Nuovo]</li> 
     <li>[!UICONTROL In corso]</li> 
     <li>[!UICONTROL Completato]</li> 
    </ul> <p>Per ulteriori informazioni sullo stato dell’attività, consulta <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Accedere all’elenco degli stati delle attività di sistema</a></p> <p>Per i problemi, lo [!UICONTROL Stato] è un’impostazione sul problema che indica se il problema è:</p> 
    <ul> 
     <li>[!UICONTROL Nuovo]</li> 
     <li>[!UICONTROL In corso]</li> 
     <li>[!UICONTROL In attesa di feedback]</li> 
     <li>[!UICONTROL In attesa]</li> 
     <li>[!UICONTROL Risolto]</li> 
     <li>[!UICONTROL Non risolvibile]</li> 
     <li>[!UICONTROL Non duplicabile]</li> 
     <li>[!UICONTROL Verifica completata]</li> 
     <li>[!UICONTROL Ri-Aperto]</li> 
    </ul> <p>Per ulteriori informazioni sugli stati del problema, consulta <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Accedere all’elenco degli stati dei problemi di sistema</a>.</p> 
    <p>Per gli obiettivi strategici, lo [!UICONTROL Stato] è un’impostazione sull’obiettivo che indica se l’obiettivo è:</p> 
     <ul> 
      <li>[!UICONTROL Attivo]</li> 
      <li>[!UICONTROL Bozza]</li> 
      <li>[!UICONTROL Inattivo]</li> 
      <li>[!UICONTROL Chiuso]</li> 
     </ul> 
     <p>Per ulteriori informazioni sugli obiettivi strategici, consulta anche “[!UICONTROL Obiettivo]” o “[!UICONTROL Obiettivi]” in questo articolo. </p> 
     <p>Per gli obiettivi strategici, questo campo è visibile solo se l’organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sulla gestione degli obiettivi strategici tramite [!DNL Workfront Goals], consulta <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] panoramica</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modifica stato]</td> 
   <td>Un [!UICONTROL Audit trail]. Viene generata una nota quando un utente modifica lo stato del progetto, dell’attività o del problema.</td> 
  </tr> 
  <tr> 
   <td>Le icone di Stato</td> 
   <td> <p>Puoi aggiungere il campo [!UICONTROL Icone di stato] incorporato come colonna nelle viste per migliorare la visibilità dei punti chiave relativi agli oggetti, ad esempio:</p> 
    <ul> 
     <li>Un oggetto a cui sono allegati dei documenti</li> 
     <li>Un oggetto che è associato a un processo di approvazione</li> 
     <li>Un oggetto a cui sono associate delle note aggiuntive</li> 
     <li>Una spesa che è fatturabile o rimborsabile </li> 
     <li>Un’attività che si trova in un percorso critico</li> 
     <li>Un utente che appartiene a un’azienda, a un team o si trova in un fuso orario diverso </li> 
    </ul> <p>Puoi aggiungere il campo [!UICONTROL Icone di stato] nelle viste dei seguenti oggetti: </p> 
    <ul> 
     <li>[!UICONTROL Attività]</li> 
     <li>[!UICONTROL Problemi]</li> 
     <li>[!UICONTROL Progetti]</li> 
     <li>[!UICONTROL Attività del modello]</li> 
     <li>[!UICONTROL Modelli]</li> 
     <li>[!UICONTROL Spese]</li> 
     <li>[!UICONTROL Documenti]</li> 
     <li>[!UICONTROL Utenti]</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Icone di stato incorporate nelle viste</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggiornamento stato]</td> 
   <td> <p>In un rapporto di progetto, attività o problema, questo campo mostra l’aggiornamento di stato più recente fornito dai proprietari degli oggetti nell’area “[!UICONTROL Aggiornamenti]”.Per i progetti, ciò significa che i commenti sono aggiunti dal proprietario del progetto, e per le attività e i problemi, che i commenti sono aggiunti dagli assegnatari.</p> 
   <p> I commenti aggiunti durante l’aggiornamento dello stato di un oggetto non vengono visualizzati nella colonna [!UICONTROL Agigornamento stato].</p> <p>Per visualizzare gli stati “[!UICONTROL Nuovo]”, “[!UICONTROL In elaborazione]”, e “[!UICONTROL Completato]”, utilizza la colonna [!UICONTROL Stato].</p> <p>Per ulteriori informazioni sugli stati, consulta l’articolo <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Aggiornare lo stato dell’attività</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stati]</td> 
   <td>Consulta gli “[!UICONTROL Stati]” in questo articolo.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>Un grafico che rappresenta lo stato delle storie (attività nella metodologia Agile) e il relativo avanzamento verso il completamento.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Ore storia]</td> 
   <td>Una metrica utilizzata per misurare la difficoltà o la complessità di una storia. I team Agile possono scegliere se utilizzare le ore o i punti.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Punti storia]</td> 
   <td>Una metrica utilizzata per misurare la difficoltà o la complessità di una storia. I team Agile possono scegliere se utilizzare le ore o i punti.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategico]</td> 
   <td>Lavoro a lungo termine che modifica l’organizzazione o il modo in cui opera.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Allineamento strategico]</td> 
   <td>Misurazione e allineamento degli obiettivi aziendali tra portfolio e programmi.</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>Viene utilizzato nelle colonne del rapporto durante l’utilizzo dell’interfaccia in modalità testo. </p>
   <p><code>[!UICONTROL stretch]</code> viene utilizzato per identificare quali colonne occupano spazio aggiuntivo non necessario per la vista. La larghezza dell’interfaccia utente dell’area di lavoro per un utente tipico è di circa 850 pixel. Ciò significa che una vista con quattro
   colonne (150 pixel ciascuna) occupa 600 di 850 pixel. Nell’interfaccia utente sono presenti ulteriori 250 pixel che verranno aggiunti alle colonne per le quali è fornita una percentuale di estensione. </p>
   <p>L’estensione di una colonna viene applicata quando viene utilizzata la riga di codice aggiuntiva <code>[!UICONTROL usewidths=true]</code> per almeno una delle colonne della vista. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Iscritti]</td> 
   <td> <p>Utenti iscritti a progetti, attività o problemi.</p> <p>Quando utilizzi questo campo in un rapporto, viene visualizzato un elenco di iscritti, separati da una virgola.</p> <p>Per ulteriori informazioni, consulta l’articolo <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Effettuare l’iscrizione agli elementi in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività di riepilogo]</td> 
   <td>Consulta “[!UICONTROL Attività principale]” in questo articolo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività secondaria]</td> 
   <td>Un’attività secondaria, situata al di sotto di un’attività principale.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Governance del sistema]</td> 
   <td>Un set di criteri che regolano le modifiche e la manutenzione di un sistema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Integrazione dei sistemi]</td> 
   <td>Il processo di collegamento fisico o funzionale tra diversi sistemi informatici e applicazioni software per agire come un insieme coordinato.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Attività]</td> 
   <td> <p>Un’attività che deve essere eseguita come un passaggio verso il raggiungimento di un obiettivo finale (completamento del progetto).</p>

<p>Le attività sono unità di lavoro più piccole finalizzate al completamento di un progetto, che rappresenta un’unità di lavoro più grande.</p>
   <p>Le attività non possono mai esistere in odo indipendente. Fanno sempre parte di un progetto. </p>
   <p>Per ulteriori informazioni sulle attività, consulta <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Panoramica sulle attività</a>.</p> 
   <p>Per informazioni sulla creazione di attività, consulta <a href="/help/quicksilver/manage-work/tasks/create-tasks/create-tasks-in-project.md">Creare attività in un progetto</a>
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attributo attività]</td> 
   <td>Altri campi od oggetti associati a un’attività e che indicano determinati dettagli sull’attività. Alcuni esempi sono [!UICONTROL Data di completamento pianificata] e [!UICONTROL Stato].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vincolo attività]</td> 
   <td>Consulta “[!UICONTROL Tipo di vincolo]” e “[!UICONTROL Data vincolo]”.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Gestione attività]</td> 
   <td>Un insieme di criteri che regola le soglie per la creazione, l’assegnazione, la chiusura e la visibilità delle attività.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Proprietario attività]</td> 
   <td>Il team o l’utente responsabile della stima dello sforzo e del completamento dell’attività</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Team]</td> 
   <td> <p>Una raccolta di utenti che lavorano per obiettivi aziendali od obiettivi simili. Questi utenti possono essere assegnati collettivamente a un elemento di lavoro assegnando il team all’elemento di lavoro.</p> <p>Per ulteriori informazioni sui team, consulta <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Panoramica sui team</a>.</p> <p>I progetti possono avere un [!UICONTROL Team di progetto] che contiene tutti gli utenti o i ruoli associati al lavoro sul progetto.</p> <p>Per ulteriori informazioni sui team di progetto, consulta <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Panoramica sul team di progetto</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Modello]</td> 
   <td> <p>I modelli di progetto sono strutture generiche dei progetti più ripetibili. Quando crei un modello di progetto, puoi definire attività, argomenti di coda, moduli personalizzati, allegare documenti o approvazioni per risparmiare tempo quando devi creare un nuovo progetto. </p> <p>Puoi allegare modelli ai progetti esistenti o utilizzarli per crearne di nuovi. Tutte le informazioni specificate nel modello vengono trasferite ai progetti creati utilizzando tale modello. </p> <p>Per ulteriori informazioni sui modelli, consulta <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Panoramica sul modello di progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività modello]</td> 
   <td>Un’attività che fa parte di un modello. Le attività modello diventano attività nel progetto creato utilizzando il modello.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>Una [!UICONTROL Nota] e la relativa raccolta di risposte relative a un particolare argomento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Miniatura]</td> 
   <td> <p> In un elenco o rapporto del [!UICONTROL Documento] viene visualizzata un’anteprima del documento in una miniatura. </p> <p> Seleziona <strong>[!UICONTROL Miniatura]</strong> per visualizzare una miniatura di 33-66 pixel nel rapporto. </p> <p>Le dimensioni della miniatura vengono regolate modificando la larghezza della colonna in un elenco o in un rapporto.</p> <p>Consulta anche “[!UICONTROL Miniatura grande]” in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indisponibilità]</td> 
   <td>Puoi generare un rapporto di [!UICONTROL Indisponibilità] per visualizzare quando gli utenti hanno indicato una non disponibilità nel loro profilo. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scheda orario]</td> 
   <td> <p>Un cartellino che consente agli utenti di immettere le ore effettive trascorse lavorando su progetti, attività o problemi, oppure le ore trascorse per altre attività non correlate al lavoro, ad esempio riunioni o formazione. Oltre a inserire la quantità di tempo impiegata, puoi indicare anche se il tempo è correlato al lavoro o equivale a un tempo di lavoro effettivo utilizzando i Tipi di ore per definire gli invii di orari. Per informazioni sulle schede orario, consulta <a href="../../../timesheets/timesheets/timesheets-overview.md">Panoramica sulle schede orario</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profilo scheda orario]</td> 
   <td> <p>Un [!UICONTROL Profilo scheda orario] è un modello che [!DNL Workfront] utilizza per creare automaticamente schede orario per gli utenti a esse associati. </p> <p>Puoi configurare diverse impostazioni da applicare a ogni scheda orario durante la creazione. Alcune di queste impostazioni sono: la frequenza con cui la scheda orario deve essere creata (settimanalmente, ogni due settimane, due volte al mese o mensilmente), il giorno di inizio della scheda orario, gli approvatori della scheda orario, i [!UICONTROL Tipi di ore] disponibili che gli utenti possono associare alle ore registrate.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL ID padre principale] </td> 
   <td> <p>Questo campo consente di identificare e filtrare i dati relativi a un gruppo di primo livello e ai relativi sottogruppi in un elenco o in un rapporto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome padre principale] </td> 
   <td> <p>Questo campo consente di identificare i dati di un gruppo di primo livello e dei relativi sottogruppi in una [!UICONTROL Vista] per un elenco o un rapporto.</p> <p>Puoi eseguire questa operazione anche utilizzando il campo [!UICONTROL ID padre principale].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ore Totali]</td> 
   <td> <p>In un [!UICONTROL Rapporto di progetto], questo campo visualizza la somma arrotondata di tutte le ore del progetto, l’ultima volta che sono state calcolate le finanze di progetto. Le [!UICONTROL Ore effettive] riflettono le ore esatte registrate nel progetto. In genere, le [!UICONTROL Ore effettive] devono corrispondere alle [!UICONTROL Ore totali]. Se il campo [!UICONTROL Ore totali] è significativamente diverso dal campo [!UICONTROL Ore effettive], è necessario ricalcolare i dati finanziari sul progetto.</p> <p>Per ulteriori informazioni sul ricalcolo dei dati finanziari del progetto, consulta l’articolo <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Ricalcolare i dati finanziari dei progetti</a>.</p> <p>In una vista Scheda orario [!UICONTROL Standard], questo campo fa riferimento al totale delle ore registrate per gli elementi delle date mostrate in una scheda orario. Il campo [!UICONTROL Ore totali] delle schede orario in questa vista incorporata fa riferimento al campo “[!UICONTROL hoursDuration]” che calcola dinamicamente la differenza di ore tra le date di inizio e di fine della scheda orario. Viene utilizzato per visualizzare la colonna [!UICONTROL Ore totali] in rosso se l’utente registra più tempo rispetto alle ore disponibili nell’intervallo di tempo della scheda orario. Per ulteriori informazioni, consulta <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">Visualizzare le ore totali nella scheda orario</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modalità di tracciamento]</td> 
   <td> <p>L’attributo di un’attività. Questo determina come e quando verranno aggiornate le timeline previste per un’attività. Ad esempio:</p> 
    <ul> 
     <li>[!UICONTROL Utente deve aggiornare] richiede che un’attività venga aggiornata manualmente. In caso contrario, diventerà [!UICONTROL In ritardo rispetto alla pianificazione], quindi [!UICONTROL In ritardo].</li> 
     <li>[!UICONTROL Completamento automatico] completerà automaticamente un’attività quando la data di scadenza, o [!UICONTROL Data di completamento pianificata], è stata superata.</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Panoramica della modalità di tracciamento delle attività</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Trigger]</td> 
   <td>Un evento che avvia uno scenario.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività con problema]</td> 
   <td>Attività incompleta con una condizione di [!UICONTROL Ritardo], [!UICONTROL In ritardo rispetto alla pianificazione] o [!UICONTROL A rischio].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività non assegnata]</td> 
   <td>Un’attività che non è assegnata ad alcun utente, ruolo o team.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di aggiornamento]</td> 
   <td> <p>Impostazione di un progetto che determina quando verrà ricalcolata la timeline prevista del progetto. Il [!UICONTROL Tipo di aggiornamento] può avere i seguenti valori:</p> 
    <ul> 
     <li>[!UICONTROL Modifica automatica e attiva]</li> 
     <li>[!UICONTROL Solo automatico]</li> 
     <li>[!UICONTROL Solo manuale] </li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selezionare il tipo di aggiornamento del progetto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utente]</td> 
   <td>Un account creato in [!DNL Workfront] per consentire a una persona di accedere e interagire con il sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Delega utente]</p> </td> 
   <td> <p>Oggetto segnalabile che indica:</p> 
    <ul> 
     <li>Quali utenti hanno delegato le approvazioni di attività, problemi e progetti</li> 
     <li>Quali utenti hanno ricevuto in delega le approvazioni di attività, problemi e progetti</li> 
     <li>Quando iniziano e terminano tali deleghe</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Creare un rapporto di delega utenti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interfaccia utente]</td> 
   <td>Tutti gli aspetti visivi e interattivi dell’applicazione [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Preferenze interfaccia utente]</td> 
   <td>[!UICONTROL Configurazione interfaccia utente]. Gli amministratori di [!DNL Workfront] possono modificare queste impostazioni per personalizzare gli aspetti dell’interfaccia utente.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Utilizzo]</td> 
   <td>La disponibilità di un utente o un ruolo in base alla pianificazione assegnata, al PTO e al carico di lavoro corrente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utilizzo utente]</td> 
   <td> <p>Una ricerca combinata con un rapporto che mostra la modalità di allocazione o allocazione in eccesso degli utenti (Risorse). Consulta “[!UICONTROL Utilizzo risorse]” in questo articolo.</p> </td> 
  </tr> 
 </tbody> 
</table>

## V - Z

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome oggetto</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Velocità]</td> 
   <td>Misura della durata totale del ciclo di lavoro (tempo che occorre per completare un lavoro) e la frequenza con cui il lavoro viene eseguito nel tempo impegnato originariamente (rapporto lavoro su impegno).</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Vista]</td> 
   <td> <p>Le viste si riferiscono a un elemento di reporting che consente di modificare le colonne in un rapporto o in un elenco di oggetti.</p> 
   <p> Vista si riferisce anche al diritto di un utente di visualizzare solo le informazioni su un oggetto, in base al proprio livello di accesso o a un livello di condivisione delle autorizzazioni su tale oggetto.</p> 
   <p>In Pianificazione di Workfront i record vengono visualizzati nella pagina del tipo di record in uno dei tipi di vista seguenti:</p>
   <ul><li>Tabella</li>
   <li>Timeline</li>
   <li>Calendario</li></ul>
   <p>In Pianificazione di Workfront le viste includono i filtri, i raggruppamenti, l’ordinamento e altre impostazioni applicate ai record sullo schermo.</p> <p>Per informazioni, consulta <a href="/help/quicksilver/planning/views/manage-record-views.md">Gestire le viste dei record</a>.</p>   
   <p>Pianificazione di Workfront richiede una licenza aggiuntiva.</p>
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Icone Vista]</td> 
   <td> <p> Questo campo è uguale a quello delle icone di stato, ma è disponibile solo per le viste seguenti: </p> 
    <ul> 
     <li> [!UICONTROL Documenti] </li> 
    </ul> <p> Per ulteriori informazioni, consulta l’articolo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Icone di stato incorporate in viste</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni ultimo mese]</td> 
   <td> <p>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato durante l’ultimo mese.<br>Per ulteriori informazioni sull’utilizzo delle informazioni negli elenchi di rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizzare l’utilizzo del rapporto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni ultimo trimestre]</td> 
   <td>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato durante l’ultimo trimestre.<br>Per ulteriori informazioni sull’utilizzo delle informazioni negli elenchi di rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >Visualizzare l’utilizzo del rapporto</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni ultimo anno]</td> 
   <td>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato durante l’ultimo anno.<br>Per ulteriori informazioni sull’utilizzo delle informazioni negli elenchi di rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizzare l’utilizzo del rapporto</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni questo mese]</td> 
   <td> <p>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato durante il mese corrente.<br>Per ulteriori informazioni sull’utilizzo delle informazioni negli elenchi di rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizzare l’utilizzo del rapporto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni questo trimestre]</td> 
   <td>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato durante questo trimestre.<br>Per ulteriori informazioni sull’utilizzo delle informazioni negli elenchi di rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizzare l’utilizzo del rapporto</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni questo anno]</td> 
   <td>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato durante l’anno corrente.<br>Per ulteriori informazioni sull’utilizzo negli elenchi di rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">Visualizzare l’utilizzo del rapporto</a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> In un rapporto, quando si utilizza l’interfaccia [!UICONTROL Modalità testo], la riga di codice in cui puoi specificare la larghezza di ogni colonna in pixel. Workfront fornisce una larghezza consigliata per ciascun campo,
anche se a seconda del tipo di campo e del formato, potresti dover apportare delle modifiche.
Utilizza la riga di codice <code>[!UICONTROL usewidths=true]</code> aggiuntiva per applicare la larghezza specificata per la colonna. 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>In un rapporto di progetto, attività o problema, l’istruzione che segue in modalità testo mostra le Ore pianificate del progetto, dell’attività o del problema:</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>Per informazioni sull’utilizzo della modalità testo, consulta <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Panoramica sulla sintassi della modalità testo</a>. </p> 
   <p><b>SUGGERIMENTO</b> 
   <p>In un rapporto di problema, l’aggiunta di uno dei campi [!UICONTROL Ore pianificate] aggiunge il campo <code>work </code> al rapporto. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lavoro]</td> 
   <td> <p>Uno dei due tipi di licenza principali. L’accesso è inferiore a [!UICONTROL Piano], ma è possibile creare e aggiornare il sistema. Un utente con una licenza Lavoro ha più capacità di un titolare di licenza [!UICONTROL Esterno], [!UICONTROL Revisore] o [!UICONTROL Richiedente].</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] Panoramica sulle licenze</a>.</p> <p>Il lavoro può fare riferimento al numero di [!UICONTROL Ore pianificate] per un progetto, un’attività o un problema. Per ulteriori informazioni, consulta il campo “[!UICONTROL lavoro]” in questa tabella. </p> <p><b>SUGGERIMENTO</b></p> <p> In un rapporto di problema, l’aggiunta di uno dei campi [!UICONTROL Ore pianificate] aggiunge il campo <code>work </code> al rapporto. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Struttura di raggruppamento del lavoro]</td> 
   <td>Una struttura gerarchica delle attività che devono essere eseguite dal team di progetto in base alla relazione principale/secondaria.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Impegno di lavoro] </td> 
   <td> 
    <p>Un project manager potrebbe decidere di utilizzare questo campo anziché [!UICONTROL Ore pianificate] per valutare l’impegno necessario per il completamento di un’attività. Questo campo è visibile solo quando sono soddisfatte le seguenti condizioni:</p> 
     <ul> 
      <li> <p>L’attività ha un [!UICONTROL Tipo di durata semplice]. </p> <p><b>SUGGERIMENTO</b></p> <p> Se aggiorni l’attività [!UICONTROL Tipo di durata] con un altro tipo, questo campo diventa nascosto. </p> </li> 
      <li>Il project manager ha abilitato il campo [!UICONTROL Utilizza impegno di lavoro] per calcolare automaticamente l’attività [!UICONTROL Ore pianificate] nel progetto. </li> 
     </ul> 
     <p>Per informazioni sull’utilizzo di [!UICONTROL Impegno di lavoro] invece di [!UICONTROL Ore pianificate] per valutare l’impegno di attività, consulta <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Panoramica dell’impegno di lavoro</a>. </p> 
     <p>Puoi visualizzare questo campo negli elenchi e nei rapporti attività.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Elemento di lavoro]</td> 
   <td> <p>Questo campo fa riferimento ad attività o problemi in [!DNL Workfront]. </p> <p>Il rapporto [!UICONTROL Elemento di lavoro] mostra le informazioni sia per le attività che per i problemi. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mix della gestione del lavoro]</td> 
   <td>Un [!UICONTROL Indicatore di prestazioni del lavoro] (WPI) relativo al rapporto tra il lavoro allocato per l’esecuzione delle attività e quello destinato alla loro modifica. L’indicatore WPI relativo al Mix, ti consente di comprendere, a livello organizzativo, se alla strategia è applicata un’allocazione effettiva del lavoro.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risorsa gestione lavoro]</td> 
   <td>Designazione di un utente tipo nel sistema che risulta idoneo a ricevere lavoro o a tracciare il tempo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ruolo e responsabilità nella gestione del lavoro]</td> 
   <td>Definizione dei proprietari e degli stakeholder per la gestione dell’ambito, dell’esecuzione e delle approvazioni del problema, dell’attività, del progetto, del programma o del portfolio designati.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL SLA per la gestione del lavoro]</td> 
   <td>Una metrica quantificabile concordata da tutti gli stakeholder.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stakeholder della gestione del lavoro]</td> 
   <td>Una gruppo di utenti con un interesse acquisito nei risultati di una richiesta di lavoro.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Punti di contatto della gestione del lavoro]</td> 
   <td>Record digitalizzati della comunicazione tra gli stakeholder.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indicatori di prestazioni lavoro] </td> 
   <td> <p>Rapporto tra mix, capacità, velocità, qualità e coinvolgimento.</p> <p>WPI è un acronimo comune per [!UICONTROL Indicatore di prestazioni del lavoro].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Processo di lavoro]</td> 
   <td> <p>Il metodo con cui il lavoro viene ricevuto, assegnato in base alle priorità ed eseguito. Il modo in cui esegui il lavoro è in genere denominato “flusso di lavoro” o “piano di progetto” (un elenco di attività con date, relazioni predecessore e così via). </p> <p>Esempi di un processo di lavoro possono essere la produzione di una singola risorsa o la consegna di una campagna con più risorse. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modello del flusso di lavoro]</td> 
   <td>Nel rapporto [!UICONTROL Approvazione bozza] questo campo mostra tutti i modelli di flusso di lavoro allegati a una bozza. Se non sono presenti modelli associati, la colonna è vuota.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Tempo di lavoro]</td> 
   <td>

<p>Rappresenta la percentuale di tempo di Equivalente tempo pieno ([!UICONTROL FTE]) in cui l’utente è disponibile per il lavoro effettivo, escluse le spese generali. Il campo [!UICONTROL Tempo di lavoro] deve essere un numero decimale con un valore massimo di 1, ma non può essere 0. Ad esempio, una disponibilità del 20% per il lavoro effettivo sarebbe 0,2.</p>
   </p>Il valore predefinito del campo è 1, che indica che un utente impiega l’intero [!UICONTROL FTE] per il lavoro effettivo relativo al progetto.  </p>
   <p>Il sistema utilizza questo numero per calcolare la disponibilità dell’utente per il lavoro effettivo correlato al progetto. </p>
   <p> Anche le eccezioni di pianificazione e le indisponibilità possono influire sulla capacità dell’utente. </p>
   <p>Per ulteriori informazioni sulla creazione di pianificazioni in Workfront, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Creare una pianificazione</a>. </p>
    <p>Workfront calcola la disponibilità di un utente in base alle preferenze di Gestione risorse nell’area [!UICONTROL Configurazione]. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Configurare le preferenze di gestione delle risorse</a>. </p> 
   <p>Puoi aggiornare il [!UICONTROL Tempo di lavoro] di un utente durante la rispettiva creazione o modifica. Per informazioni, consulta <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Modificare un profilo utente</a></p> 
   <b>SUGGERIMENTO</b> 
   <p>Imposta il valore [!UICONTROL Tempo di lavoro] su 1 per indicare che l’utente è disponibile per il lavoro correlato al progetto per l’intero equivalente tempo pieno.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Orario di lavoro]</td> 
   <td>Nella documentazione di Workfront, questo termine viene utilizzato per descrivere il tempo allocato per il lavoro, in base a una pianificazione.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>In un rapporto di progetto, attività o problema, utilizzando l’istruzione seguente in modalità testo viene visualizzato il numero di ore pianificate del progetto, attività o problema seguito dalla parola “ore”:</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>Per informazioni sull’utilizzo della modalità testo, consulta <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Panoramica di sintassi della modalità testo</a>. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Area di lavoro] </td> 
   <td> <p>In Pianificazione di Workfront, un’area di lavoro è una raccolta di tipi di record che definiscono il ciclo di vita operativo di una determinata organizzazione. Un’area di lavoro è la struttura di lavoro di un’unità organizzativa.</p>
   <p>Pianificazione di Workfront richiede una licenza aggiuntiva. </p>
   <p>Per informazioni, consulta <a href="/help/quicksilver/planning/architecture/create-workspaces.md">Creare aree di lavoro</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


