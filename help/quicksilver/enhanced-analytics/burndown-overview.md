---
title: Visualizzare la visualizzazione Burndown in Analisi avanzate
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualizzazione Burndown mostra il burndown di un progetto specifico nel tempo e ti aiuta a comprendere la relazione tra condizione del progetto, velocità e ore rimanenti, o giorni.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: 45dac4c5e8ff584546783d561c04d137697a03a4
workflow-type: tm+mt
source-wordcount: '795'
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
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>
      <p>Nuovo: Qualsiasi</p>
      <p>oppure</p>
      <p>Corrente: Business o superiore</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
      <p>Nuovo: Chiaro o superiore</p>
      <p>oppure</p>
      <p>Corrente: revisione o versione successiva</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso ai progetti in visualizzazione</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza</p> </td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisiti

Per i prerequisiti per l&#39;utilizzo di Analisi avanzate, vedere la sezione &quot;Prerequisiti&quot; in [Panoramica di Analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprendere la visualizzazione Burndown

La linea blu continua mostra la velocità pianificata dalla data di inizio alla data di completamento pianificata. Questa riga viene modificata quando il lavoro viene aggiunto, rimosso o aggiornato e diventa una riga verticale tratteggiata quando il progetto raggiunge la data di completamento pianificata.

![Velocità pianificata](assets/burndown-planned-line.png)

La linea effettiva mostra il numero di ore, o giorni, trascorsi sul progetto nel tempo. Il colore di questa riga indica ogni giorno la condizione del progetto:

* **Verde**: il progetto è in arrivo.

  ![In destinazione](assets/burndown-green.png)

* **Arancione**: progetto a rischio.

  ![A rischio](assets/burndown-orange.png)

* **Rosso**: il progetto è in difficoltà.

  ![Problemi](assets/burndown-red.png)

Per ulteriori informazioni su queste condizioni del progetto, vedere [Panoramica sulla condizione e sul tipo di condizione del progetto](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Quando la linea effettiva si sposta verticalmente verso l&#39;alto, il lavoro è stato aggiunto al progetto. Quando la linea si sposta verticalmente verso il basso, il lavoro per il progetto è stato rimosso o completato.

Sotto l’asse x della visualizzazione, puoi vedere ulteriori informazioni sulle modifiche apportate alle attività e alle ore (o ai giorni) in un dato giorno (la quantità aggiunta, la quantità completata e la differenza tra i due valori).

La visualizzazione Burndown di tutte queste informazioni consente di determinare:

* Stato del singolo progetto nel tempo
* Come i problemi in arrivo (o il lavoro non pianificato) hanno influenzato il lavoro pianificato
* Quali eventi hanno esteso il progetto oltre la data di completamento originale

Per informazioni su come ottenere i dati migliori per questa visualizzazione, consulta [Panoramica sulle analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizzare la visualizzazione Burndown

{{step1-to-analytics}}

1. (Facoltativo) Per utilizzare un intervallo di date diverso, seleziona nuove date di inizio e fine dal filtro dell’intervallo di date.

   ![Seleziona date](assets/filters-select-date-range-350x344.png)

   Per informazioni sull&#39;utilizzo del filtro dell&#39;intervallo di date, vedere [Applicare filtri in Analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condizionale) Se devi limitare il set di dati del progetto, seleziona e applica i filtri che desideri utilizzare.

   Per ulteriori informazioni sull&#39;aggiunta di filtri in Analisi avanzate, vedere [Applicare filtri in Analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Dopo aver aggiunto i filtri, vengono visualizzati i dati per un massimo di 50 progetti e i filtri rimangono attivi anche dopo che hai lasciato la pagina o disconnesso da Workfront.

1. (Facoltativo) Per ingrandire un intervallo di date, seleziona un punto nella visualizzazione per l’inizio dell’intervallo di date e trascinalo fino alla fine dell’intervallo di date.

   Tutte le altre visualizzazioni vengono aggiornate allo stesso intervallo di date e viene creato automaticamente un filtro per l’intervallo di tempo.

   ![Filtro intervallo di tempo](assets/timeframe-filter-350x220.png)

1. Nella visualizzazione Piano di volo o Mappa ad albero Progetto, fai clic su un progetto per visualizzare ulteriori informazioni.

   Vengono visualizzate le visualizzazioni Burndown e Attività in volo.

   >[!NOTE]
   >
   >Per ulteriori informazioni su queste altre visualizzazioni, consulta:
   >
   >   * [Visualizzazione del piano di volo in Analisi avanzate](../enhanced-analytics/flight-plan-overview.md)
   >   * [Visualizzazione Mappa ad albero progetto in Analisi avanzate](../enhanced-analytics/project-treemap-overview.md)
   >   * [Visualizza le Attività nella visualizzazione di volo in Analisi avanzate](../enhanced-analytics/tasks-in-flight-overview.md)
   >

1. (Facoltativo) Cambia la visualizzazione da ore pianificate a **durata**.

   L’opzione Ore pianificate è selezionata per impostazione predefinita.

   >[!NOTE]
   >
   >Selezionando **durata** tutte le informazioni sulle ore vengono convertite in giorni.\
   >![Burndown durata](assets/duration-burndown-350x112.png)\
   >Per ulteriori informazioni sulla durata nell&#39;area Analisi avanzata, vedere la sezione &quot;Visualizzazione della durata&quot; in [Panoramica analisi avanzata](../enhanced-analytics/enhanced-analytics-overview.md#duration-view).

1. Fate clic su un punto qualsiasi del grafico a linee.

   Sotto il grafico vengono visualizzate la data esatta e ulteriori informazioni sulle attività e le ore, o giorni, per il giorno selezionato.

   ![Dettagli Burndown](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >Se la velocità effettiva è una linea piatta che corre lungo l’asse x (in linea con 0 ore o 0 giorni) della visualizzazione, significa che non sono state aggiunte al progetto ore o giorni pianificati.\
   >Se la velocità effettiva è una linea piatta sopra l&#39;asse x (allineata con un numero di ore o giorni) che non scende mai, significa che nessuna attività è stata completata entro il periodo di tempo filtrato.

1. (Facoltativo) Per esportare i dati di visualizzazione, fai clic sull&#39;icona **Esporta** ![Icona Esporta](assets/export.png) nell&#39;angolo in alto a destra della visualizzazione e seleziona il formato di esportazione:

   * Grafico (PNG)
   * Tabella dati (XSLX)

1. (Facoltativo) Per visualizzare i dettagli sull’avanzamento delle attività nel progetto selezionato, osserva la visualizzazione Attività in volo che viene visualizzata sotto la visualizzazione Burndown. Per ulteriori informazioni, consulta [Visualizzare le attività nella visualizzazione di volo in Analisi avanzate](/help/quicksilver/enhanced-analytics/tasks-in-flight-overview.md).
