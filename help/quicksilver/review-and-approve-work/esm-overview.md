---
product-area: documents
navigation-topic: approvals
title: Panoramica sull’archiviazione aziendale Adobe
description: Panoramica sull’archiviazione aziendale Adobe
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
source-git-commit: c4c4eb8e04b8e43a6681a92c3ee1e3a177ad0983
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 1%

---

# Panoramica sull’archiviazione aziendale Adobe

Adobe enterprise storage è una soluzione di archiviazione basata su cloud che funge da archivio centrale per le risorse tra i prodotti aziendali Adobe. L&#39;integrazione di Workfront e Frame.io è basata sullo storage aziendale Adobe e consente una perfetta collaborazione e gestione delle risorse tra queste piattaforme.

Questa opzione di archiviazione spiana inoltre la strada a future integrazioni di gestione delle risorse con altri prodotti Adobe, come Adobe Creative Cloud.

## Funzioni chiave

* **Livello di archiviazione unificato**: lo storage aziendale Adobe funge da back-end di archiviazione condivisa per Workfront, Frame.io, Document Cloud e Creative Cloud. Ciò consente la collaborazione e la gestione delle risorse su queste piattaforme.

* **Abilitazione Content supply chain**: lo storage aziendale Adobe è un componente fondamentale per la visione Content Supply chain di Adobe, che consente ai team di gestire le risorse in corso di lavorazione senza la necessità di download manuali o di ricaricamenti in varie applicazioni Adobe.

* **Autorizzazioni e accesso centralizzati**: lo storage aziendale di Adobe supporta i controlli di accesso a livello aziendale, integrandosi con Adobe IMS (Identity Management System) per garantire autorizzazioni utente sicure e scalabili.

* **Visibilità end-to-end delle risorse**: le Assets archiviate nell&#39;archiviazione aziendale di Adobe possono essere visualizzate e gestite direttamente nelle app Workfront, Frame.io e Creative Cloud, fornendo metadati coerenti, controllo delle versioni e audit trail.

* **Integrazione con flussi di lavoro di revisione e approvazione**: lo storage aziendale di Adobe consente flussi di lavoro di revisione e approvazione creativi fungendo da fonte di verità per tutte le risorse, garantendo che il feedback e le approvazioni siano tracciati a livello centrale.

* **Storage scalabile e gestione delle quote**: lo storage aziendale Adobe offre opzioni di storage scalabili e il monitoraggio unificato delle quote tra i prodotti Adobe.

## Integrazione con flussi di lavoro di revisione e approvazione

L&#39;integrazione Workfront e Frame.io sfrutta lo storage aziendale Adobe per fornire un&#39;esperienza di revisione e approvazione unificata. Questa integrazione consente ai coordinatori dei progetti di gestire i progetti e pianificare il lavoro in Workfront, mentre i creativi, gli esperti di marketing e le parti interessate possono rivedere e approvare le risorse in Frame.io. In questo modo tutte le parti interessate possono accedere alle versioni più recenti delle risorse e il feedback è centralizzato in un’unica posizione.

Per ulteriori informazioni sull&#39;integrazione di Workfront e Frame.io, vedere [Panoramica sull&#39;integrazione di Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md).

## Differenze tra lo storage aziendale Adobe e lo storage Workfront legacy

Gli ambienti Workfront esistenti offrono una combinazione di storage aziendale Adobe e storage Workfront legacy. Tutti gli oggetti creati prima del rilascio dello storage aziendale Adobe utilizzano lo storage Workfront legacy.

Una volta attivato lo storage aziendale Adobe nell&#39;ambiente in uso, è possibile creare sia lo storage aziendale Adobe che i progetti di storage Workfront legacy.

>[!NOTE]
>
>Per impostazione predefinita, i nuovi ambienti Net dispongono di storage aziendale Adobe abilitato e non hanno la possibilità di utilizzare lo storage Workfront legacy.


### Documenti

#### Area Nuovi documenti

