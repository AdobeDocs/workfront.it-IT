---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configurare le preferenze di progetto a livello di sistema
description: In qualità di amministratore di  [!DNL Adobe Workfront] , puoi configurare le preferenze predefinite per tutti i progetti creati nel sistema. Queste preferenze influiscono sul comportamento di un progetto, di un’attività e di un problema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: 90405d79f605d788331cb7a04ebf354dc4379bf5
workflow-type: tm+mt
source-wordcount: '2693'
ht-degree: 1%

---

# Configurare le preferenze del progetto a livello di sistema

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


In qualità di amministratore [!DNL Adobe Workfront], puoi configurare le preferenze predefinite per tutti i progetti creati nel sistema. Queste preferenze influiscono sul comportamento di un progetto, di un’attività e di un problema.

>[!NOTE]
>
>Per impostazione predefinita, queste preferenze sono bloccate e gli amministratori dei gruppi non possono modificarle a livello di gruppo a meno che non vengano sbloccate per tutti i gruppi del sistema. Per ulteriori informazioni, vedere [Bloccare o sbloccare le preferenze del progetto per tutti i gruppi del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] piano</p></td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td><p>Nuovo: [!UICONTROL Standard]</p>
   Oppure
   <p>Corrente: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurare le preferenze di progetto per l’intera organizzazione

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Preferenze progetto]** > **[!UICONTROL Progetti]**.

