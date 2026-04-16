---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Crea assegnazioni avanzate
description: È possibile gestire le assegnazioni di attività o problemi utilizzando Assegnazioni avanzate.
author: Lisa
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 49f26e963647f5015955396489bfe537bbac0918
workflow-type: tm+mt
source-wordcount: '3415'
ht-degree: 1%

---

# Creare assegnazioni avanzate

<!-- Audited: 11/2025-->

<!--remove the bullet indicated when we get rid of the new/old experience of editing tasks-->


<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->

È possibile gestire le assegnazioni di attività o problemi utilizzando Assegnazioni avanzate.

È possibile modificare le seguenti informazioni di assegnazione quando si eseguono assegnazioni avanzate:

* Assegnare utenti all&#39;attività o al problema (operazione che può essere eseguita al di fuori di un&#39;assegnazione avanzata).
* Regola e ridistribuisci il numero di ore assegnate a ciascun assegnatario.
* Determina quale utente deve essere designato come proprietario o assegnatario principale dell’attività o del problema.
* Specifica il ruolo che ogni utente svolge quando lavora sull&#39;attività o sul problema.
* Aggiungere informazioni sulla fatturazione e sulla tariffa a livello di assegnazione.
* Rivedere i dettagli seguenti per ogni assegnazione: ore pianificate, costo totale e ricavi totali.

