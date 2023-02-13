---
product-area: projects
navigation-topic: manage-tasks
title: Modificare le attività in un elenco
description: È possibile modificare le informazioni sulle attività in un elenco di attività modificando i campi visualizzati nell'elenco. Per informazioni su altri modi per modificare le attività, vedere Modifica delle attività.
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '2828'
ht-degree: 2%

---

# Modificare le attività in un elenco {#edit-tasks-in-a-list}

È possibile modificare le informazioni sulle attività in un elenco di attività modificando i campi visualizzati nell&#39;elenco. Per informazioni su altri modi per modificare le attività, consulta [Modifica delle attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l’accesso a Attività e Progetti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Collaborare o autorizzazioni superiori per l'attività e il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Considerazioni sulla modifica delle attività in un elenco {#considerations-about-editing-tasks-in-a-list}

La modifica delle attività in un elenco consente di apportare modifiche rapide a più attività contemporaneamente, in modo da visualizzare in modo chiaro in che modo le modifiche potrebbero influenzare la timeline del progetto.

Quando si modificano le attività in un elenco, tenere presente quanto segue:

* Diversamente dalla necessità di autorizzazioni di gestione per l&#39;attività quando viene modificata nella casella di modifica, è possibile modificare un&#39;attività in un elenco solo con le autorizzazioni di Contribute per l&#39;attività. Questo consente di modificare le seguenti informazioni limitate per l’attività:

   * Descrizione
   * Stato
   * Percentuale completato
   * Informazioni sul modulo personalizzato

      >[!NOTE]
      >
      >È possibile modificare un campo personalizzato dell’attività in un elenco solo se si dispone delle autorizzazioni necessarie per aggiornare il campo.

   * Ore di log
   * Modifica assegnazioni
   * Visualizza informazioni finanziarie
   * Aggiungere spese, attività o problemi

* È possibile modificare un’attività negli elenchi seguenti:

   * Sezione Attività del progetto
   * Sezione Sottoattività del progetto
   * Rapporto attività

      >[!NOTE]
      >
      >Per impostazione predefinita, Workfront salva automaticamente le modifiche apportate alle attività nella sezione Sottoattività o in un rapporto delle attività.

