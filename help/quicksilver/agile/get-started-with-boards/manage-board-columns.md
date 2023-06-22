---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Gestisci colonne bacheca
description: Per impostazione predefinita, una nuova bacheca contiene tre colonne. È possibile aggiungere altre colonne, modificare l'ordine delle colonne, rinominare le colonne ed eliminare le colonne non necessarie.
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 05cac2441474e0f6ecf18aa777a5a66fefb2dba8
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 0%

---

# Gestisci colonne bacheca

Per impostazione predefinita, una nuova bacheca contiene tre colonne. È possibile aggiungere altre colonne, modificare l&#39;ordine delle colonne, rinominare le colonne ed eliminare le colonne non necessarie.

Le impostazioni delle colonne includono i criteri, che consentono di definire le opzioni per ciò che accade a una scheda quando viene spostata in quella colonna.

Per informazioni sull’ordinamento delle schede in colonne, consulta [Filtrare ed eseguire ricerche in una bacheca](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

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
   <td> <p>[!UICONTROL Request] o versione successiva</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Aggiungere una colonna a una bacheca

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Schede]**.
1. Accedi a una bacheca. Per informazioni, consulta [Creare o modificare una bacheca](../../agile/get-started-with-boards/create-edit-board.md).
1. Clic **[!UICONTROL Aggiungi colonna]** a destra delle colonne esistenti.
1. Nella nuova colonna digitare un nome e fare clic su **[!UICONTROL Aggiungi colonna]**.

   ![Aggiungi nuova colonna](assets/boards-add-column.png)

