---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configurare le preferenze di progetto a livello di sistema
description: Come un [!DNL Adobe Workfront] amministratore, puoi configurare le preferenze predefinite per tutti i progetti creati nel sistema. Queste preferenze influiscono sul comportamento di un progetto, di un’attività e di un problema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: 93a2630ec5c21f03643a29a8730046c8458c795f
workflow-type: tm+mt
source-wordcount: '2561'
ht-degree: 0%

---

# Configurare le preferenze di progetto a livello di sistema

<!--Audited: 12/2023-->

Come un [!DNL Adobe Workfront] amministratore, puoi configurare le preferenze predefinite per tutti i progetti creati nel sistema. Queste preferenze influiscono sul comportamento di un progetto, di un’attività e di un problema.

>[!NOTE]
>
>Per impostazione predefinita, queste preferenze sono bloccate e gli amministratori dei gruppi non possono modificarle a livello di gruppo a meno che non vengano sbloccate per tutti i gruppi del sistema. Per ulteriori informazioni, consulta [Blocca o sblocca le preferenze di progetto per tutti i gruppi nel sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

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
   <td> <p>[!UICONTROL Amministratore di sistema]</p> <p><b>NOTA</b>:</p><p>Se ancora non disponi dell’accesso, chiedi al tuo [!DNL Workfront] amministratore se impostano restrizioni aggiuntive nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configurare le preferenze di progetto per l’intera organizzazione

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Preferenze progetto]** > **[!UICONTROL Progetti]**.

