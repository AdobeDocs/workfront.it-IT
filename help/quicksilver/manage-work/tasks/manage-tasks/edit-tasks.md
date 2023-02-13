---
product-area: projects
navigation-topic: manage-tasks
title: Modifica delle attività
description: Modifica delle attività
author: Alina
feature: Work Management
exl-id: 572c6008-3a67-47ae-8f5d-6b871ef1f37b
source-git-commit: 9c7af82b02649f33728d05126587fb5035e9e110
workflow-type: tm+mt
source-wordcount: '3627'
ht-degree: 4%

---

# Modifica delle attività

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: some information in this area is repeated in the following articles. If you need to update a fied, update it in both:</p>
<p>** Task finances in details</p>
<p>** Task information in overview)</p>
</div>
-->


È possibile modificare le informazioni sulle attività create o su cui si dispone delle autorizzazioni di Contribute o Manage.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso*</td> 
   <td> <p>Modifica l’accesso a Attività e Progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> 
    <ul> 
     <li> <p>Autorizzazioni di Contribute per un'attività di modifica nell'area Dettagli attività </p> </li> 
     <li> <p>Gestire le autorizzazioni per un'attività per modificarla nella casella Modifica attività</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Contribuire o autorizzazioni superiori al progetto</p> </li> 
    </ul> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Limiti per la modifica delle attività

Sono presenti alcune limitazioni che potrebbero impedire la modifica delle attività.

Quando modifichi le attività, tieni presente quanto segue:

* L&#39;aggiornamento delle attività attiva le notifiche per i progetti con stato Corrente. Per evitare confusione per gli utenti assegnati alle attività, limita il più possibile le attività di modifica quando il progetto è nello stato corrente.
* Non è possibile modificare le attività in un processo di approvazione. È possibile registrare solo l&#39;ora o aggiornare lo stato di un&#39;attività in un processo di approvazione.

   ![](assets/edit-task-in-approval-process-nwe-350x148.png)

* È possibile modificare e aggiungere documenti alle attività di un progetto con stato Completato, Morto o In attesa di approvazione solo quando questa funzionalità è stata abilitata dall’amministratore di Workfront o da un amministratore di gruppo nell’area Preferenze progetto. Per informazioni sull&#39;impostazione delle preferenze del progetto, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* È sempre possibile modificare le seguenti informazioni su un&#39;attività quando il progetto è contrassegnato come Completo, Morto o in corso di approvazione:

   * Tempo di log
   * Modifica spese esistenti
   * Allegare un modulo personalizzato

## Modificare un’attività in un elenco

È possibile modificare le informazioni sulle attività in un elenco di attività, modificando i campi in linea visualizzati nella visualizzazione dell&#39;elenco.

