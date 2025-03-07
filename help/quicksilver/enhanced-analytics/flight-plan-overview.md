---
title: Visualizzare la visualizzazione del piano di volo in Analisi avanzate
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualizzazione del piano di volo mostra quanti progetti (entro i criteri di filtro applicati) erano in corso di esecuzione, quali cambiamenti di condizioni si sono verificati durante l’intero ciclo di vita di tali progetti e con quale frequenza questi progetti hanno rispettato le scadenze di completamento pianificate.
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 59e021aa3ae66e4fc8d9ce9eb57616f948e6cd90
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 4%

---

# Visualizzare la visualizzazione del piano di volo in Analisi avanzate

>[!IMPORTANT]
>
>Le funzioni di analisi avanzate verranno rimosse da Workfront la settimana del 26 maggio. Workfront Data Connect è una soluzione nuova e alternativa che può essere utilizzata per replicare qualsiasi visualizzazione avanzata di Analytics attualmente in uso. <br>Per ulteriori informazioni, consulta la [Guida all&#39;obsolescenza di Enhanced Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md).


La visualizzazione del piano di volo mostra quanti progetti (entro i criteri di filtro applicati) erano in corso di esecuzione, quali cambiamenti di condizioni si sono verificati durante l’intero ciclo di vita di tali progetti e con quale frequenza questi progetti hanno rispettato le scadenze di completamento pianificate.

![Piano di volo](assets/flight-plan-350x132.png)

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Piano Adobe Workfront</a>*</td> 
   <td> <p>Business o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica delle licenze Adobe Workfront</a>*</td> 
   <td> <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso ai progetti in visualizzazione</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso.<br>Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, vedi <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Accesso di visualizzazione al progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Prerequisiti

Per i prerequisiti per l&#39;utilizzo di Analisi avanzate, vedere la sezione &quot;Prerequisiti&quot; in [Panoramica di Analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprendere la visualizzazione del piano di volo

Nella durata effettiva di un progetto, puoi visualizzare solo le seguenti condizioni:

* Puntuale
* A Rischio
* In difficoltà

Per informazioni sulle condizioni del progetto, vedere [Panoramica sulla condizione e sul tipo di condizione del progetto](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

La visualizzazione del piano di volo mostra i seguenti dettagli del progetto:

* **Durata pianificata**: la linea blu orizzontale rappresenta la lunghezza pianificata del progetto, con i triangoli alla fine della linea che indicano la data di inizio e la data di fine.

  ![Durata pianificata](assets/planned-duration-line-350x37.png)

* **Durata effettiva**: la linea spessa e colorata sotto la durata pianificata rappresenta la lunghezza effettiva del progetto. Il colore della riga cambia a seconda delle condizioni del progetto in quel particolare momento della vita del progetto.

  ![Durata effettiva](assets/actual-duration-line.png)

* **Condizione effettiva**: la linea spessa e colorata mostra anche la condizione di un progetto in momenti diversi. Il colore della linea cambia a seconda delle condizioni del progetto:

   * **Verde**: In Destinazione
   * **Arancione**: A Rischio
   * **Rosso**: Problemi

  ![Condizione effettiva](assets/actual-condition-color.png)

Passando il cursore sopra una riga del progetto nella visualizzazione Piano di volo, puoi visualizzare informazioni sull’arco temporale pianificato del progetto, la condizione del progetto corrente e, se applicabile, la condizione personalizzata. Per ottenere una visualizzazione più dettagliata di ciò che può aver influenzato la durata o la condizione, puoi guardare le altre visualizzazioni nell’area Analisi avanzata.

La visualizzazione di queste informazioni consente di determinare:

* Gli eventi che prolungano un progetto oltre la data di completamento pianificata originale.
* Quando si verifica un problema in un progetto.
* Quanti progetti sono aperti nello stesso periodo di tempo.
* Quanti progetti sono attivi.
* Quali progetti richiedono maggiore attenzione o supporto.

Per informazioni su come ottenere i dati migliori per questa visualizzazione, consulta [Panoramica sulle analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizza la visualizzazione del piano di volo

1. Fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. (Facoltativo) Per utilizzare un intervallo di date diverso, seleziona nuove date di inizio e fine dal filtro dell’intervallo di date.

   ![Seleziona intervallo date](assets/filters-select-date-range-350x344.png)

   Per informazioni sull&#39;utilizzo del filtro dell&#39;intervallo di date, vedere [Applicare filtri in Analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condizionale) Se devi limitare il set di dati del progetto, seleziona e applica i filtri che desideri utilizzare.

   Per ulteriori informazioni sull&#39;aggiunta di filtri in Analisi avanzate, vedere [Applicare filtri in Analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Dopo aver aggiunto i filtri, vengono visualizzati i dati per un massimo di 50 progetti e i filtri rimangono attivi anche dopo che hai lasciato la pagina o disconnesso da Workfront.

1. (Facoltativo) Per ingrandire un intervallo di date, seleziona un punto nella visualizzazione per l’inizio dell’intervallo di date e trascina fino alla fine dell’intervallo di date.

   Tutte le altre visualizzazioni vengono aggiornate allo stesso intervallo di date e viene creato un filtro per l’intervallo di tempo.

   ![Filtro intervallo di tempo](assets/timeframe-filter-350x220.png)

1. (Facoltativo) Per modificare l&#39;ordinamento dei progetti, fare clic sul menu **Ordina per** nell&#39;angolo superiore destro della visualizzazione del piano di volo, quindi selezionare una nuova opzione di ordinamento:

   * **A - Z**
   * **Z - A**
   * **Data di completamento pianificata**
   * **Data inizio pianificata**

   Tutte le altre visualizzazioni nella pagina vengono aggiornate in base alla selezione dell’ordinamento.

1. (Facoltativo) Se nel set di dati sono presenti più di 50 progetti, utilizza le frecce nell’angolo in basso a sinistra della visualizzazione per passare da un gruppo di 50 progetti all’altro.

   Tutte le altre visualizzazioni nella pagina vengono aggiornate in base alla selezione della pagina.

   ![Paginazione](assets/pagination-350x118.png)

1. Passa il puntatore del mouse sul grafico a barre del progetto per visualizzare la linea blu della data e i seguenti dettagli:

   * Timeline pianificata
   * Condizione corrente
   * Condizione personalizzata (se applicabile)

   ![Grafico a barre del progetto](assets/project-bar-graph-350x143.png)

1. (Facoltativo) Per esportare i dati di visualizzazione, fai clic sull&#39;icona **Esporta** ![Icona Esporta](assets/export.png) nell&#39;angolo in alto a destra della visualizzazione, quindi seleziona il formato di esportazione:

   * **Grafico (PNG)**
   * **Tabella dati (XSLX)**

1. Per visualizzare ulteriori informazioni sul progetto, fai clic su un progetto nella visualizzazione per aprire le visualizzazioni Burndown e Attività in volo.

   Queste visualizzazioni possono aiutarti a ottenere informazioni più approfondite su cosa ha causato la deviazione del progetto. Semplificano inoltre il check-in di un progetto in corso.\
   Per ulteriori informazioni sulla visualizzazione Burndown, consulta [Visualizzare la visualizzazione Burndown in Analisi avanzate](../enhanced-analytics/burndown-overview.md). Per ulteriori informazioni sulla visualizzazione Attività in volo, consulta [Visualizzare la visualizzazione Attività in volo in Analisi avanzate](../enhanced-analytics/tasks-in-flight-overview.md).

