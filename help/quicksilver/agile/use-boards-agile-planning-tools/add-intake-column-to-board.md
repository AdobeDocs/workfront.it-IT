---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Aggiungere una colonna di assunzione a una bacheca
description: Facoltativamente, puoi aggiungere alla bacheca una colonna di assunzione che richiama automaticamente le attività e i problemi come schede collegate quando vengono aggiunti in Workfront, in base ai filtri definiti dall'utente.
author: Lisa
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: 5e73603b695ff7456216ca7a4e15ce527b01559d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Aggiungere una colonna di assunzione a una bacheca

Facoltativamente è possibile aggiungere una colonna di assunzione alla bacheca che estrae automaticamente le attività e i problemi come schede collegate quando vengono aggiunti in [!DNL Workfront], in base ai filtri definiti dall’utente. La colonna di assunzione può fungere da colonna backlog per un team Kanban, da posizione di assunzione per un team di assistenza per visualizzare i problemi man mano che vengono aggiunti a una coda di richiesta o per qualsiasi altro scopo necessario.

Su una bacheca è consentita una sola colonna di assunzione ed è sempre visualizzata come la colonna più a sinistra.

La colonna di aspirazione non è disponibile su una scheda dinamica.

La colonna di assunzione è limitata a 300 attività e a 300 problemi. Sono ordinati in base alla priorità definita per gli elementi. Per informazioni sulla priorità, consulta [Aggiorna priorità attività](/help/quicksilver/manage-work/tasks/task-information/task-priority.md) e [Aggiorna priorità del problema](/help/quicksilver/manage-work/issues/issue-information/update-issue-priority.md).

