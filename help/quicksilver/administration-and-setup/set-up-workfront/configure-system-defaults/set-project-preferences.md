---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configurare le preferenze del progetto a livello di sistema
description: Come [!DNL Adobe Workfront] amministratore, puoi configurare le preferenze predefinite per tutti i progetti creati in tutto il sistema. Queste preferenze influiscono sul comportamento del progetto, delle attività e dei problemi.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '2475'
ht-degree: 1%

---

# Configurare le preferenze del progetto a livello di sistema

Come [!DNL Adobe Workfront] amministratore, puoi configurare le preferenze predefinite per tutti i progetti creati in tutto il sistema. Queste preferenze influiscono sul comportamento del progetto, delle attività e dei problemi.

>[!NOTE]
>
>Per impostazione predefinita, queste preferenze sono bloccate e gli amministratori dei gruppi non possono modificarle a livello di gruppo a meno che non le sbloccate per tutti i gruppi in tutto il sistema. Per ulteriori informazioni, consulta [Bloccare o sbloccare le preferenze del progetto per tutti i gruppi del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore.</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurare le preferenze di progetto per l’intera organizzazione

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Preferenze del progetto]** > **[!UICONTROL Progetti]**.

1. Nella pagina visualizzata, continua con una delle 4 sezioni elencate di seguito per configurare le preferenze per [!UICONTROL Stato del progetto], [!UICONTROL Timeline], [!UICONTROL Casi aziendali]e [!UICONTROL La vita dopo la morte].
1. Se desideri che tutti i gruppi dell&#39;organizzazione utilizzino le stesse preferenze di progetto, assicurati che ogni preferenza sia bloccata ![](assets/lock-toggle-button.png) (questa è l’impostazione predefinita).

   >[!IMPORTANT]
   >
   >Quando una preferenza di progetto è bloccata, tutte le modifiche apportate a tale preferenza vengono ereditate da tutti i gruppi del sistema. È importante comunicare con gli utenti e i gruppi in tutta l’organizzazione per garantire che tutte le esigenze siano prese in considerazione nel modo in cui configuri le preferenze del progetto.

   Per informazioni sullo sblocco di una preferenza in modo che tutti i gruppi possano configurarla e gestirla autonomamente, consulta [Bloccare o sbloccare le preferenze del progetto per tutti i gruppi del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. Fai clic su **[!UICONTROL Salva]**.

* [[!UICONTROL Stato progetto]](#project-status)
* [[!UICONTROL I Timeline]](#timelines)
* [[!UICONTROL Casi di studio]](#business-cases)
* [[!UICONTROL Vita dopo la morte]](#life-after-death)

### Stato Progetto {#project-status}

Configura una delle seguenti preferenze per i progetti appena creati in tutto il sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Consenti agli utenti di creare progetti senza utilizzare un modello]</td> 
   <td>  <p>Questa preferenza consente agli utenti di creare progetti senza utilizzare un modello quando si crea un progetto dalle aree seguenti: </p>
      <ul>
        <li>
        <p>Utilizzare l’opzione [!UICONTROL Nuovo progetto] in un elenco di progetti</p>
        </li>
          <li>
          <p>Convertire un problema in un progetto dalla pagina del problema</p>
          </li>
         </ul>
        <p>Questa preferenza è attivata per impostazione predefinita. </p> 
        <p><b>NOTA</b></p>
        <p> Un amministratore di gruppo può modificare questa preferenza per un gruppo. Se un utente appartiene a più gruppi con preferenze diverse, potrà creare un progetto senza un modello se questa preferenza è abilitata per il gruppo Home.</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Imposta lo stato del nuovo progetto su]</td> 
   <td> <p>Determinare lo stato dei nuovi progetti.</p>  <p><b>NOTA</b>  
     <ul> 
      <li>Se tu o un altro [!DNL Workfront] in questo caso lo stato predefinito viene nascosto e lo stato predefinito viene modificato nel primo stato dell'elenco di stato.</li> 
     </ul> 
     <ul> 
      <li> <p>Se lo stato predefinito di un sistema o di un gruppo bloccato è impostato come stato predefinito e successivamente un utente lo sblocca, il sistema cerca di sostituirlo con uno stato bloccato dello stesso tipo di stato.</p> <p>Se non ne trova uno, cerca uno stato obbligatorio:</p> 
       <ul> 
        <li>Se è presente uno stato obbligatorio che corrisponde allo stato predefinito sbloccato, lo stato richiesto diventa quello predefinito, anche se sbloccato.</li> 
        <li>Se nessuno degli stati richiesti corrisponde allo stato predefinito sbloccato, il primo stato richiesto nell’elenco dello stato diventa lo stato predefinito.</li> 
       </ul> <p>Per informazioni sugli stati richiesti, consulta gli articoli <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Accedere all’elenco degli stati del progetto di sistema</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Accedere all'elenco degli stati delle attività del sistema</a>e <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Accedere all’elenco degli stati dei problemi del sistema</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calcola percentuale di completamento in base a]</td> 
   <td> <p>La percentuale di completamento di un progetto o di un'attività padre si basa sull'avanzamento complessivo delle attività. Queste informazioni possono essere calcolate in base alla Durata o all'Ora pianificata delle attività di un progetto.</p> <p>Se si seleziona [!UICONTROL Duration], la Durata di ogni attività in un progetto determina la percentuale di completamento totale del progetto e la Durata di ogni sottoattività determina la percentuale di completamento totale per l'attività padre.</p> <p>Se selezioni [!UICONTROL Duration], accertati di specificare le [!UICONTROL Ore tipiche per giorno lavorativo] e [!UICONTROL Giorni lavorativi tipici della settimana] nella sezione [!UICONTROL Timeline] . [!DNL Workfront] utilizza queste informazioni per calcolare la percentuale di completamento di un'attività in base alla durata. </p> <p>Se selezioni [!UICONTROL Orari pianificati], assicurati che per tutte le attività di ciascun progetto sia definita la quantità di ore pianificate e che l’importo non sia zero.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Imposta automaticamente la condizione del progetto in base allo stato di avanzamento]</td> 
   <td> <p>Questa preferenza consente agli utenti di impostare manualmente la [!UICONTROL Condition] di un progetto ([!UICONTROL On Target], [!UICONTROL At Risk], [!UICONTROL In Trouble]) o di avere [!DNL Workfront] imposta automaticamente la [!UICONTROL Condition] (Stato di avanzamento) in base alla progressione del progetto sulla timeline. Per ulteriori informazioni sulla condizione dei progetti, consulta <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Panoramica del tipo di condizione e condizione del progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Creare automaticamente linee di base]</p> </td> 
   <td> <p>Questa preferenza crea automaticamente una baseline (snapshot) dei dettagli dell'attività e del progetto quando lo stato del progetto cambia in [!UICONTROL Current]. Per informazioni sulla creazione delle linee di base, consulta <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Creare le linee di base dei progetti</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Performance Index Method] </p> </td> 
   <td> <p>Il metodo PIM (Performance Index Method) per il progetto controlla il metodo [!DNL Workfront] utilizza per calcolare le metriche del valore generato, ad esempio [!UICONTROL Cost Performance Index] (CPI) e [!UICONTROL Estimate At Completion] (EAC). Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcola [!UICONTROL Cost Performance Index] (CPI)</a> e <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcola Stima Al Completamento (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL basato su ora]</strong>: [!DNL Workfront] utilizza [!UICONTROL Planned Hours] per calcolare le metriche delle prestazioni come EAC e CPI. Quando il PIM viene calcolato in base alle ore, l'EAC viene visualizzato come numero di ore. Assicurati di disporre di un valore per [!UICONTROL Planned Hours], diverso da zero.</li> 
     <li> <p><strong>[!UICONTROL Basato sui costi]</strong>: [!DNL Workfront] utilizza [!UICONTROL Planned Labor Cost] per calcolare le metriche delle prestazioni come EAC e CPI. Assicurati che i ruoli o gli utenti del tuo lavoro siano associati ai tassi di costo per ora. Quando il PIM viene calcolato in base ai costi, l'EAC viene visualizzato come valore di valuta.</p> <p>Il project manager può modificare questa impostazione a livello di progetto, utilizzando l’area [!UICONTROL Finance] in Dettagli progetto. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gestire le informazioni nell'area di [!UICONTROL Finance] del progetto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Stima al completamento ]</p> </td> 
   <td> <p>Determinare quali dati [!DNL Workfront] utilizza per calcolare la [!UICONTROL Estimate at Completion] (EAC) che rappresenta il costo totale previsto di un progetto.</p> 
    <ul> 
     <li><strong>[!UICONTROL Calcola a livello di progetto]</strong>:l’EAC per l’attività e il progetto padre viene determinato immettendo [!UICONTROL Ore effettive] o [!UICONTROL Costo effettivo del lavoro] nelle formule EAC. Questo calcolo include [!UICONTROL Ore effettive] o [!UICONTROL Costi e spese] aggiunti direttamente all'attività o al progetto padre.</li> 
     <li> <p><strong>[!UICONTROL Roll Up from Tasks/subTasks] (Aggregazione da attività/sottoattività)</strong>: L'EAC per l'attività e il progetto padre viene determinato sommando l'EAC per ogni attività figlio. Questo calcolo esclude [!UICONTROL Ore effettive] o [!UICONTROL Costi e spese effettivi] aggiunti direttamente all'attività o al progetto padre.</p> <p>Il project manager può modificare questa impostazione a livello di progetto, utilizzando l'area [!UICONTROL Finance] in Dettagli progetto. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gestire le informazioni nell'area di [!UICONTROL Finance] del progetto</a>.</p> </li> 
    </ul> <p>Per ulteriori informazioni su come l'EAC calcola, vedi <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcola [!UICONTROL Estimate At Completion] (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### I Timeline {#timelines}

Configura una delle seguenti preferenze per i progetti appena creati in tutto il sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pianificazione da]</td> 
   <td> <p>Determinare se i nuovi progetti sono programmati a partire dalla data di inizio o dalla data di completamento al momento della creazione.</p> 
    <ul> 
     <li><strong>[!UICONTROL Data di inizio]</strong>: Ai nuovi task predefiniti per il vincolo di attività e ai project manager viene richiesto di specificare una [!UICONTROL Data inizio pianificata] per il progetto.</li> 
     <li><strong>[!UICONTROL Data di completamento]</strong>: Ai nuovi task predefiniti del vincolo di attività e ai project manager viene richiesto di specificare una [!UICONTROL Data completamento pianificato] per il progetto.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User Time Off]</td> 
   <td> <p>Determinare se l'ora dell'assegnatario principale di un'attività regola le date pianificate per tale attività su un progetto.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Considera il tempo di inattività dell'utente nelle durate delle attività]</strong>: Qualsiasi orario non programmato per l'assegnatario principale di un'attività regola le date pianificate dell'attività se l'orario di inattività si verifica durante la sua durata. Questa è l’impostazione predefinita. </p> <p>Ad esempio, se un'attività con un vincolo di [!UICONTROL Al più presto] è pianificata per l'inizio il 1° giugno e completa il 3 giugno e l'assegnatario principale ha contrassegnato il 2 giugno per il timeout, le date pianificate dell'attività si adeguano al 1° giugno al 4 giugno.</p> <p><b>IMPORTANTE</b>: La durata dell'attività non cambia quando si seleziona questa impostazione. Cambiano solo le date pianificate, a seconda del Vincolo attività.</p> </li> 
     <li><strong>[!UICONTROL Ignora tempo utente disattivato nelle durate delle attività]</strong>: Le date pianificate di ogni attività di un progetto rimangono come originariamente pianificato, anche se l'Assegnatario principale di un'attività ha un tempo di inattività durante la sua durata.</li> 
    </ul> <p>Quando selezioni le opzioni per questa impostazione, tieni presente quanto segue:</p> 
    <ul> 
     <li>Quando modifichi questa impostazione, solo i progetti e i modelli creati dopo la modifica ereditano l’impostazione aggiornata. </li> 
     <li> <p>Il valore Vincolo attività dell'attività determina le date dell'attività pianificate da modificare: </p> 
      <ul> 
       <li>La data di inizio pianificata</li> 
       <li>La data di completamento pianificata</li> 
       <li>Entrambe le date</li> 
       <li>Nessuna data. </li> 
      </ul> <p>Ad esempio, se un'attività presenta un vincolo di [!UICONTROL Fisso Dates], le date non vengono modificate quando l'Assegnatario primario ha un tempo di inattività, anche se è selezionata l'opzione [!UICONTROL Considera il tempo di inattività dell'utente nella durata dell'attività]. Per informazioni sui vincoli delle attività, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Panoramica sul vincolo di attività</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Le timeline del progetto verranno ricalcolate automaticamente</p> </td> 
   <td> <p>Determina quando viene ricalcolata la timeline di un progetto. Per informazioni sul ricalcolo della timeline del progetto, consulta <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Ricalcolare le timeline dei progetti</a>.</p> <p>Le seguenti opzioni sono abilitate per impostazione predefinita. È possibile selezionare una o più delle seguenti impostazioni:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Ogni notte]</strong>: Seleziona questa opzione per ricalcolare le timeline del progetto ogni notte. Le modifiche apportate al progetto che potrebbero influenzare la timeline non sono immediatamente visibili. [!DNL Workfront​​​] ricalcola le tempistiche di notte solo per i progetti in cui sono soddisfatte entrambe le seguenti condizioni:</p> <p> 
       <ul> 
        <li>Hanno uno stato di [!UICONTROL Current]</li> 
        <li>Aver avuto un aggiornamento negli ultimi 3 mesi</li> 
       </ul> </p> </li> 
     <li> <p><strong>Quando l’ambito di un progetto cambia</strong>: Selezionare questa opzione per ricalcolare immediatamente le timeline del progetto in seguito alla modifica dell’ambito del progetto. Per informazioni sulla modifica dell’ambito di un progetto, consulta <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Ricalcolare le timeline dei progetti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Quando più utenti vengono assegnati a un'attività, utilizza la pianificazione di]</p> </td> 
   <td> <p>Se a un progetto non è assegnata una pianificazione o se gli utenti assegnati alle attività non dispongono di una pianificazione assegnata, [!DNL Workfront] utilizza la pianificazione predefinita del sistema per calcolare la timeline delle attività.</p> <p>Se si assegnano più utenti alla stessa attività in un progetto con una pianificazione assegnata e gli utenti assegnati alle attività dispongono anche di una pianificazione assegnata loro.[!UICONTROL Workfront] utilizza le pianificazioni seguenti:</p> 
    <ul> 
     <li><strong>[!UICONTROL Assegnazione principale]</strong>: [!DNL Workfront] utilizza la pianificazione dell'assegnazione principale nell'attività per calcolare le timeline.</li> 
     <li><strong>[!UICONTROL Project]</strong>: [!DNL Workfront] utilizza la pianificazione del progetto per calcolare la timeline di ogni attività.</li> 
    </ul> <p>Per ulteriori informazioni sulle pianificazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Creare una pianificazione</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Calcoli Timeline </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Orari tipici per giorno lavorativo]</strong>: Imposta il numero di ore in un giorno lavorativo tipico per gli utenti che lavoreranno ai progetti. Il valore predefinito è 8 ore.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Giorni lavorativi tipici della settimana]</strong>: Imposta la settimana lavorativa standard per gli utenti che lavoreranno ai progetti. Il valore predefinito è 5 giorni.</li> 
    </ul> <p>Queste 2 opzioni consentono di convertire giorni in ore o settimane in giorni.</p> <p>Ad esempio, se disponi di un’attività con 8 ore pianificate e la durata viene calcolata in base all’ora pianificata, [!DNL Workfront] converte tali ore in giorni per mostrare la Durata come giorni.</p> <p>Dal campo Tipico [!UICONTROL giorni lavorativi a settimana], [!DNL Workfront] calcola il valore FTE (Full Time Equivalent) del sistema. Questo è ciò che [!DNL Workfront] utilizza per calcolare le allocazioni per gli utenti.</p> <p>Questi valori vengono utilizzati per la pianificazione delle timeline dei progetti, per l’impostazione del budget per le risorse o per il tempo di registrazione rispetto ai progetti. </p> <p>Non vengono utilizzati quando si stabiliscono fogli presenze per gli utenti nel sistema, come descritto in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Preferenze relative alla scheda attività e all'ora</a>.</p> <p><b>NOTA</b>: [!DNL Workfront] gli amministratori non possono sbloccare le preferenze di [!UICONTROL Timeline Calculations].</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Trimestri personalizzati]</p> </td> 
   <td> <p>Configura i trimestri annuali personalizzati per gli utenti che lavoreranno ai progetti. I trimestri personalizzati sono solitamente trimestri che non corrispondono alla ripartizione tradizionale dei trimestri durante un anno civile. È possibile aggiungere più trimestri personalizzati. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Abilita trimestri personalizzati per i progetti</a>.</p>  <p><b>NOTA</b>: [!DNL Workfront] gli amministratori non possono sbloccare le preferenze di [!UICONTROL Custom Quarters].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Casi di studio] {#business-cases}

È possibile creare un Business Case per i progetti appena creati in tutto il sistema per inviare richieste di progetto. È possibile definire le preferenze per determinare quali aree sono visibili nella **[!UICONTROL Business case]** modulo. È consigliabile abilitare queste opzioni in modo che altri strumenti, come [!UICONTROL Ottimizzatore Portfolio], viene aggiornato correttamente. Per ulteriori informazioni sulla visualizzazione di ciascun campo, consulta [Definire un caso aziendale](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Dopo la [!DNL Workfront] l&#39;amministratore abilita le sezioni nel [!UICONTROL Business case], il proprietario di un progetto può quindi creare un Business Case a livello di progetto. Per informazioni sulla creazione di un Business Case, vedere [Creare un business case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL Vita dopo la morte] {#life-after-death}

Configura una delle seguenti preferenze per i progetti appena creati in tutto il sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dopo che un progetto è stato contrassegnato come Completo, le persone possono ancora] </p> </td> 
   <td> <p>Determina le regole per l'organizzazione (o il gruppo, se stai configurando le preferenze di progetto per un gruppo) relative alla possibilità di eliminare un'attività o un problema dopo che lo stato del progetto è stato contrassegnato come [!UICONTROL Complete].</p> 
    <ul> 
     <li><strong>[!UICONTROL Elimina attività]</strong>: Consente agli utenti di eliminare le attività da un progetto dopo che il progetto è stato contrassegnato come [!UICONTROL Complete].<br></li> 
     <li><strong>[!UICONTROL Elimina Problemi]</strong>: Consente agli utenti di eliminare i problemi da un progetto dopo che il progetto è stato contrassegnato come [!UICONTROL Complete].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dopo che un progetto è contrassegnato come completato, morto o in attesa di approvazione, le persone possono ancora]</p> </td> 
   <td> <p>Determinare le regole per l'organizzazione (o gruppo, se si configurano le preferenze di progetto per un gruppo) relative a operazioni, problemi, documenti e altri oggetti in un progetto dopo aver contrassegnato lo stato del progetto <strong>[!UICONTROL Completato]</strong>, <strong>[!UICONTROL Dead]</strong>oppure <strong>[!UICONTROL in attesa di approvazione]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Aggiungi e modifica attività]</strong> Consente agli utenti di:
      <ul>
       <li>Modifica le attività all’interno di un progetto dopo che il progetto è stato contrassegnato come [!UICONTROL Complete], [!UICONTROL Dead] o è in attesa di approvazione. Ciò include l'aggiunta di ore e la modifica di voci di spesa in un'attività.</li>
       <li>Aggiungi attività a un progetto.</li>
      </ul></li> 
     <li><strong>[!UICONTROL Problemi di aggiunta e modifica]</strong>: Consente agli utenti di:
      <ul>
       <li>Modifica i problemi all’interno di un progetto dopo che il progetto è stato contrassegnato come [!UICONTROL Complete], [!UICONTROL Dead] o [!UICONTROL In attesa di approvazione].</li>
       <li>Aggiungi i problemi a un progetto dopo che il progetto è stato contrassegnato come [!UICONTROL Complete] o come [!UICONTROL Dead]. (Non puoi aggiungere problemi a un progetto in attesa di approvazione).</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Aggiungi documenti al progetto e alle sue attività e problematiche]</strong>: Consente agli utenti di aggiungere documenti a un progetto (o di aggiungere documenti a attività e problemi all’interno del progetto) dopo che il progetto è stato contrassegnato come [!UICONTROL Complete] o come [!UICONTROL Dead].</p> <p>Questa opzione non si applica ai progetti in attesa di approvazione.</p> </li> 
     <li> <p><strong>[!UICONTROL Allega modelli]</strong>: Consente agli utenti di allegare modelli a un progetto dopo che il progetto è stato contrassegnato come [!UICONTROL Complete] o come [!UICONTROL Dead].</p> <p>Questa opzione non si applica ai progetti in attesa di approvazione.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
