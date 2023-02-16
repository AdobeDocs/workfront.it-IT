---
content-type: reference
navigation-topic: workfront-navigation
title: Glossario di [!DNL Adobe Workfront] terminologia
description: La [!DNL Adobe Workfront] Il glossario elenca i termini comunemente utilizzati in Adobe Workfront.
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 4a33d72e234ff812a72d7d7a382226697f858df6
workflow-type: tm+mt
source-wordcount: '19106'
ht-degree: 0%

---

# Glossario di [!DNL Adobe Workfront] terminologia

>[!IMPORTANT]
>
>Questo articolo deve essere utilizzato come riferimento per comprendere i termini che si possono incontrare nel [!DNL Adobe Workfront] nella [!DNL Workfront] o quando si parla in generale di pianificazione e gestione del lavoro. Stiamo aggiornando queste informazioni e, di conseguenza, la tabella potrebbe non essere completa. Quando consideriamo esaustive queste informazioni, elimineremo questa liberatoria.

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
   <td>[!UICONTROL Livello Di Accesso]</td> 
   <td>Un profilo utente che determina il modo in cui un utente può interagire con oggetti e strumenti diversi all’interno di Workfront.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività attiva]</td> 
   <td>Un'attività incompleta in un progetto corrente su cui non è possibile lavorare da un'attività predecessore e che non dispone di un vincolo di attività con una data di inizio pianificata futura. In altre parole, oggi si può lavorare su questo tema.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Activity]</td> 
   <td>In [!DNL Workfront Goals], un’attività è un indicatore di avanzamento per un obiettivo. Può trattarsi di una barra di avanzamento aggiornata manualmente o di un progetto associato all’obiettivo. Non è possibile visualizzare le attività in un rapporto e non è possibile accedervi tramite [!DNL Workfront] API. Per informazioni sulle attività, consulta <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Guida introduttiva ai risultati e alle attività in Obiettivi di Adobe Workfront</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo effettivo]</td> 
   <td> <p>Per attività e problemi, si tratta del costo associato alle ore effettive registrate in relazione al tasso di costo per ora della risorsa assegnata all'attività o al problema. Per i progetti, si tratta di un totale di tutti i [!UICONTROL Costi effettivi] derivanti da attività e problemi relativi al progetto. Per informazioni, consulta <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Costi di tracciamento</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo effettivo]</td> 
   <td> <p>La somma degli [!UICONTROL Importi effettivi] per tutte le spese registrate per un progetto o un task.</p> <b>ESEMPIO </b>
   <p>Se si crea una spesa per l'attività 1 e si immette $600,00 nel campo [!UICONTROL Importo effettivo], il [!UICONTROL Costo effettivo] per questa attività è $600,00. </p> 
   <p>Per un progetto, [!DNL Workfront] utilizza la formula seguente per calcolare il [!UICONTROL Costo effettivo]:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs)</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ore effettive]</td> 
   <td> <p>In un rapporto di progetto, attività o problema, le [!UICONTROL Ore effettive] sono la somma di tutte le ore registrate sul progetto, sull'attività o sul problema.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span> Se dalla scheda [!UICONTROL Updates] per l’attività 1, fai clic su "Log Time" (Tempo di log) e immetti 25 ore, l’orario effettivo dell’attività 1 = 25 ore. </p> <p>[!DNL Workfront] calcola [!UICONTROL Ore effettive] per le attività o i progetti padre utilizzando le seguenti formule:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo effettivo del lavoro]</td> 
   <td> <p>Il [!UICONTROL Costo effettivo] associato al lavoro investito in un'attività o in un progetto. </p> <p>Per un'attività, [!DNL Workfront] calcola il [!UICONTROL Costo effettivo del lavoro] utilizzando la formula seguente:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Se l’attività ha un [!UICONTROL Cost Type] di [!UICONTROL User Hourly], [!DNL Workfront] utilizza la frequenza utente. Se l’attività ha un [!UICONTROL Cost Type] di [!UICONTROL Role Hourly], [!DNL Workfront] utilizza la percentuale del ruolo del lavoro per calcolare il [!UICONTROL Costo effettivo del lavoro]. </p> <p>Per un progetto, [!DNL Workfront] utilizza la formula seguente per calcolare il [!UICONTROL Costo effettivo del lavoro]:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Costi di tracciamento</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span>Ad esempio, se un utente registra 5 ore per un'attività con un [!UICONTROL User Hourly] [!UICONTROL Cost Type] e la sua tariffa oraria è di $100, il [!UICONTROL Actual Labor Cost] è di $500.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Entrate effettive] </td> 
   <td> <p>Il [!UICONTROL Entrate effettive] di un progetto o di un'attività corrisponde all'importo del denaro associato alle [!UICONTROL Ore effettive] del progetto o dell'attività. </p> <p>Per informazioni sul tracciamento dei ricavi in [!DNL Workfront], vedi <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica di fatturazione e ricavi</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Inizio Effettivo]</td> 
   <td>La marca temporale quando un utente modifica un oggetto in corso sul lavoro assegnato loro.</td> 
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
   <td>Un tipo di metodologia basata sull'evoluzione collaborativa di esigenze e soluzioni con team interfunzionali. Incoraggia la flessibilità e il cambiamento in base a una tempistica fissa.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Agile Team]</td> 
   <td>Differiscono dal team tradizionale perché prendono il loro lavoro potenziale da un backlog e ci lavorano entro un determinato periodo di tempo chiamato [!UICONTROL Iteration].</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tutti I Miei Team]</td> 
   <td> <p>Quando in [!UICONTROL filters] viene fatto riferimento a questo campo, vengono visualizzati gli utenti che appartengono ai team a cui appartiene l'utente connesso oppure gli elementi di lavoro assegnati ai team a cui appartiene l'utente connesso. </p> <p>È consigliabile utilizzare questo campo in un filtro per rendere i rapporti più generici quando vengono condivisi con altri utenti. In questo modo, puoi creare un solo rapporto che visualizzerà informazioni diverse a seconda di chi effettua l’accesso per visualizzarle, in quanto le informazioni sono sempre personalizzate per l’utente connesso. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di allocazione]</td> 
   <td> <p>Questo campo è disponibile nei seguenti tipi di rapporti:</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Project] (Dati Finanziari)</li> 
     <li>[!UICONTROL - Ora in budget]</li> 
    </ul> <p>Per<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->Rapporto Progetto (dati finanziari): </p> 
    <ul> 
     <li>Crea questo report quando cerchi di capire <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> la quantità di [!UICONTROL Pianificato ore] assegnata alle risorse.</li> 
     <li> <p>La [!UICONTROL Allocation Date] è il primo giorno (domenica) di una settimana in cui inizia l’allocazione di un [!UICONTROL Job Role] a un’attività. Una risorsa ([!UICONTROL Job Role]) può avere tutte le [!UICONTROL Allocation Dates] che ha settimane durante la [!UICONTROL Duration] delle attività a cui è assegnata. Se le attività si estendono su più mesi, il primo giorno di un mese può anche diventare una [!UICONTROL Allocation Date], se rientra nella [!UICONTROL Duration] dell’attività.</p> <p>Ad esempio, puoi assegnare un [!UICONTROL Job Role] a un’attività che si estende su 3 settimane e ha 90 [!UICONTROL Pianificato Hours]. Queste ore vengono distribuite in modo uniforme durante la durata dell'attività, il che fa sì che ogni giorno assegni 6 [!UICONTROL orario pianificato] al tuo ruolo di lavoro:</p> <p><em> [!UICONTROL Ore pianificate giornaliere] = [!UICONTROL Ore pianificate totali]/ Numero di [!UICONTROL Giorni lavorativi] durante la [!UICONTROL Durata] dell'attività </em> </p> <p>Di conseguenza, ci sono tre [!UICONTROL Allocation Date], una per ogni domenica di ogni settimana durante la [!UICONTROL Duration] dell’attività, ciascuna con un certo numero di [!UICONTROL Pianificato Ore] associate ad esse.<br>Se l’attività inizia a metà dell’ultima settimana di un mese e termina due settimane dopo l’inizio di un nuovo mese, l’attività avrà quattro date di allocazione: uno per ogni domenica di ogni settimana durante la [!UICONTROL Duration] dell’attività e uno per il primo giorno del nuovo mese.</p> <p>Per sfruttare al massimo queste informazioni, ti consigliamo di creare un <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> Report del progetto (dati finanziari) e aggiungi un raggruppamento di matrici per [!UICONTROL Allocation Date], quindi raggruppa i risultati settimanalmente, mensilmente, trimestralmente o annualmente per ottenere i dati più precisi.<br>Per informazioni sulla creazione di un raggruppamento di matrici, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Creare un rapporto sulla matrice</a>.</p> </li> 
    </ul> <p>Le informazioni finanziarie vengono compilate nei rapporti del [!UICONTROL Project (Financial Data)] solo quando i dati associati ad esso hanno meno di 5 anni. Ad esempio, se un ruolo di lavoro è stato assegnato a un'attività a gennaio 2015 e oggi è settembre 2021, un campo finanziario come [!UICONTROL Allocation Date] per il ruolo di lavoro non viene compilato nel rapporto [!UICONTROL Project (Financial Data)] . </p> 
    <div> 
     <p>Per un rapporto di tipo [!UICONTROL Budgeted Hour]:</p> 
     <ul> 
      <li>Crea questo rapporto quando cerchi di comprendere la quantità di [!UICONTROL Budgeted Hours] allocata alle risorse o ai progetti nel Planner risorse.</li> 
      <li> <p>La [!UICONTROL Allocation Date] è il primo giorno (una domenica) della settimana per la quale hai preventivato le ore nel [!UICONTROL Resource Planner]. </p> <p>Suggerimento:   <p>Se una settimana si estende per due mesi, genererà due righe nel rapporto: uno corrispondente al primo giorno della settimana (domenica della prima settimana che si svolge durante il primo mese) e la seconda riga visualizza il primo giorno del secondo mese. </p> <p>Ad esempio, se effettui il budget di 8 ore per un utente per la settimana dal 30 giugno (domenica) al 6 luglio (sabato), le due righe mostrano una [!UICONTROL Allocation Date] del 30 giugno e una del 1 luglio. </p> </p> <p>Per informazioni sulle risorse di budget nel [!DNL Resource Planner], vedi l'articolo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Risorse di bilancio [!DNL Resource Planner] utilizzo delle visualizzazioni [!UICONTROL Project] e [!UICONTROL Role]</a>.</p> <p>Per informazioni sulla creazione di un rapporto sull'ora in budget, consulta <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Rapporto: Ora budget</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Annunci]</td> 
   <td> <p>Un modo per comunicare agli utenti informazioni all'interno del sistema. Queste informazioni provengono spesso da [!DNL Workfront] all'amministratore o dall'amministratore all'utente. </p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Inviare annunci</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL App Integration]</td> 
   <td>Un’app rappresenta solitamente un connettore per un’applicazione software, ma può anche rappresentare funzioni speciali che manipolano i dati.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approvatore Decisione]</td> 
   <td> <p>Nel rapporto [!UICONTROL Verifica approvazione], questo campo visualizza le decisioni di approvazione della bozza per le bozze non più attive.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approvatore passaggio]</td> 
   <td>Nel rapporto di approvazione della bozza di questo campo vengono visualizzate informazioni su una fase corrente della bozza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approvazione]</td> 
   <td> <p>Un dato elemento di lavoro, ad esempio un'attività, un documento o una scheda attività, può richiedere che un supervisore o un altro utente si disconnetta dall'elemento di lavoro. Questo processo di disconnessione è denominato approvazione. </p> <p>Per ulteriori informazioni, consulta <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Panoramica del processo di approvazione</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di approvazione]</td> 
   <td>Nel rapporto Approvazione bozza viene visualizzata la data di approvazione di una bozza.</td> 
  </tr> 
  <tr> 
   <td>Approvatore [!UICONTROL]</td> 
   <td>Un ruolo utente o processo che deve essere disconnesso da un dato elemento di lavoro o l'utente che approva le voci orarie nei fogli ore.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assegnato A]</td> 
   <td> <p>In un rapporto sull'attività o sul problema, questo campo visualizza il proprietario dell'attività o il problema o l'assegnatario principale. Puoi anche filtrare o raggruppare in base a questo campo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment]</td> 
   <td>Utente, ruolo o team assegnati a un problema o a un'attività. I progetti, i portfolio o i programmi non possono avere assegnazioni.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assegnazioni]</td> 
   <td> <p>In un rapporto Attività o Problema, questo campo visualizza un elenco di tutte le entità (utenti, ruoli e team) assegnate all'attività o al problema. Puoi filtrare in base a questo campo utilizzando i campi [!UICONTROL Assignment Users] e [!UICONTROL Assignment Ruoli]. È possibile filtrare in base al team assegnato all'attività o al problema utilizzando il campo Team. Non è possibile raggruppare un rapporto in base a questo campo.</p> <p>Gli elementi di lavoro inseriti nel Cestino continueranno a essere visualizzati in alcuni rapporti che fanno riferimento all'oggetto [!UICONTROL Assignment] in cui un [!DNL OR] viene utilizzato il modificatore del filtro.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ruoli assegnazione]</td> 
   <td>
   <p>In un rapporto Attività o Problema, in questo campo vengono visualizzate informazioni sui ruoli del lavoro assegnati alle attività o ai problemi. Questo campo visualizza [!UICONTROL Primary Owners], nonché altri ruoli di lavoro assegnati a attività o problemi.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stato assegnazione]</td> 
   <td> <p>In un rapporto di assegnazione, attività o problema, lo [!UICONTROL Stato assegnazione] visualizza se gli utenti assegnati a un elemento di lavoro hanno fatto clic sul pulsante [!UICONTROL Lavoro su di esso] o [!UICONTROL Fine] per accettare o completare il lavoro. Esistono i seguenti [!UICONTROL Stati di assegnazione]:</p> 
    <ul> 
     <li><b>[!UICONTROL Richiesto]</b>: l’utente è stato assegnato all’attività o al problema, ma non ha ancora fatto clic sul pulsante [!UICONTROL Work On It] per iniziare a lavorarci.</li> 
     <li><b>[!UICONTROL Working]</b>: l'utente ha fatto clic sul pulsante [!UICONTROL Work On It] e sta attualmente lavorando sull'elemento. </li> 
     <li><b>[!UICONTROL Fine]</b>: l’utente ha fatto clic sul pulsante [!UICONTROL Fine] e ha completato il lavoro sull’elemento. </li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">Panoramica dei pulsanti [!UICONTROL Work On It] e [!UICONTROL Done]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team di assegnazione]</td> 
   <td>
   <p>In un rapporto sull’attività o sul problema, in questo campo vengono visualizzate informazioni sui team assegnati alle attività o ai problemi. Nel campo vengono visualizzati [!UICONTROL Primary Owners], nonché altri team assegnati a attività o problemi. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Assignment]</td> 
   <td>
   <p>In un rapporto di attività o problema, questo campo visualizza informazioni sugli utenti assegnati alle attività o ai problemi. Questo campo visualizza [!UICONTROL Primary Owners], nonché altri utenti assegnati a attività o problemi. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attribute]</td> 
   <td>Un attributo è una caratteristica di un [!DNL Workfront] oggetto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Area]</td> 
   <td> <p>Gli audit sono messaggi di sistema che registrano un’azione eseguita in Workfront. Vengono registrati i seguenti tipi di controllo:</p> 
    <ul> 
     <li>[!UICONTROL Modifica ambito]</li> 
     <li>[!UICONTROL Allegato Action]</li> 
     <li>[!UICONTROL Modifica generale]</li> 
     <li>[!UICONTROL Modifica dello stato]</li> 
     <li>[!UICONTROL Note]</li> 
     <li>[!UICONTROL Voce Combinata]</li> 
     <li>[!UICONTROL Error Entry]</li> 
     <li>[!UICONTROL Modifica dello stato]</li> 
     <li>[!UICONTROL Subscription Change]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Trail]</td> 
   <td>La raccolta di note generate automaticamente dagli eventi tracciati tramite le modifiche registrate ([!UICONTROL Audit Areas]). Ogni nota registra chi ha eseguito l’azione, cosa ha fatto e quando l’ha eseguita.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automatico E Su Modifica]</td> 
   <td> <p>Uno dei tipi [!UICONTROL Project Update]. In questo modo verranno ricalcolate le linee temporali previste e pianificate del progetto quando viene eseguito il processo di ricalcolo notturno e quando viene effettuato un aggiornamento al progetto o alle attività all’interno del progetto. </p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleziona il tipo di aggiornamento del progetto </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Disponibilità</p></td> 
   <td> <p>Questo termine viene utilizzato in relazione alla "disponibilità dell’utente" o alla "disponibilità delle risorse" e indica il tempo a disposizione della risorsa (utente o ruolo) per il lavoro. </p> 
   <p>Workfront calcola la disponibilità degli utenti utilizzando diversi campi e a seconda delle impostazioni delle preferenze di Gestione risorse del sistema. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurare le preferenze di Gestione risorse</a>. </p>
   <p>Per ulteriori informazioni sulla disponibilità delle risorse, consulta <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Guida introduttiva a Gestione risorse</a></p>
   In alternativa, la "capacità" viene utilizzata anche per fare riferimento alla disponibilità delle risorse. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Solo automatico]</td> 
   <td> <p>Uno dei tipi [!UICONTROL Project Update]. Questo ricalcola le timeline previste e pianificate quando viene eseguito il processo di ricalcolo notturno.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleziona il tipo di aggiornamento del progetto</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>Lavoro "normale" che contribuisce a realizzare gli obiettivi aziendali primari quotidiani.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Backlog]</td> 
   <td>L'area in un ambiente agile in cui vengono mantenuti nuovi problemi fino a quando non saranno pronti per essere trattati.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Linea di base]</td> 
   <td>Origine di dati su cui misurare le iterazioni in un ambiente agile.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Record di fatturazione]</td> 
   <td> <p>Registra le entrate, le ore o le spese che possono essere fatturate. Queste informazioni possono essere utilizzate per creare fatture in un sistema contabile esterno.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Creazione di record di fatturazione</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>Stato del record di fatturazione</td> 
   <td> <p>In un rapporto Record di fatturazione o Ora, lo stato di un record di fatturazione indica se il record di fatturazione è stato fatturato o non fatturato. Non è possibile eliminare un progetto o modificare l'ora associata a un record di fatturazione fatturata. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Creazione di record di fatturazione</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Branding]</td> 
   <td>Il processo di personalizzazione [!DNL Workfront] per dare all'interfaccia un aspetto che rispecchia la tua azienda utilizzando i tuoi colori e loghi.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Breadcrumb]</td> 
   <td> <p>Area nella parte superiore della pagina che mostra la posizione gerarchica della posizione dell’utente nell’applicazione.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Per ulteriori informazioni, consulta <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Panoramica delle breadcrumb</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stato budget]</td> 
   <td> <p>Campo obsoleto. Qualsiasi informazione che questo campo potrebbe visualizzare è correlata a una caratteristica che [!DNL Workfront] è stato rimosso e il campo non può essere aggiornato. </p> <p>Questo campo mostra se il progetto è stato aggiunto al piano di capacità e se per esso è stato completato il calcolo del budget. Il planner di capacità è stato rimosso da [!DNL Workfront]. </p> 
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
   <td>[!UICONTROL Data completamento budget]</td> 
   <td> <p>Campo obsoleto. Qualsiasi informazione che questo campo potrebbe visualizzare è correlata a una caratteristica che [!DNL Workfront] è stato rimosso. Impossibile aggiornare il campo. </p>
   <p> Questo campo è ancora visibile nei rapporti e negli elenchi delle attività di [!UICONTROL project] e [!UICONTROL activity].</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo preventivato]</td>

