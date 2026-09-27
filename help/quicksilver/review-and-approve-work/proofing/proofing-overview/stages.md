---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Panoramica delle fasi del flusso di lavoro automatizzato
description: Le fasi di bozza sono segmenti di tempo in cui utenti diversi esaminano una bozza. Quando la bozza si sposta da una fase all’altra, Adobe Workfront notifica ai revisori di comunicare loro quando è il momento di lavorarci.
author: Courtney
feature: Digital Content and Documents
exl-id: a03d2cf2-edb3-43b7-a739-32600f2ae2a0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 1%
---
# Panoramica delle fasi del flusso di lavoro automatizzato

Le fasi di bozza sono segmenti di tempo in cui utenti diversi esaminano una bozza. Quando la bozza si sposta da una fase all’altra, Adobe Workfront notifica ai revisori di comunicare loro quando è il momento di lavorarci.

![diagramma_stadi.png](assets/stages-diagram-350x63.png)

Gli stadi si verificano in due situazioni diverse:

* [Crea una bozza con un flusso di lavoro automatizzato](#create-a-proof-with-an-automated-workflow)
* [Assegnare scadenze a diversi revisori su una bozza](#assign-deadlines-for-different-reviewers-on-a-proof)

## Creare una bozza con un flusso di lavoro automatizzato {#create-a-proof-with-an-automated-workflow}

Quando si aggiunge un flusso di lavoro automatizzato a una bozza, è possibile impostare le fasi del lavoro di revisione che si desidera eseguire.

Quando si impostano le fasi per una bozza con un flusso di lavoro automatico:

* È possibile configurare le fasi in modo che vengano eseguite consecutivamente o contemporaneamente.
* È possibile configurare alcune fasi in modo che diventino attive solo dopo il completamento di una fase precedente.
* È possibile rendere alcune fasi private. Ciò è utile, ad esempio, per un’agenzia che rivede una bozza prima che venga condivisa con un cliente e non desidera che i commenti risultanti siano visibili al cliente.

Per istruzioni sulla creazione di fasi per una bozza con un flusso di lavoro automatico, vedere [Creare una bozza avanzata con un flusso di lavoro automatico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

>[!NOTE]
>
>Se un utente non è incluso in nessuna fase ma ha accesso al documento e apre la bozza, verrà creata una fase denominata *Workfront*.
>
>All’utente che ha aperto la bozza viene assegnato il ruolo specificato in Configurazione > Revisione e approvazione > Ruoli per i non destinatari che aprono una bozza del documento.

## Assegnare scadenze a diversi revisori su una bozza {#assign-deadlines-for-different-reviewers-on-a-proof}

Quando si assegnano scadenze di bozza diverse ai revisori su una bozza, il sistema crea una fase per ogni scadenza e raggruppa i revisori per ogni scadenza nella fase corrispondente. 

**Esempio:** Ad esempio, se crei una bozza con quattro revisori:

* Per i revisori Olivia e Tony, specificate una scadenza per le 14:00 tra qualche giorno.
* Per Aaron e Amy, specificate una scadenza per le 17:00 qualche giorno dopo.
* Non hai specificato una scadenza.

Il sistema crea una fase per ciascuno di questi tre &quot;gruppi&quot; di revisori:

![stages.png](assets/stages-350x239.png)

Se la bozza viene condivisa con un altro revisore e non si specifica una scadenza, Workfront aggiunge l&#39;utente alla fase 3, in cui non esiste alcuna scadenza. 
