---
product-area: agile-and-teams
navigation-topic: iterations
title: Creare un’iterazione
description: Le iterazioni sono un componente chiave per i team agili Scrum nella pianificazione della capacità di lavoro. [!DNL Adobe Workfront] consente ai team agili Scrum di gestire il proprio lavoro creando più iterazioni per soddisfare le esigenze del team.
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '1049'
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

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo [!DNL Workfront] amministratore.

## Aggiungi un’iterazione

Utilizza la [!UICONTROL Aggiungi iterazione] per creare rapidamente un’iterazione e aggiungere attività e problemi in un secondo momento.

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.

1. Sulla **[!UICONTROL Iterazioni]** scheda , fai clic su **[!UICONTROL Aggiungi iterazione]**.\
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
      <td role="rowheader"><strong>Obiettivo [!UICONTROL]</strong></td> 
      <td>Aggiungi eventuali obiettivi per l'iterazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Data di inizio]</strong></td> 
      <td>Immettere la data di inizio dell'iterazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Data di fine]</strong></td> 
      <td><p>Immettere la data di fine dell'iterazione. [!DNL Workfront] consiglia di impostare una data di fine non superiore a 4 settimane dalla data di inizio.</p><p>Suggerimento: Assicurati di scegliere un giorno lavorativo come data di fine. Nei calcoli del grafico a discesa vengono utilizzati solo i giorni lavorativi.<br>Per impostazione predefinita, il grafico a discesa utilizza la pianificazione predefinita per definire i giorni lavorativi (come descritto in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creare una pianificazione</a>). Oppure, per incorporare giorni non lavorativi specifici del team, i team agili possono scegliere di utilizzare una pianificazione alternativa (come descritto in "Definizione di un programma team alternativo per i grafici a cascata" in <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Creare un team agile</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Specifica la capacità dell'iterazione. È il numero di punti o ore che il team è in grado di eseguire nell’iterazione. Il numero immesso deve essere uguale o maggiore del numero di punti o ore dalla somma di tutti i brani dell'iterazione.<br>[!DNL Workfront] precompila questo campo con una capacità di 50 per impostazione predefinita. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Specifica la percentuale di messa a fuoco del team. Se tutti i membri del team si concentreranno completamente su questa iterazione, l'attenzione sarà del 100%.<br>[!DNL Workfront] precompila il campo con il 100% per impostazione predefinita. </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Invia]**. Ora che hai creato un&#39;iterazione, devi aggiungere delle storie. Per ulteriori informazioni, consulta [Aggiungere storie a un&#39;iterazione esistente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Pianificare un&#39;iterazione [!UICONTROL Backlog] scheda

Utilizza la [!UICONTROL Iterazione piano] per creare un&#39;iterazione utilizzando le attività nel backlog.

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Team]**.

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Cambia team]** icona ![Icona Cambia team](assets/switch-team-icon.png), quindi seleziona un nuovo team Scrum dal menu a discesa o cerca un team nella barra di ricerca.

1. Seleziona **[!UICONTROL Backlog]** nel pannello a sinistra. Quindi, fai clic su **[!UICONTROL Iterazione piano]**.

1. Specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Nome iterazione]</strong></td> 
      <td>Specifica un nome per l’iterazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Data di inizio]</strong></td> 
      <td> Specifica la data di inizio dell'iterazione.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Data di fine]</strong> </td> 
      <td><p>Specifica la data in cui l’iterazione deve terminare. [!DNL Workfront] consiglia di impostare una data di fine non superiore a 4 settimane dalla data di inizio.</p><p>Suggerimento: Assicurati di scegliere un giorno lavorativo come data di fine. Nei calcoli del grafico a discesa vengono utilizzati solo i giorni lavorativi.<br>Per impostazione predefinita, il grafico a discesa utilizza la pianificazione predefinita per definire i giorni lavorativi (come descritto in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creare una pianificazione</a>). Oppure, per incorporare giorni non lavorativi specifici del team, i team agili possono scegliere di utilizzare una pianificazione alternativa (come descritto in <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt--team-schedule-burndown-charts.md" class="MCXref xref">Utilizzare una pianificazione alternativa del team per i grafici a discesa</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Specifica la percentuale di messa a fuoco del team. Se tutti i membri del team si concentreranno completamente su questa iterazione, l'attenzione sarà del 100%.<br>[!DNL Workfront] precompila questo campo con il valore medio delle iterazioni passate del team. Se si tratta della prima iterazione del team, il valore del campo è 0 per impostazione predefinita.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Specifica la capacità dell'iterazione. È il numero di punti o ore che il team è in grado di eseguire nell’iterazione. Il numero immesso deve essere uguale o maggiore del numero di punti o ore dalla somma di tutti i brani dell'iterazione.<br>[!DNL Workfront] precompila questo campo con il valore medio delle iterazioni passate del team. Se si tratta della prima iterazione del team, il valore del campo è 0 per impostazione predefinita.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>Obiettivo [!UICONTROL]</strong></td> 
      <td> Specifica un obiettivo per l’iterazione. Questo campo non è obbligatorio.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Seleziona ora i brani da aggiungere all’iterazione oppure salta questo passaggio e aggiungi i brani a un’iterazione in un secondo momento. Le storie nella parte superiore del backlog hanno una priorità più alta. Le storie sono evidenziate in verde quando rientrano nella capacità; vengono evidenziati in rosso se non lo sono.\
   È possibile aggiungere attività e problemi a una singola iterazione:

   * **Per aggiungere attività all&#39;iterazione:** Sulla **[!UICONTROL Backlog]** , assicurati che **[!UICONTROL Storie]** scheda selezionata (questa scheda è selezionata per impostazione predefinita quando si visualizza il backlog). Seleziona i brani da aggiungere all&#39;iterazione.\

      Quando si aggiungono attività a un&#39;iterazione, la data di inizio dell&#39;attività viene calcolata come descritto in [[!UICONTROL Comprendere] calcolo delle date di inizio attività quando vengono aggiunte a un&#39;iterazione](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration).

   * **Per aggiungere problemi all&#39;iterazione:** Sulla **[!UICONTROL Backlog]** fai clic sulla scheda **[!UICONTROL Problemi]** scheda . Seleziona i problemi da aggiungere all&#39;iterazione.

1. Fai clic su **[!UICONTROL Salva].**
Viene creata l’iterazione.

1. (Facoltativo) Per aggiungere storie a un&#39;iterazione esistente, consulta [Aggiungere storie a un&#39;iterazione esistente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Comprendere come vengono calcolate le date di inizio attività quando vengono aggiunte a un&#39;iterazione {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

Quando aggiungi un&#39;attività come storia a un&#39;iterazione, la [!UICONTROL Deve terminare l&#39;attività] viene utilizzato un vincolo per ogni brano. Nella maggior parte dei casi, la data di inizio pianificata dell’attività viene calcolata in base alla seguente formula:

[!UICONTROL Data fine iterazione] meno (-) [!UICONTROL Durata attività] è uguale a (=) [!UICONTROL Data inizio pianificata attività]

La [!UICONTROL Data fine progetto] viene utilizzato al posto del se la data di inizio del progetto è successiva alla data di inizio dell&#39;iterazione e la data di fine del progetto è successiva alla data di fine dell&#39;iterazione.

È possibile configurare i singoli team Scrum in modo che utilizzino le date del progetto per impostazione predefinita, anziché le date di iterazione. Per informazioni, consulta la sezione . [Configura come vengono applicate le date quando si aggiungono elementi di lavoro a un&#39;iterazione](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) nell&#39;articolo [Configura punteggio](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).