<td> <p>È il costo associato alle risorse di budget per un progetto. </p>
   <p>Il campo viene visualizzato nelle seguenti aree di [!DNL Workfront] sotto i seguenti nomi:</p>
   <ul>
   <li><strong>[!UICONTROL Costo preventivato]</strong>: nel pannello [!UICONTROL Business Case Summary]</li>
   <li><strong>[!UICONTROL Cost]</strong>: nelle aree [!UICONTROL Utilization] quando le informazioni vengono visualizzate per [!UICONTROL Cost]</li>
   <li><strong>[!UICONTROL Costo preventivato progetto]</strong>: negli elenchi e nei rapporti</li>
   </ul>   
    <p>Il [!UICONTROL Budgeted Cost] per il progetto viene calcolato con la seguente formula:</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Per ulteriori informazioni sul calcolo del costo a budget e per comprendere i vari nomi di questo concetto in [!DNL Workfront], vedi <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calcola costo budget progetto</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ore previste]</td> 
   <td> <p>Le ore previste per le risorse necessarie per il lavoro da completare sui progetti. Questo campo fa riferimento alle ore in budget nell'area [!UICONTROL Resource Budgeting] del business case (o nel [!UICONTROL Resource Planner]) per il progetto o per le risorse del progetto.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprendere il [!UICONTROL Budgeted Labor Cost] e le [!UICONTROL Budgeted Hours] per i progetti</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Per informazioni sull'impostazione del budget per gli utenti nel [!DNL Resource Planner], vedi l'articolo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Risorse di bilancio [!DNL Resource Planner] utilizzo delle visualizzazioni [!UICONTROL Project] e [!UICONTROL Role]</a>. </p> 
    <p>Le ore in budget nell'area [!UICONTROL Resource Budgeting] del business case o del [!UICONTROL Resource Planner] vengono visualizzate nelle seguenti aree di [!DNL Workfront] e sotto i seguenti nomi:</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>Nome visualizzato [!UICONTROL Budgeted Hours]</strong></td> 
        <td><strong>Zone [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Hours]</td> 
        <td>Area [!UICONTROL Resource Budgeting] del business case</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Resource Planner] visualizzato da [!UICONTROL Hours]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Ore previste]</td> 
        <td> <p>Visualizzazione del rapporto sull'utilizzo [!UICONTROL Hours]</p> <p>Per ulteriori informazioni sul rapporto Utilizzo, consulta l’articolo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Panoramica del rapporto sull’ utilizzo delle risorse</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. Ore]</td> 
        <td> <p>Rapporto di [!UICONTROL Budgeted Hour]</p><p>L'oggetto [!UICONTROL Budgeted Hour] nel report Budgeted Hour (Ora in budget) fa riferimento a informazioni relative a uno strumento di gestione delle risorse obsoleto. Solo il "[!UICONTROL Bud. Il campo Ore]" in questo rapporto fa riferimento alle ore in budget nel [!UICONTROL Resource Planner] o nell'area [!UICONTROL Resource Budgeting] del progetto, Business Case]. </p> <p>Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un rapporto personalizzato</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Ore previste per il planner risorse] </td> 
        <td> <p>Nei seguenti rapporti:</p>
        <ul>
        <li>Rapporto [!UICONTROL Project]
        <li>Rapporto Progetto [!UICONTROL (Dati Finanziari)]
        <li>Rapporto attività
        <li>Rapporto [!UICONTROL Issue]
        <li>Rapporto di [!UICONTROL Budgeted Hour]</li>
        </ul>
         <p>Per ulteriori informazioni sulla creazione di un rapporto, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Creare un rapporto personalizzato</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Qualsiasi altra menzione di [!UICONTROL Budgeted Hours] in [!DNL Adobe Workfront] fa riferimento alle ore in budget con funzioni obsolete rimosse da Workfront . Si tratta di campi di sola visualizzazione e non vengono aggiornati con le informazioni correnti quando si utilizzano gli strumenti di budget delle risorse correnti. </p>
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
   <td>[!UICONTROL Costo manodopera a budget]</td> 
   <td> <p>Questo è il costo associato alle ore che, in qualità di Gestione risorse, vengono preventivate per i ruoli di lavoro per il lavoro necessario per il completamento dei progetti. </p> <p>Il [!UICONTROL Budgeted Labor Cost] in un rapporto di progetto viene calcolato utilizzando la seguente formula:</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Questo campo può fare riferimento ai seguenti elementi:</p> 
    <ul> 
     <li> <p>Costi del lavoro visualizzati nell'area [!UICONTROL Resource Budgeting] del Business Case] o nel [!UICONTROL Resource Planner] associati al costo dei ruoli di lavoro di un progetto. Per informazioni sul calcolo del costo del lavoro a budget, vedere l'articolo <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Comprendere il costo del lavoro preventivato] e le ore previste in budget per i progetti</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Costi del lavoro visualizzati nell'area [!UICONTROL Resource Budgeting] del business case che riflettono i [!UICONTROL People Cost] stimati in un'iniziativa collegata al progetto dal [!DNL Scenario Planner] quando si utilizza Planner scenario per eseguire il budget delle risorse del progetto. Per informazioni sulle iniziative, vedi <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Panoramica delle iniziative nel planner dello scenario</a>. </p> <p>La [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni sulla [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">La [!DNL Scenario Planner] panoramica</a>. </p> </li> 
     <p>Viene visualizzato nelle seguenti aree sotto i seguenti nomi:</p>
   <ul>
   <li><strong>[!UICONTROL Costo manodopera a budget]</strong>: nell'area [!UICONTROL Resource Budgeting] del business case.
   <li><strong>[!UICONTROL Costo preventivato]</strong>: nella visualizzazione [!UICONTROL Utilization] del rapporto [!UICONTROL Cost]
   <p>Per ulteriori informazioni, consulta <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Visualizza informazioni sull’utilizzo delle risorse </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: in [!DNL Resource Planner] Progetto o [!DNL Role] visualizzazioni, quando si visualizza per costo
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: nelle seguenti relazioni: 
   <ul>
    <li>Rapporto [!UICONTROL Project]</li>
    <li>Rapporto Progetto [!UICONTROL (Dati Finanziari)]</li>
    <li>Rapporto attività</li>
    <li>Rapporto [!UICONTROL Issue]</li>
    <li>Rapporto di [!UICONTROL Budgeted Hour]</li> 
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
   <td>[!UICONTROL Data inizio budget]</td> 
  <td> <p>Campo obsoleto. Qualsiasi informazione che questo campo potrebbe visualizzare è correlata a una caratteristica che [!DNL Workfront] è stato rimosso. Impossibile aggiornare il campo.</p>
  <p>Queste aree sono state rimosse da [!DNL Workfront]. </p> 
  <p>Il campo è ancora visibile nei rapporti e negli elenchi di [!UICONTROL project] e attività.</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Grafico a discesa [!UICONTROL]</td> 
   <td>Grafico a linee che fornisce una rappresentazione visiva del lavoro completato e rimanente.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case]</td> 
   <td> <p>Strumento utilizzato per valutare se un progetto deve essere spostato avanti dallo stato [!UICONTROL Idea] allo stato [!UICONTROL Planning]. In altre parole, un business case di [!UICONTROL] aiuta l'organizzazione a decidere se è utile avviare e completare il progetto o meno, specialmente quando si confrontano progetti con altri in un portfolio.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Creare un [!UICONTROL Business Case] per un progetto </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case Budgeted Hours]</td> 
   <td> <p>Campo obsoleto. Qualsiasi informazione che questo campo potrebbe visualizzare è correlata a una caratteristica che [!DNL Workfront] è stato rimosso. Impossibile aggiornare il campo.</p> <p>Questo campo è ancora visibile negli elenchi di progetti e nei rapporti delle attività di . </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assegnazione calcolata]</td> 
   <td> <p>Uno dei tipi di attività [!UICONTROL Duration]. In questo modo verrà calcolata la percentuale di un giorno lavorativo di 8 ore che l'utente assegnato all'attività verrà allocata all'attività, in base alla [!UICONTROL Duration] dell'attività e al [!UICONTROL Work Required].</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica dell’attività [!UICONTROL Duration] e [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Lavoro calcolato</td> 
   <td> <p>Una delle attività [!UICONTROL Duration Types]. In questo modo si calcolano le percentuali [!UICONTROL Work Required] su un'attività, in base alla [!UICONTROL Duration] e all'utente [!UICONTROL Assignment] (in base a un giorno lavorativo di 8 ore).</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica dell’attività [!UICONTROL Duration] e [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Calendario [!UICONTROL]</td> 
   <td> <p>Ci sono due tipi di calendari in [!DNL Workfront]: i rapporti sul calendario principale e sul calendario.</p> <p>Il calendario principale è un calendario personale che consente a un utente di gestire il proprio carico di lavoro rispetto alle ore disponibili in [!DNL Workfront]. L’utente può inoltre integrare il proprio calendario principale con [!DNL Outlook] ([!DNL Google] e [!DNL Microsoft] integrazione). </p> <p>Per ulteriori informazioni sul calendario principale, vedi <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">Visualizzazione Calendario principale</a>.</p> <p>Un rapporto calendario è un rapporto dinamico in cui gli utenti possono visualizzare la data e altri dettagli importanti di un evento, tra cui la data di scadenza, lo stato del lavoro e l’utente a cui è assegnato l’evento.</p> <p> Per ulteriori informazioni sui rapporti sul calendario, vedi <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Panoramica dei rapporti sul calendario</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Può Avviare]</td> 
   <td> <p>Questo campo indica se un'attività è pronta per iniziare a lavorare. Se l'inizio è pronto per essere lavorato sul campo [!UICONTROL Can Start] sull'attività è impostato su [!UICONTROL True]. </p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">Panoramica di "[!UICONTROL Can Start]" per le attività</a>.</p> 
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
   <td> <p>[!UICONTROL Category]</p> </td> 
   <td> <p>Una categoria è un modulo personalizzato. È possibile creare rapporti per questo oggetto e mostrarli anche in altri rapporti sugli oggetti. Non tutti gli oggetti possono avere un modulo personalizzato o una categoria. I seguenti oggetti possono avere un modulo personalizzato: <br></p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]</li> 
     <li>[!UICONTROL Problema]</li> 
     <li>Portfolio [!UICONTROL]</li> 
     <li>[!UICONTROL Document]</li> 
     <li>[!UICONTROL Spesa]</li> 
     <li>[!UICONTROL Program]</li> 
     <li>[!UICONTROL Utente]</li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome categoria]</td> 
   <td> <p>Quando viene aggiunto come colonna alla visualizzazione di uno dei seguenti oggetti, viene visualizzato un elenco di tutti i moduli personalizzati associati a tali oggetti:</p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]<br></li> 
     <li>[!UICONTROL Problema]<br></li> 
     <li>Portfolio [!UICONTROL]<br></li> 
     <li>[!UICONTROL Document]<br></li> 
     <li>[!UICONTROL Spesa]<br></li> 
     <li>[!UICONTROL Program]<br></li> 
     <li>[!UICONTROL Utente]<br></li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Management]</td> 
   <td>Area pratica incentrata sulla definizione, la comprensione e l'adattamento del lavoro pianificato ai cambiamenti di ambito, pianificazione, costo e fattori delle risorse.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Cambia ordine]</td> 
   <td>Tipo di problema sollevato rispetto a un progetto che delinea una modifica richiesta all'ambito concordato.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cambia solo]</td> 
   <td>Uno dei [!UICONTROL Update Types] del progetto. Aggiorna solo le timeline [!UICONTROL Project Projection] e [!UICONTROL Planned] quando vengono eseguiti aggiornamenti a attività o modifiche al progetto o alle attività.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cambia ordine]</td> 
   <td> <p>Uno dei tipi [!UICONTROL Issue] indica solitamente che è necessario eseguire una quantità non pianificata di lavoro prima del completamento del progetto.</p> <p>Per ulteriori informazioni sui tipi di problemi, consulta la sezione "Tipi di problemi predefiniti" nell’articolo <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Personalizzare i tipi di problemi predefiniti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività figlio]</td> 
   <td>Un’attività che è un [!UICONTROL Subtask] di un [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Children]</td> 
   <td>L'insieme di sottoattività [!UICONTROL] a un [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] e [!UICONTROL Training]</td> 
   <td>Moduli di apprendimento, certificazioni, standard o una comunità di pratiche.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit]</td> 
   <td>Strumento di comunicazione per gli utenti per impostare le aspettative relative ai risultati finali delle attività.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data del commit]</td> 
   <td>Strumento di comunicazione per gli utenti per impostare le aspettative sui risultati finali delle attività.</td> 
  </tr> 
  <tr> 
   <td>Comunicazione e reporting</td> 
   <td>Norme per rivedere le eccezioni e lo stato di salute di un progetto, programma o portafoglio</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Company]</td> 
   <td> <p>Una [!UICONTROL Company] è un'unità organizzativa in [!DNL Workfront]. </p> 
   <p> Puoi associare un utente o un progetto a un’azienda. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Creare e modificare aziende</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di completamento]</td> 
   <td> <p>Data in cui un progetto, un'attività o un problema è impostato per essere completato. Esistono diversi tipi di [!UICONTROL Date di completamento] in [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL Data effettiva di completamento]. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Panoramica del progetto [!UICONTROL Data effettiva di completamento] </a>.</li> 
     <li>[!UICONTROL Pianificazione della data di completamento]. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Imposta la [!UICONTROL Pianificazione del completamento Data]</a> e <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Panoramica dell’attività [!UICONTROL Pianificazione del completamento Data]</a>.</li> 
     <li>[!UICONTROL Data di completamento prevista]. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Panoramica della [!UICONTROL Data di completamento prevista] per progetti, attività e problemi</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completation Day]</td> 
   <td>Il giorno, relativo all’inizio del [!UICONTROL Template], in cui un’ [!UICONTROL Template Task] o un modello [!UICONTROL Template] deve essere completato.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modalità completamento]</td> 
   <td> <p>Questo indica come un progetto verrà contrassegnato come [!UICONTROL Complete]. Può avere due valori:</p> 
    <ul> 
     <li>[!UICONTROL Manuale]: Un utente deve modificare lo stato del progetto in [!UICONTROL Complete].</li> 
     <li>[!UICONTROL Automatico]: Lo stato del progetto viene automaticamente modificato in [!UICONTROL Complete] quando tutte le attività del progetto sono completate al 100% e tutti i problemi vengono chiusi.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition]</td> 
   <td> <p>Si tratta di una rappresentazione visiva dell’avanzamento di un’attività, di un problema o di un progetto.</p> <p>Per i progetti, la condizione può essere impostata manualmente dal proprietario del progetto oppure può essere impostata automaticamente da [!DNL Workfront], in base allo stato di avanzamento del progetto. </p> <p>I valori possibili per la condizione del progetto sono:</p> 
    <ul> 
     <li>[!UICONTROL Su Target]</li> 
     <li>[!UICONTROL A Rischio]</li> 
     <li>[!UICONTROL In Trouble]</li> 
    </ul> <p>Per ulteriori informazioni sulla condizione del progetto, consulta l’articolo <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Panoramica della condizione del progetto e del tipo di condizione</a>.</p>
     <p>È possibile associare le attività e creare condizioni di un problema a un numero che può essere visualizzato nei rapporti. Negli elenchi riportati di seguito vengono visualizzati i nomi e i numeri predefiniti per le condizioni di attività ed emissione. L’amministratore di sistema può aggiornare i nomi delle condizioni e aggiungere nuove condizioni con numeri diversi. Una volta associato un numero a una condizione, non è possibile modificarlo.  </p> 
     <p>Per le attività, la condizione viene impostata manualmente dal proprietario dell'attività. I valori possibili per la condizione dell'attività sono:</p> 
    <ul> 
     <li>[!UICONTROL Andando Smoothly] (0)<br></li> 
     <li> [!UICONTROL Alcune Preoccupazioni] (1)<br></li> 
     <li>[!UICONTROL Major Roadblock] (2)</li> 
    </ul> <p>Per ulteriori informazioni sulla condizione dell'attività, consulta l'articolo <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Aggiorna [!UICONTROL Condition] per attività e problemi</a>.</p> <p>Per i problemi, la condizione viene impostata manualmente dal proprietario del problema. I valori possibili per la condizione di problema sono:<br></p> 
    <ul> 
     <li>[!UICONTROL Andando Smoothly] (0)<br></li> 
     <li>[!UICONTROL Alcune Preoccupazioni] (1)<br></li> 
     <li>[!UICONTROL Major Roadblock] (2)</li> 
    </ul> 
   <p><b>NOTA</b></p>
    <p>Quando il campo [!UICONTROL Condition] viene tracciato nei rapporti [!UICONTROL Journal Entry] , i valori [!UICONTROL New] e [!UICONTROL Old Number Values] visualizzano il numero associato alla condizione anziché il nome. Se una condizione non è originariamente definita per un'attività o un problema e successivamente lo si aggiorna, la voce del giornale di registrazione che acquisisce l'aggiornamento visualizzerà il [!UICONTROL Old Number Value] del campo [!UICONTROL Condition] come -2.147.483.648. Vedi anche "[!UICONTROL New Number Value]", "[!UICONTROL Old Number Value]" e "[!UICONTROL Journal Entry]" in questo articolo. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition Update]</td> 
   <td> <p>Questo campo mostra lo stato attuale delle attività, dei progetti o dei problemi. Questa opzione mostra gli aggiornamenti più recenti forniti dai proprietari di attività, progetti o problemi nel campo [!UICONTROL Update Status] , insieme alla nuova condizione.</p> <p>I commenti effettuati sugli aggiornamenti delle condizioni non vengono visualizzati nella colonna [!UICONTROL Condition Update]; viene visualizzato solo l'aggiornamento principale.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data vincolo]</td> 
   <td> <p>Se utilizzi un [!UICONTROL Task Constraint] associato a una data specifica, ad esempio [!UICONTROL Deve iniziare su], tale data specifica diventa la [!UICONTROL Constraint Date] dell’attività.</p> <p>I vincoli task seguenti aggiornano il campo [!UICONTROL Constraint Date] :</p> 
    <ul> 
     <li>[!UICONTROL Deve Iniziare Su]</li> 
     <li>[!UICONTROL Deve Terminare Il</li> 
     <li>[!UICONTROL Start Non Oltre</li> 
     <li>[!UICONTROL Inizia Non Prima Di</li> 
    </ul> <p>Suggerimento:   
     <ul> 
      <li> <p>Un'attività con un [!UICONTROL Constraint] di [!UICONTROL Fixed Date] non ha [!UICONTROL Constraint Date]. </p> </li> 
      <li> <p> La [!UICONTROL Constraint Date] è visibile solo in un report o in una visualizzazione personalizzata.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Day]</td> 
   <td> <p>Se si utilizza un vincolo di attività in un'attività modello associata a un giorno specifico, ad esempio deve iniziare su, tale giorno specifico diventa il giorno vincolo dell'attività modello.</p> <p>I seguenti vincoli di attività aggiornano il campo [!UICONTROL Constraint Day] :</p> 
    <ul> 
     <li>[!UICONTROL Deve Iniziare Su]</li> 
     <li>[!UICONTROL Deve Terminare Il</li> 
     <li>[!UICONTROL Start Non Oltre</li> 
     <li>[!UICONTROL Inizia Non Prima Di</li> 
    </ul> <p>Suggerimento: Il [!UICONTROL Constraint Day] è visibile solo in un rapporto o in una visualizzazione personalizzata. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di vincolo]</td> 
   <td> <p>Tendenza di pianificazione di un'attività. Ad esempio, [!UICONTROL Al più presto] pianificherà l’inizio di un’attività per il più presto possibile, mentre [!UICONTROL Fine non oltre) pianificherà la fine di un’attività entro la [!UICONTROL Constraint Date] e non oltre.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sul vincolo di attività [!UICONTROL]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Menu contestuale]</td> 
   <td>Un menu, situato sul lato sinistro dello schermo, su cui gli elementi vengono modificati per essere correlati al contenuto attivo. Ad esempio, quando un utente sta visualizzando un progetto, il [!UICONTROL Menu contestuale] visualizza i collegamenti alle informazioni e agli strumenti relativi al progetto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertito Issue Originator]</td> 
   <td>Campo di un progetto o di un rapporto di attività che visualizza informazioni sull'utente che è il [!UICONTROL Contatto principale] di un problema quando il problema viene convertito in un progetto o un'attività. Il campo viene visualizzato anche nella sezione [!UICONTROL Project Details] , in cui viene visualizzato il nome del [!UICONTROL Primary Contact] del problema convertito. Vedi anche "[!UICONTROL Contatto primario]" in questo articolo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Cost]</td> 
   <td> <p>Importo monetario da spendere per il completamento di un progetto, un'attività o un problema. </p> <p>È possibile tenere traccia di vari tipi di costi per manodopera, spese e rischi correlati al progetto.Per informazioni sul rilevamento dei costi in [!DNL Workfront] vedere <a href="../../../manage-work/projects/project-finances/track-costs.md">Costi di tracciamento</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di costo]</td> 
   <td>Per un'attività, il [!UICONTROL Cost Type] determina il modo in cui l'attività accumulerà i costi. Alcuni esempi includono [!UICONTROL Fixed Hourly], [!UICONTROL User Hourly] e [!UICONTROL User Hourly plus Fixed]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dipendenze tra progetti]</td> 
   <td> <p>Un’attività di un progetto dipende da un’attività di un progetto diverso.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Creare predecessori tra progetti</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Dati Personalizzati]</td> 
   <td> <p>Dati univoci per un'organizzazione. Le organizzazioni possono personalizzare [!DNL Workfront] creazione di moduli personalizzati e campi personalizzati. Queste informazioni personalizzate possono favorire la creazione di rapporti per KPI, il controllo e il mix di domanda. </p> <p>I dati personalizzati possono essere collegati a:</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Spese]</li> 
     <li>[!UICONTROL Portfoli]</li> 
     <li>[!UICONTROL Programmi]</li> 
     <li>[!UICONTROL Iterazioni]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Data Type]</td> 
   <td>L'opzione per specificare se un campo [!UICONTROL Dati personalizzati] è memorizzato nel database come Testo, Data, Numero o Valuta.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di visualizzazione personalizzato]</td> 
   <td>Tipo di visualizzazione del campo personalizzato. Alcuni esempi includono [!UICONTROL Drop-Down], [!UICONTROL Text Field], [!UICONTROL Text Area], [!UICONTROL Radio Buttons], ecc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campo personalizzato]</td> 
   <td>Per i dati personalizzati che consentono all’utente di selezionare tra diverse opzioni, si tratta dei valori da cui un utente può selezionare. Le opzioni personalizzate sono valide solo per i pulsanti di scelta (!UICONTROL Drop-Down], [!UICONTROL Multi-Select Drop-Down], [!UICONTROL Radio Buttons] e le caselle di controllo [!UICONTROL Checkbox].</td> 
  </tr> 
  <tr> 
   <td>Etichetta del modulo personalizzato [!UICONTROL]</td> 
   <td>Quando si utilizza un tipo di visualizzazione personalizzato con opzioni personalizzate, si tratta del testo dell’interfaccia utente che verrà visualizzato nel menu a discesa, nelle caselle di controllo o nei pulsanti di scelta per tale opzione personalizzata.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valore personalizzato]</td> 
   <td>Quando si utilizza un campo personalizzato con opzioni personalizzate, si tratta del valore che verrà memorizzato nel database per una particolare opzione.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazione personalizzata]</td> 
   <td>Una definizione dei campi dati, o colonne, visualizzati per ciascun oggetto di un elenco.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Customer]</td> 
   <td>Un'organizzazione che utilizza un'istanza di Workfront.</td> 
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
   <td> <p> È possibile aggiungere questo campo in un report o in un elenco dell'oggetto report per visualizzare le dashboard sulle quali il report è elencato in un elenco. </p> <p> Puoi utilizzare questo campo per filtrare anche i rapporti elencati in un dashboard specifico. </p> <p> Per ulteriori informazioni sull’inclusione delle informazioni del dashboard nei rapporti sugli oggetti del rapporto, consulta la sezione "Informazioni sui rapporti elencati nei dashboard" nell’articolo <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Accedere e organizzare i rapporti</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data Type]</td> 
   <td>Consulta "[!UICONTROL Custom Data Type]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Giorni in ritardo]</td> 
   <td> <p>Questo campo mostra una differenza di data tra [!UICONTROL Pianificato inizio] e [!UICONTROL Oggi] se manca la [!UICONTROL Effettivo Data completamento].</p> <p>Mostra anche una differenza di data tra [!UICONTROL Completamento effettivo] e [!UICONTROL Completamento pianificato], quando è presente una [!UICONTROL Data di completamento effettivo].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Pianificazione predefinita]</td> 
   <td> <p>Orari di lavoro predefiniti personalizzabili da assegnare a utenti e progetti all’interno di un’organizzazione. </p> <p>Le pianificazioni vengono utilizzate per calcolare le date di inizio, inizio e completamento pianificate delle attività assegnate agli utenti.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Deliverable]</td> 
   <td>Beni o servizi quantificabili che devono essere forniti al termine di un progetto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Demand Management]</td> 
   <td>Punteggio e priorità dei processi di assunzione.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>Obiettivi del reparto</td> 
   <td>Obiettivi specifici di un reparto specifico che si concentra sul miglioramento delle metriche operative all'interno del reparto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency]</td> 
   <td>È inoltre possibile modificare lo stato del collegamento tra due attività che richiedono la modifica dello stato di un'attività prima dell'altra.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency Type]</td> 
   <td> <p>Tipo di relazione di pianificazione tra un'attività e i relativi predecessori. Un esempio è [!UICONTROL Finish-Start], che richiede che la prima attività debba terminare prima che la seconda attività possa essere avviata.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Panoramica dei tipi di dipendenza dell'attività</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document]</td> 
   <td>Qualsiasi file allegato a un oggetto all'interno di [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Versione documento]</td> 
   <td> <p>Ogni volta che lo stesso documento viene caricato sullo stesso oggetto, gli viene assegnato un numero di versione. Gli utenti possono visualizzare e modificare diverse opzioni per una versione precedente di un documento.</p> <p>Per ulteriori informazioni, consulta <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Gestione delle versioni dei documenti</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration]</td> 
   <td> <p>Intervallo di tempo allocato per il completamento di un problema di attività o di un progetto (in base al numero di giorni tra l'inizio pianificato e il completamento pianificato).</p> 
    <ul> 
     <li>Per le attività, il campo Durata è modificabile se il tipo di durata dell'attività non è semplice. Se il tipo di durata dell'attività è Semplice o se il Vincolo di attività è Date fisse, la durata è un calcolo eseguito da Workfront.</li> 
     <li>Per i problemi, la Durata è sempre un campo modificabile e deve rappresentare una stima di un numero di giorni che richiederebbero la risoluzione del problema.</li> 
     <li>Per i progetti, la Durata è un calcolo eseguito da [!DNL Workfront] e rappresenta la differenza nei giorni tra l'inizio pianificato del primo task e il completamento pianificato del progetto più recente.</li> 
    </ul> <p>Per ulteriori informazioni sulla differenza tra [!UICONTROL Duration] e [!UICONTROL Planned Duration] per le attività, consulta l’articolo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Differenza tra [!UICONTROL Durata pianificata] e [!UICONTROL Durata] per le attività</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Durata in minuti]</td> 
   <td>In questo campo vengono visualizzate le stesse informazioni del campo [!UICONTROL Duration] in minuti anziché in giorni. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Durata per Occorrenza]</td> 
   <td> <p>Viene visualizzato nelle caselle [!UICONTROL Task Details] e [!UICONTROL Edit Task] di un elemento padre di attività ricorrenti. Visualizza la durata di ogni attività ricorrente. Per informazioni sulla creazione di attività ricorrenti, consulta <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Creare attività ricorrenti</a>. </p> <p> <span>Le durate modificate in singole attività ricorrenti non presentano il valore indicato in questo campo.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Tipo di durata]</td> 
   <td> <p>Campo attività che indica come il lavoro necessario per completare l'attività viene allocato agli assegnatari per tutta la durata dell'attività. Rappresenta la relazione tra la [!UICONTROL Duration] dell'attività, il [!UICONTROL Work Required] e la quantità di tempo, o [!UICONTROL Allocation], che le risorse assegnate devono spendere per l'attività per completarla. </p> <p>Questo campo viene visualizzato nella scheda [!UICONTROL Details] di un’attività. </p> <p>Le opzioni sono:</p> 
    <ul> 
     <li>[!UICONTROL Assegnazione calcolata]</li> 
     <li>Lavoro calcolato</li> 
     <li>[!UICONTROL Sforzo guidato]</li> 
     <li>[!UICONTROL Semplice]</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica dell’attività [!UICONTROL Duration] e [!UICONTROL Duration Type]</a>.</p> 
    —&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Unità di durata]</td> 
   <td>Unità utilizzata per misurare il tempo in una ricerca di alimentazione.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sforzo guidato]</td> 
   <td>Relazione tra il numero di utenti e il tempo necessario al completamento dell'attività. Man mano che si aggiungono più utenti, il tempo totale programmato per il completamento dell'attività diminuisce, ma la durata dell'attività rimane invariata. Ad esempio, se un'attività sta bombardando un barile di arachidi, l'aggiunta di più persone diminuirà il tempo pianificato, ma la durata in giorni-persona rimarrà la stessa.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo trascorso]</td> 
   <td> <p>[!UICONTROL Tempo trascorso] è un'unità di tempo per la [!UICONTROL Duration] di un'attività. È l’ora compresa tra la [!UICONTROL Pianificato data di inizio] e la [!UICONTROL Pianificato data di completamento] di un’attività che include festività, fine settimana e ora di inattività. In altre parole, il tempo trascorso è il passaggio dei giorni di calendario. </p> <p>[!DNL Workfront] supporta le seguenti unità di tempo trascorse per la durata dell'attività:</p> 
    <ul> 
     <li> <p>[!UICONTROL Elapsed Minutes]</p> </li> 
     <li> <p>[!UICONTROL Ore trascorse]</p> </li> 
     <li> <p>[!UICONTROL giorni trascorsi]</p> </li> 
     <li> <p>[!UICONTROL settimane passate]</p> </li> 
     <li> <p>[!UICONTROL Mesi trascorsi]</p> </li> 
    </ul> <p>Per ulteriori informazioni sulla durata dell'attività, compreso il tempo trascorso, vedere <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica dell’attività [!UICONTROL Duration] e [!UICONTROL Duration Type]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di fine]</td> 
   <td> <p> In un report [!UICONTROL Rate], si tratta della data in cui termina un nuovo tasso di fatturazione per un ruolo di lavoro a livello di progetto. Le ore associate al progetto antecedenti a questa data vengono moltiplicate per questo tasso di fatturazione per calcolare i ricavi del progetto. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Engagement]</td> 
   <td>L’ [!UICONTROL Work Performance Indicator] (WPI) che indica quando l’impegno e la fiducia nell’attività, nel progetto, nel team o nell’organizzazione stanno diminuendo. Ciò indica che è necessario agire per rilanciare quel credo e quell'impegno. Il WPI si misurava facendo le semplici domande, "Hai capito cosa ti aspettavi? Il lavoro che ti è stato assegnato ha fatto la differenza nell'organizzazione? Hai fatto un ottimo lavoro?"</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Enterprise Goals]</td> 
   <td>Obiettivi interfunzionali che contribuiscono alle metriche degli obiettivi aziendali.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event]</td> 
   <td>Qualsiasi modifica in un progetto o in un'attività.</td> 
  </tr> 
  <tr> 
   <td>Gestore eventi [!UICONTROL]</td> 
   <td>Attività automatizzate che si verificano quando si verificano eventi. Un esempio comune è una notifica e-mail automatica.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notifica evento]</td> 
   <td>E-mail generata da un gestore di eventi.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Spese]</td> 
   <td>Costo non manodopera per attività o progetti.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Esterno]</td> 
   <td> <p>In genere, un tipo di licenza, o un utente con tale licenza, che ha solo la capacità di rivedere le informazioni nel sistema.</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] panoramica delle licenze</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Sistema Esterno]</td> 
   <td>Qualsiasi servizio o software memorizzato e gestito al di fuori del sistema di registrazione designato.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>Uno dei principali blocchi predefiniti di un rapporto o di un elemento elenco che definisce quali informazioni vengono visualizzate sullo schermo. Per ulteriori informazioni sugli elementi di reporting, consulta <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementi di reporting: filtri, visualizzazioni e raggruppamenti</a>.</p> <p>Il filtro determina i risultati visualizzati in un rapporto o in un [!DNL Workfront] elenco dei pannelli, ad esempio progetti, attività o problemi.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>Processo di gestione dei costi, delle spese e dei dati sui ricavi della manodopera in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo Fisso]</td> 
   <td>È possibile definire un importo fisso di costo per un progetto. Questo fa parte del [!UICONTROL Planned Cost] del progetto che rappresenta l'importo necessario per completare il progetto. Per informazioni sui costi, consulta <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Costi di tracciamento</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Entrate Fisse]</td> 
   <td>Puoi definire un importo fisso di ricavi per un progetto. Questo fa parte del [!UICONTROL Planned Revenue] del progetto che rappresenta l'importo che si potrebbe ottenere se si completa il progetto. Per informazioni sui ricavi, consulta <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica di fatturazione e ricavi</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Flag]</td> 
   <td> <p> Si tratta dello stesso campo delle [!UICONTROL Status Icons], ma è disponibile solo per le visualizzazioni seguenti: </p> 
    <ul> 
     <li> Modelli [!UICONTROL] </li> 
     <li> [!UICONTROL Spese] </li> 
    </ul> <p> Per ulteriori informazioni, consulta l’articolo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Icone di stato incorporate nelle visualizzazioni</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cartella]</td> 
   <td>Le cartelle vengono utilizzate per organizzare documenti o rapporti associati a un oggetto.</td> </tr>
  <tr>
  <td>FTE (Full Time Equivalent)</td> 
   <td>Equivalente a tempo pieno che indica il tempo di disponibilità di una risorsa per il lavoro. 
   Il campo FTE viene visualizzato nelle seguenti aree: 
  <ul>
   <li> Profilo dell’utente, durante la modifica o la creazione dell’utente </li>
   <li> Pianificazione risorse </li>
   <li> Planner scenario (richiede una licenza aggiuntiva per Workfront Scenario Planner) </li>
   <li> Elenchi di utenti e rapporti </li> </ul>

