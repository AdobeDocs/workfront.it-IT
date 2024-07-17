---
product-area: agile-and-teams
navigation-topic: iterations
title: Creare un’iterazione
description: Le iterazioni sono un componente chiave per i team agili Scrum nella pianificazione della capacità di lavoro. [!DNL Adobe Workfront] consente ai team agili Scrum di gestire il proprio lavoro creando più iterazioni per soddisfare le esigenze del team.
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '1057'
ht-degree: 0%

---

# Creare un’iterazione

Le iterazioni sono un componente chiave per i team agili Scrum nella pianificazione della capacità di lavoro. [!DNL Adobe Workfront] consente ai team agili Scrum di gestire il proprio lavoro creando più iterazioni per soddisfare le esigenze del team.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano o il tipo di licenza disponibile, contattare l&#39;amministratore [!DNL Workfront].

## Aggiungi un’iterazione

Utilizza la funzione [!UICONTROL Aggiungi iterazione] per creare rapidamente un&#39;iterazione e aggiungere attività e problemi in un secondo momento.

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.

1. Nella scheda **[!UICONTROL Iterazioni]**, fare clic su **[!UICONTROL Aggiungi iterazione]**.\
   ![](assets/add-iteration-adobe-350x275.png)

1. Specifica quanto segue:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Nome iterazione]</strong></td> 
      <td>Immettere il nome dell'iterazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Goal]</strong></td> 
      <td>Aggiungi eventuali obiettivi per l’iterazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Data Inizio]</strong></td> 
      <td>Immettere la data di inizio dell'iterazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Data di fine]</strong></td> 
      <td><p>Immettere la data di fine dell'iterazione. [!DNL Workfront] consiglia di impostare una data di fine non superiore a 4 settimane dalla data di inizio.</p><p>Suggerimento: scegli un giorno lavorativo come data di fine. Il grafico a dispersione usa solo giorni lavorativi nei suoi calcoli.<br>Per impostazione predefinita, il grafico a dispersione utilizza la pianificazione predefinita per definire i giorni lavorativi (come descritto in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creare una pianificazione</a>). In alternativa, per incorporare i giorni non lavorativi specifici del team, i team Agile possono scegliere di utilizzare una pianificazione alternativa (come descritto in "Definizione di una pianificazione alternativa del team per i grafici Burndown" in <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Creare un team Agile</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Specificare la capacità per l'iterazione. Questo è il numero di punti o ore che il team è in grado di raggiungere nell’iterazione. Il numero immesso deve essere uguale o maggiore del numero di punti o ore dalla somma di tutti i brani nell'iterazione.<br>[!DNL Workfront] precompila questo campo con una capacità di 50 per impostazione predefinita. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Specifica la percentuale di attivazione del team. Se tutti i membri del team si concentreranno completamente su questa iterazione, l’attenzione si concentrerà al 100%.<br>[!DNL Workfront] precompila questo campo con 100% per impostazione predefinita. </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Invia]**. Ora che hai creato un’iterazione, devi aggiungere delle storie. Per ulteriori informazioni, vedere [Aggiungere brani a un&#39;iterazione esistente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Pianifica un&#39;iterazione nella scheda [!UICONTROL Backlog]

