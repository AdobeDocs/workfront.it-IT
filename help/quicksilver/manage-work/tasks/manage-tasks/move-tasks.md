---
product-area: projects
navigation-topic: manage-tasks
title: Sposta le Attività
description: In Adobe Workfront è possibile spostare le attività in progetti diversi o in diverse attività principali.
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 2%

---

# Sposta attività

<!--Audited: 5/2025-->


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


Puoi spostare le attività in Adobe Workfront tra i seguenti oggetti:

* Un’attività ad hoc per un progetto.
* Un&#39;attività da un progetto a un altro progetto.
* Un&#39;attività di un progetto con un padre diverso in un altro progetto.
* Un&#39;attività all&#39;interno dello stesso progetto sotto un padre diverso.

È possibile spostare un&#39;attività a livello di attività oppure da un elenco di attività.

È possibile spostare una singola attività oppure spostare più attività contemporaneamente da un elenco di attività.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Nuovo: Standard </p> 
 <p>oppure</p>  
<p>Corrente: Lavoro o versione successiva </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per le attività</p> <p>Autorizzazioni Contribute (Contribute) o superiori per il progetto con la possibilità di aggiungere attività</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sullo spostamento delle attività

Quando si sposta un&#39;attività, tenere presente quanto segue:

* L&#39;amministratore di sistema o di gruppo può impedire lo spostamento di attività con ore registrate a seconda della modalità di configurazione della preferenza Consenti agli utenti di spostare attività e problemi con ore registrate nell&#39;area Configura. Per informazioni, consulta [Configurare le preferenze per attività e problemi a livello di sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Quando si sposta un&#39;attività da un progetto a un altro, è possibile che le date dell&#39;attività vengano ricalcolate. Il ricalcolo terrà conto della pianificazione utilizzata dal nuovo progetto e delle informazioni di Schedule From del progetto.

* È possibile spostare alcuni elementi associati all&#39;attività nell&#39;attività spostata durante il processo di spostamento. Tuttavia, per impostazione predefinita, i seguenti oggetti vengono trasferiti all&#39;attività spostata:

   * Problemi
   * Ore registrate
   * Commenti utente
   * Moduli personalizzati e informazioni sui campi personalizzati
   * Sottoattività

* Per impostazione predefinita, i seguenti elementi non vengono spostati con l&#39;attività:

   * Le Milestone

## Spostare le attività in un elenco

{{step1-to-projects}}

1. Nella pagina **Progetti** selezionare il progetto contenente l&#39;attività o le attività che si desidera spostare.
1. Fai clic su **Attività** nel pannello a sinistra per visualizzare l&#39;elenco delle attività.
1. Fai clic sull&#39;icona **Modalità pianificazione** ![Icona Modalità pianificazione](assets/plan-mode.png) e accertati che l&#39;interruttore **Salvataggio automatico** sia abilitato, quindi seleziona l&#39;attività o le attività che desideri spostare.

   ![Opzione salvataggio automatico](assets/autosave-icon.png)

   >[!IMPORTANT]
   >
   >Impossibile spostare le attività quando l&#39;opzione **Salvataggio automatico** è disabilitata.

1. (Facoltativo e condizionale) Se si desidera spostare le attività selezionate all&#39;interno dello stesso progetto, fare clic sulle attività selezionate, quindi trascinarle nella posizione in cui si desidera spostarle nel progetto. Le modifiche apportate alla gerarchia delle attività vengono salvate immediatamente e le informazioni associate a ogni attività vengono spostate insieme alle attività.

1. (Condizionale) Seleziona l’attività o le attività da spostare ed effettua una delle seguenti operazioni:

   * Fai clic sul menu **Altro** ![Icona Altro](assets/main-more-icon.png) nella parte superiore dell&#39;elenco delle attività, quindi fai clic su **Sposta in**.
   * Fare clic con il pulsante destro del mouse sulle attività selezionate, quindi scegliere **Sposta in**.
   * Quando selezioni un&#39;attività, fai clic sul menu **Altro** ![](assets/more-icon-task-list.png) accanto al nome dell&#39;attività nell&#39;elenco, quindi fai clic su **Sposta in**.

   Viene visualizzata la casella **Sposta attività**.

1. Continuare con lo spostamento dell&#39;attività, come descritto nella sezione [Spostare un&#39;attività a livello di attività](#move-a-task-at-the-task-level) in questo articolo.

   <!--
   is this still accurate?!
   -->

## Spostare un&#39;attività a livello di attività {#move-a-task-at-the-task-level}

Oltre a spostare le attività da un elenco di attività, è possibile spostare un&#39;attività a livello di attività dopo averla aperta.

1. Cercare un&#39;attività nel sistema Workfront.
1. Fare clic sul nome dell&#39;attività per aprirla.
1. Fai clic sull&#39;icona ](assets/main-more-icon.png) del menu a discesa **Altro** accanto al nome dell&#39;attività, quindi fai clic su **Sposta in**. ![ Viene visualizzato il pannello laterale **Sposta attività**.

