---
content-type: reference
product-area: setup
navigation-topic: use-the-gantt-chart
title: Configura la visualizzazione delle informazioni nel grafico [!UICONTROL Gantt]
description: È possibile configurare le informazioni visualizzate sia nel Diagramma di Gantt elenco attività che nel Diagramma di Gantt elenco progetti.
author: Alina
feature: Work Management
exl-id: 465365a2-d94b-47b6-a393-16770fca2714
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# Configura la visualizzazione delle informazioni nel [!UICONTROL Diagramma di Gantt]

È possibile configurare le informazioni visualizzate sia nell&#39;Elenco attività [!UICONTROL Grafico di Gantt] che nell&#39;Elenco progetti [!UICONTROL Grafico di Gantt].

## Requisiti di accesso

Per seguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso di [!UICONTROL View] o versione successiva a progetti e attività</p> <p>Nota: se non disponi ancora dell'accesso, chiedi all'amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di [!UICONTROL View] o versione successiva al progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## Comprendere le opzioni di visualizzazione

La tabella seguente descrive le opzioni di visualizzazione per il [!UICONTROL Diagramma di Gantt]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date effettive]</td> 
   <td> <img src="assets/actual-dates-in-gantt-183x213.png" alt="actual_dates_in_gantt.png" style="width: 183;height: 213;"> </td> 
   <td> <p>[!UICONTROL Actual Start Date] (Data di inizio effettiva) e [!UICONTROL Actual Completion Date] (Data di completamento effettiva) sono visualizzati con un'icona triangolare. Se [!UICONTROL Actual Completion Date] è null, verrà visualizzata solo la [!UICONTROL Actual Start Date].</p> <p>Per ulteriori informazioni sulle date di inizio e di completamento, vedere <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Panoramica del progetto [!UICONTROL Data di completamento effettiva] </a> e <a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Panoramica del progetto [!UICONTROL Data di inizio effettiva] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assegnazioni]</td> 
   <td> <img src="assets/assignments-in-gantt-312x203.png" alt="assignments_in_gantt.png" style="width: 312;height: 203;"> </td> 
   <td> <p>Mostra gli assegnatari delle attività. Passa il puntatore del mouse sul collegamento <strong>[!UICONTROL Details]</strong> accanto al nome di un assegnatario per visualizzare informazioni più dettagliate su di essi, inclusa la percentuale della loro allocazione all'attività.</p> <p>Gli assegnatari non vengono visualizzati nel grafico [!UICONTROL Gantt] quando il grafico [!UICONTROL Gantt] viene esportato in PDF. Quando il grafico di Gantt [!UICONTROL] viene esportato in PDF, gli assegnatari vengono visualizzati solo nell'elenco delle attività.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Baseline]</td> 
   <td> <img src="assets/baselines-sandbox-gantt.png" alt="baseline_sandbox_gantt.png"> </td> 
   <td> <p>Snapshot del progetto che rappresenta i dati chiave del progetto inclusi nel piano di progetto iniziale. Le linee di base possono essere utilizzate per tutta la durata del progetto. Quando si abilita la visualizzazione delle linee di base nel diagramma di Gantt [!UICONTROL], selezionare la linea di base che si desidera visualizzare. È possibile visualizzare una sola linea di base nel diagramma di Gantt [!UICONTROL] alla volta, che verrà visualizzata sotto forma di una barra grigia.</p> <p>Per ulteriori informazioni sulle previsioni, vedere <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref">Creare le previsioni del progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commit Date]</td> 
   <td> <img src="assets/commit-dates-sandbox-243x226.png" alt="commit_dates_sandbox.png" style="width: 243;height: 226;"> </td> 
   <td> <p>La data indicata da un assegnatario come impegno di quando l'attività verrà completata viene visualizzata con un marcatore nel diagramma di Gantt [!UICONTROL]. </p> <p>Per ulteriori informazioni sulle date di commit, vedere <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">[!UICONTROL Commit Date] overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL % completato]</td> 
   <td> <img src="assets/percent-complete-gantt.png" alt="percent_complete_gantt.png"> </td> 
   <td>  La percentuale di completamento dell'attività viene visualizzata nella riga dell'attività.<br><br></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percorso Critico]</td> 
   <td> <img src="assets/critical-path-2.png" alt="Percorso_critico_2.png"> </td> 
   <td>Le attività che possono influenzare la tempistica del progetto sono considerate parte del Percorso Critico e sono chiaramente contrassegnate in rosso. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone] Rombi</td> 
   <td> <img src="assets/milestone-diamonds.png" alt="milestone_diamonds.png"> </td> 
   <td> <p>Dopo l'attività associata a un'attività cardine viene visualizzata un'icona a forma di rombo. Passa il puntatore del mouse su una milestone per visualizzarne il nome e la data. L'amministratore [!DNL Workfront] determina il colore di ogni rombo milestone.</p> <p>Per ulteriori informazioni sulle milestone, vedere <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Creare un percorso milestone</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Righe [!UICONTROL Milestone]</td> 
   <td> <img src="assets/milestone-line-more-info-in-gantt-270x209.png" alt="milestone_line_more_info_in_gantt.png" style="width: 270;height: 209;"> </td> 
   <td> <p>Dopo l'attività associata a un'attività cardine viene visualizzata una linea. Passa il puntatore del mouse su una milestone per visualizzarne il nome e la data. L'amministratore [!DNL Workfront] determina il colore di ogni linea milestone.</p> <p> Per ulteriori informazioni sulle milestone, vedi  <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Crea un percorso milestone</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Predecessors]</td> 
   <td> <img src="assets/predecessor-2-269x200.png" alt="predecessor_2.png" style="width: 269;height: 200;"> </td> 
   <td> <p>Riga da un'attività all'altra che mostra la relazione predecessore tra le due attività. Per evidenziare una singola linea predecessore, posizionare il mouse su di essa. Fai clic su di esso per mantenerlo evidenziato. È possibile evidenziare una sola riga predecessore alla volta.</p> <p>Accanto a qualsiasi attività con una relazione predecessore che si estende su più pagine nel diagramma di Gantt o su qualsiasi attività con un predecessore per più progetti viene visualizzata l'icona <strong>[!UICONTROL Predecessor]</strong>.</p> <p>Fai clic sull'icona <strong>[!UICONTROL Predecessore]</strong> per visualizzare tutte le attività predecessore e successore, nonché i dettagli su ogni attività, come il nome dell'attività, il tipo di relazione predecessore e le date chiave.</p> <p>Nota: il diagramma di Gantt [!UICONTROL] in un elenco di progetti visualizza informazioni sui predecessori tra progetti. Per ulteriori informazioni su come creare relazioni di predecessori tra progetti diversi, vedi <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Creare predecessori tra progetti</a></p> <p>Per ulteriori informazioni sui predecessori, vedere <a href="../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md" class="MCXref xref">Applica predecessori</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Stato di avanzamento di [!UICONTROL]</td> 
   <td> <p>[!UICONTROL On Time] <img src="assets/task-on-time--oct.-2017.png" alt="task_on_time__Oct._2017.png"></p> <p>[!UICONTROL Dietro]    <img src="assets/task-behind--oct.-2017.png" alt="task_behind__ott._2017.png"></p> <p>[!UICONTROL A Rischio]    <img src="assets/task-at-risk.png" alt="task_at_risk.png"></p> <p>In Ritardo        <img src="assets/task-late-oct.2017.png" alt="task_late_ott.2017.png"></p> </td> 
   <td> <p> </p> <p>Stato dell'avanzamento corrente di una determinata attività. </p> <p>Per informazioni più dettagliate su ogni tipo di [!UICONTROL Progress Status], vedere <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Panoramica sullo stato di avanzamento dell'attività [!UICONTROL]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date Previste]</td> 
   <td> <img src="assets/gantt-projected-dates-272x152.png" alt="gantt_projected_dates.png" style="width: 272;height: 152;"> </td> 
   <td> <p>La sequenza temporale prevista che contrassegna [!UICONTROL Inizio previsto] e [!UICONTROL Date di completamento] in base al lavoro corrente completato, più il lavoro rimanente. </p> <p>Per ulteriori informazioni sulle date di completamento previste, vedere <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Panoramica di [!UICONTROL Data di completamento prevista] per progetti, attività e problemi</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configura opzioni di visualizzazione

1. Passare all&#39;elenco attività [!UICONTROL Grafico di Gantt] o all&#39;elenco progetti [!UICONTROL Grafico di Gantt].\
   Per ulteriori informazioni sulla posizione del [!UICONTROL Diagramma di Gantt], vedere [Introduzione al [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

1. (Facoltativo) Seleziona l&#39;impostazione **[!UICONTROL Passa a date previste]** per visualizzare le attività in base alle relative [!UICONTROL date previste]. Per impostazione predefinita, le attività vengono visualizzate in base alle [!UICONTROL Date pianificate] nel [!UICONTROL Diagramma di Gantt].
1. Fare clic sull&#39;icona Opzioni per visualizzare la finestra di dialogo **[!UICONTROL Opzioni]**.\
   ![Opzioni.png](assets/options-350x129.png)

1. Selezionare le opzioni di configurazione da visualizzare nel [!UICONTROL Diagramma di Gantt].

   >[!NOTE]
   > Non tutte le opzioni di configurazione sono disponibili nell&#39;elenco dei progetti [!UICONTROL Grafico di Gantt].

1. Fare clic in un punto qualsiasi del [!UICONTROL Diagramma di Gantt] per chiudere la finestra di dialogo **[!UICONTROL Opzioni]**.
