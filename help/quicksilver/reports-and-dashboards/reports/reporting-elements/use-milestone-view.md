---
product-area: reporting
navigation-topic: reporting-elements
title: Utilizzare la vista Milestone
description: Puoi applicare la vista Milestone (Attività cardine) a un elenco o a un rapporto di progetto.
author: Nolan
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: 32da139d7385e05436a669bdc6f36b71ad83c8d2
workflow-type: tm+mt
source-wordcount: '1291'
ht-degree: 0%

---

# Utilizzare la vista Milestone

<!-- Audited: 1/2024 -->

Puoi applicare la vista Milestone (Attività cardine) a un elenco o a un rapporto di progetto.

Prima di poter utilizzare la vista milestone, è necessario configurare i milestone, aggiungere i percorsi ai progetti e associare i milestone alle attività, come descritto negli articoli [Creare un percorso milestone](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) e [Associa attività cardine ad attività](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

La vista Milestone (Attività cardine) è disponibile quando si visualizza un elenco di progetti o un rapporto di progetto. Nelle sezioni seguenti viene descritto come visualizzare e utilizzare la vista milestone.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>piano Adobe Workfront</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront</strong></td> 
   <td> 
   <p>Nuovo: Standard</p>
   <p>Corrente: Lavoro o versione successiva </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>Accesso di visualizzazione o superiore a report, dashboard, calendari</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Visualizzare le autorizzazioni per un report di progetti per applicare la vista Milestone a un report</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Passa alla vista Milestone {#switch-to-the-milestone-view}

{{step1-to-projects}}

1. Fai clic su **Visualizza** menu a discesa, quindi fai clic su **Milestone**.

   L’elenco o il rapporto viene visualizzato in una vista Milestone.

   Per informazioni sulla vista milestone, consulta la sezione [Panoramica della vista Milestone](#milestone-view-overview) in questo articolo.

## Panoramica della vista Milestone {#milestone-view-overview}

La vista Milestone (Attività cardine) è disponibile negli elenchi dei progetti e nei rapporti sui progetti. Questa visualizzazione consente di visualizzare rapidamente tutte le attività cardine associate alle attività all&#39;interno dei progetti visualizzati.


>[!NOTE]
>
>La vista Milestone (Attività cardine) non è disponibile nelle seguenti aree:
>
>* Schede orario, nell’elenco dei progetti quando si aggiunge un progetto.


Per informazioni su come passare alla vista Milestone, consulta la sezione [Passa alla vista Milestone](#switch-to-the-milestone-view) in questo articolo.

![Progetto con vista milestone](assets/project-with-milestone-view-with-complete.png)

### Sezioni della vista Milestone

Quando si applica la vista Milestone (Attività cardine) a un elenco di progetti, i progetti vengono visualizzati nelle sezioni seguenti:

* I progetti associati a un Percorso milestone vengono visualizzati per primi, elencati sotto il nome dei rispettivi Percorsi milestone.

  Workfront ordina i progetti nella prima sezione in base ai seguenti criteri, nell’ordine indicato:

   1. ID Percorso Milestone. Puoi visualizzare l’ID del percorso milestone in un rapporto del percorso milestone.

   2. Il campo selezionato come primo campo di ordinamento per l’elenco dei progetti nella vista precedentemente applicata all’elenco dei progetti, prima di selezionare la vista Milestone (Attività cardine).

* I progetti non associati a un Percorso Milestobe vengono visualizzati accanto, nella sezione Non assegnato. Workfront ordina i progetti nella sezione Non assegnato in base al campo selezionato come primo campo di ordinamento per l’elenco dei progetti nella vista precedentemente applicata all’elenco dei progetti, prima di selezionare la vista Milestone.

### Informazioni sul progetto nella vista Milestone

Quando si visualizza l’elenco o il rapporto di un progetto nella vista Milestone (Attività cardine), sono disponibili le seguenti informazioni:

* **Date pianificate o date previste:** Specifica se visualizzare le date pianificate o previste nella vista Milestone.\
  Vengono visualizzate le date di inizio e completamento, nonché di ogni attività cardine all’interno del Percorso attività cardine.\
  Se si visualizzano le Date pianificate e si dispone anche dell&#39;accesso Gestisci al progetto, è possibile modificare le date seguenti direttamente dalla vista Milestone (se si visualizzano le Date previste, le date non possono essere modificate perché le Date previste sono calcolate e non possono essere modificate manualmente).

   * **Date di inizio progetto:** Se un progetto è programmato a partire dalla data di inizio, è possibile modificare manualmente la data di inizio del progetto e quindi calcolare la data di completamento.
   * **Date di completamento progetto:** Se un progetto è programmato a partire dalla data di completamento, è possibile modificare manualmente la data di completamento del progetto e quindi calcolare la data di inizio.
   * **Date di completamento attività:** È possibile aggiornare manualmente il completamento delle attività direttamente dalla vista Milestone.

* **Percentuale completamento:** Visualizza la percentuale di completamento di ogni attività e progetto.\
  Puoi disattivare la visualizzazione della percentuale di completamento, come descritto nella sezione [Configurare le informazioni da visualizzare nella vista Milestone](#configure-what-information-displays-in-the-milestone-view) in questo articolo.\
  Puoi regolare la percentuale di completamento direttamente dalla vista Milestone, come descritto nella sezione [Regola percentuale di completamento per le attività nella vista Milestone](#adjust-percent-complete-for-tasks-in-the-milestone-view) in questo articolo.

* **Icone di stato attività:** Accanto a ogni progetto e attività nella vista Milestone viene visualizzata un&#39;icona di stato.

   * Nei Tempi\
     ![](assets/gantt-ontime.png)

   * Indietro\
     ![](assets/gantt-behind.png)

   * A Rischio\
     ![](assets/gantt-atrisk.png)

   * In Ritardo\
     ![](assets/gantt-late.png)

  È possibile disattivare la visualizzazione di queste icone di stato, come descritto nella sezione [Configurare le informazioni da visualizzare nella vista Milestone](#configure-what-information-displays-in-the-milestone-view) in questo articolo.\
  Per informazioni più dettagliate su ciascun tipo di stato, consulta l’articolo [Panoramica sullo stato di avanzamento dell’attività](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Ombreggiatura stato attività per attività completate**: dopo aver contrassegnato un’attività come Completa, nella vista Milestone viene ombreggiato lo sfondo dell’attività per indicare se è stata completata in tempo o in ritardo:

   * **Ombreggiatura rossa per colonna attività**: lo sfondo di un’attività è rosso quando lo Stato di avanzamento è **In Ritardo**.

   * **Ombreggiatura verde per colonna attività**: lo sfondo di un’attività è verde quando lo Stato di avanzamento è **Ora di attivazione**.

* **Ombreggiatura stato progetto per le colonne Inizio progetto e Completamento progetto**:

   * **Colonna di inizio progetto**: lo sfondo della colonna Inizio progetto è rosso o verde solo quando viene popolata la data di inizio effettiva:

      * **Ombreggiatura rossa per colonna Inizio progetto**: lo sfondo della colonna Inizio progetto è rosso quando lo stato di avanzamento del progetto è **In Ritardo**.

      * **Ombreggiatura verde per la colonna Inizio progetto**: lo sfondo della colonna Inizio progetto è verde quando lo stato di avanzamento del progetto è **Ora di attivazione**.

   * **Colonna Completamento progetto**: lo sfondo della colonna Completamento progetto è rosso o verde solo quando viene popolata la data di completamento effettiva:

      * **Ombreggiatura rossa per colonna Completamento progetto**: lo sfondo della colonna di completamento del progetto è rosso quando lo stato di avanzamento del progetto è **In Ritardo**.

      * **Ombreggiatura verde per la colonna Completamento progetto**: lo sfondo della colonna Completamento progetto è verde quando lo stato di avanzamento del progetto è **Ora di attivazione**.

   * Alle colonne Inizio e Completamento non viene assegnata alcuna ombreggiatura colore quando le attività hanno lo stato Avanzamento A rischio o Indietro.

  ![Vista Milestone con sfondo](assets/milestone-view-with-shading.png)

* **Nome progetto**: il nome del progetto viene visualizzato con un collegamento al progetto.
* **Icona Condizione progetto**: accanto al nome del progetto viene visualizzata un’icona che indica la condizione del progetto.

## Configurare le informazioni da visualizzare nella vista Milestone {#configure-what-information-displays-in-the-milestone-view}

Puoi configurare se i seguenti elementi vengono visualizzati nella vista Milestone:

* Icone di stato di avanzamento
* Percentuale di completamento di progetti e attività

Per impostazione predefinita, vengono visualizzate le icone di stato del progetto e la percentuale di completamento dei progetti.

Qualsiasi modifica apportata a queste opzioni è valida solo per te; gli altri utenti non saranno interessati. Le modifiche apportate vengono mantenute al successivo accesso ad Adobe Workfront.

Per configurare la visualizzazione delle icone di stato del progetto e della percentuale di completamento dei progetti:

{{step1-to-projects}}

1. Fai clic su **Visualizza** menu a discesa, quindi fai clic su **Milestone**.\
   Se visualizzi un elenco di progetti all’interno di un Portfolio o di un programma, seleziona la **Milestone** scheda secondaria.

1. Clic **Opzioni** nell&#39;angolo superiore destro della vista Milestone.\
   ![milestone_view_options.png](assets/milestone-view-options-350x141.png)

1. Selezionare una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Stato di avanzamento</td> 
      <td> <p>Selezionare questa opzione per visualizzare le icone di stato di avanzamento accanto a ogni progetto e attività.</p> <p>Questa opzione è attivata per impostazione predefinita.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percentuale completato</td> 
      <td> <p>Selezionare questa opzione per visualizzare la percentuale di completamento accanto a ogni progetto e attività.</p> <p>Questa opzione è attivata per impostazione predefinita.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Regola percentuale di completamento per le attività nella vista Milestone {#adjust-percent-complete-for-tasks-in-the-milestone-view}

Nella vista Milestone (Attività cardine) è possibile regolare la percentuale di completamento delle attività. Non è possibile regolare la percentuale di completamento per un&#39;attività padre, ovvero un&#39;attività che contiene sottoattività.

Per regolare la percentuale di completamento di un&#39;attività nella vista Milestone:

{{step1-to-projects}}

1. Fai clic su **Visualizza** menu a discesa, quindi fai clic su **Milestone**.

1. (Condizionale) Se le percentuali di completamento non vengono visualizzate nella visualizzazione Milestone, fai clic su **Opzioni** nell’angolo superiore destro della vista Milestone, assicurati che **Percentuale completamento** è abilitato.

1. Fare clic sulla percentuale di completamento al di sotto di un&#39;attività, specificare una nuova percentuale, quindi premere Invio.
