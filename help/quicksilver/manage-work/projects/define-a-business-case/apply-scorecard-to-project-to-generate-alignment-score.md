---
navigation-topic: business-case-and-scorecards
title: Applicare una scorecard a un progetto e generare un punteggio di allineamento
description: Puoi utilizzare una scorecard per misurare il livello di allineamento di un progetto ai criteri precedentemente stabiliti per un portfolio. Una scorecard spesso riflette la missione, i valori e gli obiettivi strategici di un’organizzazione.
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: db362bd73e51b30090708822876ad02f7804d064
workflow-type: tm+mt
source-wordcount: '1229'
ht-degree: 0%

---

# Applicare una scorecard a un progetto e generare un punteggio di allineamento

<!-- Audited: 02/2024 -->

Puoi utilizzare una scorecard per misurare il livello di allineamento di un progetto ai criteri precedentemente stabiliti per un portfolio. Una scorecard spesso riflette la missione, i valori e gli obiettivi strategici di un’organizzazione.

Per ulteriori informazioni sulle scorecard e su come crearne una, consulta [Creare una scorecard](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>
   <p>Nuovo: Prime o superiore</p>
   <p>oppure</p>
   <p>Corrente: Business o superiore</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Nuovo: Standard</p>
   <p>oppure</p>
   <p>Corrente: Piano</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p> <p>Accesso ai Portfoli di visualizzazione o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td><p>Gestire le autorizzazioni per un progetto</p> <p>Visualizza o autorizzazioni superiori per un portfolio</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Scorecard progetto {#project-scorecards}

* [Panoramica delle scorecard](#scorecards-overview)
* [Applicare una scorecard a un progetto](#apply-a-scorecard-to-a-project)

### Panoramica delle scorecard {#scorecards-overview}

In genere, un project manager completa le informazioni della scorecard per produrre un valore di allineamento compreso tra 0 e 100 per il progetto. Il valore prodotto viene successivamente utilizzato quando il gestore portfolio esamina i progetti nell’ottimizzatore portfolio per confrontarli.

Per ulteriori informazioni sull’ottimizzazione del portafoglio, consulta [Panoramica di Portfoli Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

### Applicare una scorecard a un progetto

In qualità di utente con una licenza Standard o Plan e le autorizzazioni Manage (Gestisci) per un progetto, puoi allegare una scorecard al progetto.

Per ulteriori informazioni sulle autorizzazioni per i progetti, consulta [Condividere un progetto in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

È possibile aggiungere scorecard a un progetto come parte della creazione del business case per il progetto.

Per ulteriori informazioni sulla creazione di un caso di business, consulta [Creare un Business Case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Prima di poter accedere alle scorecard dal caso di business, l’amministratore di Adobe Workfront o l’amministratore gruppo deve abilitare la sezione Scorecard nell’area Business Case dei progetti. Per informazioni sulla configurazione delle preferenze del progetto e sulle aree di abilitazione del caso di business, consulta [Configurare le preferenze di progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Per applicare una scorecard a un progetto:

1. Passare a un progetto a cui si desidera applicare una scorecard.
1. Clic **Business Case** nel pannello a sinistra.
1. Trova il **Scorecard** sezione del Business Case.\
   È necessario creare una scorecard prima di **Scorecard** Questa sezione viene visualizzata sul Business Case.

   Per informazioni sulla creazione di una scorecard, consulta [Creare una scorecard](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

1. Seleziona una scorecard dal menu a discesa.

   ![Nuova scorecard](assets/new-scorecard.png)

1. Immetti una risposta per tutte le domande nella scorecard.

   Workfront applica un punteggio a ciascuna domanda e calcola un punteggio di progetto complessivo in base al punteggio individuale di ciascuna domanda.

   Per ulteriori informazioni sulla generazione del punteggio di allineamento complessivo del progetto, consulta [Generare un punteggio di allineamento per un progetto](#generate-an-alignment-score-for-a-project).

1. Clic **Salva** per salvare la scorecard e valutare il progetto.

   La scheda di valutazione è ora associata al progetto e il progetto ha un punteggio.

<!--This functionality was removed when we redesigned bulk editing projects with 23.2: 

1. (Conditional) When changes occur in the values of scorecard questions, you must recalculate the scorecard to reflect the new values for the project score. To recaulate the scorecard, do the following: 

   1. Go to a list of projects and select all projects in the list. 
   1. Click the **Edit** icon at the top of the list. 
   1. Click **Settings** in the left panel, then check the **Recalculate Scorecards** option at the end of the Settings area. 
   1. Click Save. This recalculates the score value based on the scorecards attached for all the selected projects.  

      >[!NOTE]
      >
      >   The option to recalculate scorecards has been removed from the Preview environment, when editing projects in bulk. 

-->

## Generare un punteggio di allineamento

* [Generare un punteggio di allineamento per un progetto](#generate-an-alignment-score-for-a-project)
* [Generare un punteggio di allineamento per un portfolio](#generate-an-alignment-score-for-a-portfolio)

### Generare un punteggio di allineamento per un progetto {#generate-an-alignment-score-for-a-project}

Il punteggio di allineamento è il valore prodotto dopo il completamento della scorecard.

Le scorecard contengono domande con scelte di risposta a cui sono stati assegnati valori numerici, denominati punti di allineamento. Questi punti vengono utilizzati per determinare il livello di allineamento del progetto con l’organizzazione. I punti di allineamento per ogni domanda contengono un numero compreso tra 0 e 100.

Una volta completata la scorecard, Workfront calcola il punteggio di allineamento del progetto come percentuale, utilizzando la seguente formula:

`Project Alignment Score = The sum of the question points from the scorecard met at a given time / The sum of the possible points on the scorecard`

Per ulteriori informazioni, consulta [Creare una scorecard](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

### Generare un punteggio di allineamento per un portfolio {#generate-an-alignment-score-for-a-portfolio}

Il punteggio di allineamento del portfolio è una media dei punteggi di allineamento di tutti i progetti del portfolio.

Una volta completate le scorecard dei progetti, Workfront utilizza questi valori per calcolare il punteggio di allineamento del portfolio come percentuale, utilizzando la seguente formula:

`Portfolio Alignment Score = The sum of the percentages of the project alignment scores / Number of projects in the portfolio`

>[!NOTE]
>
>Se a un progetto non è associata una scorecard e quindi non è associato un punteggio di allineamento, si considera che abbia un allineamento dello 0% nel portfolio. Il progetto viene preso in considerazione nel numero di progetti nel portfolio.

## Visualizzare il punteggio di allineamento

Puoi visualizzare il punteggio di allineamento di un progetto a livello di progetto o in Ottimizzatore Portfolio.

* [Visualizzare il punteggio di allineamento di un progetto](#view-the-alignment-score-on-a-project)
* [Visualizzare i punteggi di allineamento del progetto e del portfolio in Ottimizzatore Portfolio](#view-the-alignment-scores-of-the-project-and-of-the-portfolio-in-the-portfolio-optimizer)

### Visualizzare il punteggio di allineamento di un progetto

Se si dispone dei diritti di Contribuisci al progetto, è possibile visualizzare il punteggio di allineamento di un progetto a livello di progetto.

1. Vai al progetto di cui desideri visualizzare il Punteggio di allineamento.
1. Clic **Business Case** nel pannello a sinistra.
1. Vai a **Riepilogo del Business Case** sul lato destro dello schermo.

   Il punteggio di allineamento si trova nel Riepilogo caso di business, nel **Allineato** valore.

   ![Punteggio di allineamento in un progetto](assets/alignment-score-on-a-project.png)

### Visualizzare i punteggi di allineamento del progetto e del portfolio in Ottimizzatore Portfolio

Puoi visualizzare il punteggio di allineamento di un progetto o di un portfolio in Ottimizzatore Portfolio, se disponi dell’accesso Gestisci al portfolio.

Per ulteriori informazioni sulle informazioni visualizzate in Ottimizzatore Portfolio, vedi [Panoramica di Portfoli Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* [Individua il punteggio di allineamento del progetto in Ottimizzatore Portfolio](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [Individua il punteggio di allineamento del portfolio in Ottimizzatore Portfolio](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

  ![Punteggio di allineamento in Portfoli Optimizer](assets/alignment-score-in-portfolio-optimizer.png)

#### Individua il punteggio di allineamento del progetto in Ottimizzatore Portfolio {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

{{step1-to-portfolios}}

1. Fai clic sul nome di un portfolio.
1. Clic **Ottimizzazione Portfolio** nel pannello a sinistra.

   Viene visualizzato Ottimizzatore Portfolio.

   Il punteggio di allineamento di un progetto viene visualizzato come percentuale nel **Allineamento** dell&#39;Ottimizzatore Portfolio.

   Questo è il punteggio di allineamento del progetto in base alla scheda di valutazione associata al progetto.

#### Individua il punteggio di allineamento del portfolio in Ottimizzatore Portfolio  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

{{step1-to-portfolios}}

1. Fai clic sul nome di un portfolio.
1. Clic **Ottimizzazione Portfolio** nel pannello a sinistra.
1. Nella parte superiore di Ottimizzatore Portfolio, individua **Allineato** valore, nonché **Allineamento** che indicano il punteggio di allineamento del portfolio.

   Punteggio di allineamento del portfolio.

   Per ulteriori informazioni sulla modalità di generazione del punteggio di allineamento di un portfolio, consulta [Generare un punteggio di allineamento per un portfolio](#generate-an-alignment-score-for-a-portfolio).

## Panoramica del punteggio dell’ottimizzatore del Portfolio

Esiste una differenza tra il punteggio di allineamento e il punteggio dell’ottimizzatore del portfolio di un progetto.

Il punteggio di allineamento di un progetto viene calcolato in base ai punti ottenuti dopo il completamento della scorecard. Questo punteggio viene quindi utilizzato per determinare il punteggio di allineamento del portfolio. Il punteggio di allineamento viene visualizzato come percentuale.

Il punteggio di allineamento di un progetto viene visualizzato nel **Allineamento** dell&#39;Ottimizzatore Portfolio.

Il punteggio dell’ottimizzatore portfolio è una classificazione calcolata automaticamente nell’ottimizzatore Portfolio in base alla quale è possibile assegnare la priorità ai progetti. Il punteggio dell’ottimizzatore del portfolio viene visualizzato come icona di indicatore accompagnata da un numero e viene visualizzato nel **Punteggio** dell&#39;Ottimizzatore Portfolio. Un punteggio di Portfoli Optimizer viene generato solo quando tutte le sezioni del Business Case sono completate, ad eccezione degli Obiettivi.

Per ulteriori informazioni sulla creazione di un caso di business per un progetto, consulta [Creare un Business Case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Per ulteriori informazioni sul calcolo del punteggio dell’ottimizzatore portfolio di un progetto, consulta [Panoramica del punteggio dell’ottimizzatore del Portfolio](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).