<p>L’ETP deve essere un numero decimale massimo di 1 e non può essere 0. </p>
   <p> Un ETP di 1 (che è l’impostazione predefinita per il campo FTE di un utente, come definito nel suo profilo) significa che una risorsa (utente o ruolo) funziona per l’intero numero di ore, in base alla pianificazione che ne calcola la disponibilità. </p>
   <p>L’amministratore di Workfront decide quale pianificazione utilizzare per determinare la disponibilità dell’utente.  </p>
   <ul>
   <li> Quando si utilizza la pianificazione predefinita, Workfront utilizza l’FTE dell’utente trovato nel suo profilo per calcolare la disponibilità. </li>
   <li> Quando si utilizza la pianificazione dell'utente, Workfront utilizza l'orario di inattività dell'utente, <span class="preview">Valore del tempo di lavoro</span>e le ore di pianificazione predefinita per calcolare l’FTE dell’utente. </li> </ul>

<p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurare le preferenze di Gestione risorse</a>.  </p>
   <p>Per ulteriori informazioni sulla creazione di pianificazioni in Workfront, vedi <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Creare una pianificazione</a>. </p>

<p><b>NOTA</b></p>
   <p>Per tutti i calcoli nel Planner scenario, Workfront utilizza il seguente valore: 1 ETP = 8 ore.</p>
   <p>Per ulteriori informazioni, consulta <a href="../../../scenario-planner/get-started-with-scenario-planning.md">Guida introduttiva a Scenario Planner</a>. </p>
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
   <td>Diagramma di Gantt [!UICONTROL]</td> 
   <td> <p>Una cronologia visiva delle date del progetto in una visualizzazione calendario basata sulle date pianificate o previste mentre le attività del progetto sono attualmente pianificate.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Obiettivo [!UICONTROL]</td> 
   <td><p>Ci sono due concetti di obiettivi in [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>Obiettivi del progetto</b>: Una serie di obiettivi commerciali concordati dalle parti interessate di un progetto. Gli obiettivi del progetto fanno parte del Business Case di un progetto. </p> <p>Non puoi visualizzare gli obiettivi del progetto in elenchi o rapporti, ma puoi accedervi tramite l’API. </p> <p>Per informazioni sugli obiettivi del progetto Business Case, vedi <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Creare gli obiettivi del caso aziendale </a>. </p> </li> 
     <li> <p><b>Obiettivi strategici</b>: Un obiettivo strategico è un obiettivo creato per pianificare la strategia di lavoro per un periodo di tempo specifico. Puoi creare questi tipi di obiettivi utilizzando [!DNL Workfront Goals]. La tua organizzazione deve acquistare una licenza aggiuntiva e devi avere accesso a questa funzione per poter creare obiettivi strategici. [!DNL Workfront Goals] sono disponibili solo con una licenza aggiuntiva.</p> 
     <p>Per ulteriori informazioni, consulta <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] panoramica </a>. </p> 
     <p>Puoi visualizzare gli obiettivi strategici in un obiettivo o in un rapporto sul progetto e accedervi tramite l’API. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Gerarchia degli obiettivi]</td> 
   <td> <p>Nei rapporti Obiettivo e Progetto , questo è un campo di raccolta che visualizza gli obiettivi nella gerarchia a cui appartiene un obiettivo strategico quando si allinea ad altri obiettivi. Gli obiettivi sono separati da un delimitatore ▸. </p> <p>Solo i genitori dell'obiettivo e l'obiettivo vengono visualizzati in questo campo. Gli obiettivi dei bambini non vengono visualizzati. </p> <p>Per informazioni sull'allineamento degli obiettivi in [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Panoramica dell’allineamento degli obiettivi in [!DNL Workfront Goals]</a>. </p> 
   <p>Questo campo è visibile solo se l’organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sulla gestione degli obiettivi strategici utilizzando [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] panoramica </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Punteggio di successo dell’obiettivo]</td> 
   <td> In un rapporto sul progetto questo campo era utilizzato per fare riferimento agli obiettivi a livello di progetto associati al caso aziendale. Attualmente, si tratta di un campo obsoleto e non è associato ad alcuna funzionalità.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Obiettivi] </td> 
   <td> <p>In un rapporto di [!UICONTROL Project], si tratta di un campo di raccolta che visualizza tutti gli obiettivi strategici associati a un progetto. Gli obiettivi sono separati da virgole.</p> <p>Questo campo è visibile solo se l’organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sulla gestione degli obiettivi strategici utilizzando [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] panoramica</a>. Per ulteriori informazioni sugli obiettivi strategici e gli obiettivi del progetto in [!DNL Workfront], vedi "[!UICONTROL Goal]" in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global Interface Preferences]</td> 
   <td>Impostazioni di interfaccia che interessano tutti gli utenti. Le [!UICONTROL Global Interface Preferences] possono essere sovrascritte dalle [!UICONTROL User Interface Preferences].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Group]</td> 
   <td> <p>Un insieme di utenti (eventualmente dello stesso reparto o unità aziendale) che hanno accesso agli stessi oggetti. Oltre agli utenti, i gruppi possono essere associati a portfolio, programmi, progetti,<span> modelli di progetto,</span> aziende, team, pianificazioni, modelli di layout e profili della scheda attività.</p> <p>È inoltre possibile concedere autorizzazioni agli oggetti per gruppo. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Panoramica sui gruppi</a>.</p> <p>In un elenco o in un rapporto di oggetti di uno dei seguenti tipi, è possibile utilizzare il campo [!UICONTROL Group] per elencare gli oggetti di quel tipo associati a un particolare gruppo: utente, portafoglio, programma, progetto, <span>modello di progetto</span>, società, team, pianificazione, modello layout o profilo scheda attività.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Amministratore del gruppo]</td> 
   <td> <p>Utenti che gestiscono gli oggetti, gli accessi e gli utenti di gruppi di utenti designati.</p> <p> In un rapporto del gruppo , questo campo visualizza i nomi degli utenti designati come amministratori del gruppo nel gruppo. Per ulteriori informazioni sugli amministratori dei gruppi, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group with Administration Access]</td> 
   <td> <p> In un report [!UICONTROL Layout Template], [!UICONTROL Scheda attività] o [!UICONTROL Schedule report] (Pianificazione), in questo campo vengono visualizzati i gruppi a cui gli amministratori dei gruppi possono accedere per modificare il modello. Puoi anche filtrare il rapporto in base a questo campo. </p> <p> Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creare e gestire modelli di layout</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Grouping]</td> 
   <td> <p>Elemento di reporting utilizzato per classificare le informazioni in un elenco in base a un criterio comune.</p> <p>Per ulteriori informazioni, consulta la sezione "[!UICONTROL Groupings]" nell’articolo <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementi di reporting: filtri, visualizzazioni e raggruppamenti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Handoff Date]</td> 
   <td> <p>Data in cui un'attività diventa disponibile per il lavoro. La [!UICONTROL Handoff Date] è un calcolo e non può essere impostata manualmente. <br>Per ulteriori informazioni sulla [!UICONTROL Handoff Date], consulta l’articolo <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">Panoramica di [!UICONTROL Data di consegna attività]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Help Desk di [!UICONTROL]</td> 
   <td>La porzione di [!DNL Workfront] che contiene tutte le code di emissione. Il servizio di assistenza può essere utilizzato per elaborare i ticket di assistenza clienti, le richieste di progetto, i ticket dell’help desk, ecc. È la stessa dell’area delle richieste.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Owner]</td> 
   <td>In un rapporto di [!UICONTROL Hour], il [!UICONTROL Owner] è l’utente a cui vengono attribuite le ore. Questo è diverso dall'utente che registra effettivamente il tempo. Queste due entità possono a volte essere due utenti diversi. <br>Per ulteriori informazioni sul tempo di registrazione per un altro utente, consulta l’articolo <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Tempo di log</a>.</td> 
  </tr>

