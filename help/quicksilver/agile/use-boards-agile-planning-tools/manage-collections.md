---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Gestire i flussi di lavoro
description: Un flusso di lavoro è un gruppo configurabile di bacheche e schede per collaborare sul lavoro.
author: Lisa
feature: Agile
source-git-commit: 96819e5d81a063ad623350a0a75428629d6f7b6d
workflow-type: tm+mt
source-wordcount: '868'
ht-degree: 2%

---

# Gestire i flussi di lavoro

{{highlighted-preview}}

>[!NOTE]
>
>I flussi di lavoro sono disponibili nell’ambiente di anteprima e in Produzione tramite la funzionalità opt-in iniziale per [!UICONTROL [!DNL Workfront] Schede]. Per maggiori dettagli, vedi [Funzionalità opt-in in anteprima per le schede Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

Un flusso di lavoro è un gruppo configurabile di bacheche e schede per collaborare sul lavoro. I flussi di lavoro possono includere diversi tipi di bacheche create da modelli, <span class="preview">e un elenco a schede degli elementi di lavoro. In un flusso di lavoro è possibile tenere traccia del lavoro in iterazioni o spruzzi.</span>

<span class="preview">Per ulteriori informazioni, consulta [Utilizza l&#39;elenco delle schede](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) e [Creare un’iterazione in un flusso di lavoro](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).</span>

I flussi di lavoro vengono visualizzati sul dashboard insieme alle singole bacheche a cui hai accesso che non fanno parte di un flusso di lavoro. Per informazioni sul dashboard delle bacheche, vedete [Utilizzare il dashboard delle bacheche](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). Potete fare clic su un nome di bacheca nel dashboard per aprirlo.

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
   <td> <p>[!UICONTROL Request] o superiore</p> </td> 
  </tr> 
 </tbody> 
</table>

## Creare un flusso di lavoro

{{step1-to-boards}}

1. Fai clic su **[!UICONTROL Aggiungi flusso di lavoro]** in [!UICONTROL Flussi di lavoro] area del dashboard.
1. Digitare un nome da sostituire **[!UICONTROL Flusso di lavoro senza titolo]** e premere Invio.

   Potete aggiungere bacheche al flusso di lavoro o fare clic su [!UICONTROL **Tutte le schede**] per tornare al dashboard.

## Crea una nuova bacheca in un flusso di lavoro

1. Se non sei già in un flusso di lavoro, fai clic su [!UICONTROL **Visualizza flusso di lavoro**] nel dashboard per aprire un flusso di lavoro esistente.
1. Fai clic su **[!UICONTROL Aggiungi bacheca]** sulla [!UICONTROL Schede] scheda del flusso di lavoro.
1. Selezionate un modello per la bacheca.

| Modello | Descrizione |
|---------|----------|
| Bacheca base | Sulla bacheca sono fornite tre colonne predefinite. È possibile aggiungere nuove colonne e rinominare o eliminare le colonne predefinite. <p>Non vengono applicati criteri di colonna. |
| Bacheca Kanban | Nella bacheca sono disponibili le colonne seguenti: Backlog, Nuovo, In corso, Completo e Bloccato. È possibile aggiungere nuove colonne e rinominare o eliminare le colonne predefinite.<p>Per utilizzare il backlog, è necessario impostare i filtri per la colonna di assunzione. Per informazioni, consulta [Aggiungere una colonna di assunzione a una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Per esaminare i criteri predefiniti per ciascuna colonna, fai clic sul pulsante [!UICONTROL **Altro** menu] su una colonna e seleziona [!UICONTROL **Modifica**]. È possibile modificare uno qualsiasi di questi criteri predefiniti. Per informazioni, consulta [Gestire le colonne della bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Bacheca retrospettiva | Nella bacheca sono disponibili le colonne seguenti: Cos&#39;è andato bene? Cosa migliorare? Con chi congratularsi? Come velocizzare? È possibile aggiungere nuove colonne e rinominare o eliminare le colonne predefinite. <p>Non vengono applicati criteri di colonna. |
| <span class="preview">Processo iterazione</span> | <span class="preview">Questa è la bacheca utilizzata per definire ed eseguire un&#39;iterazione. <p>Nella bacheca sono disponibili le colonne seguenti: Backlog, Nuovo, In corso, Completo e Bloccato. Non è possibile aggiungere colonne alla bacheca. <p>Per esaminare i criteri predefiniti per ciascuna colonna, fai clic sul pulsante [!UICONTROL **Altro**] in una colonna e seleziona [!UICONTROL **Modifica**]. È possibile modificare uno qualsiasi di questi criteri predefiniti. Per informazioni, consulta [Gestire le colonne della bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).</span> |

Per ulteriori informazioni sulla configurazione della bacheca, consultate [Creare o modificare una bacheca](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtrare l&#39;elenco delle bacheche in un flusso di lavoro

Quando nell&#39;elenco delle bacheche vengono applicati filtri diversi da quelli predefiniti, viene visualizzato un indicatore sull&#39;icona del filtro ![Filtro applicato](assets/boards-filterapplied-30x30.png). Fai clic su [!UICONTROL **Cancella tutto**] per rimuovere tutti i filtri e fare clic su [!UICONTROL **Nascondi filtri**] per chiudere il pannello del filtro.

{{step1-to-boards}}

1. Nel dashboard, fai clic su [!UICONTROL **Visualizza flusso di lavoro**] per aprire un flusso di lavoro.
1. Fai clic sul pulsante [!UICONTROL **Schede**] se non è già visualizzato.
1. Fai clic su [!UICONTROL **Filtro**].
1. Selezionate le bacheche da visualizzare in base allo stato (schede archiviate, bacheche attive o tutte le bacheche).
1. Selezionate le bacheche da visualizzare per modello.

## Aggiungere membri a un flusso di lavoro

È necessario aggiungere persone e team al flusso di lavoro come membri prima di poter visualizzare il flusso di lavoro e il relativo contenuto. Un membro del flusso di lavoro può aggiungere e rimuovere membri nel flusso di lavoro e vedere quali bacheche si trovano nel flusso di lavoro.

>[!NOTE]
>
>Un membro del flusso di lavoro non può aprire una bacheca in un flusso di lavoro finché non viene aggiunto a quella specifica bacheca come membro.

{{step1-to-boards}}

1. Nel dashboard, fai clic su [!UICONTROL **Visualizza flusso di lavoro**] per aprire un flusso di lavoro.
1. Fai clic sul pulsante **[!UICONTROL Aggiungi membro]** icona ![Aggiungi membri](assets/boards-addmember-spectrum-25x25.png) per aggiungere membri e team al flusso di lavoro.

   Si tratta dello stesso processo utilizzato per aggiungere membri a una bacheca. Per ulteriori informazioni, consulta [Aggiunta o rimozione di membri da una bacheca](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

<div class="preview">

## Configurare un flusso di lavoro

{{step1-to-boards}}

1. Nel dashboard, fai clic su [!UICONTROL **Visualizza flusso di lavoro**] per aprire un flusso di lavoro.
1. Fai clic su [!UICONTROL **Configura**] per aprire [!UICONTROL Configura flusso di lavoro] pannello.
1. (Facoltativo) Digitare una descrizione del flusso di lavoro. Questa descrizione viene visualizzata sul dashboard.

   Il numero totale di schede, il numero di schede puntate e il numero di iterazioni vengono visualizzati nella sezione Elenco schede. Fai clic su [!UICONTROL **Visualizza elenco**] per aprire l’elenco e aggiungere schede. Per ulteriori informazioni, consulta [Utilizza l&#39;elenco delle schede](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   Se è stata definita un’iterazione, vengono visualizzati la data di inizio, il numero di schede e il numero di punti. Fai clic su [!UICONTROL **Visualizza bacheca di iterazione**] per aprire la bacheca. Per ulteriori informazioni, consulta [Creare un’iterazione in un flusso di lavoro](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Fai clic su [!UICONTROL **Aggiungi origine**] per definire un&#39;origine per importare le schede nel flusso di lavoro. Al momento, l’unica sorgente disponibile è [!DNL Adobe Workfront].
1. Aggiungi dei filtri per importare attività e problemi da Workfront come schede.

   L&#39;aggiunta di filtri per le origini del flusso di lavoro equivale all&#39;aggiunta di filtri per una colonna di assunzione su una bacheca di base o una bacheca Kanban. Per ulteriori informazioni, consulta [Aggiungere una colonna di assunzione a una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

</div>
