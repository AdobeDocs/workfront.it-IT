---
product-area: projects
navigation-topic: manage-tasks
title: Modificare le attività in un elenco
description: È possibile modificare le informazioni sulle attività in un elenco di attività modificando i campi visualizzati nell'elenco. Per informazioni su altri modi per modificare le attività, vedere Modificare le attività.
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: 1da2e6448f7ac6f4bd5bd76846fbfc1a23c3da77
workflow-type: tm+mt
source-wordcount: '2848'
ht-degree: 2%

---

# Modificare le attività in un elenco {#edit-tasks-in-a-list}

È possibile modificare le informazioni sulle attività in un elenco di attività modificando i campi visualizzati nell&#39;elenco. Per informazioni su altri modi per modificare le attività, vedere [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Requisiti di accesso

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
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di contribuzione o superiori per l'attività e il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

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

* È possibile controllare quando Workfront salva le modifiche apportate alle attività in un elenco. Le modifiche possono essere salvate automaticamente o manualmente.

  Per informazioni su come configurare quando Workfront salva le modifiche apportate alle attività in un elenco, vedere [Selezionare un&#39;opzione di salvataggio durante la modifica delle attività in un elenco](#select-a-save-option-when-editing-tasks-in-a-list) in questo articolo.

* Gli altri utenti devono aggiornare le proprie pagine prima di poter visualizzare gli aggiornamenti apportati a un&#39;attività.

## Selezionare un&#39;opzione di salvataggio durante la modifica delle attività in un elenco {#select-a-save-option-when-editing-tasks-in-a-list}

È possibile decidere dove vengono salvate automaticamente le modifiche apportate alle attività in un elenco, quando si verificano o se si desidera salvare manualmente ogni modifica.

>[!IMPORTANT]
>
>A seconda che le attività vengano salvate automaticamente o manualmente, è possibile che le informazioni di un altro utente vengano sovrascritte durante la modifica delle attività in un elenco. Per informazioni sul modo in cui Workfront salva le modifiche sulle attività che esegui in concomitanza con altri utenti, vedi [Panoramica sul salvataggio delle modifiche simultanee in un elenco di attività](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

Quando si salvano le modifiche in un elenco per un progetto il cui Tipo di aggiornamento è selezionato Automatico o Automatico e Al momento della modifica, Workfront aggiorna la sequenza temporale del progetto, insieme a tutte le dipendenze all&#39;interno del progetto e tra progetti. I calcoli della sequenza temporale possono richiedere molto tempo se il progetto è di grandi dimensioni o se vi sono molte dipendenze. Alcuni metodi di modifica di un elenco di attività possono essere più veloci di altri, a seconda del metodo selezionato per salvare le modifiche.

È possibile controllare quando Workfront salva le modifiche apportate alle attività in un elenco. Esistono i seguenti scenari: 

* Workfront può salvare automaticamente le modifiche dopo ogni aggiornamento.

  Per informazioni, consulta la sezione [Modifica le attività in un elenco e salva automaticamente le modifiche](#edit-tasks-in-a-list-and-automatically-save-changes) in questo articolo.

* È possibile controllare quando si applicano più modifiche contemporaneamente utilizzando manualmente un pulsante Salva.

  Per informazioni, consulta la sezione [Modificare le attività in un elenco e salvare manualmente le modifiche](#edit-tasks-in-a-list-and-manually-save-changes) in questo articolo.

### Modifica le attività in un elenco e salva automaticamente le modifiche {#edit-tasks-in-a-list-and-automatically-save-changes}

>[!TIP]
>
>Il salvataggio delle modifiche e di tutte le dipendenze del progetto potrebbe risultare più lento se il progetto contiene più di 2.000 attività o se presenta molte dipendenze.

Quando si salvano automaticamente le modifiche all&#39;elenco attività, tenere presente quanto segue:

* È possibile applicare una visualizzazione personalizzata all&#39;elenco delle attività e modificare qualsiasi campo relativo alle attività a cui si ha accesso per l&#39;aggiornamento.
* Impossibile annullare le modifiche salvate automaticamente. Questa è l&#39;impostazione predefinita.
* Workfront ricalcola automaticamente la timeline del progetto e tutte le dipendenze interne e tra progetti dopo ogni modifica, quando il tipo di aggiornamento del progetto è Automatico o Automatico e In caso di modifica. Per informazioni sul tipo di aggiornamento del progetto, vedi [Seleziona il tipo di aggiornamento del progetto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Per modificare le attività in un elenco e salvare automaticamente le modifiche:

1. Vai al progetto, quindi fai clic su **Attività** sezione.
1. Fai clic su **Menu della modalità Piano** ![](assets/qs-list-mode-or-save-mode-icon-small.png) nella parte superiore dell’elenco e assicurati che il **Salvataggio automatico** è selezionata.

   ![](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. Modifica qualsiasi campo per il quale disponi delle autorizzazioni necessarie per eseguire manualmente l’aggiornamento.

   ![](assets/inline-editing-a-task-350x26.png)

1. (Facoltativo) Premere **Escape** per annullare le modifiche.
1. Premi Invio per salvare le modifiche apportate alle attività e alla sequenza temporale del progetto.
1. (Facoltativo) Fai clic con il pulsante destro del mouse su un’attività da modificare.

   Oppure

   Fai clic su **Altro** menu ![](assets/more-icon-task-list.png) a destra del nome dell&#39;attività.

1. (Facoltativo) Seleziona una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Apri in una nuova scheda</strong></td> 
      <td>Apre l'attività in una nuova scheda del browser. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Modifica</strong></td> 
      <td><p>Apre il <strong>Modifica l'Attività</strong> , in cui è possibile modificare l'attività.</p><p>Per informazioni sulla modifica di un'attività, vedere <a href="#edit-tasks-in-a-list" class="MCXref xref">Modificare le attività in un elenco</a>.</p></td> 
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
      <td role="rowheader">Inserisci attività in alto</td> 
      <td>Inserisce un'attività sopra l'attività selezionata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserisci attività in basso</td> 
      <td>Inserisce un'attività sotto l'attività selezionata</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplica</td> 
      <td><p>Crea una versione duplicata dell'attività nello stesso progetto. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copia a</td> 
      <td><p>Copia l'attività in un altro progetto.</p><p>Per informazioni sulla copia e la duplicazione delle attività, vedere <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiare e duplicare le attività</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sposta a</td> 
      <td><p>Sposta l'attività in un altro progetto.</p><p>Per informazioni sullo spostamento delle attività, vedere <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">Sposta le attività</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

   Le modifiche vengono salvate automaticamente e non è possibile annullarle.

### Modificare le attività in un elenco e salvare manualmente le modifiche {#edit-tasks-in-a-list-and-manually-save-changes}

È possibile salvare manualmente le modifiche apportate alle attività in un elenco. Quando si salvano le modifiche in questo modo, è possibile annullarle prima di salvarle.

>[!TIP]
>
>* Non è possibile annullare le modifiche apportate alle attività in un elenco quando vengono modificate nella sezione Attività secondarie o in un report attività.
>* Non vi sono limiti al numero di modifiche che è possibile annullare. È possibile invertirli tutti singolarmente fino a raggiungere lo stato originale delle attività.
>

Quando si salvano manualmente le modifiche in un elenco di attività, tenere presente quanto segue:

* Per salvare manualmente le modifiche all&#39;elenco delle attività, è necessario disporre delle autorizzazioni per gestire sia le attività che il progetto.
* Non è possibile modificare il progetto. L’opzione per modificare il progetto è disabilitata.
* Non è possibile aggiornare le informazioni nell’intestazione del progetto. È possibile eseguire le operazioni seguenti solo quando si salvano manualmente le modifiche nell&#39;elenco delle attività:

   * Abbonati al progetto.
   * Aggiungi il progetto all’elenco dei preferiti.
   * Aprire un&#39;attività facendo clic sul relativo nome nell&#39;elenco.

* Modifica le attività in blocco. L&#39;icona Modifica è disattivata quando si selezionano più attività.
* Workfront attiva le notifiche sulle modifiche apportate alle attività solo dopo il salvataggio delle modifiche.

Esistono due modi per salvare manualmente le modifiche apportate alle attività in un elenco. Questi due modi sono descritti di seguito.

* [Salvare le modifiche in un elenco di operazioni manualmente quando si seleziona l&#39;opzione Salvataggio manuale standard](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [Salvare manualmente le modifiche in un elenco di task quando si seleziona l&#39;opzione Pianificazione manuale della sequenza temporale](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### Salvare le modifiche in un elenco di operazioni manualmente quando si seleziona l&#39;opzione Salvataggio manuale standard {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>Se il progetto contiene più di 2.000 attività o se presenta molte dipendenze, potrebbe essere necessario del tempo per identificare visivamente le modifiche apportate alle attività e il modo in cui tali modifiche influiscono su tutte le dipendenze del progetto. In questo caso, il salvataggio delle modifiche potrebbe richiedere più tempo se il progetto contiene più di 2.000 attività o se presenta molte dipendenze.

Quando si aggiornano le attività in un elenco dopo aver selezionato l&#39;opzione Salvataggio manuale standard, tenere presente quanto segue:

* È possibile applicare una visualizzazione personalizzata all&#39;elenco delle attività e modificare qualsiasi campo relativo alle attività per il quale si dispone delle autorizzazioni di gestione.
* Dopo aver fatto clic su Salva, Workfront calcola la timeline del progetto e tutte le dipendenze interne e tra progetti, se il tipo di aggiornamento del progetto è Automatico o Automatico e In caso di modifica. Per informazioni sul tipo di aggiornamento del progetto, vedi [Seleziona il tipo di aggiornamento del progetto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Per modificare i task in un elenco selezionando l&#39;opzione Salvataggio manuale standard:

1. Vai a un progetto, quindi fai clic su **Attività** sezione .
1. Fai clic su **Modalità pianificazione** menu ![](assets/qs-list-mode-or-save-mode-icon-small.png) nella parte superiore dell’elenco e seleziona **Salvataggio manuale**, quindi fai clic su **Standard** > **Applica**.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

   Viene visualizzata un’impostazione della barra degli strumenti con opzioni per annullare, ripetere e salvare le modifiche.

   ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Fai clic all’interno di qualsiasi campo per il quale disponi delle autorizzazioni necessarie per aggiornare manualmente. Il campo diventa modificabile e puoi apportare le modifiche.

   ![](assets/inline-editing-a-task-350x26.png)

1. Premi Invio per salvare temporaneamente le modifiche apportate.
1. (Facoltativo) Fai clic su **Icona Annulla** ![](assets/undo-icon-on-task-list.png) per annullare una modifica e ripristinare lo stato originale di un campo.
1. (Facoltativo e condizionale) Fai clic su **Icona Ripristina** ![](assets/redo-icon-on-task-list.png) per ripristinare la modifica annullata.

1. (Facoltativo) Fai clic con il pulsante destro del mouse su un’attività da modificare.

   Oppure

   Fai clic su **Altro** menu ![](assets/more-icon-task-list.png).

1. (Facoltativo) Seleziona una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Apri in una nuova scheda</strong> </td> 
      <td>Apre l'attività in una nuova scheda del browser. </td> 
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
      <td role="rowheader">Inserisci attività in alto</td> 
      <td>Inserisce un'attività sopra l'attività selezionata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserisci attività in basso</td> 
      <td>Inserisce un'attività sotto l'attività selezionata</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplica</td> 
      <td> <p>Crea una versione duplicata dell'attività nello stesso progetto. </p> <p>Per informazioni sulla copia e la duplicazione delle attività, vedere <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiare e duplicare le attività</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront aggiorna tutte le dipendenze interne e tra progetti quando si apportano modifiche alla sequenza temporale delle attività.
1. Clic **Salva** quando desideri mantenere le modifiche dell’attività in modo permanente e salvare la timeline del progetto.

#### Salvare manualmente le modifiche in un elenco di task quando si seleziona l&#39;opzione Pianificazione manuale della sequenza temporale {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

Salvare le modifiche e tutte le dipendenze del progetto è più veloce. Questa opzione non è disponibile per i progetti con più di 2.000 attività.

>[!IMPORTANT]
>
>È consigliabile utilizzare questa opzione quando si modifica un elenco esteso di attività con più di poche centinaia di dipendenti. Questa opzione consente di identificare visivamente le modifiche molto più rapidamente rispetto all’opzione Salvataggio manuale.

Quando si utilizza l&#39;opzione Pianificazione manuale della sequenza temporale in un elenco di task, tenere presente quanto segue:

* Non è possibile applicare l&#39;opzione Pianificazione sequenza temporale salvataggio manuale ai progetti con più di 2.000 task.
* Non è possibile applicare una visualizzazione, un filtro o un raggruppamento personalizzato all&#39;elenco delle attività. I menu a discesa Visualizza, Filtro e Raggruppamento, nonché l’icona della vista Agile, sono disattivati. La visualizzazione applicata per impostazione predefinita contiene un numero limitato di campi.
* La timeline del progetto e tutte le dipendenze interne al progetto vengono calcolate automaticamente dopo ogni modifica quando il tipo di aggiornamento del progetto è Automatico o Automatico e In caso di modifica.
* Le dipendenze tra progetti vengono calcolate dopo aver fatto clic su Salva, quando il tipo di aggiornamento del progetto è Automatico o Automatico e su Modifica. Per informazioni sul tipo di aggiornamento del progetto, vedi [Seleziona il tipo di aggiornamento del progetto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Per modificare i task in un elenco quando si utilizza l&#39;opzione Pianificazione manuale del salvataggio della sequenza temporale:

1. Vai a un progetto, quindi fai clic su **Attività** sezione.
1. Fai clic su **Modalità pianificazione** menu ![](assets/qs-list-mode-or-save-mode-icon-small.png) nella parte superiore dell’elenco e seleziona **Salvataggio manuale**, quindi fai clic su **Pianificazione sequenza temporale**> **Applica**.

   Questa opzione è disattivata per i progetti con più di 2.000 attività.

   ![](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >Quando ci si sposta dalla pagina, Workfront riattiva l&#39;opzione Salvataggio automatico.

   Osserva le seguenti modifiche nell’elenco:

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

     ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Modifica qualsiasi campo per il quale disponi delle autorizzazioni necessarie per eseguire manualmente l’aggiornamento.

   ![](assets/inline-editing-a-task-350x26.png)

1. Premi Invio per salvare temporaneamente le modifiche apportate.
1. (Facoltativo) Fai clic su **Icona Annulla** ![](assets/undo-icon-on-task-list.png) per annullare una modifica e ripristinare lo stato originale di un campo.
1. (Facoltativo e condizionale) Fai clic su **Icona Ripristina** ![](assets/redo-icon-on-task-list.png) per ripristinare la modifica annullata.

1. (Facoltativo) Fai clic con il pulsante destro del mouse su un’attività da modificare

   Oppure

   Fai clic su **Altro** menu ![](assets/more-icon-task-list.png).

1. Selezionare una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Apri in una nuova scheda</strong> </td> 
      <td>Apre l'attività in una nuova scheda del browser. </td> 
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
      <td role="rowheader">Inserisci attività in alto</td> 
      <td>Inserisce un'attività sopra l'attività selezionata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserisci attività in basso</td> 
      <td>Inserisce un'attività sotto l'attività selezionata</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplica</td> 
      <td> <p>Crea una versione duplicata dell'attività nello stesso progetto. </p> <p>Per informazioni sulla copia e la duplicazione delle attività, vedere <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copiare e duplicare le attività</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Quando si modifica la sequenza temporale di un&#39;attività, Workfront aggiorna tutte le dipendenze interne e tra progetti.
1. Clic **Salva** quando desideri mantenere le modifiche dell’attività in modo permanente e salvare la timeline del progetto.

## Modificare un&#39;attività in un elenco utilizzando il Riepilogo

1. Passare al progetto contenente le attività da modificare.
1. Clic **Attività** nel pannello a sinistra.

   Viene visualizzato l’elenco delle attività sul progetto.

1. Fare clic sul menu Altro ![](assets/more-icon-task-list.png) dopo il nome dell’attività, quindi fai clic su **Apri riepilogo**. Seleziona l’attività da modificare, quindi fai clic su **Icona Apri riepilogo** ![](assets/qs-open-summary-icon-in-new-toolbar-small.png) nell&#39;angolo superiore destro dell&#39;elenco.

   Il **Riepilogo** viene aperto.

   ![](assets/qs-task-right-panel-in-a-task-list-350x328.png)

1. (Facoltativo) Fai clic su **Icona X** in alto a destra nel Riepilogo per chiudere il pannello e modificare le attività in linea.

   Per modificare l’attività in linea, segui i passaggi relativi alla modifica di un’attività in un elenco.

   Per informazioni sulla modifica dell&#39;attività in un elenco, vedere [Considerazioni sulla modifica delle attività in un elenco](#considerations-about-editing-tasks-in-a-list) in questo articolo.

1. (Facoltativo) Immetti un aggiornamento per l’attività nella **Aggiornamenti** area.
1. Fare clic su una delle icone o aree seguenti per accedere all&#39;attività e modificare le informazioni a livello di attività:

   | Documenti | Clic **Fai clic qui per aggiungere** per aggiungere documenti all&#39;attività. |
   |---|---|
   | Dettagli | Fare clic per aggiornare le informazioni sull&#39;attività. |
   | Moduli personalizzati | Fare clic per aggiungere o rimuovere Forms personalizzato o aggiornare le informazioni nei moduli. |
   | Ore | Fai clic su per registrare le ore. |
   | Approvazioni | Fai clic su per aggiungere approvazioni attività. |

   {style="table-layout:auto"}

1. Fare clic sul pulsante Indietro del browser per tornare all&#39;elenco delle attività al termine dell&#39;aggiornamento dell&#39;attività.

## Modifica attività in blocco

È possibile modificare più attività contemporaneamente. Assicurarsi di disporre delle autorizzazioni di gestione per le attività per poterle modificare.

1. Passare a un progetto contenente attività che si desidera modificare in blocco.
1. Clic **Attività** nel pannello a sinistra.
1. Assicurati che **Salvataggio automatico** è selezionata.

   >[!IMPORTANT]
   >
   >Non è possibile modificare le attività in blocco quando si salvano le attività manualmente.

   Per ulteriori informazioni sulle modalità di salvataggio delle modifiche apportate alle attività in un elenco, vedere la sezione [Considerazioni sulla modifica delle attività in un elenco](#considerations-about-editing-tasks-in-a-list) in questo articolo.

1. Selezionare più attività nell&#39;elenco delle attività.
1. Fai clic su **Icona Modifica** ![](assets/qs-edit-icon.png).

   Il **Modifica le Attività** viene visualizzata.

1. Specificare le informazioni da modificare per tutte le attività selezionate.

   La modifica delle informazioni su tutte le attività è identica alla modifica delle informazioni su un&#39;attività. Se si desidera modificare la durata dell&#39;attività, le attività selezionate devono avere lo stesso vincolo attività; in caso contrario, **Durata** non viene compilato.

   Per ulteriori informazioni sulla modifica di un&#39;attività, vedere [Modifica attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   >[!NOTE]
   >
   >Le informazioni che si stanno modificando su tutte le attività selezionate sostituiranno le informazioni esistenti sulle singole attività, ad eccezione delle **Assegnazioni** campo. L&#39;aggiunta di un nuovo assegnatario nella modifica in blocco aggiungerà l&#39;assegnatario a tutte le attività selezionate. Se alle attività selezionate vengono assegnati altri assegnatari, questi rimarranno assegnati in aggiunta a quelli aggiunti tramite la modifica in blocco.

1. Clic **Forms personalizzato** per modificare i moduli personalizzati allegati a tutte le attività selezionate. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi.

   Se le attività selezionate non hanno moduli personalizzati comuni, in questa sezione non sono elencati moduli.

   È possibile modificare solo i campi dei moduli allegati a tutte le attività selezionate e per i quali si dispone delle autorizzazioni di modifica.

1. (Facoltativo) Nella sezione Forms personalizzato, seleziona la **Ricalcolare Espressioni Personalizzate** per garantire che tutti i campi personalizzati calcolati presenti nei moduli personalizzati allegati alle attività selezionate siano aggiornati.
1. Fai clic su **Salva modifiche**.

   Tutte le modifiche apportate sono ora visibili in tutte le attività selezionate.

Per informazioni sulla modifica in blocco di moduli personalizzati, consulta la sezione &quot;Modificare più Forms personalizzati durante la modifica in blocco di oggetti&quot; in [Gestire i moduli personalizzati allegati agli oggetti](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).
