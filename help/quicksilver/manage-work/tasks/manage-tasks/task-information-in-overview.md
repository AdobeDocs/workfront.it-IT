---
product-area: projects
navigation-topic: manage-tasks
title: Gestire le informazioni sull'attività nell'area Panoramica dettagli attività
description: Gestire le informazioni sull'attività nell'area Panoramica dettagli attività
author: Alina
feature: Work Management
exl-id: 4980b28f-914d-4cf9-813f-14983aac660b
source-git-commit: 5b7a5aff0f8bdf7cf8429ac29b50c3beaf4bd3b4
workflow-type: tm+mt
source-wordcount: '2089'
ht-degree: 5%

---

# Gestire le informazioni sull&#39;attività nell&#39;area Panoramica dettagli attività

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, do it in both articles)</p>
-->

È possibile visualizzare o modificare le informazioni di un&#39;attività accedendo all&#39;area Panoramica della sezione Dettagli attività . In quest’area è disponibile un numero limitato di campi che è possibile visualizzare o modificare. Per informazioni sulla modifica di tutte le informazioni relative a un&#39;attività, vedere [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

In questo articolo viene descritto come visualizzare o modificare le informazioni nell&#39;area Panoramica di Dettagli task. Per informazioni sull&#39;aggiornamento di altre aree di Dettagli attività, vedere i seguenti articoli:

* [Gestire i dati finanziari delle attività nella sezione Dettagli attività](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)
* [Aggiungere un modulo personalizzato a un oggetto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)
* [Gestire i moduli personalizzati allegati agli oggetti](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md)

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
   *Per informazioni sulla pianificazione, il tipo di licenza o l'accesso disponibili, contattare l'amministratore Workfront. 
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront<b> piano*</b> </p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront<b> licenza*</b> </p> </td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurazioni del livello di accesso*</strong> </td> 
   <td> <p>Accesso di visualizzazione o superiore ai progetti e alle attività</p> <p>Se disponi del livello di accesso corretto ma non riesci ancora a modificare la sezione Dettagli dell’attività, chiedi all’Adobe Workfront se ha impostato restrizioni aggiuntive nel livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Autorizzazioni Contribute o superiori per il progetto</p> <p>Visualizzare le autorizzazioni per l'attività per visualizzare le informazioni nella sezione Dettagli. </p> 
   <p>Autorizzazioni di Contribute per l'attività per aggiornare le seguenti informazioni nella sezione Dettagli:</p>

<ul>
   <li>Descrizione</li>
   <li>Stato</li>
   </ul>

<p>Gestisci le autorizzazioni per l'attività per aggiornare tutte le informazioni nella sezione Dettagli.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modificare le informazioni sull&#39;attività nella sezione Panoramica dei dettagli attività