Utilizza la funzione [!UICONTROL Iterazione piano] per creare un&#39;iterazione utilizzando le attività nel backlog.

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Cambia team]** ![Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.

1. Seleziona **[!UICONTROL Backlog]** nel pannello a sinistra. Quindi fare clic su **[!UICONTROL Iterazione piano]**.

1. Specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Nome iterazione]</strong></td> 
      <td>Specificare un nome per l'iterazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Data Inizio]</strong></td> 
      <td> Specificare la data di inizio dell'iterazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Data di fine]</strong> </td> 
      <td><p>Specificare la data di fine dell'iterazione. [!DNL Workfront] consiglia di impostare una data di fine non superiore a 4 settimane dalla data di inizio.</p><p>Suggerimento: scegli un giorno lavorativo come data di fine. Il grafico a dispersione usa solo giorni lavorativi nei suoi calcoli.<br>Per impostazione predefinita, il grafico a dispersione utilizza la pianificazione predefinita per definire i giorni lavorativi (come descritto in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creare una pianificazione</a>). In alternativa, per incorporare i giorni non lavorativi specifici del team, i team Agile possono scegliere di utilizzare una pianificazione alternativa (come descritto in <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md" class="MCXref xref">Utilizzare una pianificazione alternativa del team per i grafici a dispersione</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Specifica la percentuale di attivazione del team. Se tutti i membri del team si concentreranno completamente su questa iterazione, l’attenzione si concentrerà al 100%.<br>[!DNL Workfront] precompila questo campo con il valore medio delle iterazioni passate del team. Se si tratta della prima iterazione del team, il valore del campo è 0 per impostazione predefinita.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Specificare la capacità per l'iterazione. Questo è il numero di punti o ore che il team è in grado di raggiungere nell’iterazione. Il numero immesso deve essere uguale o maggiore del numero di punti o ore dalla somma di tutti i brani nell'iterazione.<br>[!DNL Workfront] precompila questo campo con il valore medio delle iterazioni passate del team. Se si tratta della prima iterazione del team, il valore del campo è 0 per impostazione predefinita.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Goal]</strong></td> 
      <td> Specificare un obiettivo per l'iterazione. Questo campo non è obbligatorio.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Seleziona i brani per aggiungerli ora all&#39;iterazione oppure puoi saltare questo passaggio e aggiungerli a un&#39;iterazione in un secondo momento. Le storie nella parte superiore del backlog hanno priorità più alta. Le storie vengono evidenziate in verde quando rientrano nella loro capacità; in caso contrario vengono evidenziate in rosso.\
   È possibile aggiungere sia attività che problemi a una singola iterazione:

   * **Per aggiungere attività all&#39;iterazione:** Nella scheda **[!UICONTROL Backlog]**, verificare che sia selezionata la scheda **[!UICONTROL Storie]** (questa scheda è selezionata per impostazione predefinita durante la visualizzazione del backlog). Selezionare i brani da aggiungere all&#39;iterazione.\

     Quando si aggiungono attività a un&#39;iterazione, la data di inizio dell&#39;attività viene calcolata come descritto in [[!UICONTROL Comprendere] come vengono calcolate le date di inizio dell&#39;attività quando questa viene aggiunta a un&#39;iterazione](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration).

   * **Per aggiungere problemi all&#39;iterazione:** Nella scheda **[!UICONTROL Backlog]**, fare clic sulla scheda **[!UICONTROL Problemi]**. Seleziona i problemi da aggiungere all’iterazione.

1. Fai clic su **[!UICONTROL Salva].**
Viene creata l&#39;iterazione.

1. (Facoltativo) Per aggiungere brani a un&#39;iterazione esistente, vedere [Aggiungere brani a un&#39;iterazione esistente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Informazioni sul calcolo delle date di inizio attività quando vengono aggiunte a un&#39;iterazione {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

Quando si aggiunge un&#39;attività come brano a un&#39;iterazione, per ogni brano viene utilizzato il vincolo [!UICONTROL Deve finire all&#39;attività]. Nella maggior parte dei casi, la data di inizio pianificata dell&#39;attività viene calcolata in base alla formula seguente:

[!UICONTROL Data fine iterazione] meno (-) [!UICONTROL Durata attività] è uguale (=) [!UICONTROL Data inizio attività pianificata]

Viene utilizzata la [!UICONTROL Data di fine progetto] al posto della   se la data di inizio del progetto è successiva alla data di inizio dell&#39;iterazione e la data di fine del progetto è successiva a tale data.

È possibile configurare singoli team Scrum in modo che utilizzino le date del progetto per impostazione predefinita, anziché le date di iterazione. Per informazioni, vedere la sezione [Configurare le modalità di applicazione delle date durante l&#39;aggiunta di elementi di lavoro a un&#39;iterazione](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) nell&#39;articolo [Configurare Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).
