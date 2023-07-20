---
product-area: projects
navigation-topic: manage-tasks
title: Modifica attività
description: Potete modificare le informazioni sulle attività create o sulle quali disponete delle autorizzazioni Contribute o Manage.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 572c6008-3a67-47ae-8f5d-6b871ef1f37b
source-git-commit: 4a4efe7d8a354bc9ec22a607fe6e75040e7cca24
workflow-type: tm+mt
source-wordcount: '3711'
ht-degree: 4%

---

# Modifica attività

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: some information in this area is repeated in the following articles. If you need to update a fied, update it in both:</p>
<p>** Task finances in details</p>
<p>** Task information in overview)</p>
</div>
-->


Potete modificare le informazioni sulle attività create o sulle quali disponete delle autorizzazioni Contribute o Manage.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> 
    <ul> 
     <li> <p>Concedere le autorizzazioni per un'attività per modificarla nell'area Dettagli attività </p> </li> 
     <li> <p>Gestire le autorizzazioni per un'attività per modificarla nella casella Modifica attività</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Autorizzazioni Contribute (Contribute) o superiori per il progetto</p> </li> 
    </ul> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Limitazioni per la modifica delle attività

Esistono alcune limitazioni che potrebbero impedire la modifica delle attività.

Quando modifichi le attività, tieni presente quanto segue:

* L’aggiornamento delle attività attiva le notifiche per i progetti che si trovano nello stato Corrente. Per evitare confusione per gli utenti assegnati alle attività, limita il più possibile le attività di modifica quando il progetto è nello stato Corrente.
* Non è possibile modificare le attività in un processo di approvazione. È possibile registrare solo l&#39;ora o aggiornare lo stato di un&#39;attività in un processo di approvazione.

  ![](assets/edit-task-in-approval-process-nwe-350x148.png)

* È possibile modificare e aggiungere documenti alle attività di un progetto con stato Completato, Inattivo o In attesa di approvazione solo quando l&#39;amministratore di Workfront o un amministratore di gruppo ha abilitato questa funzionalità nell&#39;area Preferenze progetto. Per informazioni sull&#39;impostazione delle preferenze di progetto, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* È sempre possibile modificare le informazioni seguenti su un&#39;attività quando il progetto è stato contrassegnato come Completo, Inattivo o si trova in un processo di approvazione:

   * Tempo di connessione
   * Modifica spese esistenti
   * Allegare un modulo personalizzato

## Modificare un’attività in un elenco

È possibile modificare le informazioni sulle attività in un elenco di attività modificando i campi in linea visualizzati nella visualizzazione dell&#39;elenco.

