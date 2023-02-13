---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '''Panoramica sul tipo di durata: Lavoro calcolato"'
description: Il lavoro calcolato è un tipo di durata che è possibile impostare per un'attività in Adobe Workfront. Per informazioni generali sui tipi di durata in Workfront, consulta Panoramica sulla durata e sul tipo di durata dell’attività.
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 1%

---

# Panoramica sul tipo di durata: Lavoro calcolato

Il lavoro calcolato è un tipo di durata che è possibile impostare per un&#39;attività in Adobe Workfront. Per informazioni generali sui tipi di durata in Workfront, vedi [Panoramica del tipo di durata e durata dell’attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Panoramica del tipo di durata del lavoro calcolato

Lavoro calcolato determina la quantità di lavoro (ore pianificate) necessaria per il completamento dell&#39;attività. È consigliabile utilizzare il tipo di durata del lavoro calcolato quando le risorse assegnate all&#39;attività vengono allocate per l&#39;intera durata dell&#39;attività.

L&#39;amministratore di Workfront o di gruppo può impostare il tipo di durata predefinito del sistema o del gruppo come Lavoro calcolato. In questo caso, tutte le nuove attività verranno create con questo tipo di durata. Per informazioni su come modificare l&#39;attività e le preferenze relative ai problemi nell&#39;ambito delle preferenze di progetto a livello di sistema o di gruppo, consulta [Configurare le preferenze relative alle attività e ai problemi a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Man mano che le risorse vengono aggiunte a un’attività, un project manager può prevedere un aumento dello sforzo pianificato. Ad esempio, una riunione di pianificazione di un&#39;ora con tre risorse rappresenta tre ore di lavoro totali richieste e una riunione di pianificazione di un&#39;ora con dieci risorse rappresenta dieci ore di lavoro necessarie. Ciò presuppone che ogni risorsa sia allocata all&#39;attività con allocazione al 100%.

## Rivedere la formula per il calcolo del lavoro richiesto quando si utilizza il tipo di durata del lavoro calcolato

Quando si utilizza il tipo di durata del lavoro calcolato su un&#39;attività, Workfront calcola la quantità di lavoro per ogni attività utilizzando le due formule seguenti. Le formule variano a seconda della percentuale di tempo che ogni risorsa viene allocata all&#39;attività e del numero di risorse assegnate a ciascuna attività:

* Formula semplificata: Se all&#39;attività è assegnata una risorsa e questa viene assegnata per il 100% del tempo disponibile, il valore Work Required per ogni attività viene calcolato utilizzando la seguente formula:

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* Formula complessa: Se assegni ogni risorsa con varie allocazioni, la formula tiene conto di queste allocazioni e tiene conto di queste variazioni:

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## Rivedere l’effetto dell’aggiunta o della rimozione di risorse dall’attività

Quando si aggiungono o rimuovono assegnatari a un&#39;attività con il tipo di durata del lavoro calcolato, la durata può essere modificata manualmente. Man mano che gli assegnatari vengono aggiunti o rimossi dall&#39;attività, le ore pianificate cambiano.

Nell’esempio seguente, l’opzione Ore tipiche per giorno di lavoro è impostata su 8 nelle Preferenze progetto in Configurazione. Ogni attività ha una Durata di 1 giorno. Man mano che il numero di assegnatari cambia, l&#39;ora pianificata cambia in base al numero di assegnatari di una determinata attività:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Numero di assegnatari (ogni 100% allocato)</strong> </p> </th> 
   <th> <p><strong>Durata</strong> </p> </th> 
   <th> <p><strong>Lavoro Necessario</strong> </p> </th> 
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
   <td> <p>16 ore</p> <p>(1 giorno x 8 ore per giorno lavorativo x 2 assegnatari = 16 ore previste)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1 giorno</p> </td> 
   <td> <p>24 Hours</p> <p>(1 giorno x 8 ore per giorno lavorativo x 3 assegnatari = 24 ore previste)</p> </td> 
  </tr> 
 </tbody> 
</table>

In questo caso, ogni assegnatario è allocato al 100% per l&#39;attività Lavoro calcolato.

![](assets/calcwork-350x71.png)

## Modificare il tipo di durata di un&#39;attività in Lavoro calcolato

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
