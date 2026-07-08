---
product-area: documents
navigation-topic: approvals
title: Panoramica dell’archiviazione cloud Adobe
description: Panoramica dell’archiviazione cloud Adobe
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YOO4BspMzbMr8iPoXRBKK65IbU5yfpiJndNuYvYF5SM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: c2fe0c6afbc9b536186bd473e95b3f82f144b06c
workflow-type: tm+mt
source-wordcount: 1061
ht-degree: 0%

---

# Panoramica dell’archiviazione cloud Adobe

Adobe Cloud Storage è una soluzione di archiviazione basata su cloud che funge da archivio centrale per le risorse tra i prodotti aziendali Adobe. L&#39;integrazione di Workfront e Frame.io è basata sull&#39;archiviazione cloud Adobe e consente la collaborazione e la gestione delle risorse tra queste piattaforme.

Questa opzione di archiviazione spiana inoltre la strada a future integrazioni di gestione delle risorse con altri prodotti Adobe, come Adobe Creative Cloud.

## Funzioni chiave

* **Livello di archiviazione unificata**: l&#39;archiviazione cloud Adobe funge da back-end di archiviazione condivisa per Workfront, Frame.io, Document Cloud e Creative Cloud. Ciò consente la collaborazione e la gestione delle risorse su queste piattaforme.

* **Abilitazione Content supply chain**: l&#39;archiviazione cloud di Adobe è un componente fondamentale per la visione Content Supply chain di Adobe, che consente ai team di gestire le risorse in corso di lavorazione senza la necessità di download manuali o di ricaricamenti in varie applicazioni Adobe.

* **Autorizzazioni e accesso centralizzati**: l&#39;archiviazione cloud di Adobe supporta controlli di accesso a livello aziendale, integrandosi con Adobe IMS (Identity Management System) per autorizzazioni utente sicure e scalabili.

* **Visibilità end-to-end delle risorse**: Assets memorizzato nell&#39;archiviazione cloud Adobe può essere visualizzato e gestito direttamente nelle app Workfront, Frame.io e Creative Cloud, fornendo metadati coerenti, controllo delle versioni e audit trail.

* **Integrazione con flussi di lavoro di revisione e approvazione**: l&#39;archiviazione cloud di Adobe abilita flussi di lavoro di revisione e approvazione creativi fungendo da fonte di verità per tutte le risorse, garantendo che il feedback e le approvazioni siano tracciati a livello centrale.

* **Archiviazione scalabile e gestione delle quote**: l&#39;archiviazione cloud Adobe offre opzioni di archiviazione scalabili e il monitoraggio unificato delle quote tra i prodotti Adobe.

## Integrazione con flussi di lavoro di revisione e approvazione

L’integrazione Workfront e Frame.io sfrutta l’archiviazione cloud Adobe per fornire un’esperienza di revisione e approvazione unificata. Questa integrazione consente ai coordinatori dei progetti di gestire i progetti e pianificare il lavoro in Workfront, mentre i creativi, gli esperti di marketing e le parti interessate possono rivedere e approvare le risorse in Frame.io. In questo modo tutte le parti interessate possono accedere alle versioni più recenti delle risorse e il feedback è centralizzato in un’unica posizione.

Per ulteriori informazioni sull&#39;integrazione di Workfront e Frame.io, vedere [Panoramica unificata su revisione e approvazione](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

## Differenze tra l’archiviazione cloud Adobe e l’archiviazione Workfront legacy

Gli ambienti Workfront esistenti offrono una combinazione di storage cloud Adobe e storage Workfront legacy. Tutti gli oggetti creati prima del rilascio dell’archiviazione cloud Adobe utilizzano l’archiviazione Workfront legacy.

Dopo aver abilitato l’archiviazione cloud di Adobe nell’ambiente in uso, puoi creare sia progetti di archiviazione cloud di Adobe che progetti di archiviazione Workfront legacy.

>[!NOTE]
>
>Per impostazione predefinita, i nuovi ambienti netti hanno l’archiviazione cloud Adobe abilitata e non hanno la possibilità di utilizzare l’archiviazione Workfront legacy.


### Documenti

#### Area Nuovi documenti

La nuova area Documenti è un’area documenti unificata riprogettata per l’archiviazione cloud Adobe.

