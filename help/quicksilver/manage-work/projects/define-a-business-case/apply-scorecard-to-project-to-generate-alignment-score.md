---
navigation-topic: business-case-and-scorecards
title: Applicare una scorecard a un progetto e generare un punteggio di allineamento
description: Puoi utilizzare una scorecard per misurare il livello di allineamento di un progetto ai criteri precedentemente stabiliti per un portfolio. Una scorecard spesso riflette la missione, i valori e gli obiettivi strategici di un’organizzazione.
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: f97c989f57d864252adf6e24f8e6b03f56d26901
workflow-type: tm+mt
source-wordcount: '1220'
ht-degree: 0%

---

# Applicare una scorecard a un progetto e generare un punteggio di allineamento

<!-- Audited: 06/2025 -->

Puoi utilizzare una scorecard per misurare il livello di allineamento di un progetto ai criteri precedentemente stabiliti per un portfolio. Una scorecard spesso riflette la missione, i valori e gli obiettivi strategici di un’organizzazione.

Per ulteriori informazioni sulle scorecard e su come crearne una, vedere [Creare una scorecard](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td>
   <p>Corrente: Prime o versione successiva</p>
   <p>oppure</p>
   <p>Legacy: aziendale o superiore</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>
   <p>Corrente: Standard</p>
   <p>oppure</p>
   <p>Legacy: Plan</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso ai progetti</p> <p>Visualizzare o accedere ai portafogli in modo più avanzato</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td><p>Gestire le autorizzazioni per un progetto</p> <p>Visualizza o autorizzazioni superiori per un portfolio</p> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Scorecard progetto {#project-scorecards}

* [Panoramica scorecard](#scorecards-overview)
* [Applicare una scorecard a un progetto](#apply-a-scorecard-to-a-project)

### Panoramica delle scorecard {#scorecards-overview}

In genere, un project manager completa le informazioni della scorecard per produrre un valore di allineamento compreso tra 0 e 100 per il progetto. Il valore prodotto viene successivamente utilizzato quando il gestore portfolio esamina i progetti nell’ottimizzatore portfolio per confrontarli.

Per ulteriori informazioni sull&#39;ottimizzazione del portfolio, vedere [Panoramica di Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

### Applicare una scorecard a un progetto

In qualità di utente con una licenza Standard o Plan e le autorizzazioni Manage (Gestisci) per un progetto, puoi allegare una scorecard al progetto.

Per ulteriori informazioni sulle autorizzazioni del progetto, vedere [Condividere un progetto in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

È possibile aggiungere scorecard a un progetto come parte della creazione del business case per il progetto.

Per ulteriori informazioni sulla creazione di un business case, vedere [Creare un business case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Prima di poter accedere alle scorecard dal caso di business, l’amministratore di Adobe Workfront o l’amministratore gruppo deve abilitare la sezione Scorecard nell’area Business Case dei progetti. Per informazioni sulla configurazione delle preferenze del progetto e sull&#39;abilitazione delle aree del caso di business, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Per applicare una scorecard a un progetto:

1. Passare a un progetto a cui si desidera applicare una scorecard.
1. Fai clic su **Business Case** nel pannello a sinistra.
1. Trova la sezione **Scorecard** del caso di business.\
   È necessario creare una scorecard prima che venga visualizzata la sezione **Scorecard** sul Business Case.

   Per informazioni sulla creazione di una scorecard, vedere [Creare una scorecard](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

1. Seleziona una scorecard dal menu a discesa.

   ![Nuova scorecard](assets/new-scorecard.png)

1. Immetti una risposta per tutte le domande nella scorecard.

   Workfront applica un punteggio a ciascuna domanda e calcola un punteggio di progetto complessivo in base al punteggio individuale di ciascuna domanda.

   Per ulteriori informazioni sulla generazione del punteggio di allineamento complessivo del progetto, vedere [Generare un punteggio di allineamento per un progetto](#generate-an-alignment-score-for-a-project).

1. Fai clic su **Salva** per salvare la scorecard e valutare il progetto.

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

Per ulteriori informazioni, vedere [Creare una scorecard](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

### Generare un punteggio di allineamento per un portfolio {#generate-an-alignment-score-for-a-portfolio}

Il punteggio di allineamento del portfolio è una media dei punteggi di allineamento di tutti i progetti del portfolio.

Una volta completate le scorecard dei progetti, Workfront utilizza questi valori per calcolare il punteggio di allineamento del portfolio come percentuale, utilizzando la seguente formula:

`Portfolio Alignment Score = The sum of the percentages of the project alignment scores / Number of projects in the portfolio`

>[!NOTE]
>
>Se a un progetto non è associata una scorecard e quindi non è associato un punteggio di allineamento, si considera che abbia un allineamento dello 0% nel portfolio. Il progetto viene preso in considerazione nel numero di progetti nel portfolio.

## Visualizzare il punteggio di allineamento

Puoi visualizzare il punteggio di allineamento di un progetto a livello di progetto o in Portfolio Optimizer.

* [Visualizzazione del punteggio di allineamento in un progetto](#view-the-alignment-score-on-a-project)
* [Visualizzare i punteggi di allineamento del progetto e del portfolio in Portfolio Optimizer](#view-the-alignment-scores-of-the-project-and-of-the-portfolio-in-the-portfolio-optimizer)

### Visualizzare il punteggio di allineamento di un progetto

Se si dispone dei diritti di Contribuisci al progetto, è possibile visualizzare il punteggio di allineamento di un progetto a livello di progetto.

1. Vai al progetto di cui desideri visualizzare il Punteggio di allineamento.
1. Fai clic su **Business Case** nel pannello a sinistra.
1. Vai a **Riepilogo del caso aziendale** sul lato destro dello schermo.

   Il punteggio di allineamento si trova nel Riepilogo caso di business, nel valore **Allineato**.

   ![Punteggio di allineamento in un progetto](assets/alignment-score-on-a-project.png)

### Visualizzare i punteggi di allineamento del progetto e del portfolio in Portfolio Optimizer

Se disponi dell’accesso Gestisci al portfolio, puoi visualizzare il punteggio di allineamento di un progetto o di un portfolio in Portfolio Optimizer.

Per ulteriori informazioni sulle informazioni visualizzate in Portfolio Optimizer, vedere [Panoramica di Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* [Individua il punteggio di allineamento del progetto in Portfolio Optimizer](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [Individuare il punteggio di allineamento del portfolio in Portfolio Optimizer](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

  ![Punteggio di allineamento in Portfolio Optimizer](assets/alignment-score-in-portfolio-optimizer.png)

#### Individua il punteggio di allineamento del progetto in Portfolio Optimizer {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

{{step1-to-portfolios}}

1. Fai clic sul nome di un portfolio.
1. Fai clic su **Ottimizzazione Portfolio** nel pannello a sinistra.

   Viene visualizzato Portfolio Optimizer.

   Il punteggio di allineamento di un progetto viene visualizzato come percentuale nella colonna **Allineamento** di Portfolio Optimizer.

   Questo è il punteggio di allineamento del progetto in base alla scheda di valutazione associata al progetto.

#### Individuare il punteggio di allineamento del portfolio in Portfolio Optimizer  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

{{step1-to-portfolios}}

1. Fai clic sul nome di un portfolio.
1. Fai clic su **Ottimizzazione Portfolio** nel pannello a sinistra.
1. Nella parte superiore di Portfolio Optimizer trova il valore **Aligned** e il contatore **Alignment**, che indicano il punteggio di allineamento del portfolio.

   Punteggio di allineamento del portfolio.

   Per ulteriori informazioni sulla generazione del punteggio di allineamento di un portfolio, vedere [Generare un punteggio di allineamento per un portfolio](#generate-an-alignment-score-for-a-portfolio).

## Panoramica del punteggio di Portfolio Optimizer

Esiste una differenza tra il punteggio di allineamento e il punteggio dell’ottimizzatore del portfolio di un progetto.

Il punteggio di allineamento di un progetto viene calcolato in base ai punti ottenuti dopo il completamento della scorecard. Questo punteggio viene quindi utilizzato per determinare il punteggio di allineamento del portfolio. Il punteggio di allineamento viene visualizzato come percentuale.

Il punteggio di allineamento di un progetto viene visualizzato nella colonna **Allineamento** di Portfolio Optimizer.

Il punteggio dell’ottimizzatore del portfolio è una classificazione calcolata automaticamente in Portfolio Optimizer in base alla quale è possibile assegnare una priorità ai progetti. Il punteggio dell&#39;ottimizzatore portfolio viene visualizzato come icona di indicatore accompagnata da un numero e viene visualizzato nella colonna **Punteggio** di Portfolio Optimizer. Un punteggio di Portfolio Optimizer viene generato solo quando vengono completate tutte le sezioni del Business Case, ad eccezione degli Obiettivi.

Per ulteriori informazioni sulla creazione di un Business Case per un progetto, vedere [Creare un Business Case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Per ulteriori informazioni sul calcolo del punteggio dell&#39;ottimizzatore portfolio di un progetto, vedere [Panoramica del punteggio dell&#39;ottimizzatore Portfolio](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).
