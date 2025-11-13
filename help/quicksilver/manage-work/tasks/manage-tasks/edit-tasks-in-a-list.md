---
product-area: projects
navigation-topic: manage-tasks
title: Modificare le attività in un elenco
description: È possibile modificare le informazioni sulle attività in un elenco di attività modificando i campi visualizzati nell'elenco. È necessario definire la Modalità pianificazione in un elenco di attività per indicare come si desidera salvare le modifiche in Workfront. È possibile salvare le modifiche manualmente o automaticamente.
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: 1f9a0e6064f83c6f0947e3c7ef596e96c934a687
workflow-type: tm+mt
source-wordcount: '2851'
ht-degree: 3%

---

# Modificare le attività in un elenco {#edit-tasks-in-a-list}

<!-- Audited: 10/2025 -->

<!--

<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

È possibile modificare le informazioni sulle attività in un elenco di attività modificando i campi visualizzati nell&#39;elenco. Per informazioni su altri modi per modificare le attività, vedere [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p>Standard<p>
   <p>Lavoro o superiore</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di contribuzione o superiori per l'attività e il progetto</p></td> 
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
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard<p>
   <p>Current: Work or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and&nbsp;Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to the task and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Considerazioni sulla modifica delle attività in un elenco {#considerations-about-editing-tasks-in-a-list}

La modifica delle attività in un elenco è un modo rapido per apportare modifiche a più attività contemporaneamente, con una chiara visualizzazione di come le modifiche potrebbero influenzare la sequenza temporale del progetto.

Quando si modificano attività in un elenco, tenere presente quanto segue:

* Diversamente dalla necessità di gestire le autorizzazioni per l&#39;attività quando la si modifica nella casella di modifica, è possibile modificare un&#39;attività in un elenco solo con le autorizzazioni Contribute per l&#39;attività. Questo consente di modificare le seguenti informazioni limitate per l&#39;attività:

   * Descrizione
   * Stato
   * Percentuale completato
   * Informazioni modulo personalizzato

     >[!NOTE]
     >
     >È possibile modificare un campo personalizzato dell&#39;attività in un elenco solo se si dispone delle autorizzazioni necessarie per aggiornare il campo.

   * Registra ore
   * Modifica assegnazioni
   * Visualizza informazioni finanziarie
   * Aggiungi spese, attività o problemi

* È possibile modificare un&#39;attività nei seguenti elenchi:

   * La sezione Attività del progetto
   * La sezione Sottoattività del progetto
   * Un rapporto di attività

     >[!NOTE]
     >
     >Per impostazione predefinita, Workfront salva automaticamente le modifiche apportate alle attività nella sezione Attività secondarie o in un report attività.

* È possibile controllare quando Workfront salva le modifiche apportate alle attività in un elenco definendo la Modalità pianificazione prima di iniziare a modificare le attività.

  Puoi scegliere se salvare le modifiche apportate da Workfront nel modo seguente:

      * Automaticamente, dopo ogni modifica
     * Manualmente, solo dopo aver fatto clic su Salva.
  
  Per informazioni su come configurare quando Workfront salva le modifiche apportate alle attività in un elenco, vedere la sezione [Modifica modalità pianificazione prima di modificare le attività in un elenco](#modify-plan-mode-before-editing-tasks-in-a-list) in questo articolo.

* Gli altri utenti devono aggiornare le proprie pagine prima di poter visualizzare gli aggiornamenti apportati a un&#39;attività.

## Modifica modalità pianificazione prima di modificare le attività in un elenco

È possibile decidere se le modifiche apportate alle attività in un elenco vengono salvate automaticamente quando si verificano oppure se si desidera salvare manualmente ogni modifica. A tale scopo, è necessario modificare la Modalità pianificazione in un elenco di attività prima di modificare le attività.

>[!IMPORTANT]
>
>A seconda che le attività vengano salvate automaticamente o manualmente, è possibile che le informazioni di un altro utente vengano sovrascritte durante la modifica delle attività in un elenco. Per ulteriori informazioni, vedere [Panoramica sul salvataggio delle modifiche simultanee in un elenco di attività](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

Quando si salvano le modifiche in un elenco per un progetto il cui Tipo di aggiornamento è selezionato Automatico o Automatico e Al momento della modifica, Workfront aggiorna la sequenza temporale del progetto, insieme a tutte le dipendenze all&#39;interno del progetto e tra progetti. I calcoli della sequenza temporale possono richiedere molto tempo se il progetto è di grandi dimensioni o se vi sono molte dipendenze. Alcuni metodi di modifica di un elenco di attività possono essere più veloci di altri, a seconda del metodo selezionato per salvare le modifiche.

È possibile controllare quando Workfront salva le modifiche apportate alle attività in un elenco. Esistono i seguenti scenari:

* Workfront può salvare automaticamente le modifiche dopo ogni aggiornamento.

  Per informazioni, vedere la sezione [Impostare la modalità di pianificazione per salvare automaticamente le modifiche](#set-the-plan-mode-to-automatically-save-changes) in questo articolo.

* È possibile controllare quando si applicano più modifiche contemporaneamente utilizzando manualmente un pulsante Salva.

  Per informazioni, vedere la sezione [Impostare la modalità di pianificazione per salvare manualmente le modifiche](#set-the-plan-mode-to-manually-save-changes) in questo articolo.

### Imposta la modalità pianificazione per salvare automaticamente le modifiche

>[!TIP]
>
>Il salvataggio delle modifiche e di tutte le dipendenze del progetto potrebbe risultare più lento se il progetto contiene più di 2.000 attività o se presenta molte dipendenze.

Quando si salvano automaticamente le modifiche all&#39;elenco attività, tenere presente quanto segue:

* È possibile applicare una visualizzazione personalizzata all&#39;elenco delle attività e modificare qualsiasi campo relativo alle attività a cui si ha accesso per l&#39;aggiornamento.
* Impossibile annullare le modifiche salvate automaticamente. Questa è l&#39;impostazione predefinita.
* Quando il tipo di aggiornamento del progetto è Automatico o Automatico e Su modifica, Workfront ricalcola automaticamente la timeline del progetto e tutte le dipendenze interne e tra progetti dopo ogni modifica. Per informazioni sul tipo di aggiornamento del progetto, vedere [Selezionare il tipo di aggiornamento del progetto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Per modificare le attività in un elenco e salvare automaticamente le modifiche:

{{step1-to-projects}}

1. Nella pagina **Progetti**, seleziona un progetto.
1. Nel pannello a sinistra, fai clic sulla sezione **Attività**.

1. Fai clic sull&#39;icona **Modalità pianificazione** ![Icona Modalità pianificazione](assets/plan-mode-icon.png) nella parte superiore dell&#39;elenco e accertati che sia selezionata l&#39;opzione **Salvataggio automatico**.

   ![Abilitare l&#39;impostazione del salvataggio automatico](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. Modifica qualsiasi campo per il quale disponi delle autorizzazioni necessarie per eseguire manualmente l’aggiornamento.

1. (Facoltativo) Premi **Esc** per annullare le modifiche.
1. Premi **Invio** (Windows) o **Ritorno** (Mac) sulla tastiera per salvare le modifiche apportate alle attività e alla sequenza temporale del progetto.
1. (Facoltativo) Fai clic con il pulsante destro del mouse su un’attività da modificare.

   Oppure

   Fare clic sul menu **Altro** ![](assets/more-icon-task-list.png) a destra del nome dell&#39;attività.

1. (Facoltativo) Seleziona una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Apri in una nuova scheda</td> 
      <td>Apre l'attività in una nuova scheda del browser. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Inserisci attività in alto</td> 
      <td>Inserisce un'attività sopra l'attività selezionata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserisci attività in basso</td> 
      <td>Inserisce un'attività sotto l'attività selezionata</td> 
     </tr>
     <tr> 
      <td role="rowheader">Modifica</td> 
      <td><p>Apre la casella Modifica attività, in cui è possibile modificare l'attività.</p><p>Per informazioni sulla modifica di un'attività, vedere <a href="#edit-tasks-in-a-list" class="MCXref xref">Modificare le attività in un elenco</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Elimina</td> 
      <td><p>Elimina l'attività.</p><p>Per informazioni sull'eliminazione delle attività, vedere <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Elimina attività</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rientro</td> 
      <td><p>Rientra l'attività di un livello. </p><p>Questa opzione viene visualizzata solo per le attività autonome.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rientro negativo</td> 
      <td><p>Riduce il rientro dell'attività di un livello. </p><p>Questa opzione viene visualizzata solo sulle attività figlio. </p></td> 
     </tr>  
     <tr> 
      <td role="rowheader">Duplica</td> 
      <td><p>Crea una versione duplicata dell'attività nello stesso progetto. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copia in...</td> 
      <td><p>Copia l'attività in un altro progetto.</p><p>Per informazioni sulla copia e la duplicazione delle attività, vedere <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiare e duplicare le attività</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sposta in...</td> 
      <td><p>Sposta l'attività in un altro progetto.</p><p>Per informazioni sullo spostamento delle attività, vedere <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">Sposta attività</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

### Imposta la modalità pianificazione per salvare manualmente le modifiche {#edit-tasks-in-a-list-and-manually-save-changes}

È possibile salvare manualmente le modifiche apportate alle attività in un elenco. Quando si salvano le modifiche in questo modo, è possibile annullarle prima di salvarle.

>[!TIP]
>
>* Non è possibile annullare le modifiche apportate alle attività in un elenco quando vengono modificate nella sezione Attività secondarie o in un report attività.
>* Non vi sono limiti al numero di modifiche che è possibile annullare. È possibile invertirle tutte una per una fino a quando non si raggiunge lo stato originale delle attività.
>

Quando si salvano manualmente le modifiche in un elenco di attività, tenere presente quanto segue:

* Per salvare manualmente le modifiche all&#39;elenco delle attività, è necessario disporre delle autorizzazioni per gestire sia le attività che il progetto.
* Non è possibile modificare il progetto. L’opzione per modificare il progetto è disabilitata.
* Non è possibile aggiornare le informazioni nell’intestazione del progetto. È possibile eseguire le operazioni seguenti solo quando si salvano manualmente le modifiche nell&#39;elenco delle attività:

   * Abbonati al progetto.
   * Aggiungi il progetto all’elenco dei preferiti.
   * Aprire un&#39;attività facendo clic sul nome corrispondente nell&#39;elenco.

* Modificare le attività in blocco. L&#39;icona Modifica è disattivata quando si selezionano più attività.
* Workfront attiva le notifiche sulle modifiche apportate alle attività solo dopo il salvataggio delle modifiche.

Esistono due modi per salvare manualmente le modifiche apportate alle attività in un elenco:

* [Salvare manualmente le modifiche in un elenco di attività quando si seleziona l&#39;opzione Salvataggio manuale standard](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [Salvare manualmente le modifiche in un elenco di task quando si seleziona l&#39;opzione Pianificazione manuale della sequenza temporale](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### Salvare le modifiche in un elenco di operazioni manualmente quando si seleziona l&#39;opzione Salvataggio manuale standard {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>Se il progetto contiene più di 2.000 attività o se presenta molte dipendenze, potrebbe essere necessario del tempo per identificare visivamente le modifiche apportate alle attività e il modo in cui tali modifiche influiscono su tutte le dipendenze del progetto. In questo caso, il salvataggio delle modifiche potrebbe richiedere più tempo del previsto.

Quando si aggiornano le attività in un elenco dopo aver selezionato l&#39;opzione Salvataggio manuale standard, tenere presente quanto segue:

* È possibile applicare una visualizzazione personalizzata all&#39;elenco delle attività e modificare qualsiasi campo relativo alle attività per il quale si dispone delle autorizzazioni di gestione.
* Quando il tipo di aggiornamento del progetto è Automatico o Automatico e In caso di modifica, Workfront calcola la timeline del progetto e tutte le dipendenze interne e tra i progetti dopo aver fatto clic su Salva. Per informazioni sul tipo di aggiornamento del progetto, vedere [Selezionare il tipo di aggiornamento del progetto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Per modificare i task in un elenco selezionando l&#39;opzione Salvataggio manuale standard:

{{step1-to-projects}}

1. Nella pagina **Progetti**, seleziona un progetto.

1. Nel pannello a sinistra, fai clic sulla sezione **Attività**.

1. Fai clic sull&#39;icona **Modalità pianificazione** ![Icona Modalità pianificazione](assets/plan-mode-icon.png) nella parte superiore dell&#39;elenco.

1. Nella finestra di dialogo **Modalità pianificazione**, seleziona **Salvataggio manuale**, quindi fai clic su **Standard**.

   ![Abilitare l&#39;impostazione di salvataggio manuale](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Fare clic su **Applica**. Viene visualizzata un’impostazione della barra degli strumenti con opzioni per annullare, ripetere e salvare le modifiche.

   ![Barra degli strumenti di salvataggio manuale](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Fai clic all’interno di qualsiasi campo per il quale disponi delle autorizzazioni necessarie per aggiornare manualmente. Il campo diventa modificabile e puoi apportare le modifiche.

1. Premi **Invio** (Windows) o **Ritorno** (Mac) sulla tastiera per salvare temporaneamente le modifiche apportate.

1. (Facoltativo) Fai clic sull&#39;icona **Annulla** ![Annulla icona](assets/undo-icon-on-task-list.png) per annullare una modifica e ripristinare lo stato originale di un campo.

1. (Facoltativo e condizionale) Fai clic sull&#39;icona **Ripeti** ![Ripeti](assets/redo-icon-on-task-list.png) per ripristinare la modifica annullata.

1. (Facoltativo) Fai clic con il pulsante destro del mouse su un’attività da modificare.

   Oppure

   Fare clic sul menu **Altro** ![](assets/more-icon-task-list.png).

1. (Facoltativo) Seleziona una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Apri in una nuova scheda</td> 
      <td>Apre l'attività in una nuova scheda del browser. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Inserisci attività in alto</td> 
      <td>Inserisce un'attività sopra l'attività selezionata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserisci attività in basso</td> 
      <td>Inserisce un'attività sotto l'attività selezionata</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Elimina</td> 
      <td>Per informazioni sull'eliminazione delle attività, vedere <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Elimina attività</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rientro</td> 
      <td> <p>Rientra l'attività di un livello. </p> <p>Questa opzione viene visualizzata solo per le attività autonome.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rientro negativo</td> 
      <td> <p>Riduce il rientro dell'attività di un livello. </p> <p>Questa opzione viene visualizzata solo sulle attività figlio. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplica</td> 
      <td> <p>Crea una versione duplicata dell'attività nello stesso progetto. </p> <p>Per informazioni sulla copia e la duplicazione delle attività, vedere <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiare e duplicare le attività</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront aggiorna tutte le dipendenze interne e tra progetti quando si apportano modifiche alla sequenza temporale delle attività.
1. Fai clic su **Salva** per mantenere le modifiche dell&#39;attività in modo permanente e salvare la sequenza temporale del progetto.

#### Salvare manualmente le modifiche in un elenco di task quando si seleziona l&#39;opzione Pianificazione manuale della sequenza temporale {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

Salvare le modifiche e tutte le dipendenze del progetto è più veloce. Questa opzione non è disponibile per i progetti con più di 2.000 attività.

>[!IMPORTANT]
>
>È consigliabile utilizzare questa opzione quando si modifica un elenco esteso di attività con più di poche centinaia di dipendenti. Questa opzione consente di identificare visivamente le modifiche molto più rapidamente rispetto all’opzione Salvataggio manuale.

Quando si utilizza l&#39;opzione Pianificazione manuale della sequenza temporale in un elenco di task, tenere presente quanto segue:

* Non è possibile applicare l&#39;opzione Pianificazione sequenza temporale salvataggio manuale ai progetti con più di 2.000 task.
* Non è possibile applicare una visualizzazione, un filtro o un raggruppamento personalizzato all&#39;elenco delle attività. I menu a discesa Visualizza, Filtro e Raggruppamento, nonché l’icona della vista Agile, sono disattivati. La visualizzazione applicata per impostazione predefinita contiene un numero limitato di campi.
* La timeline del progetto e tutte le dipendenze interne al progetto vengono calcolate automaticamente dopo ogni modifica quando il tipo di aggiornamento del progetto è Automatico o Automatico e In caso di modifica.
* Quando il tipo di aggiornamento del progetto è Automatico o Automatico e In caso di modifica, le dipendenze tra progetti vengono calcolate dopo aver fatto clic su Salva. Per informazioni sul tipo di aggiornamento del progetto, vedere [Selezionare il tipo di aggiornamento del progetto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Per modificare i task in un elenco quando si utilizza l&#39;opzione Pianificazione manuale del salvataggio della sequenza temporale:


{{step1-to-projects}}

1. Nella pagina **Progetti**, seleziona un progetto.

1. Nel pannello a sinistra, fai clic sulla sezione **Attività**.

1. Fai clic sull&#39;icona **Modalità pianificazione** ![Icona Modalità pianificazione](assets/plan-mode-icon.png) nella parte superiore dell&#39;elenco.

1. Nella finestra di dialogo **Modalità pianificazione**, seleziona **Salvataggio manuale**, quindi fai clic su **Pianificazione sequenza temporale**.

   ![Applica impostazione di pianificazione sequenza temporale](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >L&#39;opzione **Pianificazione del tempo** è disabilitata per i progetti con più di 2.000 attività.

1. Fare clic su **Applica**.

   Nell&#39;elenco si verificano le seguenti modifiche:

   * I menu a discesa Visualizza, Raggruppamento e Filtro vengono rimossi e la visualizzazione viene sostituita dai campi seguenti:

      * Numero Attività
      * Nome attività
      * Tipo di Vinconlo
      * Durata
      * Data di inizio pianificata
      * Data di completamento Pianificata
      * Predecessori
      * Assegnazioni
      * Stato
      * Percentuale completato

   * L’icona della vista Agile viene rimossa.
   * Viene visualizzata un’impostazione della barra degli strumenti con opzioni per annullare, ripetere e salvare le modifiche.

     ![Barra degli strumenti di salvataggio manuale](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Modifica qualsiasi campo per il quale disponi delle autorizzazioni necessarie per eseguire manualmente l’aggiornamento.

1. Premi **Invio** (Windows) o **Ritorno** (Mac) sulla tastiera per salvare temporaneamente le modifiche apportate.
1. (Facoltativo) Fai clic sull&#39;icona **Annulla** ![Annulla icona](assets/undo-icon-on-task-list.png) per annullare una modifica e ripristinare lo stato originale di un campo.
1. (Facoltativo e condizionale) Fare clic sull&#39;icona **Ripeti** ![Ripeti](assets/redo-icon-on-task-list.png) per ripristinare la modifica annullata.

1. (Facoltativo) Fai clic con il pulsante destro del mouse su un’attività da modificare.

   Oppure

   Fare clic sul menu **Altro** ![](assets/more-icon-task-list.png).

1. Selezionare una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Apri in una nuova scheda</td> 
      <td>Apre l'attività in una nuova scheda del browser. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Inserisci attività in alto</td> 
      <td>Inserisce un'attività sopra l'attività selezionata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserisci attività in basso</td> 
      <td>Inserisce un'attività sotto l'attività selezionata</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Elimina</td> 
      <td>Per informazioni sull'eliminazione delle attività, vedere <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Elimina attività</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rientro</td> 
      <td> <p>Rientra l'attività di un livello. </p> <p>Questa opzione viene visualizzata solo per le attività autonome.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rientro negativo</td> 
      <td> <p>Riduce il rientro dell'attività di un livello. </p> <p>Questa opzione viene visualizzata solo sulle attività figlio. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplica</td> 
      <td> <p>Crea una versione duplicata dell'attività nello stesso progetto. </p> <p>Per informazioni sulla copia e la duplicazione delle attività, vedere <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiare e duplicare le attività</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Quando si modifica la sequenza temporale di un&#39;attività, Workfront aggiorna tutte le dipendenze interne e tra progetti.
1. Fai clic su **Salva** per mantenere le modifiche dell&#39;attività in modo permanente e salvare la sequenza temporale del progetto.

## Modificare un&#39;attività in un elenco utilizzando il Riepilogo

{{step1-to-projects}}

1. Nella pagina **Progetti**, seleziona un progetto.

1. Nel pannello a sinistra, fai clic sulla sezione **Attività**. Viene visualizzato l’elenco delle attività sul progetto.

1. Seleziona l&#39;attività da modificare, quindi fai clic sull&#39;icona **Apri riepilogo** ![Apri riepilogo](assets/task-summary-icon.png) nell&#39;angolo superiore destro dell&#39;elenco. Viene aperto il pannello **Riepilogo attività**.

1. (Facoltativo) Digita un aggiornamento per l&#39;attività nell&#39;area **Aggiornamenti**.
1. Fare clic su una delle icone o aree seguenti per accedere all&#39;attività e modificare le informazioni a livello di attività:

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Documenti</td> 
      <td>Aggiungi documenti all'attività. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Moduli personalizzati</td> 
      <td>Aggiungere o rimuovere moduli personalizzati o aggiornare le informazioni sui moduli.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ore</td> 
      <td>Registra ore.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approvazioni</td> 
      <td>Aggiungi approvazioni attività.</td> 
     </tr> 
     <tr> 
    </tbody> 
   </table>

1. Fai clic su **X** nell&#39;angolo superiore destro del pannello per chiuderlo.

## Modifica attività in blocco

È possibile modificare più attività contemporaneamente. Assicurarsi di disporre delle autorizzazioni di gestione per le attività per poterle modificare.

{{step1-to-projects}}

1. Nella pagina **Progetti**, seleziona un progetto.
1. Nel pannello a sinistra, fai clic sulla sezione **Attività**.

1. Fai clic sull&#39;icona **Modalità pianificazione** ![Icona Modalità pianificazione](assets/plan-mode-icon.png) nella parte superiore dell&#39;elenco e accertati che sia selezionata l&#39;opzione **Salvataggio automatico**.

   ![Abilitare l&#39;impostazione del salvataggio automatico](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

   >[!IMPORTANT]
   >
   >Non è possibile modificare le attività in blocco quando si salvano le attività manualmente.

1. Selezionare più attività nell&#39;elenco delle attività.
1. (Facoltativo) Fai clic sul menu **Altro** ![Altro menu](assets/more-icon.png) nella parte superiore dell&#39;elenco delle attività, quindi **Ricalcola espressioni** per aggiornare tutte le informazioni nei campi personalizzati calcolati.
1. Fai clic sull&#39;icona **Modifica** ![Modifica](assets/qs-edit-icon.png). Nella nuova esperienza verrà visualizzata la finestra di dialogo **Modifica attività**.

   La modifica delle informazioni su tutte le attività è identica alla modifica delle informazioni su un&#39;attività.

   Per ulteriori informazioni sulla modifica di un&#39;attività, vedere [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. (Condizionale) Nella nuova esperienza, effettua le seguenti operazioni:

   1. Specificare le informazioni da modificare per tutte le attività selezionate in una delle seguenti aree:

      * Panoramica
      * Assegnazioni
      * Moduli personalizzati
      * Finanz
      * Impostazioni
      * Impostazioni
      * Commento

      >[!NOTE]
      >
      >* Le informazioni che stai modificando in tutte le attività selezionate sostituiranno le informazioni esistenti sulle singole attività, ad eccezione del campo **Assegnazioni**. L&#39;aggiunta di un nuovo assegnatario nella modifica in blocco aggiungerà l&#39;assegnatario a tutte le attività selezionate. Se alle attività selezionate vengono assegnati altri assegnatari, questi rimarranno assegnati in aggiunta a quelli aggiunti tramite la modifica in blocco.
      >* Se si desidera modificare la durata dell&#39;attività, le attività selezionate devono avere lo stesso vincolo attività. In caso contrario, il campo **Durata** non viene popolato.
      >
      >* Nell’elenco vengono visualizzati solo i moduli personalizzati attivi. Se le attività selezionate non hanno moduli personalizzati comuni, in questa sezione non sono elencati moduli.
      >* È possibile modificare solo i campi dei moduli allegati a tutte le attività selezionate e per i quali si dispone delle autorizzazioni di modifica.  Per informazioni sulla modifica in blocco di moduli personalizzati, vedere [Gestire i moduli personalizzati allegati agli oggetti](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).

   1. Fai clic su **Salva**.
   1. (Facoltativo) Fai clic su **Torna alla vecchia esperienza** nella parte inferiore della casella **Modifica attività**.

1. (Condizionale) Nella vecchia esperienza, effettua le seguenti operazioni:

   1. Specificare le informazioni da modificare per tutte le attività selezionate in una delle seguenti aree:

      * Panoramica
      * Impostazioni
      * Assegnazioni
      * Moduli personalizzati
      * Commento

   1. (Facoltativo) Nella sezione **Forms personalizzato**, selezionare l&#39;opzione **Ricalcola espressioni personalizzate** per assicurarsi che tutti i campi personalizzati calcolati presenti nei moduli personalizzati allegati alle attività selezionate siano aggiornati.
   1. Fai clic su **Salva modifiche**. Tutte le modifiche apportate sono ora visibili in tutte le attività selezionate.

