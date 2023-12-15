---
title: Visualizzare la visualizzazione Burndown in Analisi avanzate
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualizzazione Burndown mostra il burndown di un progetto specifico nel tempo e ti aiuta a comprendere la relazione tra condizione del progetto, velocità e ore rimanenti, o giorni.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---

# Visualizzare la visualizzazione Burndown in Analisi avanzate

<!-- Audited: 12/2023 -->

La visualizzazione Burndown mostra il burndown di un progetto specifico nel tempo e ti aiuta a comprendere la relazione tra condizione del progetto, velocità e ore rimanenti, o giorni.

![Esempio di analisi ottimizzata](assets/burndown120623.png)

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td>
      <p>Nuovo: Qualsiasi</p>
      <p>oppure</p>
      <p>Corrente: Business o superiore</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>
      <p>Nuovo: Chiaro o superiore</p>
      <p>oppure</p>
      <p>Corrente: revisione o versione successiva</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso ai progetti in visualizzazione</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso.<br>Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Prerequisiti

Per i prerequisiti per utilizzare Enhanced Analytics, consulta la sezione &quot;Prerequisiti&quot; in [Panoramica di analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md#prerequisites).

## Comprendere la visualizzazione Burndown

La linea blu continua mostra la velocità pianificata dalla data di inizio alla data di completamento pianificata. Questa riga viene modificata quando il lavoro viene aggiunto, rimosso o aggiornato e diventa una riga verticale tratteggiata quando il progetto raggiunge la data di completamento pianificata.

![Velocità pianificata](assets/burndown-planned-line.png)

La linea effettiva mostra il numero di ore, o giorni, trascorsi sul progetto nel tempo. Il colore di questa riga indica ogni giorno la condizione del progetto:

* **Verde**: il progetto è sulla destinazione.

  ![Sul target](assets/burndown-green.png)

* **Arancione**: progetto a rischio.

  ![A rischio](assets/burndown-orange.png)

* **Rosso**: il progetto è in difficoltà.

  ![Nei guai](assets/burndown-red.png)

Per ulteriori informazioni su queste condizioni del progetto, vedi [Panoramica della condizione e del tipo di condizione del progetto](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Quando la linea effettiva si sposta verticalmente verso l&#39;alto, il lavoro è stato aggiunto al progetto. Quando la linea si sposta verticalmente verso il basso, il lavoro per il progetto è stato rimosso o completato.

Sotto l’asse x della visualizzazione, puoi vedere ulteriori informazioni sulle modifiche apportate alle attività e alle ore (o ai giorni) in un dato giorno (la quantità aggiunta, la quantità completata e la differenza tra i due valori).

La visualizzazione Burndown di tutte queste informazioni consente di determinare:

* Stato del singolo progetto nel tempo
* Come i problemi in arrivo (o il lavoro non pianificato) hanno influenzato il lavoro pianificato
* Quali eventi hanno esteso il progetto oltre la data di completamento originale

Per scoprire come ottenere i dati migliori per questa visualizzazione, consulta [Panoramica di analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizzare la visualizzazione Burndown

{{step1-to-analytics}}

1. (Facoltativo) Per utilizzare un intervallo di date diverso, seleziona nuove date di inizio e fine dal filtro dell’intervallo di date.

   ![Seleziona date](assets/filters-select-date-range-350x344.png)

   Per informazioni sull’utilizzo del filtro per intervalli di date, consulta [Applicare i filtri nelle analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condizionale) Se devi limitare il set di dati del progetto, seleziona e applica i filtri che desideri utilizzare.

   Per ulteriori informazioni sull’aggiunta di filtri in Analisi avanzate, consulta [Applicare i filtri nelle analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Dopo aver aggiunto i filtri, vengono visualizzati i dati per un massimo di 50 progetti e i filtri rimangono attivi anche dopo che hai lasciato la pagina o disconnesso da Workfront.

1. (Facoltativo) Per ingrandire un intervallo di date, seleziona un punto nella visualizzazione per l’inizio dell’intervallo di date e trascinalo fino alla fine dell’intervallo di date.

   Tutte le altre visualizzazioni vengono aggiornate allo stesso intervallo di date e viene creato automaticamente un filtro per l’intervallo di tempo.

   ![Filtro intervallo temporale](assets/timeframe-filter-350x220.png)

1. Nella visualizzazione Piano di volo o Mappa ad albero Progetto, fai clic su un progetto per visualizzare ulteriori informazioni.

   Vengono visualizzate le visualizzazioni Burndown e Attività in volo.

   >[!NOTE]
   >
   >Per ulteriori informazioni su queste altre visualizzazioni, consulta:
   >
   >   * [Visualizzare la visualizzazione del piano di volo in Analisi avanzate](../enhanced-analytics/flight-plan-overview.md)
   >   * [Visualizzare la mappa ad albero del progetto in Analisi avanzate](../enhanced-analytics/project-treemap-overview.md)
   >   * [Visualizzare la visualizzazione Attività in volo in Analisi avanzate](../enhanced-analytics/tasks-in-flight-overview.md)
   >

1. (Facoltativo) Modifica la visualizzazione da ore pianificate a **durata**.

   L’opzione Ore pianificate è selezionata per impostazione predefinita.

   >[!NOTE]
   >
   >Selezione **durata** modifica le informazioni su tutte le ore in giorni.\
   >![Burndown durata](assets/duration-burndown-350x112.png)\
   >Per ulteriori informazioni sulla durata nell’area Analisi avanzata, consulta la sezione &quot;Visualizzazione della durata&quot; in [Panoramica di analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md#duration-view).

1. Fate clic su un punto qualsiasi del grafico a linee.

   Sotto il grafico vengono visualizzate la data esatta e ulteriori informazioni sulle attività e le ore, o giorni, per il giorno selezionato.

   ![Dettagli burndown](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >Se la velocità effettiva è una linea piatta che corre lungo l’asse x (in linea con 0 ore o 0 giorni) della visualizzazione, significa che non sono state aggiunte al progetto ore o giorni pianificati.\
   >Se la velocità effettiva è una linea piatta sopra l&#39;asse x (allineata con un numero di ore o giorni) che non scende mai, significa che nessuna attività è stata completata entro il periodo di tempo filtrato.

1. (Facoltativo) Per esportare i dati di visualizzazione, fai clic sul pulsante **Esporta** icona ![Icona Esporta](assets/export.png)nell’angolo in alto a destra della visualizzazione e seleziona il formato di esportazione:

   * Grafico (PNG)
   * Tabella dati (XSLX)

1. (Facoltativo) Per visualizzare i dettagli sull’avanzamento delle attività nel progetto selezionato, osserva la visualizzazione Attività in volo che viene visualizzata sotto la visualizzazione Burndown. Per ulteriori informazioni, consulta [Visualizzare la visualizzazione Attività in volo in Analisi avanzate](/help/quicksilver/enhanced-analytics/tasks-in-flight-overview.md).
