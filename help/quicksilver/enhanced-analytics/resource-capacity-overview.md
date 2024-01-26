---
title: Visualizzare la visualizzazione Capacità risorse in Analisi avanzate
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Quando visualizzi il grafico di visualizzazione della capacità delle risorse di analisi avanzate in Adobe Workfront, puoi valutare se un team è al di sopra, al di sotto o al limite della capacità.
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: 3b3ba7cc6a975af71205f7f524e1a9a91a9d3810
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Visualizzare la visualizzazione Capacità risorse in Analisi avanzate

Quando visualizzi il grafico di visualizzazione della capacità delle risorse di analisi avanzate in Adobe Workfront, puoi valutare se un team è al di sopra, al di sotto o al limite della capacità.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>piano Adobe Workfront</a>*</td> 
   <td> <p>Corrente: Business o superiore</p>
   Oppure
   <p>Nuovo: Qualsiasi</p>
    </td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront*</td> 
   <td> <p>Corrente: revisione o versione successiva</p>
   Oppure
   <p>Nuovo: Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazione del livello di accesso</td> 
   <td> <p>Accesso ai progetti in visualizzazione</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare l’autorizzazione per un progetto</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni sulla pianificazione, il tipo di licenza o l&#39;accesso disponibili, contattare l&#39;amministratore Workfront. Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisiti

Per i prerequisiti per utilizzare Enhanced Analytics, consulta la sezione &quot;Prerequisiti&quot; in [Panoramica di analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprendere il grafico Capacità risorse

Il grafico Capacità risorse mostra se un team è al di sopra, al di sotto o alla capacità. Questo calcolo si basa su:

* **Capacità disponibile**: la quantità totale di ore che un team predefinito ha a disposizione per lavorare nel periodo di tempo filtrato

  >[!NOTE]
  >
  >Se si considera un periodo di tempo futuro, la capacità disponibile viene calcolata in base alla capacità del team per gli ultimi 7 giorni. Per questo motivo, non vengono prese in considerazione eventuali ferie retribuite programmate.

* **Capacità pianificata**: la quantità totale di ore di lavoro pianificate previste dal team principale nel periodo di tempo filtrato

Questo confronto tra le ore pianificate di un team predefinito e le ore pianificate effettive può aiutarti a determinare se non stai assegnando abbastanza lavoro al team principale o se si sta verificando un esaurimento da un carico di lavoro pesante.

![](assets/resource-capacity-350x110.png)

Nella visualizzazione Capacità risorse puoi visualizzare i seguenti dettagli:

* **Capacità pianificata**: in linea con il nome di un team principale, il cerchio blu rappresenta il numero di ore pianificate assegnate al team principale.

  ![](assets/resource-capacity-blue-circle.png)

* **Capacità effettiva**: in linea con il nome di un team principale, la riga verticale rappresenta il numero di ore disponibili per il team principale.

  ![](assets/resource-capacity-vertical-line.png)

* **Sovraccapacità**: quando la linea orizzontale e il cerchio blu sono visualizzati a destra della linea verticale, al team principale è stato assegnato più lavoro di quello che può completare nel numero di ore disponibili. Ciò significa che il team potrebbe avere una capacità eccessiva per il periodo di tempo filtrato. Il numero di ore rimanenti che il team deve completare viene visualizzato a destra del cerchio blu.

  ![](assets/resource-capacity-over-capacity.png)

* **Sotto capacità**: quando la linea orizzontale e il cerchio blu vengono visualizzati a sinistra della linea verticale, il team interno ha più ore disponibili del numero di ore di lavoro pianificate che sono state assegnate. Ciò significa che la capacità del team potrebbe essere insufficiente per il periodo di tempo filtrato. Il numero aggiuntivo di ore disponibili per il completamento del lavoro da parte del team interno viene visualizzato a sinistra del cerchio blu.

  ![](assets/resource-capacity-under-capacity.png)

Passando il cursore sopra una riga, viene visualizzato il numero esatto di ore per la capacità pianificata e la capacità disponibile, nonché il numero di ore in cui il team predefinito ha una capacità eccessiva o insufficiente.

La visualizzazione di queste informazioni consente di determinare:

* Se la squadra principale è stata sovrassegnata o sottoassegnata.
* I progetti più grandi erano quelli su cui si concentrava il team interno.
* Quali team principali sono disponibili per il lavoro.

Per scoprire come ottenere i dati migliori per questa visualizzazione, consulta [Panoramica di analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizzare la visualizzazione Capacità risorse

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. Nel pannello a sinistra, seleziona **Persone**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Facoltativo) Per utilizzare un intervallo di date diverso, seleziona nuove date di inizio e fine dal filtro dell’intervallo di date.

   ![](assets/filters-select-date-range-350x344.png)

   Per informazioni sull’utilizzo del filtro per intervalli di date, consulta [Applicare i filtri nelle analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condizionale) Se non hai impostato il filtro Team, aggiungi il filtro Team e seleziona ogni team per il quale desideri visualizzare i dati.

   Per ulteriori informazioni sull’aggiunta di filtri in Analisi avanzate, consulta [Applicare i filtri nelle analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Dopo aver aggiunto i filtri, vengono visualizzati i dati per un massimo di 50 progetti e i filtri rimangono attivi anche dopo che hai lasciato la pagina o disconnesso da Workfront.

1. (Facoltativo) Per ingrandire un intervallo di date, seleziona un punto nella visualizzazione per l’inizio dell’intervallo di date e trascina fino alla fine dell’intervallo di date.

   Tutte le altre visualizzazioni vengono aggiornate allo stesso intervallo di date e viene creato un filtro per l’intervallo di tempo.

   ![](assets/timeframe-filter-350x220.png)

1. Passa il cursore del mouse sulla riga del team predefinito per vedere quante ore sono ancora disponibili da programmare, la quantità di ore pianificate per il completamento da parte del team principale e il numero totale di ore lavorate, etichettate come al di sopra, al di sotto o alla capacità.

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. (Facoltativo) Per esportare i dati di visualizzazione, fai clic sul pulsante **Icona Esporta** ![](assets/export.png) nell’angolo in alto a destra della visualizzazione, seleziona il formato di esportazione:

   * **Grafico (PNG)**
   * **Tabella dati (XSLX)**

1. Fai clic sul nome di un team principale per visualizzare ulteriori informazioni nella visualizzazione Capacità del team.

   Per ulteriori informazioni sulla visualizzazione Capacità team, consulta [Visualizzare la visualizzazione della capacità del team in Analisi avanzate](../enhanced-analytics/team-capacity-overview.md).


