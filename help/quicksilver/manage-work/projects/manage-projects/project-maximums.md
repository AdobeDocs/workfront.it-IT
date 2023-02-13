---
title: Panoramica sui limiti del progetto
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront ha dei limiti per quanti oggetti possono essere associati a un progetto. Sono stati stabiliti dei limiti per migliorare le prestazioni del prodotto e migliorare la tua esperienza con Workfront.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: 11c4028038fe3d410ee0d4f238d2138435d9a3fa
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Panoramica sui limiti del progetto

Adobe Workfront ha dei limiti per quanti oggetti possono essere associati a un progetto. Sono stati stabiliti dei limiti per migliorare le prestazioni del prodotto e migliorare la tua esperienza con Workfront.

I seguenti oggetti associati ai progetti hanno i seguenti limiti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Attività</p></td> 
   <td>  <p>Il numero massimo di attività per progetto è 5.000. Viene visualizzato un messaggio di avviso quando il numero di attività si avvicina a questo valore massimo. Una volta raggiunto il massimo, viene visualizzato un messaggio di errore e non è possibile aggiungere ulteriori attività al progetto.</p> <p>Per evitare di raggiungere questo limite massimo, sposta le attività chiuse in un altro progetto designato per le attività chiuse. Potrebbe essere necessario adeguare le relazioni relative a tali progetti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Problemi</p></td> 
   <td>  <p>Il numero massimo di problemi per progetto è 10.000. Viene visualizzato un messaggio di avviso quando il numero di problemi si avvicina a questo valore massimo. Una volta raggiunto il massimo, viene visualizzato un messaggio di errore e non è possibile aggiungere ulteriori problemi al progetto.</p> <p>Per evitare di raggiungere questo massimo, sposta i problemi chiusi in un altro progetto designato per i problemi chiusi. Potrebbe essere necessario adeguare le relazioni relative a tali progetti.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Durate</p></td> 
   <td> <p>La durata massima di un progetto deve essere di 15 anni affinché Workfront calcoli automaticamente la sua timeline. Viene visualizzato un messaggio di avviso quando la durata del progetto si avvicina al massimo. Quando viene raggiunto il massimo, viene visualizzato un messaggio di avviso e i calcoli automatici della timeline non si verificano più.</p> <p>I calcoli automatici della timeline riprenderanno non appena la durata di un progetto sarà ridotta al di sotto dei 15 anni, adeguando le date delle attività del progetto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Calcoli della timeline</p></td> 
   <td>Workfront non esegue calcoli automatici della timeline per i progetti che non sono stati aggiornati da 6 mesi e non riprenderanno finché non viene effettuato un aggiornamento.<p>Per i progetti che non sono stati aggiornati da 3 mesi, Workfront esegue i calcoli della timeline settimanali invece che notturni.</p><p>Per informazioni sul calcolo della timeline del progetto, consulta <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Ricalcolare le timeline dei progetti</a>. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->