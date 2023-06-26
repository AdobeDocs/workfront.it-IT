---
product-area: projects
navigation-topic: manage-tasks
title: Copiare e duplicare le attività
description: È possibile copiare un'attività da un progetto a un altro oppure duplicarla all'interno dello stesso progetto.
author: Alina
feature: Work Management
exl-id: daf89062-cf58-4c39-83ff-727d969a9630
source-git-commit: 1f749ba9a54ce75a917e4b1e95713ac7abeaa66b
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 1%

---

# Copiare e duplicare le attività

È possibile copiare un&#39;attività da un progetto a un altro oppure duplicarla all&#39;interno dello stesso progetto.

È possibile copiare o duplicare una o più attività o attività padre alla volta.

## Requisiti di accesso

<!-- drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a task</p> <p>Contribute or higher permissions to the project</p> 
   <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un’attività </p> <p>Autorizzazioni Contribute (Contribute) o superiori per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Considerazioni per la copia delle attività

Quando copi un’attività, tieni presente quanto segue:

* I problemi non vengono copiati con l&#39;attività.
* Le attività cardine vengono trasferite all&#39;attività copiata e rimosse dall&#39;attività originale.
* Quando si copia un&#39;attività da un progetto a un altro, le date dell&#39;attività potrebbero essere ricalcolate. Il ricalcolo terrà conto della pianificazione utilizzata dal nuovo progetto e delle informazioni di Schedule From del progetto.

Puoi copiare un’attività nelle seguenti aree dell’applicazione web Adobe Workfront:

