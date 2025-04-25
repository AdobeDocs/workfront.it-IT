---
title: Panoramica sui limiti dei progetti
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront prevede dei limiti per il numero di oggetti che possono essere associati a un progetto. Sono stati stabiliti limiti di progetto per migliorare le prestazioni del prodotto e la tua esperienza con Workfront.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Panoramica sui limiti dei progetti

Adobe Workfront prevede dei limiti per il numero di oggetti che possono essere associati a un progetto. Sono stati stabiliti limiti di progetto per migliorare le prestazioni del prodotto e la tua esperienza con Workfront.

I seguenti oggetti associati ai progetti hanno i seguenti limiti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Attività</p></td> 
   <td>  <p>Il numero massimo di attività per progetto è 5.000. Quando il numero di attività si avvicina a questo valore massimo, viene visualizzato un messaggio di avviso. Quando viene raggiunto il numero massimo, viene visualizzato un messaggio di errore e non è possibile aggiungere altre attività al progetto.</p> <p>Per evitare di raggiungere questo limite massimo, sposta le attività chiuse in un altro progetto designato per le attività chiuse. Potrebbe essere necessario adeguare le relazioni su tali progetti.</p>

<b>IMPORTANTE</b>

Per i progetti in cui le attività hanno molte dipendenze, si potrebbe verificare un peggioramento delle prestazioni durante il calcolo della sequenza temporale o durante l&#39;utilizzo del progetto.

Per questo motivo, si consiglia che il numero di attività nei progetti con dipendenze complesse sia molto inferiore al massimo consentito di 5.000 attività.

Di seguito sono riportati alcuni esempi di relazioni tra attività che possono influenzare o impedire il ricalcolo della sequenza temporale del progetto:

<ul><li>Numero di figli</li>
   <li>Rientro attività a più livelli</li>
   <li>Numero di predecessori</li>
   <li>Assegnazioni multiple</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Problemi</p></td> 
   <td>  <p>Il numero massimo di problemi per progetto è 10.000. Quando il numero di problemi si avvicina a questo valore massimo, viene visualizzato un messaggio di avviso. Quando viene raggiunto il numero massimo, viene visualizzato un messaggio di errore e non è possibile aggiungere altri problemi al progetto.</p> <p>Per evitare di raggiungere questo limite massimo, sposta i problemi chiusi in un altro progetto designato per i problemi chiusi. Potrebbe essere necessario adeguare le relazioni su tali progetti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Durate</p></td> 
   <td> <p>La durata massima di un progetto deve essere di 15 anni per consentire a Workfront di calcolarne automaticamente la timeline. Quando la durata del progetto si avvicina al valore massimo, viene visualizzato un messaggio di avvertenza. Quando viene raggiunto il valore massimo, viene visualizzato un messaggio di avvertenza e i calcoli automatici della sequenza temporale non vengono più eseguiti.</p> <p>I calcoli automatici della sequenza temporale riprenderanno non appena la durata di un progetto sarà ridotta al di sotto di 15 anni, adeguando le date delle attività del progetto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Calcoli della sequenza temporale</p></td> 
   <td>Workfront non esegue calcoli automatici della sequenza temporale per i progetti che non vengono aggiornati da 6 mesi e non riprenderanno finché non viene effettuato un aggiornamento.<p>Per i progetti che non vengono aggiornati da tre mesi, Workfront esegue calcoli della sequenza temporale settimanalmente anziché ogni notte.</p><p>Per informazioni sul calcolo della sequenza temporale del progetto, vedere <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Ricalcolare le sequenze temporali del progetto</a>. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->