1. Nella pagina **Preferenze progetto**, continua con una delle quattro sezioni elencate di seguito per configurare le preferenze per [!UICONTROL Stato progetto], [!UICONTROL Timeline], [!UICONTROL Casi aziendali] e [!UICONTROL Vita dopo la morte].
1. Se desideri che tutti i gruppi dell&#39;organizzazione utilizzino le stesse preferenze di progetto, accertati che ogni preferenza sia bloccata ![](assets/lock-toggle-button.png) (impostazione predefinita).

   >[!IMPORTANT]
   >
   >Quando una preferenza di progetto è bloccata, tutte le modifiche apportate a tale preferenza vengono ereditate da tutti i gruppi del sistema. È importante comunicare con gli utenti e i gruppi di tutta l’organizzazione per garantire che tutte le esigenze vengano considerate nel modo in cui configuri le preferenze del progetto.

   Per informazioni sullo sblocco di una preferenza in modo che tutti i gruppi possano configurarla e gestirla autonomamente, vedere [Bloccare o sbloccare le preferenze di progetto per tutti i gruppi del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. Fai clic su **[!UICONTROL Salva]**.

* [[!UICONTROL Stato progetto]](#project-status)
* [[!UICONTROL Timeline]](#timelines)
* [[!UICONTROL Casi di studio]](#business-cases)
* [[!UICONTROL Vita dopo la morte]](#life-after-death)

### Stato Progetto {#project-status}

Configura una delle seguenti preferenze per i progetti appena creati nel sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Consente agli utenti di creare progetti senza utilizzare un modello]</td> 
   <td>  <p>Questa preferenza consente agli utenti di creare progetti senza utilizzare un modello durante la creazione di un progetto dalle seguenti aree: </p>
      <ul>
        <li>
        <p>Utilizzare l'opzione [!UICONTROL Nuovo progetto] in un elenco di progetti</p>
        </li>
          <li>
          <p>Convertire un problema in un progetto dalla pagina del problema</p>
          </li>
         </ul>
        <p>Questa preferenza è attivata per impostazione predefinita. </p> 
        <p><b>NOTA</b></p>
        <p> Un amministratore di gruppo può modificare questa preferenza per un gruppo. Quando un utente appartiene a più gruppi con preferenze diverse, può creare un progetto senza modello se nel suo Gruppo predefinito è abilitata questa preferenza.</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Imposta lo stato del nuovo progetto su]</td> 
   <td> <p>Determinare lo stato dei nuovi progetti.</p>  <p><b>NOTA</b>  
     <ul> 
      <li>Se lo stato selezionato viene nascosto dall'utente o da un altro amministratore [!DNL Workfront], lo stato predefinito viene modificato nel primo stato dell'elenco degli stati.</li> 
     </ul> 
     <ul> 
      <li> <p>Se lo stato di un sistema o di un gruppo bloccato è impostato come predefinito e successivamente viene sbloccato, il sistema tenta di sostituirlo con uno stato bloccato dello stesso tipo di stato.</p> <p>Se non riesce a trovarne uno, cerca uno stato obbligatorio:</p> 
       <ul> 
        <li>Se è presente uno stato obbligatorio che equivale allo stato predefinito sbloccato, lo stato richiesto diventa lo stato predefinito, anche se è sbloccato.</li> 
        <li>Se nessuno degli stati obbligatori corrisponde allo stato predefinito sbloccato, il primo stato obbligatorio nell'elenco degli stati diventa lo stato predefinito.</li> 
       </ul> <p>Per informazioni sugli stati obbligatori, vedere gli articoli <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Accedere all'elenco degli stati dei progetti di sistema</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Accedere all'elenco degli stati delle attività di sistema</a> e <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Accedere all'elenco degli stati dei problemi di sistema</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calcola la percentuale di completamento in base a]</td> 
   <td> <p>Workfront calcola la percentuale di completamento di un progetto o di un'attività padre in base alla percentuale di completamento di ogni attività del progetto e alla Durata o alle Ore pianificate di ogni attività.</p><p>La percentuale di completamento di ogni attività viene impostata manualmente dagli assegnatari dell'attività.</p><p>È possibile scegliere se Workfront utilizzerà la Durata o le Ore pianificate delle attività per calcolare la percentuale di completamento dei progetti.</p> <p>Se si seleziona [!UICONTROL Durata], la Durata di ogni attività in un progetto determina la percentuale complessiva di completamento per il progetto e la Durata di ogni sottoattività determina la percentuale complessiva di completamento per l'attività padre.</p> <p>Se si seleziona [!UICONTROL Duration], assicurarsi di specificare [!UICONTROL Typical hours per work day] e [!UICONTROL Typical work days per week] nella sezione [!UICONTROL Timelines]. [!DNL Workfront] utilizza queste informazioni per calcolare la percentuale di completamento di un'attività in base alla Durata. </p> <p>Se si seleziona [!UICONTROL Lavoro Necessario], verificare che per tutte le attività di ogni progetto sia definita la quantità di [!UICONTROL Lavoro Necessario] e che la quantità non sia zero.</p><p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/manage-work/tasks/task-information/project-percent-complete.md">Panoramica sulla percentuale di completamento del progetto</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Imposta automaticamente la condizione del progetto in base allo stato di avanzamento]</td> 
   <td> <p>Questa preferenza consente agli utenti di impostare manualmente la condizione [!UICONTROL] di un progetto su ([!UICONTROL On Target], [!UICONTROL At Risk], [!UICONTROL In Trouble]) o di impostare [!DNL Workfront] la condizione [!UICONTROL Condition] (Stato di avanzamento) in base alla progressione del progetto nella sequenza temporale. Per ulteriori informazioni sulla condizione dei progetti, vedere <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Panoramica della condizione e del tipo di condizione del progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Crea automaticamente linee di base]</p> </td> 
   <td> <p>Questa preferenza crea automaticamente una previsione (snapshot) dei dettagli di attività e progetti quando lo stato del progetto diventa [!UICONTROL Current]. Per informazioni sulla creazione delle previsioni, vedere <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Creare le previsioni del progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Performance Index Method] </p> </td> 
   <td> <p>Il metodo PIM (Performance Index Method) per il progetto controlla il metodo [!DNL Workfront] utilizzato per calcolare le metriche del costo realizzato, ad esempio [!UICONTROL Cost Performance Index] (CPI) e [!UICONTROL Estimate At Completion] (EAC). Per ulteriori informazioni, vedere <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcolare [!UICONTROL Cost Performance Index] (CPI)</a> e <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calcolare la stima al completamento] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL Basato su Ore]</strong>: [!DNL Workfront] utilizza [!UICONTROL Lavoro Necessario] per calcolare le metriche delle prestazioni come EAC e CPI. Quando il PIM viene calcolato in base alle ore, l'EAC viene visualizzato come numero di ore. Assicurati di disporre di un valore per [!UICONTROL Planned Hours] diverso da zero.</li> 
     <li> <p><strong>[!UICONTROL Basato su Costo]</strong>: [!DNL Workfront] utilizza [!UICONTROL Costo manodopera pianificata] per calcolare le metriche delle prestazioni come EAC e CPI. Assicurati che le mansioni o gli utenti siano associati alle tariffe Costo orario. Quando il valore PIM viene calcolato in base ai costi, l'EAC viene visualizzato come valore di valuta.</p> <p>Il project manager può modificare questa impostazione a livello di progetto utilizzando l'area [!UICONTROL Finance] in [!UICONTROL Project Details]. Per ulteriori informazioni, vedere <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gestire le informazioni nell'area [!UICONTROL Finance] del progetto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Stima al completamento ]</p> </td> 
   <td> <p>Determinare i dati utilizzati da [!DNL Workfront] per calcolare la stima [!UICONTROL al completamento] (EAC) che rappresenta il costo totale previsto di un progetto.</p> 
    <ul> 
     <li><strong>[!UICONTROL Calcola a livello di progetto]</strong>: EAC per l'attività padre e il progetto vengono determinati immettendo [!UICONTROL Ore effettive] o [!UICONTROL Costo effettivo manodopera] nelle formule EAC. Questo calcolo include [!UICONTROL Ore effettive] o [!UICONTROL Costi e spese] aggiunti direttamente all'attività o al progetto padre.</li> 
     <li> <p><strong>[!UICONTROL Riporta da attività/sottoattività]</strong>: EAC per l'attività e il progetto padre viene determinato sommando EAC per ogni attività figlio. Questo calcolo esclude [!UICONTROL Ore effettive] o [!UICONTROL Costi e spese effettive] aggiunti direttamente all'attività o al progetto padre.</p> <p>Il project manager può modificare questa impostazione a livello di progetto utilizzando l'area [!UICONTROL Finance] in [!UICONTROL Project Details].Per ulteriori informazioni, vedere <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gestire le informazioni nell'area [!UICONTROL Finance] del progetto</a>.</p> </li> 
    </ul> <p>Per ulteriori informazioni sulle modalità di calcolo di EAC, vedere <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcolare [!UICONTROL Stima al completamento] (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Timeline {#timelines}

Configura una delle seguenti preferenze per i progetti appena creati nel sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pianifica Da]</td> 
   <td> <p>Determina se i nuovi progetti devono essere programmati dalla data di inizio o dalla data di completamento al momento della creazione.</p> 
    <ul> 
     <li><strong>[!UICONTROL Data inizio]</strong>: per impostazione predefinita le nuove attività vengono impostate sul vincolo attività [!UICONTROL Il prima possibile] e ai project manager viene richiesto di specificare una [!UICONTROL Data inizio pianificata] per il progetto.</li> 
     <li><strong>[!UICONTROL Data di completamento]</strong>: per impostazione predefinita le nuove attività vengono impostate sul vincolo attività [!UICONTROL Il più tardi possibile] e ai project manager viene richiesto di specificare una [!UICONTROL Data di completamento pianificata] per il progetto.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Indisponibilità utente]</td> 
   <td> <p>Determinare se l'indisponibilità dell'assegnatario principale di un'attività determina l'adeguamento delle date pianificate per l'attività in un progetto.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Considerare l'indisponibilità dell'utente per le durate dell'attività]</strong>: qualsiasi indisponibilità pianificata per l'assegnatario principale di un'attività regola le date pianificate dell'attività se l'indisponibilità si verifica durante la durata dell'attività. Questa è l'impostazione predefinita. </p> <p>Ad esempio, se un'attività con un vincolo di [!UICONTROL il prima possibile] è pianificata per iniziare il 1° giugno e completare il 3 giugno e l'assegnatario principale ha il 2 giugno contrassegnato per l'indisponibilità, le date pianificate dell'attività vengono aggiornate al 1° giugno fino al 4 giugno.</p> <p><b>IMPORTANTE</b>:</p> <p>La durata dell'attività non cambia quando si seleziona questa impostazione. Solo le date pianificate cambiano, a seconda del Vincolo attività.</p> </li> 
     <li><strong>[!UICONTROL Ignora indisponibilità dell'utente durante l'attività]</strong>: le date pianificate di ogni attività in un progetto rimangono invariate rispetto a quelle pianificate in origine, anche se l'assegnatario principale di un'attività presenta un'indisponibilità durante la sua durata.</li> 
    </ul> <p>Quando selezioni le opzioni per questa impostazione, tieni presente quanto segue:</p> 
    <ul> 
     <li>Quando modifichi questa impostazione, solo i progetti e i modelli creati dopo la modifica ereditano l’impostazione aggiornata. </li> 
     <li> <p>Il valore Vincolo attività dell'attività determina le date dell'attività pianificata da adeguare: </p> 
      <ul> 
       <li>La data di inizio pianificata</li> 
       <li>La data di completamento pianificata</li> 
       <li>Entrambe le date</li> 
       <li>Nessuna data. </li> 
      </ul> <p>Ad esempio, se un'attività ha un vincolo di [!UICONTROL Fixed Dates], le date non vengono modificate quando l'assegnatario principale presenta un'indisponibilità, anche se è selezionata l'opzione [!UICONTROL Considerate user off in task duration]. Per informazioni sui vincoli delle attività, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Panoramica sui vincoli delle attività</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Le sequenze temporali del progetto vengono ricalcolate automaticamente]</p> </td> 
   <td> <p>Determina quando viene ricalcolata la timeline di un progetto. Per informazioni sul ricalcolo della sequenza temporale del progetto, vedere <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Ricalcolare le sequenze temporali del progetto</a>.</p> <p>Le seguenti opzioni sono attivate per impostazione predefinita. È possibile selezionare una o più delle seguenti impostazioni:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Every Night]</strong>: selezionare questa opzione per ricalcolare le sequenze temporali del progetto ogni notte. Eventuali modifiche apportate al progetto che potrebbero influenzare la timeline non sono immediatamente visibili. [!DNL Workfront​​​] ricalcola le sequenze temporali di notte solo per i progetti in cui sono soddisfatte entrambe le seguenti condizioni:</p> <p> 
       <ul> 
        <li>Hanno lo stato [!UICONTROL Current]</li> 
        <li>Hai ricevuto un aggiornamento negli ultimi 3 mesi</li> 
        <li>Hanno avuto un tipo di aggiornamento di uno dei seguenti:</li>
        <ul>
        <li>Automatico e con Modifica</li>
        <li>Solo Modifica</li>
        <li>Solo Automatico</li> 
      </ul>       
    <b>SUGGERIMENTO:</b>
    <p>Questa impostazione non ha effetto sui progetti con il tipo di aggiornamento Solo manuale.</p>
    <li> <p><strong>Quando l'ambito di un progetto cambia</strong>: selezionare questa opzione per ricalcolare immediatamente le sequenze temporali del progetto quando si verifica una modifica dell'ambito del progetto. Per informazioni su cosa costituisce una modifica dell'ambito del progetto, vedere <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Ricalcolare le sequenze temporali del progetto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Quando a un'attività sono assegnati più utenti, utilizzare la pianificazione di]</p> </td> 
   <td> <p>Se a un progetto non è stata assegnata una pianificazione o se agli utenti assegnati alle relative attività non è stata assegnata una pianificazione, [!DNL Workfront] utilizza la pianificazione predefinita di sistema per calcolare la sequenza temporale delle attività.</p> <p>Se si assegnano più utenti alla stessa attività in un progetto a cui è assegnata una pianificazione e agli utenti assegnati alle attività è assegnata anche una pianificazione, [!UICONTROL Workfront] utilizza le pianificazioni seguenti:</p> 
    <ul> 
     <li><strong>[!UICONTROL Assegnazione primaria]</strong>: [!DNL Workfront] utilizza la pianificazione dell'Assegnazione primaria nell'attività per calcolare le sequenze temporali.</li> 
     <li><strong>[!UICONTROL Project]</strong>: [!DNL Workfront] utilizza la pianificazione del progetto per calcolare la sequenza temporale di ogni attività.</li> 
    </ul> <p>Per ulteriori informazioni sulle pianificazioni, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Creare una pianificazione</a>.</p> </td> 
  </tr>

