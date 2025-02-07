---
title: Panoramica di analisi avanzate
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Le funzioni di analisi avanzate sono uno strumento potente di Adobe Workfront con visualizzazioni predefinite che consentono di esaminare i dati dei progetti e identificare le tendenze con la pianificazione e il completamento. Questo approfondimento sui tuoi progetti ti aiuta a gestire il lavoro corrente e ti consente di pianificare in modo più accurato il lavoro futuro.
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 325334010d5f1206931cc9ace67f9511d614ffca
workflow-type: tm+mt
source-wordcount: '1204'
ht-degree: 3%

---

# Panoramica di analisi avanzate

Le funzioni di analisi avanzate sono uno strumento potente di Adobe Workfront con visualizzazioni predefinite che consentono di esaminare i dati dei progetti e identificare le tendenze con la pianificazione e il completamento. Questo approfondimento sui tuoi progetti ti aiuta a gestire il lavoro corrente e ti consente di pianificare in modo più accurato il lavoro futuro.

Le funzioni di analisi avanzate consentono di identificare:

* Il modo in cui pianifichi i progetti
* Quando il lavoro viene aggiunto ai progetti
* Quantità di lavoro completata per diversi progetti
* La quantità di ore o giorni necessari per completare un progetto rispetto alle ore o ai giorni pianificati da un team interno
* Frequenza con cui gli utenti completano azioni specifiche durante un progetto
* Avanzamento dei progetti e singole attività all’interno di un progetto

![Analytics](assets/nwe-full-screen-analytics-350x222.png)

Per visualizzare i casi d&#39;uso o per ulteriori informazioni sulla gestione del lavoro corrente e sulla pianificazione per il lavoro futuro con le analisi avanzate, consulta [Percorsi di apprendimento delle analisi avanzate](https://one.workfront.com/s/enhanced-analytics-program).

## Prerequisiti

Per accedere all’area Analisi avanzata, è necessario:

