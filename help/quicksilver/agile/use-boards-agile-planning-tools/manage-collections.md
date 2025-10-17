---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Gestisci flussi di lavoro
description: Un flusso di lavoro è un gruppo configurabile di schede e schede per la collaborazione sul lavoro.
author: Jenny
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 1%

---

# Gestire i flussi di lavoro

>[!IMPORTANT]
>
>I flussi di lavoro sono disponibili solo per un gruppo specifico di clienti.

Un flusso di lavoro è un gruppo configurabile di schede e schede per la collaborazione sul lavoro. I flussi di lavoro possono includere diversi tipi di bacheche create da modelli e un elenco di schede di elementi di lavoro. In un flusso di lavoro è possibile tenere traccia del lavoro in iterazioni o sprint.

Per ulteriori informazioni, vedere [Utilizzare l&#39;elenco delle schede](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) e [Creare un&#39;iterazione in un flusso di lavoro](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

I flussi di lavoro vengono visualizzati nel dashboard insieme alle singole schede a cui hai accesso che non fanno parte di un flusso di lavoro. Per informazioni sul dashboard delle bacheche, vedere [Utilizzare il dashboard delle bacheche](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). Puoi fare clic sul nome di una bacheca qualsiasi sul dashboard per aprirla.

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
   <td> 
   <p>Collaboratore o versione successiva</p> 
   <p>Richiedi o superiore</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creare un flusso di lavoro

{{step1-to-boards}}

1. Fare clic su **[!UICONTROL Aggiungi flusso di lavoro]** nell&#39;area [!UICONTROL Flussi di lavoro] del dashboard.
1. Digitare un nome per sostituire **[!UICONTROL Flusso di lavoro senza titolo]** e premere Invio.

   Puoi aggiungere delle bacheche al flusso di lavoro oppure fare clic su [!UICONTROL **Tutte le bacheche**] per tornare alla bacheca.

## Creare una nuova bacheca in un flusso di lavoro

1. Se non si è già in un flusso di lavoro, fare clic su [!UICONTROL **Visualizza flusso di lavoro**] nel dashboard per aprire un flusso di lavoro esistente.
1. Fai clic su **[!UICONTROL Aggiungi bacheca]** nella scheda [!UICONTROL Bacheche] del flusso di lavoro.
1. Seleziona un modello per la bacheca.

| Modello | Descrizione |
|---------|----------|
| Bacheca base | Sulla bacheca sono disponibili tre colonne predefinite. È possibile aggiungere nuove colonne e rinominare o eliminare le colonne predefinite. <p>Nessun criterio colonna applicato. |
| Bacheca Kanban | Nella bacheca sono disponibili le seguenti colonne: Backlog, Nuovo, In corso, Completo e In sospeso. È possibile aggiungere nuove colonne e rinominare o eliminare le colonne predefinite.<p>Per utilizzare il backlog, è necessario impostare i filtri per la colonna Acquisizione. Per informazioni, vedere [Aggiungere una colonna di acquisizione a una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Per rivedere i criteri predefiniti per ogni colonna, fare clic sul menu [!UICONTROL **Altro**] in una colonna e selezionare [!UICONTROL **Modifica**]. Puoi modificare uno qualsiasi di questi criteri predefiniti. Per informazioni, consulta [Gestire le colonne della bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Bacheca retrospettiva | Sulla bacheca sono fornite le seguenti colonne: Cosa è andato bene? Cosa si può migliorare? Chi dovremmo festeggiare? Cosa possiamo fare per muoverci più velocemente? È possibile aggiungere nuove colonne e rinominare o eliminare le colonne predefinite. <p>Nessun criterio colonna applicato. |
| Processo iterazione | Bacheca utilizzata per definire ed eseguire un&#39;iterazione. <p>Nella bacheca sono disponibili le seguenti colonne: Backlog, Nuovo, In corso, Completo e In sospeso. Non è possibile aggiungere colonne alla bacheca. <p>Per rivedere i criteri predefiniti per ogni colonna, fare clic sul menu [!UICONTROL **Altro**] in una colonna e selezionare [!UICONTROL **Modifica**]. Puoi modificare uno qualsiasi di questi criteri predefiniti. Per informazioni, consulta [Gestire le colonne della bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

Per ulteriori informazioni sulla configurazione della bacheca, vedere [Creare o modificare una bacheca](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtrare l’elenco delle bacheche in un flusso di lavoro

Quando nell&#39;elenco delle bacheche vengono applicati filtri diversi da quelli predefiniti, viene visualizzato un indicatore sull&#39;icona del filtro ![Filtro applicato](assets/boards-filterapplied-30x30.png). Fai clic su [!UICONTROL **Cancella tutto**] per rimuovere tutti i filtri, quindi fai clic su [!UICONTROL **Nascondi filtri**] per chiudere il pannello dei filtri.

{{step1-to-boards}}

1. Nel dashboard fare clic su [!UICONTROL **Visualizza flusso di lavoro**] per aprire un flusso di lavoro.
1. Fare clic sulla scheda [!UICONTROL **Bacheche**] se non è già visualizzata.
1. Fai clic su [!UICONTROL **Filtro**].
1. Seleziona le bacheche che desideri visualizzare per stato (bacheche archiviate, bacheche attive o tutte).
1. Seleziona le bacheche da visualizzare per modello.

## Aggiungere membri a un flusso di lavoro

È necessario aggiungere persone e team al flusso di lavoro come membri prima che possano visualizzarne il flusso e il contenuto. Un membro del flusso di lavoro può aggiungere e rimuovere membri nel flusso di lavoro e vedere quali bacheche sono presenti nel flusso di lavoro.

>[!NOTE]
>
>Un membro del flusso di lavoro non può aprire una bacheca in un flusso di lavoro finché non viene aggiunto come membro a tale bacheca specifica.

{{step1-to-boards}}

1. Nel dashboard fare clic su [!UICONTROL **Visualizza flusso di lavoro**] per aprire un flusso di lavoro.
1. Fare clic sull&#39;icona **[!UICONTROL Aggiungi membro]** ![Aggiungi membri](assets/boards-addmember-spectrum-25x25.png) per aggiungere membri e team al flusso di lavoro.

   È lo stesso processo utilizzato per aggiungere membri a una bacheca. Per ulteriori informazioni, vedere [Aggiungere o rimuovere membri da una bacheca](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

## Aggiungere origini a un flusso di lavoro

Una sorgente determina la provenienza delle schede nel flusso di lavoro.

{{step1-to-boards}}

1. Fai clic sull&#39;icona [!UICONTROL **Origini**] ![Origini](assets/sources-icon.png) per definire un&#39;origine per l&#39;importazione di schede nel flusso di lavoro. Al momento, l&#39;unica origine disponibile è [!DNL Adobe Workfront].
1. Aggiungi filtri per importare attività e problemi da Workfront come schede.

   L’aggiunta di filtri per le origini del flusso di lavoro è identica all’aggiunta di filtri avanzati per una colonna di acquisizione su una bacheca di base o su una bacheca Kanban. Per ulteriori informazioni, vedere [Aggiungere una colonna di acquisizione a una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Configurare un flusso di lavoro

{{step1-to-boards}}

1. Nel dashboard fare clic su [!UICONTROL **Visualizza flusso di lavoro**] per aprire un flusso di lavoro.
1. Fare clic su [!UICONTROL **Configura**] per aprire il pannello [!UICONTROL Configura flusso di lavoro].
1. (Facoltativo) Espandere [!UICONTROL **Flusso di lavoro**] e digitare una descrizione del flusso di lavoro. Questa descrizione viene visualizzata nel dashboard.
1. (Facoltativo) Espandere [!UICONTROL **Iterazioni**] per definire un processo di iterazione per questo flusso di lavoro.

   Il numero totale di carte, il numero di carte puntate e il numero di iterazioni sono visualizzati nella sezione Elenco carte. Fai clic su [!UICONTROL **Visualizza elenco**] per aprire l&#39;elenco e aggiungere schede. Per ulteriori informazioni, vedere [Utilizzare l&#39;elenco delle schede](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   Se è già stata definita un’iterazione, vengono visualizzati la data di inizio, il numero di schede e il numero di punti. Fare clic su [!UICONTROL **Visualizza bacheca**] per aprire la bacheca di iterazione. Per ulteriori informazioni, vedere [Creare un&#39;iterazione in un workflow](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Espandi [!UICONTROL **Tag**] per aggiungere tag al flusso di lavoro (facoltativo). Cercare un tag o digitare un nuovo nome di tag nella casella di ricerca e premere Invio per crearlo.