<tr> 
   <td>Stato delle Ore</td> 
   <td> <p>Attributo impostato da Workfront per le ore effettive registrate dagli utenti per attività, problemi o progetti. </p>

Le voci ora possono avere uno dei seguenti stati in Workfront:
<ul>
   <li><b>Inviato</b>: le ore sono state registrate su un progetto, un'attività o un problema. Essi fanno parte di un record di fatturazione o non sono ancora stati aggiunti a un record di fatturazione.</li>
   <li><b>Approvato</b>: le ore sono state registrate e approvate dal proprietario del progetto. Essi fanno parte di un record di fatturazione o non sono ancora stati aggiunti a un record di fatturazione.</li> 
   <li><b>Non approvato</b>: le ore sono state registrate e rifiutate dal proprietario del progetto. Essi fanno parte di un record di fatturazione o non sono ancora stati aggiunti a un record di fatturazione.</li>
   <li><b>Fatturato</b>: le ore sono state registrate, aggiunte a un record di fatturazione e lo stato del record di fatturazione è stato contrassegnato come Fatturato. Non richiedevano l’approvazione da parte del proprietario del progetto.</li>
   <li><b>Fatturato e approvato</b>: le ore sono state registrate, approvate dal proprietario del progetto e lo stato del record di fatturazione è stato contrassegnato come Fatturato.</li>
   </ul>


<p>Quando le ore fanno parte di un record di fatturazione, lo stato dell’ora indica se le ore sono state approvate o se il record di fatturazione a cui appartengono è stato fatturato. Lo stato dell’ora di una voce relativa a un’ora è visibile solo nell’elenco o nel rapporto di un’ora. </p>

<p>Per ulteriori informazioni sull'aggiunta di ore ai record di fatturazione, vedi la sezione "Aggiungi ore ai record di fatturazione" nell'articolo <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Creazione di record di fatturazione</a>.</p>

<p>Per ulteriori informazioni sull'approvazione del tempo di esecuzione dei progetti, vedi <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Richiedi tempo per l’approvazione di un progetto</a>.</p>

<p><b>SUGGERIMENTO</b></p>

