---
title: Visualizzare l’attività del progetto in Analisi avanzate
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualizzazione delle attività del progetto mostra una visualizzazione aggregata delle attività a livello di progetto, ovvero le attività di ogni persona assegnata al progetto, che si sono verificate in un intervallo di tempo specifico. Puoi limitare l’attenzione alla comprensione delle attività all’interno di un progetto, oppure puoi confrontare le attività di progetto con altri progetti in Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# Visualizzare l’attività del progetto in Analisi avanzate

<!-- Audited: 12/2023 -->

La visualizzazione delle attività del progetto mostra una visualizzazione aggregata delle attività a livello di progetto, ovvero le attività di ogni persona assegnata al progetto, che si sono verificate in un intervallo di tempo specifico. Puoi limitare l’attenzione alla comprensione delle attività all’interno di un progetto, oppure puoi confrontare le attività di progetto con altri progetti in Adobe Workfront.

>[!NOTE]
>
>La visualizzazione Attività per team si comporta in modo simile a questa, ma la visualizzazione Attività per team mostra l’attività del team principale per tutti i progetti.\
>Per informazioni sulla visualizzazione Attività per team, consulta [Visualizzare la visualizzazione Attività per team in Analisi avanzate](../enhanced-analytics/activity-by-team-overview.md).

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">piano Workfront</a></td> 
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

Per i prerequisiti per utilizzare Enhanced Analytics, consulta la sezione &quot;Prerequisiti&quot; in [Panoramica di analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprendere la visualizzazione delle attività del progetto

Le attività del progetto vengono visualizzate in colori diversi per riepilogare eventi specifici in un progetto in un determinato periodo di tempo:

* **Utenti connessi**: le caselle viola mostrano che le persone assegnate al progetto hanno effettuato l’accesso in quel giorno. Un&#39;ombreggiatura più scura indica un numero maggiore di utenti che accedono.

  ![](assets/project-activity-users-logged-in.png)

* **Modifica stato attività**: le caselle rosa mostrano che in quel giorno gli utenti hanno modificato lo stato di un’attività per il progetto. Un&#39;ombreggiatura più scura indica un numero maggiore di stati delle attività che cambiano.

  ![](assets/project-activity-task-status-changes.png)

* **Attività completate**: le caselle blu mostrano che le persone hanno completato un’attività per il progetto. Un&#39;ombreggiatura più scura indica un numero maggiore di attività completate.

  ![](assets/project-activity-tasks-completed.png)

Passando il puntatore del mouse su una casella viene visualizzato il numero esatto di volte in cui l’azione è stata completata in un dato giorno. Puoi selezionare un progetto per visualizzare un raggruppamento di queste attività per ogni singolo collaboratore del progetto.

La visualizzazione di queste informazioni consente di determinare:

* L’attività su un progetto specifico.
* L’attività di un progetto rispetto ad altri progetti.
* Quali utenti stanno lavorando a un progetto e con quale frequenza.

Per scoprire come ottenere i dati migliori per questa visualizzazione, consulta [Panoramica di analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizzare l’attività Progetto

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. (Facoltativo) Per utilizzare un intervallo di date diverso, seleziona nuove date di inizio e fine dal filtro dell’intervallo di date.

   ![](assets/filters-select-date-range-350x344.png)

   Per informazioni sull’utilizzo del filtro per intervalli di date, consulta [Applicare i filtri nelle analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >Se selezioni un intervallo di date per un periodo superiore a 3 mesi, nella visualizzazione dell’attività di Project non vengono visualizzati dati.

1. (Condizionale) Se devi limitare il set di dati del progetto, seleziona e applica i filtri che desideri utilizzare.

   Per ulteriori informazioni sull’aggiunta di filtri in Analisi avanzate, consulta [Applicare i filtri nelle analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Dopo aver aggiunto i filtri, vengono visualizzati i dati per un massimo di 50 progetti e i filtri rimangono attivi anche dopo che hai lasciato la pagina o disconnesso da Workfront.

1. (Facoltativo) Per ingrandire un intervallo di date, seleziona un punto nella visualizzazione per l’inizio dell’intervallo di date e trascina fino alla fine dell’intervallo di date.

   Tutte le altre visualizzazioni vengono aggiornate allo stesso intervallo di date e viene creato un filtro per l’intervallo di tempo.

   ![](assets/timeframe-filter-350x220.png)

1. (Facoltativo) Per modificare l’ordinamento dei progetti, fai clic sul pulsante **Ordina per** , quindi selezionare una nuova opzione di ordinamento:

   * **A - Z**
   * **Z - A**
   * **Data di completamento pianificata**
   * **Data di inizio pianificata**

   Tutte le altre visualizzazioni nella pagina vengono aggiornate in base alla selezione dell’ordinamento.

1. (Facoltativo) Se nel set di dati sono presenti più di 50 progetti, utilizza le frecce nell’angolo in basso a sinistra della visualizzazione per passare da un gruppo di 50 progetti all’altro.

   Tutte le altre visualizzazioni nella pagina vengono aggiornate in base alla selezione della pagina.

   ![](assets/pagination-350x118.png)

1. Fai clic su un progetto nella visualizzazione per visualizzare ulteriori dettagli relativi al progetto.

   L’elenco si espande per visualizzare le attività di ogni singolo collaboratore sul progetto.

1. Passa il puntatore del mouse su una casella per vedere la data in cui gli utenti hanno completato un&#39;azione, nonché il numero di volte in cui l&#39;azione è stata completata per quel giorno.

   ![](assets/project-activity-activity-pop-up-350x137.png)

1. (Facoltativo) Per esportare i dati di visualizzazione, fai clic sul pulsante **Icona Esporta** ![](assets/export.png) nell’angolo in alto a destra della visualizzazione, seleziona il formato di esportazione:

   * **Grafico (PNG)**
   * **Tabella dati (XSLX)**

