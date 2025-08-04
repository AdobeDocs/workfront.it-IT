---
product-area: templates
keywords: attività,valori predefiniti,automatizza,creazione
navigation-topic: templates-navigation-topic
title: Modificare un’attività modello
description: Dopo aver creato un modello, è possibile modificare le informazioni sulle attività del modello. Le informazioni aggiornate in un'attività modello vengono associate alle attività del progetto dopo che è stato utilizzato il modello per creare un progetto o dopo che il modello è stato allegato a un progetto.
author: Alina
feature: Work Management
exl-id: 2df8522e-7eee-4440-be0f-f7483c5acdb0
source-git-commit: a92c85ad5f58700138d7750423cc3d134d980a9e
workflow-type: tm+mt
source-wordcount: '2493'
ht-degree: 4%

---

# Modificare un’attività modello

<!--Audited: 09/2024-->

Dopo aver creato un modello, è possibile modificare le informazioni relative alle attività del modello. Le informazioni aggiornate in un&#39;attività modello vengono associate alle attività del progetto dopo che è stato utilizzato il modello per creare un progetto o dopo che il modello è stato allegato a un progetto.

Per informazioni sulla creazione di un modello, vedere [Creare un modello di progetto](../../../manage-work/projects/create-and-manage-templates/create-template.md).

È possibile modificare l&#39;attività modello oppure modificare le attività modello in blocco.

>[!NOTE]
>
>Non è possibile modificare in blocco le attività modello che appartengono a modelli diversi. È possibile modificare solo le attività modello che appartengono allo stesso modello.


## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Standard </p>
   <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso</td> 
   <td> <p>Modificare l’accesso ai modelli</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto </td> 
   <td> <p>Consente di gestire le autorizzazioni per un modello. </p> <p>Autorizzazioni di Contribute o superiori per l'attività modello.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Prima di iniziare, è necessario

* Crea un modello.

  Per informazioni sulla creazione di un modello, vedere [Creare un modello di progetto](../../../manage-work/projects/create-and-manage-templates/create-template.md).

## Modifica attività modello

È possibile modificare un&#39;attività modello utilizzando le aree Modifica attività modello o Dettagli attività modello. Nei passaggi seguenti viene descritta la modifica di un&#39;attività nella casella Modifica attività modello.

{{step1-to-templates}}

