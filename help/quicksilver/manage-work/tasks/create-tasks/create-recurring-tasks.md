---
product-area: projects
navigation-topic: create-tasks
title: Creare attività ricorrenti
description: È possibile creare attività ricorrenti per le attività da ripetere come parte di un singolo progetto.
author: Alina
feature: Work Management
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# Creare attività ricorrenti

È possibile creare attività ricorrenti per le attività da ripetere come parte di un singolo progetto.

Per informazioni generali sulle attività ricorrenti, compreso l&#39;impatto della modifica di un&#39;attività ricorrente esistente, vedere [Panoramica delle attività ricorrenti](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

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
   <td> <p>Modifica l’accesso a Attività e Progetti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni sull'accesso alle attività, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Concedere l’accesso alle attività</a>. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di Contribute per il progetto con la possibilità di aggiungere attività o versioni successive</p> <p>Quando crei un'attività, riceverai automaticamente le autorizzazioni di gestione per l'attività</p> <p> Per informazioni sulle autorizzazioni delle attività, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Condividere un’attività </a>. </p> <p>Per informazioni sulla richiesta di autorizzazioni aggiuntive, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare un’attività ricorrente

>[!NOTE]
>
>Non è possibile creare un&#39;attività ricorrente modificando un&#39;attività esistente. È necessario creare un&#39;attività da zero.

1. Passa al progetto in cui desideri creare un&#39;attività ricorrente, quindi fai clic sul pulsante **Attività** nel pannello a sinistra.
1. Fai clic su **Nuova attività**.

   Viene visualizzata la finestra di dialogo Nuova attività .

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. Fai clic su **Altre opzioni** quindi immetti un nome per l’attività nel **Nome attività** campo .
1. Continua ad aggiornare l’attività nello stesso modo in cui lo faresti se aggiungi una nuova attività. Per ulteriori informazioni sull’aggiunta di una nuova attività, consulta [Creazione di attività in un progetto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)
1. Fai clic su **Panoramica** nel pannello a sinistra.
1. Scorri verso il basso fino a **Pianificazione ricorrenza** , quindi seleziona la **Imposta attività ricorrenti** opzione .

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. In **Frequenza** dall’elenco a discesa, selezionare il numero di unità di tempo in cui si desidera che l’attività venga eseguita e il tipo di unità di tempo. Seleziona tra le seguenti opzioni:

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
      <td role="rowheader"><strong>giorno</strong> </td> 
      <td> <p>L'attività si ripete ogni giorno, ogni 2 giorni, ogni 3 giorni, e così via, a seconda della cadenza selezionata. Puoi configurare le attività in modo che vengano ripetute fino a un massimo di 6 giorni. L'impostazione predefinita è 1 giorno. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Giorno lavorativo</strong> </td> 
      <td> <p> L'attività si ripete ogni giorno lavorativo, ogni 2 giorni lavorativi, ogni 3 giorni lavorativi e così via, a seconda della cadenza selezionata. È possibile configurare le attività in modo che vengano ripetute fino a un massimo di 6 giorni lavorativi.</p> <p>Questa opzione utilizza la pianificazione predefinita definita dall'amministratore di sistema, come descritto in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creare una pianificazione</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Settimana</strong> </td> 
      <td> <p> L'attività si ripete ogni settimana, ogni 2 settimane, ogni 3 settimane, e così via, a seconda della cadenza selezionata.</p> <p>In <strong>Ripeti</strong> selezionare il giorno della settimana in cui si desidera che si verifichi ogni attività. Puoi selezionare più giorni. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mese</strong> </td> 
      <td> <p>L'attività si ripete ogni mese, ogni 2 mesi, ogni 3 mesi e così via, a seconda della cadenza selezionata. Puoi scegliere tra 1 e 12 mesi. </p> <p>In <strong>Ripeti</strong> selezionare una delle seguenti opzioni quando si desidera che l'attività si verifichi:</p> 
       <ul> 
        <li> <p><strong>ogni mese &lt;month date=""&gt;</strong> </p> <p>È possibile selezionare giorni da 1 a 30 oppure selezionare <strong>last</strong>. Ad esempio, puoi selezionare "ogni mese il 30". </p> </li> 
        <li> <p><strong>ogni mese &lt;number&gt; &lt;day of="" the="" week=""&gt;</strong> </p> <p>Nel primo menu a discesa, è possibile selezionare un numero compreso tra 1 e 4 per il numero della settimana nel mese, oppure è possibile selezionare "ultimo". </p> <p>Nel secondo menu a discesa, puoi selezionare un giorno della settimana. </p> <p>Ad esempio, puoi selezionare "ogni mese il 2° martedì". </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Se alla pianificazione del progetto è associata un&#39;eccezione di pianificazione, le attività ricorrenti non possono essere avviate durante l&#39;eccezione. Le attività ricorrenti che si verificano durante l&#39;eccezione di pianificazione vengono programmate per iniziare il primo giorno lavorativo successivo all&#39;eccezione. Per ulteriori informazioni sulle eccezioni di pianificazione, consulta l’articolo [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. In **Inizia** selezionare la data e l&#39;ora di inizio delle attività ricorrenti.
1. In **Termina** selezionare la data e l&#39;ora in cui si desidera completare le attività ricorrenti

   Oppure

   Seleziona **dopo `<number>` occorrenze** per indicare quante volte deve verificarsi l’attività ricorrente. Workfront crea lo stesso numero di ricorrenze per le attività del numero indicato in questo campo.

1. Fai clic su **Crea attività.**

   Viene visualizzato l’elenco delle attività. L&#39;attività ricorrente viene creata come padre e tutte le ricorrenze sono figli. Workfront ha generato automaticamente i nomi delle attività figlio utilizzando il nome immesso per l&#39;elemento padre seguito da un numero. Per ulteriori informazioni sui campi compilati automaticamente dall&#39;attività ricorrente padre, vedere [Panoramica delle attività ricorrenti](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. (Facoltativo) Modifica ogni attività ricorrente come qualsiasi altra attività del progetto.

   Ad esempio, è possibile aggiungere assegnazioni, predecessori, durate e modificare qualsiasi altra informazione sull&#39;attività, compresi i campi personalizzati.

   >[!IMPORTANT]
   >
   >La modifica della ricorrenza padre dopo la modifica individuale degli elementi figlio può causare informazioni diverse tra gli elementi figlio o tra gli elementi figlio e il padre. Per ulteriori informazioni, consulta [Panoramica delle attività ricorrenti](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