* Avere un piano aziendale o aziendale.

  Per ulteriori informazioni, vedere [Piani Workfront](https://www.workfront.com/plans).

* Chiedi all’amministratore di Workfront di aggiungere analisi avanzate al modello di layout.

  Per ulteriori informazioni, vedere [Analisi avanzate: aggiunta di analisi ai modelli di layout](https://one.workfront.com/s/managed-content-videos/enhanced-analytics-adding-analytics-to-layout-templates-MCH7URDSIXRREHHHF7TRTYYP2LTE).

Per visualizzare le informazioni relative ai progetti e alle attività, è necessario:

* Disporre dell&#39;autorizzazione Visualizzazione per le aree Progetti e Attività nel proprio livello di accesso.

  Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta [Creare o modificare livelli di accesso personalizzati](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Disporre dell&#39;autorizzazione Visualizzazione per attività e/o progetti specifici.

  Per informazioni sulla richiesta di accesso aggiuntivo, vedere [Richiedere l&#39;accesso agli oggetti](../workfront-basics/grant-and-request-access-to-objects/request-access.md).

## Best practice per l’analisi avanzata

Per ottenere i dati migliori per i progetti, utilizza modelli che prevedano ore e giorni di durata pianificati in modo accurato. È inoltre necessario assicurarsi che gli utenti immettano e aggiornino i campi sottostanti nel modo più accurato possibile.

>[!NOTE]
>
>Alcuni dei campi seguenti sono calcoli eseguiti da Workfront in base alle informazioni immesse dagli utenti. Non è possibile aggiornare manualmente questi campi.

* Lavoro Necessario

  Questo è il campo più importante da compilare.

  >[!NOTE]
  >
  >Se i team non utilizzano le ore pianificate, puoi comunque visualizzare alcuni dati in base alla durata del progetto.\
  >Per ulteriori informazioni, vedere la sezione [Visualizzazione durata](#duration-view) in questo articolo.

* Nome progetto

  Il nome deve essere descrittivo del progetto.

* Condizione progetto
* Stato Progetto
* Data inizio pianificata del progetto
* Data di completamento Pianificata
* Data di inizio effettiva del progetto
* Data di completamento effettiva del progetto
* Ore durata progetto
* Ore effettive progetto
* Stato attività (contrassegno delle attività completate incluso).
* Nome attività
* Percentuale di completamento attività
* Data di inizio attività pianificata
* Data Pianificata completamento Attività

>[!IMPORTANT]
>
>La visualizzazione delle modifiche apportate ad attività e progetti in Analisi avanzate può richiedere fino a 24 ore.

## Vista Durata {#duration-view}

Per impostazione predefinita, le visualizzazioni Burndown e Mappa ad albero Progetto sono basate sulle ore pianificate. Se i team non utilizzano ore pianificate, puoi guardare queste visualizzazioni in base alla durata del progetto.

In Analisi avanzate, la durata di un progetto viene calcolata con le seguenti formule:

* Intervallo temporale pianificato:

  ```
  Planned Completion Date of the project - Start Date of the project
  ```

* Giorni lavorati:

  ```
  Planned Duration for tasks completed in the selected date range / Typical hours per work day
  ```

  >[!NOTE]
  >
  >8 ore è il numero predefinito per **Ore tipiche per giorno lavorativo**. Un amministratore Adobe Workfront può aggiornare l&#39;impostazione **Ore tipiche per giorno lavorativo** in **Configurazione** > **Preferenze progetto** > **Progetti** > **Timeline**.\
  >Per ulteriori informazioni, consulta [Configurare le preferenze di progetto a livello di sistema](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Per informazioni sulla durata pianificata, vedere [Panoramica sulla durata del progetto](../manage-work/projects/planning-a-project/project-duration.md).

## Scelte rapide da tastiera

Puoi utilizzare i seguenti tasti sulla tastiera per navigare o completare azioni specifiche nell’area Analisi avanzata:

| Chiave | Azione |
|---|---|
| **Scheda** | Passa a ogni elemento della pagina, nonché a una tabella con informazioni su ogni visualizzazione che non viene visualizzata nella pagina |
| **Invio** | Apri il widget del calendario, elimina un filtro esistente, apri le opzioni Aggiungi filtro, seleziona/deseleziona i valori del filtro, applica un filtro creato, apri le opzioni di esportazione su ciascuna visualizzazione, apri i menu a discesa sulle visualizzazioni Burndown, Attività in volo e Mappa ad albero progetto |
| **Tasti di direzione** | Passa alle date nel widget del calendario, alle opzioni filtro quando si aggiunge un filtro e alle opzioni in tutti i menu a discesa nelle visualizzazioni |
| **Barra spaziatrice** | Seleziona le date nel widget del calendario, seleziona un tipo di filtro quando aggiungi un filtro, seleziona un’opzione di esportazione dal menu a discesa in ogni visualizzazione e seleziona le opzioni dai menu a discesa nelle visualizzazioni Burndown, Attività in volo e Mappa ad albero progetto |

{style="table-layout:auto"}

Se si utilizza un software per la lettura dello schermo o un plug-in, l&#39;assistente vocale legge le informazioni sullo schermo ad alta voce e descrive le azioni che si stanno completando quando si utilizzano i tasti elencati sopra.

## Visualizzazioni e funzioni di analisi migliorate

Per ulteriori informazioni sui dettagli di una funzione specifica in Analisi avanzate, sulle azioni che puoi completare per ottenere ulteriori informazioni e su cosa puoi imparare da questi dati, consulta i seguenti articoli:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Articolo</th> 
   <th>Spiegazione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Applicare filtri in analisi avanzate</a> </td> 
   <td> <p>Puoi applicare filtri personalizzati, filtri dei campi del progetto o filtri del team per visualizzare solo i progetti che soddisfano criteri specifici. Quando aggiungi dei filtri, il numero di progetti viene aggiornato di conseguenza.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">Comprendere i KPI di analisi avanzata</a> </td> 
   <td> <p>Nella parte superiore dello schermo sono riportati gli indicatori di prestazioni chiave (KPI, Key Performance Indicators) di tutti i progetti entro un intervallo di tempo specifico.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">Visualizzazione del piano di volo in Analisi avanzate</a> </p> </td> 
   <td> <p>La visualizzazione del <b>piano di volo</b> mostra che la condizione è cambiata nel corso della durata di un progetto. L’interazione con la visualizzazione ti fornisce ulteriori dettagli su date specifiche. Selezionando un progetto si aprono le visualizzazioni Burndown e Tasks in flight.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">Visualizzazione Burndown in Analisi avanzate</a> </td> 
   <td> <p>La visualizzazione <b>Burndown</b> mostra la velocità pianificata di un progetto rispetto alla quantità effettiva di ore dedicate a un progetto. L’interazione con la visualizzazione ti fornisce ulteriori dettagli sulle condizioni del progetto in una data specifica.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">Visualizza le Attività nella visualizzazione di volo in Analisi avanzate</a> </td> 
   <td> <p>La visualizzazione <b>Attività in corso</b> mostra lo stato di ogni attività all'interno di un progetto. L’interazione con la visualizzazione consente di apportare modifiche a un’attività in modo rapido e semplice.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">Visualizza la visualizzazione dell'attività del progetto in Analisi avanzate</a> </td> 
   <td> <p>La visualizzazione <b>Attività progetto</b> mostra una mappa di calore di quando gli utenti assegnati a un progetto hanno effettuato l'accesso a Workfront, hanno modificato lo stato dell'attività in quel progetto e hanno completato le attività in quel progetto. L’interazione con la visualizzazione ti consente di visualizzare questi dettagli per ogni utente. Puoi anche visualizzare date specifiche per queste azioni, nonché il numero di volte in cui ogni azione è stata completata.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">Visualizzazione Mappa ad albero progetto in Analisi avanzate</a> </td> 
   <td> <p>La visualizzazione <b>Mappa ad albero progetto</b> mostra quanto tempo è stato speso per alcuni progetti rispetto ad altri. L’interazione con la visualizzazione ti fornisce dettagli sulle condizioni del progetto, sul suo completamento pianificato e sul completamento effettivo.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">Visualizzazione dell'attività per team in Analisi avanzate</a> </td> 
   <td> <p>La visualizzazione <b>Attività per team</b> mostra una mappa di calore di quando gli utenti di un team principale accedono a Workfront, modificano lo stato di un'attività e completano un'attività. L’interazione con la visualizzazione ti consente di visualizzare questi dettagli per ogni singolo utente. Puoi anche visualizzare date specifiche per queste azioni, nonché il numero di volte in cui ogni azione è stata completata.</p> </td> 
  </tr> 
  <!-- Features permanently removed from Workfront
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">View the Resource capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Resource capacity</b> visualization shows you which home teams have the capacity to take on more work and which home teams have more work assigned to them than they can complete. Interacting with the visualization allows you to see more details about work completed and available hours for more work.&nbsp;Selecting a team opens the Team capacity visualization.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">View the Team capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Team capacity</b> visualization shows you a percentage of the amount of work a home team has completed out of the amount of work assigned to them. Interacting with the visualization allows you to see scheduled hours and planned hours for a specific date, as well as the capacity percentage and whether the home team was over, under, or at capacity on that day.</p> </td> 
  </tr>--> 
 </tbody> 
</table>
