---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Panoramica sullo stato di completamento dell'iterazione
description: Le informazioni di completamento descritte in questo articolo vengono visualizzate sopra il grafico a discesa.
author: Lisa
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
source-git-commit: 373f2522b85196d6395f189ae6cfe03449cac61a
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 0%

---

# Panoramica sullo stato di completamento dell&#39;iterazione

Le informazioni di completamento descritte in questo articolo vengono visualizzate sopra il grafico a discesa.

Percentuale di completamento su un&#39;iterazione:

![](assets/burndown-percentcomplete-350x47.png)

Queste informazioni indicano lo stato di completamento dell&#39;iterazione per il giorno attualmente selezionato nel grafico a discesa. Per impostazione predefinita, lo stato di completamento viene visualizzato in base alla data del giorno corrente.

Sono disponibili le seguenti informazioni:

* **[!UICONTROL Percentuale completata]:** Progresso generale dell&#39;iterazione

   [!UICONTROL Percentuale completata] si regola in base alla percentuale di completamento di ogni storia o attività nell’iterazione, compresi i racconti o le attività che sono solo parzialmente completate.

   Il colore del [!UICONTROL Percentuale completata] la barra di stato viene visualizzata in rosso o verde in modo che corrisponda al colore della frequenza di menu effettiva. Viene mostrato in rosso quando il tasso di abbandono è inferiore all&#39;ideale (più punti o ore rimanenti al giorno rispetto al calcolo di esaurimento ideale), e viene mostrato in verde quando il tasso di abbandono è uguale o migliore dell&#39;ideale (pari o meno punti rimanenti al giorno rispetto al calcolo di esaurimento ideale).

* **[!UICONTROL Storie completate]:** (Disponibile solo nelle iterazioni) Il numero di storie contrassegnate [!UICONTROL Completa]. Questo viene mostrato in relazione al numero totale di storie nell&#39;iterazione. Ad esempio, &quot;3 di 6&quot; indica che 3 dei 6 storie nell&#39;iterazione sono state contrassegnate [!UICONTROL Completa].
* **[!UICONTROL Punti/ore completati]:** (Disponibile solo nelle iterazioni) Il numero di punti o ore contrassegnati [!UICONTROL Completa]. Mostrato in relazione al numero totale di punti o ore nell’iterazione. Ad esempio, &quot;5 of 11&quot; indica che 5 delle 11 storie nell&#39;iterazione sono state contrassegnate [!UICONTROL Completa]. Questo numero è direttamente correlato al [!UICONTROL Percentuale completata] e viene aggiornato contemporaneamente [!UICONTROL Percentuale completata] è aggiornato.

   I punti e le ore sono associati alle storie. Quando una storia è segnata [!UICONTROL Completa], i punti o le ore associati a tale storia sono contrassegnati come Complete.

   Per impostazione predefinita, vengono utilizzati i punti. Puoi modificare questa impostazione modificando le impostazioni per il tuo team, come descritto in [Creare un team agile](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

* **[!UICONTROL Punti/ore al giorno]:** (Disponibile solo nelle iterazioni) Il numero medio di punti o ore contrassegnati [!UICONTROL Completa] ogni giorno dall&#39;inizio dell&#39;iterazione attraverso il giorno corrente.

   Questo viene calcolato in base ai punti o alle ore totali completate, suddivisi per il numero totale di giorni nel giorno corrente. (I giorni parziali sono registrati come un intero giorno.)

   Queste informazioni possono essere utili durante la pianificazione di un’iterazione futura.

* **[!UICONTROL Completamento stimato]:** La data stimata in cui l’iterazione verrà completata, in base al tasso corrente nei punti/ore al giorno (per le iterazioni).

   Quando il [!UICONTROL Completamento stimato] la data è successiva alla data di fine definita per l’iterazione; il numero di giorni lavorativi rimanenti viene visualizzato in rosso tra parentesi accanto alla [!UICONTROL Completamento stimato] data.

   Quando il [!UICONTROL Completamento stimato] la data è precedente alla data di fine pianificata dell’iterazione; il numero di giorni lavorativi rimanenti viene visualizzato in verde. (La data di fine dell’iterazione viene specificata al momento della pianificazione dell’iterazione, come descritto in [Creare un’iterazione](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md); la data di fine del progetto è la [!UICONTROL Data completamento pianificata]oppure è la data corrente se [!UICONTROL Data completamento pianificata] è nel passato. La [!UICONTROL Data completamento pianificata] per il progetto viene calcolato in base alla durata delle attività del progetto). Quando si pianifica l&#39;iterazione, se si imposta la data di fine dell&#39;iterazione per un giorno non lavorativo e l&#39;iterazione viene monitorata per terminare in tempo, la data di completamento stimato viene impostata per l&#39;ultimo giorno lavorativo precedente alla data di fine dell&#39;iterazione impostata (perché il lavoro non è pianificato per essere bruciato nei giorni non lavorativi).

   Ad esempio, &quot;(+9 giorni)&quot; indica che la data di completamento stimato è 9 giorni lavorativi dopo la data di fine pianificata dell’iterazione.

   Per ulteriori informazioni, consulta [Panoramica sullo stato di completamento dell&#39;iterazione](#Understanding-How-Days-Off-Affect-the-Burndown-Chart).
