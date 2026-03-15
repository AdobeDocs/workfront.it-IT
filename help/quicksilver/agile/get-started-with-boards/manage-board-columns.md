---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Gestisci colonne bacheca
description: A new board contains three columns by default. You can add more columns, change the order of the columns, rename columns, and delete any columns that you don't need. You can also define column policies.
author: Courtney
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '1081'
ht-degree: 4%

---

# Gestire le colonne di una bacheca

<!-- Audited: 05/2024 -->

A new board contains three columns by default. È possibile aggiungere altre colonne, modificare l&#39;ordine delle colonne, rinominare le colonne ed eliminare le colonne non necessarie.

Le impostazioni delle colonne includono i criteri, che consentono di definire le opzioni per ciò che accade a una scheda quando viene spostata in quella colonna.

Per informazioni sull&#39;ordinamento delle schede in colonne, vedere [Filtrare e cercare in una bacheca](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o successiva</p> 
   <p>Richiedente o successiva</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Add a column to a board

{{step1-to-boards}}

1. Accedi a una bacheca. Per informazioni, consulta [Creare o modificare una bacheca](../../agile/get-started-with-boards/create-edit-board.md).
1. Fai clic su **[!UICONTROL Aggiungi colonna]** a destra delle colonne esistenti.
1. Nella nuova colonna digitare un nome e fare clic su **[!UICONTROL Aggiungi colonna]**.

   ![Aggiungi nuova colonna](assets/boards-add-column.png)