<p>Le ore generali non registrate direttamente sugli elementi di lavoro non presentano lo stato di ora. </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Hour Type]</td> 
   <td> <p>Attributo che può essere impostato per le ore effettive registrate dagli utenti per attività, problemi o progetti. Questo è anche un attributo per le ore registrate che non sono direttamente collegate al lavoro, come [!UICONTROL Vacation] e [!UICONTROL Time Off].</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Gestione dei tipi di ora</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>L'ID è un indicatore alfanumerico associato a ogni oggetto in [!DNL Workfront]. Identifica in modo univoco ogni oggetto nel [!DNL Workfront] database. È possibile visualizzare l'ID di qualsiasi oggetto di un rapporto o di un elenco per ciascun oggetto. </p> <p>Suggerimento:   <p>Puoi anche visualizzare l’ID nell’URL della pagina dell’oggetto. Ad esempio, l’ID di un progetto potrebbe assomigliare al numero indicato nel seguente URL quando accedi alla pagina [!UICONTROL Project Details] (Dettagli progetto):</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Obiettivi individuali]</td> 
   <td>Obiettivi individuali che contribuiscono alle metriche degli obiettivi del team, ma non correlati allo sviluppo personale o professionale.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Accesso Ereditato]</td> 
   <td>Funzione di condivisione che consente l'accesso per propagarsi da un oggetto a un altro. Ad esempio, l’accesso ereditato dell’utente del progetto è definito nei record di programma e portfolio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>In [!DNL Workfront Scenario Planner], puoi dividere un piano in diverse iniziative per facilitarne la gestione. <span>Puoi creare un rapporto di [!UICONTROL Initiative] e accedere alle informazioni di [!UICONTROL Initiative] in un rapporto di [!UICONTROL Project].</span></p> <p>La [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni sulla [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">La [!DNL Scenario Planner] panoramica</a>. </p> <p>La [!DNL Initiative] il rapporto non è visibile nel [!DNL Workfront] a meno che la tua azienda non abbia acquistato un [!DNL Workfront Scenario Planner] licenza. Non puoi accedere a [!UICONTROL Initiatives] tramite l’API.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role]</span> </td> 
   <td> <p><span>Il tipo di rapporto Ruolo lavoro dell'iniziativa visualizza informazioni sui ruoli del lavoro associati a un'iniziativa del piano in [!DNL Workfront Scenario Planner].</span> </p> <p>La [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni sulla [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md">La [!DNL Scenario Planner] panoramica</a>. </p> <p><span>Questo tipo di rapporto non è visibile nel [!DNL Workfront] a meno che la tua azienda non abbia acquistato un [!DNL Workfront Scenario Planner] licenza.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role Hours]</span> </td> 
   <td> <p><span> In un rapporto Ruolo lavoro dell’iniziativa , viene visualizzato il numero di ore associate a un ruolo di lavoro in un’iniziativa.</span> </p> <p>La [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni sulla [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md">La [!DNL Scenario Planner] panoramica</a>. </p> <p>Questo campo e il tipo di rapporto [!UICONTROL Initiative Job Role] non sono visibili nel tuo [!DNL Workfront] a meno che la tua azienda non abbia acquistato un [!DNL Workfront Scenario Planner] licenza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role Count]</td> 
   <td> <p>In un rapporto sul ruolo del lavoro di un'iniziativa , viene visualizzato il numero di un ruolo di lavoro specifico associato a un'iniziativa.</p> <p>La [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni sulla [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md">La [!DNL Scenario Planner] panoramica</a>. </p> <p>Questo campo e il tipo di rapporto [!UICONTROL Initiative Job Role] non sono visibili nel tuo [!DNL Workfront] a meno che la tua azienda non abbia acquistato un [!DNL Workfront Scenario Planner] licenza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Iniziativa Data ultima pubblicazione]</td> 
   <td> <p>Un campo in un rapporto di [!UICONTROL Initiative], [!UICONTROL Initiative Job Role] e [!UICONTROL Project] che mostra la data dell’ultima pubblicazione di un’iniziativa del piano in un progetto. Puoi pubblicare le iniziative per creare progetti o per aggiornare progetti collegati alle iniziative.</p> <p>La [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni sulla [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md">La [!DNL Scenario Planner] panoramica</a>. </p> <p><span>Per informazioni sulle iniziative di pubblicazione, vedi</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Scenari di pubblicazione per creare e aggiornare progetti nel [!DNL Workfront Scenario Planner]</a>. Questo campo non è visibile nel [!DNL Workfront] a meno che la tua azienda non abbia acquistato un [!DNL Workfront Scenario Planner] licenza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ricerca in linea]</td> 
   <td>Durante la compilazione di un modulo, è stata eseguita una ricerca per individuare le voci disponibili per un campo specifico.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interfaccia Setup]</td> 
   <td>Area dell’applicazione che consente di definire visualizzazioni personalizzate, filtri, raggruppamenti, controlli elenco, ecc.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL È L'Obiettivo Dell'Azienda]</p></td> 
   <td> <p>In [!DNL goal reports], viene visualizzato un valore "[!UICONTROL True]/ [!UICONTROL False]" per ogni obiettivo strategico per indicare se l'organizzazione è assegnata all'obiettivo come proprietario. </p> 
   <p>Questo campo è visibile solo se l’organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sulla gestione degli obiettivi strategici utilizzando [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] panoramica </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Problema]</td> 
   <td> <p>Elemento di lavoro non pianificato che in genere indica un problema che impedisce il completamento di un'attività o di un progetto. Viene esaminato e valutato per ulteriori riflessioni sul lavoro</p> <p>Un [!UICONTROL Issue] può anche essere una richiesta di supporto (!UICONTROL Help Desk). Anche [!UICONTROL Change Orders], [!UICONTROL Requests] e [!UICONTROL Bugs] sono [!UICONTROL Issues].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Management]</td> 
   <td> <p>Il processo e le regole che disciplinano la definizione dei tipi di problema e il ciclo, il triage o il processo di traffico associati a ciascun tipo.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issuer Owner]</td> 
   <td>Il team o gli utenti responsabili della valutazione e del completamento di un problema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iteration]</td> 
   <td>Periodo di tempo in cui un team produce un insieme predefinito di risultati finali.</td> 
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
   <td>[!UICONTROL Ruolo processo]</td> 
   <td> <p>Utilizzato per identificare le funzioni e le responsabilità lavorative quotidiane di un utente. I ruoli di lavoro possono essere assegnati agli elementi di lavoro per identificare l'abilità necessaria per completare un processo di lavoro senza assegnarlo a un utente specifico. </p> <p>Un utente può avere più di un ruolo. Alcuni esempi includono Graphic Designer o Consultant.</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire ruoli di lavoro</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Journal Entry]</p> </td> 
   <td> <p>Oggetto di reporting che fornisce informazioni sugli aggiornamenti di sistema per i campi tracciati visualizzati nell'area [!UICONTROL Updates] di progetti, attività, problemi e altri oggetti.</p> <p>Per ulteriori informazioni, consulta <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Report sull'area [!UICONTROL Updates]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kanban Flag]</td> 
   <td> <p>In un rapporto attività o un rapporto di [!UICONTROL problema], il campo contrassegno kanban visualizza lo stato del flag impostato nel brano sulla bacheca kanban. I valori possibili sono [!UICONTROL On Track], [!UICONTROL Ready to Pull] e [!UICONTROL Is Blocked].</p> <p>Per ulteriori informazioni sull'impostazione dello stato del flag sulle storie sulla bacheca di storie Kanban, vedere l'articolo <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Usa i flag sulle storie sulla scheda Kanban</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI</td> 
   <td>Un valore misurabile che dimostra quanto efficacemente un'azienda stia raggiungendo gli obiettivi aziendali chiave.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>Quantità di tempo che deve trascorrere dopo che la data di completamento pianificata dell'attività predecessore è stata passata fino all'inizio dell'attività dipendente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipi Di Contrassegni]</td> 
   <td> <p>Metodo di calcolo del [!UICONTROL Lag]. Può essere:</p> 
    <ul> 
     <li>[!UICONTROL Days] (giorni lavorativi)</li> 
     <li>[!UICONTROL Calendario Days] (ignora le festività)</li> 
     <li>[!UICONTROL Percent]</li> 
     <li>[!UICONTROL Giorno della settimana]</li> 
    </ul> <p>Per ulteriori informazioni, consulta la sezione "[!UICONTROL Lag Types overview]" in <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Panoramica dei tipi di ritardo</a></p> </td> 
  </tr> 
  <tr> 
   <td>Miniatura grande [!UICONTROL]</td> 
   <td> <p> In un elenco o in un rapporto di documento viene visualizzata un'anteprima del documento in una miniatura. </p> <p>Seleziona <strong>Miniatura grande [!UICONTROL]</strong> per visualizzare una miniatura di 400 pixel nel rapporto.</p> <p>La dimensione della miniatura si regola quando si modifica la larghezza della colonna in un elenco o in un rapporto.</p> <p>Vedi anche "[!UICONTROL Thumbnail]" in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ultimi 10 visualizzatori]</td> 
   <td> <p>In un elenco di rapporti, questo campo visualizza i nomi di un massimo di 10 utenti che hanno visualizzato il rapporto più di recente.<br>Per ulteriori informazioni sull’utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizzazione dell'utilizzo dei rapporti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note sull’ultima condizione]</td> 
   <td> <p>In questo campo viene visualizzato l'ultimo aggiornamento immesso sul relativo oggetto dal proprietario dell'oggetto, ovvero l'attività o l'interazione più recente del proprietario su un oggetto.</p> <p>La [!DNL Last Condition Note] Se il testo della nota dell’ultima nota di un oggetto è stato eliminato, la colonna è vuota. Quando una nuova nota viene inserita sull’oggetto, diventa l’ultima nota e viene visualizzata nuovamente nella colonna. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data ultimo aggiornamento finanziario]</td> 
   <td>In un rapporto di progetto, questo campo acquisisce la data e l’ora dell’ultimo calcolo e aggiornamento delle finanze del progetto. Per informazioni sulle finanze dei progetti, consulta <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Panoramica sul finanziamento del progetto</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ultima Nota]</td> 
   <td> <p>In questo campo viene visualizzato l'ultimo aggiornamento immesso su un oggetto da qualsiasi utente. Questa è l’attività o l’interazione più recente su un oggetto.</p> <p>La colonna [!UICONTROL Last Note] è vuota se il testo dell’ultima nota di un oggetto è stato eliminato. Quando una nuova nota viene inserita sull’oggetto, diventa l’ultima nota e viene visualizzata nuovamente nella colonna.</p>
   <p>Quando questo campo viene aggiunto a un rapporto di attività, gli eventuali aggiornamenti rimangono sugli oggetti secondari, ad esempio problemi, sottoattività, documenti e così via. — dell'attività non viene visualizzato in questa colonna.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzato per ultimo da]</td> 
   <td> <p>In un elenco di rapporti, questo campo visualizza informazioni sull’utente che ha visualizzato il rapporto per ultimo.<br>Per ulteriori informazioni sull’utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizzazione dell'utilizzo dei rapporti</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data ultima visualizzazione]</td> 
   <td> <p>In un elenco di rapporti, questo campo visualizza la data dell’ultima visualizzazione del rapporto.<br>Per ulteriori informazioni sull’utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizzazione dell'utilizzo dei rapporti</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Layout Template]</td> 
   <td>Definito dall'amministratore di sistema o dall'amministratore di gruppo per identificare le schede e i rapporti visualizzati nell'area di lavoro di un determinato utente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Layout Type]</td> 
   <td>Insieme alle [!UICONTROL Custom Views], il [!UICONTROL Layout Type] specifica il tipo di [!UICONTROL Custom View]. Attualmente è disponibile solo l’elenco . In futuro, potrebbe diventare disponibile la vista [!UICONTROL Detail] (dettagli [!UICONTROL] di un oggetto).</td> 
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
   <td>[!UICONTROL Library Task]</td> 
   <td>Un modello per un'unica attività utilizzata per fornire una denominazione coerente delle attività [!UICONTROL] e delle attività modello in tutta l'applicazione.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di licenza]</td> 
   <td>Tipo di licenza allocata a un livello di accesso. Può essere [!UICONTROL Full User], [!UICONTROL Limited User] o [!UICONTROL Requester].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Piano Limite Licenze]</td> 
   <td> <p>In una visualizzazione o in un report di Gruppo, questo campo mostra il numero massimo di licenze di piano che possono essere assegnate agli utenti che hanno il rispettivo gruppo designato come gruppo principale.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lavoro Limite Licenze]</td> 
   <td> <p>In una visualizzazione o in un rapporto di gruppo, questo campo mostra il numero massimo di licenze di lavoro che possono essere assegnate agli utenti che hanno il rispettivo gruppo designato come gruppo principale.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utente limitato]</td> 
   <td>Un tipo di licenza che consente la creazione di un [!DNL Access Level] che contiene privilegi di sola visualizzazione, con la possibilità di inviare problemi, inserire note e caricare documenti.</td> 
  </tr> 
  <tr> 
   <td>Controlli elenco</td> 
   <td> <p>Parte di [!UICONTROL Interface Setup] che consente di collegare filtri, visualizzazioni e raggruppamenti personalizzati a singoli utenti o globalmente a tutti gli utenti.</p> </td> 
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
   <td> <p>Uno dei [!UICONTROL Project] di [!UICONTROL Update Types]. Questa impostazione consente di aggiornare le timeline [!UICONTROL Project Projection] e [!UICONTROL Planned] solo quando si fa clic su "[!UICONTROL Recalculated Timelines]" (Righe temporali ricalcolate). I progetti impostati in questo modo verranno ignorati durante il processo di ricalcolo leggero e quando il progetto o l’attività nel progetto viene aggiornato.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleziona il progetto [!UICONTROL Update Type] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>Si riferisce all'utente attualmente connesso. </p> <p>È consigliabile utilizzare questo campo in un filtro per rendere i rapporti più generici quando vengono condivisi con altri utenti. In questo modo, puoi creare un solo rapporto che visualizzerà informazioni diverse a seconda di chi effettua l’accesso per visualizzarle, in quanto le informazioni sono sempre personalizzate per l’utente connesso. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Max Users]</td> 
   <td> <p>Campo obsoleto. Qualsiasi informazione che questo campo potrebbe visualizzare è correlata a una caratteristica che [!DNL Workfront] è stato rimosso e il campo non può essere aggiornato. </p> <p>Nelle versioni precedenti di [!DNL Workfront], è possibile aggiornare questo campo durante la creazione o la modifica di un ruolo di lavoro. Mostra il numero totale di utenti che possono essere associati a un ruolo in ciascun progetto. Valore zero consentito per un numero illimitato di utenti che possono essere assegnati a un progetto. </p>Il campo è ancora visibile in alcuni rapporti ed elenchi, ma le informazioni visualizzate non possono essere aggiornate. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone]</td> 
   <td> <p>Indicatore che è possibile associare a un'attività per indicare che al completamento dell'attività è stato raggiunto un punto chiave nel progetto. In genere è possibile utilizzare le milestone per mostrare un evento significativo, ad esempio il completamento di una fase del progetto o di una serie di attività critiche. Le [!UICONTROL Milestones] sono in genere associate alle attività principali. È necessario creare le fasi cardine prima di poterle allegare alle attività. Per informazioni sulle milestone, vedi <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Creare un percorso cardine</a> e <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Associa milestone alle attività</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percorso Milestone]</td> 
   <td>Una raccolta di [!UICONTROL milestones]. I [!UICONTROL Paths] (Percorsi cardine) vengono utilizzati nei progetti per distinguere i progetti con determinati tipi di [!UICONTROL Milestones] da quelli con un set diverso di [!UICONTROL Milestones].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Attività Milestone]</td> 
   <td>Un'attività contrassegnata per indicare un evento segnalabile da misurare.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Module]</td> 
   <td>Un singolo passaggio all’interno di uno scenario in [!DNL Workfront Fusion] che esegue alcune funzioni in base all’app associata.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Il mio ruolo principale]</td> 
   <td> <p>Quando nei filtri viene fatto riferimento a questo elemento, vengono visualizzati gli utenti che hanno lo stesso [!UICONTROL Ruolo primario] dell’utente connesso oppure gli elementi di lavoro assegnati al [!UICONTROL Ruolo primario] dell’utente connesso.</p> <p>È consigliabile utilizzare questo campo in un filtro per rendere i rapporti più generici quando vengono condivisi con altri utenti. In questo modo, puoi creare un solo rapporto che visualizzerà informazioni diverse a seconda di chi effettua l’accesso per visualizzarle, in quanto le informazioni sono sempre personalizzate per l’utente connesso. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Home Team]</td> 
   <td> <p>Quando nei filtri viene fatto riferimento a questo elemento, in questo campo vengono visualizzati gli utenti che appartengono al [!UICONTROL Home Team] dell'utente connesso oppure gli elementi di lavoro assegnati al [!UICONTROL Home Team] dell'utente connesso. </p> <p>È consigliabile utilizzare questo campo in un filtro per rendere i rapporti più generici quando vengono condivisi con altri utenti. In questo modo, puoi creare un solo rapporto che visualizzerà informazioni diverse a seconda di chi effettua l’accesso per visualizzarle, in quanto le informazioni sono sempre personalizzate per l’utente connesso. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Convenzione per la denominazione]</td> 
   <td>Un set di regole a livello di organizzazione che utilizza i dati per creare nomi di progetti, attività e risultati finali.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Integrazione nativa]</td> 
   <td>Integrazione che non richiede codifica manuale o configurazione API. Denominata anche integrazione "preconfigurata".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Menu di navigazione]</td> 
   <td>Pannello centrale superiore dell’applicazione con collegamenti alle aree principali di [!UICONTROL Workfront].</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL Nuovo Valore Numero]</td> 
   <td>In un rapporto [!UICONTROL Journal Entry] viene visualizzato il valore aggiornato di un campo che sostituisce il valore del numero precedente.
   Per ulteriori informazioni, vedi "[!UICONTROL Valore del numero precedente]" in questo articolo.</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Giorno non lavorativo]</td> 
   <td>Giorno non allocato al completamento delle assegnazioni. Questo è solitamente un giorno di vacanza, una vacanza o un weekend.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note]</td> 
   <td>Un commento o un aggiornamento su un [!DNL Workfront] oggetto.</td> 
  </tr> 
  <tr> 
   <td>Testo della nota</td> 
   <td> <p>Viene visualizzato il testo di un aggiornamento immesso da un utente su qualsiasi oggetto. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Numero di obiettivi collegati]</td> 
   <td> <p>In un rapporto di [!UICONTROL Project], si tratta del numero di obiettivi strategici associati al progetto. Per informazioni sull’associazione di progetti a obiettivi strategici, consulta <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Aggiungere progetti agli obiettivi in  [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>Per informazioni sugli obiettivi strategici, vedi anche "[!UICONTROL Goal]" in questo articolo.</p> 
   <p>Questo campo è visibile solo se l’organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sulla gestione degli obiettivi strategici utilizzando [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Aggiungere progetti agli obiettivi in Obiettivi di Adobe Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object]</td> 
   <td> <p>Elementi e rapporti di lavoro di un’organizzazione, nonché i gruppi di utenti che li gestiscono in Workfront. Gli oggetti possono essere:</p> 
    <ul> 
     <li>[!UICONTROL Portfoli]</li> 
     <li>[!UICONTROL Programmi]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>Rapporti di [!UICONTROL]</li> 
     <li>[!UICONTROL Groups]</li> 
     <li>[!UICONTROL Team]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Comprendere gli oggetti in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipi di oggetti]</td> 
   <td>Se si crea un rapporto o un elenco contenente tutti i moduli personalizzati, è possibile utilizzare questo campo come visualizzazione o filtro per vedere quali tipi di oggetto sono associati a ciascun modulo. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Valore del numero precedente]</td> 
   <td>In un rapporto [!UICONTROL Journal Entry] viene visualizzato il valore originale di un campo prima dell’aggiornamento. Una volta aggiornato il valore di un campo, questo viene visualizzato come [!UICONTROL Nuovo valore numero] in un rapporto [!UICONTROL Journal Entry]. Per ulteriori informazioni, vedere anche "[!UICONTROL Nuovo valore di numero]".</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Solo Su Modifica]</td> 
   <td> <p>Uno dei tipi [!UICONTROL Project Update]. Quando questa opzione è selezionata, le timeline [!UICONTROL Project Projection] e [!UICONTROL Planned] vengono aggiornate solo quando viene effettuato un aggiornamento o una modifica al progetto o a un'attività all'interno del progetto. Non aggiorna il progetto ogni notte.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleziona il tipo di aggiornamento del progetto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Attività operazione [!UICONTROL]</td> 
   <td> <p>Il nome del [!UICONTROL Issue] nel [!DNL Workfront] database, utilizzato nei report in modalità testo o nei dati personalizzati calcolati.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aperto]</td> 
   <td>Problema o attività non completata, ma su cui si sta lavorando.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Org Chart]</td> 
   <td>Breve grafico organizzativo. Questo è un grafico che mostra la gerarchia di un'organizzazione. È inoltre disponibile la scheda nella schermata di dettaglio [!UICONTROL User] che visualizza e consente di impostare le relazioni [!UICONTROL User] e [!UICONTROL Reporting] dell'utente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Configurazione organizzativa]</td> 
   <td>Questo definisce [!UICONTROL Companies], [!UICONTROL Groups] e [!UICONTROL Security Profiles] per la tua organizzazione.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Altri gruppi]</td> 
   <td> <p>In un rapporto o in una visualizzazione in cui sono elencati gli utenti, questo campo visualizza tutti i gruppi in cui ogni utente è membro. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency]</span> </td> 
   <td> 
    <div> 
     <p>In un rapporto Ruolo lavoro, si tratta della valuta associata a un ruolo di lavoro. Si tratta di una sostituzione della [!UICONTROL Base Currency] stabilita nell'area [!UICONTROL Setup] dalla [!DNL Workfront] amministratore. </p> 
     <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire ruoli di lavoro</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Ignora fatturazione/ora valuta</span> </td> 
   <td> 
    <div> 
     <p>In un rapporto sul ruolo del lavoro, si tratta del tasso di fatturazione per ora del ruolo del lavoro utilizzando la [!UICONTROL Override Currency] selezionata del ruolo del lavoro.</p> 
     <p> Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire ruoli di lavoro</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Ignora costo valuta/ora]</span> </td> 
   <td> 
    <div> 
     <p>In un rapporto Ruolo lavoro, si tratta del tasso di costo per ora del ruolo lavoro utilizzando la [!UICONTROL Override Currency] selezionata per il ruolo lavoro. </p> 
     <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Creare e gestire ruoli di lavoro</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Owner]</td> 
   <td>Utente responsabile del completamento dell'oggetto designato.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Owner Type (Tipo proprietario)]</span> </td> 
   <td> 
    <div> 
     <p>In un rapporto Obiettivo , viene visualizzato il tipo di proprietario assegnato a un obiettivo strategico. Di seguito sono riportati i tipi di proprietario dell'obiettivo:</p> 
     <ul> 
      <li> <p>[!UICONTROL Utente]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL Group]</p> </li> 
     </ul> 
     <p>In questo campo non viene visualizzato alcun valore quando il proprietario dell’obiettivo è l’organizzazione. </p> 
     <p>Questo richiede una licenza aggiuntiva. Per informazioni su [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] panoramica</a>. </p> 
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
   <td> <p>Un [!UICONTROL parameter] è un campo personalizzato. Puoi creare un rapporto per tutti i parametri o campi personalizzati nel sistema. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Elemento padre]</td> 
   <td>In un report, questo campo mostra informazioni sull'elemento padre dell'oggetto. Ad esempio, in un rapporto di [!UICONTROL issue] potrebbe mostrare informazioni sull'attività o sul progetto in cui è registrato il problema; in un rapporto di attività, potrebbero essere visualizzate informazioni sull'attività principale diretta o sul progetto. Per ulteriori informazioni su quali oggetti possono avere elementi principali [!DNL Workfront], vedere la sezione "Interdipendenza e gerarchia degli oggetti" nell’articolo <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Comprendere gli oggetti in [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ritardo padre]</td> 
   <td>Il tempo che deve trascorrere tra l'avvio dell'attività padre e l'avvio dell'attività secondaria.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività padre]</td> 
   <td>Noto anche come attività di riepilogo . Si tratta di un’attività che dispone di sottoattività (denominate anche [!UICONTROL Children Tasks]). I valori [!UICONTROL Duration], [!UICONTROL Work Required] e [!UICONTROL Percent Complete] dell'attività padre vengono calcolati dalle sottoattività.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Risorse part-time]</td> 
   <td>Utente con licenza che ha una capacità inferiore alla pianificazione predefinita definita nel sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percent Complete]</td> 
   <td> <p>Campo di progetto, attività o problema che mostra la percentuale di lavoro associata all'attività, al progetto o al problema completato.</p> <p>È possibile aggiornare manualmente questo campo per i problemi e le attività di lavoro. </p> <p>Per i progetti e le attività principali, questo campo è un rollup da tutte le attività di lavoro e non è possibile aggiornarlo manualmente. </p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Panoramica del progetto [!UICONTROL Percent Complete]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permission]</td> 
   <td> <p>Diritti concessi a un utente su un oggetto, in genere assegnati in modo che possano completare il lavoro sull'elemento o visualizzare l'elemento. Puoi concedere autorizzazioni per:</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Portfoli]</li> 
     <li>[!UICONTROL Programmi]</li> 
     <li>Rapporti di [!UICONTROL]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Custom Forms]</li> 
     <li>[!UICONTROL Visualizzazioni]</li> 
     <li>[!UICONTROL Filters]</li> 
     <li>[!UICONTROL Raggruppamenti]</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Panoramica della condivisione delle autorizzazioni sugli oggetti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]</td> 
   <td> <p>Questo è un tipo di licenza completo nel [!DNL Workfront] sistema. Gli utenti devono disporre di questa funzionalità per accedere a tutte le funzioni di [!DNL Workfront].</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] panoramica delle licenze</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan] (nel [!DNL Scenario Planner])</td> 
   <td> <p>Un piano è l'oggetto principale quando si lavora con [!DNL Workfront] Planner scenario. Puoi delineare la strategia per il futuro a breve e lungo termine della tua azienda, identificare ogni risultato di alto livello e aggiungerlo come piano al [!DNL Workfront] Planner scenario. </p> <p>Non è possibile visualizzare [!DNL Scenario Planner] pianifica in un report e non puoi accedervi tramite [!DNL Workfront] API. </p> <p>La [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni sulla [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md">La [!DNL Scenario Planner] panoramica</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pianificato]</td> 
   <td> <p>Intervallo di tempo entro il quale è pianificato che si verifichi un evento. Quando crei progetti, attività o problemi in [!DNL Workfront], stabilisci le date di inizio e di fine pianificate e l’intervallo di tempo pianificato durante il quale si verificano. Questi valori rappresentano l'intenzione originale o la stima di quanto tempo un lavoro dovrebbe richiedere per essere completato. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vantaggio pianificato]</td> 
   <td>Questa è una voce manuale per Project Manager per stimare se il completamento di un progetto apporterà vantaggi monetari all'organizzazione. La specificazione di questo valore può essere parte della creazione di un [!UICONTROL Business Case] per il progetto. Per aggiornare questo valore, devi disporre delle autorizzazioni di gestione [!UICONTROL] per il progetto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Pianificato ore budget]</td> 
   <td> <p>In un rapporto di tipo [!UICONTROL Budgeted Hour] viene visualizzata la quantità di ore previste nel budget per i progetti o i ruoli del lavoro in [!UICONTROL Job Ruoli] nel [!UICONTROL Resource Planner]. </p> <p>Per informazioni sul budget di progetti o ruoli nel [!UICONTROL Resource Planner], consulta l’articolo <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Risorse di budget nelle visualizzazioni [!UICONTROL Resource Planner] utilizzando [!UICONTROL Project] e [!UICONTROL Role]</a>. Per informazioni sul rapporto [!UICONTROL Budgeted Hours], consulta l’articolo <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Rapporto: Ora budget</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di completamento pianificata]</td> 
   <td> <p>Puoi impostare manualmente la [!UICONTROL Planned Completion Date] su una data a scelta. Se non si imposta la [!UICONTROL Planned Completion Date], [!DNL Workfront] lo imposta automaticamente. Quando viene impostato automaticamente, la [!UICONTROL Planned CompletDate] è: [!UICONTROL Planned Start Date] + [!UICONTROL Duration]</p> <p>Per ulteriori informazioni, consulta i seguenti articoli:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Panoramica dell’attività [!UICONTROL Pianificazione del completamento Data]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Imposta la [!UICONTROL Pianificazione del completamento Data]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo pianificato]</td> 
   <td> <p>Totale del [!UICONTROL Costo manodopera pianificato] e del [!UICONTROL Costo spesa pianificata] del progetto. Questo non include il [!UICONTROL Planned Risk Cost] sul progetto.  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Durata pianificata]</td> 
   <td> <p>La [!UICONTROL Planned Duration] di un'attività è in genere uguale alla [!UICONTROL Duration] dell'attività. Rappresenta la differenza nei giorni tra [!UICONTROL Pianificato inizio] e le [!UICONTROL Pianificato date di completamento] dell’attività. </p> <p>Quando l'attività ha un tipo [!UICONTROL Duration] di [!UICONTROL Effort Driven], la [!UICONTROL Planned Duration] può essere diversa dalla [!UICONTROL Duration] dell'attività, in base al numero di risorse assegnate all'attività. </p> <p>Ad esempio, se un'attività con un tipo di [!UICONTROL Duration] di [!UICONTROL Effort Driven] ha una [!UICONTROL Duration] di 3 giorni e assegni all'attività una risorsa con una pianificazione a tempo pieno, anche la [!UICONTROL Planned Duration] è di 3 giorni. Se assegni tre risorse con una pianificazione a tempo pieno alla stessa attività, la [!UICONTROL Duration] rimane 3 giorni, ma la [!UICONTROL Durata pianificata] diventa 1 giorno. Anche la [!UICONTROL Planned Duration] (Durata pianificata) modifica le date di inizio pianificata e completamento pianificato dell’attività, in modo da riflettere la nuova [!UICONTROL Pianificato Duration] (Durata pianificata). Di conseguenza, viene interessata anche la timeline del progetto. </p> <p>Per ulteriori informazioni sulla differenza tra [!UICONTROL Duration] e [!UICONTROL Planned Duration] per le attività, consulta l’articolo <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Differenza tra [!UICONTROL Durata pianificata] e [!UICONTROL Durata] per le attività</a>.</p> <p>I progetti e i problemi non hanno una [!UICONTROL Pianificato Duration]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Minuti Di Durata Pianificati]</td> 
   <td> <p>Il [!UICONTROL Pianifica minuti di durata] di un progetto o di un problema è la [!UICONTROL Durata] del progetto o del problema in pochi minuti. </p> <p>Le attività non dispongono di un campo [!UICONTROL Planned Duration Minutes] (Minuti di durata pianificati). </p> <p>Le attività del modello hanno un campo [!UICONTROL Pianifica minuti di durata] che visualizza in minuti la [!UICONTROL Durata pianificata] dell’attività. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo previsto]</td> 
   <td> <p>La somma degli [!UICONTROL Importi pianificati] per tutte le spese registrate per un progetto o un'attività.</p> <p><b>ESEMPIO</b></p>
   <p>Se si crea una spesa per l'attività 1 e si immette $600.00 nel campo [!UICONTROL Importo pianificato], il [!UICONTROL Costo spesa pianificato] per l'attività sarà $600.00. </p> 
   <p>Per un progetto, [!DNL Workfront] utilizza la formula seguente per calcolare il costo di spesa pianificato:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Orario pianificato]</td> 
   <td> <p>Questo campo viene visualizzato nei progetti [!UICONTROL], nelle attività [!UICONTROL] e nelle aree problematiche, nei rapporti per progetti, attività o problemi e negli strumenti di gestione delle risorse come [!UICONTROL Resource Planner], [!UICONTROL Workload Balancer] e nel rapporto [!UICONTROL Utilization]. </p> <p>Mostra la quantità di ore che il proprietario del progetto stima che ogni attività o problema debba richiedere per il completamento. Per i progetti, si tratta in genere di un roll-up delle [!UICONTROL Pianificato Ore] dalle attività del progetto. </p> <p>Il campo [!UICONTROL Planned Hours] (Ore pianificate) potrebbe visualizzare informazioni diverse a seconda di dove vengono visualizzate. Per informazioni sull'orario pianificato, vedi <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Panoramica sull’orario pianificato</a>.</p> <p>Gli orari pianificati vengono memorizzati in minuti nel [!DNL Workfront] database. Quando si scrivono calcoli utilizzando questo campo, assicurarsi di tenere conto del fatto che le ore vengono visualizzate come minuti.<br></p> <p>Per impostazione predefinita, le ore pianificate vengono distribuite in modo uguale a tutti i giorni entro la durata di un elemento di lavoro e anche in modo uguale per tutte le risorse assegnate all'attività. Gli utenti possono aggiornare la quantità giornaliera di ore pianificate per un elemento di lavoro o le singole ore pianificate per ogni assegnatario.</p> <p>L’aggiornamento di questo campo è diverso per progetti, attività e problemi: </p> 
    <ul> 
     <li> <p>Per problemi, puoi aggiornare manualmente questo campo. Le ore pianificate del problema non vengono aggiunte al progetto Orari pianificati. </p> <p>Suggerimento: In un report del problema, uno dei campi [!UICONTROL Pianifica ore] viene sostituito dal campo [!UICONTROL Work]. Nel campo viene visualizzato il numero di ore pianificate relative al problema. Per ulteriori informazioni, vedere i campi "work" o "[!UICONTROL Work]" in questa tabella. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>Per le attività, è possibile aggiornare manualmente questo campo quando il [!UICONTROL Duration Type] dell'attività è [!UICONTROL Calculated Assignment] o [!UICONTROL Simple]. Questo campo è calcolato da [!DNL Workfront] quando il [!UICONTROL Duration Type] dell’attività è [!UICONTROL Calculated Work] o [!UICONTROL Effort Driven].<br>Per informazioni sulla durata dell’attività, consulta l’articolo <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica dell’attività [!UICONTROL Duration] e [!UICONTROL Duration Type]</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Per i progetti, [!DNL Workfront] calcola le ore pianificate aggiungendo tutte le ore pianificate da tutte le attività del progetto. </p> </li> 
    </ul> <p><b>SUGGERIMENTO</b></p> <p>È possibile visualizzare i rapporti di [!UICONTROL Planned Hours] nel progetto, nell’attività [!UICONTROL] o sui [!UICONTROL issues] anche utilizzando la modalità testo e facendo riferimento a campi aggiuntivi. Per ulteriori informazioni, consulta "<code>work</code>", "[!UICONTROL Work]" e "<code>workRequiredExpression</code>" campi in questa tabella. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo del lavoro pianificato]</td> 
   <td> 
    <p>Per un’attività, la frequenza oraria dell’utente o del ruolo moltiplicata per il numero di ore assegnate all’utente o al ruolo.</p> <p>Per un progetto, si tratta di un totale di tutti i [!UICONTROL Costi pianificati del lavoro] di tutte le attività.</p> <p>Il tasso di utilizzo dell'utente o del ruolo dipende dal tipo di costo selezionato per l'attività specificata. </p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/track-costs.md">Costi di tracciamento</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ricavi pianificati]</td> 
   <td> <p>Le attività e i progetti possono visualizzare un valore per [!UICONTROL Planned Revenue] in [!DNL Workfront]. [!UICONTROL Planned Revenue] rappresenta la quantità di denaro associata alle [!UICONTROL Pianificato hours] delle attività del progetto. Per i progetti, può anche includere il [!UICONTROL Fisso Revenue] del progetto. </p> <p>Per le attività, si tratta dei ricavi associati alle [!UICONTROL Pianificato ore] delle attività. Le ore pianificate di tutte le attività si estendono fino alle ore pianificate del progetto per contribuire al calcolo del progetto [!UICONTROL Pianificato Ore]. </p> 
   <p>[!DNL Workfront] calcola i ricavi pianificati per attività e progetti utilizzando le seguenti formule:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>Il progetto [!UICONTROL Planned Revenue] (Entrate pianificate) visualizzato nell'area [!UICONTROL Project Details] (Dettagli progetto) e nei rapporti sul progetto è diverso dal progetto Planned Revenue (Entrate pianificate) visualizzato nel rapporto [!UICONTROL Utilization]. </p> <p>I [!UICONTROL Pianificato Revenue] nell'area [!UICONTROL Project Details] (Dettagli progetto) riflettono i ricavi dell'attività e i ricavi fissi del progetto. Nel [!UICONTROL Planned Revenue] nel rapporto sull'utilizzo viene visualizzato [!UICONTROL Planned Revenue] (Entrate pianificate) associato solo alle attività del progetto. </p> 
     <p><b>ESEMPIO</b></p>  
      <p>Se il progetto ha 1 attività con 10 ore, assegnata a un Consulente con una tariffa oraria di $ 20 e il progetto ha un [!UICONTROL Fisso Revenue] di $ 100, il rapporto [!UICONTROL Utilization] visualizza $200 per [!UICONTROL Pianificato Revenue] (il [!UICONTROL Planned Revenue] associato alle ore sull'attività). La sezione [!UICONTROL Project Details] visualizza $300 (i [!UICONTROL Planned Revenue] dall'attività e i Fixed Revenue per il progetto). </p> 
    <p>Per informazioni sul tracciamento dei ricavi in [!DNL Workfront] vedere <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Panoramica di fatturazione e ricavi</a>. </p> 
    <p>Per informazioni sui calcoli dei ricavi pianificati nel rapporto Utilizzo, vedi <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Visualizza informazioni sull’utilizzo delle risorse </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo del rischio pianificato]</td> 
   <td> <p>Totale del [!UICONTROL Potenziale Cost] di tutti i rischi sul factoring del progetto nella loro probabilità di verificarsi. Questo importo non è incluso nel [!UICONTROL Planned Cost] del progetto.</p> <p>Il [!UICONTROL Planned Risk Cost] di un progetto viene calcolato con la seguente formula:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Profile]</td> 
   <td>Una raccolta di schede e sezioni del portale definita dall'amministratore che viene visualizzata sul [!DNL Workfront] Pagina principale dell’applicazione e altri dashboard.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Section]</td> 
   <td>Un componente di una scheda su una pagina del dashboard o del portale. Di solito un singolo rapporto, grafico, calendario o elenco di informazioni chiave.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Tab]</td> 
   <td>Scheda su un portale o dashboard contenente fino a tre sezioni del portale.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Portfolio [!UICONTROL]</td> 
   <td> <p>Una raccolta di progetti con caratteristiche unificanti. Questi progetti competono di solito per le stesse risorse, budget o fasce orarie. È possibile suddividere i Portfoli in Programmi e associare i progetti ai Programmi prima che vengano aggiunti a un Portfolio.</p> <p>Per ulteriori informazioni sui portfolio, consulta <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Panoramica del Portfolio in [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Management]</td> 
   <td>Area pratica incentrata sulla gestione di una raccolta o dei relativi programmi e iniziative di progetto.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfoli Optimizer]</td> 
   <td>A [!DNL Workfront] strumento per la valutazione e la definizione delle priorità dei progetti all'interno di un portafoglio.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio proprietario]</td> 
   <td>Le parti interessate responsabili della definizione delle priorità e del bilancio di un portafoglio.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Costo potenziale del rischio]</td> 
   <td>Questo è un campo di progetto che è possibile individuare in elenchi e rapporti. Mostra il costo potenziale dei rischi associati al progetto, qualora si verifichino. Per ulteriori informazioni consulta <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcolare il costo potenziale del rischio </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Predecessore]</td> 
   <td> <p>Attività che deve essere completata prima del completamento di un'attività dipendente. Anche un'attività contrassegnata come dipendenza [!UICONTROL] per un'altra attività. I predecessori consentono al planner di impostare la logica di dipendenza dalla sequenza, ad esempio per avviare un'attività al termine di un'altra attività.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Panoramica dei predecessori delle attività</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Società primaria]</td> 
   <td>L'azienda a cui appartiene l'utente, come indicato nelle impostazioni utente. È inoltre possibile associare le società a progetti.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contatto principale]</td> 
   <td><p>Il [!UICONTROL Contatto primario] è il creatore di un problema e viene automaticamente designato da [!DNL Workfront] quando qualcuno crea il problema. Puoi aggiornare manualmente questo campo se hai [!DNL Manage] autorizzazioni per il problema. Un problema può avere un solo contatto primario.</p> 
   <p>Se si modifica il contatto primario, l'utente originariamente designato come contatto principale dispone ancora dell'accesso [!UICONTROL Manage] al problema.</p>
   <p>Durante la conversione di un problema in un'attività o in un progetto, l'utente designato come [!UICONTROL Contatto principale] di diventa il [!UICONTROL Converted Issue Originator] del progetto o dell'attività. Se il [!UICONTROL Contatto principale] del problema viene aggiornato dopo la conversione, il [!UICONTROL Converted Issue Originator] verrà mantenuto come [!UICONTROL Contatto principale] del problema al momento in cui si è verificata la conversione. Vedi anche "[!UICONTROL Converted Issue Originator]" in questo articolo.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Priority]</td> 
   <td>Un valore che può essere assegnato a un'attività, un problema o un progetto per indicare l'importanza di tale attività. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Private]</td> 
   <td>In una [!UICONTROL Note] o in un documento, questa opzione rende l’oggetto nascosto alla maggior parte dei visualizzatori. Per una coda di un servizio di assistenza privato, solo gli utenti del team di coda possono inviare problemi a tale coda attraverso l'area del servizio di assistenza.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profile]</td> 
   <td>Tutte le informazioni su un account utente.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Program]</td> 
   <td> <p>Un sottoinsieme all’interno di un portfolio, in cui progetti simili possono essere raggruppati per ottenere un vantaggio ben definito.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Management]</td> 
   <td>Gestione delle dipendenze, dei rischi, dei problemi, dei requisiti e delle soluzioni per mantenere il programma in buona salute e raggiungere i vantaggi definiti dal programma.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Owner]</td> 
   <td>Le parti interessate responsabili della supervisione e dell'organizzazione delle attività per garantire che gli obiettivi del progetto siano allineati agli obiettivi aziendali.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Progress]</span> </td> 
   <td> <p>In un rapporto su obiettivi , viene visualizzata la percentuale di vicinanza al completamento di un obiettivo strategico. La percentuale di avanzamento viene visualizzata come numero. Per informazioni sugli obiettivi strategici, consulta anche "[!UICONTROL Goal]" in questa tabella.</p> <p>Questo campo è visibile solo se l’organizzazione ha acquistato [!DNL Workfront] Obiettivi. Per informazioni sulla gestione degli obiettivi strategici utilizzando [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> Aggiungere progetti agli obiettivi in [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stato di avanzamento]</td> 
   <td> <p>In un rapporto Progetto, Attività e Obiettivo, in questo campo viene visualizzato lo stato di avanzamento di progetti, attività o obiettivi strategici. Per ulteriori informazioni, consulta i seguenti articoli:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Panoramica sullo stato di avanzamento del progetto</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Panoramica sullo stato dell'avanzamento dell'attività</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Panoramica del progresso e della condizione dell’obiettivo in [!DNL Adobe Workfront Goals]</a> </p>
     <p>Il rapporto Obiettivo e lo stato di avanzamento di [!UICONTROL] per [!DNL goals] i campi sono visibili solo se l’organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sugli obiettivi strategici in [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] panoramica</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Project]</td> 
   <td> <p>Una grande quantità di lavoro che deve essere completata in un arco temporale specifico e deve utilizzare un budget e un numero di risorse specifici. Per renderlo gestibile, dividi il progetto in una serie di attività. Completare tutte le attività comporta il completamento del progetto. Per informazioni sulla pianificazione di un progetto, consulta <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Pianificare una panoramica del progetto</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assegnazione progetto Ore pianificate]</td> 
   <td> <p>In un rapporto Ruolo lavoro dell’iniziativa , viene visualizzato il numero di ore pianificate associate a un ruolo di lavoro assegnato alle attività o ai problemi del progetto. Questo campo e il tipo di rapporto [!UICONTROL Initiative Job Role] non vengono visualizzati nel [!DNL Workfront] a meno che la tua azienda non abbia acquistato un [!DNL Workfront Scenario Planner] licenza. Per informazioni sulla [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md">La [!DNL Workfront Scenario Planner] panoramica</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Details]</td> 
   <td>Dettagli dello stato corrente di un progetto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo preventivato progetto]</td> 
   <td> <p> Si tratta del [!UICONTROL Budgeted Cost] di un progetto visualizzato in elenchi e rapporti.</p><p>Vedi anche "[!UICONTROL Budgeted Cost]" in questo articolo.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Project Management]</td> 
   <td>Un insieme di criteri che determinano le soglie per la creazione, la categorizzazione e la denominazione dei progetti.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Project Overhead]</td> 
   <td>In un rapporto di [!UICONTROL Hour], questo campo è riservato per informazioni finanziarie collegate alle ore registrate con il tipo di ora di [!UICONTROL Project Time]. I progetti possono avere i propri tassi di fatturazione e se un’ora viene registrata direttamente su un progetto, questi tassi verranno utilizzati nei calcoli. In base alle impostazioni del progetto, i progetti possono avere anche valute diverse e può esserci una conversione di valuta per quelle ore. L'oggetto Project Overhead consente [!DNL Workfront] per ottenere quelle informazioni.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Owner]</td> 
   <td>Utente responsabile della gestione dell'ambito, della cronologia e delle assegnazioni di un progetto. Il responsabile approvazione predefinito per gli ordini di modifica, le modifiche finanziarie e i risultati finali.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Planning]</td> 
   <td>Processi per sviluppare e mantenere la pianificazione del progetto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Sponsor]</td> 
   <td>Un profilo di stakeholder a cui ogni utente deve riferirsi. In [!DNL Workfront], sono designati come [!UICONTROL Access Levels]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Teams]</td> 
   <td> <p>Insieme di utenti o ruoli assegnati a un progetto</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Panoramica del team di progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project tracking]</td> 
   <td>Dati utilizzati per misurare lo stato di salute e l’ambito di un progetto</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL proiettato]</td> 
   <td> <p>Stima della marca temporale del completamento del lavoro in base alle ore pianificate e alla percentuale di completamento di un'attività, un problema o un progetto.</p> <p>Si tratta delle date o della [!UICONTROL Duration] di attività, problemi o progetti. Di solito, indica date e durate più fedeli alla vita degli elementi di lavoro, dopo che alcuni lavori sono già stati completati o che è passato del tempo. </p> <p>Ad esempio, la [!UICONTROL Data di completamento prevista] di un'attività corrisponde alla data in cui [!DNL Workfront] stima che l'attività verrà completata, in base a quanto lavoro è stato fatto finora, a quante persone sono assegnate e a quanto tempo è trascorso dalla data di inizio.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scadenza prova]</td> 
   <td> <p>Nei rapporti che contengono l'oggetto [!UICONTROL Document Version] (ad esempio un rapporto [!UICONTROL Document Version] e un rapporto [!UICONTROL Proof Approvazione]), in questo campo viene visualizzato il giorno della settimana, della data, dell'ora del giorno e dell'anno della scadenza della bozza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Decisione sulla prova]</td> 
   <td> <p>Nei rapporti che contengono l'oggetto [!UICONTROL Document Version] (come un rapporto [!UICONTROL Document Version] e il rapporto [!UICONTROL Proof Approvazione]), questo campo visualizza lo stato decisionale della bozza (in attesa, le modifiche richieste o approvate)</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome bozza]</td> 
   <td> <p>Nei rapporti che contengono l'oggetto [!UICONTROL Document Version] (ad esempio un rapporto [!UICONTROL Document Version] e il rapporto [!UICONTROL Proof Approvazione]), questo campo visualizza il nome della bozza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Pages]</td> 
   <td> <p>Nei rapporti che contengono l'oggetto [!UICONTROL Document Version] (come un rapporto [!UICONTROL Document Version] e il rapporto [!UICONTROL Proof Approvazione]), questo campo visualizza il numero di pagine incluse nella bozza.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Progress]</td> 
   <td> <p>Nei rapporti che contengono l'oggetto [!UICONTROL Document Version] (come un rapporto [!UICONTROL Document Version] e il rapporto [!UICONTROL Proof Approvazione]), visualizza lo stato di avanzamento della bozza ([!UICONTROL Sent], [!UICONTROL Open], [!UICONTROL Commentato], [!UICONTROL Decision Made]).</p> <p>Per ulteriori informazioni, consulta <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Panoramica sull’avanzamento della bozza</a> in <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Panoramica sullo stato e sull’avanzamento della bozza</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proofing]</td> 
   <td>Un processo di revisione in cui uno o più utenti contrassegnano e commentano contenuti da modificare in un’immagine, in un documento di testo, in un video o nel contenuto web interattivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>In una [!UICONTROL Note] o in un documento, questa opzione rende l'oggetto accessibile ad altri utenti o anche a persone esterne [!DNL Workfront]. Per una coda del servizio di assistenza, [!UICONTROL Public] significa che tutti gli utenti che possono inviare i Problemi possono inviare i Problemi tramite l'area del servizio di assistenza.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Quality]</td> 
   <td>La percezione della qualità del lavoro all'interno dell'organizzazione.</td> 
  </tr> 
  <tr> 
   <td>Coda [!UICONTROL]</td> 
   <td>Chiamata anche Coda del tavolo dell'Aiuto. Progetto pubblicato nell’area dell’Aiuto per consentire agli utenti di inviare i relativi problemi. Di solito vengono create delle code per argomenti particolari, come bug, richieste di progetto, ecc.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proprietà coda]</td> 
   <td>Queste impostazioni definiscono le regole di invio dei problemi per un progetto che viene pubblicato nel servizio di assistenza di [!UICONTROL].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Argomento coda]</td> 
   <td> <p>Proprietà su una coda di supporto che consente agli utenti che inviano un problema di selezionare un argomento. Gli argomenti possono:</p> 
    <ul> 
     <li>Essere associato a un modulo dati personalizzato.</li> 
     <li>Assegna automaticamente il problema a un utente, ruolo o team tramite la regola di routing impostata sull'argomento selezionato.</li> 
     <li>Sposta il problema in un progetto o in una coda diversi attraverso la regola di routing impostata sull'argomento selezionato.</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Crea argomenti coda</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rank]</td> 
   <td> <p>In un rapporto di livello di accesso, puoi indicare manualmente un punteggio di [!UICONTROL Rank] del livello di accesso. Questo ti aiuta, come [!DNL Workfront] per identificare visivamente il livello di complessità associato a ciascun livello di accesso. Ad esempio, puoi assegnare numeri più bassi per livelli di accesso più complessi (a livello di piano) e numeri più alti per livelli di accesso meno complessi (a livello di richiedente). Non è possibile classificare i livelli di accesso standard. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ready]</td> 
   <td> <p>Questo campo in un report attività indica se un'attività Agile è stata contrassegnata come [!UICONTROL Ready] nel backlog. Questo flag si applica solo alle attività [!UICONTROL Agile], che sono attività assegnate a un team [!UICONTROL Agile]. </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Frequenza ricorrenza]</td> 
   <td> <p>Campo visualizzato nella casella [!UICONTROL Task Details] o [!UICONTROL Edit Task] di un elemento padre di attività ricorrenti. È la frequenza con cui si verificano le attività nella ricorrenza. Per informazioni sulla creazione di attività ricorrenti, consulta <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Creare attività ricorrenti</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Numero di riferimento]</td> 
   <td> <p>I progetti, le attività e i problemi vengono associati automaticamente a un numero di riferimento univoco al momento della creazione. Puoi visualizzare il [!UICONTROL Reference Number] nella pagina [!UICONTROL Details] di progetti, attività o problemi, oppure in un elenco o in un rapporto. </p> <p><b>SUGGERIMENTO</b><p><br>È possibile fare riferimento a numeri quando due elementi hanno lo stesso nome, in quanto i numeri di riferimento sono sempre univoci. </p> <p>[!DNL Workfront] genera automaticamente il numero di riferimento sequenziale a livello di sistema. A ogni progetto, attività o problema viene assegnato il numero successivo disponibile nella sequenza. <br></p> <p>Ad esempio, se l'utente A crea un'attività, [!DNL Workfront] potrebbe assegnare automaticamente all'attività il numero di riferimento 100. Se l'utente B crea un problema subito dopo, [!DNL Workfront] assegna al problema il numero di riferimento 101. Non è possibile modificare manualmente i numeri di riferimento. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema del rifiuto]</td> 
   <td>In un progetto o in un report attività, si tratta del problema creato quando l'approvazione per il progetto o l'attività viene rifiutata. Per informazioni sui problemi di rifiuto, consulta l’articolo <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Creazione di un processo di approvazione per gli elementi di lavoro</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo del rischio residuo]</td> 
   <td> <p>Campo di progetto che mostra la differenza tra il [!UICONTROL Costo di rischio pianificato] di un progetto e il totale di tutti i [!UICONTROL Costi effettivi] di tutti i rischi relativi al progetto. </p> <p>Il [!UICONTROL Costo del rischio rimanente] per un progetto viene calcolato utilizzando la seguente formula:</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ripianificazione]</td> 
   <td>Modifica delle date di un Progetto per riparare o superare i problemi. Ad esempio, un progetto in sospeso da diversi mesi dovrebbe essere ripianificato per riflettere date precise.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Report]</td> 
   <td>Un grafico o una tabella contenente informazioni su un dato [!DNL Workfront] e i relativi attributi.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request]</td> 
   <td> <p>Un tipo di problema che viene sottoposto a valutazione in una singola coda centralizzata e non è correlato a uno sforzo di lavoro continuo.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>Coda richieste [!UICONTROL]</td> 
   <td>Il backlog dei problemi gestiti da un processo di traffico e di valutazione.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Velocità richiesta]</td> 
   <td>Tempo totale del ciclo di lavoro da assumere e completare una richiesta.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requester]</td> 
   <td>In genere, si tratta di un tipo di licenza. Un utente con una licenza Richiedente può inviare richieste per il nuovo lavoro nel sistema.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo riservato]</td> 
   <td>Giorni specificati sull'orario personale di un utente, a indicare che l'utente non sarà disponibile per il lavoro. Vedere "[!UICONTROL Giorni non lavorativi]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risolvi il problema]</td> 
   <td> <p>In un rapporto sul problema, utilizza questo campo nelle visualizzazioni o nei filtri per fare riferimento al problema che risolve il problema. </p> <p>Per informazioni sulla visualizzazione della risoluzione degli oggetti nei rapporti, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Visualizzare informazioni sull’oggetto risolvibile e risolvibile in un rapporto</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sulla risoluzione e risoluzione di oggetti </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Project]</td> 
   <td> <p>In un rapporto sul problema, utilizza questo campo nelle visualizzazioni o nei filtri per fare riferimento al progetto che risolve il problema. </p> <p>Per informazioni sulla visualizzazione della risoluzione degli oggetti nei rapporti, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Visualizzare informazioni sull’oggetto risolvibile e risolvibile in un rapporto</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sulla risoluzione e risoluzione di oggetti </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Task]</td> 
   <td> <p>In un rapporto sul problema, utilizza questo campo nelle visualizzazioni o nei filtri per fare riferimento all’attività che risolve il problema. </p> <p>Per informazioni sulla visualizzazione della risoluzione degli oggetti nei rapporti, vedere <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">Visualizzare informazioni sull’oggetto risolvibile e risolvibile in un rapporto</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Panoramica sulla risoluzione e risoluzione di oggetti </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource]</td> 
   <td>Utenti e/o ruoli esistenti nel sistema e assegnati a team e attività di progetto.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Resource Management]</td> 
   <td> <p>[!UICONTROL Resource Management] è un set di strumenti aziendali che ti consente di prevedere con precisione l’utilizzo delle risorse in base alla loro disponibilità, in modo che il lavoro da eseguire sia completato in tempo e in base al budget. </p> <p>Con gli strumenti di gestione delle risorse è possibile pianificare la capacità a lungo termine e le esigenze di pianificazione a breve termine per le risorse. </p> <p>Per informazioni sulla gestione delle risorse in [!DNL Workfront], vedi <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Guida introduttiva a Gestione risorse</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>ID di Gestione risorse</td> 
   <td><p>In un rapporto di progetto, puoi utilizzare questa opzione quando crei un filtro per trovare un gestore di risorse specifico. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager]</td> 
   <td> <p>In un rapporto di progetto o in una vista a elenco, si tratta di un campo informativo che mostra gli utenti designati per eseguire attività di gestione delle risorse sul progetto.  Quando si utilizza "[!UICONTROL Resource Manager]" in un rapporto, viene visualizzato un elenco di gestori di risorse, con ogni gestore di risorse nel progetto separato da una virgola. Puoi designare fino a 30 gestori di risorse per un determinato progetto.</p> <p>Per ulteriori informazioni, consulta l’articolo <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Designare i responsabili delle risorse per un progetto o un modello </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Ore previste per il planner risorse] </td> 
   <td>Le ore previste nel budget per il progetto e le relative risorse nel [!UICONTROL Resource Planner]. Vedi anche "[!UICONTROL Budgeted Hours]" in questo articolo. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Resource Planner] </td> 
   <td>Avanzate [!DNL Workfront] strumento che consente di visualizzare e gestire le risorse tra progetti, ruoli o utenti. Per informazioni, consulta <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Panoramica di Resource Planner</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo manodopera a budget planner risorse]</td> 
   <td> <p>Si tratta del costo associato alle ore in budget per i ruoli di lavoro del progetto utilizzando il Planner risorse. </p> <p>Vedi anche "Costo del lavoro a budget" in questo articolo. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Pool di risorse]</td> 
   <td> <p>I pool di risorse sono insiemi di utenti che possono essere associati a un progetto. Gli utenti dello stesso pool di risorse appartengono solitamente allo stesso reparto, hanno competenze simili o complementari o sono finanziati dallo stesso budget. È possibile associare più pool di risorse a un progetto o a un utente. Un pool di risorse può essere assegnato esclusivamente a un progetto o condiviso da più progetti.</p> 
   <p>Per ulteriori informazioni sui pool di risorse, consulta <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Panoramica dei pool di risorse </a>.</p> 
   <p>Nei rapporti sul progetto, i pool di risorse mostrano tutti i pool associati a un progetto. Impossibile utilizzare l'oggetto in un raggruppamento.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utilizzo risorse]</td> 
   <td>Un rapporto che mostra il numero di ore disponibili in un determinato periodo di tempo e il numero di ore pianificate per ogni utente nel rapporto. Viene inoltre calcolato in [!UICONTROL Media Hours Al Day] e una percentuale di allocazione.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Risultato]</td> 
   <td>In [!DNL Workfront Goals], un risultato è un indicatore di avanzamento per un obiettivo. Può essere un numero, un valore percentuale o un importo in valuta che si aggiorna manualmente. Non è possibile visualizzare i risultati in un rapporto e non è possibile accedervi tramite [!DNL Workfront] API. Per informazioni sulle attività, consulta <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Guida introduttiva ai risultati e alle attività in Obiettivi di Adobe Workfront</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Revenue]</td> 
   <td>Importo fatturabile per l'attività o il progetto. L'importo può essere orario, fisso o una combinazione di entrambi.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di ricavi]</td> 
   <td>Il tipo di ricavi determina il modo in cui l’attività accumula ricavi. Alcuni esempi includono [!UICONTROL Fixed Hourly], [!UICONTROL Role Hourly] e [!UICONTROL Role Hourly w/Cap] (Ruolo orario fisso). Per informazioni sul tracciamento dei ricavi in [!DNL Workfront] vedere <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica di fatturazione e ricavi</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>In genere, si tratta di un tipo di licenza. Un utente con una licenza [!UICONTROL Reviewer] può rivedere e approvare gli elementi di lavoro nel sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk]</td> 
   <td> <p>Ciò può fare riferimento ai seguenti concetti in [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>Campo di un progetto che indica il rischio che un progetto può presentare. Puoi assegnare priorità all’esecuzione dei progetti in base al livello di rischio. I progetti possono presentare i seguenti livelli di rischio:</p> <p>- [!UICONTROL Molto Basso]</p> <p>- [!UICONTROL Low]</p> <p>- [!UICONTROL Medium]</p> <p>- [!UICONTROL High]</p> <p>- [!UICONTROL Molto Alto]</p> <p>I livelli di rischio indicati per un progetto non possono essere personalizzati. </p> <p> Per informazioni sull’aggiornamento del rischio di un progetto, consulta la sezione "Impostazioni progetto" dell’articolo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Modifica progetti</a>. Puoi visualizzare il campo di rischio di un progetto nei rapporti. </p> </li> 
     <li> <p>Evento che potrebbe verificarsi durante la durata di un progetto e che identifica un potenziale impatto sul costo, sull’ambito o sulla pianificazione del progetto. Puoi definire i rischi potenziali per un progetto e associare una probabilità che si verifichino o un costo durante la creazione del Business Case del progetto. Per informazioni sull’aggiunta di rischi al Business Case del progetto, consulta "Creare e modificare rischi sui progetti". </p> <p>Non puoi visualizzare i rischi definiti nel [!UICONTROL Business Case] nei rapporti. È possibile visualizzare solo diversi tipi di Costi di rischio nei rapporti e negli elenchi. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Rischio Cost]</td> 
   <td> <p>Il costo associato ai rischi di un progetto. Di seguito sono riportati i costi di rischio associati ai progetti che puoi visualizzare nei rapporti:</p> 
    <ul> 
     <li> <p>[!UICONTROL Costo effettivo]: un campo relativo a un rischio che mostra il costo effettivo del rischio che si è verificato. Oltre ai rapporti e agli elenchi, è possibile individuarli nella casella [!UICONTROL Modifica rischio] durante la modifica o la creazione di un rischio. </p> <p>Per i costi di progetto, task o emissione, vedere "[!UICONTROL Costo effettivo]" in questo articolo. </p> </li> 
     <li> <p>[!UICONTROL Costo del rischio pianificato]: un campo del progetto che mostra un totale di tutti i [!UICONTROL Potenziali Costi di rischio] per il progetto. Vedi anche "[!UICONTROL Planned Risk Cost]" in questo articolo. </p> <p>Per informazioni sul costo potenziale del rischio, consulta <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcolare il costo potenziale del rischio </a>. </p> </li> 
     <li> <p>[!UICONTROL Costo del rischio residuo]: un campo sul progetto che mostra la differenza tra il totale dei [!UICONTROL Costi effettivi] di tutti i rischi e il [!UICONTROL Costo rischio pianificato]. Vedi anche "Costo del rischio residuo" in questo articolo. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Management]</td> 
   <td>Processi per identificare, attenuare e monitorare il rischio.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td>Vedi "[!UICONTROL Job Role]" in questo articolo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing]</td> 
   <td>Assegnazione o spostamento automatica di un problema, in genere dovuto a un argomento della coda o a un percorso predefinito (regola di instradamento) per la coda.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing Rule]</td> 
   <td>Impostazione su progetti e code che assegna automaticamente un problema a un utente, a un ruolo o a un team oppure sposta il problema in un altro progetto o coda. Le regole di instradamento vengono generalmente utilizzate con le code del servizio di assistenza per assegnare automaticamente i problemi in arrivo.</td> 
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
   <td>Ricerca per la quale sono stati salvati i criteri di ricerca. Le Ricerche salvate semplificano l’esecuzione di nuovo lo stesso senza dover inserire di nuovo i criteri di ricerca.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>Scenario [!UICONTROL] (in [!DNL Workfront Fusion]) </td> 
   <td> <p>Uno scenario è composto da una serie di passaggi (moduli) che indicano come i dati devono essere trasferiti e trasformati tra app/servizi.</p> <p>Per informazioni sugli scenari in [!DNL Workfront Fusion], vedi <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] panoramica dello scenario</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scenario] (nel [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>In [!DNL Scenario Planner], uno scenario è una copia di un piano. </p> <p>La [!DNL Scenario Planner] richiede una licenza aggiuntiva. Per informazioni sulla [!DNL Workfront Scenario Planner], vedi <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">La [!DNL Scenario Planner] panoramica</a>. </p> <p>Per informazioni sulla creazione di scenari, consulta <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Creare e confrontare scenari di piano in [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule]</td> 
   <td>Il programma di lavoro settimanale, compresi gli orari di lavoro, combinato con i giorni liberi (ad esempio le vacanze) e i giorni di eccezione (ad esempio un sabato giorno lavorativo). Le pianificazioni possono essere applicate a progetti e utenti.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule Esenzione]</td> 
   <td>Noto anche come [!UICONTROL Modified Shift]. Giorni pianificati in contrasto con i normali orari di lavoro settimanali definiti dalla pianificazione. Ad esempio, un sabato programmato per funzionare, quando la pianificazione è impostata solo su Lavoro dal lunedì al venerdì, sarebbe un [!UICONTROL Schedule Esenzione].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scheduled Report]</td> 
   <td> <p>Quando si crea un rapporto di rapporti, è possibile visualizzare informazioni sulle pianificazioni del rapporto, se il rapporto è pianificato per la consegna utilizzando il campo [!UICONTROL Scheduled Report] (Rapporto pianificato). Questo campo mostra più valori, uno per ogni pianificazione di ciascun rapporto, in un elenco puntato. Per ulteriori informazioni sulla pianificazione dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Panoramica sulla consegna dei rapporti</a>.</p> <p>Poiché questo campo mostra più valori, non può essere utilizzato in un raggruppamento. Puoi accedervi solo in un filtro o in una visualizzazione. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modifica ambito]</td> 
   <td>Una [!UICONTROL Audit Trail] che, se attiva, genera una nota ogni volta che viene apportata una modifica all'ambito di un progetto o di un'attività, ad esempio se viene modificata una [!UICONTROL Task Duration] o [!UICONTROL Predecessors].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section]</td> 
   <td>Area sullo schermo, con la propria intestazione, creata per organizzare i dati personalizzati a scopo di visualizzazione.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sezione Break]</td> 
   <td>Uno spazio o un bordo tra le sezioni.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Security]</td> 
   <td>Le impostazioni che consentono a un utente di interagire con determinati oggetti del sistema e non con altri. Vedi anche "[!UICONTROL Access Levels]" in questo articolo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Setup]</td> 
   <td>Area in cui gli amministratori possono configurare configurazioni e preferenze del sistema.</td> 
  </tr> 
  <tr> 
   <td>Gravità [!UICONTROL]</td> 
   <td> <p>Gravità [!UICONTROL Severity] indica la probabilità che un articolo influisca sul completamento del lavoro. Ad esempio, un problema con elevata gravità può bloccare completamente il completamento di un task, ma un problema con bassa gravità può essere puramente cosmetico.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> Aggiorna gravità del problema</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Gravità [!UICONTROL]</td> 
   <td>Vedi "[!UICONTROL Severity]" in questo articolo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sharing]</td> 
   <td>Consente ad altri utenti di visualizzare o modificare un elemento specifico in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data Slack]</td> 
   <td>In una visualizzazione attività o in un report, la [!UICONTROL Data Slack] visualizza la data esatta in cui un'attività potrebbe avere un impatto sulla [!UICONTROL Data completamento] del progetto. Per informazioni sulla [!UICONTROL Data Slack] di un'attività, vedere <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Panoramica sulla data dello Slack attività</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Smart Assegnations]</td> 
   <td> <p>Quando si assegnano attività o problemi agli utenti, [!DNL Workfront] formula raccomandazioni ([!UICONTROL Smart Assignments]) su chi devono completare il lavoro, in base al tempo a disposizione per completarlo e alla loro relazione con il progetto.</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Panoramica delle assegnazioni intelligenti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>Indica l'oggetto principale di un altro oggetto. Ad esempio, un documento allegato a un'attività ha il nome dell'attività nel campo [!UICONTROL Source] di un report o di una visualizzazione del documento. un problema registrato in un progetto ha il nome del progetto nel campo [!UICONTROL Source] di un report o di una visualizzazione Issue. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data di inizio]</td> 
   <td> <p>Data di inizio del lavoro su un elemento. Ci sono diverse date di inizio in [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL Pianificato]</li> 
     <li>[!UICONTROL Effettivo]</li> 
     <li>[!UICONTROL proiettato] </li> 
    </ul> <p>In un rapporto Tasso , si tratta della data in cui inizia un nuovo tasso di fatturazione per un ruolo di lavoro a livello di progetto. Le ore associate al progetto dopo questa data vengono moltiplicate per questo tasso di fatturazione per calcolare i ricavi del progetto. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td> <p>Indicatore utilizzato per segnalare la posizione di un flusso di lavoro di un elemento di lavoro o di un obiettivo strategico.</p> <p>Per i progetti, lo [!UICONTROL Status] è un’impostazione del progetto che indica se il progetto è:</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL Bloccato] </li> 
     <li>[!UICONTROL Completato] </li> 
     <li>[!UICONTROL Dead]</li> 
    </ul> <p>Per ulteriori informazioni sullo stato del progetto, consulta <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Accedere all’elenco degli stati del progetto di sistema</a>.</p>
    <p>Per le attività, lo [!UICONTROL Status] è un'impostazione dell'attività che indica se l'attività è:</p> 
    <ul> 
     <li>[!UICONTROL Nuovo]</li> 
     <li>[!UICONTROL In Corso]</li> 
     <li>[!UICONTROL Completato]</li> 
    </ul> <p>Per ulteriori informazioni sullo stato dell'attività, consulta <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">Accedere all'elenco degli stati delle attività del sistema</a></p> <p>Per Problemi, lo [!UICONTROL Status] è un'impostazione sul problema che indica se il problema è:</p> 
    <ul> 
     <li>[!UICONTROL Nuovo]</li> 
     <li>[!UICONTROL In Corso]</li> 
     <li>[!UICONTROL In Attesa Del Feedback]</li> 
     <li>[!UICONTROL Bloccato]</li> 
     <li>[!UICONTROL Risolto]</li> 
     <li>[!UICONTROL non risolve]</li> 
     <li>[!UICONTROL Non Può Duplicare]</li> 
     <li>[!UICONTROL Verified Complete]</li> 
     <li>[!UICONTROL riaperto]</li> 
    </ul> <p>Per ulteriori informazioni sugli stati dei problemi, consulta <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Accedere all’elenco degli stati dei problemi del sistema</a>.</p> 
    <p>Per gli obiettivi strategici, lo [!UICONTROL Status] è un’impostazione dell’obiettivo che indica se l’obiettivo è:</p> 
     <ul> 
      <li>[!UICONTROL attivo]</li> 
      <li>[!UICONTROL Bozza]</li> 
      <li>[!UICONTROL Inattivo]</li> 
      <li>[!UICONTROL chiuso]</li> 
     </ul> 
     <p>Per ulteriori informazioni sugli obiettivi strategici, consulta anche "[!UICONTROL Goal]" o "[!UICONTROL Goals]" in questo articolo. </p> 
     <p>Per obiettivi strategici, questo campo è visibile solo se l’organizzazione ha acquistato [!DNL Workfront Goals]. Per informazioni sulla gestione degli obiettivi strategici utilizzando [!DNL Workfront Goals], vedi <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] panoramica</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modifica dello stato]</td> 
   <td>Una traccia di audit. Viene generata una nota quando un utente modifica lo stato del progetto, dell'attività o del problema.</td> 
  </tr> 
  <tr> 
   <td>Le icone di Stato</td> 
   <td> <p>Puoi aggiungere il campo [!UICONTROL Status Icons] incorporato come colonna nelle visualizzazioni per migliorare la visibilità nei punti chiave degli oggetti, ad esempio:</p> 
    <ul> 
     <li>Un oggetto presenta documenti allegati</li> 
     <li>Un oggetto è associato a un processo di approvazione</li> 
     <li>A un oggetto sono associate note aggiuntive</li> 
     <li>Una spesa è fatturabile o rimborsabile </li> 
     <li>Un'attività si trova su un percorso critico</li> 
     <li>Un utente appartiene a una società, a un team o si trova in un fuso orario diverso </li> 
    </ul> <p>È possibile aggiungere il campo [!UICONTROL Status Icons] nelle visualizzazioni dei seguenti oggetti: </p> 
    <ul> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Template Tasks]</li> 
     <li>Modelli [!UICONTROL]</li> 
     <li>[!UICONTROL Spese]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Users]</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Icone di stato incorporate nelle visualizzazioni</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stato Update]</td> 
   <td> <p>Questo campo mostra l'aggiornamento di stato più recente fornito dagli utenti nel campo '[!UICONTROL Update Status]'. I commenti sugli aggiornamenti di stato non vengono visualizzati nella colonna [!UICONTROL Status Update] (Aggiornamento stato).</p> <p>Per visualizzare gli stati '[!UICONTROL New], '[!UICONTROL In Process],' e '[!UICONTROL Complete]', utilizza la colonna [!UICONTROL Status].</p> <p>I commenti sugli aggiornamenti di stato non vengono visualizzati nella colonna [!UICONTROL Status Update] (Aggiornamento stato).</p> <p>Per ulteriori informazioni sugli stati, consulta l’articolo <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Aggiorna stato attività</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Statuses]</td> 
   <td>Vedi "[!UICONTROL Status]" in questo articolo.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>Storyboard</td> 
   <td>Grafico che rappresenta lo stato delle storie (attività nella metodologia agile) e il loro avanzamento verso il completamento.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Orario della storia]</td> 
   <td>Una metrica utilizzata per misurare la difficoltà o la complessità di una storia. I team Agile possono scegliere se utilizzare Ore o Punti.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Punti Storia]</td> 
   <td>Una metrica utilizzata per misurare la difficoltà o la complessità di una storia. I team Agile possono scegliere se utilizzare Ore o Punti.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategico]</td> 
   <td>Lavoro a lungo termine che modifica l'organizzazione o il funzionamento dell'organizzazione.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Allineamento strategico]</td> 
   <td>Misurazione e allineamento degli obiettivi aziendali tra portafogli e programmi.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sottoscrittori]</td> 
   <td> <p>Utenti abbonati a progetti, attività o problemi.</p> <p>Quando utilizzi questo campo in un rapporto, viene visualizzato un elenco di sottoscrittori, con ogni utente iscritto separato da una virgola.</p> <p>Per ulteriori informazioni, consulta l’articolo <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Iscriviti agli elementi in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL attività di riepilogo]</td> 
   <td>Consulta "[!UICONTROL Parent Task]" in questo articolo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sottoattività]</td> 
   <td>Un'attività figlio, che si trova sotto un'attività padre.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL System Governance]</td> 
   <td>Un insieme di criteri che governano i cambiamenti e la manutenzione di un sistema.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL System Integration]</td> 
   <td>Il processo di collegamento fisico o funzionale di diversi sistemi informatici e applicazioni software per agire come un insieme coordinato.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task]</td> 
   <td> <p>Un’attività che deve essere eseguita come passaggio verso il raggiungimento di un obiettivo finale (completamento del progetto).</p> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Panoramica delle attività</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Attributo attività [!UICONTROL]</td> 
   <td>Altri campi o oggetti associati a un'attività e che indicano alcuni dettagli relativi all'attività. Alcuni esempi sono [!UICONTROL Planned Completion Date] e [!UICONTROL Status].</td> 
  </tr> 
  <tr> 
   <td>Vincolo attività [!UICONTROL]</td> 
   <td>Vedere "[!UICONTROL Constraint Type]" e "[!UICONTROL Constraint Date]".</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Gestione attività]</td> 
   <td>Insieme di criteri che determinano le soglie per la creazione, l'assegnazione, la chiusura e la visibilità delle attività.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Attività Proprietario]</td> 
   <td>Il team o l'utente responsabile della stima dello sforzo e del completamento del compito</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Team]</td> 
   <td> <p>Una raccolta di utenti che lavorano per obiettivi o obiettivi aziendali simili. Questi utenti possono essere assegnati collettivamente a un elemento di lavoro assegnando il team all'elemento di lavoro.</p> <p>Per ulteriori informazioni sui team, vedi <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Panoramica sui team</a>.</p> <p>I progetti possono avere un team di progetto che contiene tutti gli utenti o i ruoli associati al lavoro sul progetto.</p> <p>Per ulteriori informazioni sui team di progetto, consulta <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Panoramica del team di progetto</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Template]</td> 
   <td> <p>I modelli di progetto sono contorni generici dei progetti più ripetibili. Quando si crea un modello di progetto, è possibile definire attività, mettere in coda argomenti, moduli personalizzati, allegare documenti o approvazioni per risparmiare tempo durante la creazione di un nuovo progetto. </p> <p>È possibile allegare modelli a progetti esistenti oppure utilizzarli per creare nuovi progetti. Tutte le informazioni specificate nel modello vengono trasferite ai progetti creati utilizzando tale modello. </p> <p>Per ulteriori informazioni sui modelli, consulta <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Panoramica modello di progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Template Task]</td> 
   <td>Attività che fa parte di un modello. Le attività modello diventano attività nel progetto creato utilizzando il modello.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>Una [!UICONTROL Note] e la relativa raccolta di risposte relative a un particolare argomento.</td> 
  </tr> 
  <tr> 
   <td>Miniatura</td> 
   <td> <p> In un elenco o in un rapporto di documento viene visualizzata un'anteprima del documento in una miniatura. </p> <p> Seleziona <strong>Miniatura</strong>  per visualizzare una miniatura di 33-66 pixel nel rapporto. </p> <p>La dimensione della miniatura si regola quando si modifica la larghezza della colonna in un elenco o in un rapporto.</p> <p>Vedi anche "[!UICONTROL Large Thumbnail]" in questo articolo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time Off]</td> 
   <td>Puoi creare un rapporto [!UICONTROL Time Off] per visualizzare quando gli utenti hanno indicato il momento di disattivazione nel loro profilo. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scheda attività]</td> 
   <td> <p>Scheda temporale che consente agli utenti di inserire le ore effettive di lavoro dedicate a progetti, attività o problemi o le ore trascorse per altre attività non correlate al lavoro, come riunioni o corsi di formazione. Oltre a specificare la quantità di tempo impiegato per il lavoro, è anche possibile indicare se l'ora è correlata al lavoro o se corrisponde al tempo di overhead utilizzando i tipi di ora per definire le voci di ora. Per informazioni sui fogli presenze, consulta <a href="../../../timesheets/timesheets/timesheets-overview.md">Panoramica sui fogli presenze</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profilo scheda attività]</td> 
   <td> <p>Un [!UICONTROL Profilo Scheda attività] è un modello che [!DNL Workfront] utilizza per creare automaticamente fogli presenze per gli utenti associati ad essi. </p> <p>È possibile configurare una serie di impostazioni che verranno applicate a ogni scheda attività durante la creazione. Alcune di queste impostazioni sono: con quale frequenza la scheda attività deve essere creata (settimanalmente, ogni due settimane, due volte al mese o al mese), il giorno di inizio della scheda attività, gli approvatori della scheda attività, i [!UICONTROL Hour Types] disponibili che gli utenti possono associare alle ore registrate.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL ID padre principale] </td> 
   <td> <p>Questo campo ti consente di identificare e filtrare i dati relativi a un gruppo di livello principale e ai relativi sottogruppi in un elenco o in un rapporto.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome padre principale] </td> 
   <td> <p>Questo campo ti consente di identificare i dati relativi a un gruppo di livello principale e ai relativi sottogruppi in una visualizzazione di un elenco o di un report.</p> <p>Puoi eseguire questa operazione anche utilizzando il campo [!UICONTROL Top Parent ID] (ID principale).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ore totali]</td> 
   <td> <p>In un rapporto sul progetto, questo campo visualizza la somma arrotondata di tutte le ore del progetto, l’ultima volta che sono state calcolate le finanze del progetto. Le [!UICONTROL Ore effettive] riflettono le ore esatte registrate nel progetto. In genere, le [!UICONTROL Ore effettive] devono corrispondere alle [!UICONTROL Ore totali]. Se il campo [!UICONTROL Total Hours] appare significativamente diverso da quello relativo alle ore effettive, è necessario ricalcolare le finanze nel progetto.</p> <p>Per ulteriori informazioni sul ricalcolo delle finanze dei progetti, consulta l’articolo <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Ricalcolare le finanze del progetto</a>.</p> <p>In una visualizzazione scheda attività standard, questo campo fa riferimento alle ore totali registrate per gli elementi per le date visualizzate in una scheda attività. Il campo [!UICONTROL Totale ore] per i fogli presenze in questa visualizzazione incorporata fa riferimento al campo "[!UICONTROL hoursDuration]" che calcola dinamicamente la differenza in ore tra le date di inizio e fine della scheda attività. Viene utilizzato per visualizzare in rosso la colonna [!UICONTROL Total Hours] se l'utente registra più tempo delle ore disponibili nell'intervallo di tempo della scheda attività. Per ulteriori informazioni, consulta <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">Visualizza le ore totali nella scheda attività</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tracking Mode] (Modalità di tracciamento)</td> 
   <td> <p>Attributo di un task. Questo ha determinato come e in che modo le timeline Proiettate verranno aggiornate per un’attività. Ad esempio:</p> 
    <ul> 
     <li>L’utente deve aggiornare deve aggiornare un’attività manualmente. In caso contrario, diventerà [!UICONTROL Behind Schedule] (Ritardo), quindi [!UICONTROL].</li> 
     <li>Il completamento automatico completerà automaticamente un'attività quando la data di scadenza, o [!UICONTROL Data completamento pianificato], verrà passata.</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Panoramica sulla modalità di tracciamento delle attività</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Trigger]</td> 
   <td>Un evento che avvia uno scenario.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trouble Task]</td> 
   <td>Attività incompleta con una condizione di ritardo, ritardo o rischio.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attività non assegnata]</td> 
   <td>Attività non assegnata ad alcun utente, ruolo o team.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo di aggiornamento]</td> 
   <td> <p>Un’impostazione del Progetto che determina quando verrà ricalcolata la timeline Progetto. Le opzioni sono:</p> 
    <ul> 
     <li>[!UICONTROL Automatico e On Change]</li> 
     <li>[!UICONTROL Solo automatico]</li> 
     <li>[!UICONTROL Solo Manuale] </li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Seleziona il tipo di aggiornamento del progetto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utente]</td> 
   <td>Un account creato in [!DNL Workfront] per consentire a una persona di accedere e interagire con il sistema.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL User Delegation]</p> </td> 
   <td> <p>Un oggetto di reporting che indica:</p> 
    <ul> 
     <li>Quali utenti hanno delegato attività, problemi e approvazioni dei progetti?</li> 
     <li>A quali utenti sono state delegate attività, problemi e approvazioni dei progetti?</li> 
     <li>Quando queste delegazioni iniziano e terminano</li> 
    </ul> <p>Per ulteriori informazioni, consulta <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Creare un rapporto Delega utenti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Interfaccia utente di [!UICONTROL]</td> 
   <td>Tutti gli aspetti visivi e interattivi della [!DNL Workfront] applicazione.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface Preferences]</td> 
   <td>[!UICONTROL User Interface Setup]. [!DNL Workfront] gli amministratori possono modificare queste impostazioni per personalizzare alcuni aspetti dell’interfaccia utente.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Utilizzo]</td> 
   <td>Disponibilità per un utente o un ruolo in base alla pianificazione, al PTO e al carico di lavoro corrente assegnati.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utilizzo utente]</td> 
   <td> <p>Una ricerca combinata con un rapporto che mostra come gli utenti (risorse) vengono allocati o allocati in eccesso. Vedi "[!UICONTROL Resource Utilization]" in questo articolo.</p> </td> 
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
   <td>Misurazione del tempo totale del ciclo di lavoro (quanto tempo è necessario per completare un pezzo di lavoro) e della frequenza del lavoro nel tempo originariamente impegnato (rapporto lavoro-a-commit).</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL View]</td> 
   <td> <p>Le visualizzazioni possono essere utilizzate per modificare le colonne di un report o di un elenco di progetti, attività o problemi, oppure per indicare il diritto di un utente di visualizzare solo le informazioni a livello di accesso o di condivisione delle autorizzazioni.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizza icone]</td> 
   <td> <p> Si tratta dello stesso campo delle icone di stato, ma è disponibile solo per le visualizzazioni seguenti: </p> 
    <ul> 
     <li> [!UICONTROL Documents] </li> 
    </ul> <p> Per ulteriori informazioni, consulta l’articolo <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Icone di stato incorporate nelle visualizzazioni</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni Il Mese Scorso]</td> 
   <td> <p>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato nell’ultimo mese.<br>Per ulteriori informazioni sull’utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizzazione dell'utilizzo dei rapporti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni ultimo trimestre]</td> 
   <td>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato nell’ultimo trimestre.<br>Per ulteriori informazioni sull’utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >Visualizzazione dell'utilizzo dei rapporti</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni L'Anno Scorso]</td> 
   <td>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato nell’ultimo anno.<br>Per ulteriori informazioni sull’utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizzazione dell'utilizzo dei rapporti</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni Questo Mese]</td> 
   <td> <p>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato durante il mese corrente.<br>Per ulteriori informazioni sull’utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizzazione dell'utilizzo dei rapporti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizza Questo Trimestre]</td> 
   <td>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato durante il trimestre.<br>Per ulteriori informazioni sull’utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Visualizzazione dell'utilizzo dei rapporti</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visualizzazioni Quest'Anno]</td> 
   <td>In un elenco di rapporti viene visualizzato il numero di volte in cui il rapporto è stato visualizzato durante l’anno.<br>Per ulteriori informazioni sull’utilizzo negli elenchi dei rapporti, consulta l’articolo <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">Visualizzazione dell'utilizzo dei rapporti</a>.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>In un rapporto di progetto, attività o problema, utilizzando la seguente istruzione in modalità testo viene visualizzata l’ora pianificata del progetto, dell’attività o del problema:</p>
   <p></p><p></p> 
   <p>Per informazioni sull’utilizzo della modalità testo, consulta <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Panoramica della sintassi della modalità testo</a>. </p> 
   <p><b>SUGGERIMENTO</b> 
   <p>In un rapporto del problema, l’aggiunta di uno dei campi [!UICONTROL Pianificato ore] aggiunge la variabile <code>work </code>al report. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work]</td> 
   <td> <p>Uno dei due tipi di licenza principali. Questo dispone di un accesso inferiore a [!UICONTROL Plan], ma può creare ed eseguire aggiornamenti nel sistema. Questo significa più funzionalità dei tipi di licenza [!UICONTROL External], [!UICONTROL Reviewer] o [!UICONTROL Requester].</p> <p>Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] panoramica delle licenze</a>.</p> <p>Il lavoro può fare riferimento al numero di ore pianificate per un progetto, un'attività o un problema. Per ulteriori informazioni, vedere il campo "[!UICONTROL work]" in questa tabella. </p> <p>Suggerimento: In un rapporto del problema, l’aggiunta di uno dei campi [!UICONTROL Pianificato ore] aggiunge la variabile <code>work </code>al report. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Struttura di suddivisione del lavoro]</td> 
   <td>Struttura gerarchica delle attività che il team di progetto deve eseguire in base alla relazione padre/figlio.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Sforzo di lavoro] </td> 
   <td> 
    <p>Un project manager potrebbe decidere di utilizzare questo campo invece di [!UICONTROL Pianifica ore] per stimare lo sforzo necessario per completare un'attività. Questo campo è visibile solo quando sono soddisfatte le seguenti condizioni:</p> 
     <ul> 
      <li> <p>L'attività ha un [!UICONTROL Simple Duration Type]. </p> <p>Suggerimento: Se si aggiorna l'attività [!UICONTROL Duration Type] a qualsiasi altro tipo, questo campo diventa nascosto. </p> </li> 
      <li>Il project manager ha abilitato [!UICONTROL Use Work Effort] per calcolare automaticamente il campo [!UICONTROL Planned Hours] dell’attività sul progetto. </li> 
     </ul> 
     <p>Per informazioni sull'utilizzo di [!UICONTROL Work Sfort] invece di [!UICONTROL Planned Hours] per stimare lo sforzo dell'attività, vedi <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Panoramica sullo sforzo di lavoro</a>. </p> 
     <p>È possibile visualizzare questo campo nei rapporti e negli elenchi delle attività.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Elemento di lavoro]</td> 
   <td> <p>Questo campo fa riferimento a attività o problemi in [!DNL Workfront]. </p> <p>Il rapporto [!UICONTROL Work Item] visualizza informazioni sia per le attività che per i problemi. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management mix]</td> 
   <td>Un [!UICONTROL Work Performance Indicator] (WPI) della proporzione di lavoro allocato per eseguire il tuo business rispetto a cambiare il tuo business. Il Mix WPI ti aiuta a capire, a livello organizzativo, se la tua strategia ha una reale allocazione del lavoro applicata ad esso.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Resource]</td> 
   <td>Designazione di un utente nel sistema idoneo a ricevere il tempo di lavoro o di tracciamento.</td> 
  </tr> 
  <tr> 
   <td>Ruolo e responsabilità di gestione del lavoro</td> 
   <td>Definizione dei proprietari e delle parti interessate per la gestione dell'ambito, dell'esecuzione e delle approvazioni del problema, del compito, del progetto, del programma o del portafoglio designato.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management SLA]</td> 
   <td>Una metrica quantificabile concordata da tutte le parti interessate.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Stakeholder]</td> 
   <td>Una raccolta di utenti con un interesse acquisito sui risultati di una richiesta di lavoro.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management touchpoints]</td> 
   <td>Registri digitali delle comunicazioni tra le parti interessate.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Indicatori delle prestazioni di lavoro] </td> 
   <td> <p>Rapporto misto, capacità, velocità, qualità e coinvolgimento.</p> <p>WPI è un acronimo comune per [!UICONTROL Work Performance Indicator].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Process]</td> 
   <td> <p>Il metodo in cui il lavoro viene ricevuto, assegnato alle priorità ed eseguito. Il modo in cui esegui il lavoro è in genere denominato "flusso di lavoro" o "piano di progetto" (un elenco di attività con date, relazioni predecessori e così via). </p> <p>Esempi di un processo di lavoro possono essere la produzione di una singola risorsa o la consegna di una campagna con più risorse. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modello di flusso di lavoro]</td> 
   <td>Nel rapporto [!UICONTROL Verifica approvazione], questo campo visualizza tutti i modelli di flusso di lavoro associati a una bozza. Se non sono presenti modelli allegati, la colonna è vuota.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL orario di lavoro]</td> 
   <td>

