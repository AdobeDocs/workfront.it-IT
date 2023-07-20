---
product-area: projects
navigation-topic: create-tasks
title: Creare attività ricorrenti
description: È possibile creare attività ricorrenti per le attività da ripetere come parte di un singolo progetto.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: 4a4efe7d8a354bc9ec22a607fe6e75040e7cca24
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Creare attività ricorrenti

È possibile creare attività ricorrenti per le attività da ripetere come parte di un singolo progetto.

Per informazioni generali sulle attività ricorrenti, incluso l&#39;impatto della modifica di un&#39;attività ricorrente esistente, vedere [Panoramica delle attività ricorrenti](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

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
   <td> <p>Modifica accesso ad attività e progetti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni sull'accesso alle attività, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Concedere l’accesso alle attività</a>. Per informazioni su come un amministratore di Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute per il progetto con la possibilità di aggiungere attività o versione successiva</p> <p>Quando crei un’attività, ricevi automaticamente le autorizzazioni di gestione per l’attività</p> <p> Per informazioni sulle autorizzazioni per le attività, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Condividere un’attività </a>. </p> <p>Per informazioni sulla richiesta di autorizzazioni aggiuntive, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Creare un’attività ricorrente

>[!NOTE]
>
>Non è possibile creare un&#39;attività ricorrente modificando un&#39;attività esistente. Creare un&#39;attività da zero.

1. Vai al progetto in cui desideri creare un’attività ricorrente, quindi fai clic sul pulsante **Attività** nel pannello a sinistra.
1. Clic **Crea Attività**.

   Viene visualizzata la finestra di dialogo Nuova attività.

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. Clic **Altre opzioni** quindi immettere un nome per l&#39;attività in **Nome attività** campo.
1. Continuare ad aggiornare l&#39;attività come si farebbe se si aggiungesse una nuova attività. Per ulteriori informazioni sull&#39;aggiunta di una nuova attività, vedere [Creare attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!TIP]
   >
   >   La Durata e le Ore pianificate indicate per una nuova attività ricorrente sono la Durata e le Ore pianificate di ciascuna occorrenza. La durata dell&#39;attività padre è il tempo che intercorre tra la data di inizio pianificata della prima attività e la data di completamento pianificata dell&#39;attività più recente. Le ore pianificate dell&#39;attività padre corrispondono al totale di tutte le ore pianificate di tutte le occorrenze.

1. Clic **Panoramica** nel pannello a sinistra.
1. Scorri verso il basso fino a **Pianificazione ricorrenza** , quindi selezionare la **Imposta come attività ricorrente** opzione.

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. In **Frequenza** dall&#39;elenco a discesa, selezionare il numero di unità di tempo in cui si desidera eseguire l&#39;attività e il tipo di unità di tempo. Selezionare una delle opzioni seguenti:

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
      <td role="rowheader"><strong>Giorno lavorativo</strong> </td> 
      <td> <p> L'attività viene ripetuta ogni giorno lavorativo, ogni 2 giorni lavorativi, ogni 3 giorni lavorativi e così via, a seconda della cadenza selezionata. È possibile configurare le attività in modo che vengano ripetute fino a ogni sesto giorno lavorativo.</p> <p>Questa opzione utilizza la pianificazione predefinita definita dall'amministratore di sistema, come descritto in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creare una pianificazione</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Settimana</strong> </td> 
      <td> <p> L'attività viene ripetuta ogni settimana, ogni 2 settimane, ogni 3 settimane e così via, a seconda della cadenza selezionata.</p> <p>In <strong>Si ripete</strong> , selezionare il giorno della settimana in cui si desidera che venga eseguita ogni attività. Puoi selezionare più giorni. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mese</strong> </td> 
      <td> <p>L'attività viene ripetuta ogni mese, ogni 2 mesi, ogni 3 mesi e così via, a seconda della cadenza selezionata. Puoi scegliere tra 1 e 12 mesi. </p> <p>In <strong>Si ripete</strong> selezionare una delle opzioni seguenti quando si desidera che l'attività venga eseguita:</p> 
       <ul> 
        <li> <p><strong>ogni mese il giorno &lt;month date=""&gt;</strong> </p> <p>È possibile selezionare i giorni da 1 a 30 oppure selezionare <strong>ultimo</strong>. Ad esempio, è possibile selezionare "ogni mese il 30". </p> </li> 
        <li> <p><strong>ogni mese il &lt;number&gt; &lt;day of="" the="" week=""&gt;</strong> </p> <p>Nel primo menu a discesa è possibile selezionare un numero compreso tra 1 e 4 come numero della settimana del mese oppure selezionare "ultimo". </p> <p>Nel secondo menu a discesa, puoi selezionare qualsiasi giorno della settimana. </p> <p>Ad esempio, puoi selezionare "ogni mese il 2° martedì". </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Se alla programmazione del progetto è associata un&#39;eccezione di programmazione, le attività ricorrenti non possono iniziare durante l&#39;eccezione. I task ricorrenti che si verificano durante l&#39;eccezione della programmazione vengono programmati per iniziare il primo giorno lavorativo successivo all&#39;eccezione. Per ulteriori informazioni sulle eccezioni alla pianificazione, consulta l’articolo [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. In **Inizia** selezionare la data e l&#39;ora in cui si desidera che inizino le attività ricorrenti.
1. In **Termina** , selezionare la data e l&#39;ora in cui si desidera che vengano completate le attività ricorrenti

   Oppure

   Seleziona **dopo `<number>` occorrenze** per indicare quante volte deve verificarsi l&#39;attività ricorrente. Workfront crea per le attività lo stesso numero di ricorrenze indicato in questo campo.

1. Clic **Crea attività.**

   Viene visualizzato l’elenco delle attività. L&#39;attività ricorrente viene creata come padre e tutte le ricorrenze sono i relativi figli. Workfront ha generato automaticamente i nomi delle attività figlio, utilizzando il nome immesso per l&#39;attività padre seguito da un numero. Per ulteriori informazioni sui campi compilati automaticamente dall&#39;attività ricorrente padre, vedere [Panoramica delle attività ricorrenti](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. (Facoltativo) Modifica ogni attività ricorrente come faresti con qualsiasi altra attività del progetto.

   È ad esempio possibile aggiungere assegnazioni, predecessori, durate e modificare qualsiasi altra informazione sull&#39;attività, inclusi i campi personalizzati.

   >[!IMPORTANT]
   >
   >La modifica della ricorrenza padre dopo la modifica dei figli singolarmente può causare informazioni diverse tra i figli o tra i figli e il padre. Per ulteriori informazioni, consulta [Panoramica delle attività ricorrenti](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
