---
title: Visualizzare la visualizzazione Attività per team in Analisi avanzate
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualizzazione Attività per team mostra le attività che avvengono durante un intervallo di tempo specifico per un team principale, consentendoti di comprendere come diversi team principali hanno trascorso il loro tempo in Adobe Workfront. A seconda di come è configurato il tuo team principale in Workfront, questa visualizzazione può fornirti informazioni diverse e rispondere a domande diverse.
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 325334010d5f1206931cc9ace67f9511d614ffca
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 7%

---

# Visualizzare la visualizzazione Attività per team in Analisi avanzate

<!-- Audited: 12/2023 -->

La visualizzazione Attività per team mostra le attività che avvengono durante un intervallo di tempo specifico per un team principale, consentendoti di comprendere come diversi team principali hanno trascorso il loro tempo in Adobe Workfront. A seconda di come è configurato il tuo team principale in Workfront, questa visualizzazione può fornirti informazioni diverse e rispondere a domande diverse.

>[!NOTE]
>
>La visualizzazione delle attività del progetto è simile a questa, ma mostra le attività in base alle persone assegnate ai progetti anziché alle persone assegnate a un team principale.\
>Per informazioni sulla visualizzazione delle attività del progetto, vedi [Visualizzare la visualizzazione delle attività del progetto in Analisi avanzate](../enhanced-analytics/project-activity-overview.md).

![Attività per team](assets/activity-by-team-350x113.png){width="700"}

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

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
   <td>
      <p>Nuovo:</p> 
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

+++

## Prerequisiti

Per i prerequisiti per l&#39;utilizzo di Analisi avanzate, vedere la sezione &quot;Prerequisiti&quot; in [Panoramica di Analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizzazione Attività per team

Le diverse attività vengono visualizzate in colori diversi per riepilogare eventi specifici nel periodo di tempo filtrato:

* **Utenti connessi**: le caselle viola mostrano che gli utenti del team principale hanno effettuato l&#39;accesso in quel giorno. Una tonalità più scura indica un numero maggiore di utenti che effettuano l’accesso.

  ![Utenti connessi](assets/project-activity-users-logged-in.png)

* **Modifica stato attività**: le caselle di colore rosa indicano che gli utenti del team principale hanno modificato lo stato di un&#39;attività in quel giorno. Una tonalità più scura indica un numero maggiore di cambiamenti di stati delle attività.

  ![Modifiche stato attività](assets/project-activity-task-status-changes.png)

* **Attività completate**: le caselle blu indicano che le persone nel team principale hanno completato un&#39;attività in quel giorno. Una tonalità più scura indica un numero maggiore di attività completate.

  ![Attività completate](assets/project-activity-tasks-completed.png)

Passando il puntatore del mouse su una casella viene visualizzato il numero esatto di volte in cui l’azione è stata completata in un dato giorno. Puoi selezionare un team per visualizzare un raggruppamento di queste attività per ogni persona nel team principale.

La visualizzazione di queste informazioni consente di determinare:

* Quali attività si verificano all’interno di un team interno e a quale ritmo.
* Quali sono i team principali che sono sovraccarichi di lavoro o utilizzano di più il sistema.
* Se la distribuzione del lavoro è appropriata per il team predefinito.

Per informazioni su come ottenere i dati migliori per questa visualizzazione, consulta [Panoramica sulle analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizzazione Attività per team

1. Fai clic sull&#39;icona del menu principale ![icona del menu principale](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. Nel pannello a sinistra, seleziona **Persone**.

   ![Area persone](assets/people-area-cropped-qs-350x276.png)

1. (Facoltativo) Per utilizzare un intervallo di date diverso, seleziona nuove date di inizio e fine dal filtro dell’intervallo di date.

   ![Seleziona intervallo date](assets/filters-select-date-range-350x344.png)

   Per informazioni sull&#39;utilizzo del filtro dell&#39;intervallo di date, vedere [Applicare filtri in Analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condizionale) Se non hai impostato il filtro Team, aggiungi il filtro Team e seleziona ogni team per il quale desideri visualizzare i dati.

   Per ulteriori informazioni sull&#39;aggiunta di filtri in Analisi avanzate, vedere [Applicare filtri in Analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Dopo aver aggiunto i filtri, vengono visualizzati i dati per un massimo di 50 progetti e i filtri rimangono attivi anche dopo che hai lasciato la pagina o disconnesso da Workfront.

1. (Facoltativo) Per ingrandire un intervallo di date, seleziona un punto nella visualizzazione per l’inizio dell’intervallo di date e trascina fino alla fine dell’intervallo di date.

   Tutte le altre visualizzazioni vengono aggiornate allo stesso intervallo di date e viene creato un filtro per l’intervallo di tempo.

   ![Filtro intervallo di tempo](assets/timeframe-filter-350x220.png)

1. Fai clic sul nome di un team

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   per visualizzare ulteriori dettagli sulle attività completate dal team principale.

   L’elenco si espande per visualizzare le attività di ogni persona assegnata al team principale.

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. Passa il puntatore del mouse su una casella colorata per visualizzare la data in cui gli utenti hanno completato un’azione e il numero di volte in cui l’azione è stata completata quel giorno.

   I colori più scuri indicano un’attività più elevata.

   ![Attività per team](assets/activity-by-team-activity-pop-up-350x155.png)

1. (Facoltativo) Per esportare i dati della visualizzazione, fai clic sull&#39;icona Esporta ![icona Esporta](assets/export.png) nell&#39;angolo in alto a destra della visualizzazione, quindi seleziona il formato di esportazione:

   * **Grafico (PNG)**
   * **Tabella dati (XSLX)**