1. (Facoltativo) Aggiorna **Nome attività**. L&#39;attività si sposta con il nuovo nome nella nuova posizione.

   >[!TIP]
   >
   >Il campo **Nome attività** è inattivo e non è modificabile quando si seleziona per spostare più attività in un elenco. Puoi passare il cursore del mouse sul campo **Nome attività** per visualizzare un elenco di tutte le attività selezionate.
   >
   >
   >![Visualizza nomi attività](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. Nel campo **Seleziona progetto di destinazione** digitare il nome del progetto in cui si desidera spostare l&#39;attività. Se si desidera spostare l&#39;attività nello stesso progetto, digitare il nome del progetto corrente.

   >[!TIP]
   >
   >* Il nome del progetto distingue tra maiuscole e minuscole.
   >* Per cercare un progetto, digita il Numero di riferimento o immetti l’ID del progetto. Questo consente di distinguere i progetti con nomi identici.
   >* Nell’elenco vengono visualizzati solo 100 progetti.

1. (Condizionale) Se non hai accesso al progetto, fai clic su **Richiedi accesso**.
1. (Facoltativo) Se disponi dell’accesso per aggiungere attività a una delle attività del progetto di destinazione, continua a spostare l’attività nel progetto di destinazione senza richiedere l’accesso.

   ![Spostamento di un&#39;attività senza richiesta di accesso](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >Messaggi simili vengono visualizzati se il progetto selezionato è in attesa di approvazione, completato o inattivo quando l’amministratore di Workfront impedisce l’aggiunta di attività a questi progetti. Per ulteriori informazioni, vedere [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Facoltativo) Nella sezione **Opzioni**, deseleziona gli elementi elencati nella tabella seguente per rimuoverli dalle attività spostate. Tutte le opzioni sono selezionate per impostazione predefinita.

   >[!IMPORTANT]
   >
   >Deselezionando gli elementi nell&#39;elenco **Opzioni** si verifica una perdita di dati. Le informazioni dall&#39;attività esistente verranno rimosse e non potranno essere recuperate.

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
      <p>Nota: quando si sposta o si copia un'attività con vincoli specifici di data in un altro progetto e le date dei vincoli dell'attività non rientrano nelle nuove date del progetto, il vincolo dell'attività viene modificato in Il più presto possibile o Il più tardi possibile oppure vengono modificate le date di Inizio pianificato o Completamento pianificato dei progetti.

   Di seguito sono riportati alcuni esempi di vincoli specifici per data:
   <ul>
      <li> Inizia il</li>
      <li> Deve essere completato il</li>
      <li> Iniziare non Prima di</li>
      <li> Iniziare non Dopo di</li>
      </ul>

   Per ulteriori informazioni, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sui vincoli delle attività</a>.</p> </td>
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
      <td>Lo stato dell'attività è impostato su Nuovo. In caso contrario, lo stato dell'attività esistente viene mantenuto. </td> 
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
      <td> <p>I documenti allegati all'attività non vengono trasferiti all'attività spostata. Sono inclusi versioni, bozze e documenti collegati.</p> <p>Non sono incluse le approvazioni dei documenti. Le approvazioni dei documenti non possono mai essere spostate quando un'attività viene spostata.</p> 
      <p>Nota: se si sceglie di non spostare i documenti con l'attività, i documenti verranno eliminati e posizionati nel Cestino per 30 giorni. Un amministratore può ripristinarli e verranno ripristinati durante l’attività spostata. </p>

   <p>Se l'attività viene eliminata dopo essere stata spostata, i documenti ripristinati verranno posizionati nell'area Documenti della pagina utente dell'amministratore che li ripristina.</p>

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



1. (Facoltativo) Nella sezione **Seleziona elemento padre**, seleziona l&#39;attività nel progetto di destinazione che diventerà l&#39;elemento padre dell&#39;attività spostata.

   >[!TIP]
   >
   >Quando si seleziona per spostare più attività in un elenco, tutte le attività selezionate diventano gli elementi figlio dell&#39;elemento padre selezionato.

   Selezionare un elemento padre eseguendo una delle operazioni seguenti:

   * Nell&#39;elenco delle attività selezionare uno dei padri nel piano di progetto.
   * Fare clic sull&#39;icona di ricerca ![Icona di ricerca](assets/search-icon.png) e cercare un&#39;attività padre per nome.

   L’attività viene visualizzata nell’elenco.

   ![Selezionare l&#39;attività padre durante lo spostamento di un&#39;attività con funzionalità di ricerca ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

   >[!NOTE]
   >
   >Se non si seleziona un&#39;attività padre, le attività vengono spostate come attività principali anziché come sottoattività e vengono posizionate alla fine dell&#39;elenco delle attività nel progetto di destinazione.

1. Fare clic su **Sposta attività**. Le attività vengono spostate nel progetto specificato come sottoattività di un&#39;attività padre o come ultime attività del progetto.
