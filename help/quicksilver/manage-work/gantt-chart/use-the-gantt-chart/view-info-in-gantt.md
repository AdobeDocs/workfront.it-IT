---
navigation-topic: use-the-gantt-chart
title: Visualizza informazioni nel [!UICONTROL Diagramma di Gantt]
description: Nell'elenco delle attività Diagramma di Gantt e nell'elenco dei progetti Diagramma di Gantt vengono visualizzate informazioni sui progetti e sulle attività.
author: Alina
feature: Work Management
exl-id: e6b55699-0831-40d4-a997-6fe3f8828ee1
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 0%

---

# Visualizza informazioni nel [!UICONTROL Diagramma di Gantt]

Nell&#39;elenco delle attività [!UICONTROL Grafico di Gantt] e nell&#39;elenco dei progetti [!UICONTROL Grafico di Gantt] vengono visualizzate informazioni sui progetti e sulle attività.

## Requisiti di accesso

Per seguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] panoramica sulle licenze*</td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso di [!UICONTROL View] o versione successiva a progetti e attività</p> <p><b>NOTA</b>

Se non disponi ancora dell&#39;accesso, chiedi all&#39;amministratore [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di [!UICONTROL View] o versione successiva al progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore [!DNL Workfront].

## Individua il [!UICONTROL Diagramma di Gantt]

È possibile individuare il diagramma di Gantt dell&#39;elenco attività e l&#39;elenco dei progetti [!UICONTROL Grafico di Gantt] da più aree in Workfront. Per ulteriori informazioni, vedere [Introduzione al [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

## Visualizza le attività nel [!UICONTROL percorso critico]

Nell&#39;elenco dei progetti [!UICONTROL Grafico di Gantt], le attività che non si trovano nel [!UICONTROL Percorso critico] vengono visualizzate come linee orizzontali azzurre. Le attività che si trovano nel [!UICONTROL Percorso critico] di un progetto vengono visualizzate come linee rosse orizzontali.

Per ulteriori informazioni sulle attività nel [!UICONTROL Percorso critico], vedere [Panoramica del progetto [!UICONTROL Percorso critico]](../../../manage-work/tasks/manage-tasks/critical-path.md).

## Visualizza le informazioni sull&#39;attività nell&#39;elenco dei progetti [!UICONTROL Diagramma di Gantt]

È possibile visualizzare le informazioni sulle attività di un progetto direttamente dall&#39;elenco dei progetti. Le attività sono elencate sotto il nome di ciascun progetto.

>[!NOTE]
>
>Impossibile modificare le attività dall&#39;elenco dei progetti [!UICONTROL Grafico di Gantt].

È possibile visualizzare le informazioni sulle attività di un progetto direttamente da un elenco di progetti nelle aree seguenti:

* Nell&#39;area [!UICONTROL Progetti]
* Entro un Portfolio
* All’interno di un programma

Per visualizzare le attività di un progetto da un elenco di progetti:

1. Passare a una delle aree sopra indicate.

   Ad esempio, dal [!UICONTROL menu principale], fare clic su **[!UICONTROL Progetti]**.

   Viene visualizzato un elenco di progetti.

1. Fai clic sull&#39;icona ![](assets/gantt-icon-nwe.png) del **[!UICONTROL Grafico di Gantt]** nell&#39;angolo superiore destro dello schermo.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: images conditioned for classic and nwe) <br></p>
   -->

1. Fare clic sull&#39;icona **[!UICONTROL Mostra elenco attività]**.

1. Nell&#39;elenco a sinistra del progetto fare clic sulla freccia a discesa accanto al nome del progetto per visualizzare tutte le attività del progetto.\
   Visualizza informazioni sull&#39;attività nel [!UICONTROL Diagramma di Gantt].\
   ![Mostra_elenco_attività_abilitato_progetto_espanso.png](assets/show-task-list-enabled-project-expanded-350x78.png)

1. (Facoltativo) Fai clic sull&#39;icona **[!UICONTROL Stampa]** nell&#39;angolo superiore destro per esportare il [!UICONTROL Diagramma di Gantt].

   >[!NOTE]
   >
   >L&#39;elenco dei progetti [!UICONTROL Grafico di Gantt] esporta solo progetti. Le informazioni sull&#39;attività non sono incluse.

## Modifica il periodo di tempo per il quale vengono visualizzate le informazioni nel [!UICONTROL Diagramma di Gantt]

È possibile modificare il periodo di tempo visualizzato nel [!UICONTROL Diagramma di Gantt] per visualizzare le informazioni a livello granulare oppure passare rapidamente a una visualizzazione giorno, settimana, mese, trimestre o anno:

