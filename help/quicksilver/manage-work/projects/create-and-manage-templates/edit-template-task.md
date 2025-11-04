---
product-area: templates
keywords: attività,valori predefiniti,automatizza,creazione
navigation-topic: templates-navigation-topic
title: Modificare un’attività modello
description: Dopo aver creato un modello, è possibile modificare le informazioni sulle attività del modello. Le informazioni aggiornate in un'attività modello vengono associate alle attività del progetto dopo che è stato utilizzato il modello per creare un progetto o dopo che il modello è stato allegato a un progetto.
author: Alina
feature: Work Management
exl-id: 2df8522e-7eee-4440-be0f-f7483c5acdb0
source-git-commit: 46133f435c665dd82d134f18d0b5de4e70bab7d7
workflow-type: tm+mt
source-wordcount: '2631'
ht-degree: 3%

---

# Modificare un’attività modello

<!--Audited: 11/2025-->

<!--take out production and preview references and new/ old experiences at release-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 
-->

Dopo aver creato un modello, è possibile modificare le informazioni relative alle attività del modello. Le informazioni aggiornate in un&#39;attività modello vengono associate alle attività del progetto dopo che è stato utilizzato il modello per creare un progetto o dopo che il modello è stato allegato a un progetto.

Per informazioni sulla creazione di un modello, vedere [Creare un modello di progetto](../../../manage-work/projects/create-and-manage-templates/create-template.md).

È possibile modificare un&#39;attività modello alla volta oppure modificare le attività modello in blocco.

>[!NOTE]
>
>Non è possibile modificare in blocco le attività modello che appartengono a modelli diversi. È possibile modificare solo le attività modello che appartengono allo stesso modello.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Piano </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazione del livello di accesso</td> 
   <td> <p>Modificare l’accesso ai modelli</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto </td> 
   <td> <p>Consente di gestire le autorizzazioni per un modello. </p> <p>Impossibile condividere un'attività modello. </p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Standard </p>
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Templates</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions </td> 
   <td> <p>Manage permissions for a template. </p> <p>You cannot share a template task. </p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Prerequisiti

Prima di iniziare, è necessario

* Crea un modello.

  Per informazioni sulla creazione di un modello, vedere [Creare un modello di progetto](../../../manage-work/projects/create-and-manage-templates/create-template.md).

## Modifica le attività modello

È possibile modificare un&#39;attività modello utilizzando le aree Modifica attività modello o Dettagli attività modello.

{{step1-to-templates}}

1. Fare clic sul nome di un modello per aprirlo.
1. Fai clic su **Attività modello** nel pannello a sinistra.
1. Fare clic sul nome di un&#39;attività modello nell&#39;elenco per aprirla.
1. Per modificare informazioni limitate sull&#39;attività modello, eseguire le operazioni seguenti:
   1. (Facoltativo) Fai clic su **Aggiornamenti** nel pannello a sinistra per aggiungere aggiornamenti all&#39;attività modello. Gli aggiornamenti delle attività del modello non vengono trasferiti alle attività del progetto quando il modello viene utilizzato per creare un progetto.
   1. (Facoltativo) Fai clic su **Documenti** nel pannello a sinistra per aggiungere documenti all&#39;attività modello. I documenti verranno trasferiti alle attività del progetto quando si utilizza il modello per creare il progetto.
   1. (Condizionale) Per modificare informazioni limitate su un&#39;attività modello, fai clic su **Dettagli attività modello** nel pannello a sinistra, quindi vai alle aree della sezione Dettagli per modificare le informazioni per ogni area.
   1. (Facoltativo) Effettuate una delle seguenti operazioni:
      * Fai clic sull&#39;icona **Comprimi tutto** ![Comprimi tutto](assets/collapse-all-icon.png) per comprimere tutte le aree.
      * Fai clic sull&#39;icona **Modifica** ![Modifica icona](assets/edit-icon.png), quindi seleziona una delle aree seguenti oppure fai clic su **Modifica tutto** per modificare le informazioni in tutte le aree:

         * Panoramica
         * Forms personalizzato
