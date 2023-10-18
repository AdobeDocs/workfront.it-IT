---
product-area: projects
navigation-topic: manage-tasks
title: Sposta attività
description: In Adobe Workfront è possibile spostare le attività in progetti diversi o in diverse attività principali.
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '1479'
ht-degree: 2%

---

# Sposta attività

Puoi spostare le attività in Adobe Workfront tra i seguenti oggetti:

* Un’attività ad hoc per un progetto.
* Un&#39;attività da un progetto a un altro progetto.
* Un&#39;attività di un progetto con un padre diverso in un altro progetto.
* Un&#39;attività all&#39;interno dello stesso progetto sotto un padre diverso.

È possibile spostare un&#39;attività a livello di attività oppure da un elenco di attività.
È possibile spostare una singola attività oppure più attività contemporaneamente da un elenco di attività.

## Requisiti di accesso

Per eseguire le azioni descritte in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenze Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per le attività</p> <p>Autorizzazioni Contribute (Contribute) o superiori per il progetto con la possibilità di aggiungere attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront.

## Considerazioni sullo spostamento delle attività

Quando si sposta un&#39;attività, tenere presente quanto segue:

* Quando si sposta un&#39;attività da un progetto a un altro, è possibile che le date dell&#39;attività vengano ricalcolate. Il ricalcolo terrà conto della pianificazione utilizzata dal nuovo progetto e delle informazioni di Schedule From del progetto.

* È possibile scegliere di spostare alcuni elementi associati all&#39;attività nell&#39;attività spostata durante il processo di spostamento. Tuttavia, per impostazione predefinita, i seguenti oggetti vengono trasferiti all&#39;attività spostata:

   * Problemi
   * Ore registrate
   * Commenti utente
   * Moduli personalizzati e informazioni sui campi personalizzati
   * Sottoattività

Per impostazione predefinita, i seguenti elementi non si spostano con l’attività:

* Le Milestone

## Spostare le attività in un elenco

1. Passare al progetto contenente l&#39;attività o le attività che si desidera spostare.
1. Clic **Attività** nel pannello a sinistra per visualizzare l’elenco delle attività.
1. Fai clic su **Modalità pianificazione** icona ![](assets/plan-mode-icon.png) e garantire che **Salvataggio automatico** l&#39;opzione è attivata, quindi selezionare le attività che si desidera spostare.

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >Impossibile spostare le attività quando **Salvataggio automatico** l&#39;interruttore è disattivato.

1. (Facoltativo e condizionale) Se si desidera spostare le attività selezionate all&#39;interno dello stesso progetto, fare clic sulle attività selezionate, trascinarle e rilasciarle nella posizione in cui si desidera spostarle nel progetto.

   Dopo aver eliminato le attività nella posizione corretta sul progetto, le modifiche apportate alla gerarchia delle attività vengono salvate immediatamente. Tutte le informazioni associate a ogni attività vengono spostate insieme alle attività.

1. (Condizionale) Seleziona l’attività o le attività da spostare ed effettua una delle seguenti operazioni:

   * Fai clic su **Altro** menu ![](assets/qs-more-menu.png) nella parte superiore dell&#39;elenco delle attività, quindi fare clic su **Sposta in**.
   * Fare clic con il pulsante destro del mouse sulle attività selezionate, quindi scegliere **Sposta in**.
   * Quando si seleziona un&#39;attività, fare clic su **Altro** menu ![](assets/more-icon-task-list.png) accanto al nome dell&#39;attività nell&#39;elenco, quindi fare clic su **Sposta in**.

   ![](assets/move-task-in-list-nwe-350x119.png)

   Viene visualizzata la casella Sposta attività