* [Modificare il periodo di tempo a livello granulare](#change-the-time-period-on-a-granular-level)
* [Visualizza informazioni per giorno, settimana, mese, trimestre o anno](#view-information-by-day-week-month-quarter-or-year)

### Modificare il periodo di tempo a livello granulare {#change-the-time-period-on-a-granular-level}

1. Passa il puntatore del mouse sulla sequenza temporale del [!UICONTROL Diagramma di Gantt], quindi trascina l&#39;indicatore di zoom da sinistra a destra per espandere o comprimere la sequenza temporale.\
   ![zoom_tool_in_gantt.png](assets/zoom-tool-in-gantt-350x180.png)

### Visualizza informazioni per giorno, settimana, mese, trimestre o anno {#view-information-by-day-week-month-quarter-or-year}

1. Nel [!UICONTROL Diagramma di Gantt], fare clic sul menu a discesa dell&#39;intervallo di tempo.

   ![](assets/timeline-options.png)

1. Seleziona un intervallo di tempo tra le seguenti opzioni disponibili:

   * **[!UICONTROL Adatta tutto]**: questa opzione visualizza la linea temporale dell&#39;intero progetto.
   * **[!UICONTROL Tutti i progetti]**: questa opzione è disponibile solo nel diagramma di Gantt dell&#39;elenco dei progetti.
   * **[!UICONTROL Anno]**
   * **[!UICONTROL Trimestre]**
   * **[!UICONTROL Mese]**
   * **[!UICONTROL Settimana]**
   * **[!UICONTROL Giorno]**

1. (Facoltativo) Seleziona un intervallo di tempo più granulare, ad esempio [!UICONTROL Settimana] o [!UICONTROL Giorno], quindi fai clic e trascina la barra di scorrimento orizzontale nella parte inferiore del [!UICONTROL Grafico di Gantt] per spostarti da sinistra a destra nella linea temporale del progetto.\
   Viene visualizzato uno snapshot della timeline del [!UICONTROL Gantt] per mostrare l&#39;intero progetto.

   >[!TIP]
   >
   >Lo snapshot della timeline viene visualizzato solo dopo aver fatto clic sulla barra di scorrimento orizzontale.

   ![stretchy_gantt_minimap_with_outline__1_.png](assets/stretchy-gantt-minimap-with-outline--1--350x140.png)

1. (Facoltativo) Fai clic in un punto qualsiasi all’interno dello snapshot della linea temporale per passare a un punto specifico della durata del progetto.\
   Oppure\
   Trascina gli handle del visualizzatore di snapshot per selezionare un intervallo di righe temporali specifico per visualizzarlo nel [!UICONTROL Gantt] principale.

## Utilizzare filtri, viste e raggruppamenti

Il [!UICONTROL Diagramma di Gantt] è una rappresentazione visiva delle informazioni attualmente visualizzate nell&#39;elenco delle attività. Puoi applicare filtri, viste e raggruppamenti agli oggetti elencati in entrambi i [!UICONTROL Grafici di Gantt].

>[!CAUTION]
>
>Non puoi applicare filtri, viste e raggruppamenti quando selezioni [!UICONTROL Manuale] salva [!UICONTROL Pianificazione sequenza temporale] per salvare le modifiche all&#39;elenco attività. Per informazioni sul salvataggio delle modifiche apportate alle attività in un elenco, vedere [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

I filtri e i raggruppamenti applicati all&#39;elenco si riflettono sia sull&#39;elenco dei progetti che sull&#39;elenco delle attività [!UICONTROL Grafici di Gantt] e sono inclusi anche quando i grafici di Gantt vengono esportati:

* Filtri\
   È possibile applicare un filtro all&#39;elenco per controllare le informazioni visualizzate nel [!UICONTROL Grafico di Gantt].\
   Per informazioni sull&#39;applicazione di un filtro, vedere [Panoramica dei filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Raggruppamenti\
   I raggruppamenti applicati all&#39;elenco si riflettono nel [!UICONTROL Diagramma di Gantt].\
   Per informazioni sull&#39;applicazione di un raggruppamento, vedere [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

Le visualizzazioni non si riflettono nel [!UICONTROL Diagramma di Gantt]. Tuttavia, quando si esporta il [!UICONTROL Diagramma di Gantt] (come descritto in [Esportare il [!UICONTROL Diagramma di Gantt] in PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)), l&#39;elenco delle attività viene esportato in aggiunta al [!UICONTROL Diagramma di Gantt], con la visualizzazione corrente applicata all&#39;elenco.

## Configura opzioni di visualizzazione

È possibile scegliere il tipo di informazioni da visualizzare in entrambi i [!UICONTROL grafici Gantt]. Per ulteriori informazioni, vedere [Configurare la visualizzazione delle informazioni nel [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).
