---
title: Visualizzazione dell’attività per team in Analisi avanzata
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualizzazione Attività per team mostra le attività che avvengono durante un intervallo di tempo specifico per un team principale, consentendoti di comprendere in che modo diversi team nazionali hanno trascorso il loro tempo in Adobe Workfront. A seconda della configurazione del team principale in Workfront, questa visualizzazione può fornire informazioni diverse e rispondere a domande diverse.
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Visualizzazione dell’attività per team in Analisi avanzata

La visualizzazione Attività per team mostra le attività che avvengono durante un intervallo di tempo specifico per un team principale, consentendoti di comprendere in che modo diversi team nazionali hanno trascorso il loro tempo in Adobe Workfront. A seconda della configurazione del team principale in Workfront, questa visualizzazione può fornire informazioni diverse e rispondere a domande diverse.

>[!NOTE]
>
>La visualizzazione delle attività Progetto è simile a questa visualizzazione, ma mostra le attività in base alle persone assegnate a progetti anziché alle persone assegnate a un team domestico.\
>Per informazioni sulla visualizzazione delle attività Progetto, consulta [Visualizzazione della visualizzazione delle attività del progetto in Analisi avanzata](../enhanced-analytics/project-activity-overview.md).

![](assets/activity-by-team-350x113.png)

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

## Visualizzazione dell’attività per team

Le diverse attività vengono visualizzate in colori diversi per riepilogare eventi specifici nel periodo di tempo filtrato:

* **Utenti connessi**: Le caselle viola mostrano che le persone del team di casa hanno effettuato l&#39;accesso quel giorno. Una tonalità più scura indica un numero maggiore di persone che accedono.

   ![](assets/project-activity-users-logged-in.png)

* **Modifica dello stato dell&#39;attività**: Le caselle rosa mostrano che le persone del team di casa hanno cambiato lo stato di un&#39;attività in quel giorno. Un&#39;ombreggiatura più scura indica un numero maggiore di stati di attività che cambiano.

   ![](assets/project-activity-task-status-changes.png)

* **Attività completate**: Le scatole blu mostrano che le persone del team di casa hanno completato un&#39;attività in quel giorno. Una tonalità più scura indica un numero maggiore di attività completate.

   ![](assets/project-activity-tasks-completed.png)

Passando il puntatore del mouse su una casella viene visualizzato il numero esatto di volte in cui l&#39;azione è stata completata in un dato giorno. Puoi selezionare un team per visualizzare un raggruppamento di queste attività da parte di ogni persona del team principale.

La visualizzazione di queste informazioni consente di determinare:

* Quali attività si verificano all’interno di un team domestico e a quale ritmo.
* Quali team domestici vengono sovraccaricati di lavoro o utilizzano di più il sistema.
* Se la distribuzione del lavoro è appropriata per la squadra di casa.

Per scoprire come ottenere i dati migliori per questa visualizzazione, consulta [Panoramica dell’analisi migliorata](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizzazione dell’attività per team

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

1. Fai clic su un nome di team

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

1. Passa il puntatore del mouse sopra una casella colorata per visualizzare la data in cui gli utenti hanno completato un’azione, nonché il numero di volte in cui l’azione è stata completata in quel giorno.

   I colori più scuri indicano un’attività più elevata.

   ![](assets/activity-by-team-activity-pop-up-350x155.png)

1. (Facoltativo) Per esportare i dati di visualizzazione, fai clic sull’icona Esporta ![](assets/export.png) nell’angolo in alto a destra della visualizzazione, quindi seleziona il formato di esportazione:

   * **Grafico (PNG)**
   * **Tabella dati (XSLX)**

