---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: "Panoramica sul tipo di durata: lavoro calcolato"
description: Il Lavoro calcolato è un Tipo di Durata che è possibile impostare per un'attività in Adobe Workfront. Per informazioni generali sui tipi di durata in Workfront, vedere Panoramica sulla durata e sul tipo di durata dell'attività.
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 1%

---

# Panoramica sul tipo di durata: lavoro calcolato

Il Lavoro calcolato è un Tipo di Durata che è possibile impostare per un&#39;attività in Adobe Workfront. Per informazioni generali sui tipi di durata in Workfront, vedere [Panoramica sulla durata dell&#39;attività e sul tipo di durata](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Panoramica del tipo di durata del lavoro calcolato

Lavoro calcolato determina la quantità di lavoro (ore pianificate) necessario per il completamento dell&#39;attività. È consigliabile utilizzare il Tipo di durata lavoro calcolato quando le risorse assegnate all&#39;attività vengono allocate per l&#39;intera durata dell&#39;attività.

Il Workfront o un amministratore di gruppo può impostare il Tipo di durata predefinito del sistema o del gruppo come Lavoro calcolato. In questo caso, tutte le nuove attività verranno create con questo Tipo di durata. Per informazioni sulla modifica delle preferenze di attività e problemi come parte delle preferenze di progetto a livello di sistema o di gruppo, consulta [Configurare le preferenze di problema e attività a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Quando si aggiungono risorse a un&#39;attività, un project manager può aspettarsi di vedere l&#39;aumento di impegno pianificato. A titolo illustrativo, una riunione di pianificazione di un&#39;ora con tre risorse rappresenta tre ore di lavoro totali richieste e una riunione di pianificazione di un&#39;ora con dieci risorse rappresenta dieci ore di lavoro richieste. Ciò presuppone che ogni risorsa sia assegnata all&#39;attività con un&#39;allocazione del 100%.

## Esaminare la formula per il calcolo del Lavoro richiesto quando si utilizza il Tipo di durata lavoro calcolato

Quando si utilizza il Tipo di durata lavoro calcolato per un&#39;attività, Workfront calcola la quantità di lavoro per ogni attività utilizzando le due formule seguenti. Le formule variano a seconda della percentuale di tempo assegnata a ogni risorsa e del numero di risorse assegnate a ogni attività:

* Formula semplificata: se all&#39;attività è assegnata una risorsa e tale risorsa viene assegnata per il 100% del tempo disponibile, il valore Lavoro richiesto per ogni attività viene calcolato con la formula seguente:

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* Formula complessa: se si assegna ogni risorsa con varie allocazioni, la formula tiene conto di queste allocazioni e tiene conto delle variazioni seguenti:

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## Verificare l&#39;effetto dell&#39;aggiunta o della rimozione di risorse dall&#39;attività

Quando si aggiungono o rimuovono assegnatari a un&#39;attività con il tipo di durata Lavoro calcolato, la Durata può essere modificata manualmente. Quando gli assegnatari vengono aggiunti o rimossi dall&#39;attività, le ore pianificate cambiano.

Nell’esempio seguente, le Ore tipiche per giorno lavorativo sono impostate su 8 nelle Preferenze progetto in Configurazione. Ogni attività ha una durata di 1 giorno. Quando cambia il numero di assegnatari, le ore pianificate cambiano in base al numero di assegnatari in una determinata attività:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Numero di assegnatari (ogni 100% allocato)</strong> </p> </th> 
   <th> <p><strong>Durata</strong> </p> </th> 
   <th> <p><strong>Ore pianificate</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>1</p> </td> 
   <td> <p>1 giorno</p> </td> 
   <td> <p>8 Hours</p> <p>(1 giorno x 8 ore per giorno lavorativo x 1 assegnatario = 8 ore pianificate)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>2</p> </td> 
   <td> <p>1 giorno</p> </td> 
   <td> <p>16 ore</p> <p>(1 giorno x 8 ore per giorno lavorativo x 2 assegnatari = 16 ore pianificate)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1 giorno</p> </td> 
   <td> <p>24 Hours</p> <p>(1 giorno x 8 ore per giorno lavorativo x 3 assegnatari = 24 ore pianificate)</p> </td> 
  </tr> 
 </tbody> 
</table>

In questo caso, ogni assegnatario è assegnato al 100% all&#39;attività Lavoro calcolato.

![](assets/calcwork-350x71.png)

## Modificare il Tipo di durata di un&#39;attività in Lavoro calcolato

Per informazioni sulla modifica del tipo di durata di un&#39;attività, vedere [Aggiornare il tipo di durata di un&#39;attività](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Work</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