I nomi dei moduli doganali vengono visualizzati solo se sono presenti moduli personalizzati allegati all’attività modello.
         * Finanz

        >[!TIP]
        >
        >Per informazioni su tutti i campi visualizzati nell&#39;area Dettagli, continuare a modificare tutti i campi utilizzando la casella Modifica attività modello, come descritto di seguito.

   1. (Facoltativo) Fai clic sulla sezione **Sottoattività** nel pannello a sinistra per aggiungere elementi secondari per l&#39;attività modello. L&#39;aggiunta di sottoattività per le attività modello è simile all&#39;aggiunta di sottoattività per le attività del progetto. Per informazioni, vedere la sezione &quot;Creare sottoattività dalla sezione Attività secondarie&quot; nell&#39;articolo [Creare sottoattività](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).
   1. (Facoltativo) Fai clic su **Spese** nel pannello a sinistra e aggiungi le spese alle attività modello. Trasferimento delle spese dell&#39;attività modello ad attività di progetto future, quando il modello viene utilizzato per creare un progetto.
   1. (Facoltativo) Fai clic su **Approvazioni** nel pannello a sinistra per creare approvazioni o allegare approvazioni globali o a livello di gruppo alle attività modello. Le approvazioni vengono trasferite ad attività di progetto future.
   1. (Facoltativo) Fai clic sulla sezione **Predecessori** nel pannello a sinistra per aggiungere predecessori per le attività modello. L’aggiunta di predecessori di attività modello è simile all’aggiunta di predecessori di attività progetto. Per informazioni, vedere [Creare una relazione predecessore utilizzando l&#39;area Predecessori](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).

1. (Facoltativo) Per modificare più attività modello in blocco, seleziona più attività modello, quindi fai clic su **Modifica** nella parte superiore dell&#39;elenco dei modelli.
1. (Condizionale) Per modificare tutte le informazioni sull&#39;attività modello o su più attività contemporaneamente, fai clic su per selezionarle da un elenco, quindi fai clic sull&#39;icona **Modifica** ![Icona Modifica](assets/edit-icon.png) nella parte superiore dell&#39;elenco.

   Viene visualizzata la casella **Modifica attività modello**.

   >[!TIP]
   >
   >Puoi anche selezionare un&#39;attività modello in un elenco, quindi fare clic su **Modifica** a destra del nome dell&#39;attività modello nell&#39;intestazione, per aprire la casella **Modifica attività modello**.

   ![Modifica attività modello](assets/edit-template-tasks-box-classic-350x356.png)

   <!--1. (Conditional) In the Production environment, -->
1. Prendere in considerazione la possibilità di specificare informazioni in una delle sezioni seguenti:

   * [Panoramica](#overview)
   * [Finanz](#finance)
   * [Impostazioni](#settings)
   * [Assegnazioni](#assignments)
   * [Moduli personalizzati](#custom-forms)
   * [Commento](#comment)

<!--1. Continue editing the template task as described in the Edit a template task using the old experience section in this article (********add hashtag anchor here*******)-->

<!--1. <span class="preview">(Conditional) In the Preview environment, click **Try new experience** in the upper-right corner of the **Edit Template Task** box </span>, then continue editing the template task as described in the Edit a template task using the new experience section in this article (********add hashtag anchor here*******).</span>
1. (Optional) Click **Switch back to old experience** at the bottom of the Edit Template Task box  
-->


<!--### Edit a template task using the old experience
(and make all the headers below "####")-->

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

<!--
<div class="preview"> 

### Edit a template task using the new experience

Consider specifying information in any of the following sections:

   * [Template task name](#template-task-name)
   * [Overview](#overview-1)
   * [Assignments](#assignments-1)
   * [Finance](#finance-1)
   * [Custom Forms](#custom-forms-1)
   * [Settings](#settings-1)
   * [Comment](#comment-1)

#### Template Task Name

1. Begin editing a template task as described above.
1. In the Edit Template Task box, click **Template Task Name** and add a name for the template task. 

   This view is not available when editing template tasks in bulk. 

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save**. 

#### Overview {#overview-1}

1. Begin editing a template task as described above.
1. In the **Edit Template Task** box, click **Overview** in the left panel. 

   ![Template task edit overview section](assets/template-task-edit-overview.png)

1. Update any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Add additional information about the template task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority</strong> </td> 
      <td> <p>This is a visual flag for you which allows you to prioritize your template tasks. </p> <p>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>None</strong> </p> </li> 
        <li> <p><strong>Low</strong> </p> </li> 
        <li> <p> <b>Normal</b></p> </li> 
        <li> <p><b>High</b> </p> </li> 
        <li> <p><b>Urgent</b> </p> </li> 
       </ul> <p>Depending on the Project Preferences selected by your Workfront administrator, the names of priorities might be different for you. For more information about editing priorities, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Create and customize priorities</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Task Constraint</strong> </td> 
      <td> <p>The task on the project created from this template will have this constraint. Task Constraints identify when a task must be completed. </p> <p>Select from the following options:</p> 
       <ul> 
        <li><strong>Fixed Dates</strong>. Specify a <strong>Planned Start</strong> and a <strong>Planned Completion Date.</strong></li> 
        <li><strong>Must Start On</strong>. Specify a <strong>Planned Start Date.</strong></li> 
        <li><strong>Must Finish On</strong>. Specify a <strong>Planned Completion Date</strong>.</li> 
        <li><strong>As Soon as Possible</strong> </li> 
        <li><strong>As Late as Possible</strong> </li> 
        <li style="font-weight: bold;"><strong>Earliest Available Time</strong> </li> 
        <li style="font-weight: bold;"><strong>Latest Available Time</strong> </li> 
        <li>Start No Later Than. Specify a <strong>Planned Start Date</strong>.</li> 
        <li><strong>Start No Earlier Than</strong>. Specify a <strong>Planned Start Date</strong>.</li> 
        <li><strong>Finish No Later Than</strong>. Specify a <strong>Planned Completion Date</strong>.</li> 
        <li><strong>Finish No Earlier Than</strong>. Specify a <strong>Planned Completion Date</strong>.</li> 
       </ul> <p>For more information on Task Constraint, see <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">Start Day</span><span style="font-weight: normal;"> (Optional and conditional)</span> </td> 
      <td> <p> You can specify the Start Day of a template task only when the Task&nbsp;Constraint is one of the following:</p> 
       <ul> 
        <li>Must Start On</li> 
        <li>Start No&nbsp;Earlier Than</li> 
        <li>Start No Later Than</li> 
        <li>Fixed Dates</li> 
       </ul> <p>This will correspond to the date within the timeline of the future project when the task will start. For all other constraints, Workfront calculates the Start Day based on predecessor dependency between the tasks. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Day</strong><span style="font-weight: normal;"> (Optional and conditional)</span> </td> 
      <td> <p> You can specify the Completion Day of a template task only when the Task Constraint is one of the following:</p> 
       <ul style="list-style-type: circle;"> 
        <li>Must Finish On</li> 
        <li>Finish No Earlier Than</li> 
        <li>Finish No Later Than</li> 
        <li>Fixed Dates</li> 
       </ul> <p>This will correspond to the date within the timeline of the future project when the task will complete. For all other constraints, Workfront calculates the Completion Day based on Duration and predecessor dependency. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>Specify a web link that relates to the information about the template task.</td> 
     </tr> 

     <tr> 
      <td role="rowheader"><strong>Work Effort</strong> </td> 
      <td>Choose from the following options:
      <ul><li>Small</li>
      <li>Medium</li>
      <li>Large</li></ul>

      <p><b>IMPORTANT</b></p>
      <p>The Work Effort field displays when editing a template task only when you select the <b>Use Work Effort to automatically calculate task Planned Hours</b> setting when editing the template.</p>

      </td> 
     </tr> 
     </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save**.

#### Assignments {#assignments-1}

1. Begin editing a template task as described above.
1. In the **Edit Template Task** box, click **Assignments** in the left panel.

   ![Template task edit assignments](assets/template-task-edit-assignments.png)

1. In the Search people, role, or teams field, start typing the name of an assignee, then select it when it displays in the list

   Or

   Click **Assign to me** to assign the template task to yourself.
1. Consider updating the following information: 

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 

<tr> 
      <td role="rowheader"><strong>Duration Type</strong> </td> 
      <td> <p>The future task created from this template will have this Duration Type. <br>The Duration Type identifies the relationship between the following:</p> 
      <ul>
      <li><p>Number of resources assigned to a task</p> </li>
      <li><p>The total effort required to complete the task</p></li> 
      <li><p>The total duration of the task </p></li></ul> <p>Using Duration Types, you can set consistent resource assignments based on the needs of the task. For more information about the Duration Type of a task, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> <p>Select from the following options:</p> 
       <ul> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Calculated Assignment</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Calculated Work</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Effort Driven</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Simple</span> <br> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Duration</strong> </td> 
      <td> <p>Specify the Duration of the future tasks, in minutes, hours, days, weeks, or months. The future task created from this template will have the Duration specified here.</p> <p>By default, Workfront measures Duration in days. This is the amount of time that you allow for the task to remain incomplete, before it must be completed. You cannot specify the Duration of a task when the <strong>Duration Type</strong> of the task is <strong>Simple</strong>, or when the <strong>Task Constraint</strong> is <strong>Fixed Dates</strong>.</p> <p><b>IMPORTANT</b></p> <p>Duration is typically the amount of time between the Planned Start and the Planned Completion Dates of a template task, and for this reason, it affects the timeline of the template. This determines the timeline of the future project created from the template. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planned Hours</strong> </td> 
      <td> <p>Specify the number of Planned Hours for the future task on the project created with this template. This is the amount of actual time it would take the assignees of the task to complete it. You can only specify the number of Planned Hours for a task when the <strong>Duration Type</strong> is set to <strong>Calculated Assignment</strong>. </p> </td> 
     </tr> 
  </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save**.

#### Finance {#finance-1}

1. Begin editing a template task as described above.
1. In the **Edit Template Task** box, click **Finance** in the left panel.

   ![Template task edit finance section](assets/template-task-edit-finance.png)

1. Update any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Cost Type</strong> </td> 
      <td> <p>Specify the Cost Type for the future task. This is going to determine how the Cost on the task is calculated, based on the number of hours on the tasks. </p> <p>Select from the following options:</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>No Cost</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Fixed Hourly</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>User Hourly</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Role Hourly</span> </p> </li> 
       </ul> <p>For more information about tracking costs, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Revenue Type</strong> </td> 
      <td> <p>Specify the Revenue Type for the future task. This is going to determine how the Revenue on the task is calculated, based on the number of hours on the tasks.</p> <p style="font-weight: normal;">Select from the following options: </p> 
       <ul> 
        <li> <p style="font-weight: normal;">Not Billable</p> </li> 
        <li> <p style="font-weight: normal;">User Hourly</p> </li> 
        <li> <p style="font-weight: normal;">Role Hourly</p> </li> 
        <li> <p style="font-weight: normal;">Fixed Hourly</p> </li> 
        <li> <p style="font-weight: normal;">User Hourly w/Cap</p> </li> 
        <li> <p style="font-weight: normal;">Role Hourly w/Cap</p> </li> 
        <li> <p style="font-weight: normal;">User Hourly Plus Fixed</p> </li> 
        <li> <p style="font-weight: normal;">Role Hourly Plus Fixed</p> </li> 
        <li> <p style="font-weight: normal;">Fixed Revenue</p> </li> 
       </ul> <p>For more information about tracking revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save**.


#### Custom Forms {#custom-forms}

You can define custom forms to be automatically attached by default to tasks when the tasks are added to a project. For information about setting up the project to include default task custom forms, see the "Tasks" section in the article [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

You can also add custom forms to the future tasks of a project when the project is created from a template, by adding the custom forms to the template tasks. 

1. Begin editing a template task as described above.
1. In the **Edit Template Task** box, click **Custom Forms** in the left panel.

   ![Template task edit custom forms section](assets/template-task-edit-custom-forms.png)

1. Select the custom form or forms that you want to associate with the template task. 

   You must build the custom forms before they are available to select in this field. 
   Only active custom forms display in the list. 

   For more information about building custom forms, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). 

   You can add up to ten custom forms to a template task. 
   The forms are automatically added to the tasks created from the template. 
1. (Conditional and optional) If you attached a custom form to the template task, edit any fields on the form. You must specify all required fields before you can save the template task.

   >[!NOTE]
   >
   >Depending on how your Workfront administrator set the permissions for the sections in your custom form, not everyone can view or edit the same fields on a given custom form. The permissions to edit fields within a section of a custom form depend on the permissions you have on the template task or the future task.   
   >For information about setting permissions on sections of a custom form, see [Share a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).   
   >For information about setting task permissions, see [Share a task](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).   
   >For information about setting template permissions, see [Share a template](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save**.

#### Settings {#settings-1}

1. Begin editing a template task as described above.
1. In the **Edit Template Task Box**, click **Settings** in the left panel.

   ![Template task edit settings section](assets/template-task-edit-settings.png)

1. Update any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Milestone</b></p></strong> </td> 
      <td> <p>Choose a milestone to associate with the selected template task.</p>
      
   <p><b>IMPORTANT</b></p>
   <p>You must associate a milestone path with a template for this field to display. For more information, see <a href="../create-and-manage-templates/edit-templates.md">Edit project templates</a>.</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>Tracking Mode</strong> </td> 
      <td> <p>Specify how the progress status of the future task will be tracked. </p> <p>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>User Must Update</strong> </p> </li> 
        <li> <p><strong>Assume on Time</strong> </p> </li> 
        <li> <p><strong>Ignore Late Warnings</strong> </p> </li> 
        <li> <p><strong>Autocomplete</strong> </p> </li> 
        <li> <p><strong>Predecessor</strong> </p> </li> 
       </ul> <p>For more information about the Tracking Mode on tasks, see <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Task Tracking Mode overview</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Reminder Notifications</strong> </td> 
      <td> <p>Select which Reminder Notifications you would like to attach to the template task. They will be attached to the future tasks on the project created from this template. Your system administrator must configure Reminder Notifications before you can select them on a task. For more information about configuring Reminder Notifications, see <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Set up reminder notifications</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approval Process</strong> </td> 
      <td> <p>Select the approval process you want to associate with the template task. Your Workfront administrator must define system-level task Approval Processes before you can associate them with template tasks. <span>A user with administrative access to Approval processes can also create group-specific approval processes.</span> For more information about creating approval processes, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Create an approval process for work items</a>.</p> <p>Consider the following when adding approval processes: </p> 
       <ul> 
       <li>Only active approval processes display in the list. </li> 
       <li> <p>System-wide and group-specific approval processes display in the list. Approval processes associated with a group other than that of the template do not display in the list.</p> <p>Important: If the group associated with the template changes, the group-specific approval process becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">How group and approval process changes affect assigned approval processes</a>. </p> </li> 
       <li> <p>If you added a single-use approval process, it displays as "&lt;Custom&gt;" in this field. For information, see <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associate a new or existing approval process with work</a>. </p>  </li> 
       <li> <p>When bulk-editing template tasks, the following scenarios exist:</p> 
       <ul> 
       <li> <p>When you select template tasks from the same template group, both system-level and group-level approval processes display in this field.</p> </li> 
       <li> <p>When you select template tasks from different template groups, only system-level approval processes display in this field.</p> </li> 
       <li> <p>When any of the template tasks has a single-use approval process attached, it is replaced by the system-level <span>or group-level approval process</span> you select. </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr> 
     
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save**.

#### Comment {#comment-1}

1. Begin editing a template task as described above.
1. In the **Edit Template Task** box, click **Comment** in the left panel.

   ![Template task edit Comment section](assets/template-task-edit-comment.png)

1. In the **Add an update to the template task** area, specify a comment that you want to display in the updates stream of the template task in the available field. This comment is visible for everyone with View access to the template and the template task and with access to view Notes.
1. Click **Save**.

   When you or another user creates a project from this template, all settings you applied to template tasks become the settings for the project tasks.

</div>

-->