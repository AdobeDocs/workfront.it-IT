---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Creare un’iterazione in un flusso di lavoro
description: Un'iterazione è una quantità di tempo riservata per il completamento del lavoro. Alcuni team agili possono fare riferimento a un’iterazione come sprint.
author: Jenny
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Creare un’iterazione in un flusso di lavoro

>[!IMPORTANT]
>
>I flussi di lavoro sono disponibili solo per un gruppo specifico di clienti.

Un&#39;iterazione è una quantità di tempo riservata per il completamento del lavoro. Alcuni team agili possono fare riferimento a un’iterazione come sprint.

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

## Creare un’iterazione in un flusso di lavoro

{{step1-to-boards}}

1. Aprire il flusso di lavoro in cui si desidera aggiungere l&#39;iterazione. Per aprire un flusso di lavoro, fare clic su [!UICONTROL **Visualizza flusso di lavoro**].
1. Creare un&#39;iterazione utilizzando uno dei seguenti metodi:

   * Nella visualizzazione iterazione della scheda Elenco schede fare clic su [!UICONTROL **Crea iterazione**].
   * Nella visualizzazione elenco della scheda Elenco schede fare clic su [!UICONTROL **Crea iterazione**].
   * Nella scheda Bacheche, fai clic su [!UICONTROL **Aggiungi bacheca**] e seleziona [!UICONTROL **Processo iterazione**] come modello della bacheca. Quindi, aprire la bacheca di iterazione e fare clic su [!UICONTROL **Configura iterazioni**].

1. Nella finestra di dialogo Dettagli iterazione, aggiungi le seguenti informazioni:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Nome iterazione]</strong></td> 
      <td>Nome dell'iterazione, ad esempio "Sprint 1".</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Lunghezza iterazione]</strong></td> 
      <td>Durata dell'iterazione, in giorni, settimane o mesi.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Data di inizio]</strong></td> 
      <td>Data di inizio dell'iterazione. La data di fine viene immessa automaticamente in base alla lunghezza dell'iterazione.</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su [!UICONTROL **Salva**].

   L&#39;iterazione viene ora visualizzata nella vista iterazione dell&#39;elenco delle schede e nell&#39;area delle metriche sulla bacheca iterazione.

   Per aggiungere schede a un&#39;iterazione, vedere [Utilizzare l&#39;elenco delle schede](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

## Modificare un’iterazione esistente

1. Per aprire un flusso di lavoro, fare clic su [!UICONTROL **Visualizza flusso di lavoro**].
1. Aprire l&#39;iterazione utilizzando uno dei seguenti metodi:

   * Nella vista iterazione della scheda Elenco schede fare clic sull&#39;icona [!UICONTROL **Dettagli iterazione**] ![Dettagli iterazione](assets/iteration-details-button.png).
   * Nella bacheca iterazione fare clic sull&#39;icona [!UICONTROL **Dettagli iterazione**] ![Dettagli iterazione](assets/iteration-details-button.png) nell&#39;area delle metriche in alto a destra.

1. Nel pannello [!UICONTROL Configurazione iterazione], modifica l&#39;iterazione in base alle esigenze.
1. Per modificare il nome dell&#39;iterazione, espandere [!UICONTROL **Dettagli iterazione**].

   Una volta avviata un&#39;iterazione, è possibile modificarne solo il nome e non le date o la lunghezza.

<!--   

1. <span class="preview">To add goals to the iteration, expand [!UICONTROL **Goals**].</span>
1. <span class="preview">Click [!UICONTROL **Add goal**], and type the goal name.</span>

   <span class="preview">As goals are completed during the iteration, you can select the check box to mark them complete, or click the **Delete** icon ![Delete icon](assets/delete.png) to delete a goal. The metrics area on the top right of the iteration shows how many goals exist and how many have been completed.</span>

<div class="preview">

## Assign cards to the next iteration

Use the [!UICONTROL Next Iteration] column to move cards from the current iteration to the next iteration, without sending them to the backlog first.

1. Move a card to the [!UICONTROL **Next Iteration**] column, or add a new card directly in the column.
1. Access the next iteration by clicking the [!UICONTROL **Next Iteration**] column title, or by clicking the up-pointing arrow next to the iteration name on the top of the screen.

   The cards that you marked to come over to the next iteration are placed in the columns that correspond with their status.

</div>
-->

## Eliminare un’iterazione

1. Fare clic sulla scheda [!UICONTROL **Elenco schede**] nel flusso di lavoro e aprire la visualizzazione iterazione.
1. Fai clic sull&#39;icona **Elimina** ![Elimina](assets/delete.png) accanto all&#39;iterazione.
1. Fare clic su [!UICONTROL **Elimina iterazione**] nel messaggio di conferma.
