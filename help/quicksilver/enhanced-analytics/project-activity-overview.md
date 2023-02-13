---
title: Visualizzazione della visualizzazione delle attività del progetto in Analisi avanzata
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualizzazione dell’attività Progetto mostra una visualizzazione aggregata delle attività a livello di progetto, ovvero le attività di ogni persona assegnata al progetto, che si sono verificate durante un intervallo di tempo specifico. È possibile limitare l’attenzione per comprendere le attività all’interno di un progetto, oppure confrontare le attività di progetto con altri progetti in Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 1%

---

# Visualizzazione della visualizzazione delle attività del progetto in Analisi avanzata

La visualizzazione dell’attività Progetto mostra una visualizzazione aggregata delle attività a livello di progetto, ovvero le attività di ogni persona assegnata al progetto, che si sono verificate durante un intervallo di tempo specifico. È possibile limitare l’attenzione per comprendere le attività all’interno di un progetto, oppure confrontare le attività di progetto con altri progetti in Adobe Workfront.

>[!NOTE]
>
>La visualizzazione Attività per team si comporta in modo simile a questa visualizzazione, ma la visualizzazione Attività per team mostra l’attività del team principale per tutti i progetti.\
>Per informazioni sulla visualizzazione Attività per team, consulta [Visualizzazione dell’attività per team in Analisi avanzata](../enhanced-analytics/activity-by-team-overview.md).

<!--WRITER bad link; there is no Activity by Team.png
[![](assets/project-activity-350x114.png)](../Resources/Images/Analytics/Activity by Team.png)
-->

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">piano Workfront</a>*</td> 
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

## Comprendere la visualizzazione dell’attività Progetto

Le attività del progetto vengono visualizzate in colori diversi per riepilogare eventi specifici in un progetto per un periodo di tempo:

* **Utenti connessi**: Le caselle viola mostrano che le persone assegnate al progetto hanno effettuato l’accesso in quel giorno. Una tonalità più scura indica un numero maggiore di persone che accedono.

   ![](assets/project-activity-users-logged-in.png)

* **Modifica dello stato dell&#39;attività**: Le caselle rosa mostrano che le persone hanno cambiato lo stato di un&#39;attività per il progetto in quel giorno. Un&#39;ombreggiatura più scura indica un numero maggiore di stati di attività che cambiano.

   ![](assets/project-activity-task-status-changes.png)

* **Attività completate**: Le caselle blu mostrano che le persone hanno completato un’attività per il progetto. Una tonalità più scura indica un numero maggiore di attività completate.

   ![](assets/project-activity-tasks-completed.png)

Passando il puntatore del mouse su una casella viene visualizzato il numero esatto di volte in cui l&#39;azione è stata completata in un dato giorno. Puoi selezionare un progetto per visualizzare un raggruppamento di tali attività per ogni singolo collaboratore del progetto.

La visualizzazione di queste informazioni consente di determinare:

* L’attività relativa a un progetto specifico.
* L’attività di un progetto rispetto ad altri.
* Quali utenti stanno lavorando a un progetto e con quale frequenza.

Per scoprire come ottenere i dati migliori per questa visualizzazione, consulta [Panoramica dell’analisi migliorata](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizzazione della visualizzazione dell’attività Progetto

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. (Facoltativo) Per utilizzare un intervallo di date diverso, seleziona nuove date di inizio e di fine dal filtro dell’intervallo di date.

   ![](assets/filters-select-date-range-350x344.png)

   Per informazioni sull’utilizzo del filtro dell’intervallo di date, consulta [Applicazione di filtri in Analisi avanzata](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >Se selezioni un intervallo di date per un periodo superiore a 3 mesi, la visualizzazione dell’attività Progetto non visualizza alcun dato.

1. (Condizionale) Se devi limitare il set di dati del progetto, seleziona e applica i filtri che desideri utilizzare.

   Per ulteriori informazioni sull’aggiunta di filtri nell’analisi avanzata, consulta [Applicazione di filtri in Analisi avanzata](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Dopo aver aggiunto i filtri, vengono visualizzati i dati per un massimo di 50 progetti e i filtri rimangono attivi anche dopo aver lasciato la pagina o disconnesso da Workfront.

1. (Facoltativo) Per ingrandire un intervallo di date, seleziona un punto sulla visualizzazione per l’inizio dell’intervallo di date e trascina fino alla fine dell’intervallo di date.

   Tutte le altre visualizzazioni vengono aggiornate con lo stesso intervallo di date e viene creato un filtro per l’intervallo di tempo.

   ![](assets/timeframe-filter-350x220.png)

1. (Facoltativo) Per modificare l&#39;ordine dei progetti, fai clic sul pulsante **Ordina per** quindi selezionate una nuova opzione di ordinamento:

   * **A - Z**
   * **Z - A**
   * **Data di completamento pianificata**
   * **Data inizio pianificata**

   Tutte le altre visualizzazioni nella pagina vengono aggiornate in base alla selezione dell’ordinamento.

1. (Condizionale) Se nel set di dati sono presenti più di 50 progetti, utilizza le frecce nell’angolo in basso a sinistra della visualizzazione per passare da un gruppo di 50 progetti all’altro.

   Tutte le altre visualizzazioni nella pagina vengono aggiornate in base alla selezione della pagina.

   ![](assets/pagination-350x118.png)

1. Fai clic su un progetto nella visualizzazione per visualizzare ulteriori dettagli sul progetto.

   L’elenco si espande per visualizzare le attività di ogni singolo collaboratore nel progetto.

1. Passa il puntatore del mouse su una casella per visualizzare la data in cui gli utenti hanno completato un’azione, nonché il numero di volte in cui l’azione è stata completata per quel giorno.

   ![](assets/project-activity-activity-pop-up-350x137.png)

1. (Facoltativo) Per esportare i dati di visualizzazione, fai clic sul pulsante **Icona Esporta** ![](assets/export.png) nell’angolo in alto a destra della visualizzazione, quindi seleziona il formato di esportazione:

   * **Grafico (PNG)**
   * **Tabella dati (XSLX)**