Per ulteriori informazioni sulle colonne, consulta [Gestire le colonne della bacheca](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). Per informazioni sulle schede collegate, vedi [Utilizzare schede collegate sulle bacheche](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

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
   <td> <p>[!DNL Request] o superiore</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Creare una colonna di assunzione utilizzando filtri semplici

>[!NOTE]
>
>I filtri semplici sono disponibili solo tramite la funzionalità opt-in iniziale per le schede Adobe Workfront.

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **[!UICONTROL Schede]**.
1. Accedete a una bacheca. Per informazioni, consulta [Creare o modificare una bacheca](../../agile/get-started-with-boards/create-edit-board.md).
1. Fai clic su **[!UICONTROL Configura]** sulla destra della bacheca per aprire il pannello Configura .
1. Espandi **[!UICONTROL Scheda]**.
1. Attiva **[!UICONTROL Assorbimento dinamico di elementi a bordo]**.

   ![Opzioni filtro semplici per le colonne di entrata](assets/intake-column-simple-filters.png)

   La colonna di assunzione viene aggiunta a sinistra della tavola. Rimane vuoto finché non vengono applicati filtri.

1. (Facoltativo) Cerca e seleziona [!DNL Workfront] [!UICONTROL **Progetti**].
1. (Facoltativo) Cerca e seleziona l’utente o il team [!UICONTROL **Assegnazioni**].
1. Seleziona [!UICONTROL **Includi lavoro completato**] per visualizzare le attività e i problemi con uno stato Completo nella colonna di assunzione.

   >[!NOTE]
   >
   >Se questa opzione non è selezionata, quando le schede in altri stati sono contrassegnate come complete, verranno &quot;ritirate&quot; dalla bacheca e non verranno più visualizzate.

1. Fai clic su [!UICONTROL **Applica**].

   Tutti gli oggetti vengono visualizzati nella colonna di immissione della bacheca come schede collegate.

   ![Colonna acquisizione](assets/intake-column-added3.png)

## Creare una colonna di input utilizzando filtri avanzati

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **[!UICONTROL Schede]**.
1. Accedete a una bacheca. Per informazioni, consulta [Creare o modificare una bacheca](../../agile/get-started-with-boards/create-edit-board.md).
1. Fai clic su **[!UICONTROL Configura]** sulla destra della bacheca per aprire il pannello Configura .
1. Espandi **[!UICONTROL Scheda]**.
1. Attiva **[!UICONTROL Assorbimento dinamico di elementi a bordo]**.

   La colonna di assunzione viene aggiunta a sinistra della tavola. Rimane vuoto finché non vengono applicati filtri.

1. Fai clic su [!UICONTROL **Utilizzare filtri avanzati**].
1. Fai clic su **[!UICONTROL Origini del filtro]** e seleziona **[!UICONTROL Attività]** o **[!UICONTROL Problemi]**.

   ![Opzioni filtro avanzate della colonna di input](assets/intake-column-advanced-filters1.png)

   >[!NOTE]
   >
   >È possibile filtrare la colonna di assunzione per includere sia le attività che i problemi, ma è necessario impostare i filtri separatamente per ciascun tipo di oggetto.
   >
   >Sono inoltre disponibili filtri salvati e filtri predefiniti di sistema da selezionare.

1. Nel pannello del filtro, fai clic su **[!UICONTROL Nuovo filtro]** per iniziare.

   ![Fai clic su Nuovo filtro](assets/intake-filter-dialog5.png)

1. Crea il filtro e fai clic su **[!UICONTROL Salva come nuovo]**.

   ![Generatore di filtri](assets/intake-filter-dialog6.png)

   Questo esempio mostra un filtro per le attività di un progetto specifico che si trovano nello stato di [!UICONTROL Nuovo] o [!UICONTROL In corso]e sono assegnati a me.

   Per informazioni sulla creazione di un filtro, consulta la sezione &quot;Creare o modificare un filtro nel generatore standard&quot; nell’articolo [Creare o modificare i filtri in [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

1. Denomina il filtro e fai clic su **[!UICONTROL Salva]**.

   ![Digitare un nome per il filtro](assets/intake-filter-dialog7.png)

   Assegnare al filtro un nome univoco ti consente di cercarlo in un secondo momento.

1. Il filtro viene visualizzato nell’elenco dei filtri salvati e viene applicato automaticamente alla colonna di assunzione. Fai clic sulla X nella parte superiore del pannello del filtro per chiuderlo.

   ![Filtro salvato](assets/intake-filter-dialog8.png)

1. (Facoltativo) Per condividere il filtro con altri utenti, passa il puntatore del mouse sul filtro salvato e fai clic sul pulsante **[!UICONTROL Altro]** menu ![Icona menu Altro](assets/more-icon-spectrum.png), quindi seleziona **[!UICONTROL Condividi]**. Scegli gli utenti o i team con cui condividere nella casella Condivisione filtro . Per ulteriori informazioni, consulta [Condividere un filtro, una visualizzazione o un raggruppamento](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
1. (Facoltativo) Per includere attività e problemi nella colonna di assunzione, fare clic su **[!UICONTROL Origini del filtro]** e selezionare l&#39;altro oggetto per creare un altro filtro.
1. Al termine dell’aggiunta dei filtri, controlla la colonna di immissione per verificare che siano visualizzate le attività e i problemi corretti.

   ![Colonna acquisizione](assets/intake-column-added3.png)

   >[!NOTE]
   >
   >Per aggiornare i filtri in qualsiasi momento, apri il pannello Configura e fai clic su **[!UICONTROL Origini del filtro]** e selezionando **[!UICONTROL Attività]** o **[!UICONTROL Problemi]**.

## Utilizzare la colonna di assunzione

Le schede nella colonna di assunzione non sono modificabili finché non le si spostano in altre colonne della bacheca. Potete fare clic sulla scheda per aprirla in una visualizzazione di sola lettura oppure fare clic su ![Apri attività o problema](assets/boards-launch-icon.png) per aprire l’attività o il problema in una nuova scheda del browser.


Potete riordinare manualmente gli elementi nella colonna di assunzione.

Le icone in alto a destra della colonna di assunzione mostrano il numero di schede attualmente presenti nella colonna e il numero di filtri applicati.

1. (Facoltativo) Per cercare un elemento nella colonna di assunzione, fare clic su ![Icona Ricerca](assets/search-icon.png) nella colonna .
1. (Facoltativo) Per spostare una scheda dalla colonna di assunzione in un&#39;altra colonna, trascinate la scheda nella posizione desiderata.

   Oppure

   Fai clic sul pulsante **[!UICONTROL Altro]** menu ![Icona menu Altro](assets/more-icon-spectrum.png) sulla scheda e seleziona **[!UICONTROL Sposta]**. Quindi, sul **[!UICONTROL Sposta elemento]** scegliere un&#39;altra colonna e selezionare **[!UICONTROL Sposta]**.

1. (Facoltativo) Per eliminare la colonna di assunzione, fare clic sul pulsante **[!UICONTROL Altro]** menu ![Icona menu Altro](assets/more-icon-spectrum.png) e seleziona **[!UICONTROL Elimina]**.
