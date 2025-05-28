---
title: Visualizzare l’attività del progetto in Analisi avanzate
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualizzazione delle attività del progetto mostra una visualizzazione aggregata delle attività a livello di progetto, ovvero le attività di ogni persona assegnata al progetto, che si sono verificate in un intervallo di tempo specifico. Puoi limitare l’attenzione alla comprensione delle attività all’interno di un progetto, oppure puoi confrontare le attività di progetto con altri progetti in Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 8%

---

# Visualizzare l’attività del progetto in Analisi avanzate

>[!IMPORTANT]
>
>Analisi avanzata è stato rimosso da Workfront il 27 maggio. Workfront Data Connect è una soluzione nuova e alternativa che può essere utilizzata per replicare qualsiasi visualizzazione avanzata di Analytics attualmente in uso. <br>Per ulteriori informazioni, consulta la [Guida all&#39;obsolescenza di Enhanced Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md).


<!-- Audited: 12/2023 -->

La visualizzazione delle attività del progetto mostra una visualizzazione aggregata delle attività a livello di progetto, ovvero le attività di ogni persona assegnata al progetto, che si sono verificate in un intervallo di tempo specifico. Puoi limitare l’attenzione alla comprensione delle attività all’interno di un progetto, oppure puoi confrontare le attività di progetto con altri progetti in Adobe Workfront.

>[!NOTE]
>
>La visualizzazione Attività per team si comporta in modo simile a questa, ma la visualizzazione Attività per team mostra l’attività del team principale per tutti i progetti.\
>Per informazioni sulla visualizzazione Attività per team, consulta [Visualizzazione Attività per team in Analisi avanzate](../enhanced-analytics/activity-by-team-overview.md).

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">piano Workfront</a></td> 
   <td> <p>Business o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica sulle licenze di Adobe Workfront</a></td> 
   <td>   <p>Nuovo:</p> 
   <ul><li>Light o Higher</li></ul>
   <p>Corrente:</p>
   <ul><li>Revisione o superiore</li></ul>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso ai progetti in visualizzazione</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisiti

Per i prerequisiti per l&#39;utilizzo di Analisi avanzate, vedere la sezione &quot;Prerequisiti&quot; in [Panoramica di Analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprendere la visualizzazione delle attività del progetto

Le attività del progetto vengono visualizzate in colori diversi per riepilogare eventi specifici in un progetto in un determinato periodo di tempo:

* **Utenti connessi**: le caselle viola mostrano che gli utenti assegnati al progetto hanno effettuato l&#39;accesso in quel giorno. Una tonalità più scura indica un numero maggiore di utenti che effettuano l’accesso.

  ![Utenti connessi](assets/project-activity-users-logged-in.png)

* **Modifica stato attività**: le caselle di colore rosa indicano che in quel giorno le persone hanno modificato lo stato di un&#39;attività per il progetto. Una tonalità più scura indica un numero maggiore di cambiamenti di stati delle attività.

  ![Modifica stato attività](assets/project-activity-task-status-changes.png)

* **Attività completate**: le caselle blu indicano che le persone hanno completato un&#39;attività per il progetto. Una tonalità più scura indica un numero maggiore di attività completate.

  ![Attività completate](assets/project-activity-tasks-completed.png)

Passando il puntatore del mouse su una casella viene visualizzato il numero esatto di volte in cui l’azione è stata completata in un dato giorno. Puoi selezionare un progetto per visualizzare un raggruppamento di queste attività per ogni singolo collaboratore del progetto.

La visualizzazione di queste informazioni consente di determinare:

* L’attività su un progetto specifico.
* L’attività di un progetto rispetto ad altri progetti.
* Quali utenti stanno lavorando a un progetto e con quale frequenza.

Per informazioni su come ottenere i dati migliori per questa visualizzazione, consulta [Panoramica sulle analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizzare l’attività Progetto

1. Fai clic sull&#39;icona del menu principale ![icona del menu principale](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. (Facoltativo) Per utilizzare un intervallo di date diverso, seleziona nuove date di inizio e fine dal filtro dell’intervallo di date.

   ![Seleziona intervallo date](assets/filters-select-date-range-350x344.png)

   Per informazioni sull&#39;utilizzo del filtro dell&#39;intervallo di date, vedere [Applicare filtri in Analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >Se selezioni un intervallo di date per un periodo superiore a 3 mesi, nella visualizzazione dell’attività di Project non vengono visualizzati dati.

1. (Condizionale) Se devi limitare il set di dati del progetto, seleziona e applica i filtri che desideri utilizzare.

   Per ulteriori informazioni sull&#39;aggiunta di filtri in Analisi avanzate, vedere [Applicare filtri in Analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Dopo aver aggiunto i filtri, vengono visualizzati i dati per un massimo di 50 progetti e i filtri rimangono attivi anche dopo che hai lasciato la pagina o disconnesso da Workfront.

1. (Facoltativo) Per ingrandire un intervallo di date, seleziona un punto nella visualizzazione per l’inizio dell’intervallo di date e trascina fino alla fine dell’intervallo di date.

   Tutte le altre visualizzazioni vengono aggiornate allo stesso intervallo di date e viene creato un filtro per l’intervallo di tempo.

   ![Filtro intervallo di tempo](assets/timeframe-filter-350x220.png)

1. (Facoltativo) Per modificare l&#39;ordinamento dei progetti, fare clic sul menu **Ordina per**, quindi selezionare una nuova opzione di ordinamento:

   * **A - Z**
   * **Z - A**
   * **Data di completamento pianificata**
   * **Data inizio pianificata**

   Tutte le altre visualizzazioni nella pagina vengono aggiornate in base alla selezione dell’ordinamento.

1. (Facoltativo) Se nel set di dati sono presenti più di 50 progetti, utilizza le frecce nell’angolo in basso a sinistra della visualizzazione per passare da un gruppo di 50 progetti all’altro.

   Tutte le altre visualizzazioni nella pagina vengono aggiornate in base alla selezione della pagina.

   ![Paginazione](assets/pagination-350x118.png)

1. Fai clic su un progetto nella visualizzazione per visualizzare ulteriori dettagli relativi al progetto.

   L’elenco si espande per visualizzare le attività di ogni singolo collaboratore sul progetto.

1. Passa il puntatore del mouse su una casella per vedere la data in cui gli utenti hanno completato un&#39;azione, nonché il numero di volte in cui l&#39;azione è stata completata per quel giorno.

   ![Popup attività](assets/project-activity-activity-pop-up-350x137.png)

1. (Facoltativo) Per esportare i dati di visualizzazione, fai clic sull&#39;**icona Esporta** ![icona Esporta](assets/export.png) nell&#39;angolo in alto a destra della visualizzazione, quindi seleziona il formato di esportazione:

   * **Grafico (PNG)**
   * **Tabella dati (XSLX)**

