---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Gestire le colonne della bacheca
description: Per impostazione predefinita, una nuova bacheca contiene tre colonne. È possibile aggiungere altre colonne, modificare l’ordine delle colonne, rinominare le colonne ed eliminare le colonne non necessarie.
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 2dfa3e7b215a8234453b2d688031c993978e02ae
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# Gestire le colonne della bacheca

Per impostazione predefinita, una nuova bacheca contiene tre colonne. È possibile aggiungere altre colonne, modificare l’ordine delle colonne, rinominare le colonne ed eliminare le colonne non necessarie.

Le impostazioni colonna includono criteri che ti consentono di definire le opzioni per ciò che accade a una scheda quando viene spostata in quella colonna.

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

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Aggiungere una colonna a una bacheca

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Schede]**.
1. Accedete a una bacheca. Per informazioni, consulta [Creare o modificare una bacheca](../../agile/get-started-with-boards/create-edit-board.md).
1. Fai clic su **[!UICONTROL Aggiungi colonna]** a destra delle colonne esistenti.
1. Nella nuova colonna, digita un nome e fai clic su **[!UICONTROL Aggiungi colonna]**.

   ![Aggiungi nuova colonna](assets/boards-add-column.png)

>[!TIP]
>
>Per aggiungere una colonna di aspirazione, vedi [Aggiungere una colonna di assunzione a una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Riordinare le colonne su una bacheca

1. Accedete alla bacheca.
1. Trascina e rilascia le colonne nell’ordine corretto. Assicurati di selezionare la parte superiore della colonna prima di trascinarla in un’altra posizione.

   ![Trascina la colonna](assets/boards-dragdropcolumn.png)

## Rinominare una colonna di una bacheca

1. Accedete alla bacheca.
1. Fare clic sul nome della colonna, digitare il nuovo nome e premere Invio.

   Oppure

   Fai clic sul pulsante **[!UICONTROL Altro]** menu ![Menu Altro](assets/more-icon-spectrum.png) nella colonna e seleziona **[!UICONTROL Modifica]**. Nell’area Impostazioni, digita il nuovo nome nel campo **[!UICONTROL Nome colonna]** e fai clic su **[!UICONTROL Chiudi]**.

## Eliminare una colonna di una bacheca

1. Accedete alla bacheca.
1. Fai clic sul pulsante **[!UICONTROL Altro]** menu ![Menu Altro](assets/more-icon-spectrum.png) nella colonna e seleziona **[!UICONTROL Elimina]**.

   >[!NOTE]
   >
   >Impossibile eliminare le colonne contenenti schede, incluse le schede archiviate. Se tenti di eliminare una colonna contenente schede, devi scegliere un’altra colonna per tali schede.

## Conteggio schede display

Puoi utilizzare un’impostazione di configurazione per visualizzare il numero di schede in ogni colonna.

Se si utilizza il limite WIP su una colonna, non viene aggiunto un contatore di schede separato. Per ulteriori informazioni sui limiti WIP, vedi [Gestire [!UICONTROL Lavori in corso] Limite (WIP) su una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Accedete alla bacheca.
1. Fai clic su **[!UICONTROL Configura]** sulla destra della bacheca per aprire il pannello Configura .
1. Espandi **[!UICONTROL Colonna]**.
1. Attiva **[!UICONTROL Visualizza il conteggio delle schede delle colonne]**.

   ![Attiva contatore carte](assets/display-card-count.png)

   Il contatore delle schede viene visualizzato nella parte superiore di ogni colonna.

1. Fai clic su **[!UICONTROL Nascondi configurazione]** per chiudere [!UICONTROL Configura] pannello.

## Definire le impostazioni e i criteri delle colonne

1. Accedete alla bacheca.
1. Fai clic sul pulsante **[!UICONTROL Altro]** menu ![Menu Altro](assets/more-icon-spectrum.png) nella colonna e seleziona **[!UICONTROL Modifica]**.

   La [!UICONTROL Impostazioni] viene visualizzata l&#39;area. La **[!UICONTROL Nome colonna]** ti consente di sapere per quale colonna stai definendo le impostazioni.

1. Abilita la **[!UICONTROL Aggiorna automaticamente i valori dei campi]** criterio per modificare automaticamente alcuni valori di campo quando una scheda viene spostata in questa colonna.

   ![Impostazioni colonna e criteri](assets/boards-column-policies-enabled.png)

1. (Facoltativo) Imposta un valore per lo stato della scheda:

   1. Seleziona la **[!UICONTROL Stato]** casella di controllo.

   1. Seleziona lo stato da applicare a una scheda quando viene spostata in questa colonna.

      ![Stato per le colonne](assets/boards-column-status.png)

      Vengono visualizzate anche le opzioni di traduzione dello stato per le schede collegate. (La traduzione dello stato non si applica alle schede ad hoc.) Queste opzioni determinano lo stato applicato all&#39;attività o al problema in [!DNL Workfront] quando una scheda connessa viene spostata in questa colonna.

   1. Per modificare le selezioni di conversione dello stato predefinite, fai clic sul pulsante **[!UICONTROL Modifica]** icona ![Icona Modifica](assets/edit-icon-spectrum.png).
   1. Selezionare uno stato per le attività e uno stato per i problemi. Solo il valore predefinito [!DNL Workfront] gli stati sono disponibili, non quelli personalizzati.

   >[!NOTE]
   >
   >Se utilizzi stati personalizzati in [!DNL Workfront], al primo spostamento di una scheda connessa in questa colonna viene richiesto di scegliere uno stato. Ad esempio, se il progetto connesso ha più tipi di stato a cui corrispondono tutti [!UICONTROL Completato], è necessario scegliere lo stato da utilizzare in [!DNL Workfront]. Potete impostare la scelta come predefinita in modo da non dover effettuare la selezione ogni volta che spostate una scheda nella colonna.
   >Per ulteriori informazioni sugli stati, consulta [Panoramica sugli stati](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

1. (Facoltativo) Imposta un valore per gli assegnatari della scheda:

   1. Seleziona la **[!UICONTROL Assegnatari]** casella di controllo.
   1. Seleziona un&#39;azione.

      * **[!UICONTROL Aggiungi assegnatari]:** Gli assegnatari selezionati vengono aggiunti all&#39;elenco esistente di assegnatari su una scheda quando viene spostata in questa colonna.
      * **[!UICONTROL Ignora assegnatari]:** Gli assegnatari selezionati sovrascrivono tutti gli altri assegnatari e diventano gli unici assegnatari di una scheda quando viene spostata in questa colonna.
   1. Seleziona gli assegnatari dall’elenco a discesa. Solo i membri della bacheca possono scegliere tra. Per ulteriori informazioni, consulta [Aggiunta o rimozione di membri da una bacheca](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

      ![Assegnazioni per colonna](assets/boards-column-assignees.png)


1. (Facoltativo) Imposta un valore per i tag della scheda:

   1. Seleziona la **[!UICONTROL Schede]** casella di controllo.
   1. Seleziona un&#39;azione.

      * **[!UICONTROL Aggiungi tag]:** I tag selezionati vengono aggiunti all’elenco esistente di tag su una scheda quando viene spostata in questa colonna.
      * **[!UICONTROL Ignora tag]:** I tag selezionati sovrascrivono tutti gli altri tag e diventano gli unici tag presenti in una scheda quando viene spostata in questa colonna.
   1. Seleziona i tag dall’elenco a discesa. Solo i tag già creati nel [!UICONTROL Gestione tag] sono disponibili per la scelta. Per informazioni sull’aggiunta di nuovi tag, consulta [Aggiungi tag](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Tag per colonna](assets/boards-column-tags.png)


1. Abilita la **[!UICONTROL Limite lavori in corso]** criterio per limitare il numero di schede che possono essere aggiunte alla colonna. Quindi, digita il numero limite nel **[!UICONTROL Imposta limite]** campo .

   ![Limite WIP per colonna](assets/boards-wip-limit-in-column.png)

   Per ulteriori informazioni, consulta [Gestire il limite Work in Progress (WIP) su una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Fai clic su **[!UICONTROL Chiudi]** per uscire dall’area Impostazioni e visualizzare la colonna e le relative schede.
