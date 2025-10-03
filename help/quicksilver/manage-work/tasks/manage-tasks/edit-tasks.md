---
product-area: projects
navigation-topic: manage-tasks
title: Modifica le Attività
description: Potete modificare le informazioni sulle attività create o sulle quali disponete delle autorizzazioni Contribute o Manage. In questo articolo viene descritto come cercare, trovare e modificare un'attività, se si dispone delle autorizzazioni necessarie.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 572c6008-3a67-47ae-8f5d-6b871ef1f37b
source-git-commit: 3b5452c51c19edfafc9244c2cfd58d7174732375
workflow-type: tm+mt
source-wordcount: '3829'
ht-degree: 4%

---

# Modifica attività

<!--Audited: 07/2024-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: some information in this area is repeated in the following articles. If you need to update a field, update it in both:</p>
<p>** Task finances in details</p>
<p>** Task information in overview)</p>
</div>
-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 
-->


Potete modificare le informazioni sulle attività create o sulle quali disponete delle autorizzazioni Contribute o Manage.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Standard</p>
   <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> 
    <ul> 
     <li> <p>Concedere le autorizzazioni per un'attività per modificare le informazioni seguenti nell'area Dettagli attività: </p>
     <ul>
     <li>Descrizione</li>
     <li>Stato</li>
     </ul>  
      </li> 
     <li> <p>Gestire le autorizzazioni per un'attività per modificare tutte le informazioni nell'area Dettagli e nella casella Modifica attività</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Autorizzazioni Contribute (Contribute) o superiori per il progetto</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limitazioni per la modifica delle attività

Esistono alcune limitazioni che potrebbero impedire la modifica delle attività.

Quando modifichi le attività, tieni presente quanto segue:

* L’aggiornamento delle attività attiva le notifiche per i progetti che si trovano nello stato Corrente. Per evitare confusione per gli utenti assegnati alle attività, limita il più possibile le attività di modifica quando il progetto è nello stato Corrente.
* Non è possibile modificare le attività in un processo di approvazione. È possibile registrare solo l&#39;ora o aggiornare lo stato di un&#39;attività in un processo di approvazione.

  ![Modifica attività con processo di approvazione](assets/edit-task-in-approval-process-nwe-350x148.png)

* È possibile modificare e aggiungere documenti alle attività di un progetto con stato Completato, Inattivo o In attesa di approvazione solo quando l&#39;amministratore di Workfront o un amministratore di gruppo ha abilitato questa funzionalità nell&#39;area Preferenze progetto. Per informazioni sull&#39;impostazione delle preferenze di progetto, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* È sempre possibile modificare le informazioni seguenti su un&#39;attività quando il progetto è stato contrassegnato come Completo, Inattivo o si trova in un processo di approvazione:

   * Registra ore
   * Modifica spese esistenti
   * Allega un modulo personalizzato

* Gli altri utenti devono aggiornare le proprie pagine prima di poter visualizzare gli aggiornamenti apportati a un&#39;attività.

## Modificare un’attività in un elenco

È possibile modificare le informazioni sulle attività in un elenco di attività modificando i campi in linea visualizzati nella visualizzazione dell&#39;elenco.

