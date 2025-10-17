---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Aggiungere una colonna Acquisizione a una bacheca
description: Facoltativamente, puoi aggiungere alla bacheca una colonna di acquisizione che richiama automaticamente le attività e i problemi come schede collegate quando vengono aggiunte in Workfront, in base ai filtri definiti.
author: Jenny
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1033'
ht-degree: 3%

---

# Aggiungere una colonna Acquisizione a una bacheca

<!-- Audited: 5/2025 -->

Facoltativamente, puoi aggiungere alla bacheca una colonna di acquisizione che richiama automaticamente le attività e i problemi come schede collegate quando vengono aggiunte in [!DNL Workfront] in base ai filtri definiti. La colonna Acquisizione può fungere da colonna di backlog per un team Kanban, da posizione di acquisizione per un team di supporto per visualizzare i problemi man mano che vengono aggiunti a una coda di richieste o per qualsiasi altro scopo.

È consentita una sola colonna di acquisizione su una bacheca, che viene sempre visualizzata come la colonna più a sinistra.

La colonna Acquisizione non è disponibile su una bacheca dinamica. Tuttavia, puoi aggiornare i filtri che definiscono quali schede vengono inserite in una bacheca dinamica. Quando si modificano questi filtri su una scheda dinamica, le impostazioni della scheda che non fanno parte dell’attività o del problema di Workfront (come i tag) vengono reimpostate.

>[!NOTE]
>
>Per motivi di sicurezza, solo il proprietario di una bacheca può modificarne i filtri nel pannello Configura.

La colonna Assunzione è limitata a 300 attività e 300 problemi. L’ordine predefinito degli elementi nella colonna Acquisizione è il seguente:

Attività:

* Ordine principale: nome progetto
* Ordine secondario: struttura dettaglio lavoro

Problemi:

* Ordine principale: nome progetto
* Ordine secondario: numero di riferimento

>[!IMPORTANT]
>
>Si consiglia di aggiornare frequentemente la bacheca se più utenti lavorano contemporaneamente sulla bacheca. L’aggiornamento della pagina consente di mantenere aggiornate le modifiche visive sulla bacheca e impedisce problemi come lo spostamento di schede duplicate nella bacheca dalla colonna acquisizione.
>
>Per eseguire la sincronizzazione con Workfront e inserire nuove attività e problemi nella colonna della bacheca o dell&#39;accettazione, fare clic sul menu Altro ![[!UICONTROL Altro menu]](assets/more-menu.png) accanto al nome della bacheca e selezionare Sincronizza elementi connessi.

