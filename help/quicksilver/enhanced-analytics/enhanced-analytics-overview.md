---
title: Panoramica dell’analisi migliorata
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: L’analisi avanzata è uno strumento potente in Adobe Workfront con visualizzazioni predefinite che ti consente di esaminare i dati del progetto e identificare le tendenze in fase di pianificazione e completamento. Queste informazioni approfondite sui progetti consentono di gestire il lavoro corrente e di pianificare in modo più preciso il lavoro futuro.
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 2%

---

# Panoramica dell’analisi migliorata

L’analisi avanzata è uno strumento potente in Adobe Workfront con visualizzazioni predefinite che ti consente di esaminare i dati del progetto e identificare le tendenze in fase di pianificazione e completamento. Queste informazioni approfondite sui progetti consentono di gestire il lavoro corrente e di pianificare in modo più preciso il lavoro futuro.

L’analisi avanzata può aiutarti a identificare:

* Modalità di pianificazione dei progetti
* Quando il lavoro viene aggiunto ai progetti
* Quantità di lavoro da completare per progetti diversi
* Quantità di ore o giorni necessari per completare un progetto rispetto alle ore o ai giorni pianificati per un team principale
* Con quale frequenza gli utenti completano azioni specifiche durante un progetto
* Lo stato di avanzamento dei progetti e i singoli compiti all&#39;interno di un progetto

![](assets/nwe-full-screen-analytics-350x222.png)

