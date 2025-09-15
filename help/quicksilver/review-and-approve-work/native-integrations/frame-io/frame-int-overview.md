---
product-area: documents
navigation-topic: approvals
title: Panoramica dell’integrazione Frame.io
description: Panoramica dell’integrazione Frame.io
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 701f3fc2c885363b5f61fb9d77049c7d4c41963d
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---


# Panoramica dell’integrazione Frame.io

L’integrazione Workfront e Frame.io consente ai coordinatori dei progetti di gestire i progetti e pianificare il lavoro in Workfront, mentre i creativi, gli esperti di marketing e le parti interessate possono rivedere e approvare le risorse in Frame.io.

## Basato su Adobe Enterprise Storage Management

Il nucleo di questa integrazione è Adobe Enterprise Storage Management (ESM), una soluzione di storage basata su cloud che funge da archivio centrale per le risorse tra i prodotti aziendali Adobe, inclusi Workfront e Frame.io.

I principali vantaggi di Adobe Enterprise Storage Management includono:

* Livello di storage unificato per risorse creative e di gestione del lavoro
* Autorizzazioni centralizzate tramite Adobe IMS per il controllo sicuro degli accessi
* Visibilità completa delle risorse nelle app Workfront, Frame.io e Creative Cloud <!--coming soon?-->
* Storage scalabile e gestione delle quote per le esigenze aziendali

Per ulteriori dettagli, vedere [Panoramica di Adobe Enterprise Storage Management](help/quicksilver/review-and-approve-work/esm-overview.md).

## Revisione e approvazione unificate

L&#39;integrazione Workfront e Frame.io utilizza la funzionalità di approvazione unificata di Workfront per gestire le revisioni e le approvazioni. Con le approvazioni unificate, puoi:

* Crea e gestisci revisioni e approvazioni direttamente da Workfront
* Monitorare lo stato di revisioni e approvazioni in tempo reale
* Centralizzare feedback e approvazioni in un&#39;unica posizione
* Assicurati che tutte le parti interessate abbiano accesso alle versioni più recenti delle risorse
* Utilizzare i revisori AI per automatizzare le revisioni di conformità al brand
* e altro ancora

Per ulteriori informazioni, vedere [Unified document approvals: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### Utilizzare il visualizzatore Frame.io

L&#39;integrazione si collega anche al visualizzatore Frame.io. Il visualizzatore Frame.io fornisce

* Strumenti di markup e commento
* Cronologia e confronto delle versioni
* Commenti con marca temporale per le recensioni video
* Accesso mobile per revisioni e approvazioni in movimento

Per ulteriori informazioni, vedere [Introduzione all&#39;integrazione Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md).

#### Limitazioni della revisione video

<!--need to confirm these-->

#### Tipi di file supportati nel visualizzatore Frame.io

Il visualizzatore Frame.io supporta tutti i tipi comuni di video, immagini, audio, PDF e MS® Office. Per un elenco dettagliato dei file supportati, vedere [Tipi in Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Accesso e licenze per il visualizzatore Frame.io

Il visualizzatore Frame.io è disponibile per tutti gli utenti di Workfront con una licenza a pagamento. Non è richiesta alcuna licenza Frame.io aggiuntiva per utilizzare il visualizzatore Frame.io per le revisioni e le approvazioni con questa integrazione.

Se la tua organizzazione desidera sfruttare ulteriori funzionalità Frame.io, ad esempio caricare le risorse direttamente nei progetti in Frame.io, puoi acquistare una licenza Enterprise Frame.io. <!--link to Frame.io enterprise license info or who to contacT?-->

La funzionalità di verifica Workfront non è disponibile con questa integrazione.

## Potente gestione dei progetti in Workfront

Con l&#39;integrazione Workfront e Frame.io, i coordinatori dei progetti possono sfruttare le potenti funzionalità di gestione dei progetti di Workfront per pianificare, tracciare e gestire il lavoro.

Per ulteriori informazioni sulla gestione dei progetti in Workfront, vedere [Progetti: indice articolo](/help/quicksilver/manage-work/projects/projects-toc.md).

### Struttura imposta e convenzioni di denominazione

Poiché questa integrazione viene creata utilizzando ESM, esistono alcune convenzioni di denominazione e struttura applicate di cui tenere conto durante la gestione di progetti e documenti.

* I nomi degli oggetti devono essere univoci e non possono essere duplicati
* ESM richiede nomi univoci per gli oggetti peer con lo stesso padre nella struttura gerarchica
* I documenti non possono avere lo stesso nome se appartengono allo stesso progetto

Tenendo presenti queste limitazioni, Workfront rinomina automaticamente gli oggetti o i documenti in base alle esigenze per evitare conflitti.

### Gestione dei documenti in Workfront

I documenti vengono gestiti a livello di progetto con questa integrazione e non possono essere caricati sulle attività o sui problemi in questo momento.

L’accesso ai documenti viene gestito anche a livello di progetto. Se un utente ha accesso a un progetto, può accedere a tutti i documenti associati a tale progetto.

<!--Documents can't be dragged as full folders.-->

### Limitazioni dell’esperienza documentale

Poiché questa integrazione viene creata utilizzando ESM, esistono alcune limitazioni all&#39;esperienza del documento originale in Workfront:

#### Limitazioni

Le seguenti funzionalità non saranno incluse in questa integrazione:

* Provider di documenti esterni
* Accesso alle prove
* Visualizzatore documenti in Workfront


#### Limitazioni temporanee

Per il momento, non sono disponibili le seguenti funzionalità:

* Documenti preferiti
* Richiedi documenti
* Inviare documenti ad Adobe Experience Manager Assets
* Approvazioni in più fasi
* Caricare documenti in commenti o aggiornamenti in Workfront
* Carica documenti in attività o problemi in Workfront