Per ulteriori informazioni sulle colonne, vedere [Gestisci colonne bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). Per informazioni sulle schede collegate, vedere [Utilizzare le schede collegate sulle schede](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

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

## Creare una colonna di acquisizione utilizzando filtri semplici

{{step1-to-boards}}

1. Nel dashboard, seleziona una bacheca.
1. Fai clic su **Configura** a destra della bacheca per aprire il pannello **Configura**.
1. Seleziona la sezione **Bacheca**. Vengono visualizzati nuovi campi.
1. Attiva **acquisizione dinamica di elementi nella bacheca**. La colonna dell’aspirazione vuota viene visualizzata sul lato sinistro della bacheca.

   ![Opzioni filtro semplice colonna acquisizione](assets/board-section.png)

1. (Facoltativo) Cerca e seleziona [!DNL Workfront] [!UICONTROL **Progetti**].
1. (Facoltativo) Cerca e seleziona l&#39;utente o il team [!UICONTROL **Assegnazioni**].
1. Fare clic su **Applica**. Gli oggetti vengono visualizzati nella colonna di acquisizione della bacheca come schede collegate.

   ![Colonna acquisizione](assets/intake-column-added3.png)

## Creare una colonna di acquisizione utilizzando filtri avanzati

{{step1-to-boards}}

1. Nel dashboard, seleziona una bacheca.
1. Fai clic su **Configura** a destra della bacheca per aprire il pannello **Configura**.
1. Seleziona la sezione **Bacheca**. Vengono visualizzati nuovi campi.
1. Attiva **acquisizione dinamica di elementi nella bacheca**. La colonna dell’aspirazione vuota viene visualizzata sul lato sinistro della bacheca.

1. Fare clic su [!UICONTROL **Usa filtri avanzati**].

1. Fai clic su **[!UICONTROL Aggiungi origini filtro]**, quindi seleziona **[!UICONTROL Attività]** o **[!UICONTROL Problemi]**.

   ![Opzioni filtro avanzate colonna acquisizione](assets/add-filter-sources-options.png)

   >[!NOTE]
   >
   >È possibile filtrare la colonna Acquisizione in modo da includere sia attività che problemi, ma è necessario impostare i filtri separatamente per ogni tipo di oggetto.
   >
   >Inoltre, sono disponibili filtri salvati e filtri di sistema predefiniti da selezionare.

1. Nel pannello dei filtri, fai clic su **[!UICONTROL Nuovo filtro]**.

1. Genera il filtro, quindi fai clic su **[!UICONTROL Salva come nuovo]**.

   ![Generatore di filtri](assets/intake-filter-dialog6.png)

   L&#39;esempio precedente mostra un filtro per le attività di un progetto specifico con stato [!UICONTROL Nuovo] o [!UICONTROL In corso].

   >[!NOTE]
   >
   >Si consiglia di non utilizzare il carattere jolly &quot;Me&quot; (utente connesso) in un filtro della bacheca, perché non è garantito che vengano sempre visualizzate le attività o i problemi per l’utente connesso. Dopo aver configurato la bacheca con le attività e i problemi corretti, puoi filtrarla per mostrare gli elementi per un assegnatario specifico. Per ulteriori informazioni, consulta [Filtrare e cercare in una bacheca](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   Per ulteriori dettagli sulla creazione di un filtro, vedere la sezione Creare o modificare un filtro nel generatore standard nell&#39;articolo [Creare o modificare filtri in [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

1. Assegna un nome al filtro, quindi fai clic su **[!UICONTROL Salva]**. Il filtro viene visualizzato nell’elenco dei filtri salvati e viene applicato automaticamente alla colonna Acquisizione.

   ![Inserimento di un nuovo nome di filtro](assets/save-as-modal.png)

1. Fai clic sulla X nella parte superiore del pannello del filtro per chiuderlo.

1. (Facoltativo) Per condividere il filtro con altri utenti, passa il puntatore del mouse sul filtro salvato, fai clic sul menu **[!UICONTROL Altro]** ![Icona altro menu](assets/more-menu.png) e seleziona **[!UICONTROL Condividi]**. Scegliere gli utenti o i team con cui condividere nella casella **Condivisione filtro**. Per ulteriori informazioni, vedere [Condividere un filtro, una visualizzazione o un raggruppamento](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
1. (Facoltativo) Per includere sia attività che problemi nella colonna Acquisizione, fare clic su **[!UICONTROL Filtra origini]** e selezionare l&#39;altro oggetto per creare un altro filtro.
1. Dopo aver aggiunto i filtri, controlla la colonna Acquisizione per verificare che vengano visualizzate le attività e i problemi corretti.

   ![Colonna acquisizione](assets/intake-column-added3.png)

   >[!NOTE]
   >
   >Puoi aggiornare i filtri in qualsiasi momento aprendo il pannello Configura, facendo clic su **[!UICONTROL Filtra origini]** e selezionando **[!UICONTROL Attività]** o **[!UICONTROL Problemi]**.

## Utilizzare la colonna Acquisizione

Le schede nella colonna Acquisizione non sono modificabili finché non vengono spostate in altre colonne della bacheca. Puoi fare clic sulla scheda per aprirla in una visualizzazione di sola lettura, oppure fare clic su ![Apri attività o problema](assets/boards-launch-icon.png) per aprire l&#39;attività o il problema in una nuova scheda del browser.

Puoi riordinare manualmente gli elementi nella colonna Acquisizione.

Le icone in alto a destra nella colonna Acquisizione mostrano quante schede ci sono attualmente nella colonna e quanti filtri vengono applicati.

1. (Facoltativo) Per cercare un elemento nella colonna Acquisizione, fare clic su ![Icona Ricerca](assets/search-icon.png) nella colonna.
1. (Facoltativo) Per spostare una scheda dalla colonna Acquisizione a un’altra colonna, trascina e rilascia la scheda nella posizione in cui desideri che venga visualizzata.

   Oppure

   Fai clic sul menu **[!UICONTROL Altro]** ![Icona altro menu](assets/more-menu.png) sulla scheda e seleziona **[!UICONTROL Sposta]**. Quindi, nella casella **Sposta [ELEMENTO]**, scegliere un&#39;altra colonna e selezionare **[!UICONTROL Sposta]**.

1. (Facoltativo) Per eliminare la colonna Acquisizione, fai clic sul menu **[!UICONTROL Altro]** ![Icona altro menu](assets/more-menu.png) e seleziona **[!UICONTROL Elimina]**.
