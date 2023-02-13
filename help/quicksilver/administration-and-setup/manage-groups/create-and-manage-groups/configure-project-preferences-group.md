---
title: Configurare le preferenze di progetto per un gruppo
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: Se sei un amministratore di gruppo e un amministratore di Adobe Workfront sblocca una preferenza di progetto per tutti i gruppi del sistema, puoi configurare tale preferenza affinché il gruppo influisca su tutti i progetti successivi creati dal gruppo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: 11c4028038fe3d410ee0d4f238d2138435d9a3fa
workflow-type: tm+mt
source-wordcount: '2643'
ht-degree: 3%

---

# Configurare le preferenze di progetto per un gruppo

Se sei un amministratore di gruppo e un amministratore di Adobe Workfront sblocca una preferenza di progetto per tutti i gruppi del sistema, puoi configurare tale preferenza affinché il gruppo influisca su tutti i progetti successivi creati dal gruppo.

Se ci sono gruppi al di sopra del gruppo che gestisci, i loro amministratori possono farlo anche per il tuo gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

>[!NOTE]
>
>* In genere, una preferenza sbloccata rimane sbloccata a tempo indeterminato. Se l’amministratore di Workfront lo blocca nuovamente, l’impostazione di sistema ha effetto nuovamente e le impostazioni relative alle preferenze effettuate dagli amministratori del gruppo vengono perse.
>* Le preferenze impostate per il gruppo associato a un progetto hanno la precedenza sulle preferenze impostate per il gruppo Home dell’utente che crea il progetto.
>* Alcune preferenze a livello di gruppo influiscono sui modelli di progetto creati per il gruppo. Per ulteriori informazioni, consulta la sezione . [Visualizza, utilizza e crea modelli per il gruppo dall’area Gruppi](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) nell&#39;articolo [Creare e modificare i modelli di progetto di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Dopo che un amministratore di Workfront sblocca una preferenza a livello di sistema, puoi configurarla e bloccarla per garantire che tutti gli utenti del gruppo e dei sottogruppi utilizzino la stessa configurazione. Ciò è parallelo alla possibilità che un amministratore di Workfront debba configurare e bloccare una preferenza per tutti gli utenti del sistema. Per ulteriori informazioni, consulta [Bloccare o sbloccare un progetto, un&#39;attività o una preferenza di problema per i sottogruppi](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


