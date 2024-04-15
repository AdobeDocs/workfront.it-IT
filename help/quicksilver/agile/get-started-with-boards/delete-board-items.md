---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Eliminare o archiviare una scheda da una bacheca
description: Quando elimini una scheda da una bacheca, questa viene eliminata definitivamente e non può essere ripristinata. Quando si archivia una scheda, questa viene inviata all'archivio e può essere successivamente ripristinata nella bacheca.
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: 46099e6ceba4310453743c023823e8952f5ce553
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---

# Eliminare o archiviare una scheda da una bacheca

Quando elimini una scheda ad hoc da una bacheca, questa viene eliminata definitivamente e non può essere ripristinata. Le schede collegate possono essere aggiunte manualmente a una bacheca dopo essere state eliminate.

Se elimini una scheda connessa da una scheda dinamica, questa verrà visualizzata nuovamente quando aggiorni la scheda, perché questo tipo di scheda richiama tutte le attività e i problemi di un progetto specifico. Per eliminare la scheda, devi eliminare l’attività o il problema connesso dal progetto Workfront.

Quando elimini una scheda collegata da qualsiasi altro tipo di scheda che dispone di una colonna di acquisizione, la scheda viene visualizzata nuovamente nella colonna di acquisizione quando si aggiorna la scheda se l’attività o il problema connesso non è ancora contrassegnato come completato. Per ulteriori informazioni sulle colonne di assunzione, consulta [Aggiungere una colonna Acquisizione a una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

Quando si archivia una scheda, questa viene inviata all&#39;archivio e può essere successivamente ripristinata nella bacheca.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Request] o versione successiva</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Eliminare una scheda da una bacheca

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Schede]**.
1. Accedi a una bacheca. Per informazioni, consulta [Creare o modificare una bacheca](../../agile/get-started-with-boards/create-edit-board.md).
1. Fai clic su **[!UICONTROL Altro]** menu ![Menu Altro](assets/more-icon-spectrum.png) sulla scheda e seleziona **[!UICONTROL Elimina]**.
1. Clic **[!UICONTROL Elimina]** sul messaggio di conferma.

## Archiviare una scheda da una bacheca

1. Accedi alla bacheca.
1. Fai clic su **[!UICONTROL Altro]** menu ![Menu Altro](assets/more-icon-spectrum.png) sulla scheda e seleziona **[!UICONTROL Archivia]**.

   Le schede archiviate sono nascoste dalla bacheca a meno che non si applichi un filtro per visualizzarle. Per ulteriori informazioni, consulta [Filtrare una bacheca per mostrare le schede archiviate](#filter-a-board-to-show-archived-cards) in questo articolo.

   Un [!UICONTROL Archivia] icona ![Archivia](assets/archive-icon-spectrum-25x20.png) viene visualizzato sulle schede archiviate. Non puoi modificare una scheda archiviata, ma puoi eliminarla o spostarla in un’altra colonna.

1. Per ripristinare una scheda archiviata, fai clic su **[!UICONTROL Altro]** menu ![Menu Altro](assets/more-icon-spectrum.png) sulla scheda e seleziona **[!UICONTROL Ripristina]**.

## Filtrare una bacheca per mostrare le schede archiviate {#filter-a-board-to-show-archived-cards}

Per impostazione predefinita, su una bacheca vengono visualizzate solo le schede attive. Puoi filtrare la bacheca per visualizzare anche eventuali schede archiviate.

1. Accedi alla bacheca.
1. Clic [!UICONTROL **Configura**] sulla destra della bacheca per aprire il pannello Configura.
1. Espandi [!UICONTROL **Schede**].
1. Attiva [!UICONTROL **Visualizza le schede archiviate sulla bacheca**].
1. Clic [!UICONTROL **Filtro**], espandi [!UICONTROL Schede archiviate] e seleziona **[!UICONTROL Schede archiviate]** per visualizzare le schede archiviate.

   Il filtro mostra il numero di schede archiviate.

   ![Filtra schede archiviate](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >Il [!UICONTROL Schede archiviate] La sezione non è disponibile nel filtro se non hai attivato l’impostazione di configurazione per visualizzare le schede archiviate. Per ulteriori informazioni, consulta [Personalizzare i campi visualizzati su una scheda](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Seleziona **[!UICONTROL Schede archiviate]** per cancellare l&#39;opzione e visualizzare solo le schede attive.
