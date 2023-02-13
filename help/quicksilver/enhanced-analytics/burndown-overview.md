---
title: Visualizzare la visualizzazione a discesa in Analisi avanzata
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualizzazione a discesa mostra il raggruppamento di un progetto specifico nel tempo e ti aiuta a comprendere il rapporto tra la condizione del progetto, la velocità e le ore rimanenti, o i giorni.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: d337008d4fca8c41b98b10f9059ec1cc379811e1
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---

# Visualizzare la visualizzazione a discesa in Analisi avanzata

La visualizzazione a discesa mostra il raggruppamento di un progetto specifico nel tempo e ti aiuta a comprendere il rapporto tra la condizione del progetto, la velocità e le ore rimanenti, o i giorni.

![](assets/burndown-350x112.png)

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

## Comprendere la visualizzazione a discesa

La linea blu continua mostra la velocità pianificata dalla data di inizio alla data di completamento pianificata. Questa linea si regola quando il lavoro viene aggiunto, rimosso o aggiornato e diventa una linea verticale tratteggiata quando il progetto raggiunge la data di completamento pianificata.

![](assets/burndown-planned-line.png)

La riga effettiva mostra il numero di ore o giorni trascorsi nel progetto nel tempo. Il colore di questa linea indica ogni giorno la condizione del progetto:

* **Verde**: Il progetto è in target.

   ![](assets/burndown-green.png)

* **Arancio**: Il progetto è a rischio.

   ![](assets/burndown-orange.png)

* **Rosso**: Il progetto è nei guai.

   ![](assets/burndown-red.png)

Per ulteriori informazioni su queste condizioni del progetto, consulta [Panoramica del tipo di condizione e condizione del progetto](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Quando la linea effettiva si sposta in verticale, il lavoro è stato aggiunto al progetto. Quando la linea si sposta verso il basso in verticale, il lavoro è stato rimosso o completato per il progetto.

Sotto l’asse x della visualizzazione, puoi visualizzare ulteriori informazioni sulla modifica delle attività e delle ore (o dei giorni) in un dato giorno (la quantità aggiunta, la quantità completata e la differenza tra i due).

La visualizzazione di tutte queste informazioni nella visualizzazione a discesa consente di determinare:

* La salute del singolo progetto nel tempo
* Come i problemi in arrivo (o lavoro non pianificato) hanno influenzato il lavoro pianificato.
* Quali eventi hanno esteso il progetto oltre la data di completamento originale.

Per scoprire come ottenere i dati migliori per questa visualizzazione, consulta [Panoramica dell’analisi migliorata](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizzare la visualizzazione a discesa

1. Fai clic sull’icona Menu principale ![](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. (Facoltativo) Per utilizzare un intervallo di date diverso, seleziona nuove date di inizio e di fine dal filtro dell’intervallo di date.

   ![](assets/filters-select-date-range-350x344.png)

   Per informazioni sull’utilizzo del filtro dell’intervallo di date, consulta [Applicazione di filtri in Analisi avanzata](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condizionale) Se devi limitare il set di dati del progetto, seleziona e applica i filtri che desideri utilizzare.

   Per ulteriori informazioni sull’aggiunta di filtri nell’analisi avanzata, consulta [Applicazione di filtri in Analisi avanzata](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Dopo aver aggiunto i filtri, vengono visualizzati i dati per un massimo di 50 progetti e i filtri rimangono attivi anche dopo aver lasciato la pagina o disconnesso da Workfront.

1. (Facoltativo) Per ingrandire un intervallo di date, seleziona un punto sulla visualizzazione per l’inizio dell’intervallo di date e trascina fino alla fine dell’intervallo di date.

   Tutte le altre visualizzazioni vengono aggiornate con lo stesso intervallo di date e viene creato un filtro per l’intervallo di tempo.

   ![](assets/timeframe-filter-350x220.png)

1. Nella visualizzazione del piano di volo o della mappa ad albero del progetto, fai clic su un progetto per visualizzare ulteriori informazioni.

   Vengono visualizzate le visualizzazioni Burndown e Attività in volo .

   >[!NOTE]
   >
   >Per ulteriori informazioni su queste altre visualizzazioni, consulta:
   >
   >   
   >   
   >   * [Visualizzazione della visualizzazione del piano di volo in Analisi avanzata](../enhanced-analytics/flight-plan-overview.md)
   >   * [Visualizzare la visualizzazione della mappa del percorso del progetto in Analisi avanzata](../enhanced-analytics/project-treemap-overview.md)
   >   * [Visualizzazione delle attività nella visualizzazione dei voli in Enhanced analytics](../enhanced-analytics/tasks-in-flight-overview.md)


1. (Facoltativo) Cambia la visualizzazione da ore pianificate a **durata**.

   L’opzione Orari pianificati è selezionata per impostazione predefinita.

   >[!NOTE]
   >
   >Selezione **durata** cambia tutte le informazioni sulle ore in giorni.\
   >![](assets/duration-burndown-350x112.png)\
   >Per ulteriori informazioni sulla durata nell’area Analisi avanzata, consulta la sezione &quot;Vista a tempo&quot; in [Panoramica dell’analisi migliorata](../enhanced-analytics/enhanced-analytics-overview.md).

1. Fai clic su un punto qualsiasi del grafico a linee.

   Di seguito sono visualizzate la data esatta e ulteriori informazioni sulle attività e le ore (o i giorni) per il giorno selezionato.

   ![](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >Se la velocità effettiva è una linea piatta che viene eseguita lungo l’asse x (in linea con 0 ore o 0 giorni) della visualizzazione, significa che non sono state aggiunte al progetto ore o giorni pianificati.\
   >Se la velocità effettiva è una linea piatta sopra l&#39;asse x (in linea con un numero di ore o un numero di giorni) che non si abbassa mai, ciò significa che nessuna attività è stata completata entro il periodo di tempo filtrato.

1. (Facoltativo) Per esportare i dati di visualizzazione, fai clic sul pulsante **Esporta** icona ![](assets/export.png)nell’angolo in alto a destra della visualizzazione, quindi seleziona il formato di esportazione:

   * **Grafico (PNG)**
   * **Tabella dati (XSLX)**

1. (Facoltativo) Per visualizzare i dettagli sull’avanzamento delle attività nel progetto selezionato, osserva la visualizzazione Attività in volo visualizzata sotto la visualizzazione a discesa.