Questa interfaccia aggiornata semplifica la navigazione, migliora la chiarezza e semplifica la gestione delle revisioni e delle approvazioni da parte dei team in un unico ambiente unificato. Per ulteriori informazioni, vedere [Panoramica dell&#39;area Documenti](/help/quicksilver/documents/managing-documents/documents-area.md).

#### Nuovo modello di autorizzazione documento

>[!IMPORTANT]
>
>Nell’archiviazione cloud Adobe, le autorizzazioni per i documenti funzionano in modo diverso rispetto all’archiviazione Workfront legacy. I documenti ereditano le autorizzazioni dal progetto, dall’attività o dal problema a cui sono collegati.

I documenti non possono essere condivisi singolarmente. Viene invece generata automaticamente una cartella per ogni attività o problema ed eredita le autorizzazioni dall’attività o dal problema. Tutti i documenti caricati sull’attività o sul problema vengono memorizzati nella cartella generata.

Per ulteriori informazioni sul nuovo modello di autorizzazione dei documenti, vedere [Autorizzazioni degli oggetti e panoramica del livello di accesso per il modello di archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

##### Oggetti collegati nelle cartelle

A livello di progetto, le cartelle generate dal sistema visualizzano un oggetto collegato. La cartella viene automaticamente denominata come l’attività o il problema a cui appartiene. Per cartelle collegate si intende il modo in cui il sistema riconosce l’attività o il problema su cui la cartella deve essere visualizzata.

Per ulteriori informazioni, vedere [Funzionamento delle autorizzazioni per i documenti](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

#### Adobe Cloud Drive

Adobe Cloud Drive è un’applicazione desktop che consente di montare i progetti di archiviazione cloud di Adobe come un’unità nel computer Mac o Windows. Puoi aprire, modificare e salvare i file in qualsiasi applicazione mentre Adobe Cloud Drive mantiene il tuo lavoro sincronizzato con l’archiviazione cloud di Adobe. Per ulteriori informazioni, consulta [Panoramica di Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/adobe-cloud-drive-overview.md).

## Oggetti Workfront

La tabella seguente confronta le funzioni dell’archiviazione cloud Adobe e dell’archiviazione Workfront legacy per gli oggetti Workfront.

Gli oggetti di Workfront includono portfolio, programmi, progetti, modelli, attività e problemi.

| Archiviazione cloud Adobe | Archiviazione legacy di Workfront |
|---|---|
| <ul><li>Utilizza l’archiviazione cloud di Adobe</li><li>Integrato con Frame.io</li><li>Utilizza la nuova esperienza Documenti</li><li>Applica convenzioni di denominazione severe</li><li>La condivisione diretta dei documenti non è disponibile</li><li>I documenti sono disponibili in altri prodotti Adobe come Frame.io e Creative Cloud</li></ul> | <ul><li>Utilizza l’archiviazione Workfront</li><li>Utilizza il visualizzatore di bozze</li><li>Supporta la condivisione di singoli documenti</li></ul> |

### Spostare, copiare e convertire gli oggetti

Nella maggior parte degli scenari è possibile spostare, copiare e convertire oggetti Workfront tra modelli di memorizzazione simili. Ad esempio, puoi spostare un’attività da un progetto di archiviazione cloud Adobe a un altro progetto di archiviazione cloud Adobe.

In tre casi specifici, puoi convertire un oggetto di archiviazione Workfront legacy in archiviazione cloud Adobe:

* Converti un’attività di archiviazione Workfront legacy in un progetto di archiviazione cloud Adobe.
* Converti un portfolio di archiviazione Workfront legacy in un portfolio di archiviazione cloud Adobe.
* Crea un progetto di archiviazione cloud Adobe da un modello di archiviazione Workfront legacy.

Durante queste conversioni, i documenti e le cartelle di documenti non vengono spostati dall’archiviazione legacy di Workfront all’archiviazione cloud di Adobe.

Per ulteriori informazioni, vedere [Portabilità dell&#39;oggetto](/help/quicksilver/review-and-approve-work/workfront-storage.md#object-portability) in [Passare a Workfront nell&#39;archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Abilita archiviazione cloud Adobe

È necessaria una versione di Workfront che supporti l’archiviazione cloud di Adobe. Se la tua organizzazione non utilizza già una versione supportata, contatta il rappresentante del tuo account Adobe.

Per informazioni sull&#39;abilitazione dell&#39;archiviazione cloud Adobe nel tuo ambiente, consulta [Abilitare l&#39;archiviazione cloud Adobe per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

>[!NOTE]
>
>I nuovi clienti hanno l’archiviazione cloud Adobe abilitata per impostazione predefinita e non hanno la possibilità di utilizzare l’archiviazione Workfront legacy.



## Archiviazione cloud Adobe in ambienti sandbox

L&#39;archiviazione cloud di Adobe è disponibile in [!DNL Workfront] ambienti sandbox, quindi puoi testarla prima di abilitarla in produzione. Tuttavia, il visualizzatore Frame.io non è disponibile in sandbox, pertanto l’esperienza completa di revisione e approvazione unificata deve essere convalidata in produzione.

Se disponi di una sandbox di aggiornamento personalizzata, devi aggiornarla dopo l’aggiornamento a una versione di Workfront che supporta l’archiviazione cloud di Adobe per accedere alle funzionalità di archiviazione cloud di Adobe nella sandbox. Per ulteriori informazioni, vedere [L&#39;ambiente Sandbox di aggiornamento personalizzato [!DNL Adobe Workfront] &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

## Considerazioni

* È possibile che Workfront non sia sincronizzato con Frame.io o Creative Cloud, ad esempio una risorsa eliminata in Workfront ma ancora visualizzata in Frame.io, contatta il supporto Workfront per sincronizzare nuovamente il tuo ambiente.