>[!TIP]
>
>Per aggiungere una colonna Acquisizione, vedi [Aggiungere una colonna Acquisizione a una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Riordinare le colonne su una bacheca

1. Accedi alla bacheca.
1. Trascinare le colonne nell&#39;ordine corretto. Assicurarsi di selezionare la parte superiore della colonna prima di trascinarla in un&#39;altra posizione.

   ![Trascina la colonna](assets/boards-dragdropcolumn.png)

## Rinominare una colonna della bacheca

1. Accedi alla bacheca.
1. Fare clic sul nome della colonna, digitare il nuovo nome e premere Invio.

   Oppure

   Fai clic su **[!UICONTROL Altro]** menu ![Menu Altro](assets/more-icon-spectrum.png) nella colonna e seleziona **[!UICONTROL Modifica]**. Nell&#39;area Impostazioni, digitare il nuovo nome nella **[!UICONTROL Nome colonna]** e fai clic su **[!UICONTROL Chiudi]**.

## Eliminare una colonna della bacheca

Quando elimini una colonna da una bacheca, non può essere recuperata.

1. Accedi alla bacheca.
1. Fai clic su **[!UICONTROL Altro]** menu ![Menu Altro](assets/more-icon-spectrum.png) nella colonna e seleziona **[!UICONTROL Elimina]**.

   >[!NOTE]
   >
   >Impossibile eliminare le colonne che contengono schede, incluse le schede archiviate. Se tenti di eliminare una colonna che contiene schede, devi scegliere un’altra colonna per tali schede.

## Visualizza conteggio schede

Puoi utilizzare un’impostazione di configurazione per visualizzare il numero di schede in ogni colonna.

Se si utilizza il limite WIP in una colonna, non viene aggiunto un contatore di schede separato. Per ulteriori informazioni sui limiti WIP, vedere [Gestire [!UICONTROL Lavoro in corso] Limite (WIP) su una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Accedi alla bacheca.
1. Clic **[!UICONTROL Configura]** sulla destra della bacheca per aprire il pannello Configura.
1. Espandi **[!UICONTROL Colonna]**.
1. Attiva **[!UICONTROL Visualizza un conteggio colonne schede]**.

   ![Attiva contatore schede](assets/display-card-count.png)

   Il contatore di schede viene visualizzato nella parte superiore di ogni colonna.

1. Clic **[!UICONTROL Nascondi configurazione]** per chiudere [!UICONTROL Configura] pannello.

## Definire le impostazioni e i criteri delle colonne

1. Accedi alla bacheca.
1. Fai clic su **[!UICONTROL Altro]** menu ![Menu Altro](assets/more-icon-spectrum.png) nella colonna e seleziona **[!UICONTROL Modifica]**.

   Il [!UICONTROL Impostazioni] viene visualizzata. Il **[!UICONTROL Nome colonna]** consente di sapere per quale colonna si stanno definendo le impostazioni.

1. Abilita **[!UICONTROL Aggiorna automaticamente i valori dei campi]** criterio per modificare automaticamente alcuni valori di campo quando una scheda viene spostata in questa colonna.

   ![Impostazioni e criteri colonna](assets/boards-column-policies-enabled.png)

1. (Facoltativo) Imposta un valore per lo stato della scheda:

   1. Seleziona la **[!UICONTROL Stato]** casella di controllo.

   1. Selezionare lo stato da applicare a una scheda quando viene spostata in questa colonna.

      ![Stato delle colonne](assets/boards-column-status.png)

      Vengono visualizzate anche le opzioni di traduzione dello stato per le schede collegate. La traduzione dello stato non si applica alle schede ad hoc. Queste opzioni determinano lo stato personalizzato applicato all’attività o al problema in [!DNL Workfront] quando una scheda collegata viene spostata in questa colonna.

   1. Seleziona un [!UICONTROL **Personalizzato**] stato da applicare alla scheda per le attività e per i problemi.

      Quando una scheda viene spostata in questa colonna, [!DNL Workfront] prima tenta di applicare lo stato personalizzato (ad esempio, Risolto). Se lo stato personalizzato selezionato non è disponibile per tale scheda, viene richiesto di scegliere un altro stato che corrisponda allo stato del sistema (dal passaggio b sopra). Per ulteriori informazioni sugli stati, consulta [Panoramica sugli stati](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      Inoltre, se lo stato dell’attività o del problema connesso viene modificato nello stato personalizzato o di sistema impostato nella policy di colonna, la scheda viene automaticamente spostata nella colonna.

1. (Facoltativo) Imposta un valore per gli assegnatari della carta:

   1. Seleziona la **[!UICONTROL Assegnatari]** casella di controllo.
   1. Seleziona un’azione.

      * **[!UICONTROL Aggiungi su assegnatari]:** Gli assegnatari selezionati vengono aggiunti all&#39;elenco esistente di assegnatari su una scheda quando questa viene spostata in questa colonna.
      * **[!UICONTROL Sostituisci assegnatari]:** Gli assegnatari selezionati sostituiscono tutti gli altri assegnatari e diventano gli unici assegnatari su una scheda quando viene spostata in questa colonna.
   1. Seleziona gli assegnatari dall’elenco a discesa. Solo i membri della bacheca sono disponibili per la scelta. Per ulteriori informazioni, consulta [Aggiungere o rimuovere membri da una bacheca](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

      ![Assegnatari per colonna](assets/boards-column-assignees.png)


1. (Facoltativo) Imposta un valore per i tag della scheda:

   1. Seleziona la **[!UICONTROL Schede]** casella di controllo.
   1. Seleziona un’azione.

      * **[!UICONTROL Aggiungi su tag]:** I tag selezionati vengono aggiunti all&#39;elenco esistente di tag su una scheda quando questa viene spostata in questa colonna.
      * **[!UICONTROL Sostituisci tag]:** I tag selezionati sostituiscono tutti gli altri tag e diventano gli unici tag di una scheda quando viene spostata in questa colonna.
   1. Seleziona i tag dall’elenco a discesa. Solo i tag già creati nel [!UICONTROL Gestione tag] sono disponibili per la scelta. Per informazioni sull’aggiunta di nuovi tag, consulta [Aggiungi tag](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Tag per colonna](assets/boards-column-tags.png)


1. Abilita **[!UICONTROL Limite work in progress]** criterio per limitare il numero di schede che possono essere aggiunte alla colonna. Quindi, digita il numero limite nel **[!UICONTROL Imposta limite]** campo.

   ![Limite WIP per colonna](assets/boards-wip-limit-in-column.png)

   Per ulteriori informazioni, consulta [Gestire il limite WIP (Work In Progress) su una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Clic **[!UICONTROL Chiudi]** per uscire dall&#39;area Impostazioni e visualizzare la colonna e le relative schede.
