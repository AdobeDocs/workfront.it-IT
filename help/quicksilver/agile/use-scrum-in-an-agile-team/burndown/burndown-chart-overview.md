---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Panoramica del grafico a burn-down Agile
description: Il grafico burndown fornisce una rappresentazione visiva dell'avanzamento delle storie nell'iterazione o nel progetto. Il tasso di burndown effettivo viene misurato rispetto al tasso di burndown ideale per l’iterazione o la timeline del progetto.
author: Lisa
feature: Agile
exl-id: 414e3315-35ed-4aa4-a2d8-be42ec585f29
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# Panoramica del grafico a burn-down Agile

Il grafico a burn-down fornisce una rappresentazione visiva dell&#39;avanzamento delle storie nell&#39;iterazione. Il tasso di burndown effettivo viene misurato rispetto al tasso di burndown ideale per la timeline di iterazione.

Il grafico a burn-down viene regolato in base al giorno selezionato. Il giorno corrente è quello predefinito. Quando viene selezionato un giorno precedente, tutti i dati nel grafico a discesa e tutti i valori nel [!UICONTROL stato di completamento] sopra il grafico a dispersione vengono ricalcolati per rappresentare i dati così come erano alla fine del giorno selezionato. È possibile selezionare i giorni passati o il giorno corrente, ma non i giorni futuri.

![](assets/agile-iteration-burndown-350x88.png)

## Indicatori visivi

