---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Panoramica di Portfolio Optimizer
description: '[!UICONTROL Portfolio Optimizer] è lo strumento utilizzato per la valutazione e il confronto dei progetti. Il processo di revisione e confronto dei valori di Business Case per i progetti assegnati a un portfolio è il modo in cui un gestore di portfolio può dare priorità ai progetti e generare il massimo valore per un''organizzazione.'
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: c53e7d2229032c59710a8f955de53cfbd7fc6df4
workflow-type: tm+mt
source-wordcount: '1647'
ht-degree: 0%

---

# Panoramica di [!UICONTROL Portfolio Optimizer]

<!-- Audited: 01/2024 -->

[!UICONTROL Portfolio Optimizer] è lo strumento utilizzato per la valutazione e il confronto dei progetti. Il processo di revisione e confronto dei valori [!UICONTROL Caso di business] per i progetti assegnati a un portfolio è il modo in cui un gestore di portfolio può dare priorità ai progetti e generare il maggior valore per un&#39;organizzazione.

![Ottimizzatore Portfolio con progetti](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

Lo scopo di [!UICONTROL Ottimizzatore portfolio] è quello di fornire un&#39;interfaccia tramite la quale un gestore di portfolio, un comitato direttivo o un ufficio di gestione prodotti possono visualizzare informazioni di riepilogo sul caso di business di ciascun progetto. I progetti possono quindi essere classificati in base a valori e obiettivi strategici o in base al loro punteggio complessivo.

[!UICONTROL Portfolio Optimizer] può fornire assistenza solo se sono stati completati i seguenti prerequisiti:

* I [!UICONTROL casi aziendali] sono stati completati nei progetti. Per informazioni, vedere gli articoli in [Definire un caso di business: indice articolo](../../projects/define-a-business-case/define-business-case.md).
* Un portfolio è definito nell&#39;area Panoramica progetto della sezione Dettagli progetto per i progetti che si desidera esaminare.
* Hai indicato il Budget del progetto e il Beneficio pianificato per i progetti che desideri rivedere. Costi fissi e Redditi fissi sono facoltativi ma aggiungono valore. Per ulteriori informazioni, vedere [Campi finanziari progetto](../../projects/project-finances/project-finances-overview-1.md).

Per informazioni sull&#39;individuazione di [!UICONTROL Portfolio Optimizer], vedere [Individuare il [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## Finanze in [!UICONTROL Portfolio Optimizer]

Puoi visualizzare lo stato finanziario del tuo portfolio in qualsiasi momento durante la durata dei tuoi progetti utilizzando [!UICONTROL Portfolio Optimizer].

Quando si lavora con i dati finanziari in [!UICONTROL Portfolio Optimizer], tenere presente quanto segue:

* A ciascuno dei progetti viene assegnato un punteggio quando i relativi [!UICONTROL casi aziendali] vengono completati in base ai criteri corrispondenti in [!UICONTROL Portfolio Optimizer]. Ad esempio, i progetti a basso costo o ad alto allineamento ricevono un punteggio più alto.

  Per ulteriori informazioni sul calcolo del punteggio dell&#39;ottimizzatore portfolio di un progetto, vedere [Panoramica del punteggio [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* I calcoli finanziari per il [!UICONTROL Portfolio Optimizer] utilizzano il [!UICONTROL Costo preventivato] nel [!UICONTROL Business Case] del progetto.
* Puoi assegnare manualmente la priorità ai progetti in [!UICONTROL Portfolio Optimizer], tenendo conto di tutte le informazioni relative. Ad esempio, dati finanziari, allineamento alle scorecard e ROI.

### Aree finanziarie in [!UICONTROL Portfolio Optimizer] {#the-financial-areas-in-the-portfolio-optimizer}

È possibile visualizzare le informazioni finanziarie nelle seguenti aree di [!UICONTROL Portfolio Optimizer]:

* **[!UICONTROL Intestazione Portfolio]**: in quest&#39;area vengono visualizzate le informazioni finanziarie raccolte da tutti i progetti del portfolio. Viene visualizzato su ogni scheda dell&#39;oggetto Portfolio.
* **[!UICONTROL Portfolio Finances for Selected Projects]**: in quest&#39;area vengono visualizzate le informazioni finanziarie raccolte dai progetti selezionati in [!UICONTROL Portfolio Optimizer]. È possibile aggiungere o rimuovere progetti e capire in che modo questo influirà sulle finanze del portfolio visualizzando le informazioni in quest’area.
* **[!UICONTROL Finanza progetti]**: in quest&#39;area vengono visualizzate le informazioni finanziarie di ogni progetto elencato in [!UICONTROL Portfolio Optimizer].

### Campi finanziari in [!UICONTROL Portfolio Optimizer] {#the-financial-fields-in-the-portfolio-optimizer}

I seguenti campi finanziari vengono visualizzati in [!UICONTROL Portfolio Optimizer]:

* [Intestazione Portfolio](#portfolio-header)
* [Finanziamenti Portfolio per i progetti selezionati](#portfolio-finances-for-selected-projects)

#### Intestazione Portfolio {#portfolio-header}

![Intestazione Portfolio](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] calcola i campi finanziari nell&#39;intestazione del portfolio utilizzando informazioni provenienti da progetti con stati che equivalgono solo a [!UICONTROL Approvato] o [!UICONTROL Corrente].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nome campo</strong> </th> 
   <th><strong>Descrizione</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL On Time]</td> 
   <td> <p>Percentuale di progetti nel portfolio considerati come [!UICONTROL On Time]. È visibile da qualsiasi scheda all’interno di un portfolio.</p> <p>Un progetto è considerato [!UICONTROL On Time] quando il progetto <strong>[!UICONTROL Condition]</strong> è <strong>[!UICONTROL On Target]</strong>. <br>Per ulteriori informazioni su [!UICONTROL Project Conditions], vedere l'articolo <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Overview of Project Condition and Condition Type</a>.</p> <p>La percentuale di <strong>[!UICONTROL On Time]</strong> viene calcolata utilizzando la formula seguente:</p> <p><em>[!UICONTROL On Time Portfolio Percentage] = Numero di progetti [!UICONTROL On Time]/ Numero totale di progetti in uno stato [!UICONTROL Current] o [!UICONTROL Approved]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nel Budget]</td> 
   <td> <p>Percentuale di progetti nel portfolio considerati [!UICONTROL On Budget]. Visibile da qualsiasi scheda all'interno di un portfolio .</p> <p>I progetti sono <strong>[!UICONTROL Nel Budget]</strong> se non hanno superato il budget predefinito. <br>Per ulteriori informazioni sul budget di un progetto, vedere l'articolo <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">[!UICONTROL Gestisci] informazioni nell'area Finanza progetto</a>.</p> <p>La percentuale di [!UICONTROL nel budget] viene calcolata utilizzando la formula seguente:</p> <p><em>[!UICONTROL Percentuale su progetti Portfolio nel budget] = Numero di progetti [!UICONTROL nel budget]/ Numero totale di progetti </em><em>in uno stato [!UICONTROL corrente] o [!UICONTROL approvato]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>ROI (per portfolio)</td> 
   <td> <p>Il [!UICONTROL Return on Investment] (ROI) per il portfolio viene calcolato prendendo in considerazione il [!UICONTROL Benefit] totale di [!UICONTROL Portfolio] e il totale dei [!UICONTROL Budgeted Costs] dei progetti. È visibile da qualsiasi scheda all’interno di un portfolio.</p> <p>Il valore del ROI di Portfolio viene calcolato utilizzando la formula seguente:</p> <p><em>ROI Portfolio = ([!UICONTROL Total Benefit] - [!UICONTROL Total Budgeted Cost])/ [!UICONTROL Total Cost] * 100</em> </p> <p>Per ulteriori informazioni sul calcolo del ROI per un progetto, vedere l'articolo <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">Calcolare il ROI</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Allineato] o [!UICONTROL Punteggio Allineamento] </td> 
   <td> <p>Media di tutti i valori [!UICONTROL Punteggio allineamento progetto], calcolati dopo il completamento della [!UICONTROL Scorecard] nel business case  del progetto. Il punteggio di allineamento di ciascun progetto è elencato nella colonna [!UICONTROL Alignment] di [!UICONTROL Portfolio Optimizer]. È visibile da qualsiasi scheda all’interno di un portfolio.</p> <p>Per ulteriori informazioni sulla generazione di un punteggio di allineamento per un progetto, vedere l'articolo <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Applicare una scorecard a un progetto e generare un punteggio di allineamento</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valore Netto]</td> 
   <td> <p>La somma di tutti i [!UICONTROL Valori netti] di tutti i progetti nel portfolio. È visibile da qualsiasi scheda all’interno di un portfolio.</p> <p>Per ulteriori informazioni sulle modalità di calcolo di [!UICONTROL Net Value] per un progetto, vedere l'articolo <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calcolare il valore netto</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Finanziamenti Portfolio per i progetti selezionati {#portfolio-finances-for-selected-projects}

![Dati finanziari di Portfolio](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nome campo</strong> </th> 
   <th><strong>Descrizione</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Numero di progetti]</td> 
   <td> <p>Numero totale di progetti attivi nel portfolio. I progetti considerati attivi in un portfolio possono trovarsi in uno dei seguenti stati:</p> 
    <ul> 
     <li>[!UICONTROL corrente]</li> 
     <li>[!UICONTROL Planning]</li> 
     <li>[!UICONTROL approvato]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budget]</td> 
   <td>È possibile aggiornare manualmente questo campo per indicare il budget totale per l'intero portfolio. Questo budget viene utilizzato per tutti i progetti all'interno del portfolio. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rimanente]</td> 
   <td> <p>Il budget rimanente dopo il [!UICONTROL Total Cost] su tutti i progetti all'interno del portfolio è stato sottratto dal Budget del portfolio.</p> <p>Il [!UICONTROL Budget Portfolio rimanente] viene calcolato utilizzando la seguente formula:</p> <p><em>[!UICONTROL Budget Portfolio rimanente] = [!UICONTROL Budget Portfolio totale] - Costo preventivato totale  di tutti i progetti Portfolio</em> </p> <p>Il campo Budget del portfolio è una voce manuale nel campo Budget di Portfolio Optimizer. </p> <p>Per ulteriori informazioni sul tracciamento dei costi di un progetto, vedere <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tracciare i costi</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo Totale]</td> 
   <td> <p>Somma dei costi di tutti i progetti visualizzati in [!UICONTROL Portfolio Optimizer]. Il costo di ciascun progetto è uguale al costo preventivato del progetto visualizzato in [!UICONTROL Business Case Summary]. </p> <p>Per ulteriori informazioni sui campi finanziari dei progetti in [!UICONTROL Business Case], vedere la sezione "Informazioni sui campi finanziari nel Business Case" nell'articolo <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Creare un Business Case per un progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risk] </td> 
   <td> <p>La somma di tutti i [!UICONTROL Costi di rischio potenziale] di tutti i progetti inclusi nel portfolio. Il [!UICONTROL Potential Risk Cost] di ciascun progetto è elencato nella colonna [!UICONTROL Risk] del [!UICONTROL Portfolio Optimizer]. </p> <p>Per ulteriori informazioni sul calcolo dei rischi per i progetti, vedere l'articolo <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcolare il costo del rischio potenziale</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benefit]</td> 
   <td> <p>La somma di tutti i valori [!UICONTROL Planned Benefit] di tutti i progetti nel portfolio. Il valore del Vantaggio pianificato di ciascun progetto è elencato nella colonna [!UICONTROL Benefit] di [!UICONTROL Portfolio Optimizer]. </p> <p>Per ulteriori informazioni su [!UICONTROL Planned Benefit] di un progetto, vedi l'articolo <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Panoramica del Planned Benefit del progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Indicatore [!UICONTROL Rischio per Valore Netto]</td> 
   <td> <p>Misura il valore [!UICONTROL Rischio potenziale], tenendo conto del valore [!UICONTROL Valore netto] fornito da tutti i progetti nel portfolio. Per ottenere la massima efficienza all’interno del portfolio, è importante notare che l’indicatore di [!UICONTROL Risk] è basso e che l’indicatore di [!UICONTROL Valore netto] è alto. </p> <p>Per ulteriori informazioni sul calcolo del rischio per [!UICONTROL Valore netto], vedere l'articolo <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">Calcolare il rischio per il valore netto in un portfolio</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizza [!UICONTROL Portfolio Optimizer]