Per informazioni sulla modifica delle attività negli elenchi, vedere [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

## Modificare un&#39;attività in un elenco utilizzando il Riepilogo

Potete modificare un&#39;attività in un elenco utilizzando il pannello Riepilogo. Per informazioni sulla modifica di un&#39;attività nel pannello Riepilogo, vedere la sezione &quot;Modifica un&#39;attività nel Riepilogo&quot; nell&#39;articolo [Modifica attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

## Modificare un&#39;attività nella casella Modifica attività

È possibile modificare un&#39;attività utilizzando le aree Modifica attività o Dettagli attività. Nei passaggi seguenti viene descritta la modifica di un&#39;attività nella casella Modifica attività.

{{step1-click-main-menu}}

1. Fai clic su **Progetti**, quindi fai clic sul nome di un progetto per aprirlo.
1. Fai clic su **Attività** nel pannello a sinistra.
1. Fare clic sull&#39;attività da modificare.
1. (Condizionale) Per modificare informazioni limitate su un&#39;attività, fai clic su **Dettagli attività** nel pannello a sinistra.

   ![](assets/nwe-task-details-expanded-350x273.png)

   È consigliabile modificare le informazioni nelle aree seguenti della sezione Dettagli attività:

   * **Panoramica**

     L&#39;area viene espansa per impostazione predefinita.

   * **Moduli personalizzati**

     I nomi dei moduli doganali vengono visualizzati solo se all’oggetto sono allegati moduli personalizzati.

   * **Finanza**

   >[!NOTE]
   >
   >A seconda della modalità di modifica del modello di layout da parte dell&#39;amministratore di Workfront o del gruppo, i campi nell&#39;area Dettagli attività potrebbero essere ridisposti o non visualizzati. Per informazioni, vedere [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Per informazioni sui campi visibili nella sezione Dettagli attività, continuare a modificare l&#39;attività nella casella Modifica attività come descritto di seguito.

   Per modificare le informazioni nella sezione Dettagli, effettuare le seguenti operazioni:

   1. (Facoltativo) Fai clic sull&#39;icona **Comprimi tutto** ![](assets/collapse-all-icon.png) nell&#39;angolo superiore destro per comprimere tutte le aree.
   1. (Facoltativo e condizionale) Quando un&#39;area è compressa, fare clic sulla **freccia rivolta a destra** ![](assets/right-pointing-arrow.png) accanto a ogni area per espandere l&#39;area che si desidera modificare.
   1. Per ulteriori informazioni sulla modifica delle informazioni nella scheda Dettagli attività, vedere gli articoli seguenti:

      * [Gestire le informazioni sull&#39;attività nell&#39;area Panoramica dettagli attività](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)
      * [Gestire i dati finanziari delle attività nella sezione Dettagli attività](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)

   1. (Facoltativo) Se non sono presenti moduli personalizzati allegati all&#39;attività, inizia a digitare il nome di un modulo nel campo **Aggiungi modulo personalizzato**, quindi selezionalo quando viene visualizzato nell&#39;elenco, quindi fai clic su **Salva modifiche**.
   1. (Facoltativo) Fai clic sull&#39;icona **Esporta** ![](assets/export.png) per esportare le informazioni sulla panoramica e sui moduli personalizzati in un file PDF, quindi fai clic su **Esporta**. Selezionare una delle opzioni seguenti:

      * Seleziona tutto (viene visualizzato solo se è allegato almeno un modulo personalizzato)
      * Panoramica
      * Nome di uno o più moduli personalizzati

      Il file PDF viene scaricato nel computer.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Per ulteriori informazioni, vedere [Esportare moduli personalizzati e dettagli oggetto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

1. (Condizionale) Per modificare tutte le informazioni sull&#39;attività, in qualità di utente con autorizzazioni di gestione per l&#39;attività, fai clic sul menu **Altro** ![](assets/more-icon.png) accanto al nome dell&#39;attività, quindi fai clic su **Modifica**.

   Oppure

   Da un elenco di attività, seleziona un&#39;attività, quindi fai clic sull&#39;icona **Modifica** ![](assets/edit-icon.png) nella parte superiore dell&#39;elenco.

   Viene visualizzata la casella Modifica task (Edit Task).

   >[!IMPORTANT]
   >
   >Per visualizzare l’opzione Modifica, è necessario disporre delle autorizzazioni di gestione per l’attività.

   Tutti i campi delle attività sono disponibili nella casella Modifica attività e sono raggruppati per le aree elencate nel pannello a sinistra.

   >[!NOTE]
   >
   >A seconda della modalità di modifica del modello di layout da parte dell&#39;amministratore di Workfront o del gruppo, i campi nell&#39;area Dettagli attività potrebbero essere ridisposti o non visualizzati. Per informazioni, vedere [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Prendere in considerazione la possibilità di specificare informazioni in una delle sezioni seguenti:

   * [Nome attività](#task-name)
   * [Panoramica](#overview)
   * [Assegnazioni](#assignments)
   * [Moduli personalizzati](#Custom%C2%A0F)
   * [Finanza](#finance)
   * [Impostazioni](#settings)
   * [Commento](#comment)

   >[!NOTE]
   >
   >A seconda del modo in cui l&#39;amministratore di Workfront o il gruppo imposta il modello di layout, i campi nella casella Modifica attività potrebbero essere ridisposti o non visualizzati. Per informazioni, vedere [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### Nome attività {#task-name}

1. Inizia a modificare l’attività come descritto in precedenza.
1. Fai clic su **Nome attività** nel pannello a sinistra.

   ![](assets/nwe-task-name-section-edit-task-box-350x122.png)

1. Aggiorna il nome dell&#39;attività.

1. Fai clic su **Salva** o continua con le sezioni seguenti.

### Panoramica {#overview}

1. Inizia a modificare l’attività come descritto in precedenza.
1. Fai clic su **Panoramica** nel pannello a sinistra.

   ![](assets/nwe-overview-section-edit-task-box-350x257.png)

1. Aggiorna le seguenti informazioni sull&#39;attività:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Aggiungere ulteriori informazioni sull'attività. </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Sezione informazioni di base</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stato</td> 
      <td> <p>Selezionare lo stato dell'attività che indica la fase di sviluppo in cui si trova l'attività.</p> <p><b>SUGGERIMENTO</b>

   È possibile aggiornare lo Stato dell&#39;attività nell&#39;intestazione dell&#39;attività. </p>

   <p>L'amministratore del Workfront o del gruppo può personalizzare i nomi degli stati delle attività. Per informazioni, vedere <a href="/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md">Creare o modificare uno stato</a>. 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Priorità</td> 
      <td> <p>Questo è un flag visivo che ti consente di assegnare la priorità alle attività. </p> <p>Selezionare una delle opzioni seguenti: </p> 
       <ul> 
      <li> <p> Nessuno</p> </li> 
      <li> <p> Basso </p> </li> 
      <li> <p>Normal </p> </li> 
      <li> <p>Alta </p> </li> 
      <li> <p> Urgente </p> </li> 
       </ul> <p>A seconda delle Preferenze di progetto selezionate dall'amministratore di Workfront, i nomi delle priorità potrebbero essere diversi. Per informazioni sulle priorità delle attività, vedere <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">Aggiorna priorità attività</a>. </p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Sezione vincoli e date attività</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vincolo attività</td> 
      <td> <p>Decidere quando l'attività deve essere completata specificando un vincolo attività. </p> <p>Selezionare una delle opzioni seguenti: </p> 
       <ul> 
      <li> <p><span>Date fisse</span> </p> <p>Specifica un <strong>Inizio pianificato</strong> e una <strong>Data di completamento pianificata</strong>. </p> </li> 
      <li> <p><span>Deve Iniziare Il</span> </p> <p>Specifica una <strong>data inizio pianificata</strong>. </p> </li> 
      <li> <p><span>Deve Terminare Il</span> </p> <p>Specifica una <strong>data di completamento pianificata</strong>. </p> </li> 
       </ul> 
       <ul> 
      <li> <p><span>Il Prima Possibile</span></p> </li> 
      <li> <p><span>Più tardi possibile</span></p> </li> 
      <li> <p><span>Primo Orario Disponibile</span></p> </li> 
      <li> <p> <span>Ultimo Orario Disponibile</span></p> </li> 
      <li> <p><span>Inizia Non Dopo Di</span> </p> </li> 
      <li> <p>Specifica una data di inizio pianificata</p> </li> 
      <li> <p><span>Iniziare Non Prima Di</span> </p> <p>Specifica una <strong>data inizio pianificata</strong>. </p> </li> 
      <li> <p> Termina <span>Non Dopo Di</span></p> <p>Specifica una <strong>data di completamento pianificata</strong>. </p> </li> 
      <li> <p> Termina <span>Non Prima Di</span></p> <p>Specifica una <strong>data di completamento pianificata</strong></p> </li> 
       </ul> <p>Per ulteriori informazioni sul vincolo attività, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sul vincolo attività</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Conferma data e ora</td> 
      <td> <p>Si tratta della data entro la quale l’utente assegnato all’attività si impegna a completarla. Questo può essere diverso dalla Data di completamento pianificata. Solo gli assegnatari possono modificare questo campo. Per informazioni sulle date di conferma in Workfront, vedere <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Panoramica sulla data di conferma</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora di inizio pianificate</td> 
      <td> <p>Quando è pianificato l’inizio dell’attività. La data di inizio pianificata di un'attività viene impostata e influenzata da diversi fattori:</p> 
       <ul> 
      <li>A seconda della preferenza a livello di sistema per la data di inizio pianificata dell'attività, la data di inizio di una nuova attività in un progetto può essere la data odierna o la data di inizio del progetto, per impostazione predefinita. <span>Anche l'amministratore del gruppo associato al progetto può impostare questa preferenza per il gruppo.</span> Per ulteriori informazioni sulle preferenze per le attività a livello di sistema o di gruppo, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configurare le preferenze per attività e problemi a livello di sistema</a>.</li> 
      <li>A seconda dei predecessori dell'attività, la data di inizio pianificata viene scelta da Workfront come data disponibile successiva alla fine o all'inizio del predecessore, a seconda della relazione del predecessore. Per ulteriori informazioni sulle relazioni con i predecessori, vedere <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Panoramica sui predecessori delle attività</a>.</li> 
      <li>Il project manager o il proprietario dell'attività possono impostare manualmente la data di inizio pianificata quando il vincolo dell'attività è Date fisse o Deve iniziare il. Per ulteriori informazioni sui vincoli delle attività, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sui vincoli delle attività</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora di completamento pianificate</td> 
      <td> <p>Data di completamento prevista, come visualizzata quando l'attività è pianificata. Workfront imposta la data di completamento pianificata utilizzando alcuni dei fattori seguenti:</p> 
       <ul> 
      <li>La data di completamento pianificata viene calcolata a partire dalla data di inizio pianificata aggiungendo la Durata dell'attività alla data di inizio pianificata. Quando il project manager o Workfront specifica la durata dell'attività, viene attivato un aggiornamento della data di completamento pianificata. Se la data pianificata cambia, ciò accade spesso perché la Durata dell'attività è stata aggiornata.</li> 
      <li>Il project manager o il proprietario dell'attività possono impostare manualmente la data di completamento pianificata quando il vincolo dell'attività è Date fisse o Deve finire il. Per ulteriori informazioni sui vincoli delle attività, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sui vincoli delle attività</a>.</li> 
      <li>Se il Tipo di Durata dell'attività cambia e il numero di risorse sulle attività cambia contemporaneamente, cambierà anche la data di completamento pianificata. Per ulteriori informazioni sui tipi di durata, vedere <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica sulla durata dell'attività e sul tipo di durata</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora di inizio effettive</td> 
      <td> <p>Specificare una data di inizio effettiva per l'attività. Il valore predefinito viene generalmente popolato automaticamente quando si modifica lo stato dell'attività in In corso. La data di inizio effettiva può anche essere modificata manualmente dal project manager o dal proprietario dell'attività. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora di completamento effettive</td> 
      <td> <p>Specificare la data e l'ora effettive di completamento dell'attività. La data e l'ora predefinite di completamento di un'attività coincidono sempre con l'ora effettiva in cui lo stato diventa Completato. Il project manager o il proprietario dell'attività può inoltre modificare manualmente la data di completamento effettiva. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>Sezione Orario di lavoro</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Impegno di lavoro </td> 
      <td>

   <p>Quantità di lavoro necessaria per completare l'attività. È possibile che il project manager decida di utilizzare questo campo anziché le ore pianificate per stimare lo sforzo necessario per completare un'attività. Questo campo è visibile solo quando sono soddisfatte le seguenti condizioni:</p> 
      <ul> 
      <li> <p>L’attività ha un tipo di durata semplice. </p> <p><b>SUGGERIMENTO</b>

   Se si modifica il Tipo di durata dell&#39;attività, questo campo viene oscurato. </p> </li>
   <li>Il project manager ha abilitato il campo Usa impegno di lavoro per calcolare automaticamente le ore pianificate dell'attività nel progetto. </li> 
      </ul> 
      <p>Selezionare una delle opzioni seguenti:</p> 
      <ul> 
      <li>Piccola</li> 
      <li>Medium <span style="font-weight: normal;">(valore predefinito per una nuova attività)</span></li> 
      <li>Grande</li> 
      </ul> 
      <p><b>NOTA</b>

   L&#39;aggiornamento della quantità di lavoro potrebbe aggiornare le ore pianificate dell&#39;attività. L&#39;aggiornamento è immediato se il tipo di aggiornamento del progetto è Automatico. Quando il tipo di aggiornamento del progetto è Manuale, è necessario ricalcolare la sequenza temporale per visualizzare le ore pianificate aggiornate. </p>

   <p>Per informazioni sull'utilizzo dell'Impegno di lavoro invece delle Ore pianificate per stimare l'impegno di attività, vedere <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Panoramica sull'impegno di lavoro</a>. </p> 
    </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva** o continua con le sezioni seguenti.

### Assegnazioni {#assignments}

1. Inizia a modificare l’attività come descritto in precedenza.
1. Fai clic su **Assegnazioni** nel pannello a sinistra.

   ![](assets/nwe-assignments-section-edit-task-box-350x217.png)

1. Fai clic su **Cerca persone, mansione e team** e inizia a digitare il nome di un utente, una mansione o un team che desideri assegnare all&#39;attività, quindi fai clic su di esso o premi Invio quando viene visualizzato nell&#39;elenco.

   >[!NOTE]
   >
   >Se il nome dell&#39;utente contiene un carattere speciale, è necessario includere tale carattere nel campo di ricerca.

   >[!TIP]
   >
   >Puoi assegnare più utenti, mansioni o team. Puoi assegnare solo utenti attivi, mansioni e team.
   >
   >Se un utente, una mansione o un team è stato assegnato prima della disattivazione, rimane assegnato all&#39;elemento di lavoro. In questo caso, consigliamo quanto segue:
   >
   >* Riassegnare l&#39;elemento di lavoro alle risorse attive.
   >* Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.

1. (Facoltativo) Indica se un assegnatario è l&#39;assegnatario principale dell&#39;attività, selezionando il pulsante di opzione **Proprietario** accanto al nome. Un team non può essere l&#39;assegnatario principale di un&#39;attività.
1. (Condizionale e facoltativo) Aggiorna i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipo di Durata</td> 
      <td> <p>Questo identifica la relazione tra i seguenti: </p> 
       <ul> 
      <li> <p>Numero di risorse assegnate a un'attività </p> </li> 
      <li> <p>Lo sforzo totale richiesto per completare l'attività </p> </li> 
      <li> <p> Durata totale dell'attività. </p> </li> 
       </ul> <p>L'amministratore di Workfront o un amministratore gruppo seleziona l'impostazione predefinita Tipo di durata per le attività del sistema o del gruppo. Per informazioni sull'impostazione delle impostazioni predefinite del progetto, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configurare le preferenze relative a problemi e attività a livello di sistema</a>. </p> <p>I tipi di durata consentono di impostare assegnazioni di risorse coerenti in base alle esigenze dell'attività. Per ulteriori informazioni sul tipo di durata di un'attività, vedere <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica sulla durata e sul tipo di durata dell'attività</a>. </p> <p>Selezionare una delle opzioni seguenti: </p> 
       <ul> 
      <li> <p>Incarico Calcolato </p> </li> 
      <li> <p> Lavoro Calcolato </p> </li> 
      <li> <p>Impegno Aggiuntivo </p> </li> 
      <li> <p>Semplice</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Durata per Occorrenza</td> 
      <td> <p>Viene visualizzato solo sull'elemento padre delle attività ricorrenti. Viene visualizzata la durata di ogni attività ricorrente, definita al momento della creazione dell'attività. Per informazioni sulla creazione di attività ricorrenti, vedere <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Creare attività ricorrenti</a>. </p> <p> <b>NOTA</b>

   Le durate modificate in singole attività ricorrenti non visualizzano il valore indicato in questo campo. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Durata</td> 
      <td> 
      <div> 
      <div> 
      <p>Quantità di tempo che consente a un'attività di rimanere aperta prima del completamento. </p> 
      <p><b>IMPORTANTE</b>

   Poiché la durata dell&#39;attività corrisponde in genere al tempo che intercorre tra l&#39;inizio pianificato e le date di completamento pianificate, influisce sulla sequenza temporale del progetto.</p>

   <p>Per indicare la durata dell'attività e l'unità di tempo, eseguire le operazioni seguenti:</p> 
      <ul> 
      <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Digita il periodo di tempo e seleziona una delle unità di tempo disponibili nel menu a discesa.</p> <p><b>SUGGERIMENTO</b></p>
      Quando si aggiorna la Durata delle attività in un elenco di attività, è possibile utilizzare l'abbreviazione per l'unità di tempo. </p> </li> 
      </ul> 
      <p> Nella tabella seguente è possibile scegliere tra le opzioni relative al tempo normale o al tempo trascorso: </p> 
      <table style="table-layout:auto"> 
      <col> 
      <col data-mc-conditions=""> 
      <tbody> 
      <tr> 
      <td>Unità di tempo</td> 
      <td>Abbreviazione</td> 
      </tr> 
      <tr> 
      <td>Minutes</td> 
      <td>M</td> 
      </tr> 
      <tr> 
      <td>Ore</td> 
      <td>H</td> 
      </tr> 
      <tr> 
      <td>Giorni. Questa è l'impostazione predefinita. </td> 
      <td>Dsbld</td> 
      </tr> 
      <tr> 
      <td>Weeks</td> 
      <td>M</td> 
      </tr> 
      <tr> 
      <td>Months</td> 
      <td>T</td> 
      </tr> 
      <tr> 
      <td>Minuti trascorsi</td> 
      <td>EM</td> 
      </tr> 
      <tr> 
      <td>Ore trascorse</td> 
      <td>EH</td> 
      </tr> 
      <tr> 
      <td>Giorni trascorsi</td> 
      <td>ED</td> 
      </tr> 
      <tr> 
      <td>Settimane trascorse</td> 
      <td>EW</td> 
      </tr> 
      <tr> 
      <td>Mesi trascorsi</td> 
      <td>ET</td> 
      </tr> 
      </tbody> 
   </table>

   <p><b>NOTA</b>

   <p>Il tempo trascorso è un'unità di tempo per la durata di un'attività. Si tratta del tempo che intercorre tra la Data inizio pianificata e la Data completamento pianificata di un'attività e che include ferie, fine settimana e ferie. In altre parole, il tempo trascorso è il trascorrere dei giorni di calendario.

   L&#39;orario regolare prende in considerazione le festività, i fine settimana e le ferie e le esclude dalla Durata dell&#39;attività. Per ulteriori informazioni sulla durata dell&#39;attività, vedere <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica sulla durata e sul tipo di durata dell&#39;attività</a>. </p>
   </div> 
   </div> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Lavoro Necessario</td> 
   <td> <p>Specifica il numero di ore pianificate per l'attività, in ore. Quantità di tempo effettivo necessario agli assegnatari dell'attività per completare l'attività. È possibile specificare solo il numero di ore pianificate per un'attività quando il tipo di durata è impostato su Assegnazione calcolata. Per ulteriori informazioni sui tipi di durata, vedere <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica sulla durata dell'attività e sul tipo di durata</a>.</p> 
   <b>NOTA</b>
   <p>
   Quando si creano attività ricorrenti, le ore pianificate sono quelle di ogni occorrenza. Le ore pianificate delle attività padre sono il totale di tutte le ore pianificate di tutte le occorrenze. Per informazioni sulla creazione di attività ricorrenti, vedere <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Creare attività ricorrenti</a>.
   </p>

   </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Allocazione</td> 
   <td> <p>Se il vincolo dell'attività è Lavoro calcolato o Impegno, specificare <strong>Allocazione %</strong> (percentuale di allocazione) per ogni assegnatario. Quantità di tempo della pianificazione dell'assegnatario che può trascorrere per l'attività. Se si modifica la percentuale di allocazione per un assegnatario, verranno modificate le ore pianificate di un'attività. </p> <p>Quando Vincolo attività è Semplice, è possibile specificare quanto segue:</p> 
      <ul> 
      <li> <p>Ore di allocazione di ciascun assegnatario.</p> </li> 
      <li> <p>Ore pianificate dell'attività</p> </li> 
      <li> <p>Durata dell’attività</p> </li> 
      </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Mansione dell'assegnatario</td> 
   <td> <p>Selezionare una mansione dal menu a discesa <strong>Ruolo dell'assegnatario</strong> quando si seleziona una persona come assegnatario. Questo è il ruolo che l’assegnatario può svolgere per questa attività. </p> <p><b>SUGGERIMENTO</b>

   Nel menu a discesa vengono visualizzati solo i ruoli associati a ciascun assegnatario nel relativo profilo.</p> </td>
   </tr> 
      </tbody> 
      </table>

1. Fai clic su **Salva** o continua con le sezioni seguenti.

### Moduli personalizzati

È possibile definire moduli personalizzati predefiniti da allegare automaticamente alle attività quando queste vengono aggiunte a un progetto. Per informazioni sulla configurazione del progetto per includere moduli personalizzati predefiniti per tutte le nuove attività, vedere la sezione &quot;Attività&quot; nell&#39;articolo [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Inizia a modificare l’attività come descritto in precedenza.
1. Fai clic su **Forms personalizzato** nel pannello a sinistra oppure sul nome di un modulo personalizzato, se è già allegato.

   ![](assets/nwe-custom-forms-section-edit-task-box-350x127.png)

1. Fare clic su **Aggiungi modulo personalizzato** e selezionare il modulo o i moduli personalizzati che si desidera associare all&#39;attività. Devi creare i moduli personalizzati prima che siano disponibili per la selezione in questo campo. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi.

   Per ulteriori informazioni sulla creazione di moduli personalizzati, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).È possibile aggiungere fino a dieci moduli personalizzati a un&#39;attività

1. (Condizionale) Se hai allegato un modulo personalizzato all’attività, modifica eventuali campi del modulo. È necessario specificare tutti i campi obbligatori prima di salvare l&#39;attività.

   >[!NOTE]
   >
   >A seconda di come l’amministratore di Workfront imposta le autorizzazioni per le sezioni nel modulo personalizzato, non tutti possono visualizzare o modificare gli stessi campi in un determinato modulo personalizzato. Le autorizzazioni per modificare i campi all’interno di una sezione di un modulo personalizzato dipendono dalle autorizzazioni di cui disponi per l’attività stessa. Per informazioni sull&#39;impostazione delle autorizzazioni per l&#39;attività, vedere [Condividere un&#39;attività](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

1. Fai clic su **Salva** o continua con le sezioni seguenti.

### Finanz {#finance}

1. Inizia a modificare l&#39;attività come descritto nella sezione [Modifica attività](#Edit2) in questo articolo.
1. Fai clic su **Finanza** nel pannello a sinistra.

   ![](assets/nwe-finance-section-edit-task-box-350x298.png)

1. Aggiorna i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipo di costo</td> 
      <td> <p>Specificare il tipo di costo per l'attività. Questo determinerà come viene calcolato il costo dell'attività, in base al numero di ore sulle attività. </p> <p>Selezionare una delle opzioni seguenti: </p> 
       <ul> 
        <li> <p>Nessun Costo</p> </li> 
        <li> <p>Ore Fisse </p> </li> 
        <li> <p> Ore Utente </p> </li> 
        <li> <p> Ore Ruolo</p> </li> 
       </ul> <p>Per ulteriori informazioni sul tracciamento dei costi, vedere <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tracciare i costi</a> . L'amministratore di Workfront o un amministratore di gruppo seleziona l'impostazione Tipo di costo predefinita per le attività del sistema o del gruppo. Per informazioni sull'impostazione delle impostazioni predefinite del progetto, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze del progetto a livello di sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di entrate</td> 
      <td> <p>Specificare il tipo di retribuzione per l'attività. Questo determinerà il modo in cui vengono calcolati i Ricavi sull'attività, in base al numero di ore sulle attività. </p> <p>Selezionare una delle opzioni seguenti: </p> 
       <ul> 
      <li> <p> Non Fatturabile </p> </li> 
      <li> <p>Ore Utente </p> </li> 
      <li> <p>Ore Ruolo </p> </li> 
      <li> <p>Ore Fisse </p> </li> 
      <li> <p>Ore utente con limite </p> </li> 
      <li> <p>Ore ruolo con limite </p> </li> 
      <li> <p>Ore Utente più Fisso </p> </li> 
      <li> <p>Ore Ruolo più Fisso </p> </li> 
      <li> <p>Reddito Fisso </p> </li> 
       </ul> <p>Per ulteriori informazioni sul tracciamento dei ricavi, vedi<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica su fatturazione e ricavi</a> . </p> <p>L'amministratore di Workfront o l'amministratore di gruppo seleziona l'impostazione Tipo di retribuzione predefinita per le attività del sistema o del gruppo. Per informazioni sull'impostazione delle impostazioni predefinite del progetto, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze del progetto a livello di sistema</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva** o continua con la sezione seguente.

### Impostazioni {#settings}

1. Inizia a modificare l&#39;attività come descritto nella sezione [Modifica attività](#Edit2) in questo articolo.
1. Fai clic su **Impostazioni** nel pannello a sinistra.

   ![](assets/nwe-settings-section-edit-task-box-350x304.png)

1. Aggiorna i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Modalità Tracciamento</td> 
      <td> <p>Specificare la modalità di verifica dello stato di avanzamento dell'attività. </p> <p>Selezionare una delle opzioni seguenti: </p> 
       <ul> 
      <li> <p> Utente deve Aggiornare </p> </li> 
      <li> <p>Presupponi puntuale </p> </li> 
      <li> <p>Ignora Avvertimenti di Ritardo</p> </li> 
      <li> <p> Completamento automatico </p> </li> 
      <li> <p>Predecessore </p> </li> 
       </ul> <p>Per ulteriori informazioni sulla modalità di verifica delle attività, vedere <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Panoramica sulla modalità di verifica delle attività</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Livellamento Risorse</td> 
      <td> <p>Selezionare il campo <strong>Escludi dal livellamento risorse</strong> se si desidera escludere dal livellamento le risorse assegnate all'attività.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ritardo di Livellamento</td> 
      <td> <p>Specifica il ritardo di livellamento in ore. </p> <p> Per ulteriori informazioni sui ritardi di livellamento, vedere <a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">Aggiorna ritardo di livellamento attività</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processo di approvazione</td> 
      <td> <p>Selezionare un processo di approvazione da associare all'attività. Prima di poter associare i processi alle attività, l'amministratore di Workfront deve definirli a livello di sistema. Un utente con accesso amministrativo ai processi di approvazione può anche creare processi di approvazione specifici per il gruppo. </p> <p>Per ulteriori informazioni sulla creazione di processi di approvazione, vedere <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md">Creare un processo di approvazione per gli elementi di lavoro</a>. Quando aggiungi processi di approvazione, tieni presente quanto segue: </p> 
       <ul>

   <li> <p>Nell'elenco vengono visualizzati solo i processi di approvazione attivi. </p> </li>

   <li> <p>I processi di approvazione a livello di sistema e di gruppo vengono visualizzati nell’elenco. Un processo di approvazione associato a un gruppo diverso da quello del progetto non viene visualizzato nell’elenco. </p>

   <p><b>IMPORTANTE</b>

   Se il gruppo del progetto cambia, il processo di approvazione specifico del gruppo precedentemente allegato diventa un processo di approvazione a utente singolo. Per ulteriori informazioni su come le modifiche al gruppo del progetto o le modifiche al processo di approvazione influiscono sulle impostazioni di approvazione, vedere <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">Come le modifiche al gruppo e al processo di approvazione influiscono sui processi di approvazione assegnati</a>. </p>

   </li>

   <li> <p>È possibile definire processi di approvazione predefiniti da allegare automaticamente alle attività quando queste vengono aggiunte a un progetto. Per informazioni sulla configurazione del progetto per includere i processi di approvazione attività predefiniti, vedere la sezione "Attività" nell'articolo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Modifica progetti</a>. </p> </li>

   <li> <p>Quando si modificano attività in blocco, si verificano i seguenti scenari: </p> 
      <ul> 
      <li> <p>Quando si selezionano più attività dallo stesso gruppo, in questo campo vengono visualizzati sia i processi di approvazione a livello di sistema che quelli a livello di gruppo. </p> </li> 
      <li> <p>Quando si selezionano più attività da gruppi diversi, in questo campo vengono visualizzati solo i processi di approvazione a livello di sistema. </p> </li> 
      <li> <p>Quando a una delle attività è associato un processo di approvazione a utente singolo, questo viene sostituito dal processo di approvazione a livello di sistema o di gruppo selezionato. </p> </li>

   </ul> </li> 
      </ul> </td> 
     </tr> 
    </tbody> 
   </table>
    </li>

1. Fai clic su **Salva** o continua con la sezione seguente.

<!--notes from the table: <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)</p>       -->

### Commento

1. Inizia a modificare l&#39;attività come descritto nella sezione [Modifica attività](#Edit2) in questo articolo.
1. Fai clic su **Commento** nel pannello a sinistra.

   ![Sezione commenti sulla casella dell&#39;attività di modifica](assets/comment-section-on-edit-task-box.png)

1. Aggiungi un aggiornamento nello spazio fornito.
1. (Facoltativo) Aggiungi una delle seguenti opzioni all’aggiornamento:

   * Aggiungi utenti o team all&#39;aggiornamento nell&#39;area **Assegna tag a persone** o utilizza @ per includerli nell&#39;aggiornamento.
   * Seleziona la casella di controllo **Privato per la mia azienda** per mantenere l&#39;aggiornamento privato per gli utenti della tua azienda.

     >[!TIP]
     >
     >L&#39;impostazione **Privato per la mia società** è disponibile solo quando il tuo profilo Workfront è associato a una società.
1. Fai clic su **Salva**.

## Modificare un’attività nell’intestazione dell’attività (limitato)

È possibile modificare una quantità limitata di informazioni nell&#39;intestazione dell&#39;attività.

L&#39;amministratore del sistema o del gruppo può personalizzare i campi visualizzati nell&#39;intestazione dell&#39;attività. Per ulteriori informazioni, vedere [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).


![](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)

Per impostazione predefinita, nell&#39;intestazione dell&#39;attività sono inclusi i campi seguenti:

* Nome attività
* Percentuale completata

  Per informazioni, vedere [Visualizzare e aggiornare la percentuale di completamento per le attività](/help/quicksilver/manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).
* Assegnazioni
* Data di completamento Pianificata

  >[!CAUTION]
  >
  >Alcuni vincoli di attività e altre dipendenze potrebbero impedire la modifica della Data di completamento pianificata di un&#39;attività. Per informazioni sui vincoli attività, vedere [Panoramica sui vincoli attività](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Stato
* Prendere decisioni di approvazione se si è impostati come approvatore in un processo di approvazione corrente

## Modifica attività in blocco

È possibile modificare le attività in blocco in un elenco e aggiornarne tutte le informazioni contemporaneamente quando si seleziona di salvare automaticamente le modifiche apportate alle attività nell&#39;elenco.

Per informazioni sul salvataggio di attività in blocco, vedere la sezione &quot;Modifica attività in blocco&quot; nell&#39;articolo [Modifica attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).