La configurazione a livello di gruppo è possibile anche per le preferenze relative a attività e problemi e per le preferenze relative alla scheda attività e alle ore. Per informazioni, consulta [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) e [Configurare le preferenze relative a schede attività e ora per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

Per informazioni su come un amministratore di Workfront sblocca una preferenza di progetto, consulta [Bloccare o sbloccare le preferenze del progetto per tutti i gruppi del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> <p>È necessario essere un amministratore del gruppo o un amministratore di Workfront. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Amministratori di gruppo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo amministratore Workfront.

## Configurare una preferenza di progetto sbloccata per un gruppo

>[!TIP]
>
>Gli amministratori di Workfront possono ignorare i passaggi 1-4 selezionando Configurazione > Preferenze progetto > Progetti e quindi ricercando il nome del gruppo nella casella nella parte superiore della pagina.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Fare clic sul nome del gruppo di cui si desidera configurare le preferenze di progetto.
1. Nel pannello a sinistra, fai clic su **Preferenze del progetto**.
1. Nella pagina visualizzata, continua con una delle 4 sezioni elencate di seguito per configurare le preferenze per Stato del progetto, Timeline, Casi aziendali e Vita dopo la morte.

   >[!TIP]
   >
   >Se passi il puntatore del mouse su una preferenza e viene visualizzata una descrizione comandi che indica che è bloccata, puoi chiedere all’amministratore di Workfront di sbloccarla per tutti i gruppi dell’organizzazione.

* [Stato progetto](#project-status)
* [I Timeline](#timelines)
* [Casi di studio](#business-cases)
* [Vita dopo la morte](#life-after-death)

### Stato Progetto {#project-status}

Configura una delle seguenti preferenze per i progetti appena creati associati al gruppo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>Consenti agli utenti di creare progetti senza utilizzare un modello</td>
<td><p>Questa preferenza consente agli utenti di creare progetti senza utilizzare un modello quando si crea un progetto dalle aree seguenti:</p>
<ul>
<li><p>Utilizzare l’opzione Nuovo progetto in un elenco di progetti</p></li>

<li><p>Convertire un problema in un progetto dalla pagina del problema</p></li>
</ul>

<p>Questa preferenza è attivata per impostazione predefinita a livello di sistema.</p>
<p><b>NOTA</b></p>
<p>Se un utente appartiene a più gruppi con preferenze diverse, potrà creare un progetto senza un modello se almeno uno dei gruppi dispone di questa preferenza abilitata.</p>
</td></tr>
  <tr> 
   <td role="rowheader">Imposta lo stato del nuovo progetto su</td> 
   <td> <p>Determinare lo stato dei nuovi progetti.</p> <p><b>NOTA</b>   
     <ul> 
      <li>Se lo stato selezionato è nascosto da un utente o da un altro amministratore Workfront, lo stato predefinito viene modificato nel primo stato dell’elenco di stato.</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">Per le preferenze del progetto di gruppo, è possibile selezionare come stato predefinito solo uno stato bloccato o uno stato obbligatorio.</li> 
      <li> <p>Se lo stato predefinito di un sistema o di un gruppo bloccato è impostato come stato predefinito e successivamente un utente lo sblocca, il sistema cerca di sostituirlo con uno stato bloccato dello stesso tipo di stato.</p> <p>Se non ne trova uno, cerca uno stato obbligatorio:</p> 
       <ul> 
        <li>Se è presente uno stato obbligatorio che corrisponde allo stato predefinito sbloccato, lo stato richiesto diventa quello predefinito, anche se sbloccato.</li> 
        <li>Se nessuno degli stati richiesti corrisponde allo stato predefinito sbloccato, il primo stato richiesto nell’elenco dello stato diventa lo stato predefinito.</li> 
       </ul> <p>Per informazioni sugli stati richiesti, consulta gli articoli <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Accedere all’elenco degli stati del progetto di sistema</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Accedere all'elenco degli stati delle attività del sistema</a>e <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Accedere all’elenco degli stati dei problemi del sistema</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calcola la percentuale di completamento sulla base di</td> 
   <td> <p>La percentuale di completamento di un progetto o di un'attività padre si basa sull'avanzamento complessivo delle attività. Queste informazioni possono essere calcolate in base alla Durata o all'Ora pianificata delle attività di un progetto.</p> <p>Se si seleziona Durata, la Durata di ogni attività in un progetto determina la percentuale di completamento totale del progetto e la Durata di ogni sottoattività determina la percentuale di completamento totale per l'attività padre.</p> <p>Se si seleziona Durata, assicurarsi di specificare gli orari tipici per giorno lavorativo e i giorni lavorativi tipici per settimana nella sezione Timeline. Workfront utilizza queste informazioni per calcolare la percentuale di completamento di un'attività in base alla Durata. </p> <p>Se si seleziona Orari pianificati, assicurarsi che per tutte le attività di ciascun progetto sia definito il numero di ore pianificate e che l'importo non sia zero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Imposta automaticamente la condizione del progetto sulla base dello stato di avanzamento</td> 
   <td> <p>Questa preferenza consente agli utenti di impostare manualmente la condizione di un progetto (Su Target, A rischio, Nei problemi) o di impostare automaticamente la condizione (Stato avanzamento) in base alla progressione del progetto sulla timeline. Per ulteriori informazioni sulla condizione dei progetti, consulta <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Panoramica del tipo di condizione e condizione del progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Crea linee di base automaticamente</p> </td> 
   <td> <p>Questa preferenza crea automaticamente una baseline (snapshot) dei dettagli dell'attività e del progetto quando lo stato del progetto diventa Corrente. Per informazioni sulla creazione delle linee di base, consulta <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Creare le linee di base dei progetti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Metodo Indicizzazione Performance </p> </td> 
   <td> <p>Il metodo PIM (Performance Index Method) per il progetto controlla il metodo utilizzato da Workfront per calcolare le metriche del valore generato, ad esempio Indice prestazioni costo (CPI) e Stima al completamento (EAC). Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcola indice di prestazione dei costi (CPI)</a>e <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcola Stima Al Completamento (EAC)</a></p> 
    <ul> 
     <li><strong>Basato su ora</strong>: Workfront utilizza le ore pianificate per calcolare le metriche delle prestazioni come EAC e CPI. Quando il PIM viene calcolato in base alle ore, l'EAC viene visualizzato come numero di ore. Assicurati di avere un valore per Orari pianificati diverso da zero.</li> 
     <li> <p><strong>Basato sui costi</strong>: Workfront utilizza il costo del lavoro pianificato per calcolare le metriche delle prestazioni come EAC e CPI. Assicurati che i ruoli o gli utenti del tuo lavoro siano associati ai tassi di costo per ora. Quando il PIM viene calcolato in base ai costi, l'EAC viene visualizzato come valore di valuta.</p> <p>Il project manager può modificare questa impostazione a livello di progetto utilizzando l'area Finanza in Dettagli progetto. Per ulteriori informazioni, vedere <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gestire le informazioni nell'area di finanziamento del progetto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Stima al completamento </p> </td> 
   <td> <p>Determinare i dati utilizzati da Workfront per calcolare la stima al completamento (EAC) che rappresenta il costo totale previsto di un progetto.</p> 
    <ul> 
     <li><strong>Calcola a livello di progetto</strong>: l'EAC per l'attività e il progetto padre viene determinato inserendo le ore effettive o il costo effettivo del lavoro nelle formule EAC. Questo calcolo include le ore o i costi effettivi e le spese aggiunte direttamente all'attività o al progetto padre.</li> 
     <li> <p><strong>Eseguire il rollup da attività/sottoattività</strong>: L'EAC per l'attività e il progetto padre viene determinato sommando l'EAC per ogni attività figlio. Questo calcolo esclude le ore effettive o i costi e le spese effettivi aggiunti direttamente all'attività o al progetto padre.</p> <p>Il project manager può modificare questa impostazione a livello di progetto utilizzando l'area Finanza in Dettagli progetto. Per ulteriori informazioni, vedere <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gestire le informazioni nell'area di finanziamento del progetto</a>.</p> </li> 
    </ul> <p>Per ulteriori informazioni su come l'EAC calcola, vedi <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcola Stima Al Completamento (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### I Timeline {#timelines}

Configura una delle seguenti preferenze per i progetti appena creati associati al gruppo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pianifica da</td> 
   <td> <p>Determinare se i nuovi progetti sono programmati a partire dalla data di inizio o dalla data di completamento al momento della creazione.</p> 
    <ul> 
     <li><strong>Data di inizio</strong>: Per impostazione predefinita, ai nuovi task viene richiesto di specificare una data di inizio pianificata per il progetto.</li> 
     <li><strong>Data completamento</strong>: Per impostazione predefinita, ai nuovi task viene richiesto di specificare una data di completamento pianificata per il progetto in quanto più tardi possibile Vincolo attività e ai project manager.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Indisponibilità utente</td> 
   <td> <p>Determinare se l'ora dell'assegnatario principale di un'attività regola le date pianificate per tale attività su un progetto.</p> 
    <ul> 
     <li> <p><strong>Considerare il tempo di inattività dell'utente nelle durate delle attività</strong>: Qualsiasi orario non programmato per l'assegnatario principale di un'attività regola le date pianificate dell'attività se l'orario di inattività si verifica durante la sua durata. Questa è l’impostazione predefinita. </p> <p>Ad esempio, se un'attività con un vincolo il più presto possibile inizia il 1° giugno e viene completata il 3 giugno e l'assegnatario principale ha il 2 giugno contrassegnato per il timeout, le date pianificate dell'attività si adeguano al 1° giugno e al 4 giugno.</p> <p><b>IMPORTANTE</b>: La durata dell'attività non cambia quando si seleziona questa impostazione. Cambiano solo le date pianificate, a seconda del Vincolo attività.</p> </li> 
     <li><strong>Ignora il tempo di inattività dell'utente nelle durate dell'attività</strong>: Le date pianificate di ogni attività di un progetto rimangono come originariamente pianificato, anche se l'Assegnatario principale di un'attività ha un tempo di inattività durante la sua durata.</li> 
    </ul> <p>Quando selezioni le opzioni per questa impostazione, tieni presente quanto segue:</p> 
    <ul> 
     <li>Quando modifichi questa impostazione, solo i progetti e i modelli creati dopo la modifica ereditano l’impostazione aggiornata. </li> 
     <li> <p>Il valore Vincolo attività dell'attività determina le date dell'attività pianificate da modificare: </p> 
      <ul> 
       <li>La data di inizio pianificata</li> 
       <li>La data di completamento pianificata</li> 
       <li>Entrambe le date</li> 
       <li>Nessuna data. </li> 
      </ul> <p>Ad esempio, se un'attività presenta un Vincolo di date fisse, le date non vengono modificate quando l'Assegnatario principale ha un tempo di inattività, anche se è selezionata l'opzione Considera il tempo di inattività dell'utente nella durata dell'attività. Per informazioni sui vincoli delle attività, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Panoramica sul vincolo di attività</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Le sequenze temporali dei progetti saranno ricalcolate automaticamente</strong> </p> </td> 
   <td> <p>Determina quando viene ricalcolata la timeline di un progetto. Per informazioni sul ricalcolo della timeline del progetto, consulta <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Ricalcolare le timeline dei progetti</a>.</p> <p>Le seguenti opzioni sono abilitate per impostazione predefinita. È possibile selezionare una o più delle seguenti impostazioni:</p> 
    <ul> 
     <li> <p><strong>Ogni notte</strong>: Seleziona questa opzione per ricalcolare le timeline del progetto ogni notte. Le modifiche apportate al progetto che potrebbero influenzare la timeline non sono immediatamente visibili. Workfront ​ ​ ricalcola le tempistiche di notte solo per i progetti in cui sono soddisfatte entrambe le seguenti condizioni:</p> <p> 
       <ul> 
        <li>Hanno lo stato Current</li> 
        <li>Aver avuto un aggiornamento negli ultimi 3 mesi</li> 
       </ul> </p> </li> 
     <li> <p><strong>Quando l’ambito di un progetto cambia</strong>: Selezionare questa opzione per ricalcolare immediatamente le timeline del progetto in seguito alla modifica dell’ambito del progetto. Per informazioni sulla modifica dell’ambito di un progetto, consulta <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Ricalcolare le timeline dei progetti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Quando più utenti vengono assegnati a un'attività, utilizza la pianificazione del</strong> </p> </td> 
   <td> <p>Se a un progetto non è assegnata una pianificazione o se gli utenti assegnati alle attività non dispongono di una pianificazione assegnata, Workfront utilizza la pianificazione predefinita del sistema per calcolare la cronologia delle attività.</p> <p>Se si assegnano più utenti alla stessa attività in un progetto con una pianificazione assegnata e gli utenti assegnati alle attività dispongono anche di una pianificazione assegnata a loro, Workfront utilizza le seguenti pianificazioni:</p> 
    <ul> 
     <li><strong>Assegnazione principale</strong>: Workfront utilizza la pianificazione dell'assegnazione principale sull'attività per calcolare le timeline.</li> 
     <li><strong>Progetto</strong>: Workfront utilizza la pianificazione del progetto per calcolare la timeline di ogni attività.</li> 
    </ul> <p>Per ulteriori informazioni sulle pianificazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Creare una pianificazione</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Calcoli sequenza temporale </p> </td> 
   <td> 
    <ul> 
     <li><strong>Orari tipici per giorno lavorativo</strong>: Imposta il numero di ore in un giorno lavorativo tipico per gli utenti che lavoreranno ai progetti. Il valore predefinito è 8 ore.</li> 
    </ul> 
    <ul> 
     <li><strong>Giorni di lavoro tipici a settimana</strong>: Imposta la settimana lavorativa standard per gli utenti che lavoreranno ai progetti. Il valore predefinito è 5 giorni.</li> 
    </ul> <p>Queste 2 opzioni consentono di convertire giorni in ore o settimane in giorni.</p> <p>Ad esempio, se disponi di un’attività con 8 ore pianificate e la durata viene calcolata in base all’ora pianificata, Workfront converte tali ore in giorni per mostrare la durata come giorni.</p> <p>Dal campo Giorni lavorativi tipici per settimana, Workfront calcola il valore FTE (Full Time Equivalent) del sistema. Questo è ciò che Workfront utilizza per calcolare le allocazioni per gli utenti.</p> <p>Questi valori vengono utilizzati per la pianificazione delle timeline dei progetti, per l’impostazione del budget per le risorse o per il tempo di registrazione rispetto ai progetti. </p> <p>Non vengono utilizzati quando si stabiliscono fogli presenze per gli utenti nel sistema, come descritto in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Configurare le preferenze relative a schede attività e ora</a>.</p> <p><b>NOTA</b>: Gli amministratori di Workfront non possono sbloccare le preferenze per i calcoli della timeline.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>Trimestri personalizzati</strong> </p> </td> 
   <td> <p>Configura i trimestri annuali personalizzati per gli utenti che lavoreranno ai progetti. I trimestri personalizzati sono solitamente trimestri che non corrispondono alla ripartizione tradizionale dei trimestri durante un anno civile. È possibile aggiungere più trimestri personalizzati. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Abilita trimestri personalizzati per i progetti</a>.</p> <p><b>NOTA</b>: Gli amministratori di Workfront non possono sbloccare le preferenze dei trimestri personalizzati.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Casi di studio {#business-cases}

È possibile creare un Business Case per i progetti appena creati associati al gruppo per inviare richieste di progetto. È possibile definire le preferenze per determinare quali aree sono visibili nella **Business case** modulo. Abilita queste opzioni in modo che altri strumenti, come Portfoli Optimizer, si aggiornino correttamente. Per ulteriori informazioni sulla visualizzazione di ciascun campo, consulta [Definire un caso aziendale](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Dopo che l&#39;amministratore di Workfront abilita le sezioni del Business Case, un proprietario del progetto può quindi creare un Business Case a livello di progetto. Per informazioni sulla creazione di un Business Case, vedere [Creare un business case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### Vita dopo la morte  {#life-after-death}

Configura una delle seguenti preferenze per i progetti appena creati associati al gruppo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>Dopo aver contrassegnato un progetto come Completo, le persone possono ancora</strong> </p> </td> 
   <td> <p>Determina le regole per l'organizzazione (o gruppo, se stai configurando le preferenze di progetto per un gruppo) per determinare se un'attività o un problema può essere eliminato dopo che lo stato del progetto è stato contrassegnato come Completato.</p> 
    <ul> 
     <li><strong>Elimina attività</strong>: Consente agli utenti di eliminare le attività da un progetto dopo che il progetto è stato contrassegnato come Completo.<br></li> 
     <li><strong>Elimina problemi</strong>: Consente agli utenti di eliminare i problemi da un progetto dopo che il progetto è stato contrassegnato come Completo.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Dopo che un progetto è contrassegnato come Completo, Morto o In attesa di approvazione, le persone possono ancora</strong> </p> </td> 
   <td> <p>Determinare le regole per l'organizzazione (o gruppo, se si configurano le preferenze di progetto per un gruppo) relative a operazioni, problemi, documenti e altri oggetti in un progetto dopo aver contrassegnato lo stato del progetto <strong>Completa</strong>, <strong>Morto</strong>oppure <strong>Approvazione in sospeso</strong>.</p> 
    <ul> 
     <li><strong>Aggiungi e modifica attività</strong> Consente agli utenti di: 
      <ul> 
       <li>Modifica le attività all’interno di un progetto dopo che il progetto è stato contrassegnato come Completato, Morto o In attesa di approvazione. Ciò include l'aggiunta di ore e la modifica di voci di spesa in un'attività.</li> 
       <li>Aggiungi attività a un progetto.</li> 
      </ul></li> 
     <li><strong>Aggiungi e modifica problemi</strong>: Consente agli utenti di: 
      <ul> 
       <li>Modifica i problemi all’interno di un progetto dopo che il progetto è stato contrassegnato come Completato, Morto o In attesa di approvazione.</li> 
       <li>Aggiungi i problemi a un progetto dopo che il progetto è stato contrassegnato come Completato o Morto. (Non è possibile aggiungere problemi a un progetto in attesa di approvazione.)</li> 
      </ul></li> 
     <li> <p><strong>Aggiungere documenti al progetto e alle relative attività e problematiche</strong>: Consente agli utenti di aggiungere documenti a un progetto (o di aggiungere documenti a attività e problemi all’interno del progetto) dopo che il progetto è stato contrassegnato come Completo o Morto.</p> <p>Questa opzione non si applica ai progetti in attesa di approvazione.</p> </li> 
     <li> <p><strong>Allega modelli</strong>: Consente agli utenti di allegare modelli a un progetto dopo che il progetto è stato contrassegnato come Completo o Morto.</p> <p>Questa opzione non si applica ai progetti in attesa di approvazione.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
