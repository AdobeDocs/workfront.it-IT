---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Panoramica di Portfoli Optimizer
description: Il [!UICONTROL Ottimizzatore Portfolio] è lo strumento utilizzato per la valutazione e il confronto dei progetti. Il processo di revisione e confronto dei valori di Business Case per i progetti assegnati a un portfolio è il modo in cui un gestore di portfolio può dare priorità ai progetti e generare il massimo valore per un'organizzazione.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: fb1c7ade6622db391e0dac54f37603efe9dc0a58
workflow-type: tm+mt
source-wordcount: '1649'
ht-degree: 0%

---

# [!UICONTROL Ottimizzatore Portfolio] panoramica

Il [!UICONTROL Ottimizzatore Portfolio] è lo strumento utilizzato per la valutazione e il confronto dei progetti. Il processo di revisione e confronto [!UICONTROL Business Case] i valori per i progetti assegnati a un portfolio sono il modo in cui un gestore di portfolio può dare priorità ai progetti e generare il valore maggiore per un’organizzazione.

![](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

Scopo della [!UICONTROL ottimizzatore portfolio] fornisce un’interfaccia tramite la quale un gestore di portafoglio, un comitato direttivo o un ufficio di gestione prodotti può visualizzare informazioni sintetiche sul business case di ciascun progetto. I progetti possono quindi essere classificati in base a valori e obiettivi strategici o in base al loro punteggio complessivo.

Il [!UICONTROL Ottimizzatore Portfolio] puoi fornirti assistenza solo se hai soddisfatto i seguenti prerequisiti:

* Il [!UICONTROL Casi di studio] sono state completate per i progetti. Per informazioni, consulta gli articoli in [Definire un caso di business: indice articolo](../../projects/define-a-business-case/define-business-case.md).
* Un portfolio è definito nell&#39;area Panoramica progetto della sezione Dettagli progetto per i progetti che si desidera esaminare.
* Hai indicato il Budget del progetto e il Beneficio pianificato per i progetti che desideri rivedere. Costi fissi e Redditi fissi sono facoltativi ma aggiungono valore. Per informazioni, consulta [Campi finanziari progetto](../../projects/project-finances/project-finances-overview-1.md).

Per informazioni su come individuare [!UICONTROL Ottimizzatore Portfolio], vedi [Individua il [!UICONTROL Ottimizzatore Portfolio]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## Finanze nel [!UICONTROL Ottimizzatore Portfolio]

* [Le aree finanziarie nel [!UICONTROL Ottimizzatore Portfolio]](#the-financial-areas-in-the-portfolio-optimizer)
* [I settori finanziari nella [!UICONTROL Ottimizzatore Portfolio]](#the-financial-fields-in-the-portfolio-optimizer)

Lo stato finanziario del portfolio è visibile in qualsiasi momento durante la durata dei progetti utilizzando [!UICONTROL Ottimizzatore Portfolio].

Quando si lavora con le risorse finanziarie nel [!UICONTROL Ottimizzatore Portfolio]:

* Ad ognuno dei progetti viene assegnato un punteggio quando [!UICONTROL Casi di studio] vengono completate in base ai criteri corrispondenti nel [!UICONTROL Ottimizzatore Portfolio]. Ad esempio, i progetti a basso costo o ad alto allineamento ricevono un punteggio più alto.

  Per ulteriori informazioni sul calcolo del punteggio dell’ottimizzatore del portfolio di un progetto, consulta l’articolo [Panoramica di [!UICONTROL Ottimizzatore Portfolio] Punteggio](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* I calcoli finanziari per [!UICONTROL Ottimizzatore Portfolio] utilizzare il [!UICONTROL Costo preventivato] nel [!UICONTROL Business Case] del progetto.
* Puoi assegnare manualmente la priorità ai progetti in [!UICONTROL Ottimizzatore Portfolio], tenendo conto di tutte le informazioni che li riguardano. Ciò include dati finanziari, allineamento alle scorecard, ROI, ad esempio.

### Le aree finanziarie nel [!UICONTROL Ottimizzatore Portfolio] {#the-financial-areas-in-the-portfolio-optimizer}

È possibile visualizzare le informazioni finanziarie nelle seguenti aree del [!UICONTROL Ottimizzatore Portfolio]:

* **[!UICONTROL Intestazione Portfolio]**: quest’area mostra le informazioni finanziarie raccolte da tutti i progetti del portfolio. Viene visualizzato su ogni scheda dell&#39;oggetto Portfolio.
* **[!UICONTROL Finanze di Portfolio per i progetti selezionati]**: quest’area mostra le informazioni finanziarie raccolte dai progetti selezionati nella sezione [!UICONTROL Ottimizzatore Portfolio]. È possibile aggiungere o rimuovere progetti e capire in che modo questo influirà sulle finanze del portfolio visualizzando le informazioni in quest’area.
* **[!UICONTROL Finanze progetti]**: in quest’area vengono visualizzate le informazioni finanziarie di ciascun progetto elencato nella sezione [!UICONTROL Ottimizzatore Portfolio].

### I settori finanziari nella [!UICONTROL Ottimizzatore Portfolio] {#the-financial-fields-in-the-portfolio-optimizer}

I seguenti campi finanziari vengono visualizzati nel [!UICONTROL Ottimizzatore Portfolio]:

* [Intestazione Portfolio](#portfolio-header)
* [Finanziamenti Portfoli per i progetti selezionati](#portfolio-finances-for-selected-projects)

#### Intestazione Portfolio {#portfolio-header}

![](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] calcola i campi finanziari nell’intestazione del portfolio utilizzando le informazioni dei progetti con stati che equivalgono solo a [!UICONTROL Approvato] o [!UICONTROL Corrente].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nome del campo</strong> </th> 
   <th><strong>Descrizione</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL On Time]</td> 
   <td> <p>Percentuale di progetti nel portfolio considerati come [!UICONTROL On Time]. È visibile da qualsiasi scheda all’interno di un Portfolio.</p> <p>Un progetto è considerato [!UICONTROL On Time] quando il progetto <strong>Condizione [!UICONTROL]</strong> è <strong>[!UICONTROL Su Target]</strong>. <br>Per ulteriori informazioni su [!UICONTROL Condizioni progetto], vedere l'articolo <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Panoramica della condizione e del tipo di condizione del progetto</a>.</p> <p>Il <strong>[!UICONTROL On Time]</strong> la percentuale viene calcolata utilizzando la seguente formula:</p> <p><em>[!UICONTROL su percentuale Portfolio di lavoro] = Numero di progetti [!UICONTROL su tempo]/ Numero totale di progetti in uno stato [!UICONTROL corrente] o [!UICONTROL approvato]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nel Budget]</td> 
   <td> <p>Percentuale di progetti nel portfolio considerati [!UICONTROL On Budget]. È visibile da qualsiasi scheda all'interno di un Portfolio [!UICONTROL].</p> <p>I progetti sono <strong>[!UICONTROL Nel Budget]</strong> quando non hanno superato il budget predefinito. <br>Per ulteriori informazioni sul budget di un progetto, consulta l’articolo <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Informazioni su [!UICONTROL Gestisci] nell'area Finanza progetto</a>.</p> <p>La percentuale di [!UICONTROL nel budget] viene calcolata utilizzando la formula seguente:</p> <p><em>[!UICONTROL Su Percentuale Portfolio Budget] = Numero di progetti [!UICONTROL Su Budget]/ Numero totale di progetti </em><em>in uno stato [!UICONTROL Current] o [!UICONTROL Approved]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>ROI (per portfolio)</td> 
   <td> <p>Il [!UICONTROL Return on Investment] (ROI) per il portfolio viene calcolato prendendo in considerazione il [!UICONTROL Benefit] totale del [!UICONTROL Portfolio] e il totale dei [!UICONTROL Costi preventivati] dei progetti. È visibile da qualsiasi scheda all’interno di un Portfolio.</p> <p>Il valore del ROI Portfolio viene calcolato utilizzando la formula seguente:</p> <p><em>ROI Portfolio = ([!UICONTROL Total Benefit] - [!UICONTROL Total Budgeted Cost])/ [!UICONTROL Total Cost] * 100</em> </p> <p>Per ulteriori informazioni su come viene calcolato il ROI per un progetto, consulta l’articolo <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">Calcola il ritorno sull’investimento (ROI)</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Allineato] o [!UICONTROL Punteggio Allineamento] </td> 
   <td> <p>Media di tutti i valori [!UICONTROL Punteggio allineamento progetto] calcolati dopo il completamento della [!UICONTROL Scorecard] nel business case [!UICONTROL] del progetto. Il punteggio di allineamento di ciascun progetto è elencato nella colonna [!UICONTROL Alignment] dell'Ottimizzatore Portfolio [!UICONTROL]. È visibile da qualsiasi scheda all’interno di un portfolio.</p> <p>Per ulteriori informazioni sulla generazione di un punteggio di allineamento per un progetto, consulta l’articolo <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Applicare una scorecard a un progetto e generare un punteggio di allineamento</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valore Netto]</td> 
   <td> <p>La somma di tutti i [!UICONTROL Valori netti] di tutti i progetti nel portfolio. È visibile da qualsiasi scheda all’interno di un portfolio.</p> <p>Per ulteriori informazioni sul calcolo di [!UICONTROL Valore Netto] per un progetto, vedere l'articolo <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calcola valore netto</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Finanziamenti Portfoli per i progetti selezionati {#portfolio-finances-for-selected-projects}

![](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nome del campo</strong> </th> 
   <th> <p><strong>Descrizione</strong> </p> <p> </p> </th> 
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
   <td> <p>Il budget rimanente dopo tutti i [!UICONTROL Costi preventivati] su tutti i progetti all'interno del portfolio è stato sottratto dal Budget del portfolio.</p> <p>Il [!UICONTROL Budget Portfolio rimanente] viene calcolato utilizzando la seguente formula:</p> <p><em>[!UICONTROL Budget Portfolio rimanente] = [!UICONTROL Budget Portfolio totale] - Totale [!UICONTROL Costo preventivato] di Tutti i progetti Portfolio</em> </p> <p>Il [!UICONTROL Costo preventivato] complessivo di tutti i progetti nel portfolio è rappresentato nella barra degli indicatori sotto il campo Budget. </p> <p>Per ulteriori informazioni sul tracciamento dei costi di un progetto, consulta l’articolo<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tracciare i costi</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Costo Totale]</td> 
   <td> <p>Somma dei costi di tutti i progetti visualizzati in [!UICONTROL Portfoli Optimizer]. Il costo di ciascun progetto è uguale al costo preventivato del progetto visualizzato in [!UICONTROL Business Case Summary]. </p> <p>Per ulteriori informazioni sui campi finanziari dei progetti nel Business Case di [!UICONTROL], vedere la sezione "Informazioni sui campi finanziari nel Business Case" nell'articolo <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Creare un Business Case per un progetto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risk] </td> 
   <td> <p>La somma di tutti i [!UICONTROL Costi di rischio potenziale] di tutti i progetti inclusi nel portfolio. Il [!UICONTROL Potential Risk Cost] di ciascun progetto è elencato nella colonna [!UICONTROL Risk] del [!UICONTROL Portfoli Optimizer]. </p> <p>Per ulteriori informazioni sul calcolo dei rischi per i progetti, vedere l'articolo <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcola costo rischio potenziale </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benefit]</td> 
   <td> <p>La somma di tutti i valori [!UICONTROL Planned Benefit] di tutti i progetti nel portfolio. Il valore del Vantaggio pianificato di ciascun progetto è elencato nella colonna [!UICONTROL Benefit] di [!UICONTROL Portfoli Optimizer]. </p> <p>Per ulteriori informazioni su [!UICONTROL Planned Benefit] di un progetto, consulta l’articolo <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Panoramica del beneficio pianificato del progetto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Indicatore [!UICONTROL Rischio per Valore Netto]</td> 
   <td> <p>Misura il valore del rischio potenziale di [!UICONTROL] tenendo conto del valore del [!UICONTROL Valore netto] fornito da tutti i progetti nel portfolio. Per ottenere la massima efficienza all’interno del portfolio, è importante notare che l’indicatore di [!UICONTROL Risk] è basso e che l’indicatore di [!UICONTROL Valore netto] è alto. </p> <p>Per ulteriori informazioni sul calcolo del rischio per [!UICONTROL Valore netto], vedere l'articolo <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">Calcolare il rischio per il valore netto in un portfolio</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizzare [!UICONTROL Ottimizzatore Portfolio]

Puoi personalizzare solo l’area dell’elenco dei progetti del [!UICONTROL Ottimizzatore Portfolio] utilizzando le impostazioni per modificare le informazioni nell&#39;elenco.

Le icone e le opzioni seguenti sono disponibili per [!UICONTROL Ottimizzatore Portfolio]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Icona in Ottimizzatore Portfolio</td> 
   <td>Nome</td> 
   <td>Funzione</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[!UICONTROL Imposta priorità progetto]</td> 
   <td>Usa questa icona quando vuoi salvare l'ordine dei progetti, in base alla loro priorità. </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-optimize-icon-in-optimizer.png"> </td> 
   <td>Portafoglio di [!UICONTROL Optimize]</td> 
   <td>Utilizza questa icona per ottimizzare il portfolio in base ai seguenti valori finanziari dei progetti:
    <ul>
     <li>[!UICONTROL Costo]</li>
     <li>[!UICONTROL Alignment]</li>
     <li>Valore [!UICONTROL]</li>
     <li>[!UICONTROL Rischio per il Beneficio]</li>
     <li>[!UICONTROL ROI]</li>
    </ul><p>Per ulteriori informazioni sull’ottimizzazione del tuo portfolio, consulta l’articolo <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">Ottimizza progetti in [!UICONTROL Portfoli Optimizer] </a>.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>Icone [!UICONTROL Annulla]/ [!UICONTROL Ripeti]</td> 
   <td>Utilizzare queste icone per annullare o ripristinare le modifiche apportate a [!UICONTROL Portfoli Optimizer] prima del salvataggio.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portfolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>Progetti [!UICONTROL Show]/ [!UICONTROL Hide unselected]</td> 
   <td>Utilizza queste icone per visualizzare o nascondere i progetti nel portfolio che hai deselezionato.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[!UICONTROL Export] </td> 
   <td> <p>Utilizzare questa icona per esportare i dati nell'area di [!UICONTROL Project Prioritization] di [!UICONTROL Portfoli Optimizer]. Puoi esportarlo nei seguenti formati:</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>[!UICONTROL Tab] Delimitato</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferences_portfolio_optimizer.png"> </td> 
   <td>[!UICONTROL Preferenze]</td> 
   <td> <p>Utilizzare questa icona per modificare i campi del progetto visualizzati nelle colonne di [!UICONTROL Portfoli Optimizer] o per modificare i progetti visualizzati in [!UICONTROL Optimizer] in base ai relativi stati. </p> <p>Suggerimento  
     <ul> 
      <li> <p>Non tutti [!DNL Workfront] i campi standard sono disponibili per l’aggiunta nelle colonne. </p> </li> 
     </ul> 
     <ul> 
      <li> <p>Puoi aggiungere solo i campi personalizzati con un valore diverso da zero in qualsiasi progetto del portfolio.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