>[!NOTE]
>
>Quando si assegnano gli utenti al lavoro, la loro disponibilità in base alle loro pianificazioni influisce sulle date pianificate e previste delle attività e dei problemi. Per informazioni sulle pianificazioni, vedere [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Aree di Adobe Workfront in cui è possibile effettuare assegnazioni avanzate

Questo articolo descrive come accedere alle assegnazioni avanzate nell’intestazione dell’attività o del problema.

Inoltre, puoi effettuare assegnazioni avanzate nelle seguenti aree di Workfront:

* Negli elenchi e nei report quando il campo Assegnazioni viene visualizzato nella visualizzazione.
* Nella sezione Assegnazioni durante la modifica di un&#39;attività. Per ulteriori informazioni, vedere [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md). <!--When we remove the old/ new experience: take this bullet out completely; in the new Edit Task experience, this is no longer possible-->
* Nell’intestazione dell’attività o del problema, nell’area Assegnazioni.
* Nel Bilanciatore dei carichi di lavoro. Per ulteriori informazioni, consulta [Assegnare il lavoro manualmente utilizzando il Bilanciatore dei carichi di lavoro](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td> <p>Per aggiungere fatturazione e tassi di costo alle assegnazioni di attività e utilizzare la ricerca avanzata: Ultimate flusso di lavoro</p> <p>Per creare assegnazioni avanzate: qualsiasi pacchetto Workfront o Workflow</p></td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Work o successiva</p>
   </td> 
  </tr> 
  <tr> 
   <td role>Configurazioni del livello di accesso</td> 
   <td> <p>Modifica l'accesso ad Attività e Issues</p>  </td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td> <p>Autorizzazioni di contribuzione o di livello superiore per l’attività o il problema</p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creazione di assegnazioni avanzate - Pacchetto Workflow Ultimate

Questo layout di Assegnazioni avanzate si applica solo alle attività. Per i problemi, vedi [Crea assegnazioni avanzate - tutti gli altri pacchetti](#create-advanced-assignments--all-other-packages).

<!--

>[!NOTE]
>
>Use the experience switcher to choose between the old and new Advanced Assignments experiences. For information about the old experience, see [Create Advanced Assignments – all other packages](#create-advanced-assignments--all-other-packages), below.

-->

1. Vai al progetto a cui desideri assegnare un&#39;attività.
1. Fai clic su **Attività** o **Problemi** nel pannello a sinistra, quindi sul nome di un&#39;attività nell&#39;elenco.

   >[!TIP]
   >
   >È possibile effettuare assegnazioni avanzate direttamente nell&#39;elenco delle attività. Fai clic all&#39;interno del campo **Assegnazioni** sulla stessa riga dell&#39;attività, quindi fai clic su **Avanzate** nella parte inferiore dell&#39;elenco oppure sull&#39;icona **Persone** nell&#39;angolo superiore destro della casella Assegnazioni per aprire la finestra Assegnazioni avanzate. Passare al passaggio 5 per continuare la creazione di assegnazioni avanzate.
   >![Fare clic su Avanzate o sull&#39;icona Persone](assets/access-aa-from-lists.png)

1. Fai clic su **Assegna a** nel campo **Assegnazioni** nell&#39;intestazione dell&#39;attività

   Oppure

   Fare clic su uno dei nomi assegnati se l&#39;attività è già assegnata.

1. Fare clic su **Avanzate**.

   ![Fare clic su Avanzate](assets/assignments-from-task-header-0825.png)

   Viene visualizzata la finestra Assegnazioni avanzate.

   ![Finestra Assegnazioni avanzate](assets/advanced-assignments-031826.png)

1. Esaminare le informazioni sulla durata dell&#39;attività in base alle esigenze. Questi campi sono tutti di sola visualizzazione da Assegnazioni avanzate e puoi aggiornarli nell’attività.

   Per informazioni sulla durata dell&#39;attività, sui tipi di durata, sulle unità di tempo e sulle ore pianificate, vedere [Panoramica sulla durata dell&#39;attività e sul tipo di durata](/help/quicksilver/manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   >[!NOTE]
   >
   >Se una colonna di dati che desideri visualizzare non è visualizzata, puoi aggiungerla. Vedere [Aggiungi e rimuovi colonne nell&#39;elenco Assegnazioni avanzate](#add-and-remove-columns-on-the-advanced-assignments-list), di seguito.

1. (Facoltativo) Seleziona **Ore**, **FTE** o **Percentuale** per visualizzare le allocazioni.

   Puoi vedere quanto un utente viene assegnato nelle ore pianificate, come percentuale della sua capacità, o in FTE (equivalente a tempo pieno, scala 0-1). L&#39;impostazione predefinita è Ore.

   Per informazioni sull&#39;FTE, vedere [Configurare le preferenze di gestione delle risorse](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

1. Fai clic su **Nuova riga** per aggiungere un&#39;assegnazione all&#39;attività.

1. Fai clic nella colonna **Assegnatario** per aggiungere un utente o un team. Inizia a digitare il nome dell’utente o del team, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.

   >[!NOTE]
   >
   >Se il nome contiene un carattere speciale, è necessario includerlo nel campo di ricerca.

   Quando aggiungi un utente con una mansione principale, viene popolato il **Ruolo assegnatario**.

   Se all&#39;utente sono assegnati attributi al proprio profilo, questi vengono inseriti nell&#39;assegnazione del task.

1. Per aggiungere una mansione quando non si conosce l&#39;utente che lavorerà sull&#39;attività, fare clic nella colonna **Ruolo assegnatario**. Inizia a digitare il nome della mansione, quindi fai clic sul nome quando viene visualizzato nell’elenco a discesa.

   >[!NOTE]
   >
   >Se il nome contiene un carattere speciale, è necessario includerlo nel campo di ricerca.

   Se alla mansione sono assegnati attributi dalla scheda delle tariffe di un progetto, gli attributi vengono inseriti nell&#39;assegnazione dell&#39;attività.

   Quando si assegna un utente in un secondo momento utilizzando il campo Assegnatario, la ricerca di base segue questo algoritmo:

   * Corrispondenza completa: Ruolo e tutti gli attributi
   * Corrispondenza parziale: Ruolo e alcuni attributi
   * Solo corrispondenza ruolo

   Per informazioni sulla ricerca avanzata, vedere [Utilizzare la ricerca avanzata](#use-the-advanced-search) in questo articolo.

1. (Facoltativo) Continua ad aggiungere assegnatari nelle nuove righe per aggiungere più risorse all&#39;attività.

   >[!TIP]
   >
   >* Puoi assegnare più utenti, mansioni o team. Puoi assegnare solo utenti attivi, mansioni e team. È consentito un massimo di 200 assegnatari per attività.
   >
   >
   >* Quando aggiungi un’assegnazione utente, osserva l’avatar, il ruolo principale dell’utente o il suo indirizzo e-mail per distinguere gli utenti con nomi identici.
   >Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono aggiunti.
   >Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, vedere [Concedere l&#39;accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* Se un utente, una mansione o un team è stato assegnato prima della disattivazione, rimane assegnato all&#39;elemento di lavoro. In questo caso, consigliamo quanto segue:
   >   
   >   * Riassegnare l&#39;elemento di lavoro alle risorse attive.
   >   * Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.

1. Per contrassegnare un assegnatario come proprietario dell&#39;attività, selezionare la casella di controllo relativa alla riga e fare clic su **Imposta principale** nella barra delle azioni nella parte inferiore della finestra Assegnazioni avanzate.

   Per impostazione predefinita, Workfront contrassegna il primo utente o mansione assegnato a un&#39;attività come Proprietario o Assegnazione principale. Impossibile designare un team come proprietario principale di un&#39;attività.

   Se il proprietario principale dell&#39;attività non è visualizzato, è possibile aggiungere la colonna **Is Primary** alla tabella.

   >[!IMPORTANT]
   >
   >A seconda della modalità di impostazione delle preferenze di progetto da parte dell&#39;amministratore di Workfront o del gruppo, Workfront potrebbe utilizzare la pianificazione del proprietario dell&#39;attività per calcolare la sequenza temporale dell&#39;attività quando più utenti sono assegnati all&#39;attività. Per informazioni su più assegnatari di attività, vedere la sezione [Considerazioni per più assegnazioni a mansioni, team e utenti](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md#considerations-for-multiple-assignments-to-job-roles-teams-and-users) nell&#39;articolo [Assegnare attività](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

1. Per ogni utente nella colonna **Assegnatario**, specificare le informazioni seguenti:

   * (Facoltativo) **Ruolo per fatturazione**: cerca e seleziona la mansione per la fatturazione per questa specifica attività e assegnatario.

     Il ruolo per la fatturazione viene utilizzato solo per questa assegnazione e non viene applicato automaticamente alle altre assegnazioni dell&#39;utente. Ad esempio, il ruolo principale di un utente è Designer, ma su un’attività si comporta come Senior Designer e la tariffa di fatturazione dovrebbe rispecchiare tale funzione. Il ruolo per la fatturazione si applica solo agli utenti e non può essere utilizzato su altre mansioni.

     Quando si applica una mansione per la fatturazione all’assegnazione dell’utente, è possibile utilizzare la tariffa associata alla mansione per la fatturazione al posto delle tariffe utente o mansione nei calcoli di fatturazione e ricavi.

     È inoltre possibile impostare una mansione a livello di progetto per la fatturazione per un utente e tale valore viene utilizzato in tutte le assegnazioni dell&#39;utente per tale progetto.

     Per ulteriori informazioni, vedere [Impostare una mansione per la fatturazione](/help/quicksilver/manage-work/projects/project-finances/set-up-job-role-for-billing.md).

   * **Allocazione**: quando il tipo di durata di un&#39;attività è Semplice, specificare il numero di ore che ogni utente o mansione deve assegnare all&#39;attività. La somma di tutte le ore assegnate a ciascun utente è uguale al numero nel campo **Ore pianificate** nella parte superiore della finestra Assegnazioni avanzate. In tutti gli altri casi, specificare la percentuale di tempo (o allocazione) che l&#39;assegnatario deve dedicare alla risoluzione dell&#39;attività.

     >[!TIP]
     >
     >Dopo aver modificato manualmente le allocazioni delle assegnazioni per le attività, le ore pianificate delle attività potrebbero essere aggiornate di conseguenza. Non è possibile modificare manualmente le allocazioni per i team assegnati alle attività. Per ulteriori informazioni, consulta la sezione [Aggiornare le ore pianificate per l&#39;attività durante la gestione delle allocazioni utente](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md#update-task-planned-hours-when-managing-user-allocations) nell&#39;articolo [Panoramica sulle ore pianificate](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

   * **Attributi**: tutti gli attributi disponibili per l&#39;utente sono visualizzati nei campi degli attributi. L’amministratore imposta gli attributi che vengono aggiunti al profilo utente o associati a una mansione in una scheda tariffa. Per ulteriori informazioni, vedere [Definire gli attributi del tasso](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md) e [Modificare il profilo di un utente](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     Gli attributi sono attualmente di sola lettura nelle assegnazioni utente. Possono essere modificati per le mansioni.

   * **Valuta tasso**: la valuta per la fatturazione e le tariffe viene ricavata automaticamente dal progetto, ma è possibile modificare la valuta per questa assegnazione.

   * (Facoltativo) **Tariffa di fatturazione**: la tariffa di fatturazione può provenire da altre aree del sistema, ad esempio schede di tariffa. Per ulteriori informazioni, vedere [Panoramica sulla gerarchia dei ricavi e dei costi](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md). È possibile sostituire manualmente la tariffa di fatturazione per questa assegnazione specifica in questo campo e sostituirà tutte le altre tariffe per l&#39;utente nei calcoli dei ricavi.
   * (Facoltativo) **Tariffa di costo**: la tariffa di costo può provenire da altre aree del sistema. Per ulteriori informazioni, vedere [Panoramica sulla gerarchia dei ricavi e dei costi](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md). È possibile sostituire manualmente la tariffa per questa specifica assegnazione in questo campo e sostituirà tutte le altre tariffe per l&#39;utente nei calcoli dei costi.
   * **Fatturabile**: selezionare questa opzione per includere l&#39;assegnazione nei calcoli finanziari. Deselezionare questa opzione per escludere l&#39;assegnazione dai calcoli finanziari.

     Questo campo è attivato per impostazione predefinita per tutte le assegnazioni quando l&#39;attività ha un tipo di ricavo.

1. (Facoltativo) Per visualizzare i dati di assegnazione per data per un utente o un ruolo, selezionare la riga della tabella e fare clic su **Visualizza per date** nella barra delle azioni nella parte inferiore della finestra Assegnazioni avanzate. Per ulteriori informazioni, vedere [Visualizzare i dati di assegnazione per date](#view-assignment-data-by-dates) in questo articolo.
1. (Facoltativo) Per eliminare una o più assegnazioni dall&#39;elenco, selezionare la casella di controllo per ogni riga e fare clic su **Elimina** nella barra delle azioni nella parte inferiore della finestra Assegnazioni avanzate.
1. Fai clic su **Salva** o **Salva e chiudi** al termine della modifica delle assegnazioni avanzate.

### Aggiungere e rimuovere colonne nell&#39;elenco Assegnazioni avanzate

I campi devono esistere prima di poterli aggiungere all&#39;elenco.

1. Fai clic su **+** in alto a destra dell&#39;elenco per aprire **Gestione colonne**.

   ![Gestione colonna assegnazioni avanzate](assets/aa-column-manager.png)

1. Seleziona la scheda **Proprietà** o **KPI** per scegliere il tipo di campo da aggiungere.

   Proprietà come ubicazione o centro di costo forniscono informazioni contestuali. KPI basati sulla tempistica, ad esempio i ricavi o i valori di suddivisione dei costi tra periodi di tempo.

1. Cerca un campo oggetto esistente nella sezione **Available**, quindi fai clic su **+** a destra del nome del campo per aggiungerlo alla colonna **Selected**.
1. Fai clic su **-** a destra di un campo nella sezione **Selected** per rimuoverlo dall&#39;elenco.
1. Fai clic su **Salva**.

   Per ulteriori informazioni sul gestore colonne, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### Applicare una visualizzazione all&#39;elenco Assegnazioni avanzate

Una vista è un set personalizzato di disposizioni per le colonne che puoi applicare all’elenco.

1. Fai clic sul menu a discesa **Visualizzazioni** e seleziona la visualizzazione da applicare all&#39;elenco.

   **Le visualizzazioni di sistema** sono viste aggiunte dall&#39;amministratore di sistema e non possono essere modificate. **Le mie viste** sono viste create o condivise con te.

1. Fai clic su **Nuova visualizzazione** nel menu a discesa **Visualizzazioni** per creare una visualizzazione.

   Quando aggiungi, rimuovi o riordina le colonne, le modifiche vengono salvate automaticamente nella vista. Alla successiva applicazione di questa visualizzazione, le colonne rimangono invariate.

   Per ulteriori informazioni sulle visualizzazioni, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### Utilizzare la ricerca avanzata

La ricerca avanzata consente di individuare l&#39;utente o la mansione corretta da aggiungere all&#39;assegnazione.

1. Per aprire la finestra di ricerca avanzata, effettuare una delle seguenti operazioni:

   * Fai clic su **Ricerca avanzata** in alto a destra nella finestra Assegnazioni avanzate.
   * Selezionare una riga di assegnazione e fare clic su **Ricerca avanzata** nella barra delle azioni nella parte inferiore della finestra Assegnazioni avanzate. Verrà aperta la ricerca avanzata con i filtri applicati automaticamente per l&#39;assegnazione specifica.

1. Selezionare la scheda Utenti o Ruoli nella finestra di ricerca avanzata.
1. Applica i filtri come necessario:

   1. Fai clic su **Filtro** sopra l&#39;elenco.
   1. Nella casella Filtro fare clic su **Aggiungi condizione**.
   1. Seleziona un campo in base al quale filtrare.
   1. Seleziona un modificatore di filtro, ad esempio &quot;Ha uno di&quot;, &quot;Non ha nessuno di&quot;, &quot;È prima&quot; o &quot;È dopo&quot;. Le opzioni del modificatore variano a seconda del tipo di campo in base al quale si sta filtrando.
   1. Seleziona il valore o i valori del campo. A seconda del tipo di campo in base al quale si sta filtrando, è possibile che venga richiesto di selezionare l&#39;elemento da un elenco, cercarlo o utilizzare un calendario per selezionare un intervallo di date.

   Il filtro viene applicato automaticamente all’elenco. Per ulteriori informazioni sui filtri, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

1. Cerca un ruolo o un utente.

   Quando si cerca un utente che corrisponde a un’assegnazione di un ruolo, vengono visualizzate solo le corrispondenze complete (ruolo e tutti gli attributi).

1. Fare clic su **+** per aggiungere colonne alla tabella. Per ulteriori informazioni, vedere [Aggiungere e rimuovere colonne nell&#39;elenco Assegnazioni avanzate](#add-and-remove-columns-on-the-advanced-assignments-list).
1. Seleziona uno o più utenti o ruoli e fai clic su **Aggiungi utenti** o **Aggiungi ruoli** nella barra delle azioni nella parte inferiore della finestra.

   Le assegnazioni vengono aggiunte alla finestra Assegnazioni avanzate.

### Visualizza dati assegnazione per date

La finestra **Visualizza per date** per le assegnazioni avanzate mostra l&#39;intera cronologia delle date valide dell&#39;assegnazione per un utente o un ruolo specifico. Vengono visualizzate le modifiche passate e future.

Di seguito sono riportati alcuni esempi di elementi validi in base alla data che possono influire sulla cronologia delle assegnazioni.

* Mansione principale/altre mansioni dell&#39;utente
* Mansione a livello di progetto per la fatturazione
* Fatturazione profilo utente/tariffe di costo
* Sostituzione progetto fatturazione/tariffe di costo (utente o mansione)
* Valuta tariffe schede per ruolo/attributi
* Attributi Utente
* Pianificazione utente

Si noti che non si tratta di un elenco completo e che il campo modificato non viene necessariamente visualizzato nella tabella dei dati di assegnazione, ma influisce sulle tariffe o sugli attributi di fatturazione e costo per l&#39;utente o la mansione.

È possibile visualizzare i dati di assegnazione solo in base alle date per un singolo utente o ruolo.

1. Selezionare la riga della tabella per un utente o un ruolo e fare clic su **Visualizza per date** nella barra delle azioni nella parte inferiore della finestra Assegnazioni avanzate.

   Viene visualizzata la finestra **Visualizza per date**. Dati di sola lettura.

   Ogni riga della tabella rappresenta una modifica valida per la data dell&#39;assegnazione. Se non è stata apportata alcuna modifica valida per la data, la tabella conterrà una riga con i dati correnti. I campi evidenziati evidenziano ciò che è stato modificato e indicano la data di inizio e di fine di ciascun aggiornamento. Ad esempio, se la tariffa di fatturazione è cambiata da 202 il 20 agosto a 205 il 21 agosto, la tariffa viene evidenziata. Il testo tra parentesi indica dove è stata apportata la modifica alla tariffa, ad esempio un progetto.

   ![Finestra Visualizza per date](assets/resource-changes-view-by-dates.png)

   Dopo aver esaminato i dati, fare clic sulla freccia in alto a sinistra per tornare alla finestra Assegnazioni avanzate.

## Crea assegnazioni avanzate - tutti gli altri pacchetti

Questo layout di Assegnazioni avanzate si applica sia alle attività che ai problemi.

1. Vai al progetto a cui desideri assegnare un’attività o un problema.
1. Fai clic su **Attività** o **Problemi** nel pannello a sinistra, quindi fai clic sul nome di un&#39;attività o di un problema nell&#39;elenco.

   >[!TIP]
   >
   >Puoi effettuare assegnazioni avanzate direttamente nell’elenco delle attività o dei problemi. Fai clic all&#39;interno del campo **Assegnazioni** sulla stessa riga dell&#39;attività o del problema, quindi fai clic su **Avanzate** nella parte inferiore dell&#39;elenco oppure sull&#39;icona **Persone** nell&#39;angolo superiore destro della casella Assegnazioni per aprire la finestra Assegnazioni avanzate. Passare al passaggio 5 per continuare la creazione di assegnazioni avanzate.
   >![Fare clic su Avanzate o sull&#39;icona Persone](assets/access-aa-from-lists.png)

1. Fai clic su **Assegna a** nel campo **Assegnazioni** nell&#39;intestazione dell&#39;attività o del problema

   Oppure

   Se l’attività o il problema è già assegnato, fai clic su uno dei nomi assegnati.

1. Fare clic su **Avanzate**.

   ![Fare clic su Avanzate](assets/assignments-from-task-header-0825.png)

1. Nel campo **Cerca persone, mansione e team**, inizia a digitare il nome di un utente, una mansione o un team, quindi fai clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   >[!NOTE]
   >
   >Se il nome dell&#39;utente contiene un carattere speciale, è necessario includere tale carattere nel campo di ricerca.

1. (Facoltativo) Continua ad aggiungere assegnatari nella casella **Cerca persone, mansioni e team** per aggiungere più risorse all&#39;attività o al problema.

   >[!TIP]
   >
   >* Puoi assegnare più utenti, mansioni o team. Puoi assegnare solo utenti attivi, mansioni e team.
   >
   >
   >* Quando aggiungi un’assegnazione utente, osserva l’avatar, il ruolo principale dell’utente o il suo indirizzo e-mail per distinguere gli utenti con nomi identici.
   >Gli utenti devono essere associati ad almeno una mansione per visualizzarla quando vengono aggiunti.
   >Per consentire agli utenti di visualizzare le e-mail degli utenti, nel proprio livello di accesso deve essere abilitata l’impostazione Visualizza informazioni di contatto. Per informazioni, vedere [Concedere l&#39;accesso agli utenti](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* Se un utente, una mansione o un team è stato assegnato prima della disattivazione, rimane assegnato all&#39;elemento di lavoro. In questo caso, consigliamo quanto segue:
   >   
   >   * Riassegnare l&#39;elemento di lavoro alle risorse attive.
   >   * Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.

1. Per ogni utente nella colonna **Assegnatario**, specificare le informazioni seguenti:

   * **Proprietario**: passa il puntatore del mouse sul nome dell&#39;assegnatario e fai clic su **Imposta come principale** nel campo Proprietario se desideri contrassegnare l&#39;assegnatario come proprietario dell&#39;attività o del problema. Una casella di controllo verde indica che l’utente specificato è il contatto principale dell’attività o del problema. Adobe Workfront contrassegna come Proprietario o Assegnazione principale il primo utente o mansione assegnato a un&#39;attività o a un problema. Un team non può essere designato come proprietario principale di un’attività o di un problema.

     >[!IMPORTANT]
     >
     >A seconda della modalità di impostazione delle preferenze di progetto da parte dell&#39;amministratore di Workfront o del gruppo, Workfront potrebbe utilizzare la pianificazione del proprietario dell&#39;attività per calcolare la sequenza temporale dell&#39;attività quando più utenti sono assegnati all&#39;attività. Per informazioni su più assegnatari di attività, vedere la sezione [Considerazioni per più assegnazioni a mansioni, team e utenti](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md#considerations-for-multiple-assignments-to-job-roles-teams-and-users) nell&#39;articolo [Assegnare attività](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **Allocazioni**: quando il tipo di durata di un&#39;attività è Semplice, specificare il numero di ore che ogni utente o mansione deve assegnare all&#39;attività. La somma di tutte le ore assegnate a ciascun utente è uguale al numero nel campo **Ore pianificate** nella parte inferiore della colonna Allocazioni. In tutti gli altri casi, specifica la percentuale di tempo (o allocazione) che l’assegnatario deve dedicare alla risoluzione dell’attività o del problema.

     >[!TIP]
     >   
     >   * Dopo aver modificato manualmente le allocazioni delle assegnazioni per le attività, le ore pianificate delle attività potrebbero essere aggiornate di conseguenza. Per ulteriori informazioni, consulta la sezione [Aggiornare le ore pianificate per l&#39;attività durante la gestione delle allocazioni utente](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md#update-task-planned-hours-when-managing-user-allocations) nell&#39;articolo [Panoramica sulle ore pianificate](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).
     >   * Non è possibile modificare manualmente le allocazioni di assegnazione in caso di problemi.
     >   * Non è possibile modificare manualmente le allocazioni per i team assegnati alle attività.

   * **Ruolo dell&#39;assegnatario:** Selezionare il ruolo che l&#39;utente deve utilizzare per l&#39;esecuzione di questa assegnazione.  Il Ruolo principale dell’utente viene visualizzato per impostazione predefinita. Fai clic nella casella **Ruolo dell&#39;assegnatario** per selezionare un altro ruolo. Quando prima assegni l’attività o il problema a un ruolo e poi aggiungi un utente che può svolgere quel ruolo come seconda assegnazione, l’elenco degli utenti suggeriti viene filtrato per gli utenti che possono adempiere ai ruoli già assegnati all’attività e al problema.

     ![Ruolo dell&#39;assegnatario](assets/advanced-assignments-select-role.png)

   * **Tipo di durata**: disponibile solo per le attività. Fai clic sul nome del Tipo di durata e seleziona un Tipo di durata dal menu a discesa. Per informazioni sui tipi di durata, vedere [Panoramica sulla durata dell&#39;attività e sul tipo di durata](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **Durata:** È possibile aggiornare questo campo per un&#39;attività quando si dispone delle autorizzazioni di gestione per l&#39;attività.

     Per ulteriori informazioni, vedere [Panoramica sulla durata e sul tipo di durata dell&#39;attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). Quando si modificano in blocco le informazioni di assegnazione, viene visualizzata una finestra di dialogo simile che consente di assegnare utenti, ore, allocazione e proprietario dell&#39;attività.

   * **Ore pianificate**: quando il tipo di durata è Assegnazione calcolata o Semplice, aggiorna il numero di ore pianificate. Di conseguenza, le percentuali di allocazione o le ore per ogni risorsa vengono distribuite in modo uniforme. Workfront calcola le ore pianificate quando il tipo di durata è Lavoro calcolato o Impegno guidato. Per ulteriori informazioni, vedere [Panoramica sulla durata e sul tipo di durata dell&#39;attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. Fai clic su **Salva**.


