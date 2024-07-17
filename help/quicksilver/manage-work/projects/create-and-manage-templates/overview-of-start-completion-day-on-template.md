---
product-area: templates
navigation-topic: templates-navigation-topic
title: Panoramica dei giorni di inizio e completamento in un modello
description: È possibile utilizzare i modelli di progetto per acquisire la maggior parte dei processi, delle informazioni e delle impostazioni ripetibili associati ai progetti dell'organizzazione. Anche se i progetti hanno date di inizio e di completamento specifiche, i modelli hanno giorni di inizio e di completamento generici come indicazione di dove tali date ricadranno sul progetto, in base alla sequenza temporale complessiva del progetto.
author: Alina
feature: Work Management
exl-id: caa0e7b1-37c3-4973-92ce-cc93df4e4186
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# Panoramica dei giorni di inizio e completamento in un modello

È possibile utilizzare i modelli di progetto per acquisire la maggior parte dei processi, delle informazioni e delle impostazioni ripetibili associati ai progetti dell&#39;organizzazione. Anche se i progetti hanno date di inizio e di completamento specifiche, i modelli hanno giorni di inizio e di completamento generici come indicazione di dove tali date ricadranno sul progetto, in base alla sequenza temporale complessiva del progetto.

**Esempio:** se la data di inizio di un progetto è il 1 aprile e si desidera che un&#39;attività inizi il 3 aprile (due giorni dopo l&#39;inizio del progetto), l&#39;attività corrispondente nel modello che crea il progetto deve iniziare il giorno 2 del modello, dove il primo giorno del modello è considerato il giorno 0.

## Giorno Inizio

Quando si lavora con modelli e attività modello, considera quanto segue:

* Per impostazione predefinita, i modelli hanno un Giorno iniziale pari a 0 e le attività modello e il modello mostrano un Giorno iniziale pari a 0. Il giorno di inizio delle attività modello può cambiare, ma questo non modifica il giorno di inizio del modello.
* Il giorno di inizio di un&#39;attività modello rappresenta il numero di giorni lavorativi che Workfront aggiunge alla Data inizio pianificata dell&#39;attività quando un progetto viene creato dal modello. Ad esempio, è possibile avere un modello con una sola attività e il giorno di inizio dell&#39;attività modello è 4. Il giorno di inizio del modello è ancora 0. Quando si crea un progetto da questo modello in cui la modalità di pianificazione del progetto è Data inizio e la data di inizio pianificata del progetto è il 1° novembre 2019, la nuova attività creata aggiunge 4 giorni a questa data e imposta il valore Data inizio pianificata al 5 novembre 2019.

Di seguito sono riportate alcune azioni che potrebbero modificare il giorno di inizio delle attività modello:

* Aggiorna la durata delle attività modello predecessore
* Aggiornare i vincoli delle attività

  Quando si utilizzano vincoli di attività basati sulla data, è possibile aggiornare manualmente il giorno di inizio delle attività modello. Alcuni esempi di vincoli delle attività basati sulla data sono date fisse, inizio non prima di, inizio non dopo di, inizio non deve iniziare il.

* Aggiornare i predecessori delle attività modello

## Giorno di completamento

Il giorno di completamento del modello è il giorno in cui viene completata l&#39;ultima attività modello. Per impostazione predefinita, tutte le attività modello e il modello visualizzano il giorno di completamento 1, poiché Workfront presuppone che qualsiasi attività modello abbia una durata di 1 giorno. Il giorno di completamento delle attività del modello può cambiare, cambiando anche il giorno di completamento del modello. Il giorno di completamento del modello diventa la data di completamento pianificata del progetto futuro e i giorni di completamento delle attività del modello diventano le date di completamento pianificate delle attività del progetto future.

Di seguito sono riportate alcune azioni che potrebbero modificare il giorno di completamento delle attività modello:

* Aggiorna la durata delle attività modello
* Aggiornare i vincoli delle attività

  Quando si utilizzano vincoli di attività basati sulla data, è possibile aggiornare manualmente il giorno di completamento delle attività modello. Alcuni esempi di vincoli delle attività basati sulla data sono le date fisse, Finire non prima del, Finire non dopo il, Finire non dopo il.

* Aggiornare i predecessori delle attività modello

## Utilizzare i modelli pianificati dal completamento

È possibile pianificare un modello dal giorno di completamento. Per ulteriori informazioni, vedere [Modifica modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Quando si utilizzano modelli pianificati dalla data di completamento, considera quanto segue:

* Se si modifica il giorno di inizio, il vincolo Attività viene impostato su Deve iniziare il.
* La modifica del giorno di completamento imposta il vincolo attività su Deve finire al.
* Quando il modello viene programmato dal giorno di completamento, il giorno Vincolato attività viene calcolato dal giorno di completamento.

  **Esempio:** la durata del modello è di 285 giorni e l&#39;attività modello ha una durata di 60 giorni. Se si imposta il vincolo attività su Deve iniziare il e Vincola giorno su 120, il giorno di inizio sarà 165 (285 - 120) e il giorno di completamento sarà 225 (165 + 60). Pertanto, quando si modifica il giorno di inizio, viene effettivamente interpretato come giorno vincolo.