La nuova area documenti è un&#39;area documenti unificata riprogettata per lo storage aziendale Adobe.

Questa interfaccia aggiornata semplifica la navigazione, migliora la chiarezza e semplifica la gestione delle revisioni e delle approvazioni da parte dei team in un unico ambiente unificato. Per ulteriori informazioni, vedere [Panoramica dell&#39;area Documenti](/help/quicksilver/documents/managing-documents/documents-area.md).

#### Nuovo modello di autorizzazione documento

>[!IMPORTANT]
>
>Nello storage aziendale Adobe, le autorizzazioni per i documenti funzionano in modo diverso rispetto allo storage Workfront legacy. I documenti ereditano le autorizzazioni dal progetto, dall’attività o dal problema a cui sono collegati.

I documenti non possono essere condivisi singolarmente. Viene invece generata automaticamente una cartella per ogni attività o problema ed eredita le autorizzazioni dall’attività o dal problema. Tutti i documenti caricati sull’attività o sul problema vengono memorizzati nella cartella generata.

Per ulteriori informazioni sul nuovo modello di autorizzazioni del documento, vedere [Autorizzazioni degli oggetti e panoramica del livello di accesso per il modello di archiviazione aziendale Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

##### Oggetti collegati nelle cartelle

A livello di progetto, le cartelle generate dal sistema visualizzano un oggetto collegato. La cartella viene automaticamente denominata come l’attività o il problema a cui appartiene. Per cartelle collegate si intende il modo in cui il sistema riconosce l’attività o il problema su cui la cartella deve essere visualizzata.

Per ulteriori informazioni, vedere [Funzionamento delle autorizzazioni per i documenti](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Oggetti Workfront

La tabella seguente confronta le funzioni dello storage aziendale Adobe e dello storage Workfront legacy per gli oggetti Workfront.

Gli oggetti di Workfront includono portfolio, programmi, progetti, modelli, attività e problemi.

| Storage aziendale Adobe | Storage Workfront legacy |
|---|---|
| <ul><li>Utilizza lo storage aziendale Adobe</li><li>Integrato con Frame.io</li><li>Utilizza la nuova esperienza Documenti</li><li>Applica convenzioni di denominazione severe</li><li>La condivisione diretta dei documenti non è disponibile</li><li>I documenti sono disponibili in altri prodotti Adobe come Frame.io e Creative Cloud</li></ul> | <ul><li>Utilizza l’archiviazione Workfront</li><li>Utilizza il visualizzatore di bozze</li><li>Supporta la condivisione di singoli documenti</li></ul> |

### Spostare, copiare e convertire gli oggetti

È possibile spostare, copiare e convertire oggetti Workfront tra modelli di memorizzazione simili. È ad esempio possibile spostare un&#39;attività da un progetto di storage aziendale Adobe a un altro progetto di storage aziendale Adobe. Non è possibile spostare un&#39;attività da un progetto di storage aziendale Adobe a un progetto di storage Workfront legacy.

Queste azioni sono disponibili nel menu Altro relativo a un’attività o a un problema. Ogni azione rispetta l’integrità dei documenti, l’ereditarietà delle autorizzazioni e le regole di storage aziendale di Adobe.

## Abilitare lo storage aziendale Adobe

I clienti esistenti possono abilitare lo storage aziendale Adobe nel proprio ambiente al momento del rinnovo del contratto. Per ulteriori informazioni sull&#39;abilitazione dello storage aziendale Adobe, consulta [Abilitare lo storage aziendale Adobe per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

>[!NOTE]
>
>I nuovi clienti hanno lo storage aziendale Adobe abilitato per impostazione predefinita e non hanno la possibilità di utilizzare lo storage Workfront legacy.



## Considerazioni

* È possibile che Workfront non sia sincronizzato con Frame.io o Creative Cloud, ad esempio una risorsa eliminata in Workfront ma ancora visualizzata in Frame.io, contatta il supporto Workfront per sincronizzare nuovamente il tuo ambiente.


