---
product-area: templates
navigation-topic: templates-navigation-topic
title: Panoramica dei giorni di inizio e di completamento in un modello
description: È possibile utilizzare i modelli di progetto per acquisire la maggior parte dei processi, delle informazioni e delle impostazioni ripetibili associati ai progetti dell’organizzazione. Sebbene i progetti abbiano date di inizio e di completamento specifiche, i modelli dispongono di giorni di inizio e completamento generici come indicazione del punto in cui tali date rientreranno nel progetto, in base alla cronologia complessiva del progetto.
author: Alina
feature: Work Management
exl-id: caa0e7b1-37c3-4973-92ce-cc93df4e4186
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---

# Panoramica dei giorni di inizio e di completamento in un modello

È possibile utilizzare i modelli di progetto per acquisire la maggior parte dei processi, delle informazioni e delle impostazioni ripetibili associati ai progetti dell’organizzazione. Sebbene i progetti abbiano date di inizio e di completamento specifiche, i modelli dispongono di giorni di inizio e completamento generici come indicazione del punto in cui tali date rientreranno nel progetto, in base alla cronologia complessiva del progetto.

**Esempio:** Se la data di inizio di un progetto è il 1° aprile e si desidera che un&#39;attività inizi il 3 aprile (due giorni dopo l&#39;inizio del progetto), l&#39;attività corrispondente nel modello che crea il progetto dovrebbe iniziare il 2° giorno del modello, dove il primo giorno del modello è considerato il Giorno 0.

## Giorno Inizio

Quando si utilizzano modelli e attività modello, tenere presente quanto segue:

* Per impostazione predefinita, i modelli hanno un Giorno iniziale pari a 0 e le attività del modello e il modello mostra un Giorno iniziale pari a 0. Il giorno di inizio delle attività del modello può cambiare, ma questo non cambia il giorno di inizio del modello.
* Il giorno di inizio di un&#39;attività modello rappresenta il numero di giorni lavorativi aggiunti da Workfront alla data di inizio pianificata dell&#39;attività quando un progetto viene creato dal modello. Ad esempio, è possibile avere un modello con una sola attività e il giorno iniziale dell&#39;attività modello è 4. Il giorno iniziale del modello è ancora 0. Quando crei un progetto da questo modello in cui la modalità di pianificazione del progetto è Data di inizio e la data di inizio pianificata del progetto è il 1° novembre 2019, l&#39;attività appena creata aggiunge 4 giorni a questa data e imposta il valore della data di inizio pianificata sul 5 novembre 2019.

Di seguito sono riportate alcune azioni che potrebbero modificare il giorno di inizio delle attività del modello:

* Aggiornare la durata delle attività del modello predecessore
* Aggiornare i vincoli di attività

   Quando si utilizzano i vincoli di attività basati sulla data, è possibile aggiornare manualmente il giorno iniziale delle attività del modello. Alcuni esempi di vincoli di attività basati su data sono date fisse, Start non prima di, Start non più tardi di, Deve iniziare su .

* Aggiornare i predecessori delle attività del modello

## Giorno di completamento

Il giorno di completamento del modello è il giorno in cui l&#39;ultima attività del modello viene completata. Per impostazione predefinita, tutte le attività del modello e il modello mostrano un giorno di completamento pari a 1, in quanto Workfront presuppone che qualsiasi attività del modello abbia una durata di 1 giorno. Il giorno di completamento delle attività del modello può cambiare e questo cambia anche il giorno di completamento del modello. Il giorno di completamento del modello diventa la data di completamento pianificata del progetto futuro e i giorni di completamento delle attività del modello diventano le date di completamento pianificate delle attività future del progetto.

Di seguito sono riportate alcune azioni che potrebbero modificare il giorno di completamento delle attività del modello:

* Aggiorna la durata delle attività del modello
* Aggiornare i vincoli di attività

   Quando si utilizzano i vincoli di attività basati sulla data, è possibile aggiornare manualmente il giorno di completamento delle attività del modello. Alcuni esempi di vincoli di attività basati su data sono date fisse, la fine non prima di, la fine non più tardi di, deve terminare il.

* Aggiornare i predecessori delle attività del modello

## Utilizzare i modelli pianificati da Completamento

È possibile pianificare un modello dal giorno di completamento. Per ulteriori informazioni, consulta [Modificare i modelli di progetto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Quando si utilizzano modelli pianificati da Data completamento, tenere presente quanto segue:

* La modifica del giorno iniziale imposta il vincolo dell&#39;attività su Deve iniziare su.
* La modifica del giorno di completamento imposta il vincolo dell&#39;attività su Deve terminare su.
* Quando il modello è programmato dal giorno di completamento, il giorno del vincolo del task viene calcolato dal giorno di completamento.

   **Esempio:** La durata del modello è di 285 giorni e si dispone di un&#39;attività modello con una durata di 60 giorni. Se si imposta il Vincolo attività su Deve iniziare il giorno e Vincolo su 120, verrà visualizzato un Giorno iniziale di 165 (285 - 120) e un Giorno completamento di 225 (165 + 60). Quindi, quando si modifica il giorno iniziale, viene interpretato come giorno vincolo.