Il grafico a burn-down contiene i seguenti indicatori visivi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-dottedblue.png" alt=""> </td> 
   <td> <p>Percentuale di burndown ideale in base a quando è iniziata l'iterazione.</p> <p>Questa riga non viene visualizzata se l’ambito dell’iterazione non cambia mai (le ore o i punti non vengono mai aggiunti o rimossi).</p> <p>Questa linea viene visualizzata come piatta quando il lavoro viene eseguito in un giorno libero. Per ulteriori informazioni, consulta <a title="Utilizzo del grafico Burndown Agile" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">Effetti dei giorni liberi sul grafico a dispersione</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-solidblue.png" alt=""> </td> 
   <td> <p>Percentuale di burndown ideale in base alle storie o alle attività correnti.</p> <p>La velocità di burn-down ideale corrente (linea blu continua) differisce dalla velocità di burndown ideale originale (linea blu punteggiata) quando le ore o i punti vengono aggiunti o rimossi dall'iterazione dopo l'inizio dell'iterazione.</p> <p>Questa linea viene visualizzata come piatta quando il lavoro viene eseguito in un giorno libero.</p> <p>Per ulteriori informazioni, consulta <a title="Utilizzo del grafico Burndown Agile" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">Effetti dei giorni liberi sul grafico a dispersione</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-red.png" alt=""> </td> 
   <td> <p>Il tasso di burndown effettivo viene visualizzato in rosso quando il tasso di burndown è inferiore all’ideale (più punti o ore rimanenti al giorno rispetto al calcolo del burndown ideale).</p> <p>La formula seguente viene utilizzata per calcolare il tasso di burn-down effettivo:</p> <p>[SOMMA (valore punto o ora del lavoro in corso * percentuale di completamento) + valore punto o ora del lavoro completato]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-green.png" alt=""> </td> 
   <td> <p>Il tasso di burndown effettivo viene visualizzato in verde quando il tasso di burndown è uguale o migliore dell’ideale (sono rimasti meno punti al giorno del calcolo del burndown ideale).</p> <p>La formula seguente viene utilizzata per calcolare il tasso di burn-down effettivo:</p> <p>[SOMMA (valore punto o ora del lavoro in corso * percentuale di completamento) + valore punto o ora del lavoro completato]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>Modifica dell’ambito (le ore o i punti vengono aggiunti o rimossi dall’iterazione).</p> <p>Le modifiche di ambito vengono sempre visualizzate come una linea verticale a metà giornata. Inoltre, un punto blu viene visualizzato nel mezzo di qualsiasi giorno in cui si è verificata una modifica dell’ambito.</p> <p>L'asse verticale del grafico a bruciatura mostra i punti o le ore del brano.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>Modifica nell’intervallo di date (la durata dell’iterazione aumenta o diminuisce).</p> <p>Un punto blu viene visualizzato al centro di qualsiasi giorno in cui la durata dell'iterazione è stata modificata.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>Un punto verde o rosso viene visualizzato sulla frequenza di masterizzazione effettiva ogni volta che il lavoro viene masterizzato. (Quando il tasso di burn-down effettivo in quel giorno è rosso, il punto è rosso; quando il tasso di burndown effettivo in quel giorno è verde, il punto è verde.)</p> <p>Il lavoro viene masterizzato quando si verifica una delle seguenti situazioni:</p> 
    <ul> 
     <li> Il [!UICONTROL Percent Complete] viene aumentato nella storia.<br>[!UICONTROL Percent Complete] viene aumentato quando: 
      <ul> 
       <li> <p>Modificato manualmente</p> </li> 
       <li> <p>Il numero di punti o ore viene aggiornato sulla storia</p> </li> 
      </ul></li>  
     <li>Lo stato del brano è cambiato in [!UICONTROL Complete]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Effetti dei giorni liberi sul grafico a dispersione {#how-days-off-affect-the-burndown-chart}

La pianificazione predefinita definita in [!DNL Workfront] influisce sul grafico burndown escludendo i giorni liberi (fine settimana e festivi) dal burndown. Il grafico a dispersione utilizza la pianificazione predefinita per definire i giorni lavorativi (come descritto in  [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)).

I team agili possono incorporare giorni non lavorativi specifici del team definendo una pianificazione alternativa (come descritto nell’articolo [Utilizzare una pianificazione alternativa per i grafici a dispersione](../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md)). Questa pianificazione alternativa viene quindi riportata nel grafico a discesa di qualsiasi iterazione assegnata al team. La pianificazione alternativa influisce solo sul grafico a dispersione.

I giorni liberi vengono riportati nel grafico a dispersione solo se:

* Il lavoro era stato precedentemente registrato in un giorno di ferie. (Viene visualizzato il giorno in cui è stato registrato il lavoro.)

  Quando il lavoro viene registrato in un giorno libero:

   * Qualsiasi lavoro registrato non viene incluso nel calcolo del burn-down ideale perché il team non è programmato per eseguire alcun lavoro.
   * Le linee di burn-down ideali (la linea blu continua e la linea blu tratteggiata) vengono visualizzate come piatte nel grafico burndown per qualsiasi giorno in cui il lavoro è stato completato o nel giorno in cui si sta visualizzando il grafico burndown (se si sta visualizzando in un giorno libero).
   * Il lavoro registrato viene incluso nel calcolo di altre statistiche di burndown come il completamento stimato e la media di punti o ore al giorno.

* Stai visualizzando il grafico a bruciatura in un giorno libero. Il giorno visualizzato viene visualizzato nel grafico a dispersione.
* Il lavoro rimanente totale per l&#39;iterazione viene completato in un giorno libero.

  Quando un utente completa il lavoro rimanente totale per l’iterazione in un giorno libero, il [!UICONTROL Completamento stimato] visualizza la data in cui è stata completata l’iterazione.

  Quando si pianifica l&#39;iterazione, se si imposta la data di fine dell&#39;iterazione per un giorno non lavorativo e si tiene traccia della fine puntuale dell&#39;iterazione, [!UICONTROL Completamento stimato] la data viene impostata per l&#39;ultimo giorno lavorativo precedente alla data di fine dell&#39;iterazione impostata (poiché il lavoro non è programmato per essere masterizzato in giorni non lavorativi).

  La data di fine dell&#39;iterazione viene specificata quando l&#39;iterazione viene pianificata, come descritto nell&#39;articolo [Creare un’iterazione](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
