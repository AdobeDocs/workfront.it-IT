---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: Visualizzare la mappa ad albero del progetto in Analisi avanzate
description: La visualizzazione Mappa ad albero progetto è una visualizzazione delle ore, o giorni, lavorate in una specifica finestra di tempo rispetto ad altre attività lavorative per dimensioni. Questo ti aiuta a capire quanto tempo le persone si sono dedicate a un progetto.
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 325334010d5f1206931cc9ace67f9511d614ffca
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 2%

---

# Visualizzare la mappa ad albero del progetto in Analisi avanzate

<!-- Audited: 12/2023 -->

La visualizzazione Mappa ad albero progetto è una visualizzazione delle ore, o giorni, lavorate in una specifica finestra di tempo rispetto ad altre attività lavorative per dimensioni. Questo ti aiuta a capire quanto tempo le persone si sono dedicate a un progetto.

![Mappa ad albero progetto](assets/project-treemap-350x126.png){width="700"}

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">piano Adobe Workfront</a></td> 
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

+++

## Prerequisiti

Per i prerequisiti per l&#39;utilizzo di Analisi avanzate, vedere la sezione &quot;Prerequisiti&quot; in [Panoramica di Analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprendere la visualizzazione Mappa ad albero progetto

Le caselle nella visualizzazione Mappa ad albero Progetto rappresentano i progetti e le dimensioni delle caselle mostrano un confronto tra la quantità di tempo trascorso su progetti diversi. Più grande è la casella, maggiore è il tempo trascorso sul progetto.

La visualizzazione Mappa ad albero Progetto è composta da:

* **Caselle blu chiaro più piccole**: i progetti con un numero inferiore di ore o giorni vengono visualizzati come caselle più piccole con un colore blu chiaro.

  ![Scatola più piccola](assets/project-treemap-smaller-box.png)

* **Caselle blu più grandi e scure**: i progetti con più ore o giorni vengono visualizzati come caselle più grandi con un colore blu scuro.

  ![Casella più grande](assets/project-treemap-larger-box-350x205.png)

* **Caselle blu di dimensioni Medium**: i progetti compresi tra le due categorie vengono visualizzati come caselle di medie dimensioni con una sfumatura blu tra i colori blu scuro e blu chiaro. Ci sono 3 possibili sfumature di blu per le scatole di medie dimensioni.

La legenda a destra mostra un raggruppamento di ore completate per ogni tonalità di blu. Questa legenda è dinamica e si aggiorna in base ai dati.

![Ore mappa ad albero completate](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>Se osservi la visualizzazione Mappa ad albero del progetto per durata anziché per ore pianificate, questa legenda mostra un raggruppamento dei giorni di lavoro per ogni tonalità di blu.\
>![Giorni mappa ad albero lavorati](assets/project-treemap-days-worked.png)>

La visualizzazione di queste informazioni consente di determinare:

* La priorità degli elementi su cui si sta lavorando durante l’intervallo di date selezionato.
* Quali team trascorrono il tempo a disposizione.
* Se i team si concentrano sulle cose giuste.
* Quando si fa clic su un progetto specifico, quanto l’ambito di un progetto è cambiato in quel periodo di tempo.

Per informazioni su come ottenere i dati migliori per questa visualizzazione, consulta [Panoramica sulle analisi avanzate](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizzare la mappa ad albero del progetto

1. Fai clic sull&#39;icona del menu principale ![icona del menu principale](assets/main-menu-icon-16x12.png), quindi seleziona **Analytics**.
1. (Facoltativo) Per utilizzare un intervallo di date diverso, seleziona nuove date di inizio e fine dal filtro dell’intervallo di date.

   ![Seleziona intervallo date](assets/filters-select-date-range-350x344.png)

   Per informazioni sull&#39;utilizzo del filtro dell&#39;intervallo di date, vedere [Applicare filtri in Analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condizionale) Se devi limitare il set di dati del progetto, seleziona e applica i filtri che desideri utilizzare.

   Per ulteriori informazioni sull&#39;aggiunta di filtri in Analisi avanzate, vedere [Applicare filtri in Analisi avanzate](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Dopo aver aggiunto i filtri, vengono visualizzati i dati per un massimo di 50 progetti e i filtri rimangono attivi anche dopo che hai lasciato la pagina o disconnesso da Workfront.

1. (Facoltativo) Per modificare l&#39;ordinamento dei progetti, fai clic sul menu **Ordina per** nell&#39;angolo superiore destro della visualizzazione Mappa ad albero progetto, quindi seleziona una nuova opzione di ordinamento:

   * **A - Z**
   * **Z - A**
   * **Data di completamento pianificata**
   * **Data inizio pianificata**

   Tutte le altre visualizzazioni nella pagina vengono aggiornate in base alla selezione dell’ordinamento.

1. (Facoltativo) Se nel set di dati sono presenti più di 50 progetti, utilizza le frecce nell’angolo in basso a sinistra della visualizzazione per passare da un gruppo di 50 progetti all’altro.

   Tutte le altre visualizzazioni nella pagina vengono aggiornate in base alla selezione della pagina.

   ![Paginazione](assets/pagination-350x118.png)

1. (Facoltativo) Cambia la visualizzazione da **ore pianificate** a **durata**.

   L’opzione Ore pianificate è selezionata per impostazione predefinita.

1. Passa il cursore del mouse su un progetto per vedere la condizione del progetto, il numero di ore pianificate totali, il numero di ore completate totali e il numero medio di ore dedicate al progetto al giorno.

   ![Dettagli progetto mappa ad albero](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >Se hai selezionato la visualizzazione **duration**, visualizzerai i seguenti dettagli sulla durata:
   >
   >* **Intervallo temporale pianificato**: il numero di giorni pianificati per il completamento del progetto.
   >* **Giorni di lavoro**: la durata pianificata per ogni attività completata entro l&#39;intervallo di date selezionato nella parte superiore, divisa per il numero di ore in un giorno.
   >   
   >![Durata mappa ad albero](assets/duration-treemap-350x159.png)
   >
   >Per ulteriori informazioni sulla durata, consulta la sezione &quot;Visualizzazione durata&quot; in [Panoramica analisi avanzata](../enhanced-analytics/enhanced-analytics-overview.md).

1. (Facoltativo) Per esportare i dati di visualizzazione, fai clic sull&#39;**icona Esporta** ![icona Esporta](assets/export.png) nell&#39;angolo in alto a destra della visualizzazione, quindi seleziona il formato di esportazione:

   * **Grafico (PNG)**
   * **Tabella dati (XSLX)**

1. Fai clic su un progetto per aprire le visualizzazioni Burndown e Attività in volo e ottenere informazioni più approfondite su come le attività e le ore, o i giorni, hanno contribuito alla dimensione di un progetto.

Per ulteriori informazioni sulla visualizzazione Burndown, consulta [Visualizzare la visualizzazione Burndown in Analisi avanzate](../enhanced-analytics/burndown-overview.md). Per ulteriori informazioni sulla visualizzazione Attività in volo, consulta [Visualizzare la visualizzazione Attività in volo in Analisi avanzate](../enhanced-analytics/tasks-in-flight-overview.md).