Per visualizzare i casi di utilizzo o ulteriori informazioni sulla gestione del lavoro corrente e sulla pianificazione del lavoro futuro con l’analisi avanzata, consulta [Percorsi di apprendimento di analisi migliorati](https://one.workfront.com/s/enhanced-analytics-program).

## Prerequisiti

Per accedere all’area Analisi avanzata, devi:

* Avere un piano aziendale o aziendale.

   Per ulteriori informazioni, consulta [Piani Workfront](https://www.workfront.com/plans).

* Chiedi al tuo amministratore Workfront di aggiungere l&#39;analisi avanzata al modello di layout.

   Per ulteriori informazioni, consulta [Analisi avanzata: Aggiunta di analisi ai modelli di layout](https://one.workfront.com/s/managed-content-videos/enhanced-analytics-adding-analytics-to-layout-templates-MCH7URDSIXRREHHHF7TRTYYP2LTE).

Per visualizzare le informazioni relative a progetti e attività, è necessario:

* Disporre dell&#39;autorizzazione Visualizza per le aree Progetti e Attività nel livello di accesso.

   Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta [Creare o modificare livelli di accesso personalizzati](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Disporre dell&#39;autorizzazione Visualizza per attività e/o progetti specifici.

   Per informazioni sulla richiesta di accesso aggiuntivo, vedi [Richiedere l’accesso agli oggetti](../workfront-basics/grant-and-request-access-to-objects/request-access.md).

## Best practice per l’analisi avanzata

Per ottenere i dati migliori per i progetti, utilizza modelli con ore pianificate e giorni di durata accurati. È inoltre necessario assicurarsi che gli utenti inseriscano e aggiornino i campi riportati di seguito nel modo più accurato possibile.

>[!NOTE]
>
>Alcuni dei campi seguenti sono calcoli eseguiti da Workfront in base alle informazioni immesse dagli utenti. Non è possibile aggiornare manualmente questi campi.

* Lavoro Necessario

   Questo è il campo più importante da compilare.

   >[!NOTE]
   >
   >Se i team non utilizzano le ore pianificate, puoi comunque visualizzare alcuni dati in base alla durata del progetto.\
   >Per ulteriori informazioni, consulta la sezione . [Vista a lungo termine](#duration-view) in questo articolo.

* Nome progetto

   Il nome deve essere descrittivo del progetto.

* Condizione progetto
* Stato Progetto
* Data di inizio prevista del progetto
* Data di completamento Pianificata
* Data di inizio effettiva del progetto
* Data di fine effettiva del progetto
* Durata del progetto Ore
* Ore effettive del progetto
* Stato attività (incluso il contrassegno delle attività completate).
* Nome attività
* Percentuale attività completata
* Data inizio pianificata attività
* Data Pianificata completamento Attività

>[!IMPORTANT]
>
>Le modifiche apportate a attività e progetti possono richiedere fino a 24 ore per riflettere in Analisi avanzata.

## Vista a lungo termine {#duration-view}

Per impostazione predefinita, le visualizzazioni Mappa a discesa e Mappa ad albero del progetto si basano sulle ore pianificate. Se i tuoi team non utilizzano le ore pianificate, puoi guardare queste visualizzazioni in base alla durata del progetto.

In Analisi avanzata, la durata di un progetto viene calcolata dalle seguenti formule:

* Periodo programmato:

   ```
   Planned Completion Date of the project - Start Date of the project
   ```

* Giorni lavorati:

   ```
   Planned Duration for tasks completed in the selected date range / Typical hours per work day
   ```

   >[!NOTE]
   >
   >8 ore è il numero predefinito per **Orari tipici per giorno lavorativo**. Un amministratore Adobe Workfront può aggiornare **Orari tipici per giorno lavorativo** impostando **Configurazione** > **Preferenze del progetto** > **Progetti** > **Timeline**.\
   >Per ulteriori informazioni, consulta [Configurare le preferenze del progetto a livello di sistema](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Per informazioni sulla durata prevista, vedi [Panoramica della durata del progetto](../manage-work/projects/planning-a-project/project-duration.md).

## Scelte rapide da tastiera

Puoi utilizzare i seguenti tasti sulla tastiera per navigare o completare azioni specifiche nell’area Analisi avanzata:

| Chiave | Azione |
|---|---|
| **Linguetta** | Passa a ogni elemento della pagina, nonché a una tabella con informazioni su ogni visualizzazione che non viene visualizzata sulla pagina |
| **Invio** | Apri il widget del calendario, elimina un filtro esistente, apri le opzioni del filtro Aggiungi, seleziona/deseleziona i valori del filtro, applica un filtro creato, apri le opzioni di esportazione per ogni visualizzazione, apri i menu a discesa nelle visualizzazioni Masterizzazione, Attività in volo e Mappa del progetto |
| **Tasti freccia** | Passa alle date del widget calendario, alle opzioni filtro quando aggiungi un filtro e alle opzioni di tutti i menu a discesa delle visualizzazioni |
| **Barra spaziatrice** | Seleziona le date nel widget calendario, seleziona un tipo di filtro quando aggiungi un filtro, seleziona un’opzione di esportazione dal menu a discesa di ciascuna visualizzazione e seleziona le opzioni dai menu a discesa nelle visualizzazioni a discesa, Attività in volo e Mappa degli alberi Progetto |

{style=&quot;table-layout:auto&quot;}

Se si utilizza un software per la lettura dello schermo o un plug-in, l’assistente vocale legge le informazioni sullo schermo ad alta voce e descrive le azioni che si stanno completando quando si utilizzano i tasti elencati sopra.

## Viste e funzionalità di analisi migliorate

Per ulteriori informazioni sui dettagli di una funzione specifica in Analisi avanzata, sulle azioni che puoi completare per ottenere ulteriori informazioni e su cosa puoi imparare da questi dati, vedi i seguenti articoli:

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
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Applicazione di filtri in Analisi avanzata</a> </td> 
   <td> <p>Puoi applicare filtri personalizzati, filtri per campi di progetto o filtri per team per visualizzare solo i progetti che soddisfano criteri specifici. Quando si aggiungono filtri, il numero di progetti viene aggiornato di conseguenza.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">Comprendere i KPI di analisi migliorati</a> </td> 
   <td> <p>Gli indicatori prestazioni chiave (KPI, Key Performance Indicators) per tutti i progetti entro un intervallo di tempo specifico si trovano nella parte superiore dello schermo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">Visualizzazione della visualizzazione del piano di volo in Analisi avanzata</a> </p> </td> 
   <td> <p>La <b>piano di volo</b> La visualizzazione mostra che la condizione è cambiata nel corso della vita di un progetto. L’interazione con la visualizzazione fornisce ulteriori dettagli su date specifiche. Quando si seleziona un progetto, vengono aperte le Attività e le Attività nelle visualizzazioni dei voli.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">Visualizzare la visualizzazione a discesa in Analisi avanzata</a> </td> 
   <td> <p>La <b>Burn</b> la visualizzazione mostra la velocità pianificata di un progetto rispetto alla quantità effettiva di ore dedicate a un progetto. L’interazione con la visualizzazione fornisce ulteriori dettagli sulla condizione del progetto in una data specifica.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">Visualizzazione delle attività nella visualizzazione dei voli in Enhanced analytics</a> </td> 
   <td> <p>La <b>Compiti in volo</b> La visualizzazione mostra lo stato di ogni attività all’interno di un progetto. L’interazione con la visualizzazione consente di apportare modifiche rapide e semplici a un’attività.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">Visualizzazione della visualizzazione delle attività del progetto in Analisi avanzata</a> </td> 
   <td> <p>La <b>Attività del progetto</b> La visualizzazione mostra una mappa di calore che indica quando gli utenti sono stati assegnati a un progetto che ha effettuato l’accesso a Workfront, lo stato dell’attività in quel progetto e le attività completate in quel progetto. L’interazione con la visualizzazione consente di visualizzare questi dettagli per ogni utente. Puoi anche visualizzare date specifiche per queste azioni, nonché il numero di volte in cui ciascuna azione è stata completata.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">Visualizzare la visualizzazione della mappa del percorso del progetto in Analisi avanzata</a> </td> 
   <td> <p>La <b>Treemap del progetto</b> La visualizzazione mostra quanto tempo è stato speso per alcuni progetti rispetto ad altri. L’interazione con la visualizzazione fornisce dettagli sulle condizioni del progetto, sul completamento del progetto pianificato e sul completamento effettivo del progetto.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">Visualizzazione dell’attività per team in Analisi avanzata</a> </td> 
   <td> <p>La <b>Attività per team</b> La visualizzazione mostra una mappa di calore del momento in cui gli utenti di un team principale hanno effettuato l’accesso a Workfront, hanno modificato lo stato di un’attività e completato un’attività. L’interazione con la visualizzazione consente di visualizzare questi dettagli per ogni singolo utente. Puoi anche visualizzare date specifiche per queste azioni, nonché il numero di volte in cui ciascuna azione è stata completata.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">Visualizzazione della visualizzazione della capacità delle risorse in Analisi avanzata</a> </td> 
   <td> <p>La <b>Capacità delle risorse</b> La visualizzazione mostra quali team domestici sono in grado di svolgere più lavoro e quali team domestici dispongono di più lavoro da assegnare di quanti possano completare. L’interazione con la visualizzazione ti consente di visualizzare ulteriori dettagli sul lavoro completato e sulle ore disponibili per ulteriore lavoro. Quando si seleziona un team, viene visualizzata la visualizzazione della capacità del team.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">Visualizzazione della visualizzazione della capacità del team in Analisi avanzata</a> </td> 
   <td> <p>La <b>Capacità del team</b> la visualizzazione mostra una percentuale della quantità di lavoro che un team domestico ha completato rispetto alla quantità di lavoro assegnata loro. L’interazione con la visualizzazione ti consente di visualizzare le ore pianificate e pianificate per una data specifica, nonché la percentuale di capacità e se il team principale è stato superato, meno o alla capacità in quel giorno.</p> </td> 
  </tr> 
 </tbody> 
</table>
