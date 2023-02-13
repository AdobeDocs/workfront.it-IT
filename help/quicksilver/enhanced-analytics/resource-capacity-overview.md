---
title: Visualizzazione della visualizzazione della capacità delle risorse in Analisi avanzata
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualizzazione della capacità delle risorse mostra se un team è finito, sotto o alla capacità. Questo calcolo si basa su - EDIT ME.
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 0%

---

# Visualizzazione della visualizzazione della capacità delle risorse in Analisi avanzata

La visualizzazione della capacità delle risorse mostra se un team è finito, sotto o alla capacità.

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
   <td> <p>Visualizza accesso a progetti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso.<br>Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Per i prerequisiti per l’utilizzo di Analytics avanzato, consulta la sezione &quot;Prerequisiti&quot; in [Panoramica dell’analisi migliorata](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprendere la visualizzazione della capacità della risorsa

La visualizzazione della capacità delle risorse mostra se un team è finito, sotto o alla capacità. Questo calcolo si basa su:

* **Capacità disponibile**: La quantità totale di ore disponibili per il lavoro di un team domestico nel periodo di tempo filtrato

   >[!NOTE]
   >
   >Se stai osservando un periodo di tempo futuro, la capacità disponibile viene calcolata in base alla capacità del team per gli ultimi 7 giorni. Per questo motivo, non viene preso in considerazione alcun PTO pianificato.

* **Capacità prevista**: Quantità totale di ore di lavoro pianificate previste dal team di origine nel periodo di tempo filtrato

Questo confronto tra le ore pianificate e le ore pianificate effettive di un team domestico può aiutarti a determinare se non stai assegnando abbastanza lavoro al team principale o se potrebbero essere in fase di esaurimento da un carico di lavoro pesante.

![](assets/resource-capacity-350x110.png)

Nella visualizzazione della capacità delle risorse, puoi vedere i seguenti dettagli:

* **Capacità prevista**: In linea con il nome del team principale, il cerchio blu rappresenta il numero di ore pianificate assegnate al team principale.

   ![](assets/resource-capacity-blue-circle.png)

* **Capacità effettiva**: In linea con il nome del team principale, la linea verticale rappresenta il numero di ore disponibili per il team principale.

   ![](assets/resource-capacity-vertical-line.png)

* **Sovracapacità**: Quando la linea orizzontale e il cerchio blu vengono visualizzati a destra della linea verticale, al team principale è stato assegnato più lavoro di quello che possono completare nel numero di ore disponibili. Ciò significa che il team potrebbe superare la capacità per il periodo di tempo filtrato. Il numero rimanente di ore necessarie al completamento del team viene visualizzato a destra del cerchio blu.

   ![](assets/resource-capacity-over-capacity.png)

* **Incapacità**: Quando la linea orizzontale e il cerchio blu vengono visualizzati a sinistra della linea verticale, il team principale dispone di più ore disponibili del numero di ore di lavoro pianificate assegnate. Ciò significa che il team potrebbe essere in grado di utilizzare il periodo di tempo filtrato. Il numero aggiuntivo di ore disponibili per il team principale per completare il lavoro viene visualizzato a sinistra del cerchio blu.

   ![](assets/resource-capacity-under-capacity.png)

Passando il puntatore del mouse sopra una riga si può vedere il numero esatto di ore per la capacità pianificata e la capacità disponibile, nonché il numero di ore in cui il team di origine ha superato o è in grado di raggiungere la capacità.

La visualizzazione di queste informazioni consente di determinare:

* Se la squadra principale è stata sovrassegnata o sottoassegnata.
* Quali sono stati i progetti più grandi su cui si è concentrata la squadra domestica.
* Quali home team sono disponibili per il lavoro.

Per scoprire come ottenere i dati migliori per questa visualizzazione, consulta [Panoramica dell’analisi migliorata](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizzazione della visualizzazione della capacità della risorsa

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. Nel pannello a sinistra, seleziona **Persone**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Facoltativo) Per utilizzare un intervallo di date diverso, seleziona nuove date di inizio e di fine dal filtro dell’intervallo di date.

   ![](assets/filters-select-date-range-350x344.png)

   Per informazioni sull’utilizzo del filtro dell’intervallo di date, consulta [Applicazione di filtri in Analisi avanzata](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condizionale) Se non hai impostato il filtro Team, aggiungi il filtro Team e seleziona ogni team per il quale desideri visualizzare i dati.

   Per ulteriori informazioni sull’aggiunta di filtri nell’analisi avanzata, consulta [Applicazione di filtri in Analisi avanzata](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Dopo aver aggiunto i filtri, vengono visualizzati i dati per un massimo di 50 progetti e i filtri rimangono attivi anche dopo aver lasciato la pagina o disconnesso da Workfront.

1. (Facoltativo) Per ingrandire un intervallo di date, seleziona un punto sulla visualizzazione per l’inizio dell’intervallo di date e trascina fino alla fine dell’intervallo di date.

   Tutte le altre visualizzazioni vengono aggiornate con lo stesso intervallo di date e viene creato un filtro per l’intervallo di tempo.

   ![](assets/timeframe-filter-350x220.png)

1. Passa il puntatore del mouse sulla linea del team principale per vedere quante ore sono ancora disponibili per la pianificazione, la quantità di ore pianificate per il completamento del team principale e il numero totale di ore lavorate, etichettate come in eccesso, in esaurimento o alla capacità.

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. (Facoltativo) Per esportare i dati di visualizzazione, fai clic sul pulsante **Icona Esporta** ![](assets/export.png) nell’angolo in alto a destra della visualizzazione, quindi seleziona il formato di esportazione:

   * **Grafico (PNG)**
   * **Tabella dati (XSLX)**

1. Fai clic sul nome del team principale per visualizzare ulteriori informazioni nella visualizzazione della capacità del team.

   Per ulteriori informazioni sulla visualizzazione della capacità del team, consulta [Visualizzazione della visualizzazione della capacità del team in Analisi avanzata](../enhanced-analytics/team-capacity-overview.md).