</tr> 
  <tr> 
   <td role="rowheader"> <p>Quando un utente viene assegnato a un’attività, usa la pianificazione di...</p> </td> 
   <td> 
<p>Se a un progetto non è stata assegnata una pianificazione o se agli utenti assegnati alle relative attività non è stata assegnata una pianificazione, [!DNL Workfront] utilizza la pianificazione predefinita di sistema per calcolare la sequenza temporale delle attività.</p>

<p>Se si assegna un utente a un'attività di un progetto a cui sono associate sia il progetto che l'utente assegnato alle attività, [!UICONTROL Workfront] utilizza le pianificazioni seguenti:</p> 
    <ul> 
     <li><strong>[!UICONTROL Utente]</strong>: [!DNL Workfront] utilizza la pianificazione dell'utente assegnato nell'attività per calcolare le timeline.</li> 
     <li><strong>[!UICONTROL Project]</strong>: [!DNL Workfront] utilizza la pianificazione del progetto per calcolare la sequenza temporale dell'attività.</li> 
    </ul> <p>Per ulteriori informazioni sulle pianificazioni, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Creare una pianificazione</a>.</p>
</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Calcoli sequenza temporale] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Ore tipiche per giorno lavorativo]</strong>: imposta il numero di ore in un giorno lavorativo tipico per gli utenti che lavoreranno sui progetti. Il valore predefinito è 8 ore.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Giorni lavorativi tipici alla settimana]</strong>: imposta la settimana lavorativa standard per gli utenti che lavorano sui progetti. Il valore predefinito è 5 giorni.</li> 
    </ul> <p>Queste 2 opzioni convertono i giorni in ore o le settimane in giorni.</p> <p>Ad esempio, se un'attività ha 8 ore pianificate e la durata è calcolata in base alle ore pianificate, [!DNL Workfront] le converte in giorni in modo da visualizzare la Durata come giorni.</p> <p>Dal campo Tipico [!UICONTROL giorni lavorativi alla settimana], [!DNL Workfront] calcola il valore FTE (Full Time Equivalent) per il sistema. Questo è ciò che [!DNL Workfront] utilizza per calcolare le allocazioni per gli utenti.</p> <p>Questi valori vengono utilizzati per la pianificazione delle sequenze temporali dei progetti, la definizione del budget per le risorse o la registrazione del tempo rispetto ai progetti. </p> <p>Non vengono utilizzati quando si stabiliscono schede orario per gli utenti nel sistema, come descritto in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Configure] timesheet and hour preferences</a>.</p> <p><b>NOTA</b>:</p> <p>[!DNL Workfront] Gli amministratori non possono sbloccare le preferenze di [!UICONTROL Timeline Calculation].</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Trimestri Personalizzati]</p> </td> 
   <td> <p>Configura trimestri annuali personalizzati per gli utenti che lavoreranno ai progetti. I trimestri personalizzati sono solitamente trimestri che non corrispondono alla ripartizione tradizionale dei trimestri durante un anno di calendario. È possibile aggiungere più trimestri personalizzati. Per ulteriori informazioni, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Abilitare i trimestri personalizzati per i progetti</a>.</p>  <p><b>NOTA</b>: </p><p>[!DNL Workfront] Gli amministratori non possono sbloccare le preferenze di [!UICONTROL Trimestri personalizzati].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Casi di studio] {#business-cases}

È possibile creare un Business Case per i nuovi progetti creati in tutto il sistema per inviare richieste di progetto. È possibile definire le preferenze per determinare quali aree sono visibili nel modulo **[!UICONTROL Business Case]**. È consigliabile attivare queste opzioni in modo che altri strumenti, ad esempio [!UICONTROL Ottimizzatore Portfolio], vengano aggiornati correttamente. Per ulteriori informazioni su ogni campo, vedere [Definire un caso di business: indice articolo](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Dopo che l&#39;amministratore [!DNL Workfront] ha abilitato le sezioni nel [!UICONTROL caso di business], un proprietario del progetto può creare un caso di business a livello di progetto. Per informazioni sulla creazione di un caso aziendale, vedere [Creare un caso aziendale per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL Vita dopo la morte] {#life-after-death}

Configura una delle seguenti preferenze per i progetti appena creati nel sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dopo aver contrassegnato un progetto come Completo, è ancora possibile] </p> </td> 
   <td> <p>Determina le regole per l'organizzazione (o il gruppo, se stai configurando le preferenze di progetto per un gruppo) relative alla possibilità di eliminare un'attività o un problema dopo che lo stato del progetto è stato contrassegnato come [!UICONTROL Complete].</p> 
    <ul> 
     <li><strong>[!UICONTROL Elimina attività]</strong>: consente agli utenti di eliminare attività da un progetto dopo che è stato contrassegnato come [!UICONTROL Complete].<br></li> 
     <li><strong>[!UICONTROL Elimina problemi]</strong>: consente agli utenti di eliminare i problemi da un progetto dopo che è stato contrassegnato come [!UICONTROL Complete].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dopo aver contrassegnato un progetto come Completo, Inattivo o In attesa di approvazione, è ancora possibile]</p> </td> 
   <td> <p>Determina le regole per l'organizzazione (o il gruppo, se stai configurando le preferenze di progetto per un gruppo) per quanto riguarda ciò che accade ad attività, problemi, documenti e altri oggetti in un progetto dopo che lo stato del progetto è stato contrassegnato <strong>[!UICONTROL Complete]</strong>, <strong>[!UICONTROL Dead]</strong>, o è <strong>[!UICONTROL Pending Approval]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Aggiungi e modifica attività:]</strong> Consente agli utenti di:
      <ul>
       <li><p>Modifica le attività all'interno di un progetto dopo che è stato contrassegnato come [!UICONTROL Complete], [!UICONTROL Dead] o come [!UICONTROL Pending Approval].</p>
           <p>Nota: anche quando questa opzione non è selezionata, gli utenti possono aggiungere e modificare voci di spesa. Le ore di registrazione sono impostate separatamente. Per consentire o impedire agli utenti di registrare il tempo sui progetti con stato Complete (Completato) o Dead (Inattivo), vedere <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurare le preferenze di orario e scheda orario</a>.</p></li>
       <li>Aggiungere attività a un progetto.</li>
      </ul></li>
     <li><strong>[!UICONTROL Aggiungi e modifica problemi]</strong>: consente agli utenti di:
      <ul>
       <li>Modifica i problemi all'interno di un progetto dopo che è stato contrassegnato [!UICONTROL Complete], [!UICONTROL Dead] o [!UICONTROL Pending Approval].</li>
       <li>Aggiungi problemi a un progetto dopo che è stato contrassegnato come [!UICONTROL Complete] o [!UICONTROL Dead]. Non è possibile aggiungere problemi a un progetto [!UICONTROL Pending Approval].</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Aggiungi documenti al progetto e alle relative attività e problemi]</strong>: consente agli utenti di aggiungere documenti a un progetto (o di aggiungere documenti alle attività e ai problemi all'interno del progetto) dopo che il progetto è stato contrassegnato come [!UICONTROL Complete] o [!UICONTROL Dead].</p> <p>Questa opzione non si applica ai progetti in attesa di approvazione.</p> </li> 
     <li> <p><strong>[!UICONTROL Allega modelli]</strong>: consente agli utenti di allegare modelli a un progetto contrassegnato come [!UICONTROL Complete] o [!UICONTROL Dead].</p> <p>Questa opzione non si applica ai progetti in attesa di approvazione.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
