---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Panoramica del grafico a discesa Agile
description: Il grafico a discesa fornisce una rappresentazione visiva del progresso dei racconti attraverso l’iterazione o il progetto . Il tasso di abbandono effettivo viene misurato in base al tasso di abbandono ideale per l’iterazione o la timeline del progetto.
author: Lisa
feature: Agile
exl-id: 414e3315-35ed-4aa4-a2d8-be42ec585f29
source-git-commit: 373f2522b85196d6395f189ae6cfe03449cac61a
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# Panoramica del grafico a discesa Agile

Il grafico a discesa fornisce una rappresentazione visiva del progresso delle storie attraverso l&#39;iterazione. Il tasso di abbandono effettivo viene misurato in base al tasso di abbandono ideale per la timeline dell’iterazione.

Il grafico a discesa si regola in base al giorno selezionato. Il giorno corrente è quello predefinito. Quando selezioni un giorno precedente, tutti i dati nel grafico a discesa e tutti i valori nel [!UICONTROL stato di completamento] la sezione sopra il grafico a discesa viene ricalcolata per rappresentare i dati come alla fine del giorno selezionato. (È possibile selezionare gli ultimi giorni o il giorno corrente; non è possibile selezionare giorni in futuro.)

![](assets/agile-iteration-burndown-350x88.png)

## Indicatori visivi