<p><span class="preview">Rappresenta la percentuale del tempo equivalente a tempo pieno (FTE) disponibile per il lavoro effettivo, esclusi i costi comuni. Il tempo di lavoro deve essere un numero decimale fino a 1 e non può essere 0. Ad esempio, una disponibilità del 20% per il lavoro effettivo sarebbe 0,2.</span>  </p>
   </p><span class="preview">L’impostazione predefinita del campo è 1, a indicare che un utente spende l’intero FTE sul lavoro effettivo correlato al progetto.</span>   </p>
   <p><span class="preview">Il sistema utilizza questo numero per calcolare la disponibilità dell'utente per il lavoro effettivo relativo al progetto. </span></p>
   <p> <span class="preview">Le eccezioni di pianificazione e il tempo di inattività potrebbero influire anche sulla capacità dell'utente.</span> </p>
   <p><span class="preview">Per ulteriori informazioni sulla creazione di pianificazioni in Workfront, consulta Creare una pianificazione. (INSERISCI COLLEGAMENTO)</span> </p>
    <p>Workfront calcola la disponibilità di un utente in base alle preferenze di Gestione risorse nell’area Configurazione. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Configurare le preferenze di Gestione risorse</a>. </p> 
   <p><span class="preview">È possibile aggiornare l'orario di lavoro di un utente quando si modifica o si crea l'utente. Per informazioni, consulta <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Modificare il profilo di un utente</a></span></p> 
   <b>SUGGERIMENTO</b> 
   <p><span class="preview">Impostare il valore Ora di lavoro su 1 per indicare che l’utente è disponibile per il lavoro relativo al progetto per l’intero equivalente a tempo pieno.</span></p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Orario di lavoro]</td> 
   <td>Nella documentazione di Workfront, questo termine viene utilizzato per descrivere il tempo assegnato al lavoro, in base a una pianificazione.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>In un rapporto di progetto, attività o problema, utilizzando la seguente istruzione in modalità testo viene visualizzato il numero di ore pianificate del progetto, dell'attività o del problema seguito dalla parola "Ore":</p>
   <p></p><p></p>
    <p>Per informazioni sull’utilizzo della modalità testo, consulta <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Panoramica della sintassi della modalità testo</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
