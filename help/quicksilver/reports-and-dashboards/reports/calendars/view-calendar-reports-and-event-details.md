---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Visualizzare i report del calendario e i dettagli degli eventi
description: Puoi visualizzare i rapporti del calendario e i dettagli dell’evento che hai creato o che sono stati condivisi con te in Adobe Workfront.
author: Lisa
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Visualizzare i report del calendario e i dettagli dell’evento

Puoi visualizzare i rapporti del calendario e i dettagli dell’evento che hai creato o che sono stati condivisi con te in Adobe Workfront.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Collaboratore</p>
       <p>Richiesta</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso a report, dashboard e calendari in visualizzazione o superiore</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td>Visualizza o autorizzazioni superiori per il report calendario</td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare un report calendario

<!--{{step1-to-calendars}}-->

1. Fai clic sull&#39;icona **[!UICONTROL Menu principale]** ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Menu principale]** ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su **[!UICONTROL Calendari]**.

   A seconda del livello di accesso, è possibile che vengano elencati i calendari seguenti:

   * Calendario [!DNL Adobe Workfront] predefinito

     Workfront crea un calendario per l&#39;utente in base ai progetti, alle attività e ai problemi assegnati all&#39;utente o ai team, ai gruppi o ai ruoli a cui l&#39;utente è assegnato.

   * Calendari creati

     Per informazioni sulla creazione di calendari, vedere [Panoramica sui report calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

   * Calendari condivisi con altri utenti

     Per informazioni sulla condivisione dei calendari, vedere [[!UICONTROL Condividere un calendario] report](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

1. (Condizionale) Fai clic sull&#39;elenco a discesa **[!UICONTROL Visualizza]**, quindi seleziona la durata del calendario da visualizzare.
   ![Durata calendario](assets/view-menu-calendar-report-350x189.png)
È possibile scegliere tra le seguenti visualizzazioni di report calendario:

   * **[!UICONTROL Mese]**: visualizza quattro settimane del calendario
   * **[!UICONTROL Settimana]**: visualizza una settimana del calendario
   * **[!UICONTROL Gantt]**: visualizza una visualizzazione continua del calendario

     Puoi visualizzare altri eventi in una visualizzazione **Gantt** scorrendo verso il basso o lateralmente. Un simbolo di caricamento viene visualizzato quando i dati vengono compilati per la vista.

   >[!NOTE]
   >
   >Nelle visualizzazioni **Mese** e **Settimana**, gli eventi correnti o futuri (compresi gli eventi che si estendono su più giorni, purché contengano oggi o un giorno futuro) presentano uno sfondo che corrisponde al colore nel progetto o nel raggruppamento del calendario. Gli eventi passati presentano un&#39;ombreggiatura più chiara per indicare che non sono più correnti, ma è comunque possibile selezionarli e visualizzarli.

1. (Facoltativo) Se visualizzi il calendario nelle visualizzazioni **Mese** o **Settimana**, puoi modificare la visualizzazione del calendario con le seguenti opzioni:

   <!--   * To include or exclude weekends:
      1. On the **[!UICONTROL Calendar]** toolbar, click **[!UICONTROL Calendar Actions]**, then from the drop-down list select either **[!UICONTROL Show Weekend]** or **[!UICONTROL Hide Weekend]**.-->

   * Per modificare rapidamente le date visualizzate:

      1. Sulla barra degli strumenti **[!UICONTROL Calendario]** fare clic sulla freccia sinistra dell&#39;indicatore di data per tornare al calendario o sulla freccia destra per spostarsi in avanti.

         ![Fare clic sulla freccia per modificare la data](assets/click-arrows-to-change-dates-calendar-report.png)

         Le date visualizzate vengono regolate in base a un intervallo basato sulla visualizzazione del calendario corrente. Ad esempio, se visualizzi il calendario nella visualizzazione **Settimana**, il calendario visualizza una settimana avanti o una settimana indietro, a seconda della freccia selezionata.

      1. (Facoltativo) Per tornare al giorno corrente, fare clic su [!UICONTROL **Oggi**].

1. (Facoltativo) Per nascondere gli eventi di un progetto o di un raggruppamento del calendario collegato al calendario, deselezionare il raggruppamento del progetto o del calendario nell&#39;elenco dei progetti.
   ![Nascondi eventi](assets/hide-events-for-project-or-cal-grouping.png)
È possibile rendere nuovamente visibili gli eventi selezionando il [!UICONTROL progetto] o il raggruppamento del calendario nell&#39;elenco dei progetti.

## Visualizza dettagli evento report calendario

Puoi visualizzare i dettagli di un evento in un calendario, sia per gli eventi correnti che per quelli passati.

1. Vai all’evento per il quale desideri conoscere i dettagli, quindi fai clic sull’evento. I dettagli vengono visualizzati in un pannello sul lato destro.
1. (Facoltativo) Per aprire il progetto, l’attività o il problema associato, fai clic sul titolo dell’oggetto.
