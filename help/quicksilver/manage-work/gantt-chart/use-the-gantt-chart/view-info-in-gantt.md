---
navigation-topic: use-the-gantt-chart
title: Visualizza le informazioni nel  [!UICONTROL Diagramma di Gantt]
description: Elenco attività Diagramma di Gantt e Elenco progetti Diagramma di Gantt visualizza informazioni su progetti e attività.
author: Alina
feature: Work Management
exl-id: e6b55699-0831-40d4-a997-6fe3f8828ee1
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '930'
ht-degree: 1%

---

# Visualizza le informazioni nel  [!UICONTROL Diagramma di Gantt]

Elenco attività [!UICONTROL Diagramma di Gantt] e l&#39;elenco dei progetti [!UICONTROL Diagramma di Gantt] visualizza informazioni su progetti e attività.

## Requisiti di accesso

Devi disporre dei seguenti elementi per seguire i passaggi descritti in questo articolo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] panoramica delle licenze*</td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizzazione progetti e attività o accesso successivo</p> <p><b>NOTA</b>

Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l&#39;amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>[!UICONTROL View] o accesso successivo al progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Individua il  [!UICONTROL Diagramma di Gantt]

È possibile individuare sia l&#39;elenco delle attività Diagramma di Gantt che l&#39;elenco dei progetti [!UICONTROL Diagramma di Gantt] da più aree in Workfront. Per ulteriori informazioni, consulta [Introduzione al [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

## Visualizza le attività [!UICONTROL Percorso critico]

Nell’elenco dei progetti [!UICONTROL Diagramma di Gantt], le attività che non sono nella [!UICONTROL Percorso critico] vengono visualizzate come linee orizzontali azzurre. Attività in [!UICONTROL Percorso critico] di un progetto viene visualizzato come linee orizzontali rosse.

Per ulteriori informazioni sulle attività nel [!UICONTROL Percorso critico], vedi [Panoramica del progetto [!UICONTROL Percorso critico]](../../../manage-work/tasks/manage-tasks/critical-path.md).

## Visualizza le informazioni sull&#39;attività nell&#39;elenco dei progetti [!UICONTROL Diagramma di Gantt]

È possibile visualizzare le informazioni sull&#39;attività di un progetto direttamente dall&#39;elenco dei progetti. Le attività sono elencate con il nome di ciascun progetto.

>[!NOTE]
>
>Non è possibile modificare le attività dall’elenco dei progetti [!UICONTROL Diagramma di Gantt].

È possibile visualizzare le informazioni sull&#39;attività di un progetto direttamente da un elenco di progetti nelle aree seguenti:

* In [!UICONTROL Progetti] area
* All&#39;interno di un Portfolio
* All&#39;interno di un programma

Per visualizzare le attività di un progetto da un elenco di progetti:

1. Passare ad una delle aree sopra menzionate.

   Ad esempio, dal [!UICONTROL Menu principale], fai clic su **[!UICONTROL Progetti]**.

   Viene visualizzato un elenco di progetti.

1. Fai clic sul pulsante **[!UICONTROL Diagramma di Gantt]** icona ![](assets/gantt-icon-nwe.png) nell&#39;angolo superiore destro dello schermo.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: images conditioned for classic and nwe) <br></p>
   -->

1. Fai clic sul pulsante **[!UICONTROL Mostra elenco attività]** icona.

1. Nell’elenco dei progetti a sinistra, fai clic sulla freccia a discesa accanto al nome del progetto per visualizzare le attività del progetto.\
   Vengono visualizzate le informazioni sull&#39;attività nel  [!UICONTROL Diagramma di Gantt].\
   ![Show_task_list_enabled_project_expand.png](assets/show-task-list-enabled-project-expanded-350x78.png)

1. (Facoltativo) Fai clic sul pulsante **[!UICONTROL Stampa]** nell’angolo in alto a destra per esportare [!UICONTROL Diagramma di Gantt].

   >[!NOTE]
   >
   >Elenco progetti [!UICONTROL Diagramma di Gantt] esporta solo progetti. Informazioni attività non incluse.

## Modificare il periodo di tempo per il quale le informazioni vengono visualizzate nel [!UICONTROL Diagramma di Gantt]

È possibile regolare il periodo di tempo visualizzato nel [!UICONTROL Diagramma di Gantt] per visualizzare informazioni a livello granulare, oppure puoi passare rapidamente a una visualizzazione giorno, settimana, mese, trimestre o anno:

* [Modificare il periodo di tempo a livello granulare](#change-the-time-period-on-a-granular-level)
* [Visualizza le informazioni per giorno, settimana, mese, trimestre o anno](#view-information-by-day-week-month-quarter-or-year)

### Modificare il periodo di tempo a livello granulare {#change-the-time-period-on-a-granular-level}

1. Passa il cursore del mouse sulla timeline  [!UICONTROL Diagramma di Gantt], quindi trascinare l&#39;indicatore dello zoom da sinistra a destra per espandere o contrarre la timeline.\
   ![zoom_tool_in_gantt.png](assets/zoom-tool-in-gantt-350x180.png)

### Visualizza le informazioni per giorno, settimana, mese, trimestre o anno {#view-information-by-day-week-month-quarter-or-year}

1. In  [!UICONTROL Diagramma di Gantt], fai clic sul menu a discesa dell’intervallo di tempo .

   ![](assets/timeline-options.png)

1. Seleziona un intervallo di tempo tra le seguenti opzioni disponibili:

   * **[!UICONTROL Adatta tutto]**: Questa opzione visualizza la linea temporale dell’intero progetto.
   * **[!UICONTROL Tutti i progetti]**: Questa opzione è disponibile solo nel diagramma di Gantt Elenco progetti.
   * **[!UICONTROL Anno]**
   * **[!UICONTROL Trimestre]**
   * **[!UICONTROL Mese]**
   * **[!UICONTROL Settimana]**
   * **[!UICONTROL giorno]**

1. (Facoltativo) Seleziona un intervallo di tempo più granulare, ad esempio [!UICONTROL Settimana] o [!UICONTROL Giorno], quindi fai clic e trascina la barra di scorrimento orizzontale nella parte inferiore del  [!UICONTROL Diagramma di Gantt] per spostarsi da sinistra a destra nella linea temporale del progetto.\
   Un’istantanea della timeline [!UICONTROL Gantt] viene visualizzato per mostrare l’intero progetto.

   >[!TIP]
   >
   >Lo snapshot della timeline viene visualizzato solo dopo aver fatto clic sulla barra di scorrimento orizzontale.

   ![stretchy_gantt_minimap_with_struttura_1_.png](assets/stretchy-gantt-minimap-with-outline--1--350x140.png)

1. (Facoltativo) Fai clic in un punto qualsiasi all’interno dell’istantanea della linea temporale per passare a un punto specifico della durata del progetto.\
   Oppure\
   Trascina le maniglie del visualizzatore snapshot per selezionare un intervallo di linee temporali specifico da visualizzare nella [!UICONTROL Gantt].

## Utilizzare filtri, visualizzazioni e raggruppamenti

La [!UICONTROL Diagramma di Gantt] è una rappresentazione visiva delle informazioni attualmente visualizzate nell’elenco delle attività. È possibile applicare filtri, viste e raggruppamenti agli oggetti elencati in entrambi [!UICONTROL Diagramma di Gantt]s.

>[!CAUTION]
>
>Non è possibile applicare filtri, viste e raggruppamenti quando si seleziona [!UICONTROL Manuale] save [!UICONTROL Pianificazione temporale] per salvare le modifiche all&#39;elenco delle attività. Per informazioni sul salvataggio delle modifiche apportate alle attività in un elenco, vedere [Modificare le attività in un elenco](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

I filtri e i raggruppamenti applicati all’elenco si riflettono sia nell’elenco dei progetti che nell’elenco delle attività  [!UICONTROL Diagramma di Gantt]e sono inclusi anche quando vengono esportati i diagrammi di Gantt:

* Filtri\
   È possibile applicare un filtro all’elenco per controllare le informazioni visualizzate nella [!UICONTROL Diagramma di Gantt].\
   Per informazioni sull’applicazione di un filtro, consulta  [Panoramica dei filtri in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Raggruppamenti\
   I raggruppamenti applicati all’elenco si riflettono sul [!UICONTROL Diagramma di Gantt].\
   Per informazioni sull’applicazione di un raggruppamento, consulta  [Panoramica sui raggruppamenti in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

Le visualizzazioni non vengono riportate sulla [!UICONTROL Diagramma di Gantt]. Tuttavia, quando esporti il [!UICONTROL Diagramma di Gantt] (come descritto in  [Esporta il [!UICONTROL Diagramma di Gantt] a PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)), l’elenco delle attività viene esportato in aggiunta al [!UICONTROL Diagramma di Gantt], con la visualizzazione corrente applicata all’elenco.

## Configurare le opzioni di visualizzazione

È possibile scegliere il tipo di informazioni da visualizzare in entrambi [!UICONTROL Diagramma di Gantt]. Per ulteriori informazioni, consulta [Configurare la modalità di visualizzazione delle informazioni nel [!UICONTROL Diagramma di Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).