Per informazioni sulla modifica delle attività negli elenchi, vedere [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

## Modificare un&#39;attività in un elenco utilizzando il Riepilogo

Potete modificare un&#39;attività in un elenco utilizzando il pannello Riepilogo. Per informazioni sulla modifica di un&#39;attività nel pannello Riepilogo, consultate la sezione &quot;Modifica un&#39;attività nel Riepilogo&quot; nel [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) articolo.

## Modificare un&#39;attività nella casella Modifica attività

È possibile modificare un&#39;attività utilizzando le aree Modifica attività o Dettagli attività. Nei passaggi seguenti viene descritta la modifica di un&#39;attività nella casella Modifica attività.

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront.

1. Clic **Progetti**, quindi fai clic sul nome di un progetto per aprirlo.
1. Clic **Attività** nel pannello a sinistra.
1. Fare clic sull&#39;attività da modificare.
1. (Condizionale) Per modificare informazioni limitate su un’attività, in qualità di utente con autorizzazioni Contribute (Contribuisci), fai clic su **Dettagli Attività** nel pannello a sinistra.

   ![](assets/nwe-task-details-expanded-350x273.png)

   È consigliabile modificare le informazioni nelle aree seguenti della sezione Dettagli attività:

   * **Panoramica**

     L&#39;area viene espansa per impostazione predefinita.

   * **Moduli personalizzati**

     I nomi dei moduli doganali vengono visualizzati solo se all’oggetto sono allegati moduli personalizzati.

   * **Finanz**

   >[!NOTE]
   >
   >A seconda della modalità di modifica del modello di layout da parte dell&#39;amministratore di Workfront o del gruppo, i campi nell&#39;area Dettagli attività potrebbero essere ridisposti o non visualizzati. Per informazioni, consulta [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Per informazioni sui campi visibili nella sezione Dettagli attività, continuare a modificare l&#39;attività nella casella Modifica attività come descritto di seguito.

   Per modificare le informazioni nella sezione Dettagli, effettuare le seguenti operazioni:

   1. (Facoltativo) Fai clic su **Comprimi tutto** icona ![](assets/collapse-all-icon.png) nell&#39;angolo superiore destro per comprimere tutte le aree.
   1. (Facoltativo e condizionale) Quando un&#39;area è compressa, fare clic sul pulsante **freccia rivolta verso destra** ![](assets/right-pointing-arrow.png) accanto a ogni area per espandere l&#39;area da modificare.
   1. Per ulteriori informazioni sulla modifica delle informazioni nella scheda Dettagli attività, vedere gli articoli seguenti:

      * [Gestire le informazioni sull&#39;attività nell&#39;area Panoramica dettagli attività](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)
      * [Gestire i dati finanziari delle attività nella sezione Dettagli attività](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)

   1. (Facoltativo) Se non sono presenti moduli personalizzati allegati all’attività, inizia a digitare il nome di un modulo nel campo **Aggiungi modulo personalizzato** , quindi selezionarlo quando viene visualizzato nell&#39;elenco, quindi fare clic su **Salva modifiche**.
   1. (Facoltativo) Fai clic su **Esporta** icona ![](assets/export.png) per esportare le informazioni sulla panoramica e sui moduli personalizzati in un file PDF, fai clic su **Esporta**. Selezionare una delle opzioni seguenti:

      * Seleziona tutto (viene visualizzato solo se è allegato almeno un modulo personalizzato)
      * Panoramica
      * Nome di uno o più moduli personalizzati

      Il file PDF viene scaricato nel computer.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Per ulteriori informazioni, consulta [Esportare moduli personalizzati e dettagli oggetto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

1. (Condizionale) Per modificare tutte le informazioni sull’attività, in qualità di utente con autorizzazioni di gestione per l’attività, fai clic su **Altro** menu ![](assets/more-icon.png) accanto al nome dell&#39;attività, quindi fare clic su **Modifica**.

   Oppure

   In un elenco di attività, selezionare un&#39;attività, quindi fare clic sul pulsante **Modifica** icona ![](assets/edit-icon.png) nella parte superiore dell’elenco.

   Viene visualizzata la casella Modifica task (Edit Task).

   >[!IMPORTANT]
   >
   >Per visualizzare l&#39;opzione Modifica, è necessario disporre delle autorizzazioni di gestione per l&#39;attività.

   Tutti i campi delle attività sono disponibili nella casella Modifica attività e sono raggruppati per le aree elencate nel pannello a sinistra.

   >[!NOTE]
   >
   >A seconda della modalità di modifica del modello di layout da parte dell&#39;amministratore di Workfront o del gruppo, i campi nell&#39;area Dettagli attività potrebbero essere ridisposti o non visualizzati. Per informazioni, consulta [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Prendere in considerazione la possibilità di specificare informazioni in una delle sezioni seguenti:

   * [Nome attività](#task-name)
   * [Panoramica](#overview)
   * [Assegnazioni](#assignments)
   * [Moduli personalizzati](#Custom%C2%A0F)
   * [Finanz](#finance)
   * [Impostazioni](#settings)

   >[!NOTE]
   >
   >A seconda del modo in cui l&#39;amministratore di Workfront o il gruppo imposta il modello di layout, i campi nella casella Modifica attività potrebbero essere ridisposti o non visualizzati. Per informazioni, consulta [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### Nome attività {#task-name}

1. Inizia a modificare l’attività come descritto in precedenza.
1. Clic **Nome attività** nel pannello a sinistra.

   ![](assets/nwe-task-name-section-edit-task-box-350x122.png)

1. Aggiorna il nome dell&#39;attività.

1. Clic **Salva** oppure continuare con le sezioni seguenti.

### Panoramica {#overview}

1. Inizia a modificare l’attività come descritto in precedenza.
1. Clic **Panoramica** nel pannello a sinistra.

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
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Sezione Informazioni di base</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stato</td> 
      <td> <p>Selezionare lo stato dell'attività che indica la fase di sviluppo in cui si trova l'attività.</p> <p><b>SUGGERIMENTO</b>

   È possibile aggiornare lo Stato dell&#39;attività nell&#39;intestazione dell&#39;attività. </p> </td>
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
       </ul> <p>A seconda delle Preferenze di progetto selezionate dall'amministratore di Workfront, i nomi delle priorità potrebbero essere diversi. Per informazioni sulle priorità delle attività, vedere <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">Aggiorna Priorità Attività</a>. </p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Sezione Date attività e vincoli</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vincolo attività</td> 
      <td> <p>Decidere quando l'attività deve essere completata specificando un vincolo attività. </p> <p>Selezionare una delle opzioni seguenti: </p> 
       <ul> 
      <li> <p><span>Dati Fissi</span> </p> <p>Specifica un <strong>Inizio pianificato</strong> e un <strong>Data di completamento Pianificata</strong>. </p> </li> 
      <li> <p><span>Deve ininziare al</span> </p> <p>Specifica un <strong>Data Inizio Pianificata</strong>. </p> </li> 
      <li> <p><span>Deve Finire al</span> </p> <p>Specifica un <strong>Data di completamento Pianificata</strong>. </p> </li> 
       </ul> 
       <ul> 
      <li> <p><span>Il prima possibile</span></p> </li> 
      <li> <p><span>Più tardi possibile</span></p> </li> 
      <li> <p><span>Primo Orario Disponibile</span></p> </li> 
      <li> <p> <span>Ultimo Orario Disponibile</span></p> </li> 
      <li> <p><span>Iniziare non Dopo di</span> </p> </li> 
      <li> <p>Specifica una data di inizio pianificata</p> </li> 
      <li> <p><span>Iniziare non Prima di</span> </p> <p>Specifica un <strong>Data Inizio Pianificata</strong>. </p> </li> 
      <li> <p> Fine <span>Non oltre il</span></p> <p>Specifica un <strong>Data di completamento Pianificata</strong>. </p> </li> 
      <li> <p> Fine <span>Non Prima Di</span></p> <p>Specifica un <strong>Data di completamento Pianificata</strong></p> </li> 
       </ul> <p>Per ulteriori informazioni su Vincolo attività, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sui vincoli delle attività</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Conferma data e ora</td> 
      <td> <p>Si tratta della data entro la quale l’utente assegnato all’attività si impegna a completarla. Può essere diverso dalla Data di completamento pianificata. Solo gli assegnatari possono modificare questo campo. Per informazioni sulle date di conferma in Workfront, consulta <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Panoramica sulla data di conferma</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora di inizio pianificate</td> 
      <td> <p>Quando è pianificato l’inizio dell’attività. La data di inizio pianificata di un'attività viene impostata e influenzata da diversi fattori:</p> 
       <ul> 
      <li>A seconda della preferenza a livello di sistema per la data di inizio pianificata dell'attività, la data di inizio di una nuova attività in un progetto può essere la data odierna o la data di inizio del progetto, per impostazione predefinita. <span>Anche l’amministratore del gruppo associato al progetto può impostare questa preferenza per il gruppo.</span> Per ulteriori informazioni sulle preferenze per le attività a livello di sistema o di gruppo, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configurare le preferenze per attività e problemi a livello di sistema</a>.</li> 
      <li>A seconda dei predecessori dell'attività, la data di inizio pianificata viene scelta da Workfront come data disponibile successiva alla fine o all'inizio del predecessore, a seconda della relazione del predecessore. Per ulteriori informazioni sulle relazioni predecessori, vedere <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Panoramica dei predecessori delle attività</a>.</li> 
      <li>Il project manager o il proprietario dell'attività possono impostare manualmente la data di inizio pianificata quando il vincolo dell'attività è Date fisse o Deve iniziare il. Per ulteriori informazioni sui vincoli delle attività, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sui vincoli delle attività</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora di completamento pianificate</td> 
      <td> <p>Data di completamento prevista, come visualizzata quando l'attività è pianificata. La data di completamento pianificata può essere impostata da diversi fattori:</p> 
       <ul> 
      <li>La data di completamento pianificata viene calcolata a partire dalla data di inizio pianificata aggiungendo la Durata dell'attività alla data di inizio pianificata. Quando il project manager o Workfront specifica la durata dell'attività, viene attivato un aggiornamento della data di completamento pianificata. Se la data pianificata cambia, spesso sarà perché la Durata del è stata aggiornata.</li> 
      <li>Il project manager o il proprietario dell'attività possono impostare manualmente la data di completamento pianificata quando il vincolo dell'attività è Date fisse o Deve finire il. Per ulteriori informazioni sui vincoli delle attività, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sui vincoli delle attività</a>.</li> 
      <li>Se il Tipo di Durata dell'attività cambia e il numero di risorse sulle attività cambia contemporaneamente, cambierà anche la data di completamento pianificata. Per ulteriori informazioni sui tipi di durata, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica sulla durata e sul tipo di durata dell'attività</a>.</li> 
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
      <li>Piccolo</li> 
      <li>Medio <span style="font-weight: normal;">(valore predefinito per una nuova attività)</span></li> 
      <li>Grande</li> 
      </ul> 
      <p><b>NOTA</b>

   L&#39;aggiornamento della quantità di lavoro potrebbe aggiornare le ore pianificate dell&#39;attività. L&#39;aggiornamento è immediato se il tipo di aggiornamento del progetto è Automatico. Quando il tipo di aggiornamento del progetto è Manuale, è necessario ricalcolare la sequenza temporale per visualizzare le ore pianificate aggiornate. </p>

   <p>Per informazioni sull'utilizzo dell'Impegno di lavoro invece delle Ore pianificate per stimare l'impegno dell'attività, vedere <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Panoramica sull’impegno di lavoro</a>. </p> 
    </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Salva** oppure continuare con le sezioni seguenti.

### Assegnazioni {#assignments}

1. Inizia a modificare l’attività come descritto in precedenza.
1. Clic **Assegnazioni** nel pannello a sinistra.

   ![](assets/nwe-assignments-section-edit-task-box-350x217.png)

1. Clic **Cerca persone, ruolo e team** e iniziare a digitare il nome di un utente, ruolo o team che si desidera assegnare all&#39;attività, quindi fare clic su di esso o premere Invio quando viene visualizzato nell&#39;elenco.

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

1. (Facoltativo) Indicare se l&#39;assegnatario è l&#39;assegnatario principale dell&#39;attività selezionando la **Proprietario** accanto al nome. Un team non può essere l&#39;assegnatario principale di un&#39;attività.
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
       </ul> <p>Il tuo amministratore Workfront <span> o un amministratore di gruppo</span> seleziona l’impostazione predefinita Tipo di durata per le attività nel sistema o nel gruppo. Per informazioni sull'impostazione delle impostazioni predefinite del progetto, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze di progetto a livello di sistema</a>. </p> <p>I tipi di durata consentono di impostare assegnazioni di risorse coerenti in base alle esigenze dell'attività. Per ulteriori informazioni sul Tipo di durata di un'attività, vedere <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica sulla durata e sul tipo di durata dell'attività</a>. </p> <p>Selezionare una delle opzioni seguenti: </p> 
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
      <td>Minuti</td> 
      <td>M</td> 
      </tr> 
      <tr> 
      <td>Ore</td> 
      <td>H</td> 
      </tr> 
      <tr> 
      <td>Giorni. Questa è l'impostazione predefinita. </td> 
      <td>Dsbld</td> 
      </tr> 
      <tr> 
      <td>Settimane</td> 
      <td>M</td> 
      </tr> 
      <tr> 
      <td>Mesi</td> 
      <td>G</td> 
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
   <td> <p>Specifica la quantità di ore pianificate per l'attività, in ore. Quantità di tempo effettivo necessario agli assegnatari per completare l'attività. È possibile specificare la quantità di ore pianificate per un'attività solo quando il tipo di durata è impostato su Assegnazione calcolata. Per ulteriori informazioni sui tipi di durata, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica sulla durata e sul tipo di durata dell'attività</a>.</p> 
   <b>NOTA</b>
   <p>
   Quando si creano attività ricorrenti, le ore pianificate sono quelle di ogni occorrenza. Le ore pianificate delle attività padre sono il totale di tutte le ore pianificate di tutte le occorrenze. Per informazioni sulla creazione di attività ricorrenti, vedere <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Creare attività ricorrenti</a>.
   </p>

   </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Allocazione</td> 
   <td> <p>Se il vincolo attività è Lavoro calcolato o Basato sulle risorse, specificare <strong>% allocazione</strong> (percentuale di allocazione) per ogni assegnatario. Quantità di tempo della pianificazione dell'assegnatario che può trascorrere per l'attività. Se si modifica la percentuale di allocazione per un assegnatario, verranno modificate le ore pianificate di un'attività. </p> <p>Quando Vincolo attività è Semplice, è possibile specificare quanto segue:</p> 
      <ul> 
      <li> <p>Ore di allocazione di ciascun assegnatario.</p> </li> 
      <li> <p>Ore pianificate dell'attività</p> </li> 
      <li> <p>Durata dell’attività</p> </li> 
      </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Mansione dell'assegnatario</td> 
   <td> <p>Seleziona un ruolo dal <strong>Ruolo dell'assegnatario</strong> menu a discesa quando hai selezionato una persona come assegnatario. Questo è il ruolo che l’assegnatario può svolgere per questa attività. </p> <p><b>SUGGERIMENTO</b>

   Nel menu a discesa vengono visualizzati solo i ruoli associati a ciascun assegnatario nel relativo profilo.</p> </td>
   </tr> 
      </tbody> 
      </table>

1. Clic **Salva** oppure continuare con le sezioni seguenti.

### Moduli personalizzati

È possibile definire moduli personalizzati predefiniti da allegare automaticamente alle attività quando queste vengono aggiunte a un progetto. Per informazioni sulla configurazione del progetto per includere moduli personalizzati predefiniti per tutte le nuove attività, vedere la sezione &quot;Attività&quot; nell&#39;articolo [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Inizia a modificare l’attività come descritto in precedenza.
1. Clic **Forms personalizzato** nel pannello a sinistra, oppure fai clic sul nome di un modulo personalizzato, se è già allegato.

   ![](assets/nwe-custom-forms-section-edit-task-box-350x127.png)

1. Clic **Aggiungi modulo personalizzato** e selezionare il modulo o i moduli personalizzati che si desidera associare all&#39;attività. Devi creare i moduli personalizzati prima che siano disponibili per la selezione in questo campo. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi.

   Per ulteriori informazioni sulla creazione di moduli personalizzati, consulta [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).È possibile aggiungere fino a dieci moduli personalizzati a un&#39;attività.

1. (Condizionale) Se hai allegato un modulo personalizzato all’attività, modifica eventuali campi del modulo. È necessario specificare tutti i campi obbligatori prima di salvare l&#39;attività.

   >[!NOTE]
   >
   >A seconda di come l’amministratore di Workfront imposta le autorizzazioni per le sezioni nel modulo personalizzato, non tutti possono visualizzare o modificare gli stessi campi in un determinato modulo personalizzato. Le autorizzazioni per modificare i campi all’interno di una sezione di un modulo personalizzato dipendono dalle autorizzazioni di cui disponi per l’attività stessa. Per informazioni sull&#39;impostazione delle autorizzazioni per le attività, vedere [Condividere un’attività](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

1. Clic **Salva** oppure continuare con le sezioni seguenti.

### Finanz {#finance}

1. Inizia a modificare l&#39;attività come descritto in [Modifica attività](#Edit2) in questo articolo.
1. Clic **Finanza** nel pannello a sinistra.

   ![](assets/nwe-finance-section-edit-task-box-350x298.png)

1. Aggiorna i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipo Cst</td> 
      <td> <p>Specificare il tipo di costo per l'attività. Questo determinerà come viene calcolato il costo dell'attività, in base al numero di ore sulle attività. </p> <p>Selezionare una delle opzioni seguenti: </p> 
       <ul> 
        <li> <p>Nessun Costo</p> </li> 
        <li> <p>Ore Fisse </p> </li> 
        <li> <p> Ore Utente </p> </li> 
        <li> <p> Ore Ruolo</p> </li> 
       </ul> <p>Per ulteriori informazioni sul tracciamento dei costi, consulta <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tracciare i costi</a> . L'amministratore di Workfront o un amministratore di gruppo seleziona l'impostazione Tipo di costo predefinita per le attività del sistema o del gruppo. Per informazioni sull'impostazione delle impostazioni predefinite del progetto, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze di progetto a livello di sistema</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di Reddito</td> 
      <td> <p>Specificare il tipo di retribuzione per l'attività. Questo determinerà il modo in cui vengono calcolati i Ricavi sull'attività, in base al numero di ore sulle attività. </p> <p>Selezionare una delle opzioni seguenti: </p> 
       <ul> 
      <li> <p> Non Fatturabile </p> </li> 
      <li> <p>Ore Utente </p> </li> 
      <li> <p>Ore Ruolo </p> </li> 
      <li> <p>Ore Fisse </p> </li> 
      <li> <p>Ore Utente w/Cap </p> </li> 
      <li> <p>Ore Ruolo w/Cap </p> </li> 
      <li> <p>Ore Utente più Fisso </p> </li> 
      <li> <p>Ore Ruolo più Fisso </p> </li> 
      <li> <p>Reddito Fisso </p> </li> 
       </ul> <p>Per ulteriori informazioni sul tracciamento dei ricavi, consulta<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica su fatturazione e ricavi</a> . </p> <p>L'amministratore di Workfront o l'amministratore di gruppo seleziona l'impostazione Tipo di retribuzione predefinita per le attività del sistema o del gruppo. Per informazioni sull'impostazione delle impostazioni predefinite del progetto, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze di progetto a livello di sistema</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **Salva** oppure continuare con la sezione seguente.

### Impostazioni {#settings}

1. Inizia a modificare l&#39;attività come descritto in [Modifica attività](#Edit2) in questo articolo.
1. Clic **Impostazioni** nel pannello a sinistra.

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
       </ul> <p>Per ulteriori informazioni sulla modalità di tracciamento delle attività, consulta <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Panoramica sulla modalità di monitoraggio attività</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Livellamento Risorse</td> 
      <td> <p>Seleziona la <strong>Escludi dal livellamento risorse</strong> se si desidera escludere dal livellamento le risorse assegnate all'attività.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ritardo di Livellamento</td> 
      <td> <p>Specifica il ritardo di livellamento, in ore. </p> <p> Per ulteriori informazioni sul livellamento dei ritardi, consulta <a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">Ritardo livellamento attività di aggiornamento</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processo di approvazione</td> 
      <td> <p>Selezionare un processo di approvazione da associare all'attività. Prima di poter associare i processi alle attività, l'amministratore di Workfront deve definirli a livello di sistema. Un utente con accesso amministrativo ai processi di approvazione può anche creare processi di approvazione specifici per il gruppo. </p> <p>Per ulteriori informazioni sulla creazione di processi di approvazione, vedere <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md">Creare un processo di approvazione per gli elementi di lavoro</a>. Quando aggiungi processi di approvazione, tieni presente quanto segue: </p> 
       <ul>

   <li> <p>Nell'elenco vengono visualizzati solo i processi di approvazione attivi. </p> </li>

   <li> <p>I processi di approvazione a livello di sistema e di gruppo vengono visualizzati nell’elenco. Un processo di approvazione associato a un gruppo diverso da quello del progetto non viene visualizzato nell’elenco. </p>

   <p><b>IMPORTANTE</b>

   Se il gruppo del progetto cambia, il processo di approvazione specifico del gruppo precedentemente allegato diventa un processo di approvazione a utente singolo. Per ulteriori informazioni su come le modifiche al gruppo del progetto o le modifiche nel processo di approvazione influiscono sulle impostazioni di approvazione, vedi <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">Effetti delle modifiche al gruppo e al processo di approvazione sui processi di approvazione assegnati</a>. </p>

   </li>

   <li> <p>È possibile definire processi di approvazione predefiniti da allegare automaticamente alle attività quando queste vengono aggiunte a un progetto. Per informazioni sulla configurazione del progetto per includere i processi di approvazione delle attività predefiniti, vedere la sezione "Attività" nell'articolo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Modifica progetti</a>. </p> </li>

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

1. Fai clic su **Salva**.

<!--notes from the table: <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)</p>       -->

## Modificare un’attività nell’intestazione dell’attività (limitato)

È possibile modificare una quantità limitata di informazioni nell&#39;intestazione dell&#39;attività.

L&#39;amministratore del sistema o del gruppo può personalizzare i campi visualizzati nell&#39;intestazione dell&#39;attività. Per ulteriori informazioni, consulta [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).


![](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)

Per impostazione predefinita, nell’intestazione del progetto sono inclusi i seguenti campi:

* Nome attività
* Percentuale completata
* Assegnazioni
* Data e ora di completamento pianificate

  >[!CAUTION]
  >
  >Alcuni vincoli di attività e altre dipendenze potrebbero impedire la modifica di questo campo. Per informazioni sui vincoli delle attività, vedere [Panoramica sui vincoli delle attività](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Stato
* Prendere decisioni di approvazione se si è impostati come approvatore in un processo di approvazione corrente

## Modifica attività in blocco

È possibile modificare le attività in blocco in un elenco e aggiornarne tutte le informazioni contemporaneamente quando si seleziona di salvare automaticamente le modifiche apportate alle attività nell&#39;elenco.

Per informazioni sul salvataggio di attività in blocco, vedere la sezione &quot;Modifica attività in blocco&quot; nell&#39;articolo [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).