>[!TIP]
>
>Per aggiungere una colonna acquisizione, vedere [Aggiungere una colonna acquisizione a una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Riordinare le colonne su una bacheca

1. Accedi alla bacheca.
1. Drag and drop the columns into the correct order. Be sure to select the top of the column before dragging it to another location.

   ![Drag and drop column](assets/boards-dragdropcolumn.png)

## Rinominare una colonna della bacheca

1. Accedi alla bacheca.
1. Fare clic sul nome della colonna, digitare il nuovo nome e premere Invio.

   Oppure

   Fai clic sul menu **[!UICONTROL Altro]** ![Altro menu](assets/more-icon-spectrum.png) nella colonna e seleziona **[!UICONTROL Modifica]**. Nell&#39;area Impostazioni digitare il nuovo nome nel campo **[!UICONTROL Nome colonna]** e fare clic su **[!UICONTROL Chiudi]**.

## Eliminare una colonna della bacheca

Quando elimini una colonna da una bacheca, non può essere recuperata.

1. Accedi alla bacheca.
1. Fai clic sul menu **[!UICONTROL Altro]** ![Altro menu](assets/more-icon-spectrum.png) nella colonna e seleziona **[!UICONTROL Elimina]**.

   >[!NOTE]
   >
   >Impossibile eliminare le colonne che contengono schede, incluse le schede archiviate. Se tenti di eliminare una colonna che contiene schede, devi scegliere un’altra colonna per tali schede.

## Display card count

Puoi utilizzare un’impostazione di configurazione per visualizzare il numero di schede in ogni colonna.

Se si utilizza il limite WIP in una colonna, non viene aggiunto un contatore di schede separato. Per ulteriori informazioni sui limiti WIP, vedere [Gestione del limite [!UICONTROL Work in Progress] (WIP) in una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Accedi alla bacheca.
1. Fai clic su **[!UICONTROL Configura]** a destra della bacheca per aprire il pannello Configura.
1. Espandi **[!UICONTROL Colonna]**.
1. Turn on **[!UICONTROL Display a column card count]**.

   ![Turn on card counter](assets/display-card-count.png)

   The card counter appears at the top of each column.

1. Fare clic su **[!UICONTROL Nascondi configurazione]** per chiudere il pannello [!UICONTROL Configura].

## Define column settings and policies

I criteri colonna includono l&#39;aggiornamento automatico dei valori dei campi e l&#39;impostazione di un limite work in progress.

Il criterio per l’aggiornamento dello stato funziona automaticamente sia per la scheda che per la colonna:

* Quando una scheda viene spostata in una colonna con una policy, lo stato della scheda viene aggiornato allo stato definito nella policy. Questo vale sia per le schede ad hoc che per quelle connesse.
* Quando lo stato di una scheda ad hoc o connessa viene aggiornato sulla scheda in modo che corrisponda allo stato della colonna nel criterio o lo stato di una scheda connessa viene aggiornato in un’altra posizione in Workfront, la scheda viene automaticamente spostata in tale colonna. Inoltre, se uno stato personalizzato di una scheda corrisponde allo stato di sistema assegnato alla colonna, la scheda viene spostata in tale colonna.

Una scheda rimarrà in una colonna in cui viene posizionata se lo stato della scheda non corrisponde a nessuno stato impostato nei criteri di colonna esistenti.

1. Accedi alla bacheca.
1. Fai clic sul menu **[!UICONTROL Altro]** ![Altro menu](assets/more-icon-spectrum.png) nella colonna e seleziona **[!UICONTROL Modifica]**.

   Verrà visualizzata l&#39;area [!UICONTROL Impostazioni]. Il **[!UICONTROL Nome colonna]** consente di sapere per quale colonna si stanno definendo le impostazioni.

1. Abilita il criterio **[!UICONTROL Aggiorna automaticamente i valori dei campi]** per modificare automaticamente alcuni valori dei campi quando una scheda viene spostata in questa colonna.

   ![Impostazioni e criteri colonna](assets/boards-column-policies-enabled.png)

1. (Optional) Set a value for the card status:

   1. Select the **[!UICONTROL Status]** check box.

   1. Select the status to apply to a card when it is moved to this column.

      ![Status for columns](assets/boards-column-status.png)

      The status translation options for connected cards are also displayed. La traduzione dello stato non si applica alle schede ad hoc. Queste opzioni determinano lo stato personalizzato applicato all&#39;attività o al problema in [!DNL Workfront] quando una scheda connessa viene spostata in questa colonna.

   1. Seleziona uno stato [!UICONTROL **Personalizzato**] da applicare alla scheda per le attività e per i problemi.

      Quando una scheda viene spostata in questa colonna, [!DNL Workfront] tenta prima di applicare lo stato personalizzato (ad esempio, Risolto). Se lo stato personalizzato selezionato non è disponibile per tale scheda, viene richiesto di scegliere un altro stato che corrisponda allo stato del sistema (dal passaggio b sopra). Per ulteriori informazioni sugli stati, vedere [Panoramica sugli stati](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      Inoltre, se lo stato dell’attività o del problema connesso viene modificato nello stato personalizzato o di sistema impostato nella policy di colonna, la scheda viene automaticamente spostata nella colonna.

1. (Facoltativo) Imposta un valore per gli assegnatari della carta:

   1. Selezionare la casella di controllo **[!UICONTROL Assegnatari]**.
   1. Seleziona un’azione.

      * **[!UICONTROL Aggiungi assegnatari]:** Gli assegnatari selezionati vengono aggiunti all&#39;elenco esistente di assegnatari su una scheda quando questa viene spostata in questa colonna.
      * **[!UICONTROL Sostituisci assegnatari]:** Gli assegnatari selezionati sovrascrivono tutti gli altri assegnatari e diventano gli unici assegnatari su una scheda quando viene spostata in questa colonna.

   1. Fai clic su [!UICONTROL **Aggiungi assegnazione**] e cerca un utente. Selezionare gli assegnatari dai risultati della ricerca. Tutti gli utenti e i team di Workfront sono disponibili tra cui scegliere.

      ![Assegnatari per colonna](assets/boards-column-assignees.png)

1. (Facoltativo) Imposta un valore per i tag della scheda:

   1. Selezionare la casella di controllo **[!UICONTROL Schede]**.
   1. Seleziona un’azione.

      * **[!UICONTROL Aggiungi su tag]:** I tag selezionati vengono aggiunti all&#39;elenco esistente di tag su una scheda quando viene spostata in questa colonna.
      * **[!UICONTROL Ignora tag]:** I tag selezionati sovrascrivono tutti gli altri tag e diventano gli unici tag di una scheda quando viene spostata in questa colonna.

   1. Seleziona i tag dall’elenco a discesa. Only tags already created in the [!UICONTROL Tag Manager] are available to choose from. For information on adding new tags, see [Add tags](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Tags for column](assets/boards-column-tags.png)

1. Enable the **[!UICONTROL Work in progress limit]** policy to limit the number of cards that can be added to the column. Then, type the limit number in the **[!UICONTROL Set limit]** field.

   ![Limite WIP per colonna](assets/boards-wip-limit-in-column.png)

   Per ulteriori informazioni, vedere [Gestire il limite WIP in una bacheca](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Fai clic su **[!UICONTROL Chiudi]** per uscire dall&#39;area Impostazioni e visualizzare la colonna e le relative schede.
