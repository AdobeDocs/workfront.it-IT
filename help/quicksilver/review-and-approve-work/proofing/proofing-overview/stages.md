---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Panoramica delle fasi del flusso di lavoro automatizzato
description: Le fasi di prova sono segmenti di tempo in cui diversi utenti rivedono una bozza. Man mano che la bozza si sposta da una fase all’altra, Adobe Workfront notifica ai revisori di comunicare loro quando è il momento di lavorare su di essa.
author: Courtney
feature: Digital Content and Documents
exl-id: a03d2cf2-edb3-43b7-a739-32600f2ae2a0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Panoramica delle fasi del flusso di lavoro automatizzato

Le fasi di prova sono segmenti di tempo in cui diversi utenti rivedono una bozza. Man mano che la bozza si sposta da una fase all’altra, Adobe Workfront notifica ai revisori di comunicare loro quando è il momento di lavorare su di essa.

![stage_diagramma.png](assets/stages-diagram-350x63.png)

Gli stadi si verificano in due situazioni diverse:

* [Creare una bozza con un flusso di lavoro automatizzato](#create-a-proof-with-an-automated-workflow)
* [Assegnare scadenze per diversi revisori su una bozza](#assign-deadlines-for-different-reviewers-on-a-proof)

## Creare una bozza con un flusso di lavoro automatizzato {#create-a-proof-with-an-automated-workflow}

Quando aggiungi un flusso di lavoro automatizzato a una bozza, imposta le fasi del lavoro di revisione che desideri eseguire.

Quando si impostano gli stadi per una bozza con un flusso di lavoro automatico:

* È possibile configurare le fasi per l’esecuzione consecutiva o simultanea.
* È possibile configurare alcune fasi affinché diventino attive solo al completamento di una fase precedente.
* Si possono rendere privati alcuni stadi. Ciò è utile, ad esempio, per un’agenzia che esamina una bozza prima che venga condivisa con un cliente e non desidera che i commenti risultanti siano visibili al cliente.

Per istruzioni sulla creazione di fasi per una bozza con un flusso di lavoro automatizzato, consulta [Creare una bozza avanzata con un flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

>[!NOTE]
>
>Se un utente non è incluso in alcuna fase ma ha accesso al documento e apre la bozza, il sistema crea una fase chiamata *Workfront*.
>
>All’utente che ha aperto la bozza viene assegnato il ruolo specificato in Configurazione > Revisione e approvazione > Ruoli per i non destinatari che aprono una bozza di documento.

## Assegnare scadenze per diversi revisori su una bozza {#assign-deadlines-for-different-reviewers-on-a-proof}

Quando assegni diversi termini di correzione ai revisori su una bozza, il sistema crea una fase per ogni scadenza e raggruppa i revisori per ogni scadenza nella fase corrispondente. 

**Esempio:** Ad esempio, se crei una bozza con quattro revisori:

* Per i revisori Olivia e Tony, specifica una scadenza per le 14:00 tra qualche giorno.
* Per Aaron e Amy, specifichi una scadenza per le 17:00 qualche giorno dopo.
* Non specifichi una scadenza per te stesso.

Il sistema crea una fase per ciascuno di questi tre &quot;gruppi&quot; di revisori:

![stage.png](assets/stages-350x239.png)

Se la bozza viene condivisa con un altro revisore e non viene specificata una scadenza, Workfront aggiunge l&#39;utente a Stage 3, dove non esiste una scadenza. 
