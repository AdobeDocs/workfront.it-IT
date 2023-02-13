---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Panoramica dei campi finanziari del Business Case
description: La sottoscheda Business case include campi finanziari per il progetto. Affinché alcuni campi finanziari abbiano valori, è necessario completare le aree corrispondenti del Business Case.
author: Alina
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 2%

---

# Panoramica dei campi finanziari del Business Case

La sottoscheda Business case include campi finanziari per il progetto. Affinché alcuni campi finanziari abbiano valori, è necessario completare le aree corrispondenti del Business Case.  

I seguenti campi finanziari del progetto vengono visualizzati nel Business Case:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="col">Nome del campo</th> 
   <th scope="col">Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Allineamento completato </td> 
   <td> <p>Visualizza l’allineamento del progetto in base alla relativa scorecard. Un valore percentuale elevato indica che il progetto è ben allineato con lo scopo e gli obiettivi dell’organizzazione. <br>Per ulteriori informazioni sull’utilizzo delle scorecard, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">Creare una scorecard</a>.</p> <p>Questo campo viene visualizzato nell'area Riepilogo del caso aziendale. </p> </td> 
  </tr> 
  <tr> 
   <td>Bdg prv</td> 
   <td> <p>Costo totale stimato associato al progetto all’avvio del progetto.</p> <p>Il costo preventivato per il progetto viene calcolato con la seguente formula:<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Per calcolare il costo del lavoro preventivato, in Adobe Workfront vengono utilizzate le ore previste dal planner risorse.<br>Per ulteriori informazioni sul calcolo del costo preventivato, vedere <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calcola costo preventivato</a>. </p> <p>Questo campo viene visualizzato nell'area Riepilogo del caso aziendale.</p> </td> 
  </tr> 
  <tr> 
   <td>Costo spesa preventivato</td> 
   <td> <p>Costo preventivato di tutte le spese del progetto. </p> <p>Viene calcolata con la seguente formula:</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>Per ulteriori informazioni sul calcolo delle spese, vedere <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Gestione delle spese di progetto </a>.</p> <p>Questo campo viene visualizzato nell'area Spese.</p> </td> 
  </tr> 
  <tr> 
   <td>Lav Bdg prv</td> 
   <td> <p>Costo associato alle risorse assegnate per completare il lavoro sul progetto.</p> <p>Il costo del lavoro a budget per il progetto viene calcolato con la seguente formula:<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code></p> <p>Per calcolare il costo del lavoro preventivato, in Workfront vengono utilizzate le ore previste dal planner risorse.<br>Per ulteriori informazioni sul calcolo del costo del lavoro a budget, vedere <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprendere i costi del lavoro e le ore previste per i progetti</a>.</p> <p>Questo campo viene visualizzato nell'area Resource Budgeting del Business Case. </p> </td> 
  </tr> 
  <tr> 
   <td>Costi pianificati</td> 
   <td> <p>È lo stesso del costo di spesa a budget. </p> <p>Nota: Il costo pianificato delle spese è diverso dal costo pianificato per il progetto. Il costo pianificato delle spese viene calcolato come Importo pianificato delle spese del progetto, mentre il costo pianificato viene calcolato utilizzando le ore pianificate del progetto. </p> <p>Questo campo viene visualizzato nell'area Spese per ogni spesa.</p> </td> 
  </tr> 
  <tr> 
   <td>Valore Netto</td> 
   <td> <p>Si tratta del valore totale previsto del progetto dopo il calcolo del suo vantaggio e l'eliminazione dei costi.</p> <p>Il valore netto per il progetto viene calcolato con la seguente formula:<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>. <br></p> <p>Per ulteriori informazioni sul calcolo del valore netto, vedere <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calcola valore netto</a>.<br></p> <p>Questo campo viene visualizzato nell'area Riepilogo del caso aziendale.</p> </td> 
  </tr> 
  <tr> 
   <td>Benef Pian</td> 
   <td>Una stima manuale del vantaggio monetario per la tua organizzazione al termine del progetto. Può trattarsi di qualsiasi importo di valuta ed è specifico per te e per ogni progetto gestito. Il beneficio pianificato non può avere un valore negativo. Questo campo viene visualizzato nell'area Riepilogo del caso aziendale e può essere modificato nell'area Informazioni progetto del caso aziendale. </td> 
  </tr> 
  <tr> 
   <td>Costo potenziale dei rischi</td> 
   <td> <p>Questo è il costo potenziale di tutti i rischi sul progetto. </p> <p>Viene calcolata utilizzando la seguente formula:</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>Per ulteriori informazioni sui rischi relativi al progetto, consulta <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Creare e modificare i rischi relativi ai progetti</a>.</p> <p>Questo campo viene visualizzato nell'area Riepilogo del caso aziendale.</p> </td> 
  </tr> 
  <tr> 
   <td>Rischio Potenziale</td> 
   <td> <p>Nel Business Case Summary, si tratta dell'importo del costo di tutti i rischi, se necessario, in base alla loro probabilità. Ad esempio, se un rischio ha un costo potenziale di 100 $ e una probabilità di verificarsi del 10%, il rischio potenziale è di 10 $. Il rischio potenziale nel Business Case Summary è calcolato con la seguente formula:</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> per tutti i rischi. </p> </td> 
  </tr> 
  <tr> 
   <td>Costo di attenuazione del rischio</td> 
   <td> <p>Il costo del piano di mitigazione per i rischi stimati potrebbe verificarsi sul progetto.<br>Per ulteriori informazioni sui rischi relativi al progetto, consulta <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Creare e modificare i rischi relativi ai progetti</a>.</p> <p>Questo campo viene visualizzato nell’area Rischi per ogni rischio specificato nel progetto.</p> </td> 
  </tr> 
  <tr> 
   <td>Costo potenziale per un rischio</td> 
   <td> <p>Il costo finanziario stimato quando i rischi definiti sul progetto si verificherebbero effettivamente, indipendentemente dalla loro probabilità. </p> <p>Si tratta di un campo aggiornato manualmente che viene visualizzato su ogni rischio nell'area Rischi del Business Case. </p> </td> 
  </tr> 
  <tr> 
   <td>Rischi Costo potenziale totale</td> 
   <td> <p>Si tratta del costo finanziario totale stimato di tutti i rischi definiti sul progetto quando si sono effettivamente verificati. </p> <p>Viene calcolata con la seguente formula:</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>Viene visualizzato come un numero di valuta accanto al titolo dell'area Rischi del Business Case.</p> </td> 
  </tr> 
 </tbody> 
</table>