È possibile personalizzare solo l&#39;area dell&#39;elenco dei progetti di [!UICONTROL Portfolio Optimizer] utilizzando le impostazioni per modificare le informazioni nell&#39;elenco.

Le icone e le opzioni seguenti sono disponibili per [!UICONTROL Portfolio Optimizer]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Icona in Portfolio Optimizer</strong></td> 
   <td><strong>Nome</strong></td> 
   <td><strong>Funzione</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[!UICONTROL Imposta priorità progetto]</td> 
   <td><p>Usa questa icona quando vuoi salvare l'ordine dei progetti, in base alla loro priorità.</p>
   <p>Per utilizzare <b>Imposta priorità progetto</b> è necessario disporre delle autorizzazioni di gestione per tutti i progetti dell'elenco</p>.
    </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-optimize-icon-in-optimizer.png"> </td> 
   <td>Portafoglio di [!UICONTROL Optimize]</td> 
   <td>Utilizza questa icona per ottimizzare il portfolio in base ai seguenti valori finanziari dei progetti:
    <ul>
     <li>[!UICONTROL Costo]</li>
     <li>[!UICONTROL Alignment]</li>
     <li>Valore </li>
     <li>[!UICONTROL Rischio per il Beneficio]</li>
     <li>[!UICONTROL ROI]</li>
    </ul><p>Per ulteriori informazioni sull'ottimizzazione del portfolio, vedere l'articolo <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">Ottimizzare i progetti in [!UICONTROL Portfolio Optimizer]</a>.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>Icone [!UICONTROL Annulla]/ [!UICONTROL Ripeti]</td> 
   <td>Utilizzare queste icone per annullare o ripristinare le modifiche apportate a [!UICONTROL Portfolio Optimizer] prima del salvataggio.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portfolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>[!UICONTROL Show]/[!UICONTROL Hide] progetti non selezionati</td> 
   <td>Utilizza queste icone per visualizzare o nascondere i progetti nel portfolio che hai deselezionato.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[!UICONTROL Export] </td> 
   <td> <p>Utilizzare questa icona per esportare i dati nell'area [!UICONTROL Project Prioritization] di [!UICONTROL Portfolio Optimizer]. Puoi esportarlo nei seguenti formati:</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>[!UICONTROL Tab] Delimitato</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferences_portfolio_optimizer.png"> </td> 
   <td>[!UICONTROL Preferenze]</td> 
   <td> <p>Utilizzare questa icona per modificare i campi del progetto visualizzati nelle colonne di [!UICONTROL Portfolio Optimizer] o per modificare i progetti visualizzati in [!UICONTROL Optimizer] in base ai relativi stati. </p> <p>Suggerimento  
     <ul> 
      <li> <p>Non tutti i [!DNL Workfront] campi standard sono disponibili per l'aggiunta nelle colonne. </p> </li> 
     </ul> 
     <ul> 
      <li> <p>Puoi aggiungere solo i campi personalizzati con un valore diverso da zero in qualsiasi progetto del portfolio.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
