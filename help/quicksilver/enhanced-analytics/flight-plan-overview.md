---
title: Visualizzazione della visualizzazione del piano di volo in Analisi avanzata
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualizzazione del piano di volo mostra quanti progetti (nell’ambito dei criteri di filtro applicati) erano in volo, quali cambiamenti di condizione sono avvenuti durante la durata di questi progetti e quanto strettamente questi progetti hanno rispettato le scadenze di completamento previste.
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 2%

---

# Visualizzazione della visualizzazione del piano di volo in Analisi avanzata

La visualizzazione del piano di volo mostra quanti progetti (nell’ambito dei criteri di filtro applicati) erano in volo, quali cambiamenti di condizione sono avvenuti durante la durata di questi progetti e quanto strettamente questi progetti hanno rispettato le scadenze di completamento previste.

![](assets/flight-plan-350x132.png)

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
   <td> <p>Visualizza l’accesso al progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Prerequisiti

Per i prerequisiti per l’utilizzo di Analytics avanzato, consulta la sezione &quot;Prerequisiti&quot; in [Panoramica dell’analisi migliorata](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprendere la visualizzazione del piano di volo

Nella durata effettiva di un progetto, è possibile visualizzare solo le seguenti condizioni del progetto:

* Puntuale
* A Rischio
* In difficoltà

Per informazioni sulle condizioni del progetto, consulta [Panoramica del tipo di condizione e condizione del progetto](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

La visualizzazione del piano di volo mostra i seguenti dettagli del progetto:

* **Durata prevista**: La linea blu orizzontale rappresenta la lunghezza prevista del progetto, con i triangoli a una delle estremità della linea che indicano la data di inizio e la data di fine.

   ![](assets/planned-duration-line-350x37.png)

* **Durata effettiva**: La linea spessa e colorata al di sotto della durata prevista rappresenta la lunghezza effettiva del progetto. Il colore della linea cambia a seconda della condizione del progetto in quel particolare momento della vita del progetto.

   ![](assets/actual-duration-line.png)

* **Condizione effettiva**: La linea spessa e colorata mostra anche la condizione di un progetto in diversi momenti nel tempo. Il colore della linea cambia a seconda della condizione del progetto:

   * **Verde**: Su Target
   * **Arancio**: A rischio
   * **Rosso**: In problemi

   ![](assets/actual-condition-color.png)

Passando il puntatore del mouse su una riga del progetto nella visualizzazione Piano di volo, è possibile visualizzare informazioni sull’intervallo di tempo pianificato del progetto, sulla condizione del progetto corrente e, se applicabile, sulla condizione personalizzata. Per ottenere una visualizzazione più approfondita di ciò che potrebbe aver influenzato la durata o la condizione, puoi esaminare le altre visualizzazioni nell’area Analisi avanzata.

La visualizzazione di queste informazioni consente di determinare:

* Eventi che estendono un progetto oltre la data di completamento pianificata originale.
* Quando un progetto inizia ad avere problemi.
* Quanti progetti sono aperti nello stesso periodo di tempo.
* Quanti progetti sono attivi.
* Quali progetti necessitano di maggiore attenzione o sostegno.

Per informazioni su come ottenere i dati migliori per questa visualizzazione, consulta [Panoramica dell’analisi migliorata](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizzazione della visualizzazione del piano di volo

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. (Facoltativo) Per utilizzare un intervallo di date diverso, seleziona nuove date di inizio e di fine dal filtro dell’intervallo di date.

   ![](assets/filters-select-date-range-350x344.png)

   Per informazioni sull’utilizzo del filtro dell’intervallo di date, consulta [Applicazione di filtri in Analisi avanzata](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condizionale) Se devi limitare il set di dati del progetto, seleziona e applica i filtri che desideri utilizzare.

   Per ulteriori informazioni sull’aggiunta di filtri nell’analisi avanzata, consulta [Applicazione di filtri in Analisi avanzata](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Dopo aver aggiunto i filtri, vengono visualizzati i dati per un massimo di 50 progetti e i filtri rimangono attivi anche dopo aver lasciato la pagina o disconnesso da Workfront.

1. (Facoltativo) Per ingrandire un intervallo di date, seleziona un punto sulla visualizzazione per l’inizio dell’intervallo di date e trascina fino alla fine dell’intervallo di date.

   Tutte le altre visualizzazioni vengono aggiornate con lo stesso intervallo di date e viene creato un filtro per l’intervallo di tempo.

   ![](assets/timeframe-filter-350x220.png)

1. (Facoltativo) Per modificare l&#39;ordine dei progetti, fai clic sul pulsante **Ordina per** nell’angolo in alto a destra della visualizzazione Piano di volo , seleziona una nuova opzione di ordinamento:

   * **A - Z**
   * **Z - A**
   * **Data di completamento pianificata**
   * **Data inizio pianificata**

   Tutte le altre visualizzazioni nella pagina vengono aggiornate in base alla selezione dell’ordinamento.

1. (Condizionale) Se nel set di dati sono presenti più di 50 progetti, utilizza le frecce nell’angolo in basso a sinistra della visualizzazione per passare da un gruppo di 50 progetti all’altro.

   Tutte le altre visualizzazioni nella pagina vengono aggiornate in base alla selezione della pagina.

   ![](assets/pagination-350x118.png)

1. Passa il puntatore del mouse sul grafico a barre del progetto per visualizzare la data in blu e i dettagli seguenti:

   * Timeline pianificata
   * Condizione attuale
   * Condizione personalizzata (se applicabile)

   ![](assets/project-bar-graph-350x143.png)

1. (Facoltativo) Per esportare i dati di visualizzazione, fai clic sul pulsante **Esporta** icona ![](assets/export.png) nell’angolo in alto a destra della visualizzazione, quindi seleziona il formato di esportazione:

   * **Grafico (PNG)**
   * **Tabella dati (XSLX)**

1. Per visualizzare ulteriori informazioni sul progetto, fai clic su un progetto sulla visualizzazione per aprire il menu a discesa e le attività nelle visualizzazioni dei voli.

   Queste visualizzazioni possono aiutarti a ottenere informazioni più approfondite su cosa ha causato l’interruzione della realizzazione del progetto. Inoltre, consentono di eseguire facilmente il check-in di un progetto in corso.\
   Per ulteriori informazioni sulla visualizzazione a discesa, consulta [Visualizzare la visualizzazione a discesa in Analisi avanzata](../enhanced-analytics/burndown-overview.md). Per ulteriori informazioni sulle attività nella visualizzazione dei voli, consulta [Visualizzazione delle attività nella visualizzazione dei voli in Enhanced analytics](../enhanced-analytics/tasks-in-flight-overview.md).

