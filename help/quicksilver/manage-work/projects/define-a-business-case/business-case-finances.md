---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Panoramica dei campi finanziari del Business Case
description: La scheda secondaria Caso di business include i campi finanziari per il progetto. Affinché alcuni campi finanziari abbiano valori, è necessario completare le aree corrispondenti del Business Case.
author: Becky
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 2%

---

# Panoramica dei campi finanziari del Business Case

La scheda secondaria Caso di business include i campi finanziari per il progetto. Affinché alcuni campi finanziari abbiano valori, è necessario completare le aree corrispondenti del Business Case.

Nel Business Case vengono visualizzati i seguenti campi finanziari del progetto:

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
   <td>Allineamento completato </td> 
   <td> <p>Visualizza l'allineamento del progetto in base alla relativa scorecard. Un valore percentuale elevato indica che il progetto è ben allineato con lo scopo e gli obiettivi dell’organizzazione. <br>Per ulteriori informazioni sull'utilizzo delle scorecard, vedere <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">Creare una scorecard</a>.</p> <p>Questo campo viene visualizzato nell'area Riepilogo caso di business. </p> </td> 
  </tr> 
  <tr> 
   <td>Bdg prv</td> 
   <td> <p>Costo totale stimato da associare al progetto all'avvio del progetto.</p> <p>Il costo preventivato per il progetto viene calcolato con la seguente formula:<br></p> <p><code>Budgeted Cost = Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfront utilizza le ore preventivate della Programmazione risorse per calcolare il Costo manodopera preventivato.<br>Per ulteriori informazioni sul calcolo del costo preventivato, vedere <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calcolare il costo preventivato</a>. </p> <p>Questo campo viene visualizzato nell'area Riepilogo caso di business.</p> </td> 
  </tr> 
  <tr> 
   <td>Costo spesa preventivato</td> 
   <td> <p>Il costo preventivato di tutte le spese del progetto. </p> <p>Viene calcolata con la seguente formula:</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>Per ulteriori informazioni sul calcolo delle spese, vedere <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Gestire le spese del progetto </a>.</p> <p>Questo campo viene visualizzato nell'area Spese.</p> </td> 
  </tr> 
  <tr> 
   <td>Lav Bdg prv</td> 
   <td> <p>Il costo associato alle risorse assegnate per completare il lavoro sul progetto.</p> <p>Il costo manodopera preventivato per il progetto viene calcolato con la seguente formula:<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code><br></p> <p>Workfront utilizza le ore preventivate della Programmazione risorse per calcolare il Costo manodopera preventivato.<br>Per ulteriori informazioni sul calcolo del costo manodopera preventivato, vedere <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprendere il costo manodopera preventivato e le ore preventivate per i progetti</a>.</p> <p>Questo campo viene visualizzato nell'area Budget risorse del Business Case. </p> </td> 
  </tr> 
  <tr> 
   <td>Costo pianificato spese</td> 
   <td> <p>È lo stesso del costo spesa preventivato. </p> <p>Nota: il Costo pianificato spese è diverso dal Costo pianificato per il progetto. Il Costo pianificato spese viene calcolato utilizzando l'Importo pianificato delle spese del progetto, mentre il Costo pianificato viene calcolato utilizzando le Ore pianificate del progetto. </p> <p>Questo campo viene visualizzato nell'area Spese, per ogni spesa.</p> </td> 
  </tr> 
  <tr> 
   <td>Valore Netto</td> 
   <td> <p>Si tratta del valore totale previsto del progetto dopo il calcolo del vantaggio e l'eliminazione dei costi.</p> <p>Il valore netto del progetto viene calcolato con la formula seguente:<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>. <br></p> <p>Per ulteriori informazioni sul calcolo del valore netto, vedere <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calcolare il valore netto</a>.<br></p> <p>Questo campo viene visualizzato nell'area Riepilogo caso di business.</p> </td> 
  </tr> 
  <tr> 
   <td>Benef Pian</td> 
   <td>Stima manuale del benefit monetario per l'organizzazione al completamento del progetto. Può essere una qualsiasi quantità di valuta ed è specifica per te e per ogni progetto che gestisci. Il benefit pianificato non può avere un valore negativo. Questo campo viene visualizzato nell'area Riepilogo caso di business e può essere modificato nell'area Informazioni progetto del caso di business. </td> 
  </tr> 
  <tr> 
   <td>Costo potenziale dei rischi</td> 
   <td> <p>Questo è il costo potenziale di tutti i rischi del progetto. </p> <p>Viene calcolata utilizzando la seguente formula:</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>Per ulteriori informazioni sui rischi nel progetto, vedere <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Creare e modificare i rischi nei progetti</a>.</p> <p>Questo campo viene visualizzato nell'area Riepilogo caso di business.</p> </td> 
  </tr> 
  <tr> 
   <td>Rischio Potenziale</td> 
   <td> <p>Nel Riepilogo caso di business, questo è l'importo del costo di tutti i rischi nel caso in cui si verifichino, in base alla loro probabilità. Ad esempio, se un rischio ha un costo potenziale di 100 dollari e una probabilità di verificarsi del 10%, il rischio potenziale è di 10 dollari. Il Rischio potenziale nel Riepilogo caso di business viene calcolato con la seguente formula:</p> <p><code>Potential Risk = SUM(Risk Potential Cost x Probability)</code> per tutti i rischi. </p> </td> 
  </tr> 
  <tr> 
   <td>Costo di Mitigazione del Rischio</td> 
   <td> <p>Il costo del piano di mitigazione per i rischi che si stanno stimando potrebbe verificarsi sul progetto.<br>Per ulteriori informazioni sui rischi nel progetto, vedere <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Creare e modificare i rischi nei progetti</a>.</p> <p>Questo campo viene visualizzato nell'area Rischi per ogni rischio specificato nel progetto.</p> </td> 
  </tr> 
  <tr> 
   <td>Costo potenziale per un rischio</td> 
   <td> <p>Il costo finanziario stimato quando i rischi definiti sul progetto si verificherebbero effettivamente, indipendentemente dalla loro probabilità. </p> <p>Si tratta di un campo aggiornato manualmente che viene visualizzato su ogni rischio nell'area Rischi del Business Case. </p> </td> 
  </tr> 
  <tr> 
   <td>Rischi Costo Potenziale Totale</td> 
   <td> <p>Si tratta del costo finanziario totale stimato di tutti i rischi definiti nel progetto quando si sono effettivamente verificati. </p> <p>Viene calcolata con la seguente formula:</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>Viene visualizzato come numero di valuta accanto al titolo dell'area Rischi del Business Case.</p> </td> 
  </tr> 
 </tbody> 
</table>
