---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Panoramica sullo stato e sull’avanzamento della bozza
description: È possibile visualizzare informazioni sull'avanzamento di una bozza nel processo di revisione e visualizzare un riepilogo generale dello stato di decisione della bozza dall'area Documenti.
author: Courtney
feature: Digital Content and Documents
exl-id: 78e81070-ff82-4d82-90a3-6e0cd176b290
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 1%

---

# Panoramica sullo stato e sull’avanzamento della bozza

È possibile visualizzare informazioni sull&#39;avanzamento di una bozza nel processo di revisione e visualizzare un riepilogo generale dello stato di decisione della bozza dall&#39;area Documenti.

## Panoramica sull’avanzamento della bozza

L’avanzamento della bozza indica il lavoro svolto su una bozza dal momento dell’invio della bozza ai destinatari al momento in cui prendono una decisione sulla bozza. Accanto al nome della bozza vengono visualizzate le icone di avanzamento S, O, C e D che forniscono informazioni sull’avanzamento della bozza.

![Stato di avanzamento della modifica di elementi esistenti](assets/proof-edit-existing-progress-350x62.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Icona avanzamento</strong> </p> </td> 
   <td> <p><strong>Descrizione</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt=""> </p> <p><strong>Inviato</strong> </p> </td> 
   <td> <p>La bozza è stata inviata ai destinatari assegnati.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>Aperto</strong> </p> </td> 
   <td> <p>Tutti i destinatari assegnati aprono la pagina Dettagli bozza o Bozza.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>Commenti effettuati</strong> </p> </td> 
   <td> <p>Tutti i destinatari assegnati aggiungono almeno un commento alla bozza.</p> <p>Se alla bozza non sono assegnati revisori, l'icona <strong>C</strong> non viene visualizzata sulla barra di avanzamento.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt=""> </p> <p><strong>Decisione effettuata</strong> </p> </td> 
   <td> <p>Tutti gli approvatori assegnati prendono una decisione sulla bozza, Tutti gli approvatori assegnati prendono una decisione sulla bozza, a meno che il creatore della bozza non specifichi che è necessaria una sola decisione.</p> <p>Se non sono presenti approvatori (responsabili delle decisioni) designati per la bozza, l'icona <strong>D</strong> non viene visualizzata nella barra di avanzamento. </p> </td> 
  </tr> 
 </tbody> 
</table>

Le icone di avanzamento possono essere visualizzate nei seguenti colori per indicare determinate informazioni sull’avanzamento della bozza:

* **Verde**: completato.
* **Bianco**: non completato.
* **Arancione**: non completato e scadenza inferiore a 24 ore.
* **Rosso**: non completato e scaduto il termine.

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Levels of proof progress</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront Proof uses the progress icons to track a proof's progress at each of the following levels:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each reviewer, based on that person's activity on the proof.&nbsp;</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each stage, based on the progress the reviewer on the stage who is most behind in the proofing process.&nbsp;To learn more about stages, see <a href="../../../review-and-approve-work/proofing/proofing-overview/stages.md" class="MCXref xref">Automated Workflow Stages overview</a>.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For the proof, based on the progress of the stage (group of reviewers) who is the most behind in the proofing process.</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For an example of how Workfront Proof determines progress using the reviewer or stage that is most behind,&nbsp;suppose three reviewers on a proof need to make a&nbsp;decision. If two of them have made their&nbsp;decision&nbsp;but the third has not, the progress bar for the proof does not show&nbsp;the D in green because of the outstanding&nbsp;decision.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If the Primary Decision Maker setting is selected on a proof and the primary decision maker submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Similarly, if the Only One Decision Required setting is selected on a proof and any reviewer submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

## Panoramica sullo stato della bozza

Lo stato della bozza visualizza lo stato delle decisioni necessarie per la bozza. Lo stato della bozza è determinato dal partecipante che si trova nel &quot;caso peggiore&quot;. Si supponga, ad esempio, di avere tre decisioni sulla bozza: due hanno lo stato **Accettato** e uno ha lo stato **Rifiutato**. La decisione &quot;caso peggiore&quot; di **Rifiutato** sovrascrive le altre decisioni e lo stato complessivo della bozza viene visualizzato come **Rifiutato**. 

![Stato modifica bozza esistente](assets/proof-edit-existing-progress-350x62.png)

Le opzioni di stato standard sono le seguenti:

* In Attesa
* Approvato
* Approvato con modifiche
* Modifiche richieste
* Non pertinente

Se nel tuo account sono configurate decisioni personalizzate, le opzioni di stato riflettono le impostazioni di decisione personalizzate.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Viewing proof progress and status</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> You can view the progress and status of proofs for individual documents. </p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-progress-and-status-for-a-document" class="MCXref xref">View proof progress and status&nbsp;for a document</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-approval-information-in-home" class="MCXref xref">View proof approval information&nbsp;in Home</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-progress-and-status-for-a-document">View proof progress and status&nbsp;for a document</h3>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">If a proof has not already been generated for the document in Adobe Workfront, generate it, as described in the articles.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Documents area, under the proof's name, click <strong>Proof Details</strong>.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Proofing Details</strong> box that appears, the proof's progress for each stage, then click <strong>Done</strong>.</li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Under the proof's name, click <strong>Proofing Workflow</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <img src="assets/click-proofing-workflow-qs-350x149.png" style="width: 350;height: 149;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
   -->
<!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   These screenshots will need to change with new terminology ("Review Workflow" for this one?)
   </MadCap:conditionalText>
   <br> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Workflow information that appears, scroll down to see the proof's progress for each stage:</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/scroll-to-see-socd-for-stages-qs-350x152.png" style="width: 350;height: 152;"> </p>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-approval-information-in-home">View proof approval information&nbsp;in Home</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can view information about proofs that you have submitted for approval. Proof approval information is displayed in the Home area only while the proof is pending approval.&nbsp;For information about how to view information about proof approvals in the Home area, see&nbsp;<a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">View approvals </a>.</p>
-->