1. Continua a spostare l’attività come descritto nella sezione [Spostare un&#39;attività a livello di attività](#move-a-task-at-the-task-level) in questo articolo, a partire dal passaggio 4.

   <!--
   is this still accurate?!
   -->

## Spostare un&#39;attività a livello di attività {#move-a-task-at-the-task-level}

Oltre a spostare le attività da un elenco di attività, è possibile spostare un&#39;attività anche a livello di attività dopo averla aperta.

1. Cercare un&#39;attività nel sistema Workfront.
1. Fare clic sul nome dell&#39;attività per aprirla.
1. Fai clic su **Altro** menu a discesa ![](assets/qs-more-menu.png) accanto al nome dell&#39;attività, quindi fare clic su **Sposta in**. Viene visualizzata la casella Sposta attività.

   ![](assets/move-task-at-task-level-nwe-350x222.png)

1. (Facoltativo) Aggiorna il **Nome attività**. L&#39;attività si sposta con il nuovo nome nella nuova posizione. Workfront non registra il nome originale dell’attività.

   >[!TIP]
   >
   >Il campo Nome attività è inattivo e non è modificabile quando si seleziona per spostare più attività in un elenco. È possibile passare il cursore del mouse sul campo Nome attività per visualizzare un elenco di tutte le attività selezionate.
   >
   >
   >![](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. Digita il nome del **Progetto di destinazione** nel punto in cui si desidera spostare l&#39;attività **Seleziona progetto di destinazione** campo.

   Se si desidera spostare l&#39;attività nello stesso progetto, digitare il nome del progetto corrente.

   >[!TIP]
   >
   >* Il nome del progetto distingue tra maiuscole e minuscole.
   >* Puoi anche iniziare a digitare il Numero di riferimento o immettere l’ID del progetto. Questo potrebbe aiutarti a distinguere i progetti con nomi identici.
   >* Nell’elenco vengono visualizzati solo 100 progetti.

1. (Condizionale) Fai clic su **Richiedi accesso** per richiedere l’accesso al progetto, se non hai accesso al progetto selezionato.
1. (Facoltativo) Se disponi dell’accesso per aggiungere attività a una delle attività del progetto di destinazione, continua a spostare l’attività al progetto di destinazione selezionato senza richiedere l’accesso.

   ![](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >Messaggi simili vengono visualizzati se il progetto selezionato è in attesa di approvazione, completato o inattivo, quando l’amministratore di Workfront impedisce l’aggiunta di attività a questi progetti. Per ulteriori informazioni, consulta [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Facoltativo) Fai clic su **Opzioni** nel pannello a sinistra

   Oppure

   Scorri verso il basso fino a **Opzioni** nella casella Sposta attività, quindi deselezionare gli elementi elencati nella tabella seguente per rimuoverli dalle attività spostate. Tutte le opzioni sono selezionate per impostazione predefinita.

   >[!IMPORTANT]
   >
   >Deselezionando gli elementi nell&#39;elenco Opzioni si verifica una perdita di dati. Le informazioni dell&#39;attività esistente verranno rimosse e non potranno essere recuperate.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Seleziona tutto</td> 
      <td>Deselezionate questa opzione per rimuovere tutte le informazioni dall'attività quando la spostate nella nuova posizione. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vincolo Data</td> 
      <td> <p>Il vincolo attività viene impostato su Il più presto possibile o Il più tardi possibile in base all'impostazione Modalità pianificazione del progetto.</p> <p> Se questa opzione è selezionata, il vincolo corrente dell'attività viene trasferito insieme all'attività. </p> 
      <p><b>NOTA</b>

   Quando si sposta o si copia un&#39;attività con vincoli specifici di data in un altro progetto e le date dei vincoli dell&#39;attività non rientrano nelle date del nuovo progetto, il vincolo dell&#39;attività viene modificato in Il più presto possibile o Il più tardi possibile oppure le date di Inizio pianificato o Completamento pianificato dei progetti vengono modificate.

   Di seguito sono riportati alcuni esempi di vincoli specifici per data:
   <ul>
      <li> Inizia il</li>
      <li> Deve Finire al</li>
      <li> Iniziare non Prima di</li>
      <li> Iniziare non Dopo di</li>
      </ul>

   Per informazioni sui vincoli delle attività e sul modo in cui possono essere influenzati i vincoli delle attività o le date del progetto, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sui vincoli delle attività</a> e cercare un vincolo specifico.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Assegnazioni</td> 
      <td> <p>Tutte le assegnazioni vengono rimosse dall'attività. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processo di approvazione</td> 
      <td>Tutti i processi di approvazione vengono rimossi dall'attività.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Avanzamento</td> 
      <td>Lo stato dell'attività è Nuovo. In caso contrario, lo stato dell'attività esistente viene mantenuto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informazioni finanziarie</td> 
      <td>Le informazioni finanziarie dell'attività vengono rimosse e Workfront aggiorna il tipo di costo dell'attività su Nessun costo e il tipo di ricavo dell'attività su Non fatturabile. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tutti i predecessori</td> 
      <td> <p>Se selezionata, la relazione diventa un predecessore di più progetti quando si sposta l'attività in un altro progetto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenti</td> 
      <td> <p>I documenti allegati all'attività non vengono trasferiti all'attività spostata. Sono inclusi versioni, bozze e documenti collegati.</p> <p>Non sono incluse le approvazioni di documenti. Le approvazioni dei documenti non possono mai essere spostate quando un'attività viene spostata.</p> 
      <b>NOTA</b>

   Se si sceglie di non spostare i documenti con l&#39;attività, i documenti verranno eliminati e posizionati nel Cestino per 30 giorni. Un amministratore può ripristinarli e verranno ripristinati durante l’attività spostata.

   Se l&#39;attività viene eliminata dopo essere stata spostata, i documenti ripristinati verranno posizionati nell&#39;area Documenti della pagina utente dell&#39;amministratore che li ripristina.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche promemoria</td> 
      <td>I promemoria dell'attività non vengono trasferiti all'attività spostata. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spese</td> 
      <td>Le spese registrate per l'attività non vengono trasferite all'attività spostata. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autorizzazioni</td> 
      <td> <p>Workfront rimuove i nomi di tutte le entità visualizzate nell'elenco Condivisione dell'attività. </p> </td> 
     </tr> 
    </tbody> 
   </table>



1. (Facoltativo) Fai clic su **Seleziona elemento padre** nel pannello a sinistra

   Oppure

   Scorri fino a **Seleziona elemento padre** , quindi selezionare nel progetto di destinazione l&#39;attività che si desidera diventare padre dell&#39;attività spostata.

   >[!TIP]
   >
   >Quando si seleziona per spostare più attività in un elenco, tutte le attività selezionate diventano gli elementi figlio dell&#39;elemento padre selezionato.

   Selezionare un elemento padre eseguendo una delle operazioni seguenti:

   * Nell&#39;elenco delle attività selezionare uno dei padri nel piano di progetto.
   * Fai clic sull’icona di ricerca ![Icona Ricerca](assets/search-icon.png) e cercare un&#39;attività padre per nome.

   L’attività viene visualizzata nell’elenco.

   ![Selezionare l&#39;attività padre quando si sposta un&#39;attività con funzionalità di ricerca ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Dopo averlo trovato, seleziona il pulsante di opzione relativo al genitore.

   Se non si seleziona un&#39;attività padre, le attività vengono spostate come attività principali anziché come attività secondarie e si trovano alla fine dell&#39;elenco delle attività nel progetto di destinazione.

1. Clic **Sposta attività**

   Oppure

   Clic **Sposta le attività** quando si selezionano più attività in un elenco.

   Le attività spostate si trovano ora nel progetto specificato e sono sottoattività di un&#39;attività padre o ultime attività del progetto.
