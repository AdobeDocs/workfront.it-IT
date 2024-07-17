---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Visualizzare i report del calendario e i dettagli dell’evento
description: Puoi visualizzare i rapporti del calendario e i dettagli dell’evento che hai creato o che sono stati condivisi con te in Adobe Workfront.
author: Lisa
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# Visualizzare i report del calendario e i dettagli dell’evento

Puoi visualizzare i rapporti del calendario e i dettagli dell’evento che hai creato o che sono stati condivisi con te in Adobe Workfront.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Request] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso*</strong></td> 
   <td> <p>Accesso di [!UICONTROL View] o versione successiva a [!UICONTROL Reports], [!UICONTROL Dashboards] e [!UICONTROL Calendars]</p> <p>Nota: se non disponi ancora dell'accesso, chiedi all'amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Autorizzazioni di [!UICONTROL View] o superiori per il report del calendario</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## Visualizzare un report calendario

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Calendari]**.

   A seconda del livello di accesso, è possibile che vengano elencati i calendari seguenti:

   * Calendario [!DNL Adobe Workfront] predefinito\

     Workfront crea un calendario per l&#39;utente in base ai progetti, alle attività e ai problemi assegnati all&#39;utente o ai team, ai gruppi o ai ruoli a cui l&#39;utente è assegnato.
   * Calendari creati\

     Per informazioni sulla creazione di calendari, vedere [Panoramica sui report calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

   * Calendari condivisi con altri utenti\

     Per informazioni sulla condivisione dei calendari, vedere [[!UICONTROL Condividere un calendario] report](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

1. (Condizionale) Fai clic sull&#39;elenco a discesa **[!UICONTROL Visualizza]**, quindi seleziona la durata del calendario da visualizzare.\
   ![Durata calendario](assets/view-menu-calendar-report-350x189.png)\
   È possibile scegliere tra le seguenti visualizzazioni di report calendario:

   * **[!UICONTROL Mese]**: visualizza quattro settimane del calendario
   * **[!UICONTROL Settimana]**: visualizza una settimana del calendario
   * **[!UICONTROL Gantt]**: visualizza una visualizzazione continua del calendario\

     ![[!UICONTROL Rapporto calendario Gantt]](assets/gantt-calendar-report.png)
Puoi visualizzare altri eventi in una visualizzazione [!UICONTROL Gantt] scorrendo verso il basso o lateralmente. Un simbolo di caricamento viene visualizzato quando i dati vengono compilati per la vista.
   >[!NOTE]
   >
   >Nelle visualizzazioni [!UICONTROL Mese] e [!UICONTROL Settimana], gli eventi correnti o futuri (compresi gli eventi che si estendono su più giorni, purché contengano oggi o un giorno futuro) presentano uno sfondo che corrisponde al colore nel progetto o nel raggruppamento del calendario. Gli eventi passati presentano un&#39;ombreggiatura più chiara per indicare che non sono più correnti, ma è comunque possibile selezionarli e visualizzarli.

1. (Facoltativo) Se visualizzi il calendario nelle visualizzazioni [!UICONTROL Mese] o [!UICONTROL Settimana], puoi modificare la visualizzazione del calendario con le seguenti opzioni:

   * Per includere o escludere i fine settimana:

      1. Sulla barra degli strumenti **[!UICONTROL Calendario]**, fai clic su **[!UICONTROL Azioni calendario]**, quindi seleziona **[!UICONTROL Mostra fine settimana]** o **[!UICONTROL Nascondi fine settimana]** dall&#39;elenco a discesa.
   * Per modificare rapidamente le date visualizzate:

      1. Sulla barra degli strumenti **[!UICONTROL Calendario]** fare clic sulla freccia sinistra dell&#39;indicatore di data per tornare al calendario o sulla freccia destra per spostarsi in avanti.\

         ![Fare clic sulla freccia per modificare la data](assets/click-arrows-to-change-dates-calendar-report.png)\
         Le date visualizzate vengono regolate in base a un intervallo basato sulla visualizzazione del calendario corrente. Ad esempio, se visualizzi il calendario nella visualizzazione [!UICONTROL Settimana], il calendario visualizza una settimana avanti o una settimana indietro, a seconda della freccia selezionata.

      1. (Facoltativo) Per tornare al giorno corrente, fai clic su **Today**.


1. (Facoltativo) Per visualizzare un calendario a schermo intero, fare clic sulle frecce a schermo intero sul lato destro della barra degli strumenti **[!UICONTROL Calendario]**.
   ![Fare clic sulla freccia per modificare la data](assets/click-arrows-to-change-dates-calendar-report.png)\
   Premere ESC per tornare alla visualizzazione normale del calendario.

1. (Facoltativo) Per nascondere gli eventi di un progetto o di un raggruppamento del calendario collegato al calendario, deselezionare il raggruppamento del progetto o del calendario nell&#39;elenco dei progetti.
   ![Nascondi eventi](assets/hide-events-for-project-or-cal-grouping.png)\
   È possibile rendere nuovamente visibili gli eventi selezionando il [!UICONTROL progetto] o il raggruppamento del calendario nell&#39;elenco dei progetti.

## Visualizza dettagli evento report calendario

Puoi visualizzare i dettagli di un evento in un calendario, sia per gli eventi correnti che per quelli passati.

1. Vai all’evento per il quale desideri conoscere i dettagli, quindi fai clic sull’evento.\
   Viene visualizzata una pagina di dettagli per l’evento.\
   ![calendar_report_EventDetails.png](assets/calendar-report-eventdetails-350x145.png)

1. (Facoltativo) Per visualizzare ulteriori dettagli sull&#39;oggetto:

   1. Passa il puntatore del mouse sul nome del progetto, dell’attività o del problema.

      Viene visualizzata una pagina dei dettagli dell&#39;oggetto.\
      ![additional_object_details_-_calendar_report.png](assets/additional-object-details---calendar-report-350x131.png)

   1. (Facoltativo) Per aprire il progetto, l’attività o il problema associato, fai clic sul titolo dell’oggetto.
   1. (Facoltativo) Per chiudere tutte le pagine dei dettagli aperte, fai clic in un punto qualsiasi al di fuori delle pagine dei dettagli dell’evento.