* È possibile controllare quando Workfront salva le modifiche apportate alle attività in un elenco. Le modifiche possono essere salvate automaticamente o salvate manualmente.

   Per informazioni su come configurare quando Workfront salva le modifiche apportate alle attività in un elenco, consulta la [Selezionare un&#39;opzione di salvataggio durante la modifica di attività in un elenco](#select-a-save-option-when-editing-tasks-in-a-list) in questo articolo.

## Selezionare un&#39;opzione di salvataggio durante la modifica di attività in un elenco {#select-a-save-option-when-editing-tasks-in-a-list}

È possibile decidere dove le modifiche apportate alle attività di un elenco vengono salvate automaticamente, in base al loro verificarsi o se si desidera salvare manualmente ogni modifica.

>[!IMPORTANT]
>
>A seconda che le attività vengano salvate automaticamente o manualmente, è possibile sovrascrivere le informazioni di qualcun altro durante la modifica delle attività in un elenco. Per informazioni sul modo in cui Workfront salva le modifiche alle attività che convengono con altri utenti, consulta [Panoramica del salvataggio delle modifiche simultanee all&#39;interno di un elenco di attività](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

Quando si salvano le modifiche in un elenco per un progetto con l’opzione Automatico o Automatico e l’opzione Su modifica selezionata come Tipo di aggiornamento, Workfront aggiorna la timeline del progetto, insieme a tutte le dipendenze tra progetti e progetti. I calcoli della timeline possono richiedere molto tempo se il progetto è di grandi dimensioni o se sono presenti molte dipendenze. Alcuni metodi per modificare un elenco di attività possono essere più veloci di altri, a seconda del metodo selezionato per salvare le modifiche.

È possibile controllare quando Workfront salva le modifiche apportate alle attività in un elenco. Esistono i seguenti scenari: 

* Dopo ogni aggiornamento, Workfront può salvare automaticamente le modifiche.

   Per informazioni, consulta la sezione . [Modificare le attività in un elenco e salvare automaticamente le modifiche](#edit-tasks-in-a-list-and-automatically-save-changes) in questo articolo.

* Puoi avere il controllo su quando applicare più modifiche alla volta utilizzando manualmente un pulsante Salva.

   Per informazioni, consulta la sezione . [Modificare le attività in un elenco e salvare manualmente le modifiche](#edit-tasks-in-a-list-and-manually-save-changes) in questo articolo.

### Modificare le attività in un elenco e salvare automaticamente le modifiche {#edit-tasks-in-a-list-and-automatically-save-changes}

>[!TIP]
>
>Il salvataggio delle modifiche e di tutte le dipendenze del progetto potrebbe essere più lento se il progetto ha più di 2000 attività o se ha molte dipendenze.

Quando si salva automaticamente l&#39;elenco delle attività, tenere presente quanto segue:

* È possibile applicare una visualizzazione personalizzata all&#39;elenco delle attività e modificare tutti i campi relativi alle attività che è possibile aggiornare.
* Non è possibile annullare le modifiche salvate automaticamente. Questa è l’impostazione predefinita.
* Workfront ricalcola automaticamente la timeline del progetto e tutte le dipendenze tra progetti e progetti dopo ogni modifica, quando il tipo di aggiornamento del progetto è Automatico o Automatico e In caso di modifica. Per informazioni sul tipo di aggiornamento del progetto, consulta [Seleziona il tipo di aggiornamento del progetto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Per modificare le attività in un elenco e salvare automaticamente le modifiche:

1. Vai al progetto, quindi fai clic sul pulsante **Attività** sezione .
1. Fai clic sul pulsante **Menu della modalità Piano** ![](assets/qs-list-mode-or-save-mode-icon-small.png) in cima all&#39;elenco e assicurati che il **Salvataggio automatico** è selezionata.

   ![](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. Modifica qualsiasi campo per cui disponi delle autorizzazioni per l’aggiornamento manuale.

   ![](assets/inline-editing-a-task-350x26.png)

1. (Facoltativo) Premere **Esc** per annullare le modifiche.
1. Premi Invio per salvare le modifiche apportate alle attività e alla timeline del progetto.
1. (Facoltativo) Fai clic con il pulsante destro del mouse su un&#39;attività da modificare.

   Oppure

   Fai clic sul pulsante **Altro** menu ![](assets/more-icon-task-list.png) a destra del nome dell&#39;attività.

1. (Facoltativo) Seleziona tra le seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Apri in una nuova scheda</strong></td> 
      <td>Apre l’attività in una nuova scheda del browser. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Modifica</strong></td> 
      <td><p>Apre la <strong>Modifica attività</strong> in cui è possibile modificare l’attività.</p><p>Per informazioni sulla modifica di un’attività, consulta <a href="#edit-tasks-in-a-list" class="MCXref xref">Modificare le attività in un elenco</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Elimina</td> 
      <td><p>Elimina l'attività.</p><p>Per informazioni sull'eliminazione delle attività, vedere <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Elimina attività</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rientro</td> 
      <td><p>Fa rientrare l’attività di un livello. </p><p>Questa opzione viene visualizzata solo su attività autonome.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rientro negativo</td> 
      <td><p>Esclude l'attività di un livello. </p><p>Questa opzione viene visualizzata solo sulle attività secondarie. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserisci attività in alto</td> 
      <td>Inserisce un’attività sopra l’attività selezionata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserisci attività in basso</td> 
      <td>Inserisce un’attività sotto l’attività selezionata</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplica</td> 
      <td><p>Crea una versione duplicata dell’attività all’interno dello stesso progetto. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copia a</td> 
      <td><p>Copia l’attività in un altro progetto.</p><p>Per informazioni sulla copia e la duplicazione delle attività, consulta <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copia e duplica le attività</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sposta a</td> 
      <td><p>Sposta l'attività in un altro progetto.</p><p>Per informazioni sullo spostamento delle attività, consulta <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">Sposta attività</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

   Le modifiche vengono salvate automaticamente e non è possibile annullarle.

### Modificare le attività in un elenco e salvare manualmente le modifiche {#edit-tasks-in-a-list-and-manually-save-changes}

È possibile salvare manualmente le modifiche apportate alle attività in un elenco. Quando si salvano le modifiche in questo modo, è possibile invertire le modifiche prima di salvarle.

>[!TIP]
>
>* Non è possibile annullare le modifiche apportate alle attività in un elenco quando vengono modificate nella sezione Sottoattività o in un rapporto di attività.
>* Non esistono limitazioni sul numero di modifiche che è possibile annullare. È possibile annullare tutte le attività una per una fino a raggiungere lo stato originale delle attività.
>


Quando si salvano manualmente le modifiche in un elenco di attività, tenere presente quanto segue:

* Per salvare manualmente le modifiche all’elenco delle attività, è necessario disporre delle autorizzazioni per gestire sia le attività che il progetto.
* Non è possibile modificare il progetto. L’opzione per modificare il progetto è disabilitata.
* Non è possibile aggiornare le informazioni nell’intestazione del progetto. È possibile eseguire le operazioni seguenti solo quando si salvano manualmente le modifiche nell&#39;elenco delle attività:

   * Iscriviti al progetto.
   * Aggiungi il progetto all’elenco dei preferiti.
   * Apri un’attività facendo clic sul nome corrispondente nell’elenco.

* Modifica le attività in blocco. L’icona Modifica è disabilitata quando si selezionano più attività.
* Workfront attiva le notifiche sulle modifiche apportate alle attività solo dopo aver salvato le modifiche.

Esistono due modi per salvare manualmente le modifiche alle attività in un elenco. Questi due modi sono descritti di seguito.

* [Salvare manualmente le modifiche in un elenco di attività quando si seleziona l’opzione Salva manuale standard](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [Salvare manualmente le modifiche in un elenco di attività quando si seleziona l&#39;opzione Salva manuale pianificazione timeline](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### Salvare manualmente le modifiche in un elenco di attività quando si seleziona l’opzione Salva manuale standard {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>Se il progetto ha più di 2000 attività o se ha molte dipendenze, potrebbe essere necessario un po&#39; di tempo per identificare visivamente le modifiche apportate alle attività e il modo in cui tali modifiche influiscono su tutte le dipendenze del progetto. In questo caso, il salvataggio delle modifiche potrebbe richiedere più tempo se il progetto ha più di 2000 attività o se presenta molte dipendenze.

Quando si aggiornano le attività in un elenco dopo aver selezionato l&#39;opzione Salva manuale standard, tenere presente quanto segue:

* È possibile applicare una visualizzazione personalizzata all&#39;elenco delle attività e modificare tutti i campi relativi alle attività che si dispone delle autorizzazioni per gestire in tale visualizzazione.
* Dopo aver fatto clic su Salva, Workfront calcola la timeline del progetto e tutte le dipendenze tra progetti e progetti, quando il tipo di aggiornamento del progetto è Automatico o Automatico e In caso di modifica. Per informazioni sul tipo di aggiornamento del progetto, consulta [Seleziona il tipo di aggiornamento del progetto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Per modificare le attività in un elenco quando si seleziona l’opzione Salva manuale standard:

1. Passa a un progetto, quindi fai clic sul pulsante **Attività** sezione .
1. Fai clic sul pulsante **Modalità piano** menu ![](assets/qs-list-mode-or-save-mode-icon-small.png) in alto nell’elenco e seleziona **Salvataggio manuale**, quindi fai clic su **Standard** > **Applica**.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

   Viene visualizzata un’impostazione della barra degli strumenti con le opzioni per annullare, ripristinare e salvare le modifiche.

   ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Fai clic all’interno di qualsiasi campo per il quale disponi delle autorizzazioni per l’aggiornamento manuale. Il campo diventa modificabile ed è possibile apportare le modifiche desiderate.

   ![](assets/inline-editing-a-task-350x26.png)

1. Premi Invio per salvare temporaneamente le modifiche apportate.
1. (Facoltativo) Fai clic sul pulsante **Icona Annulla** ![](assets/undo-icon-on-task-list.png) per annullare una modifica e ripristinare lo stato originale di un campo.
1. (Facoltativo e condizionale) Fai clic sul pulsante **Icona Ripristina** ![](assets/redo-icon-on-task-list.png) per ripristinare la modifica annullata.

1. (Facoltativo) Fare clic con il pulsante destro del mouse su un&#39;attività da modificare.

   Oppure

   Fai clic sul pulsante **Altro** menu ![](assets/more-icon-task-list.png).

1. (Facoltativo) Seleziona tra le seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Apri in una nuova scheda</strong> </td> 
      <td>Apre l’attività in una nuova scheda del browser. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Elimina</td> 
      <td>Per informazioni sull'eliminazione delle attività, vedere <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Elimina attività</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rientro</td> 
      <td> <p>Fa rientrare l’attività di un livello. </p> <p>Questa opzione viene visualizzata solo su attività autonome.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rientro negativo</td> 
      <td> <p>Esclude l'attività di un livello. </p> <p>Questa opzione viene visualizzata solo sulle attività secondarie. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserisci attività in alto</td> 
      <td>Inserisce un’attività sopra l’attività selezionata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserisci attività in basso</td> 
      <td>Inserisce un’attività sotto l’attività selezionata</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplica</td> 
      <td> <p>Crea una versione duplicata dell’attività all’interno dello stesso progetto. </p> <p>Per informazioni sulla copia e la duplicazione delle attività, consulta <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copia e duplica le attività</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront aggiorna tutte le dipendenze tra progetti e progetti quando apporti modifiche alla timeline delle attività.
1. Fai clic su **Salva** per mantenere le modifiche dell’attività in modo permanente e salvare la timeline del progetto.

#### Salvare manualmente le modifiche in un elenco di attività quando si seleziona l&#39;opzione Salva manuale pianificazione timeline {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

Il salvataggio delle modifiche e di tutte le dipendenze del progetto è più rapido. Non è disponibile per progetti con più di 2000 attività.

>[!IMPORTANT]
>
>Si consiglia di utilizzare questa opzione quando si modifica un lungo elenco di attività con più di poche centinaia di dipendenze. L’utilizzo di questa opzione consente di identificare visivamente le modifiche molto più rapidamente rispetto all’utilizzo dell’opzione Salva manuale.

Quando si utilizza l&#39;opzione Salva manuale pianificazione timeline in un elenco di attività, tenere presente quanto segue:

* Non è possibile applicare l&#39;opzione Salva manuale pianificazione temporale a progetti con più di 2000 attività.
* Non è possibile applicare una visualizzazione, un filtro o un raggruppamento personalizzati all&#39;elenco delle attività. I menu a discesa Visualizza, Filtro e Raggruppamento e l’icona di visualizzazione Agile sono disattivati. La visualizzazione applicata per impostazione predefinita contiene un numero limitato di campi.
* La timeline del progetto e di tutte le dipendenze del progetto vengono calcolate automaticamente dopo ogni modifica quando il tipo di aggiornamento del progetto è Automatico o Automatico e In caso di modifica.
* Le dipendenze tra progetti vengono calcolate dopo aver fatto clic su Salva, quando il tipo di aggiornamento del progetto è Automatico o Automatico e su Modifica. Per informazioni sul tipo di aggiornamento del progetto, consulta [Seleziona il tipo di aggiornamento del progetto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Per modificare le attività in un elenco quando si utilizza l&#39;opzione Salva manuale pianificazione timeline:

1. Passa a un progetto, quindi fai clic sul pulsante **Attività** sezione .
1. Fai clic sul pulsante **Modalità piano** menu ![](assets/qs-list-mode-or-save-mode-icon-small.png) in alto nell’elenco e seleziona **Salvataggio manuale**, quindi fai clic su **Pianificazione temporale**> **Applica**.

   Questa opzione è oscurata per i progetti con più di 2000 attività.

   ![](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >Quando ti allontani da questa pagina, Workfront riattiva l’opzione Salvataggio automatico .

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
   * Viene visualizzata un’impostazione della barra degli strumenti con le opzioni per annullare, ripristinare e salvare le modifiche.

      ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)


1. Modifica qualsiasi campo per cui disponi delle autorizzazioni per l’aggiornamento manuale.

   ![](assets/inline-editing-a-task-350x26.png)

1. Premi Invio per salvare temporaneamente le modifiche apportate.
1. (Facoltativo) Fai clic sul pulsante **Icona Annulla** ![](assets/undo-icon-on-task-list.png) per annullare una modifica e ripristinare lo stato originale di un campo.
1. (Facoltativo e condizionale) Fai clic sul pulsante **Icona Ripristina** ![](assets/redo-icon-on-task-list.png) per ripristinare la modifica annullata.

1. (Facoltativo) Fai clic con il pulsante destro del mouse su un&#39;attività da modificare

   Oppure

   Fai clic sul pulsante **Altro** menu ![](assets/more-icon-task-list.png).

1. Seleziona tra le seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Apri in una nuova scheda</strong> </td> 
      <td>Apre l’attività in una nuova scheda del browser. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Elimina</td> 
      <td>Per informazioni sull'eliminazione delle attività, vedere <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Elimina attività</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rientro</td> 
      <td> <p>Fa rientrare l’attività di un livello. </p> <p>Questa opzione viene visualizzata solo su attività autonome.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rientro negativo</td> 
      <td> <p>Esclude l'attività di un livello. </p> <p>Questa opzione viene visualizzata solo sulle attività secondarie. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserisci attività in alto</td> 
      <td>Inserisce un’attività sopra l’attività selezionata.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inserisci attività in basso</td> 
      <td>Inserisce un’attività sotto l’attività selezionata</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplica</td> 
      <td> <p>Crea una versione duplicata dell’attività all’interno dello stesso progetto. </p> <p>Per informazioni sulla copia e la duplicazione delle attività, consulta <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Copia e duplica le attività</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Quando si modifica la timeline di un’attività, Workfront aggiorna tutte le dipendenze tra progetti e progetti.
1. Fai clic su **Salva** per mantenere le modifiche dell’attività in modo permanente e salvare la timeline del progetto.

## Modificare un’attività in un elenco utilizzando il Riepilogo

1. Passa al progetto contenente le attività da modificare.
1. Fai clic su **Attività** nel pannello a sinistra.

   Viene visualizzato l’elenco delle attività del progetto.

1. Fai clic sul menu Altro ![](assets/more-icon-task-list.png) dopo il nome dell&#39;attività, fai clic su **Apri riepilogo**. Seleziona l’attività da modificare, quindi fai clic sul pulsante **Icona Apri riepilogo** ![](assets/qs-open-summary-icon-in-new-toolbar-small.png) nell&#39;angolo superiore destro dell&#39;elenco.

   La **Riepilogo** si apre.

   ![](assets/qs-task-right-panel-in-a-task-list-350x328.png)

1. (Facoltativo) Fai clic sul pulsante **Icona X** in alto a destra in Riepilogo per chiudere il pannello e modificare le attività in linea.

   Segui i passaggi per modificare un’attività in un elenco per modificarla in linea.

   Per informazioni sulla modifica dell’attività in un elenco, consulta [Considerazioni sulla modifica delle attività in un elenco](#considerations-about-editing-tasks-in-a-list) in questo articolo.

1. (Facoltativo) Digita un aggiornamento per l’attività nel **Aggiornamenti** area.
1. Fare clic su una delle icone o aree seguenti per passare all&#39;attività e modificare le informazioni a livello di attività:

   | Documenti | Fai clic su **Fai clic qui per aggiungere** per aggiungere documenti all&#39;attività. |
   |---|---|
   | Dettagli | Fai clic su per aggiornare le informazioni sull’attività. |
   | Moduli personalizzati | Fare clic per aggiungere o rimuovere Custom Forms o per aggiornare le informazioni sui moduli. |
   | Ore | Fai clic su per registrare le ore. |
   | Approvazioni | Fare clic su per aggiungere le approvazioni delle attività. |

   {style=&quot;table-layout:auto&quot;}

1. Fai clic sul pulsante Indietro del browser per tornare all’elenco delle attività al termine dell’aggiornamento dell’attività.

## Modifica in blocco le attività

È possibile modificare più attività contemporaneamente. Assicurati di disporre delle autorizzazioni di gestione per le attività per poterle modificare.

1. Passa a un progetto contenente attività da modificare in blocco.
1. Fai clic su **Attività** nel pannello a sinistra.
1. Assicurati che **Salvataggio automatico** è selezionata.

   >[!IMPORTANT]
   >
   >Non è possibile modificare le attività in blocco quando si salvano le attività manualmente.

   Per ulteriori informazioni sulle modalità di salvataggio delle modifiche apportate alle attività in un elenco, vedere la sezione [Considerazioni sulla modifica delle attività in un elenco](#considerations-about-editing-tasks-in-a-list) in questo articolo.

1. Selezionare diverse attività nell&#39;elenco delle attività.
1. Fai clic sul pulsante **Icona Modifica** ![](assets/qs-edit-icon.png).

   La **Modifica attività** viene visualizzata la finestra di dialogo.

1. Specificare le informazioni che si desidera modificare per tutte le attività selezionate.

   La modifica delle informazioni su tutte le attività è identica alla modifica delle informazioni su un&#39;attività. Se si desidera modificare la durata dell&#39;attività, le attività selezionate devono avere lo stesso Vincolo di attività; altrimenti, **Durata** il campo non viene compilato.

   Per ulteriori informazioni sulla modifica di un’attività, consulta [Modifica delle attività](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   >[!NOTE]
   >
   >Le informazioni che si stanno modificando su tutte le attività selezionate sostituiranno quelle esistenti sulle singole attività, ad eccezione delle **Assegnazioni** campo . L’aggiunta di un nuovo assegnatario nella modifica collettiva aggiunge tale assegnatario a tutte le attività selezionate. Se altri assegnatari vengono assegnati alle attività selezionate, rimarranno assegnati in aggiunta a quello aggiunto tramite la modifica collettiva.

1. Fai clic su **Forms personalizzato** per modificare i moduli personalizzati associati a tutte le attività selezionate. Nell’elenco vengono visualizzati solo i moduli personalizzati attivi.

   Se le attività selezionate non dispongono di moduli personalizzati comuni, in questa sezione non sono elencati moduli.

   È possibile modificare solo i campi dei moduli associati a tutte le attività selezionate e che si dispone delle autorizzazioni di modifica.

1. (Facoltativo) Nella sezione Forms personalizzato, seleziona la **Ricalcola espressioni personalizzate** per garantire che tutti i campi personalizzati calcolati presenti nei moduli personalizzati associati alle attività selezionate siano aggiornati.
1. Fai clic su **Salva modifiche**.

   Tutte le modifiche apportate sono ora visibili su tutte le attività selezionate.

Per informazioni sulla modifica collettiva di moduli personalizzati, vedere la sezione &quot;Modificare più Forms personalizzati durante la modifica collettiva di oggetti&quot; in [Gestione di moduli personalizzati associati agli oggetti](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).
