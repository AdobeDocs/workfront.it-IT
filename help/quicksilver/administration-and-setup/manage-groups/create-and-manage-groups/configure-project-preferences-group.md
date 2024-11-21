---
title: Configurare le preferenze del progetto per un gruppo
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: Adobe Workfront Se l'amministratore di un gruppo sblocca una preferenza di progetto per tutti i gruppi del sistema, è possibile configurare tale preferenza affinché il gruppo influisca su tutti i progetti successivi creati dal gruppo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: ef7f5d00bd74feee5e06b935c4bb8a18ee8b08a8
workflow-type: tm+mt
source-wordcount: '2825'
ht-degree: 1%

---

# Configurare le preferenze di progetto per un gruppo


<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Adobe Workfront Se l&#39;amministratore di un gruppo sblocca una preferenza di progetto per tutti i gruppi del sistema, è possibile configurare tale preferenza affinché il gruppo influisca su tutti i progetti successivi creati dal gruppo.

Se al di sopra del gruppo gestito sono presenti gruppi, anche gli amministratori possono eseguire questa operazione per il gruppo. Lo stesso vale per gli amministratori di Workfront (per qualsiasi gruppo).

>[!NOTE]
>
>* In genere, una preferenza sbloccata rimane sbloccata a tempo indeterminato. Se l&#39;amministratore di Workfront la sblocca nuovamente, l&#39;impostazione di sistema riprende ad avere effetto e le impostazioni relative alle preferenze impostate dagli amministratori di gruppo andranno perse.
>* Le preferenze impostate per il gruppo associato a un progetto hanno la precedenza su quelle impostate per il gruppo predefinito dell&#39;utente che crea il progetto.
>* Alcune preferenze a livello di gruppo influiscono sui modelli di progetto creati per il gruppo. Per ulteriori informazioni, vedere la sezione [Visualizzare, utilizzare e creare modelli per il gruppo dall&#39;area Gruppi](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) nell&#39;articolo [Creare e modificare i modelli di progetto di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Dopo che un amministratore di Workfront ha sbloccato una preferenza a livello di sistema, è possibile configurarla e quindi bloccarla per assicurarsi che tutti gli utenti del gruppo e dei relativi sottogruppi utilizzino la stessa configurazione. Ciò è parallelo alla possibilità che un amministratore di Workfront deve configurare e bloccare una preferenza per tutti gli utenti del sistema. Per ulteriori informazioni, vedere [Bloccare o sbloccare un progetto, un&#39;attività o una preferenza di problema per i sottogruppi](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

La configurazione a livello di gruppo è possibile anche per le preferenze di attività e problemi e per le preferenze di schede orario e ore. Per informazioni, consulta [Configurare le preferenze per attività e problemi per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) e [Configurare le preferenze per ore e schede orario per un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

Per informazioni su come un amministratore di Workfront sblocca una preferenza di progetto, vedere [Bloccare o sbloccare le preferenze di progetto per tutti i gruppi del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>Oppure</p>
       <p>Corrente: Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Devi essere un amministratore di gruppo del gruppo o un amministratore di sistema.</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurare una preferenza di progetto sbloccata per un gruppo

>[!TIP]
>
>Se sei un amministratore di Workfront, puoi evitare i passaggi 1-4 andando in Configurazione > Preferenze progetto > Progetti, quindi cercando il nome del gruppo nella casella nella parte superiore della pagina.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Gruppi** ![](assets/groups-icon.png).

1. Fai clic sul nome del gruppo di cui desideri configurare le preferenze di progetto.
1. Nel pannello a sinistra, fai clic su **Preferenze progetto**.
1. Nella pagina visualizzata, continua con una delle 4 sezioni elencate di seguito per configurare le preferenze per lo stato del progetto, le timeline, i casi di business e la vita dopo la morte.

   >[!TIP]
   >
   >Se passi il cursore del mouse su una preferenza e viene visualizzato un suggerimento che informa che è bloccata, puoi chiedere all’amministratore di Workfront di sbloccarla per tutti i gruppi dell’organizzazione.

* [Stato progetto](#project-status)
* [Timeline](#timelines)
* [Casi di studio](#business-cases)
* [Vita dopo la morte](#life-after-death)

### Stato Progetto {#project-status}

Configura una delle seguenti preferenze per i progetti appena creati associati al gruppo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>Consenti agli utenti di creare progetti senza utilizzare un modello</td>
<td><p>Questa preferenza consente agli utenti di creare progetti senza utilizzare un modello durante la creazione di un progetto dalle seguenti aree:</p>
<ul>
<li><p>Utilizzare l’opzione Nuovo progetto in un elenco di progetti</p></li>

<li><p>Convertire un problema in un progetto dalla pagina del problema</p></li>
</ul>

<p>Questa preferenza è attivata per impostazione predefinita a livello di sistema.</p>
<p><b>NOTA</b></p>
<p>Quando un utente appartiene a più gruppi con preferenze diverse, gli sarà consentito creare un progetto senza un modello se almeno uno dei loro gruppi ha questa preferenza abilitata.</p>
</td></tr>
  <tr> 
   <td role="rowheader">Imposta lo stato del nuovo progetto su</td> 
   <td> <p>Determinare lo stato dei nuovi progetti.</p> <p><b>NOTA</b>   
     <ul> 
      <li>Se lo stato selezionato viene nascosto dall'utente o da un altro amministratore di Workfront, lo stato predefinito viene modificato nel primo stato dell'elenco di stato.</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">Per le preferenze di progetto di gruppo, è possibile selezionare solo uno stato bloccato o uno stato obbligatorio come stato predefinito.</li> 
      <li> <p>Se lo stato di un sistema o di un gruppo bloccato è impostato come predefinito e successivamente viene sbloccato, il sistema tenta di sostituirlo con uno stato bloccato dello stesso tipo di stato.</p> <p>Se non riesce a trovarne uno, cerca uno stato obbligatorio:</p> 
       <ul> 
        <li>Se è presente uno stato obbligatorio che equivale allo stato predefinito sbloccato, lo stato richiesto diventa lo stato predefinito, anche se è sbloccato.</li> 
        <li>Se nessuno degli stati obbligatori corrisponde allo stato predefinito sbloccato, il primo stato obbligatorio nell'elenco degli stati diventa lo stato predefinito.</li> 
       </ul> <p>Per informazioni sugli stati obbligatori, vedere gli articoli <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Accedere all'elenco degli stati dei progetti di sistema</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Accedere all'elenco degli stati delle attività di sistema</a> e <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Accedere all'elenco degli stati dei problemi di sistema</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Calcola la percentuale di completamento in base a</td> 
   <td> <p>La percentuale di completamento di un progetto o di un'attività padre si basa sull'avanzamento complessivo delle attività. Queste informazioni possono essere calcolate in base alla Durata o alle Ore pianificate delle attività di un progetto.</p> <p>Se si seleziona Durata, la Durata di ogni attività di un progetto determina la percentuale di completamento complessiva per il progetto e la Durata di ogni sottoattività determina la percentuale di completamento complessiva per l'attività padre.</p> <p>Se si seleziona Durata, assicurarsi di specificare le ore tipiche per giorno lavorativo e le giornate lavorative tipiche per settimana nella sezione Timeline. Workfront utilizza queste informazioni per calcolare la percentuale di completamento di un'attività in base alla durata. </p> <p>Se si seleziona Ore pianificate, verificare che tutte le attività di ogni progetto abbiano la quantità di Ore pianificate definita e che la quantità non sia zero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Imposta automaticamente la condizione del progetto sulla base dello stato di avanzamento</td> 
   <td> <p>Questa preferenza consente agli utenti di impostare manualmente la condizione di un progetto (On Target, At Risk, In Trouble) o far impostare automaticamente da Workfront la condizione (Stato di avanzamento) in base alla progressione del progetto nella sequenza temporale. Per ulteriori informazioni sulla condizione dei progetti, vedere <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Panoramica della condizione e del tipo di condizione del progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Crea linee di base automaticamente</p> </td> 
   <td> <p>Questa preferenza crea automaticamente una previsione (snapshot) dei dettagli di attività e progetti quando lo stato del progetto diventa Corrente. Per informazioni sulla creazione delle previsioni, vedere <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Creare le previsioni del progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Metodo indice prestazioni </p> </td> 
   <td> <p>Il metodo PIM (Performance Index Method) per il progetto controlla il metodo utilizzato da Workfront per calcolare le metriche del Valore guadagnato, quali l'Indice di prestazione dei costi (IPC) e la Stima al completamento (CES). Per ulteriori informazioni, vedere <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcolare l'indice di prestazioni dei costi (CPI)</a>e <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcolare la stima al completamento (EAC)</a></p> 
    <ul> 
     <li><strong>Basato sulle ore</strong>: Workfront utilizza le ore pianificate per calcolare metriche delle prestazioni come EAC e CPI. Quando il PIM viene calcolato in base alle ore, l'EAC viene visualizzato come numero di ore. Assicurati di disporre di un valore per Ore pianificate diverso da zero.</li> 
     <li> <p><strong>Basato sui costi</strong>: Workfront utilizza il costo della manodopera pianificata per calcolare le metriche delle prestazioni come EAC e CPI. Assicurati che le mansioni o gli utenti siano associati alle tariffe Costo orario. Quando il valore PIM viene calcolato in base ai costi, l'EAC viene visualizzato come valore di valuta.</p> <p>Il project manager può modificare questa impostazione a livello di progetto utilizzando l'area Finanza in Dettagli progetto. Per ulteriori informazioni, vedere <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gestire le informazioni nell'area Finanza progetto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Stima al completamento </p> </td> 
   <td> <p>Determinare i dati utilizzati da Workfront per calcolare la stima al completamento (CES) che rappresenta il costo totale previsto di un progetto.</p> 
    <ul> 
     <li><strong>Calcola a livello di progetto</strong>:EAC per l'attività padre e il progetto vengono determinati immettendo le ore effettive o il costo effettivo della manodopera nelle formule EAC. Questo calcolo include le ore effettive o i costi e le spese aggiunti direttamente al task o al progetto padre.</li> 
     <li> <p><strong>Rollup da attività/sottoattività</strong>: l'EAC per l'attività e il progetto padre viene determinato sommando l'EAC per ogni attività figlio. Questo calcolo esclude le ore effettive o i costi e le spese effettivi aggiunti direttamente al task o al progetto padre.</p> <p>Il project manager può modificare questa impostazione a livello di progetto utilizzando l'area Finanza in Dettagli progetto. Per ulteriori informazioni, vedere <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gestire le informazioni nell'area Finanza progetto</a>.</p> </li> 
    </ul> <p>Per ulteriori informazioni sulle modalità di calcolo di EAC, vedere <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcolare la stima al completamento (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Timeline {#timelines}

Configura una delle seguenti preferenze per i progetti appena creati associati al gruppo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pianifica da</td> 
   <td> <p>Determina se i nuovi progetti devono essere programmati dalla data di inizio o dalla data di completamento al momento della creazione.</p> 
    <ul> 
     <li><strong>Data inizio</strong>: per impostazione predefinita, le nuove attività vengono impostate sul vincolo Il più presto possibile e ai project manager viene richiesto di specificare una data inizio pianificata per il progetto.</li> 
     <li><strong>Data di completamento</strong>: per impostazione predefinita, le nuove attività vengono impostate sul vincolo Attività il più tardi possibile e ai project manager viene richiesto di specificare una data di completamento pianificata per il progetto.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Indisponibilità utente</td> 
   <td> <p>Determinare se l'indisponibilità dell'assegnatario principale di un'attività determina l'adeguamento delle date pianificate per l'attività in un progetto.</p> 
    <ul> 
     <li> <p><strong>Considerare l'indisponibilità dell'utente per le durate dell'attività</strong>: qualsiasi indisponibilità pianificata per l'assegnatario principale di un'attività regola le date pianificate dell'attività se l'indisponibilità si verifica durante la durata dell'attività. Questa è l'impostazione predefinita. </p> <p>Ad esempio, se un'attività con un vincolo Il più presto possibile è programmata per iniziare il 1° giugno e completare il 3 giugno e l'assegnatario principale ha il 2 giugno contrassegnato per l'indisponibilità, le date pianificate dell'attività vengono aggiornate dal 1° al 4 giugno.</p> <p><b>IMPORTANTE</b>: la durata dell'attività non cambia quando si seleziona questa impostazione. Solo le date pianificate cambiano, a seconda del Vincolo attività.</p> </li> 
     <li><strong>Ignora indisponibilità utente durante l'attività</strong>: le date pianificate di ogni attività in un progetto rimangono invariate rispetto a quelle pianificate in origine, anche se l'assegnatario principale di un'attività presenta un'indisponibilità durante la sua durata.</li> 
    </ul> <p>Quando selezioni le opzioni per questa impostazione, tieni presente quanto segue:</p> 
    <ul> 
     <li>Quando modifichi questa impostazione, solo i progetti e i modelli creati dopo la modifica ereditano l’impostazione aggiornata. </li> 
     <li> <p>Il valore Vincolo attività dell'attività determina le date dell'attività pianificata da adeguare: </p> 
      <ul> 
       <li>La data di inizio pianificata</li> 
       <li>La data di completamento pianificata</li> 
       <li>Entrambe le date</li> 
       <li>Nessuna data. </li> 
      </ul> <p>Ad esempio, se un'attività ha un vincolo di date fisse, le date non vengono modificate quando l'assegnatario principale presenta un'indisponibilità, anche se è selezionata l'opzione Considera indisponibilità dell'utente nella durata dell'attività. Per informazioni sui vincoli delle attività, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Panoramica sui vincoli delle attività</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Le sequenze temporali del progetto verranno ricalcolate automaticamente</strong> </p> </td> 
   <td> <p>Determina quando viene ricalcolata la timeline di un progetto. Per informazioni sul ricalcolo della sequenza temporale del progetto, vedere <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Ricalcolare le sequenze temporali del progetto</a>.</p> <p>Le seguenti opzioni sono attivate per impostazione predefinita. È possibile selezionare una o più delle seguenti impostazioni:</p> 
    <ul> 
     <li> <p><strong>Ogni notte</strong>: selezionare questa opzione per ricalcolare le sequenze temporali del progetto ogni notte. Eventuali modifiche apportate al progetto che potrebbero influenzare la timeline non sono immediatamente visibili. Workfront​​​ ricalcola le sequenze temporali di notte solo per i progetti in cui sono soddisfatte entrambe le seguenti condizioni:</p> <p> 
       <ul> 
        <li>Hanno lo stato Attuale</li> 
        <li>Hai ricevuto un aggiornamento negli ultimi 3 mesi</li> 
       </ul> </p> </li> 
     <li> <p><strong>Quando l'ambito di un progetto cambia</strong>: selezionare questa opzione per ricalcolare immediatamente le sequenze temporali del progetto quando si verifica una modifica dell'ambito del progetto. Per informazioni su cosa costituisce una modifica dell'ambito del progetto, vedere <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Ricalcolare le sequenze temporali del progetto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Quando più utenti sono assegnati a un'attività, usa la pianificazione di ...</strong> </p> </td> 
   <td> <p>Se a un progetto non è stata assegnata una pianificazione o se agli utenti assegnati alle relative attività non è stata assegnata una pianificazione, Workfront utilizza la pianificazione predefinita del sistema per calcolare la sequenza temporale delle attività.</p> <p>Se si assegnano più utenti alla stessa attività di un progetto, a cui è assegnata anche una pianificazione, Workfront utilizza le pianificazioni riportate di seguito.</p> 
    <ul> 
     <li><strong>Assegnazione principale</strong>: Workfront utilizza la pianificazione dell'assegnazione principale per calcolare le sequenze temporali.</li> 
     <li><strong>Progetto</strong>: Workfront utilizza la pianificazione del progetto per calcolare la sequenza temporale di ogni attività.</li> 
    </ul> <p>Per ulteriori informazioni sulle pianificazioni, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Creare una pianificazione</a>.</p> </td> 
  </tr> 
 <tr> 
   <td role="rowheader"> <p><span class="preview"><strong>Quando un utente è assegnato a un'attività, utilizzare la pianificazione di...</strong></span> </p> </td> 
   <td> <div class="preview"><p>Se a un progetto non è stata assegnata una pianificazione o se agli utenti assegnati alle relative attività non è stata assegnata una pianificazione, [!DNL Workfront] utilizza la pianificazione predefinita di sistema per calcolare la sequenza temporale delle attività.</p>

<p>Se si assegna un utente a un'attività di un progetto a cui è associata sia la pianificazione del progetto che quella dell'utente, in [!UICONTROL Workfront] verranno utilizzate le pianificazioni seguenti:</p> 
    <ul> 
     <li><strong>[!UICONTROL Utente]</strong>: pianificazione dell'utente assegnato all'attività per il calcolo delle timeline.</li> 
     <li><strong>[!UICONTROL Project]</strong>: pianificazione del progetto per il calcolo della sequenza temporale dell'attività.</li> 
    </ul> <p>Per ulteriori informazioni sulle pianificazioni, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Creare una pianificazione</a>.</p></div></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Calcoli timeline </p> </td> 
   <td> 
    <ul> 
     <li><strong>Ore tipiche per giorno lavorativo</strong>: imposta il numero di ore in un giorno lavorativo tipico per gli utenti che lavoreranno ai progetti. Il valore predefinito è 8 ore.</li> 
    </ul> 
    <ul> 
     <li><strong>Giorni lavorativi tipici per settimana</strong>: imposta la settimana lavorativa standard per gli utenti che lavoreranno ai progetti. Il valore predefinito è 5 giorni.</li> 
    </ul> <p>Queste 2 opzioni convertono i giorni in ore o le settimane in giorni.</p> <p>Se ad esempio si dispone di un'attività con 8 ore pianificate e la durata viene calcolata in base alle ore pianificate, Workfront converte tali ore in giorni in modo da visualizzare la Durata come giorni.</p> <p>Nel campo Giorni lavorativi tipici per settimana, Workfront calcola il valore FTE (Full Time Equivalent) per il sistema. Questo è ciò che utilizza Workfront per calcolare le allocazioni per gli utenti.</p> <p>Questi valori vengono utilizzati per la pianificazione delle sequenze temporali dei progetti, la definizione del budget per le risorse o la registrazione del tempo rispetto ai progetti. </p> <p>Non vengono utilizzati quando si stabiliscono schede orario per gli utenti nel sistema, come descritto in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Configurare le preferenze per le ore e la scheda orario</a>.</p> <p><b>NOTA</b>: gli amministratori di Workfront non possono sbloccare le preferenze Calcoli sequenza temporale.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>Trimestri personalizzati</strong> </p> </td> 
   <td> <p>Configura trimestri annuali personalizzati per gli utenti che lavoreranno ai progetti. I trimestri personalizzati sono solitamente trimestri che non corrispondono alla ripartizione tradizionale dei trimestri durante un anno di calendario. È possibile aggiungere più trimestri personalizzati. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Abilitare i trimestri personalizzati per i progetti</a>.</p> <p><b>NOTA</b>: gli amministratori di Workfront non possono sbloccare le preferenze per i trimestri personalizzati.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Casi di studio {#business-cases}

È possibile creare un Business Case per i nuovi progetti creati associati al gruppo per inviare richieste di progetto. È possibile definire le preferenze per determinare quali aree sono visibili nel modulo **Business Case**. È consigliabile attivare queste opzioni in modo che altri strumenti, ad esempio Ottimizzatore Portfolio, vengano aggiornati correttamente. Per ulteriori informazioni su ogni campo, vedere [Definire un caso di business: indice articolo](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Dopo che l’amministratore di Workfront abilita le sezioni del caso di business, un proprietario del progetto può creare un caso di business a livello di progetto. Per informazioni sulla creazione di un caso aziendale, vedere [Creare un caso aziendale per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### Vita dopo la morte  {#life-after-death}

Configura una delle seguenti preferenze per i progetti appena creati associati al gruppo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>Dopo aver contrassegnato un progetto come completato, è ancora possibile</strong> </p> </td> 
   <td> <p>Determina le regole per l'organizzazione (o il gruppo, se stai configurando le preferenze di progetto per un gruppo) relative alla possibilità di eliminare un'attività o un problema dopo che lo stato del progetto è stato contrassegnato come Completo.</p> 
    <ul> 
     <li><strong>Elimina attività</strong>: consente agli utenti di eliminare le attività da un progetto dopo che è stato contrassegnato come completato.<br></li> 
     <li><strong>Elimina problemi</strong>: consente agli utenti di eliminare i problemi da un progetto dopo che è stato contrassegnato come completato.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Dopo aver contrassegnato un progetto come Completo, Inattivo o In attesa di approvazione, è ancora possibile</strong> </p> </td> 
   <td> <p>Determina le regole per la tua organizzazione (o gruppo, se stai configurando le preferenze del progetto per un gruppo) riguardo a cosa succede ad attività, problemi, documenti e altri oggetti in un progetto dopo che lo stato del progetto è stato contrassegnato come <strong>Completo</strong>, <strong>Inattivo</strong>, o è <strong>In attesa di approvazione</strong>.</p> 
    <ul> 
     <li><strong>Aggiungi e modifica attività</strong> Consente agli utenti di: 
      <ul> 
       <li>Modifica le attività all’interno di un progetto dopo che il progetto è stato contrassegnato come Completo, Inattivo o In attesa di approvazione. Ciò include l'aggiunta di ore e la modifica delle voci di spesa per un'attività.</li> 
       <li>Aggiungere attività a un progetto.</li> 
      </ul></li> 
     <li><strong>Aggiungi e modifica problemi</strong>: consente agli utenti di: 
      <ul> 
       <li>Modifica i problemi all’interno di un progetto dopo che il progetto è stato contrassegnato come Completo, Inattivo o In attesa di approvazione.</li> 
       <li>Aggiungi problemi a un progetto dopo che questo è stato contrassegnato come Completo o Inattivo. Non è possibile aggiungere problemi a un progetto in attesa di approvazione.</li> 
      </ul></li> 
     <li> <p><strong>Aggiungi documenti al progetto e alle relative attività e problemi</strong>: consente agli utenti di aggiungere documenti a un progetto (o di aggiungere documenti alle attività e ai problemi del progetto) dopo che il progetto è stato contrassegnato come Completo o Inattivo.</p> <p>Questa opzione non si applica ai progetti in attesa di approvazione.</p> </li> 
     <li> <p><strong>Allega modelli</strong>: consente agli utenti di allegare modelli a un progetto dopo che è stato contrassegnato come Completo o Inattivo.</p> <p>Questa opzione non si applica ai progetti in attesa di approvazione.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
