---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: Visualizzare la visualizzazione della mappa del percorso del progetto in Analisi avanzata
description: La visualizzazione della mappa ad albero del progetto è una visualizzazione delle ore (o dei giorni) lavorate in una specifica finestra di tempo rispetto ad altre attività lavorative di dimensioni diverse. Questo ti aiuta a capire quanto tempo le persone hanno dedicato a un progetto.
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 1%

---

# Visualizzare la visualizzazione della mappa del percorso del progetto in Analisi avanzata

La visualizzazione della mappa ad albero del progetto è una visualizzazione delle ore (o dei giorni) lavorate in una specifica finestra di tempo rispetto ad altre attività lavorative di dimensioni diverse. Questo ti aiuta a capire quanto tempo le persone hanno dedicato a un progetto.

![](assets/project-treemap-350x126.png)

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

## Visualizzazione della mappa ad albero del progetto

Le caselle nella visualizzazione mappa ad albero del progetto rappresentano i progetti e le dimensioni delle caselle mostrano un confronto tra il tempo trascorso in progetti diversi. Più grande è la scatola, più tempo è speso per il progetto.

La visualizzazione della mappa ad albero del progetto è composta da:

* **Caselle blu più piccole e leggere**: I progetti che hanno meno ore o giorni vengono visualizzati come caselle più piccole con un colore blu chiaro.

   ![](assets/project-treemap-smaller-box.png)

* **Caselle blu scure più grandi**: I progetti che hanno più ore (o giorni) vengono visualizzati come caselle più grandi con un colore blu scuro.

   ![](assets/project-treemap-larger-box-350x205.png)

* **Cassette blu di medie dimensioni**: I progetti che rientrano tra le due categorie vengono visualizzati come caselle di medie dimensioni con un’ombreggiatura blu tra i colori blu scuro e blu chiaro. Ci sono 3 possibili sfumature di blu per le scatole di medie dimensioni.

La legenda sul lato destro mostra una suddivisione delle ore completate per ogni tonalità di blu. Questa legenda è dinamica e si aggiorna in base ai dati.

![](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>Se osservi la visualizzazione della mappa ad albero del progetto per durata invece che per ore pianificate, questa legenda mostra un raggruppamento dei giorni lavorati per ogni tonalità di blu.\
>![](assets/project-treemap-days-worked.png)>

La visualizzazione di queste informazioni consente di determinare:

* La priorità degli elementi su cui lavorare durante l’intervallo di date selezionato.
* Su cosa le squadre stanno trascorrendo del tempo.
* Se i team si concentrano sulle cose giuste.
* Quando fai clic su un progetto specifico, quanto cambia l’ambito di un progetto in quel periodo di tempo.

Per scoprire come ottenere i dati migliori per questa visualizzazione, consulta [Panoramica dell’analisi migliorata](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizzare la visualizzazione della mappa del percorso del progetto

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. (Facoltativo) Per utilizzare un intervallo di date diverso, seleziona nuove date di inizio e di fine dal filtro dell’intervallo di date.

   ![](assets/filters-select-date-range-350x344.png)

   Per informazioni sull’utilizzo del filtro dell’intervallo di date, consulta [Applicazione di filtri in Analisi avanzata](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condizionale) Se devi limitare il set di dati del progetto, seleziona e applica i filtri che desideri utilizzare.

   Per ulteriori informazioni sull’aggiunta di filtri nell’analisi avanzata, consulta [Applicazione di filtri in Analisi avanzata](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Dopo aver aggiunto i filtri, vengono visualizzati i dati per un massimo di 50 progetti e i filtri rimangono attivi anche dopo aver lasciato la pagina o disconnesso da Workfront.

1. (Facoltativo) Per modificare l&#39;ordine dei progetti, fai clic sul pulsante **Ordina per** nell’angolo in alto a destra della visualizzazione Mappa del progetto, quindi seleziona una nuova opzione di ordinamento:

   * **A - Z**
   * **Z - A**
   * **Data di completamento pianificata**
   * **Data inizio pianificata**

   Tutte le altre visualizzazioni nella pagina vengono aggiornate in base alla selezione dell’ordinamento.

1. (Condizionale) Se nel set di dati sono presenti più di 50 progetti, utilizza le frecce nell’angolo in basso a sinistra della visualizzazione per passare da un gruppo di 50 progetti all’altro.

   Tutte le altre visualizzazioni nella pagina vengono aggiornate in base alla selezione della pagina.

   ![](assets/pagination-350x118.png)

1. (Facoltativo) Modificare la visualizzazione da **ore previste** a **durata**.

   L’opzione Orari pianificati è selezionata per impostazione predefinita.

1. Passa il cursore del mouse su un progetto per visualizzare la condizione del progetto, nonché il numero di ore pianificate totali, il numero di ore completate totali e il numero medio di ore trascorse al giorno sul progetto.

   ![](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >Se hai selezionato la **durata** visualizzi i seguenti dettagli sulla durata:
   >
   >* **Intervallo di tempo pianificato**: Numero di giorni pianificati per il completamento del progetto.
   >* **Giorni lavorati**: Durata pianificata per ogni attività completata entro l&#39;intervallo di date selezionato in alto, divisa per il numero di ore in un giorno.

   >   
   >![](assets/duration-treemap-350x159.png)
   >
   >Per ulteriori informazioni sulla durata, consulta la sezione &quot;Vista a tempo&quot; in [Panoramica dell’analisi migliorata](../enhanced-analytics/enhanced-analytics-overview.md).

1. (Facoltativo) Per esportare i dati di visualizzazione, fai clic sul pulsante **Icona Esporta** ![](assets/export.png) nell’angolo in alto a destra della visualizzazione, quindi seleziona il formato di esportazione:

   * **Grafico (PNG)**
   * **Tabella dati (XSLX)**

1. Fai clic su un progetto per aprire le visualizzazioni Abbandono e Attività in volo per comprendere meglio in che modo le attività e le ore (o i giorni) hanno contribuito alla dimensione di un progetto.

Per ulteriori informazioni sulla visualizzazione a discesa, consulta [Visualizzare la visualizzazione a discesa in Analisi avanzata](../enhanced-analytics/burndown-overview.md). Per ulteriori informazioni sulle attività nella visualizzazione dei voli, consulta [Visualizzazione delle attività nella visualizzazione dei voli in Enhanced analytics](../enhanced-analytics/tasks-in-flight-overview.md).