Il grafico a discesa contiene i seguenti indicatori visivi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-dottedblue.png" alt=""> </td> 
   <td> <p>Tasso di esaurimento ideale in base all’inizio dell’iterazione.</p> <p>Questa riga non viene visualizzata se l’ambito dell’iterazione non cambia mai (ore o punti non vengono mai aggiunti o rimossi).</p> <p>Questa linea viene visualizzata come piatta quando il lavoro viene svolto in un giorno libero. Per ulteriori informazioni, consulta <a title="Utilizzo del grafico a discesa Agile" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">Effetti dei giorni di inattività sul grafico a discesa</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-solidblue.png" alt=""> </td> 
   <td> <p>Tasso di esaurimento ideale in base alle storie o ai compiti correnti.</p> <p>Il tasso di abbandono ideale attuale (linea blu piena) differisce dal tasso di abbandono ideale originale (linea blu punteggiata) quando le ore o i punti vengono aggiunti o rimossi dall’iterazione dopo l’inizio dell’iterazione.</p> <p>Questa linea viene visualizzata come piatta quando il lavoro viene svolto in un giorno libero.</p> <p>Per ulteriori informazioni, consulta <a title="Utilizzo del grafico a discesa Agile" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">Effetti dei giorni di inattività sul grafico a discesa</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-red.png" alt=""> </td> 
   <td> <p>Il tasso di abbandono effettivo viene visualizzato in rosso quando il tasso di abbandono è inferiore all’ideale (più punti o ore rimanenti al giorno rispetto al calcolo di esaurimento ideale).</p> <p>La formula seguente viene utilizzata per calcolare il tasso di raggruppamento effettivo:</p> <p>[SOMMA(Valore al punto o all'ora del lavoro in corso * Percentuale completamento) + Valore al punto o all'ora del lavoro completato]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-green.png" alt=""> </td> 
   <td> <p>Il tasso di abbandono effettivo viene mostrato in verde quando il tasso di raggruppamento è uguale o migliore dell’ideale (pari o inferiore ai punti rimanenti al giorno rispetto al calcolo di raggruppamento ideale).</p> <p>La formula seguente viene utilizzata per calcolare il tasso di raggruppamento effettivo:</p> <p>[SOMMA(Valore al punto o all'ora del lavoro in corso * Percentuale completamento) + Valore al punto o all'ora del lavoro completato]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>Modifica dell’ambito (le ore o i punti vengono aggiunti o rimossi dall’iterazione).</p> <p>Le modifiche all’ambito vengono sempre visualizzate come linea verticale al centro della giornata. Inoltre, un punto blu viene visualizzato nel mezzo di qualsiasi giorno in cui si è verificata una modifica dell’ambito.</p> <p>L'asse verticale del grafico a discesa mostra i punti o le ore del brano.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>Modifica dell’intervallo di date (la durata dell’iterazione viene aumentata o diminuita).</p> <p>Un punto blu viene visualizzato a metà di qualsiasi giorno in cui è stata modificata la durata dell’iterazione.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>Un punto verde o rosso viene visualizzato sul tasso di abbandono effettivo ogni volta che il lavoro viene bruciato. (Quando il tasso di abbandono effettivo in quel giorno è rosso, il punto è rosso; quando il tasso di abbandono effettivo in quel giorno è verde, il punto è verde.)</p> <p>Il lavoro viene bruciato quando si verifica uno dei seguenti casi:</p> 
    <ul> 
     <li> La percentuale di completamento viene aumentata sulla storia.<br>La percentuale di completamento viene aumentata quando: 
      <ul> 
       <li> <p>Modificato manualmente</p> </li> 
       <li> <p>Il numero di punti o ore viene aggiornato sulla storia</p> </li> 
      </ul></li>  
     <li>Lo stato della storia viene modificato in [!UICONTROL Complete]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Effetti dei giorni di inattività sul grafico a discesa {#how-days-off-affect-the-burndown-chart}

La pianificazione predefinita definita in [!DNL Workfront] influenza il grafico a discesa escludendo i giorni di inattività (fine settimana e festività) dal menu a discesa. Il grafico a discesa utilizza la pianificazione predefinita per definire i giorni lavorativi (come descritto in  [Creare una pianificazione](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)).

I team Agile possono incorporare giorni non lavorativi specifici del team definendo una pianificazione alternativa (come descritto nell’articolo [Utilizzare una pianificazione alternativa del team per i grafici a discesa](../../../agile/use-scrum-in-an-agile-team/burndown/use-alt--team-schedule-burndown-charts.md)). Questa pianificazione alternativa viene quindi visualizzata nel grafico a discesa di qualsiasi iterazione assegnata al team. La pianificazione alternativa influisce solo sul grafico a discesa.

I giorni liberi vengono riportati nel grafico a discesa solo se:

* Il lavoro è stato precedentemente registrato un giorno di inattività. (Viene visualizzato il giorno in cui il lavoro è stato registrato).

   Quando il lavoro viene connesso in un giorno di inattività:

   * Qualsiasi lavoro registrato non è incluso nel calcolo del raggruppamento ideale perché il team non è pianificato per eseguire alcun lavoro.
   * Le linee a discesa ideali (linea blu piena e linea blu tratteggiata) vengono visualizzate come piatte nel grafico a discesa per qualsiasi giorno in cui il lavoro è stato completato o il giorno in cui si sta visualizzando il grafico a discesa (se si sta visualizzando in un giorno libero).
   * Il lavoro registrato è incluso nel calcolo di altre statistiche di suddivisione, come il completamento stimato e i punti o le ore medie al giorno.

* Il grafico a discesa viene visualizzato in un giorno libero. Il giorno visualizzato viene visualizzato nel grafico a discesa.
* Il lavoro totale rimanente per l&#39;iterazione viene completato in un giorno libero.

   Quando un utente completa il lavoro totale rimanente per l&#39;iterazione in un giorno libero, il [!UICONTROL Completamento stimato] visualizza la data di completamento dell’iterazione.

   Quando si pianifica l&#39;iterazione, se si imposta la data di fine dell&#39;iterazione per un giorno non lavorativo e l&#39;iterazione sta eseguendo il monitoraggio per terminare in tempo, la [!UICONTROL Completamento stimato] La data viene impostata per l&#39;ultimo giorno lavorativo precedente alla data di fine dell&#39;iterazione impostata (perché il lavoro non è pianificato per essere bruciato nei giorni non lavorativi).

   La data di fine dell’iterazione viene specificata al momento della pianificazione dell’iterazione, come descritto nell’articolo [Creare un’iterazione](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