* A livello di attività, da **Icona Altro** ![](assets/qs-more-menu-19x7.png) a destra del nome dell&#39;attività.

  Per informazioni, vedere [Copiare un&#39;attività a livello di attività](#copy-a-task-at-the-task-level) in questo articolo.

* In un elenco di attività, eseguendo una delle operazioni seguenti:

   * Fare clic con il pulsante destro del mouse sul nome di un&#39;attività.
   * Selezionare l&#39;attività o le attività ed espandere **Altro** icona ![](assets/more-icon-task-list.png) nella parte superiore dell&#39;elenco delle attività.
   * Selezionare un&#39;attività ed espandere **Altro** icona ![](assets/more-icon-task-list.png) accanto al nome dell&#39;attività.

     Questa opzione non è disponibile quando si selezionano più attività.

  Per informazioni, vedere [Copiare le attività in un elenco](#copy-tasks-in-a-list) in questo articolo.

## Copiare le attività in un elenco {#copy-tasks-in-a-list}

1. Passare al progetto contenente l&#39;attività o le attività che si desidera copiare.

   Oppure

   Passare a un report attività.

1. Clic **Attività** nel pannello a sinistra.
1. Fai clic su **Menu della modalità Piano** ![](assets/qs-list-mode-or-save-mode-icon-small.png) , quindi **Salvataggio automatico**.

   >[!IMPORTANT]
   >
   >È possibile copiare le attività in un elenco solo quando si salvano automaticamente le modifiche. Per informazioni sul salvataggio delle opzioni durante la modifica delle attività, consulta [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Selezionare l&#39;attività o le attività che si desidera copiare ed effettuare una delle seguenti operazioni:

   * Fai clic su **Menu Altro** nella parte superiore dell&#39;elenco delle attività, quindi fare clic su **Copia in**.
   * Fare clic con il pulsante destro del mouse sulle attività selezionate, quindi scegliere **Copia in**.
   * Quando si seleziona un&#39;attività, fare clic su **Altro** menu ![](assets/more-icon-task-list.png) accanto al nome dell&#39;attività nell&#39;elenco, quindi fare clic su **Copia in**.

   ![](assets/copy-task-in-list-nwe-350x131.png)

1. Continua a copiare l’attività come descritto nella sezione [Copiare un&#39;attività a livello di attività](#copy-a-task-at-the-task-level) a partire dal passaggio 4.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this still accurate?!)
   </MadCap:conditionalText>
   -->

## Copiare un&#39;attività a livello di attività {#copy-a-task-at-the-task-level}

Oltre a copiare le attività in un elenco di attività, è possibile copiare un&#39;attività dopo averla aperta. 

1. Cercare un&#39;attività nel sistema Workfront.
1. Fare clic sul nome dell&#39;attività per aprirla. 
1. Fai clic su **Altro** menu a discesa ![](assets/qs-more-menu.png) accanto al nome dell&#39;attività, quindi fare clic su **Copia** **a**.

   ![](assets/taskcopy-to-at-the-task-level-nwe-350x200.png)

   Viene visualizzata la casella Copia attività.

1. (Facoltativo) Aggiorna il **Nome attività**.

   >[!TIP]
   >
   >Questo campo è inattivo e non è modificabile quando si seleziona per copiare più attività in un elenco. È possibile passare il cursore del mouse sul campo Nome attività per visualizzare un elenco di tutte le attività selezionate.
   >
   >![](assets/copy-task-multiple-tasks-box-with-list-of-task-names-nwe-350x130.png)

1. Digita il nome del **Progetto di destinazione** dove si desidera copiare l&#39;attività in **Seleziona progetto di destinazione** campo. 

   >[!TIP]
   >
   >* Il nome del progetto distingue tra maiuscole e minuscole.
   >* Puoi anche iniziare a digitare il Numero di riferimento o immettere l’ID del progetto. Questo potrebbe aiutarti a distinguere i progetti con nomi identici.
   >* Nell’elenco vengono visualizzati solo 100 progetti.

   Il nome del progetto corrente viene visualizzato per impostazione predefinita. Se si desidera copiare l&#39;attività all&#39;interno dello stesso progetto, lasciare questo campo invariato.

1. (Condizionale) Fai clic su **richiedi accesso** per richiedere l’accesso al progetto, se non hai accesso al progetto selezionato.
1. (Facoltativo) Continua a copiare l&#39;attività nel progetto di destinazione selezionato senza richiedere l&#39;accesso se disponi dell&#39;accesso per aggiungere attività a una delle attività nel progetto di destinazione.

   ![](assets/copy-task-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Messaggi simili vengono visualizzati se il progetto selezionato è in attesa di approvazione, completato o inattivo, quando l’amministratore di Workfront impedisce l’aggiunta di attività a questi progetti. Per ulteriori informazioni, consulta [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. Clic **Opzioni** nel pannello a sinistra, deseleziona gli attributi dell’attività che non desideri copiare con l’attività. Tutte le opzioni sono selezionate per impostazione predefinita.

   >[!TIP]
   >
   Selezione e deselezione **Seleziona tutto** deseleziona tutte le opzioni.

   Deseleziona le seguenti opzioni per non trasferirle all’attività copiata. La tabella seguente descrive cosa accade quando le opzioni vengono deselezionate:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Vincolo Data</td> 
      <td> <p>Il vincolo attività viene impostato su Il più presto possibile o Il più tardi possibile in base all'impostazione Modalità pianificazione del progetto.</p> <p> Se selezionata, il vincolo corrente dell'attività viene trasferito all'attività copiata. </p> <p>Nota: quando si sposta o si copia un'attività con vincoli specifici di data in un altro progetto e le date dei vincoli dell'attività non rientrano nelle date del nuovo progetto, il vincolo dell'attività viene modificato in Il più presto possibile o Il più tardi possibile oppure vengono modificate le date di Inizio pianificato o Completamento pianificato dei progetti. Alcuni esempi di vincoli specifici della data sono Deve iniziare il, Deve finire il, Deve iniziare non prima del, Inizia non dopo il, ecc. Per informazioni sui vincoli delle attività e sul modo in cui possono essere influenzati i vincoli delle attività o le date del progetto, vedere <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Panoramica sui vincoli delle attività</a> e cercare un vincolo specifico.</p> </td> 
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
      <td>Lo stato dell'attività è Nuovo. In caso contrario, l'attività copiata mantiene lo stato dell'attività esistente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informazioni finanziarie</td> 
      <td>Le informazioni finanziarie dell'attività vengono rimosse.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tutti i predecessori</td> 
      <td> <p>Ciò significa che le dipendenze non verranno riportate alle attività copiate. </p> <p>Se questa opzione è selezionata, i predecessori all'interno del gruppo di attività copiate vengono mantenuti, mentre gli altri vengono eliminati.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenti</td> 
      <td> <p>I documenti allegati all'attività non vengono trasferiti all'attività copiata. Sono inclusi versioni, bozze e documenti collegati.</p> <p>Non sono incluse le approvazioni di documenti. Le approvazioni dei documenti non possono mai essere copiate quando un'attività viene copiata.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifiche promemoria</td> 
      <td>I promemoria dell'attività non vengono trasferiti all'attività copiata. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spese</td> 
      <td>Le spese registrate per l'attività non vengono trasferite all'attività copiata. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autorizzazioni</td> 
      <td>Workfront rimuove i nomi di tutte le entità visualizzate nell'elenco Condivisione dell'attività. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dati personalizzati</td> 
      <td> <p>I valori dei campi personalizzati vengono cancellati e i moduli personalizzati vengono trasferiti all'attività copiata. </p> <p>Quando questa opzione è selezionata, i moduli e i valori dei campi personalizzati vengono trasferiti all'attività copiata. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1.  (Facoltativo) Fai clic su **Seleziona elemento padre** nel pannello a sinistra, seleziona l’attività nel progetto di destinazione che desideri diventi l’attività principale dell’attività copiata.

   >[!TIP]
   >
   Quando si seleziona per copiare più attività in un elenco, tutte le attività selezionate diventano gli elementi figlio dell&#39;elemento padre selezionato.

   Selezionare un elemento padre eseguendo una delle operazioni seguenti:

   * Nell&#39;elenco delle attività selezionare uno dei padri nel piano di progetto.
   * Fai clic sull’icona di ricerca ![Icona Ricerca](assets/search-icon.png) e cercare un&#39;attività padre per nome.

   L&#39;attività dovrebbe essere visualizzata nell&#39;elenco.

   ![Selezionare l&#39;attività padre quando si sposta un&#39;attività con funzionalità di ricerca ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Dopo averlo trovato, seleziona il pulsante di opzione relativo al genitore. 

   Se non si seleziona un&#39;attività padre, le attività vengono copiate come attività principali anziché come sottoattività e verranno inserite alla fine dell&#39;elenco delle attività nel progetto di destinazione. 

1. Clic **Copia attività**

   Oppure

   Clic **Copia attività** quando si selezionano più attività in un elenco.
Le attività copiate si trovano ora nel progetto specificato e sono sottoattività dell&#39;attività padre selezionata o delle ultime attività del progetto.

## Duplica attività

È possibile duplicare rapidamente un&#39;attività in un elenco di attività se è necessaria un&#39;attività identica nello stesso progetto.

* [Considerazioni sulla duplicazione delle attività](#considerations-for-duplicating-tasks)
* [Duplica attività](#duplicate-tasks)

### Considerazioni sulla duplicazione delle attività {#considerations-for-duplicating-tasks}

* È possibile duplicare un&#39;attività in un elenco di attività solo se l&#39;elenco è ordinato in base al numero di attività.

* La nuova attività avrà lo stesso nome dell&#39;attività originale.
* Impossibile selezionare le informazioni da duplicare nella nuova attività. Per impostazione predefinita, quasi tutte le informazioni dell&#39;attività originale vengono trasferite all&#39;attività duplicata, inclusa la relazione padre.
* I seguenti elementi non vengono trasferiti alla nuova attività:

   * Ore registrate
   * Note
   * Problemi
   * Solo i predecessori che fanno parte dello stesso gruppo di attività copiate vengono copiati con le attività successori.

     **Esempio:** Ad esempio, se si copia contemporaneamente l&#39;Attività 2 e il suo predecessore, l&#39;Attività 1, si disporrà di una copia dell&#39;Attività 2 e di una copia dell&#39;Attività 1. La copia dell&#39;attività 1 sarà la copia precedente dell&#39;attività 2. Ma se copi solo l&#39;Attività 2 senza copiare il suo predecessore, allora la sua copia non avrà alcun predecessore.

* Quando si duplica un&#39;attività padre, vengono duplicate anche tutte le attività figlio, anche quando le attività figlio non sono selezionate.
* È possibile duplicare più attività contemporaneamente.

  Tuttavia, non è possibile duplicare più attività non sequenziali contemporaneamente.

* Le attività cardine vengono spostate nella nuova attività e rimosse dall&#39;attività originale.

### Duplica attività

1. Passare al progetto contenente l&#39;attività o le attività che si desidera duplicare.
1. Clic **Attività** nel pannello a sinistra.
1. Esegui una delle operazioni seguenti:

   * (Condizionale) Fai clic su **Menu della modalità Piano** ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **Salvataggio automatico**, seleziona le attività da duplicare, quindi fai clic sul pulsante **Menu Altro** ![](assets/qs-more-menu-29x11.png) > **Duplica**.

     ![](assets/duplicate-tasks-in-list-nwe-350x196.png)

   * (Condizionale) Fai clic su **Menu della modalità Piano** ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **Salvataggio manuale** > **Standard** o **Pianificazione sequenza temporale**, quindi eseguire le operazioni seguenti:

      1. Selezionare l&#39;attività o le attività da duplicare e fare clic su **Duplica**.
      1. (Facoltativo) Fai clic su **Annulla** per annullare le modifiche e non duplicare le attività.
      1. (Facoltativo e condizionale) Fai clic su **Ripeti** se in precedenza hai fatto clic su **Annulla**, per mantenere le modifiche e duplicare le attività.

      1. Clic **Salva** per salvare le modifiche.

   1. Modificare le attività in un elenco