1. Passare a un&#39;attività che si desidera visualizzare o modificare.
1. Clic **Dettagli Attività** nel pannello a sinistra .
1. Vai a **Panoramica** per visualizzare ulteriori informazioni sull&#39;attività.

   Per impostazione predefinita, Panoramica è la prima area della sezione Dettagli attività ed è espansa.

   >[!NOTE]
   >
   >A seconda del modo in cui l’amministratore di Workfront o il gruppo imposta il modello di layout, i campi nella sezione Dettagli attività potrebbero essere ridisposti o non visualizzati. Per informazioni, consulta [Personalizzare la visualizzazione Dettagli utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Fai clic su **Modifica** icona ![](assets/edit-icon.png) nell’angolo superiore destro della sezione Dettagli, quindi fai clic su **Panoramica**.

   >[!TIP]
   >
   >Non puoi modificare i campi generati automaticamente da Workfront o per i quali non disponi delle autorizzazioni necessarie.

1. Modificare qualsiasi campo disponibile per la modifica facendo clic sul campo o facendo clic su **+Aggiungi** per aggiungere informazioni a un campo vuoto.
1. Visualizzare o modificare uno dei campi elencati di seguito.

   Impossibile modificare tutti i campi.  

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descrizione</td> 
      <td> <p>Informazioni aggiuntive sull'attività</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Numero di riferimento</td> 
      <td>Si tratta di un valore univoco per l'attività generata da Workfront per tutti gli oggetti del sistema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>Gli utenti con i permessi Manage (Gestione) di un’attività possono specificare un collegamento a una pagina interna o esterna in questo campo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stato</td> 
      <td> <p>Selezionare lo stato dell'attività che indica la fase di sviluppo in cui si trova l'attività.</p> <p>Suggerimento: è possibile aggiornare lo stato dell'attività nell'intestazione dell'attività. </p> </td> 
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
     <tr> 
      <td role="rowheader">Durata</td> 
      <td> 
       <div> 
        <div> 
         <p>Quantità di tempo che consente a un'attività di rimanere aperta prima del completamento. </p> 
         <p>Importante: poiché la durata dell'attività corrisponde in genere al periodo di tempo che intercorre tra l'inizio pianificato e le date di completamento pianificate, influisce sulla sequenza temporale del progetto.</p> 
         <p>Per indicare la durata dell'attività e l'unità di tempo, eseguire le operazioni seguenti:</p> 
         <ul> 
          <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Digita il periodo di tempo e seleziona una delle unità di tempo disponibili nel menu a discesa.</p> </li> </ul>

   <p><strong>SUGGERIMENTO</strong></p> <p> Quando si aggiorna la Durata delle attività in un elenco di attività, è possibile utilizzare l'abbreviazione per l'unità di tempo. </p>      <p> Nella tabella seguente è possibile scegliere tra le opzioni relative al tempo normale o al tempo trascorso: </p> 
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
         <p><strong>NOTA</strong> </p>
         <p> Il tempo trascorso è un'unità di tempo per la durata di un'attività. Si tratta del tempo che intercorre tra la Data inizio pianificata e la Data completamento pianificata di un'attività e che include ferie, fine settimana e ferie. In altre parole, il tempo trascorso è il trascorrere dei giorni di calendario. L'orario regolare prende in considerazione le festività, i fine settimana e le ferie e le esclude dalla Durata dell'attività. Per ulteriori informazioni sulla durata dell'attività, vedere <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica sulla durata e sul tipo di durata dell'attività</a>. </p> 
         <p> 
         <!--You cannot specify the Duration of a task when the Duration Type of the task is Simple, or when the Task Constraint is Fixed Dates. (NOTE: Anna said this is now possible for all duration types in the Assignments area. It's not here, but to clear confusion, I am drafting this out of here.)--></p> 
        </div> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Durata prevista</td> 
      <td> <p>Differenza in giorni tra la data di inizio prevista e la data di completamento prevista. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Durata effettiva</td> 
      <td> <p>Differenza in giorni tra la data di inizio effettiva e la data di completamento effettiva. Questo è quanto tempo ci è voluto per completare il lavoro. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ore pianificate</td> 
      <td> <p>Specifica la quantità di ore pianificate per l'attività, in ore. Quantità di tempo effettivo necessario agli assegnatari per completare l'attività. È possibile specificare la quantità di ore pianificate per un'attività solo quando il tipo di durata è impostato su Assegnazione calcolata. Per ulteriori informazioni sui tipi di durata, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica sulla durata e sul tipo di durata dell'attività</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ore effettive</td> 
      <td>Le ore registrate dagli utenti sull'attività. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Impegno di lavoro </td> 
      <td> 
       <div> 
        <p>Quantità di lavoro necessaria per completare l'attività. È possibile che il project manager decida di utilizzare questo campo anziché le ore pianificate per stimare lo sforzo necessario per completare un'attività. Questo campo è visibile solo quando sono soddisfatte le seguenti condizioni:</p> 
        <ul> 
         <li> <p>L’attività ha un tipo di durata semplice. </p> <p>Suggerimento: se si modifica il tipo di durata dell'attività, questo campo viene oscurato. </p> </li> 
         <li>Il project manager ha abilitato il campo Usa impegno di lavoro per calcolare automaticamente le ore pianificate dell'attività nel progetto. </li> 
        </ul> 
        <p>Selezionare una delle opzioni seguenti:</p> 
        <ul> 
         <li>Piccolo</li> 
         <li>Medio <span style="font-weight: normal;">(valore predefinito per una nuova attività)</span></li> 
         <li>Grande</li> 
        </ul> 
        <p><strong>NOTA</strong></p> 
        <p> L'aggiornamento della quantità di lavoro potrebbe aggiornare le ore pianificate dell'attività. L'aggiornamento è immediato se il tipo di aggiornamento del progetto è Automatico. Quando il tipo di aggiornamento del progetto è Manuale, è necessario ricalcolare la sequenza temporale per visualizzare le ore pianificate aggiornate. </p> 
        <p>Per informazioni sull'utilizzo dell'Impegno di lavoro invece delle Ore pianificate per stimare l'impegno dell'attività, vedere <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Panoramica sull’impegno di lavoro</a>. </p> 
       </div> </td> 
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
      <td role="rowheader">Data di inizio pianificata</td> 
      <td> <p>Quando è pianificato l’inizio dell’attività. La data di inizio pianificata di un'attività viene impostata e influenzata da diversi fattori:</p> 
       <ul> 
        <li>A seconda della preferenza a livello di sistema per la data di inizio pianificata dell'attività, la data di inizio di una nuova attività in un progetto può essere la data odierna o la data di inizio del progetto, per impostazione predefinita. <span>Anche l’amministratore del gruppo associato al progetto può impostare questa preferenza per il gruppo.</span> Per ulteriori informazioni sulle preferenze per le attività a livello di sistema o di gruppo, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configurare le preferenze per attività e problemi a livello di sistema</a>.</li> 
        <li>A seconda dei predecessori dell'attività, la data di inizio pianificata viene scelta da Workfront come data disponibile successiva alla fine o all'inizio del predecessore, a seconda della relazione del predecessore. Per ulteriori informazioni sulle relazioni predecessori, vedere <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Panoramica dei predecessori delle attività</a>.</li> 
        <li>Il project manager o il proprietario dell'attività possono impostare manualmente la data di inizio pianificata quando il vincolo dell'attività è Date fisse o Deve iniziare il. Per ulteriori informazioni sui vincoli delle attività, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sui vincoli delle attività</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data di inizio prevista</td> 
      <td> <p>La data di inizio effettiva dell'attività in base all'avanzamento e al completamento delle attività precedenti. Questo è un campo calcolato e non puoi modificarlo manualmente.</p> <p> La data di inizio prevista e la data di inizio pianificata iniziano con la stessa, quando un progetto è pianificato per la prima volta. La data di inizio prevista può essere spostata dall'inizio pianificato se il progetto si evolve e l'attività non è ancora stata avviata. Per ulteriori informazioni sulle date di inizio previste, consulta <a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">Panoramica della data di inizio prevista del progetto</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data d'Inizio Reale</td> 
      <td> <p>Specificare una data di inizio effettiva per l'attività. Il valore predefinito viene generalmente popolato automaticamente quando si modifica lo stato dell'attività in In corso. La data di inizio effettiva può anche essere modificata manualmente dal project manager o dal proprietario dell'attività. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data di completamento Pianificata</td> 
      <td> <p>Data di completamento prevista, come visualizzata quando l'attività è pianificata. La data di completamento pianificata può essere impostata da diversi fattori:</p> 
       <ul> 
        <li>La data di completamento pianificata viene calcolata a partire dalla data di inizio pianificata aggiungendo la Durata dell'attività alla data di inizio pianificata. Quando il project manager o Workfront specifica la durata dell'attività, viene attivato un aggiornamento della data di completamento pianificata. Se la data pianificata cambia, spesso sarà perché la Durata del è stata aggiornata.</li> 
        <li>Il project manager o il proprietario dell'attività possono impostare manualmente la data di completamento pianificata quando il vincolo dell'attività è Date fisse o Deve finire il. Per ulteriori informazioni sui vincoli delle attività, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sui vincoli delle attività</a>.</li> 
        <li>Se il Tipo di Durata dell'attività cambia e il numero di risorse sulle attività cambia contemporaneamente, cambierà anche la data di completamento pianificata. Per ulteriori informazioni sui tipi di durata, consulta <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Panoramica sulla durata e sul tipo di durata dell'attività</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data di completamento Previsto</td> 
      <td> <p>La data "reale" di completamento dell'attività in base all'avanzamento delle attività precedenti e agli aggiornamenti di avanzamento dell'attività da parte dell'assegnatario. Questo è un campo calcolato e non puoi modificarlo manualmente.</p> <p> La data di completamento prevista e la data di completamento pianificata iniziano con lo stesso valore, quando un progetto viene pianificato per la prima volta. Se il progetto si evolve e l'attività non è ancora stata avviata, la data di completamento prevista può essere spostata dal completamento pianificato. Per ulteriori informazioni sulle date di completamento previste, consulta <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Panoramica della data di completamento prevista per progetti, attività e problemi</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data di completamento effettiva</td> 
      <td> <p>Specificare la data e l'ora effettive di completamento dell'attività. La data e l'ora predefinite di completamento di un'attività coincidono sempre con l'ora effettiva in cui lo stato diventa Completato. Il project manager o il proprietario dell'attività può inoltre modificare manualmente la data di completamento effettiva. </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Conferma data</td> 
      <td> <p>Si tratta della data entro la quale l’utente assegnato all’attività si impegna a completarla. Può essere diverso dalla Data di completamento pianificata. Solo gli assegnatari possono modificare questo campo. Per informazioni sulle date di conferma in Workfront, consulta <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Panoramica sulla data di conferma</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Data inserimento</td> 
      <td>Data di creazione dell'attività.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Immesso da</td> 
      <td>Persona che ha creato l’attività.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Data ultimo aggiornamento</td> 
      <td> <p>Data dell'ultimo aggiornamento dell'attività. </p> <p>Suggerimento: Workfront registra una data aggiornata ogni volta che un utente modifica e salva un'attività.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ultimo aggiornamento di</td> 
      <td> <p>Persona che ha aggiornato per ultima l’attività.</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Frequenza ricorrenza</td> 
      <td> <p>Viene visualizzato solo sull'elemento padre delle attività ricorrenti. Frequenza con cui si verificano le attività nella ricorrenza. Per informazioni sulla creazione di attività ricorrenti, vedere <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Creare attività ricorrenti</a>. </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Durata per Occorrenza</td> 
      <td> <p>Viene visualizzato solo sull'elemento padre delle attività ricorrenti. Viene visualizzata la durata di ogni attività ricorrente. Per informazioni sulla creazione di attività ricorrenti, vedere <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Creare attività ricorrenti</a>. </p> <p><strong>NOTA</strong></p> <p> Le durate modificate in singole attività ricorrenti non visualizzano il valore indicato in questo campo. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted, to keep it focused JUST on the Overview section and not others.) </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Custom Forms</strong> to add or forms or edit information on the existing custom forms.&nbsp;</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Expand any of the existing custom forms to edit them, or start typing in the <strong>Add custom form</strong> box in the upper-right corner to add a new form. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about adding or editing custom forms, see the following articles:</p>
   -->

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md" class="MCXref xref">Add a custom form to an object</a> </li>   
     -->

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md" class="MCXref xref">Manage custom forms attached to objects</a> </li>   
     -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click&nbsp;<strong>Finance</strong>, then <strong>Edit Finance</strong> to view or edit financial information for the task. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Expand the <strong>Finance</strong> area in the Details section, then double-click any editable field to update it. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about editing financial information for a task, see <a href="../../../manage-work/tasks/manage-tasks/task-finances-in-details.md" class="MCXref xref">Manage task finances in the Task Details section</a>. </p>
   -->

1. Clic **Salva modifiche**.
