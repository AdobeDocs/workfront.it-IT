---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Panoramica sullo stato di completamento dell'iterazione
description: Le informazioni di completamento descritte in questo articolo vengono visualizzate sopra il grafico a dispersione.
author: Lisa
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 0%

---

# Panoramica sullo stato di completamento dell&#39;iterazione

Le informazioni di completamento descritte in questo articolo vengono visualizzate sopra il grafico a dispersione.

Percentuale di completamento in un&#39;iterazione:

![](assets/burndown-percentcomplete-350x47.png)

Queste informazioni indicano lo stato di completamento dell&#39;iterazione per il giorno attualmente selezionato nel grafico a dispersione. Per impostazione predefinita, lo stato di completamento viene visualizzato in base alla data del giorno corrente.

Sono disponibili le seguenti informazioni:

* **[!UICONTROL Percentuale completata]:** Stato complessivo dell&#39;iterazione

  [!UICONTROL La percentuale di completamento] viene regolata in base alla percentuale di completamento di ogni storia o attività all&#39;interno dell&#39;iterazione, incluse le storie o le attività completate solo parzialmente.

  Il colore della barra di stato [!UICONTROL Percent Complete] viene visualizzato in rosso o verde per corrispondere al colore della frequenza di masterizzazione effettiva. Viene mostrato in rosso quando il tasso di burndown è inferiore all&#39;ideale (rimangono più punti o ore al giorno rispetto al calcolo del burndown ideale) e in verde quando il tasso di burndown è uguale o migliore dell&#39;ideale (rimangono meno punti al giorno rispetto al calcolo del burndown ideale).

* **[!UICONTROL Storie completate]:** (disponibile solo nelle iterazioni) Numero di storie contrassegnate come [!UICONTROL Complete]. Questo viene mostrato in relazione al numero totale di storie nell&#39;iterazione. Ad esempio, &quot;3 di 6&quot; indica che 3 dei 6 brani nell&#39;iterazione sono stati contrassegnati come [!UICONTROL Complete].
* **[!UICONTROL Punti completati/Ore]:** (disponibile solo in iterazioni) Il numero di punti o ore contrassegnato come [!UICONTROL Completo]. Mostrato in relazione al numero totale di punti o ore nell&#39;iterazione. Ad esempio, &quot;5 di 11&quot; indica che 5 degli 11 brani nell&#39;iterazione sono stati contrassegnati come [!UICONTROL Completati]. Questo numero è direttamente correlato al calcolo di [!UICONTROL Percent Complete] e viene aggiornato contemporaneamente a [!UICONTROL Percent Complete].

  I punti e le ore sono associati alle storie. Quando una storia è contrassegnata come [!UICONTROL Completa], i punti o le ore associati a essa sono contrassegnati come Completati.

  Per impostazione predefinita, vengono utilizzati i punti. Puoi modificare questa impostazione modificando le impostazioni per il tuo team, come descritto in [Creare un team Agile](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

* **[!UICONTROL Punti / Ore al giorno]:** (Disponibile solo in iterazioni) Numero medio di punti o ore contrassegnate [!UICONTROL Complete] ogni giorno dall&#39;inizio dell&#39;iterazione fino al giorno corrente.

  Viene calcolato in base al totale di punti o ore completate, diviso per il numero totale di giorni nel giorno corrente. (I giorni parziali vengono registrati come un giorno intero).

  Queste informazioni possono essere utili quando si pianifica un’iterazione futura.

* **[!UICONTROL Completamento stimato]:** La data stimata in cui l&#39;iterazione verrà completata, in base alla tariffa corrente in Punti/Ore al Giorno (per le iterazioni).

  Quando la data di [!UICONTROL completamento stimato] è successiva alla data di fine definita per l&#39;iterazione, il numero di giorni lavorativi rimanenti viene visualizzato in rosso tra parentesi accanto alla data di [!UICONTROL completamento stimato].

  Quando la data di [!UICONTROL completamento stimato] è precedente alla data di fine pianificata dell&#39;iterazione, il numero di giorni lavorativi rimanenti viene visualizzato in verde. (La data di fine dell&#39;iterazione viene specificata quando l&#39;iterazione è pianificata, come descritto in [Creare un&#39;iterazione](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md); la data di fine del progetto è la [!UICONTROL Data di completamento pianificata], oppure la data corrente se la [!UICONTROL Data di completamento pianificata] è nel passato. La [!UICONTROL Data di completamento pianificata] per il progetto viene calcolata in base alla durata delle attività nel progetto.) Quando si pianifica l&#39;iterazione, se si imposta la data di fine dell&#39;iterazione per un giorno non lavorativo e l&#39;iterazione tiene traccia della fine puntuale, la data di completamento stimata viene impostata per l&#39;ultimo giorno lavorativo precedente alla data di fine dell&#39;iterazione impostata (poiché il lavoro non è programmato per essere masterizzato in giorni non lavorativi).

  Ad esempio, &quot;(+9 giorni)&quot; indica che la data di completamento stimata è 9 giorni lavorativi più tardi della data di fine pianificata dell’iterazione.

  Per ulteriori informazioni, vedere [Panoramica sullo stato di completamento dell&#39;iterazione](#Understanding-How-Days-Off-Affect-the-Burndown-Chart).
