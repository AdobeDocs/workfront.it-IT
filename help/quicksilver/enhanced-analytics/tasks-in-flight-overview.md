---
title: Visualizzazione delle attività nella visualizzazione dei voli in Enhanced analytics
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualizzazione Attività in volo mostra il numero di attività (all’interno dei criteri di filtro applicati) in corso per un progetto, la percentuale di lavoro completato per ogni attività e il livello di pianificazione delle attività.
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---

# Visualizzazione delle attività nella visualizzazione dei voli in Enhanced analytics

La visualizzazione Attività in volo mostra il numero di attività (all’interno dei criteri di filtro applicati) in corso per un progetto, la percentuale di lavoro completato per ogni attività e il livello di pianificazione delle attività.

![](assets/tasks-in-flight-possible-replacement-350x104.png)

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">piano Adobe Workfront</a>*</td> 
   <td> <p>Aziende o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica sulle licenze di Adobe Workfront</a>*</td> 
   <td> <p>Revisione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizza accesso a progetti</p> <p>Visualizza l'accesso alle attività (per aggiornare le attività, è necessario modificare l'accesso alle attività).</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso.<br>Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza l'autorizzazione sia per gli oggetti progetto che per gli oggetti attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Per i prerequisiti per l’utilizzo di Analytics avanzato, consulta la sezione &quot;Prerequisiti&quot; in [Panoramica dell’analisi migliorata](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprendere le attività nella visualizzazione dei voli

La visualizzazione Attività nel piano di volo mostra i seguenti dettagli dell’attività:

* **Durata prevista attività**: La lunghezza di una barra delle attività indica la durata pianificata, in base alla data di inizio e alla data di completamento dell&#39;attività.

   ![](assets/tasks-in-flight-duration-350x80.png)

* **Sforzo di lavoro completato**: Il colore blu scuro all’interno di una barra delle attività indica la quantità di lavoro completato per un’attività. Questa percentuale di completamento viene visualizzata a destra della barra delle attività.

   ![](assets/tasks-in-flight-dark-blue-350x35.png)

* **Sforzo di lavoro rimanente**: Il colore blu chiaro all’interno di una barra delle attività indica la quantità di lavoro da completare per un’attività.

   ![](assets/tasks-in-flight-light-blue-350x35.png)

Queste informazioni possono essere utili per determinare:

* Dove lo sforzo di lavoro è stato concentrato.
* Quali compiti potrebbero mettere a rischio un progetto?
* Quanto è vicino il completamento di un&#39;attività.
* Con chi devi parlare di un compito specifico.

Per scoprire come ottenere i dati migliori per questa visualizzazione, consulta [Panoramica dell’analisi migliorata](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizzazione delle attività nella visualizzazione dei voli

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. (Facoltativo) Per utilizzare un intervallo di date diverso, seleziona nuove date di inizio e di fine dal filtro dell’intervallo di date.

   ![](assets/filters-select-date-range-350x344.png)

   Per informazioni sull’utilizzo del filtro dell’intervallo di date, consulta [Applicazione di filtri in Analisi avanzata](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condizionale) Se devi limitare il set di dati del progetto, seleziona e applica i filtri che desideri utilizzare.

   Per ulteriori informazioni sull’aggiunta di filtri nell’analisi avanzata, consulta [Applicazione di filtri in Analisi avanzata](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Dopo aver aggiunto i filtri, vengono visualizzati i dati per un massimo di 50 progetti e i filtri rimangono attivi anche dopo aver lasciato la pagina o disconnesso da Workfront.

1. Nella visualizzazione del piano di volo o della mappa ad albero del progetto, fai clic su un progetto per visualizzare ulteriori informazioni.

   Vengono visualizzate le visualizzazioni Burndown e Attività in volo .

   >[!NOTE]
   >
   >Per ulteriori informazioni su queste altre visualizzazioni, consulta:
   >
   >   
   >   
   >   * [Visualizzazione della visualizzazione del piano di volo in Analisi avanzata](../enhanced-analytics/flight-plan-overview.md)
   >   * [Visualizzare la visualizzazione della mappa del percorso del progetto in Analisi avanzata](../enhanced-analytics/project-treemap-overview.md)
   >   * [Visualizzare la visualizzazione a discesa in Analisi avanzata](../enhanced-analytics/burndown-overview.md)


1. (Facoltativo) Per ingrandire un intervallo di date, seleziona un punto sulla visualizzazione per l’inizio dell’intervallo di date e trascina fino alla fine dell’intervallo di date.

   Tutte le altre visualizzazioni vengono aggiornate con lo stesso intervallo di date e viene creato un filtro per l’intervallo di tempo.

   ![](assets/timeframe-filter-350x220.png)

1. (Facoltativo) Per modificare l&#39;ordine delle attività, fai clic sul pulsante **Ordina per** quindi selezionate una nuova opzione di ordinamento:

   * **Data di completamento**
   * **In ordine alfabetico A-Z**
   * **Struttura a ripartizione del lavoro** Questa opzione corrisponde all’ordine in cui le attività vengono visualizzate nel progetto.

   Tutte le altre visualizzazioni nella pagina vengono aggiornate in base alla selezione dell’ordinamento.

1. Esaminare l&#39;avanzamento delle attività nel progetto selezionato, quindi passare il cursore del mouse su un&#39;attività specifica per visualizzare il numero di ore pianificate, la data di scadenza prevista e la percentuale di completamento.

   ![](assets/tasks-in-flight-task-details-350x242.png)

1. Fare clic su un&#39;attività per aprire i dettagli dell&#39;attività sul lato destro della schermata, dove è possibile visualizzare ulteriori informazioni sull&#39;attività, visualizzare o immettere aggiornamenti o apportare modifiche all&#39;attività.

   ![](assets/task-details-qs-350x675.png)

1. (Facoltativo) Per esportare i dati di visualizzazione, fai clic sul pulsante **Icona Esporta** ![](assets/export.png) nell’angolo in alto a destra della visualizzazione, quindi seleziona il formato di esportazione:

   * **Grafico (PNG)**
   * **Tabella dati (XSLX)**

