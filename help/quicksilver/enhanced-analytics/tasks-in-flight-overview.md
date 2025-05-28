---
title: Visualizzare la visualizzazione Attività in volo in Analisi avanzate
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualizzazione Attività in volo mostra quante attività (entro i criteri di filtro applicati) sono in corso per un progetto, la percentuale di lavoro completato per ogni attività e come sono programmate le attività.
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 4%

---

# Visualizzare la visualizzazione Attività in volo in Analisi avanzate

>[!IMPORTANT]
>
>Analisi avanzata è stato rimosso da Workfront il 27 maggio. Workfront Data Connect è una soluzione nuova e alternativa che può essere utilizzata per replicare qualsiasi visualizzazione avanzata di Analytics attualmente in uso. <br>Per ulteriori informazioni, consulta la [Guida all&#39;obsolescenza di Enhanced Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md).


La visualizzazione Attività in volo mostra quante attività (entro i criteri di filtro applicati) sono in corso per un progetto, la percentuale di lavoro completato per ogni attività e come sono programmate le attività.

![Attività in corso](assets/tasks-in-flight-possible-replacement-350x104.png)

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">Piano Adobe Workfront</a>*</td> 
   <td> <p>Business o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica delle licenze Adobe Workfront</a>*</td> 
   <td> <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso ai progetti in visualizzazione</p> <p>Accesso di visualizzazione alle attività (per aggiornare le attività, è necessario l'accesso di modifica alle attività).</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso.<br>Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, vedi <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza autorizzazioni per oggetti progetto e attività</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Prerequisiti

Per i prerequisiti per l&#39;utilizzo di Analisi avanzate, vedere la sezione &quot;Prerequisiti&quot; in [Panoramica di Analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprendere la visualizzazione Attività in volo

La visualizzazione Attività nel piano di volo mostra i seguenti dettagli di attività:

* **Durata attività pianificata**: la lunghezza di una barra delle attività indica la durata pianificata, basata sulla data di inizio e sulla data di completamento dell&#39;attività.

  ![Attività nella durata del volo](assets/tasks-in-flight-duration-350x80.png)

* **Impegno di lavoro completato**: il colore blu scuro all&#39;interno di una barra delle attività indica la quantità di lavoro completato per un&#39;attività. La percentuale di completamento viene visualizzata a destra della barra delle applicazioni.

  ![Attività in volo blu scuro](assets/tasks-in-flight-dark-blue-350x35.png)

* **Impegno di lavoro rimanente**: il colore blu chiaro nella barra delle attività indica la quantità di lavoro da completare per un&#39;attività.

  ![Attività in volo azzurro](assets/tasks-in-flight-light-blue-350x35.png)

Queste informazioni possono essere utili per determinare:

* Dove l&#39;impegno lavorativo è stato concentrato.
* Quali attività potrebbero mettere a rischio un progetto.
* Quanto è vicina al completamento un’attività.
* A chi riviolgersi per un’attività specifica.

Per informazioni su come ottenere i dati migliori per questa visualizzazione, consulta [Panoramica sulle analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizza la visualizzazione Attività in volo

1. Fai clic sull&#39;icona del menu principale ![icona del menu principale](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. (Facoltativo) Per utilizzare un intervallo di date diverso, seleziona nuove date di inizio e fine dal filtro dell’intervallo di date.

   ![Seleziona intervallo date](assets/filters-select-date-range-350x344.png)

   Per informazioni sull&#39;utilizzo del filtro dell&#39;intervallo di date, vedere [Applicare filtri in Analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condizionale) Se devi limitare il set di dati del progetto, seleziona e applica i filtri che desideri utilizzare.

   Per ulteriori informazioni sull&#39;aggiunta di filtri in Analisi avanzate, vedere [Applicare filtri in Analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Dopo aver aggiunto i filtri, vengono visualizzati i dati per un massimo di 50 progetti e i filtri rimangono attivi anche dopo che hai lasciato la pagina o disconnesso da Workfront.

1. Nella visualizzazione Piano di volo o Mappa ad albero Progetto, fai clic su un progetto per visualizzare ulteriori informazioni.

   Vengono visualizzate le visualizzazioni Burndown e Attività in volo.

   >[!NOTE]
   >
   >Per ulteriori informazioni su queste altre visualizzazioni, consulta:
   >
   >   
   >   
   >   * [Visualizzazione del piano di volo in Analisi avanzate](../enhanced-analytics/flight-plan-overview.md)
   >   * [Visualizzazione Mappa ad albero progetto in Analisi avanzate](../enhanced-analytics/project-treemap-overview.md)
   >   * [Visualizzazione Burndown in Analisi avanzate](../enhanced-analytics/burndown-overview.md)
   >   
   >

1. (Facoltativo) Per ingrandire un intervallo di date, seleziona un punto nella visualizzazione per l’inizio dell’intervallo di date e trascina fino alla fine dell’intervallo di date.

   Tutte le altre visualizzazioni vengono aggiornate allo stesso intervallo di date e viene creato un filtro per l’intervallo di tempo.

   ![Filtro intervallo di tempo](assets/timeframe-filter-350x220.png)

1. (Facoltativo) Per modificare l&#39;ordinamento delle attività, fare clic sul menu **Ordina per**, quindi selezionare una nuova opzione di ordinamento:

   * **Data di completamento**
   * **Alfabeticamente A-Z**
   * **Struttura funzionale** (questa opzione corrisponde all&#39;ordine di visualizzazione delle attività nel progetto).

   Tutte le altre visualizzazioni nella pagina vengono aggiornate in base alla selezione dell’ordinamento.

1. Esamina l’avanzamento delle attività nel progetto selezionato, quindi passa il cursore su un’attività specifica per visualizzare il numero di ore pianificate, la data di scadenza pianificata e la percentuale di completamento.

   ![Attività nei dettagli del volo](assets/tasks-in-flight-task-details-350x242.png)

1. Fare clic su un&#39;attività per aprirne i dettagli sul lato destro della schermata, dove è possibile visualizzare ulteriori informazioni sull&#39;attività, visualizzare o immettere aggiornamenti o apportare modifiche all&#39;attività.

   ![Dettagli attività](assets/task-details-qs-350x675.png)

1. (Facoltativo) Per esportare i dati di visualizzazione, fai clic sull&#39;**icona Esporta** ![icona Esporta](assets/export.png) nell&#39;angolo in alto a destra della visualizzazione, quindi seleziona il formato di esportazione:

   * **Grafico (PNG)**
   * **Tabella dati (XSLX)**