1. Fare clic sul nome di un modello per aprirlo.
1. Fai clic su **Attività modello** nel pannello a sinistra.
1. Fare clic sul nome di un&#39;attività modello nell&#39;elenco per aprirla.
1. (Facoltativo) Fai clic sulla sezione **Predecessori** nel pannello a sinistra per aggiungere predecessori per le attività modello. L’aggiunta di predecessori di attività modello è simile all’aggiunta di predecessori di attività progetto. Per informazioni, vedere [Creare una relazione predecessore utilizzando l&#39;area Predecessori](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
1. (Facoltativo) Fai clic sulla sezione **Sottoattività** nel pannello a sinistra per aggiungere elementi secondari per l&#39;attività modello. L&#39;aggiunta di sottoattività per le attività modello è simile all&#39;aggiunta di sottoattività per le attività del progetto. Per informazioni, vedere la sezione &quot;Creare sottoattività dalla sezione Attività secondarie&quot; nell&#39;articolo [Creare sottoattività](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).

1. (Condizionale) Per modificare informazioni limitate su un&#39;attività modello, fai clic su **Dettagli attività modello** nel pannello a sinistra, quindi vai alle aree della sezione Dettagli per modificare le informazioni per ogni area.
1. (Facoltativo) Fai clic sull&#39;icona **Comprimi tutto** ![Comprimi tutto](assets/collapse-all-icon.png) per comprimere tutte le aree.
1. Per modificare le informazioni nella sezione Dettagli, fai clic sull&#39;icona **Modifica** ![Modifica icona](assets/edit-icon.png), quindi seleziona una delle aree seguenti oppure fai clic su **Modifica tutto** per modificare le informazioni in tutte le aree:

   * Panoramica
   * Moduli personalizzati

     I nomi dei moduli doganali vengono visualizzati solo se all’oggetto sono allegati moduli personalizzati.

   * Finanz

   >[!TIP]
   >
   >Per informazioni su tutti i campi visualizzati nell&#39;area Dettagli, continuare a modificare tutti i campi utilizzando la casella Modifica attività modello, come descritto di seguito.
1. (Facoltativo) Per modificare più attività modello in blocco, seleziona più attività modello, quindi fai clic su **Modifica** nella parte superiore dell&#39;elenco dei modelli.
1. (Condizionale) Per modificare tutte le informazioni sull&#39;attività modello o su più attività contemporaneamente, fai clic su per selezionarle da un elenco, quindi fai clic sull&#39;icona **Modifica** ![Icona Modifica](assets/edit-icon.png) nella parte superiore dell&#39;elenco.

   Viene visualizzata la casella **Modifica attività modello**.

   >[!TIP]
   >
   >È inoltre possibile selezionare un&#39;attività modello in un elenco, quindi fare clic su Modifica per aprire la casella Modifica attività modello.

   ![Modifica attività modello](assets/edit-template-tasks-box-classic-350x356.png)

1. Prendere in considerazione la possibilità di specificare informazioni in una delle sezioni seguenti:

   * [Panoramica](#overview)
   * [Finanz](#finance)
   * [Impostazioni](#settings)
   * [Assegnazioni](#assignments)
   * [Moduli personalizzati](#custom-forms)
   * [Commento](#comment)

### Panoramica {#overview}

1. Inizia a modificare un’attività modello come descritto in precedenza.
1. Fare clic su **Panoramica**.

   ![modifica_attività_panoramica.png](assets/edit-task-overview-350x438.png)

1. Aggiorna uno dei seguenti elementi:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nome</strong> </td> 
      <td>Specificare un nome per l'attività modello. Questo campo non viene visualizzato quando si modificano in blocco attività modello.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descrizione</strong> </td> 
      <td>Aggiungere ulteriori informazioni sull'attività modello.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>Specificare un collegamento Web relativo alle informazioni sull'attività modello.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorità</strong> </td> 
      <td> <p>Questo è un flag visivo che ti consente di assegnare una priorità alle attività del modello. </p> <p>Selezionare una delle opzioni seguenti:</p> 
       <ul> 
        <li> <p><strong>Nessuno</strong> </p> </li> 
        <li> <p><strong>Basso</strong> </p> </li> 
        <li> <p> <b>Normale</b></p> </li> 
        <li> <p><b>Alta</b> </p> </li> 
        <li> <p><b>Urgente</b> </p> </li> 
       </ul> <p>A seconda delle Preferenze di progetto selezionate dall'amministratore di Workfront, i nomi delle priorità potrebbero essere diversi. Per ulteriori informazioni sulla modifica delle priorità, vedere <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Creare e personalizzare le priorità</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tipo di Durata</strong> </td> 
      <td> <p>L'attività futura creata da questo modello avrà questo Tipo di Durata. <br>Il tipo di durata identifica la relazione tra:</p> <p>- numero di risorse assegnate a un'attività</p> <p>- lo sforzo totale richiesto per completare l'attività</p> <p>- la durata totale dell'attività. </p> <p>I tipi di durata consentono di impostare assegnazioni di risorse coerenti in base alle esigenze dell'attività. Per ulteriori informazioni sul tipo di durata di un'attività, vedere <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica sulla durata e sul tipo di durata dell'attività</a>.</p> <p>Selezionare una delle opzioni seguenti:</p> 
       <ul> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Assegnazione calcolata</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Lavoro Calcolato</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Basato Sulle Risorse</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Semplice</span> <br> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Durata</strong> </td> 
      <td> <p>Specificare la Durata delle attività future in minuti, ore, giorni, settimane o mesi. La durata dell'attività futura creata da questo modello sarà specificata qui.</p> <p>Per impostazione predefinita, Workfront misura la durata in giorni. Questo è il tempo che si consente all'attività di rimanere incompleta, prima che debba essere completata. Impossibile specificare la durata di un'attività quando il <strong>Tipo di durata</strong> dell'attività è <strong>Semplice</strong> o quando il <strong>Vincolo attività</strong> è <strong>Date fisse</strong>.</p> <p><b>IMPORTANTE</b></p> <p>La durata è in genere il tempo che intercorre tra l'inizio pianificato e le date di completamento pianificate di un'attività modello e, per questo motivo, influisce sulla sequenza temporale del modello. Questo determina la timeline del progetto futuro creato dal modello. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ore pianificate</strong> </td> 
      <td> <p>Specifica il numero di ore pianificate per l'attività futura nel progetto creato con questo modello. Quantità di tempo effettivo necessario agli assegnatari per completare l'attività. È possibile specificare solo il numero di ore pianificate per un'attività quando <strong>Tipo di durata</strong> è impostato su <strong>Assegnazione calcolata</strong>. </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Vincolo attività</strong> </td> 
      <td> <p>Questo vincolo si applica all’attività sul progetto creata da questo modello. I vincoli task identificano quando un task deve essere completato. </p> <p>Selezionare una delle opzioni seguenti:</p> 
       <ul> 
        <li><strong>Date fisse</strong>. Specifica un <strong>Inizio pianificato</strong> e una <strong>Data di completamento pianificata.</strong></li> 
        <li><strong>Deve Iniziare Il</strong>. Specifica una <strong>data di inizio pianificata.</strong></li> 
        <li><strong>Deve Terminare Il</strong>. Specifica una <strong>data di completamento pianificata</strong>.</li> 
        <li><strong>Più presto possibile</strong> </li> 
        <li><strong>Più tardi possibile</strong> </li> 
        <li style="font-weight: bold;"><strong>Primo Orario Disponibile</strong> </li> 
        <li style="font-weight: bold;"><strong>Ultimo Orario Disponibile</strong> </li> 
        <li>Inizia Non Più Tardi Di. Specifica una <strong>data inizio pianificata</strong>.</li> 
        <li><strong>Iniziare Non Prima Di</strong>. Specifica una <strong>data inizio pianificata</strong>.</li> 
        <li><strong>Fine Non Oltre Il</strong>. Specifica una <strong>data di completamento pianificata</strong>.</li> 
        <li><strong>Fine Non Prima Di</strong>. Specifica una <strong>data di completamento pianificata</strong>.</li> 
       </ul> <p>Per ulteriori informazioni sul vincolo attività, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sul vincolo attività</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">Giorno d'inizio</span><span style="font-weight: normal;"> (facoltativo e condizionale)</span> </td> 
      <td> <p> È possibile specificare il giorno di inizio di un'attività modello solo quando il vincolo attività è uno dei seguenti:</p> 
       <ul> 
        <li>Deve ininziare al</li> 
        <li>Iniziare non Prima di</li> 
        <li>Iniziare non Dopo di</li> 
        <li>Dati Fissi</li> 
       </ul> <p>Corrisponde alla data di inizio dell'attività nella sequenza temporale del progetto futuro. Per tutti gli altri vincoli, Workfront calcola il giorno di inizio in base alla dipendenza del predecessore tra le attività. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Giorno di completamento</strong><span style="font-weight: normal;"> (facoltativo e condizionale)</span> </td> 
      <td> <p> È possibile specificare il giorno di completamento di un'attività modello solo quando il vincolo attività è uno dei seguenti:</p> 
       <ul style="list-style-type: circle;"> 
        <li>Deve essere completato il</li> 
        <li>Completa non prima di</li> 
        <li>Completa entro e non oltre</li> 
        <li>Dati Fissi</li> 
       </ul> <p>Corrisponde alla data di completamento dell'attività nella sequenza temporale del progetto futuro. Per tutti gli altri vincoli, Workfront calcola il giorno di completamento in base alla durata e alla dipendenza predecessore. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Continua a modificare le sezioni seguenti, a seconda delle informazioni che desideri modificare.

   Oppure

   Fai clic su **Salva modifiche**.

### Finanz {#finance}

1. Inizia a modificare un’attività modello come descritto in precedenza.
1. Fare clic su **Finanza**.

   ![modifica_attività_finanza.png](assets/edit-task-finance-350x216.png)

1. Aggiorna uno dei seguenti elementi:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Tipo di costo</strong> </td> 
      <td> <p>Specificare il tipo di costo per l'attività futura. Questo determinerà il modo in cui viene calcolato il costo dell'attività, in base al numero di ore delle attività. </p> <p>Selezionare una delle opzioni seguenti:</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>Nessun costo</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Ore Fisse</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Ore Utente</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Ore Ruolo</span> </p> </li> 
       </ul> <p>Per ulteriori informazioni sul tracciamento dei costi, vedere <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tracciare i costi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tipo di Reddito</strong> </td> 
      <td> <p>Specificare il tipo di retribuzione per l'attività futura. Questo determinerà il modo in cui vengono calcolati i Ricavi sull'attività, in base al numero di ore sulle attività.</p> <p style="font-weight: normal;">Selezionare una delle opzioni seguenti: </p> 
       <ul> 
        <li> <p style="font-weight: normal;">Non Fatturabile</p> </li> 
        <li> <p style="font-weight: normal;">Ore Utente</p> </li> 
        <li> <p style="font-weight: normal;">Ore Ruolo</p> </li> 
        <li> <p style="font-weight: normal;">Ore Fisse</p> </li> 
        <li> <p style="font-weight: normal;">Ore utente con limite</p> </li> 
        <li> <p style="font-weight: normal;">Ore ruolo con limite</p> </li> 
        <li> <p style="font-weight: normal;">Ore Utente più Fisso</p> </li> 
        <li> <p style="font-weight: normal;">Ore Ruolo più Fisso</p> </li> 
        <li> <p style="font-weight: normal;">Reddito Fisso</p> </li> 
       </ul> <p>Per ulteriori informazioni sul tracciamento dei ricavi, vedere <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica su fatturazione e ricavi</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Continua a modificare le sezioni seguenti, a seconda delle informazioni che desideri modificare.

   Oppure

   Fai clic su **Salva modifiche**.

### Impostazioni {#settings}

1. Inizia a modificare un’attività modello come descritto in precedenza.
1. Fare clic su **Impostazioni**.

   ![Modifica impostazioni attività modello](assets/edit-template-tasks-settings-classic-350x231.png)

1. Aggiorna uno dei seguenti elementi:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Milestone</b></p></strong> </td> 
      <td> <p>Scegliere un'attività cardine da associare all'attività modello selezionata.</p>

   <p><b>IMPORTANTE</b></p>
   <p>È necessario associare un percorso milestone a un modello per visualizzare questo campo. Per ulteriori informazioni, vedere <a href="../create-and-manage-templates/edit-templates.md">Modifica modelli di progetto</a>.</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>Modalità di tracciamento</strong> </td> 
      <td> <p>Specificare come verrà tracciato lo stato di avanzamento dell'attività futura. </p> <p>Selezionare una delle opzioni seguenti:</p> 
       <ul> 
        <li> <p><strong>L'Utente Deve Aggiornare</strong> </p> </li> 
        <li> <p><strong>Presupponi alle ore</strong> </p> </li> 
        <li> <p><strong>Ignora avvisi di ritardo</strong> </p> </li> 
        <li> <p><strong>Completamento automatico</strong> </p> </li> 
        <li> <p><strong>Predecessore</strong> </p> </li> 
       </ul> <p>Per ulteriori informazioni sulla modalità di verifica delle attività, vedere <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Panoramica sulla modalità di verifica delle attività</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Processo di approvazione</strong> </td> 
      <td> <p>Selezionare il processo di approvazione da associare all'attività modello. Prima di poter essere associati alle attività modello, l'amministratore di Workfront deve definire i processi di approvazione delle attività a livello di sistema. <span>Un utente con accesso amministrativo ai processi di approvazione può inoltre creare processi di approvazione specifici per il gruppo.</span> Per ulteriori informazioni sulla creazione dei processi di approvazione, vedere <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Creare un processo di approvazione per gli elementi di lavoro</a>.</p> <p>Quando aggiungi processi di approvazione, tieni presente quanto segue: </p> 
       <ul> 
       <li>Nell'elenco vengono visualizzati solo i processi di approvazione attivi. </li> 
       <li> <p>I processi di approvazione a livello di sistema e di gruppo vengono visualizzati nell’elenco. I processi di approvazione associati a un gruppo diverso da quello del modello non vengono visualizzati nell’elenco.</p> <p>Importante: se il gruppo associato al modello cambia, il processo di approvazione specifico del gruppo diventa un processo di approvazione a utente singolo. Per ulteriori informazioni su come le modifiche al gruppo del progetto o le modifiche al processo di approvazione influiscono sulle impostazioni di approvazione, vedere <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Come le modifiche al gruppo e al processo di approvazione influiscono sui processi di approvazione assegnati</a>. </p> </li> 
       <li> <p>Se hai aggiunto un processo di approvazione a utente singolo, in questo campo viene visualizzato come "&lt;Personalizzato&gt;". Per informazioni, vedere <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associa un processo di approvazione nuovo o esistente a un lavoro</a>. </p> <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will be valid only for Classic when they edit the Edit Template box in NWE)</p>--> </li> 
       <li> <p>Quando si modificano in blocco le attività modello, si verificano i seguenti scenari:</p> 
       <ul> 
       <li> <p>Quando si selezionano le attività modello dallo stesso gruppo di modelli, in questo campo vengono visualizzati sia i processi di approvazione a livello di sistema che quelli a livello di gruppo.</p> </li> 
       <li> <p>Quando si selezionano le attività modello da diversi gruppi di modelli, in questo campo vengono visualizzati solo i processi di approvazione a livello di sistema.</p> </li> 
       <li> <p>Quando a una delle attività modello è associato un processo di approvazione a utente singolo, questo viene sostituito dal processo di approvazione a livello di sistema <span>o di gruppo</span> selezionato. </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Avvisi di Promemoria</strong> </td> 
      <td> <p>Selezionare gli Avvisi di Promemoria da allegare all'attività modello. Saranno allegati alle attività future del progetto creato da questo modello. L'amministratore di sistema deve configurare gli Avvisi di Promemoria prima che sia possibile selezionarli in un'attività. Per ulteriori informazioni sulla configurazione delle notifiche di promemoria, vedere <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configurare le notifiche di promemoria</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Continua a modificare le sezioni seguenti, a seconda delle informazioni che desideri modificare.

   Oppure

   Fai clic su **Salva modifiche**.

### Assegnazioni {#assignments}

1. Inizia a modificare un’attività modello come descritto in precedenza.
1. Fai clic su **Assegnazioni**.

   ![assegnazioni_modifica_attività.png](assets/assignments-edit-tasks-350x87.png)

1. Fai clic su **Aggiungi assegnatario** per aggiungere un nuovo assegnatario all&#39;attività modello. È possibile assegnare utenti, ruoli o team a un&#39;attività. È possibile avere più assegnatari per un&#39;attività. Alle attività future verranno assegnate le stesse risorse quando verranno create da questa attività modello.
1. (Facoltativo) Se hai più assegnatari, seleziona il pulsante di opzione **Proprietario** per indicare quale utente o ruolo è considerato il Proprietario dell&#39;attività o l&#39;assegnatario principale. Workfront contrassegna il primo utente o ruolo assegnato a un&#39;attività modello come Proprietario o Assegnatario principale.
1. (Condizionale e facoltativo) Se il vincolo dell&#39;attività è Lavoro calcolato o Impegno, specifica **Allocazione %** (percentuale di allocazione) per ogni assegnatario. Quantità di tempo della pianificazione dell&#39;assegnatario che può trascorrere per l&#39;attività. Se si modifica la percentuale di allocazione per un assegnatario, verranno modificate le ore pianificate di un&#39;attività.
1. (Condizionale e facoltativo) Se il vincolo attività è Semplice, specifica le **Ore** di ciascun assegnatario

   Oppure

   Specifica il numero totale di **ore pianificate** per l&#39;attività modello. In questo modo le ore totali vengono distribuite equamente tra tutti gli assegnatari.

1. (Condizionale e facoltativo) Se il vincolo attività è Semplice, specifica la **Durata** dell&#39;attività modello in giorni. Questa diventerà la durata dell&#39;attività creata da questo modello.
1. (Facoltativo) Seleziona un ruolo dal menu a discesa **Ruolo dell&#39;assegnatario**. Questo è il ruolo che l’assegnatario può svolgere per questa attività futura. Nel menu a discesa vengono visualizzati solo i ruoli associati a ciascun assegnatario nel relativo profilo.
1. (Facoltativo) Continua a modificare le sezioni seguenti, a seconda delle informazioni che desideri modificare.

   Oppure

   Fai clic su **Salva modifiche**.

### Moduli personalizzati {#custom-forms}

È possibile definire moduli personalizzati da allegare automaticamente per impostazione predefinita alle attività quando queste vengono aggiunte a un progetto. Per informazioni sulla configurazione del progetto per includere moduli personalizzati per attività predefiniti, vedere la sezione &quot;Attività&quot; nell&#39;articolo [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

È inoltre possibile aggiungere moduli personalizzati alle attività future di un progetto quando il progetto viene creato da un modello, aggiungendo i moduli personalizzati alle attività del modello.

1. Inizia a modificare un’attività modello come descritto in precedenza.
1. Fare clic su **Forms personalizzato**.

   ![custom_forms_edit_task.png](assets/custom-forms-edit-task-350x136.png)

1. Selezionare il modulo o i moduli personalizzati che si desidera associare all&#39;attività modello.

   Devi creare i moduli personalizzati prima che siano disponibili per la selezione in questo campo.
Nell’elenco vengono visualizzati solo i moduli personalizzati attivi.
Per ulteriori informazioni sulla creazione di moduli personalizzati, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
È possibile aggiungere fino a dieci moduli personalizzati a un&#39;attività modello.
I moduli vengono aggiunti automaticamente alle attività create dal modello.
1. (Condizionale e facoltativo) Se si è allegato un modulo personalizzato all&#39;attività modello, modificare tutti i campi del modulo. È necessario specificare tutti i campi obbligatori prima di salvare l&#39;attività modello.

   >[!NOTE]
   >
   >A seconda di come l’amministratore di Workfront imposta le autorizzazioni per le sezioni nel modulo personalizzato, non tutti possono visualizzare o modificare gli stessi campi in un determinato modulo personalizzato. Le autorizzazioni per modificare i campi all’interno di una sezione di un modulo personalizzato dipendono dalle autorizzazioni di cui disponi per l’attività modello o per l’attività futura.\
   >Per informazioni sull&#39;impostazione delle autorizzazioni per le sezioni di un modulo personalizzato, vedere [Condividi modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).\
   >Per informazioni sull&#39;impostazione delle autorizzazioni per l&#39;attività, vedere [Condividere un&#39;attività](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).\
   >Per informazioni sull&#39;impostazione delle autorizzazioni per i modelli, vedere [Condividere un modello](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Facoltativo) Continua a modificare la sezione seguente, a seconda delle informazioni che desideri modificare.

   Oppure

   Fai clic su **Salva modifiche**.

### Commento {#comment}

1. Inizia a modificare un’attività modello come descritto in precedenza.
1. Fai clic su **Commento**.

   ![commento_modifica_attività.png](assets/comment-edit-task-350x138.png)

1. Nel campo disponibile, specifica un commento da visualizzare nel flusso di aggiornamenti dell’attività modello. Questo commento è visibile a tutti coloro che dispongono dell&#39;accesso di visualizzazione al modello e all&#39;attività modello e dell&#39;accesso di visualizzazione alle note.
1. Fai clic su **Salva modifiche**.

   Quando un utente crea un progetto a partire da questo modello, tutte le impostazioni applicate alle attività modello diventano le impostazioni delle attività progetto.