1. Il giorno **Preferenze progetto** , continuare con una delle 4 sezioni elencate di seguito per configurare le preferenze per [!UICONTROL Stato progetto], [!UICONTROL Timeline], [!UICONTROL Casi di studio], e [!UICONTROL Vita dopo la morte].
1. Se desideri che tutti i gruppi dell’organizzazione utilizzino le stesse preferenze di progetto, accertati che ogni preferenza sia bloccata ![](assets/lock-toggle-button.png) (impostazione predefinita).

   >[!IMPORTANT]
   >
   >Quando una preferenza di progetto è bloccata, tutte le modifiche apportate a tale preferenza vengono ereditate da tutti i gruppi del sistema. È importante comunicare con gli utenti e i gruppi di tutta l’organizzazione per garantire che tutte le esigenze vengano considerate nel modo in cui configuri le preferenze del progetto.

   Per informazioni sullo sblocco di una preferenza in modo che tutti i gruppi possano configurarla e gestirla autonomamente, vedere [Blocca o sblocca le preferenze di progetto per tutti i gruppi nel sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

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
      <li>Se lei o un altro [!DNL Workfront] l'amministratore nasconde lo stato selezionato qui. lo stato predefinito passa al primo stato nell'elenco stato.</li> 
     </ul> 
     <ul> 
      <li> <p>Se lo stato di un sistema o di un gruppo bloccato è impostato come predefinito e successivamente viene sbloccato, il sistema tenta di sostituirlo con uno stato bloccato dello stesso tipo di stato.</p> <p>Se non riesce a trovarne uno, cerca uno stato obbligatorio:</p> 
       <ul> 
        <li>Se è presente uno stato obbligatorio che equivale allo stato predefinito sbloccato, lo stato richiesto diventa lo stato predefinito, anche se è sbloccato.</li> 
        <li>Se nessuno degli stati obbligatori corrisponde allo stato predefinito sbloccato, il primo stato obbligatorio nell'elenco degli stati diventa lo stato predefinito.</li> 
       </ul> <p>Per informazioni sugli stati richiesti, vedi gli articoli <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Accedere all’elenco degli stati del progetto di sistema</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Accedere all'elenco degli stati delle attività di sistema</a>, e <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Accedere all’elenco degli stati dei problemi di sistema</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calcola la percentuale di completamento in base a]</td> 
   <td> <p>Workfront calcola la percentuale di completamento di un progetto o di un'attività padre in base alla percentuale di completamento di ogni attività del progetto e alla Durata o alle Ore pianificate di ogni attività.</p><p>La percentuale di completamento di ogni attività viene impostata manualmente dagli assegnatari dell'attività.</p><p>È possibile scegliere se Workfront utilizzerà la Durata o le Ore pianificate delle attività per calcolare la percentuale di completamento dei progetti.</p> <p>Se si seleziona [!UICONTROL Durata], la Durata di ogni attività in un progetto determina la percentuale complessiva di completamento per il progetto e la Durata di ogni sottoattività determina la percentuale complessiva di completamento per l'attività padre.</p> <p>Se si seleziona [!UICONTROL Duration], assicurarsi di specificare [!UICONTROL Typical hours per work day] e [!UICONTROL Typical work days per week] nella sezione [!UICONTROL Timelines]. [!DNL Workfront] utilizza queste informazioni per calcolare la percentuale di completamento di un'attività in base alla durata. </p> <p>Se si seleziona [!UICONTROL Lavoro Necessario], verificare che per tutte le attività di ogni progetto sia definita la quantità di [!UICONTROL Lavoro Necessario] e che la quantità non sia zero.</p><p>Per ulteriori informazioni, consulta <a href="/help/quicksilver/manage-work/tasks/task-information/project-percent-complete.md">Panoramica sulla percentuale di completamento del progetto</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Imposta automaticamente la condizione del progetto in base allo stato di avanzamento]</td> 
   <td> <p>Questa preferenza consente agli utenti di impostare manualmente la condizione [!UICONTROL] di un progetto su ([!UICONTROL On Target], [!UICONTROL At Risk], [!UICONTROL In Trouble]) o su [!DNL Workfront] imposta automaticamente la condizione [!UICONTROL Condition] (Stato di avanzamento) in base alla progressione del progetto nella sequenza temporale. Per ulteriori informazioni sulle condizioni dei progetti, consulta <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Panoramica della condizione e del tipo di condizione del progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Crea automaticamente linee di base]</p> </td> 
   <td> <p>Questa preferenza crea automaticamente una previsione (snapshot) dei dettagli di attività e progetti quando lo stato del progetto diventa [!UICONTROL Current]. Per informazioni sulla creazione delle linee di base, vedere <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Crea linee di base progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Performance Index Method] </p> </td> 
   <td> <p>Il metodo PIM (Performance Index Method) per il progetto controlla il metodo [!DNL Workfront] utilizza per calcolare le metriche del Valore guadagnato, ad esempio [!UICONTROL Cost Performance Index] (CPI) e [!UICONTROL Estimate At Completion] (EAC). Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calcola [!UICONTROL Cost Performance Index] (CPI)</a> e <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calcola Stima Al Completamento] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL basato su ore]</strong>: [!DNL Workfront] utilizza [!UICONTROL Planned Hours] per calcolare le metriche delle prestazioni come EAC e CPI. Quando il PIM viene calcolato in base alle ore, l'EAC viene visualizzato come numero di ore. Assicurati di disporre di un valore per [!UICONTROL Planned Hours] diverso da zero.</li> 
     <li> <p><strong>[!UICONTROL Basato Su Costo]</strong>: [!DNL Workfront] utilizza [!UICONTROL Planned Labor Cost] per calcolare le metriche delle prestazioni come EAC e CPI. Assicurati che le mansioni o gli utenti siano associati alle tariffe Costo orario. Quando il valore PIM viene calcolato in base ai costi, l'EAC viene visualizzato come valore di valuta.</p> <p>Il project manager può modificare questa impostazione a livello di progetto utilizzando l'area [!UICONTROL Finance] in [!UICONTROL Project Details]. Per ulteriori informazioni, consulta <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gestisci informazioni nell'area [!UICONTROL Finance] del progetto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Stima al completamento ]</p> </td> 
   <td> <p>Determinare i dati [!DNL Workfront] utilizza per calcolare la [!UICONTROL Estimate at Completion] (EAC) che rappresenta il costo totale previsto di un progetto.</p> 
    <ul> 
     <li><strong>[!UICONTROL Calcola a livello di progetto]</strong>: l'EAC per l'attività e il progetto padre viene determinato immettendo [!UICONTROL Ore effettive] o [!UICONTROL Costo effettivo manodopera] nelle formule EAC. Questo calcolo include [!UICONTROL Ore effettive] o [!UICONTROL Costi e spese] aggiunti direttamente all'attività o al progetto padre.</li> 
     <li> <p><strong>[!UICONTROL Riporta da attività/sottoattività]</strong>: l’EAC per l’attività e il progetto principali viene determinato sommando l’EAC per ogni attività secondaria. Questo calcolo esclude [!UICONTROL Ore effettive] o [!UICONTROL Costi e spese effettive] aggiunti direttamente all'attività o al progetto padre.</p> <p>Il project manager può modificare questa impostazione a livello di progetto utilizzando l'area [!UICONTROL Finance] in [!UICONTROL Project Details].Per ulteriori informazioni, vedere <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Gestisci informazioni nell'area [!UICONTROL Finance] del progetto</a>.</p> </li> 
    </ul> <p>Per ulteriori informazioni sulle modalità di calcolo di EAC, vedere <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calcola [!UICONTROL Stima Al Completamento] (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### I Timeline {#timelines}

Configura una delle seguenti preferenze per i progetti appena creati nel sistema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pianifica Da]</td> 
   <td> <p>Determina se i nuovi progetti devono essere programmati dalla data di inizio o dalla data di completamento al momento della creazione.</p> 
    <ul> 
     <li><strong>[!UICONTROL Data Inizio]</strong>: per impostazione predefinita, le nuove attività vengono impostate sul vincolo [!UICONTROL As Soon Possible] e ai project manager viene richiesto di specificare una [!UICONTROL Planned Start Date] (Data di inizio pianificata) per il progetto.</li> 
     <li><strong>[!UICONTROL Data di completamento]</strong>: per impostazione predefinita, le nuove attività vengono impostate sul vincolo [!UICONTROL As Late Possible] e ai project manager viene richiesto di specificare una [!UICONTROL Planned Completion Date] per il progetto.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Indisponibilità utente]</td> 
   <td> <p>Determinare se l'indisponibilità dell'assegnatario principale di un'attività determina l'adeguamento delle date pianificate per l'attività in un progetto.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Considera l'indisponibilità dell'utente durante l'attività]</strong>: qualsiasi indisponibilità programmata per l'assegnatario principale di un'attività regola le date pianificate dell'attività se l'indisponibilità si verifica durante la durata dell'attività. Questa è l'impostazione predefinita. </p> <p>Ad esempio, se un'attività con un vincolo di [!UICONTROL il prima possibile] è pianificata per iniziare il 1° giugno e completare il 3 giugno e l'assegnatario principale ha il 2 giugno contrassegnato per l'indisponibilità, le date pianificate dell'attività vengono aggiornate al 1° giugno fino al 4 giugno.</p> <p><b>IMPORTANTE</b>:</p> <p>La durata dell'attività non cambia quando si seleziona questa impostazione. Solo le date pianificate cambiano, a seconda del Vincolo attività.</p> </li> 
     <li><strong>[!UICONTROL Ignora indisponibilità utente durante l'attività]</strong>: le date pianificate per ogni attività in un progetto rimangono invariate rispetto alla pianificazione iniziale, anche se l'assegnatario principale di un'attività presenta un'indisponibilità durante la sua durata.</li> 
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
   <td> <p>Determina quando viene ricalcolata la timeline di un progetto. Per informazioni sul ricalcolo della sequenza temporale del progetto, consultate <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Ricalcolare i timeline dei progetti</a>.</p> <p>Le seguenti opzioni sono attivate per impostazione predefinita. È possibile selezionare una o più delle seguenti impostazioni:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Ogni notte]</strong>: seleziona questa opzione per ricalcolare le timeline del progetto ogni notte. Eventuali modifiche apportate al progetto che potrebbero influenzare la timeline non sono immediatamente visibili. [!DNL Workfront​​​] ricalcola le sequenze temporali di notte solo per i progetti in cui sono soddisfatte entrambe le seguenti condizioni:</p> <p> 
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
    <li> <p><strong>Quando l’ambito di un progetto cambia</strong>: seleziona questa opzione per ricalcolare immediatamente le timeline del progetto in seguito a una modifica dell’ambito del progetto. Per informazioni su cosa costituisce una modifica dell’ambito di un progetto, consulta <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Ricalcolare i timeline dei progetti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Quando a un'attività sono assegnati più utenti, utilizzare la pianificazione di]</p> </td> 
   <td> <p>Se a un progetto non è stata assegnata una pianificazione o se agli utenti assegnati alle sue attività non è stata assegnata una pianificazione, [!DNL Workfront] utilizza la pianificazione predefinita del sistema per calcolare la sequenza temporale delle attività.</p> <p>Se si assegnano più utenti alla stessa attività in un progetto a cui è assegnata una pianificazione e agli utenti assegnati alle attività è assegnata anche una pianificazione, [!UICONTROL Workfront] utilizza le pianificazioni seguenti:</p> 
    <ul> 
     <li><strong>[!UICONTROL Assegnazione primaria]</strong>: [!DNL Workfront] utilizza la pianificazione dell'assegnazione principale per l'attività per calcolare le sequenze temporali.</li> 
     <li><strong>Progetto [!UICONTROL]</strong>: [!DNL Workfront] utilizza la pianificazione del progetto per calcolare la sequenza temporale di ciascuna attività.</li> 
    </ul> <p>Per ulteriori informazioni sulle pianificazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Creare una pianificazione</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Calcoli sequenza temporale] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Ore tipiche per giornata lavorativa]</strong>: imposta il numero di ore in una giornata di lavoro tipica per gli utenti che lavoreranno sui progetti. Il valore predefinito è 8 ore.</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL Giornate di lavoro tipiche a settimana]</strong>: imposta la settimana lavorativa standard per gli utenti che lavorano sui progetti. Il valore predefinito è 5 giorni.</li> 
    </ul> <p>Queste 2 opzioni convertono i giorni in ore o le settimane in giorni.</p> <p>Ad esempio, se un'attività ha 8 ore pianificate e la durata viene calcolata in base alle ore pianificate, [!DNL Workfront] converte tali ore in giorni in modo da visualizzare la Durata come giorni.</p> <p>Dal campo Tipico [!UICONTROL giorni lavorativi per settimana], [!DNL Workfront] calcola il valore FTE (Full Time Equivalent) del sistema. Questo è ciò che [!DNL Workfront] utilizza per calcolare le allocazioni per gli utenti.</p> <p>Questi valori vengono utilizzati per la pianificazione delle sequenze temporali dei progetti, la definizione del budget per le risorse o la registrazione del tempo rispetto ai progetti. </p> <p>Non vengono utilizzati quando si stabiliscono schede orario per gli utenti nel sistema, come descritto in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Preferenze orario e scheda orario di [!UICONTROL Configure]</a>.</p> <p><b>NOTA</b>:</p> <p>[!DNL Workfront] Gli amministratori non possono sbloccare le preferenze di [!UICONTROL Timeline Calculation].</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Trimestri Personalizzati]</p> </td> 
   <td> <p>Configura trimestri annuali personalizzati per gli utenti che lavoreranno ai progetti. I trimestri personalizzati sono solitamente trimestri che non corrispondono alla ripartizione tradizionale dei trimestri durante un anno di calendario. È possibile aggiungere più trimestri personalizzati. Per ulteriori informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Abilita trimestri personalizzati per i progetti</a>.</p>  <p><b>NOTA</b>: </p><p>[!DNL Workfront] Gli amministratori non possono sbloccare le preferenze di [!UICONTROL Trimestri personalizzati].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Casi di studio] {#business-cases}

È possibile creare un Business Case per i nuovi progetti creati in tutto il sistema per inviare richieste di progetto. È possibile definire le preferenze per determinare quali aree sono visibili sul **[!UICONTROL Business Case]** modulo. È consigliabile attivare queste opzioni in modo che altri strumenti, come [!UICONTROL Ottimizzatore Portfolio], aggiorna correttamente. Per ulteriori informazioni sulla visualizzazione di ogni campo, consulta [Definire un caso di business: indice articolo](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Dopo il [!DNL Workfront] l&#39;amministratore abilita le sezioni nel [!UICONTROL Business Case], un Proprietario del progetto può quindi creare un Business Case a livello di progetto. Per informazioni sulla creazione di un caso di business, vedere [Creare un Business Case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

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
     <li><strong>[!UICONTROL Elimina attività]</strong>: consente agli utenti di eliminare le attività da un progetto dopo che questo è stato contrassegnato come [!UICONTROL Complete].<br></li> 
     <li><strong>[!UICONTROL Elimina problemi]</strong>: consente agli utenti di eliminare i problemi da un progetto dopo che questo è stato contrassegnato come [!UICONTROL Complete].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dopo aver contrassegnato un progetto come Completo, Inattivo o In attesa di approvazione, è ancora possibile]</p> </td> 
   <td> <p>Determina le regole per l'organizzazione (o il gruppo, se stai configurando le preferenze di progetto per un gruppo) relative a cosa succede ad attività, problemi, documenti e altri oggetti in un progetto dopo che lo stato del progetto è stato contrassegnato <strong>[!UICONTROL Complete]</strong>, <strong>[!UICONTROL Dead]</strong>, o è <strong>[!UICONTROL In Attesa Di Approvazione]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL Aggiungi e modifica attività]</strong> Consente agli utenti di:
      <ul>
       <li>Modifica le attività all'interno di un progetto dopo che è stato contrassegnato come [!UICONTROL Complete], [!UICONTROL Dead] o come [!UICONTROL Pending Approval]. Ciò include l'aggiunta di ore e la modifica delle voci di spesa per un'attività.</li>
       <li>Aggiungere attività a un progetto.</li>
      </ul></li> 
     <li><strong>[!UICONTROL Aggiungi e modifica problemi]</strong>: consente agli utenti di:
      <ul>
       <li>Modifica i problemi all'interno di un progetto dopo che è stato contrassegnato [!UICONTROL Complete], [!UICONTROL Dead] o [!UICONTROL Pending Approval].</li>
       <li>Aggiungi problemi a un progetto dopo che è stato contrassegnato come [!UICONTROL Complete] o [!UICONTROL Dead]. Non è possibile aggiungere problemi a un progetto [!UICONTROL Pending Approval].</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Aggiungi documenti al progetto e alle relative attività e problemi]</strong>: consente agli utenti di aggiungere documenti a un progetto (o di aggiungere documenti alle attività e ai problemi all’interno del progetto) dopo che il progetto è stato contrassegnato come [!UICONTROL Complete] o [!UICONTROL Dead].</p> <p>Questa opzione non si applica ai progetti in attesa di approvazione.</p> </li> 
     <li> <p><strong>[!UICONTROL Allega modelli]</strong>: consente agli utenti di allegare modelli a un progetto contrassegnato come [!UICONTROL Complete] o [!UICONTROL Dead].</p> <p>Questa opzione non si applica ai progetti in attesa di approvazione.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
