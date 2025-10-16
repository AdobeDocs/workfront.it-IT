---
product-area: projects
navigation-topic: create-tasks
title: Crea attività ricorrenti
description: È possibile creare attività ricorrenti per le attività da ripetere come parte di un singolo progetto.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 0%

---

# Creare attività ricorrenti

<!--Audited: 01/2024-->

È possibile creare attività ricorrenti per le attività da ripetere come parte di un singolo progetto.

Per informazioni generali sulle attività ricorrenti, compreso l&#39;impatto della modifica di un&#39;attività ricorrente esistente, vedere [Panoramica sulle attività ricorrenti](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

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
   <td> <p>Standard</p> 
   <p>Lavoro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ad attività e progetti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute per il progetto con la possibilità di aggiungere attività o versione successiva</p> 
   <p>Quando crei un’attività, ricevi automaticamente le autorizzazioni di gestione per l’attività</p> 
    </td> 
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
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p> 
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> 
   <p>When you create a task you automatically receive Manage permissions to the task</p> 
   <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>.</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator. For more information about access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Creare un’attività ricorrente

>[!NOTE]
>
>Non è possibile creare un&#39;attività ricorrente modificando un&#39;attività esistente. Creare un&#39;attività da zero.

1. Vai al progetto in cui desideri creare un&#39;attività ricorrente, quindi fai clic sulla sezione **Attività** nel pannello a sinistra.
1. Fai clic su **Nuova attività**.

   Viene visualizzata la finestra di dialogo Nuova attività.

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. Fai clic su **Altre opzioni**, quindi immetti un nome per l&#39;attività nel campo **Nome attività**.
1. Continuare ad aggiornare l&#39;attività come si farebbe se si aggiungesse una nuova attività. Per ulteriori informazioni sull&#39;aggiunta di una nuova attività, vedere [Creare attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!TIP]
   >
   >   La Durata e le Ore pianificate indicate per una nuova attività ricorrente sono la Durata e le Ore pianificate di ciascuna occorrenza. La durata dell&#39;attività padre è il tempo che intercorre tra la data di inizio pianificata della prima attività e la data di completamento pianificata dell&#39;attività più recente. Le ore pianificate dell&#39;attività padre corrispondono al totale di tutte le ore pianificate di tutte le occorrenze.

1. Fai clic su **Panoramica** nel pannello a sinistra.
1. Scorri verso il basso fino alla sezione **Pianificazione ricorrenza**, quindi seleziona l&#39;opzione **Imposta come attività ricorrente**.

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. Nell&#39;elenco a discesa **Frequenza** selezionare il numero di unità di tempo in cui si desidera eseguire l&#39;attività e il tipo di unità di tempo. Selezionare una delle opzioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Tipo di Ricorrenza</th> 
      <th>Descrizione</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Giorno</strong> </td> 
      <td> <p>L'attività viene ripetuta ogni giorno, ogni 2 giorni, ogni 3 giorni e così via, a seconda della cadenza selezionata. È possibile configurare le attività in modo che vengano ripetute fino a ogni 6 giorni. L'impostazione predefinita è 1 giorno. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Giorno Lavorativo</strong> </td> 
      <td> <p> L'attività viene ripetuta ogni giorno lavorativo, ogni 2 giorni lavorativi, ogni 3 giorni lavorativi e così via, a seconda della cadenza selezionata. È possibile configurare le attività in modo che vengano ripetute fino a ogni sesto giorno lavorativo.</p> <p>Questa opzione utilizza la pianificazione predefinita definita dall'amministratore di sistema, come descritto in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creare una pianificazione</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Settimana</strong> </td> 
      <td> <p> L'attività viene ripetuta ogni settimana, ogni 2 settimane, ogni 3 settimane e così via, a seconda della cadenza selezionata.</p> <p>Nel campo <strong>Ripeti</strong>, seleziona il giorno della settimana in cui desideri eseguire ogni attività. Puoi selezionare più giorni. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mese</strong> </td> 
      <td> <p>L'attività viene ripetuta ogni mese, ogni 2 mesi, ogni 3 mesi e così via, a seconda della cadenza selezionata. Puoi scegliere tra 1 e 12 mesi. </p> <p>Nel campo <strong>Ripeti</strong>, seleziona una delle seguenti opzioni per eseguire l'attività:</p> 
       <ul> 
        <li> <p><strong>ogni mese il giorno &lt;data mese&gt;</strong> </p> <p>È possibile selezionare i giorni da 1 a 30 oppure selezionare <strong>last</strong>. Ad esempio, è possibile selezionare "ogni mese il 30". </p> </li> 
        <li> <p><strong>ogni mese il &lt;numero&gt; &lt;giorno della settimana&gt;</strong> </p> <p>Nel primo menu a discesa è possibile selezionare un numero compreso tra 1 e 4 come numero della settimana del mese oppure selezionare "ultimo". </p> <p>Nel secondo menu a discesa, puoi selezionare qualsiasi giorno della settimana. </p> <p>Ad esempio, puoi selezionare "ogni mese il 2° martedì". </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Se alla programmazione del progetto è associata un&#39;eccezione di programmazione, le attività ricorrenti non possono iniziare durante l&#39;eccezione. I task ricorrenti che si verificano durante l&#39;eccezione della programmazione vengono programmati per iniziare il primo giorno lavorativo successivo all&#39;eccezione. Per ulteriori informazioni sulle eccezioni alla pianificazione, vedere l&#39;articolo [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. Nel campo **Inizi** selezionare la data e l&#39;ora in cui si desidera iniziare le attività ricorrenti.
1. Nel campo **Termina**, selezionare la data e l&#39;ora in cui si desidera che vengano completate le attività ricorrenti

   Oppure

   Seleziona **dopo `<number>` occorrenze** per indicare quante volte deve verificarsi l&#39;attività ricorrente. Workfront crea per le attività lo stesso numero di ricorrenze indicato in questo campo.

1. Fai clic su **Crea attività.**

   Viene visualizzato l’elenco delle attività. L&#39;attività ricorrente viene creata come padre e tutte le ricorrenze sono i relativi figli. Workfront ha generato automaticamente i nomi delle attività figlio, utilizzando il nome immesso per l&#39;attività padre seguito da un numero. Le attività ricorrenti vengono inserite alla fine dell&#39;elenco delle attività.

   Per ulteriori informazioni sui campi compilati automaticamente dall&#39;attività padre ricorrente, vedere [Panoramica sulle attività ricorrenti](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. (Facoltativo) Modifica ogni attività ricorrente come faresti con qualsiasi altra attività del progetto.

   È ad esempio possibile aggiungere assegnazioni, predecessori, durate e modificare qualsiasi altra informazione sull&#39;attività, inclusi i campi personalizzati.

   >[!IMPORTANT]
   >
   >La modifica della ricorrenza padre dopo la modifica dei figli singolarmente può causare informazioni diverse tra i figli o tra i figli e il padre. Per ulteriori informazioni, vedere [Panoramica delle attività ricorrenti](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