Per informazioni sulle attività di modifica negli elenchi, consulta [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

## Modificare un’attività in un elenco utilizzando il Riepilogo

Puoi modificare un’attività in un elenco utilizzando il pannello Riepilogo . Per informazioni sulla modifica di un’attività nel pannello Riepilogo, consulta la sezione &quot;Modifica un’attività nel riepilogo&quot; nella sezione [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) articolo.

## Modificare un’attività nella casella Modifica attività

È possibile modificare un&#39;attività utilizzando le aree Modifica attività o Dettagli attività. I passaggi seguenti descrivono la modifica di un’attività nella casella Modifica attività.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Progetti**, quindi fai clic sul nome di un progetto per aprirlo.
1. Fai clic su **Attività** nel pannello a sinistra.
1. Fare clic sull&#39;attività da modificare.
1. (Facoltativo) Per modificare informazioni limitate su un’attività, fai clic su **Dettagli attività** nel pannello a sinistra.

   ![](assets/nwe-task-details-expanded-350x273.png)

   Prendi in considerazione la modifica delle informazioni nelle seguenti aree nella sezione Dettagli attività :

   * **Panoramica**

      Questa area viene espansa per impostazione predefinita.

   * **Moduli personalizzati**

      I nomi dei moduli doganali vengono visualizzati solo se all’oggetto sono associati moduli personalizzati.

   * **Finanz**
   >[!NOTE]
   >
   >A seconda del modo in cui l’amministratore di Workfront o di gruppo ha modificato il modello di layout, i campi nell’area Dettagli attività potrebbero essere ridisposti o non visualizzati. Per informazioni, consulta [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Per informazioni sui campi visibili nella sezione Dettagli attività,

   continuare a modificare l’attività nella casella Modifica attività come descritto di seguito.

   Per modificare le informazioni nella sezione Dettagli, procedi come segue:

   1. (Facoltativo) Fai clic sul pulsante **Comprimi tutto** icona ![](assets/collapse-all-icon.png) nell&#39;angolo in alto a destra per comprimere tutte le aree.
   1. (Facoltativo e condizionale) Quando un’area viene compressa, fai clic sul pulsante **freccia verso destra** ![](assets/right-pointing-arrow.png) accanto a ogni area per espandere l’area da modificare.
   1. Per ulteriori informazioni sulla modifica delle informazioni nella scheda Dettagli attività, vedere i seguenti articoli:

      * [Gestire le informazioni sulle attività nell&#39;area Panoramica dettagli attività](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)
      * [Gestire le finanze attività nella sezione Dettagli attività](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)
   1. (Facoltativo) Se non sono presenti moduli personalizzati collegati all’attività, inizia a digitare il nome di un modulo nella **Aggiungi modulo personalizzato** , quindi selezionalo quando viene visualizzato nell’elenco, quindi fai clic su **Salva modifiche**.
   1. (Facoltativo) Fai clic sul pulsante **Esporta** icona ![](assets/export.png) per esportare le informazioni generali e i moduli personalizzati in un file PDF, fai clic su **Esporta**. Seleziona una delle seguenti opzioni:

      * Seleziona tutto (viene visualizzato solo quando è presente almeno un modulo personalizzato allegato)
      * Panoramica
      * Nome di uno o più moduli personalizzati

      Il file PDF viene scaricato sul computer.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Per ulteriori informazioni, consulta [Esportare moduli personalizzati e dettagli dell’oggetto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).




1. Per modificare tutte le informazioni sull’attività, fai clic sul pulsante **Altro** menu ![](assets/more-icon.png) accanto al nome dell’attività, quindi fai clic su **Modifica**.

   Oppure

   Da un elenco di attività, seleziona un’attività, quindi fai clic sul pulsante **Modifica** icona ![](assets/edit-icon.png) in cima all&#39;elenco.

   Viene visualizzata la casella Modifica attività.

   >[!IMPORTANT]
   >
   >Per visualizzare l’opzione Modifica, è necessario disporre delle autorizzazioni di gestione per l’attività.

   Tutti i campi attività sono disponibili nella casella Modifica attività e sono raggruppati in base alle aree elencate nel pannello a sinistra.

   >[!NOTE]
   >
   >A seconda del modo in cui l’amministratore di Workfront o di gruppo ha modificato il modello di layout, i campi nell’area Dettagli attività potrebbero essere ridisposti o non visualizzati. Per informazioni, consulta [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   È consigliabile specificare le informazioni in una delle sezioni seguenti:

   * [Nome attività](#task-name)
   * [Panoramica](#overview)
   * [Assegnazioni](#assignments)
   * [Moduli personalizzati](#Custom%C2%A0F)
   * [Finanz](#finance)
   * [Impostazioni](#settings)

   >[!NOTE]
   >
   >A seconda della modalità di configurazione del modello di layout da parte dell’amministratore di Workfront o dell’amministratore di gruppo, i campi della casella Modifica attività potrebbero essere ridisposti o non visualizzati. Per informazioni, consulta [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### Nome attività {#task-name}

1. Inizia a modificare l’attività come descritto sopra.
1. Fai clic su **Nome attività** nel pannello a sinistra.

   ![](assets/nwe-task-name-section-edit-task-box-350x122.png)

1. Aggiorna il nome dell&#39;attività.

1. Fai clic su **Salva** o continuare con le sezioni seguenti.

### Panoramica {#overview}

1. Inizia a modificare l’attività come descritto sopra.
1. Fai clic su **Panoramica** nel pannello a sinistra.

   ![](assets/nwe-overview-section-edit-task-box-350x257.png)

1. Aggiorna le seguenti informazioni sull&#39;attività:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td>Aggiungi ulteriori informazioni sull’attività. </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Sezione Informazioni di base</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stato</td> 
      <td> <p>Selezionare lo stato dell'attività che indica lo stato di sviluppo dell'attività.</p> <p><b>SUGGERIMENTO</b>

   È possibile aggiornare lo stato dell&#39;attività nell&#39;intestazione dell&#39;attività. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Priorità</td> 
      <td> <p>Questo è un flag visivo che ti consente di assegnare priorità alle attività. </p> <p>Seleziona tra le seguenti opzioni: </p> 
       <ul> 
      <li> <p> Nessuno</p> </li> 
      <li> <p> Basso </p> </li> 
      <li> <p>Normal </p> </li> 
      <li> <p>Alta </p> </li> 
      <li> <p> Urgente </p> </li> 
       </ul> <p>A seconda delle preferenze del progetto selezionate dall’amministratore di Workfront, i nomi delle priorità potrebbero essere diversi. Per informazioni sulle priorità delle attività, consulta <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">Aggiorna priorità attività</a>. </p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Sezione Date attività e vincoli</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vincolo attività</td> 
      <td> <p>Decidere quando l'attività deve essere completata specificando un Vincolo di attività. </p> <p>Seleziona tra le seguenti opzioni: </p> 
       <ul> 
      <li> <p><span>Dati Fissi</span> </p> <p>Specifica una <strong>Inizio pianificato</strong> e <strong>Data completamento pianificata</strong>. </p> </li> 
      <li> <p><span>Deve ininziare al</span> </p> <p>Specifica una <strong>Data di inizio prevista</strong>. </p> </li> 
      <li> <p><span>Deve Finire al</span> </p> <p>Specifica una <strong>Data completamento pianificata</strong>. </p> </li> 
       </ul> 
       <ul> 
      <li> <p><span>Il più presto possibile</span></p> </li> 
      <li> <p><span>Il più tardi possibile</span></p> </li> 
      <li> <p><span>Primo Orario Disponibile</span></p> </li> 
      <li> <p> <span>Ultimo Orario Disponibile</span></p> </li> 
      <li> <p><span>Iniziare non Dopo di</span> </p> </li> 
      <li> <p>Specificare una data di inizio pianificata</p> </li> 
      <li> <p><span>Iniziare non Prima di</span> </p> <p>Specifica una <strong>Data di inizio prevista</strong>. </p> </li> 
      <li> <p> Fine <span>Entro</span></p> <p>Specifica una <strong>Data completamento pianificata</strong>. </p> </li> 
      <li> <p> Fine <span>Non precedente a</span></p> <p>Specifica una <strong>Data completamento pianificata</strong></p> </li> 
       </ul> <p>Per ulteriori informazioni sul vincolo di attività, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sul vincolo di attività</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora dell’impegno</td> 
      <td> <p>Data in cui l’utente assegnato all’attività si impegna a completare l’attività. Può essere diverso dalla data di completamento pianificata. Solo gli assegnatari possono modificare questo campo. Per informazioni sulle date di commit in Workfront, vedi <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Panoramica sulla data del commit</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora di inizio pianificate</td> 
      <td> <p>Quando è pianificato l'avvio dell'attività. La data di inizio pianificata di un'attività viene impostata e influenzata da una serie di fattori:</p> 
       <ul> 
      <li>A seconda delle preferenze a livello di sistema per la data di inizio pianificata dell'attività, la data di inizio di una nuova attività su un progetto può essere oggi o la data di inizio del progetto, per impostazione predefinita. <span>Anche l’amministratore del gruppo associato al progetto può impostare questa preferenza per il gruppo.</span> Per ulteriori informazioni sulle preferenze delle attività a livello di sistema o di gruppo, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configurare le preferenze relative alle attività e ai problemi a livello di sistema</a>.</li> 
      <li>A seconda dei predecessori dell’attività, la data di inizio pianificata viene selezionata da Workfront come la data successiva disponibile dopo il termine dei predecessori, oppure come data di inizio, a seconda della relazione predecessore. Per ulteriori informazioni sulle relazioni predecessori, vedi <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Panoramica dei predecessori delle attività</a>.</li> 
      <li>Il project manager o il proprietario dell'attività possono impostare manualmente la data di inizio pianificata quando il vincolo dell'attività è Fisse date o Deve iniziare su. Per ulteriori informazioni sui vincoli delle attività, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sul vincolo di attività</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora del completamento pianificati</td> 
      <td> <p>Data di completamento prevista, come mostrato al momento della pianificazione dell'attività. La data di completamento prevista può essere impostata da una serie di fattori:</p> 
       <ul> 
      <li>La data di completamento pianificata viene calcolata a partire dalla data di inizio pianificata aggiungendo la Durata dell'attività alla data di inizio pianificata. Quando il project manager o Workfront specifica la durata dell'attività, viene attivato un aggiornamento alla data di completamento pianificata. Se la data pianificata cambia, spesso accade perché è stata aggiornata la Durata del .</li> 
      <li>Il project manager o il proprietario dell'attività possono impostare manualmente la data di completamento pianificato quando il vincolo dell'attività è Fisse date o Deve terminare su. Per ulteriori informazioni sui vincoli delle attività, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sul vincolo di attività</a>.</li> 
      <li>Se il tipo di durata dell'attività cambia e il numero di risorse sulle attività cambia contemporaneamente, cambia anche la data di completamento pianificata. Per ulteriori informazioni sui tipi di durata, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica del tipo di durata e durata dell’attività</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora di inizio effettive</td> 
      <td> <p>Specificare una data di inizio effettiva per l'attività. Il valore predefinito viene generalmente compilato automaticamente quando lo stato dell'attività viene modificato in In corso. La data di inizio effettiva può anche essere modificata manualmente dal project manager o dal proprietario dell'attività. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data e ora del completamento effettivo</td> 
      <td> <p>Specificare la data e l'ora effettive al completamento dell'attività. La data e l'ora predefinite in cui un'attività viene completata coincide sempre con l'ora effettiva in cui lo stato viene completato. La data di completamento effettiva può anche essere modificata manualmente dal project manager o dal proprietario dell'attività. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>Sezione sull'orario di lavoro</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Impegno di lavoro </td> 
      <td>

   <p>L'entità dello sforzo necessario per completare l'attività. Il project manager potrebbe decidere di utilizzare questo campo invece di Orari pianificati per stimare lo sforzo necessario per completare un'attività. Questo campo è visibile solo quando sono soddisfatte le seguenti condizioni:</p> 
      <ul> 
      <li> <p>L'attività ha un tipo di durata semplice. </p> <p><b>SUGGERIMENTO</b>

   Se si modifica il tipo di durata dell&#39;attività, questo campo viene oscurato. </p> </li>
   <li>Il project manager ha abilitato il campo Use Work Ffort per calcolare automaticamente l'attività Orari pianificati sul progetto. </li> 
      </ul> 
      <p>Seleziona tra le seguenti opzioni:</p> 
      <ul> 
      <li>Piccolo</li> 
      <li>Media <span style="font-weight: normal;">(valore predefinito per una nuova attività)</span></li> 
      <li>Grande</li> 
      </ul> 
      <p><b>NOTA</b>

   L&#39;aggiornamento della quantità di sforzo potrebbe aggiornare l&#39;attività Orari pianificati. L&#39;aggiornamento è immediato se il tipo di aggiornamento del progetto è Automatico. Quando il tipo di aggiornamento del progetto è Manuale, è necessario ricalcolare la timeline per visualizzare l’orario pianificato aggiornato. </p>

   <p>Per informazioni sull'utilizzo dello sforzo di lavoro anziché dell'orario pianificato per stimare lo sforzo dell'attività, vedere <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Panoramica sullo sforzo di lavoro</a>. </p> 
    </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva** o continuare con le sezioni seguenti.

### Assegnazioni {#assignments}

1. Inizia a modificare l’attività come descritto sopra.
1. Fai clic su **Assegnazioni** nel pannello a sinistra.

   ![](assets/nwe-assignments-section-edit-task-box-350x217.png)

1. Fai clic su **Cercare persone, ruoli e team** e iniziare a digitare il nome di un utente, ruolo o team che si desidera assegnare all&#39;attività, quindi fare clic su di essa o premere Invio quando viene visualizzato nell&#39;elenco.

   >[!NOTE]
   >
   >Se il nome dell’utente contiene un carattere speciale, è necessario includere il carattere speciale nel campo di ricerca.

   >[!TIP]
   >
   >È possibile assegnare più utenti, ruoli o team. È possibile assegnare solo utenti attivi, ruoli e team.
   >
   >Se un utente, un ruolo di lavoro o un team è stato assegnato prima della disattivazione, rimangono assegnati all&#39;elemento di lavoro. In questo caso, si consiglia quanto segue:
   >
   >* Riassegna l&#39;elemento di lavoro alle risorse attive.
   >* Associare gli utenti di un team disattivato a un team attivo e riassegnare l&#39;elemento di lavoro al team attivo.


1. (Facoltativo) Indicare se un assegnatario è l&#39;assegnatario principale dell&#39;attività, selezionando la **Proprietario** pulsante di scelta accanto al nome. Un team non può essere l&#39;assegnatario principale di un&#39;attività.
1. (Condizionale e facoltativo) Aggiorna i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipo di Durata</td> 
      <td> <p>Questo identifica la relazione tra i seguenti elementi: </p> 
       <ul> 
      <li> <p>Numero di risorse assegnate a un'attività </p> </li> 
      <li> <p>Sforzo totale necessario per completare l'attività </p> </li> 
      <li> <p> Durata totale dell'attività. </p> </li> 
       </ul> <p>Amministratore Workfront <span> o un amministratore di gruppo</span> seleziona l'impostazione predefinita Tipo di durata per le attività nel sistema o nel gruppo. Per informazioni sull’impostazione dei valori predefiniti del progetto, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze del progetto a livello di sistema</a>. </p> <p>I tipi di durata consentono di impostare assegnazioni di risorse coerenti in base alle esigenze dell'attività. Per ulteriori informazioni sul tipo di durata di un'attività, vedere <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica del tipo di durata e durata dell’attività</a>. </p> <p>Seleziona tra le seguenti opzioni: </p> 
       <ul> 
      <li> <p>Incarico Calcolato </p> </li> 
      <li> <p> Lavoro Calcolato </p> </li> 
      <li> <p>Impegno Aggiuntivo </p> </li> 
      <li> <p>Semplice</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Durata per Occorrenza</td> 
      <td> <p>Viene visualizzato solo sull'elemento padre delle attività ricorrenti. Visualizza la durata di ogni attività ricorrente. Per informazioni sulla creazione di attività ricorrenti, consulta <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Creare attività ricorrenti</a>. </p> <p> <b>NOTA</b>

   Le durate modificate in singole attività ricorrenti non presentano il valore indicato in questo campo. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Durata</td> 
      <td> 
      <div> 
      <div> 
      <p>Questo è il tempo necessario per consentire a un'attività di rimanere aperta prima del completamento. </p> 
      <p><b>IMPORTANTE</b>

   Poiché la durata dell’attività corrisponde in genere alla quantità di tempo tra l’inizio pianificato e le date di completamento pianificato, influisce sulla timeline del progetto.</p>

   <p>Per indicare la Durata dell'attività e l'unità di tempo, eseguire le operazioni seguenti:</p> 
      <ul> 
      <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Digita il periodo di tempo e seleziona dal menu a discesa le unità di tempo disponibili.</p> <p><b>SUGGERIMENTO</b></p>
      Quando si aggiorna la Durata delle attività in un elenco di attività, è possibile utilizzare l'abbreviazione per l'unità di tempo. </p> </li> 
      </ul> 
      <p> Puoi scegliere tra le opzioni relative al tempo regolare o al tempo trascorso nella tabella seguente: </p> 
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
      <td>Giorni. Questa è l’impostazione predefinita. </td> 
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

   <p>Il tempo trascorso è un'unità di tempo per la durata di un'attività. È l'intervallo tra la data di inizio pianificata e la data di completamento pianificata di un'attività che include le festività, i fine settimana e l'ora di inattività. In altre parole, il tempo trascorso è il passaggio dei giorni di calendario.

   L&#39;ora regolare prende in considerazione le festività, i fine settimana e l&#39;ora di riposo e li esclude dalla Durata dell&#39;attività. Per ulteriori informazioni sulla durata dell&#39;attività, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica del tipo di durata e durata dell’attività</a>. </p>
   </div> 
   </div> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Lavoro Necessario</td> 
   <td> <p>Specifica la quantità di ore pianificate per l'attività, in ore. Questo è il tempo effettivo necessario agli assegnatari dell'attività per completarla. È possibile specificare solo la quantità di ore pianificate per un'attività quando il tipo di durata è impostato su Assegnazione calcolata. Per ulteriori informazioni sui tipi di durata, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica del tipo di durata e durata dell’attività</a>.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Allocazione</td> 
   <td> <p>Se il Vincolo attività è Calcolato Lavoro o Sforzo guidato, specificare il <strong>% allocazione</strong> (percentuale di assegnazione) per ciascun assegnatario. Indica la quantità di tempo dalla pianificazione dell'assegnatario che possono trascorrere per questa attività. La modifica della percentuale di allocazione per un assegnatario modificherà le ore pianificate di un'attività. </p> <p>Quando il vincolo di attività è semplice, è possibile specificare quanto segue:</p> 
      <ul> 
      <li> <p>Orari di allocazione di ciascun assegnatario.</p> </li> 
      <li> <p>Orario pianificato dell’attività</p> </li> 
      <li> <p>Durata dell'attività</p> </li> 
      </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Mansione dell'assegnatario</td> 
   <td> <p>Seleziona un ruolo dal <strong>Ruolo dell'assegnatario</strong> menu a discesa quando hai selezionato una persona come assegnatario. Questo è il ruolo che l'assegnatario può svolgere su questo compito. </p> <p><b>SUGGERIMENTO</b>

   Nel menu a discesa vengono visualizzati solo i ruoli di lavoro associati a ciascun assegnatario nel proprio profilo.</p> </td>
   </tr> 
      </tbody> 
      </table>

1. Fai clic su **Salva** o continuare con le sezioni seguenti.

### Moduli personalizzati

È possibile definire moduli personalizzati predefiniti da associare automaticamente alle attività quando le attività vengono aggiunte a un progetto. Per informazioni sull&#39;impostazione del progetto per includere moduli personalizzati delle attività predefiniti per tutte le nuove attività, vedere la sezione &quot;Attività&quot; nell&#39;articolo [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Inizia a modificare l’attività come descritto sopra.
1. Fai clic su **Forms personalizzato** nel pannello a sinistra, oppure fare clic sul nome di un modulo personalizzato, se è già allegato.

   ![](assets/nwe-custom-forms-section-edit-task-box-350x127.png)

1. Fai clic su **Aggiungi modulo personalizzato** selezionare il modulo o i moduli personalizzati che si desidera associare all&#39;attività. È necessario creare i moduli personalizzati prima che siano disponibili per la selezione in questo campo. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi.

   Per ulteriori informazioni sulla creazione di moduli personalizzati, vedere [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)È possibile aggiungere fino a dieci moduli personalizzati a un’attività.

1. (Condizionale) Se all’attività è stato allegato un modulo personalizzato, è necessario modificare tutti i campi del modulo. È necessario specificare tutti i campi obbligatori prima di salvare l’attività.

   >[!NOTE]
   >
   >A seconda di come l’amministratore di Workfront ha impostato le autorizzazioni per le sezioni del modulo personalizzato, non tutti possono visualizzare o modificare gli stessi campi in un determinato modulo personalizzato. Le autorizzazioni per modificare i campi all’interno di una sezione di un modulo personalizzato dipendono dalle autorizzazioni disponibili per l’attività stessa. Per informazioni sull&#39;impostazione delle autorizzazioni per le attività, consulta [Condividere un’attività](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

1. Fai clic su **Salva** o continuare con le sezioni seguenti.

### Finanz {#finance}

1. Inizia a modificare l’attività come descritto in [Modifica delle attività](#Edit2) in questo articolo.
1. Fai clic su **Finanza** nel pannello a sinistra.

   ![](assets/nwe-finance-section-edit-task-box-350x298.png)

1. Aggiorna i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipo Cst</td> 
      <td> <p>Specificare il tipo di costo per l'attività. Questo determinerà il calcolo del costo dell'attività, in base al numero di ore relative alle attività. </p> <p>Seleziona tra le seguenti opzioni: </p> 
       <ul> 
        <li> <p>Nessun Costo</p> </li> 
        <li> <p>Ore Fisse </p> </li> 
        <li> <p> Ore Utente </p> </li> 
        <li> <p> Ore Ruolo</p> </li> 
       </ul> <p>Per ulteriori informazioni sui costi di tracciamento, vedi <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Costi di tracciamento</a> . L'amministratore di Workfront o un amministratore di gruppo seleziona l'impostazione predefinita Tipo di costo per le attività nel sistema o nel gruppo. Per informazioni sull’impostazione dei valori predefiniti del progetto, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze del progetto a livello di sistema</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di Reddito</td> 
      <td> <p>Specifica il tipo di ricavi per l'attività. Questo determinerà il modo in cui vengono calcolati i Ricavi sull'attività, in base al numero di ore sulle attività. </p> <p>Seleziona tra le seguenti opzioni: </p> 
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
       </ul> <p>Per ulteriori informazioni sul tracciamento dei ricavi, vedi<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Panoramica di fatturazione e ricavi</a> . </p> <p>L'amministratore di Workfront o l'amministratore di gruppo seleziona l'impostazione Tipo di ricavi predefinito per le attività nel sistema o nel gruppo. Per informazioni sull’impostazione dei valori predefiniti del progetto, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurare le preferenze del progetto a livello di sistema</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva** oppure continua con la sezione seguente.

### Impostazioni {#settings}

1. Inizia a modificare l’attività come descritto in [Modifica delle attività](#Edit2) in questo articolo.
1. Fai clic su **Impostazioni** nel pannello a sinistra.

   ![](assets/nwe-settings-section-edit-task-box-350x304.png)

1. Aggiorna i campi seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Modalità Tracciamento</td> 
      <td> <p>Specificare il modo in cui viene tracciato lo stato di avanzamento dell’attività. </p> <p>Seleziona tra le seguenti opzioni: </p> 
       <ul> 
      <li> <p> Utente deve Aggiornare </p> </li> 
      <li> <p>Presupponi in tempo </p> </li> 
      <li> <p>Ignora Avvertimenti di Ritardo</p> </li> 
      <li> <p> Autocompletamento </p> </li> 
      <li> <p>Predecessore </p> </li> 
       </ul> <p>Per ulteriori informazioni sulla modalità di tracciamento delle attività, consulta <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Panoramica sulla modalità di tracciamento delle attività</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Livellamento Risorse</td> 
      <td> <p>Seleziona la <strong>Escludi dal livellamento delle risorse</strong> se si desidera escludere dal livellamento le risorse assegnate all'attività.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ritardo di Livellamento</td> 
      <td> <p>Specificare il ritardo di livellamento in ore. </p> <p> Per ulteriori informazioni sui ritardi di livellamento, vedi <a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">Aggiorna ritardo livellamento attività</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processo di approvazione</td> 
      <td> <p>Selezionare un processo di approvazione da associare all'attività. Prima di poter essere associati alle attività, l'amministratore di Workfront deve definire i processi di approvazione a livello di sistema. Un utente con accesso amministrativo ai processi di approvazione può anche creare processi di approvazione specifici per gruppo. </p> <p>Per ulteriori informazioni sulla creazione dei processi di approvazione, consulta <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md">Creazione di un processo di approvazione per gli elementi di lavoro</a>. Quando si aggiungono processi di approvazione, considera quanto segue: </p> 
       <ul>

   <li> <p>Nell’elenco vengono visualizzati solo i processi di approvazione attivi. </p> </li>

   <li> <p>Nell'elenco vengono visualizzati i processi di approvazione a livello di sistema e di gruppo. Un processo di approvazione associato a un gruppo diverso da quello del progetto non viene visualizzato nell’elenco. </p>

   <p><b>IMPORTANTE</b>

   Se il gruppo del progetto viene modificato, il processo di approvazione specifico del gruppo precedentemente allegato diventa un processo di approvazione a uso singolo. Per ulteriori informazioni su come le modifiche apportate al gruppo del progetto o al processo di approvazione influiscono sulle impostazioni di approvazione, vedere <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">Effetti delle modifiche al processo di approvazione e di gruppo sui processi di approvazione assegnati</a>. </p>

   </li>

   <li> <p>È possibile definire processi di approvazione predefiniti da associare automaticamente alle attività quando le attività vengono aggiunte a un progetto. Per informazioni sull'impostazione del progetto per includere i processi di approvazione delle attività predefiniti, vedere la sezione "Attività" nell'articolo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Modifica progetti</a>. </p> </li>

   <li> <p>Quando si eseguono attività di modifica in serie, si verificano i seguenti scenari: </p> 
      <ul> 
      <li> <p>Quando si selezionano più attività dallo stesso gruppo, in questo campo vengono visualizzati sia i processi di approvazione a livello di sistema che quelli a livello di gruppo. </p> </li> 
      <li> <p>Quando si selezionano più attività da gruppi diversi, in questo campo vengono visualizzati solo i processi di approvazione a livello di sistema. </p> </li> 
      <li> <p>Quando una delle attività presenta un processo di approvazione a uso singolo, viene sostituita dal processo di approvazione a livello di sistema o di gruppo selezionato. </p> </li>

   </ul> </li> 
      </ul> </td> 
     </tr> 
    </tbody> 
   </table>
    </li>

1. Fai clic su **Salva**.

<!--notes from the table: <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)</p>       -->

## Modificare un&#39;attività nell&#39;intestazione dell&#39;attività (limitata)

È possibile modificare una quantità limitata di informazioni nell&#39;intestazione dell&#39;attività.

L’amministratore di sistema o di gruppo può personalizzare i campi visualizzati nell’intestazione dell’attività. Per ulteriori informazioni, consulta [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).


![](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)

Per impostazione predefinita, nell’intestazione del progetto sono inclusi i campi seguenti:

* Nome attività
* Percentuale completata
* Assegnazioni
* Data e ora del completamento pianificati

   >[!CAUTION]
   >
   >Alcuni vincoli di attività e altre dipendenze potrebbero impedire la modifica di questo campo. Per informazioni sui vincoli di attività, vedere [Panoramica sul vincolo di attività](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Stato
* Prendere decisioni di approvazione se si è impostati come approvatore in un processo di approvazione corrente

## Modifica in blocco le attività

È possibile modificare le attività in blocco in un elenco e aggiornare tutte le relative informazioni contemporaneamente quando si seleziona per salvare automaticamente le modifiche apportate alle attività nell&#39;elenco.

Per informazioni sul salvataggio in blocco delle attività, consulta la sezione &quot;Modifica attività in blocco&quot; nell’articolo [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).
