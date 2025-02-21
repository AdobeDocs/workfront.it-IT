---
product-area: reporting
navigation-topic: reporting-elements
title: Utilizzare la vista Milestone
description: Puoi applicare la vista Milestone (Attività cardine) a un elenco o a un rapporto di progetto.
author: Nolan
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1312'
ht-degree: 0%

---

# Utilizzare la vista Milestone

<!-- Audited: 11/2024 -->

Puoi applicare la vista Milestone (Attività cardine) a un elenco o a un rapporto di progetto.

Prima di poter utilizzare la vista milestone, è necessario configurare le milestone, aggiungere percorsi milestone ai progetti e associare le milestone alle attività, come descritto negli articoli [Creare un percorso milestone](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) e [Associare le milestone alle attività](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

La vista Milestone (Attività cardine) è disponibile quando si visualizza un elenco di progetti o un rapporto di progetto. Nelle sezioni seguenti viene descritto come visualizzare e utilizzare la vista milestone.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
      <p>Nuovo:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Corrente:</p>
         <ul>
         <li><p>Lavoro o superiore</p></li>
         </ul>
   </td>
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

+++

## Passa alla vista Milestone {#switch-to-the-milestone-view}

{{step1-to-projects}}

1. Fai clic sul menu a discesa **Visualizza**, quindi fai clic su **Milestone**.

   L’elenco o il rapporto viene visualizzato in una vista Milestone.

   Per informazioni sulla visualizzazione milestone, vedere la sezione [Panoramica della visualizzazione milestone](#milestone-view-overview) in questo articolo.

## Panoramica della vista Milestone {#milestone-view-overview}

La vista Milestone (Attività cardine) è disponibile negli elenchi dei progetti e nei rapporti sui progetti. Questa visualizzazione consente di visualizzare rapidamente tutte le attività cardine associate alle attività all&#39;interno dei progetti visualizzati.


>[!NOTE]
>
>La vista Milestone (Attività cardine) non è disponibile nelle seguenti aree:
>
>* Schede orario, nell’elenco dei progetti quando si aggiunge un progetto.


Per informazioni su come passare alla vista Milestone, vedere la sezione [Passare alla vista Milestone](#switch-to-the-milestone-view) in questo articolo.

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

* **Date pianificate o date previste:** Specificare se si desidera visualizzare le date pianificate o le date previste nella vista Milestone.\
  Vengono visualizzate le date di inizio e completamento, nonché di ogni attività cardine all’interno del Percorso attività cardine.\
  Se si visualizzano le Date pianificate e si dispone anche dell&#39;accesso Gestisci al progetto, è possibile modificare le date seguenti direttamente dalla vista Milestone (se si visualizzano le Date previste, le date non possono essere modificate perché le Date previste sono calcolate e non possono essere modificate manualmente).

   * **Date inizio progetto:** Se un progetto è pianificato a partire dalla data di inizio, è possibile modificare manualmente la data di inizio del progetto, quindi calcolare la data di completamento.
   * **Date di completamento progetto:** Se un progetto è programmato dalla data di completamento, è possibile modificare manualmente la data di completamento del progetto e la data di inizio viene quindi calcolata.
   * **Date di completamento attività:** Puoi aggiornare manualmente il completamento delle attività direttamente dalla vista Milestone.

* **Percentuale completamento:** Visualizza la percentuale di completamento di ogni attività e progetto.\
  È possibile disattivare la visualizzazione della percentuale di completamento, come descritto nella sezione [Configurare le informazioni visualizzate nella vista Milestone](#configure-what-information-displays-in-the-milestone-view) in questo articolo.\
  Puoi regolare la percentuale di completamento direttamente dalla vista Milestone, come descritto nella sezione [Regola percentuale di completamento per le attività nella vista Milestone](#adjust-percent-complete-for-tasks-in-the-milestone-view) in questo articolo.

* **Icone di stato attività:** Accanto a ogni progetto e attività nella visualizzazione Milestone viene visualizzata un&#39;icona di stato.

   * Nei Tempi\
     ![Icona orario](assets/gantt-ontime.png)

   * Indietro\
     ![Icona Indietro](assets/gantt-behind.png)

   * A Rischio\
     ![Icona a rischio](assets/gantt-atrisk.png)

   * In Ritardo\
     ![Icona ritardo](assets/gantt-late.png)

  È possibile disattivare la visualizzazione di queste icone di stato, come descritto nella sezione [Configurare le informazioni visualizzate nella vista Milestone](#configure-what-information-displays-in-the-milestone-view) in questo articolo.\
  Per informazioni più dettagliate su ciascun tipo di stato, vedere l&#39;articolo [Panoramica sullo stato di avanzamento dell&#39;attività](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Ombreggiatura stato attività per attività completate**: dopo aver contrassegnato un&#39;attività come Completa, lo sfondo dell&#39;attività viene ombreggiato nella vista Milestone per indicare se l&#39;attività è stata completata in tempo o in ritardo:

   * **Sfondo rosso per la colonna attività**: lo sfondo di un&#39;attività è rosso quando lo stato di avanzamento è **In ritardo**.

   * **Ombreggiatura verde per la colonna attività**: lo sfondo di un&#39;attività è verde quando lo stato di avanzamento è **Ora di attivazione**.

* **Ombreggiatura stato progetto per le colonne Inizio progetto e Completamento del progetto**:

   * **Colonna inizio progetto**: lo sfondo della colonna Inizio progetto è rosso o verde solo quando la data di inizio effettivo è popolata:

      * **Ombreggiatura rossa per colonna inizio progetto**: lo sfondo della colonna inizio progetto è rosso quando lo stato di avanzamento del progetto è **In ritardo**.

      * **Ombreggiatura verde per la colonna Inizio progetto**: lo sfondo della colonna Inizio progetto è verde quando lo stato di avanzamento del progetto è **Ora di inizio**.

   * **Colonna completamento progetto**: lo sfondo della colonna Completamento progetto è rosso o verde solo quando viene popolata la data di completamento effettiva:

      * **Sfondo rosso per la colonna di completamento del progetto**: lo sfondo della colonna di completamento del progetto è rosso quando lo stato di avanzamento del progetto è **In ritardo**.

      * **Ombreggiatura verde per la colonna di completamento del progetto**: lo sfondo della colonna di completamento del progetto è verde quando lo stato di avanzamento del progetto è **Nei tempi**.

   * Alle colonne Inizio e Completamento non viene assegnata alcuna ombreggiatura colore quando le attività hanno lo stato Avanzamento A rischio o Indietro.

  ![Vista milestone con sfondo](assets/milestone-view-with-shading.png)

* **Nome progetto**: il nome del progetto viene visualizzato con un collegamento al progetto.
* **Icona condizione progetto**: accanto al nome del progetto viene visualizzata un&#39;icona che indica la condizione del progetto.

## Configurare le informazioni da visualizzare nella vista Milestone {#configure-what-information-displays-in-the-milestone-view}

Puoi configurare se i seguenti elementi vengono visualizzati nella vista Milestone:

* Icone di stato di avanzamento
* Percentuale di completamento di progetti e attività

Per impostazione predefinita, vengono visualizzate le icone di stato del progetto e la percentuale di completamento dei progetti.

Qualsiasi modifica apportata a queste opzioni è valida solo per te; gli altri utenti non saranno interessati. Le modifiche apportate vengono mantenute al successivo accesso ad Adobe Workfront.

Per configurare la visualizzazione delle icone di stato del progetto e della percentuale di completamento dei progetti:

{{step1-to-projects}}

1. Fai clic sul menu a discesa **Visualizza**, quindi fai clic su **Milestone**.\
   Se visualizzi un elenco di progetti all&#39;interno di un Portfolio o di un Programma, seleziona la scheda secondaria **Milestone**.

1. Fai clic su **Opzioni** nell&#39;angolo superiore destro della visualizzazione Milestone.\
   ![opzioni_vista_milestone.png](assets/milestone-view-options-350x141.png)

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

1. Fai clic sul menu a discesa **Visualizza**, quindi fai clic su **Milestone**.

1. (Condizionale) Se le percentuali di completamento non vengono visualizzate nella visualizzazione Milestone, fai clic su **Opzioni** nell&#39;angolo superiore destro della visualizzazione Milestone, quindi assicurati che **Percentuale di completamento** sia abilitato.

1. Fare clic sulla percentuale di completamento al di sotto di un&#39;attività, specificare una nuova percentuale, quindi premere Invio.
