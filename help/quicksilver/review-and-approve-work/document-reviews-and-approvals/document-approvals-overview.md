---
product-area: documents
navigation-topic: approvals
title: Panoramica sulla revisione e sull’approvazione unificata
description: Ulteriori informazioni sulla revisione e l'approvazione unificate fornite da Workfront e Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 32cb95c2-8d12-492b-ad89-b38e2a337fc5
source-git-commit: df02fa91f5cf87e73a9bf6183b57d42ba965ba09
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---


# Panoramica sulla revisione e sull’approvazione unificata

La revisione e l&#39;approvazione unificate basate su Workfront e Frame.io consentono ai coordinatori dei progetti di gestire i progetti e pianificare il lavoro in Workfront, mentre i creativi, gli esperti di marketing e le parti interessate possono rivedere e approvare le risorse in Frame.io.

## Requisiti di integrazione

* Workfront e Frame.io devono essere distribuiti nella stessa organizzazione Identity Management System (IMS).

* Gli utenti possono appartenere a una sola istanza di Workfront all’interno dell’organizzazione IMS.

* L’istanza di Workfront deve essere abilitata sullo storage aziendale Adobe Unified Experience e Adobe.

* L’integrazione deve essere configurata da Adobe Professional Services.


## Basato sullo storage aziendale Adobe

La revisione e l&#39;approvazione unificate si basano sullo storage aziendale Adobe, una soluzione di storage basata su cloud che funge da archivio centrale per le risorse dei prodotti aziendali Adobe, inclusi Workfront e Frame.io. <!--, and Creative Cloud.-->

I principali vantaggi dello storage aziendale Adobe includono:

* Livello di storage unificato per risorse creative e di gestione del lavoro
* Autorizzazioni centralizzate con Adobe Identity Management System (IMS) per il controllo sicuro degli accessi
* Visibilità completa delle risorse in Workfront e Frame.io <!--, and Creative Cloud apps -->
* Storage scalabile e gestione delle quote per le esigenze aziendali

Per ulteriori dettagli, consulta [Panoramica sull&#39;archiviazione aziendale di Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Revisione e approvazione unificate

Con la revisione e l&#39;approvazione unificate, puoi:

* Crea e gestisci revisioni e approvazioni direttamente da Workfront
* Monitorare lo stato di revisioni e approvazioni in tempo reale
* Centralizzare feedback e approvazioni in un&#39;unica posizione
* Assicurati che tutte le parti interessate abbiano accesso alle versioni più recenti delle risorse
* Utilizzare i revisori AI per automatizzare le revisioni di conformità al brand
* e molto altro

Per ulteriori informazioni, vedere [Unified document approvals: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### Utilizzare il visualizzatore Frame.io

Utilizza il visualizzatore Frame.io per rivedere e approvare le risorse. Il visualizzatore Frame.io fornisce

* Strumenti di markup e commento
* Cronologia e confronto delle versioni
* Commenti con marca temporale per le recensioni video
* Accesso mobile per revisioni e approvazioni in movimento

Per ulteriori informazioni, vedere [Introduzione alla revisione e all&#39;approvazione unificate](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md).

#### Limiti di revisione video

Per le richieste di bozze video, il limite massimo annuale è fissato al 10% del totale delle licenze Workfront a pagamento di un&#39;organizzazione: Standard e Light. Questo limite viene applicato a livello di organizzazione.

Gli amministratori di Workfront ricevono notifiche quando l’utilizzo raggiunge l’80% e il 100% del limite.

Questo limite non si applica ai clienti Frame.io Enterprise.

#### Tipi di file supportati nel visualizzatore Frame.io

Il visualizzatore Frame.io supporta tutti i tipi comuni di video, immagini, audio, PDF e MS® Office. Per un elenco dettagliato dei file supportati, vedere [Tipi di file supportati in Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Accesso e licenze per il visualizzatore Frame.io

Il visualizzatore Frame.io è il visualizzatore predefinito per tutti i flussi di lavoro di revisione e approvazione di Workfront. È incluso automaticamente per tutti gli utenti di Workfront con una licenza a pagamento. Non è richiesta alcuna licenza Frame.io aggiuntiva per utilizzare il visualizzatore Frame.io per le revisioni e le approvazioni.

Se la tua organizzazione desidera sfruttare le funzionalità Frame.io aggiuntive disponibili con questa integrazione, ad esempio per caricare le risorse direttamente nei progetti in Frame.io, puoi acquistare una licenza Frame.io Enterprise. Contatta il rappresentante del tuo account Adobe per pianificare una demo ed esplorare i vantaggi della soluzione Frame.io completa.

La funzionalità Workfront Proofing non è disponibile con questa integrazione.

## Potente gestione dei progetti in Workfront

I coordinatori dei progetti possono sfruttare le potenti funzionalità di gestione dei progetti di Workfront per pianificare, tracciare e gestire il lavoro.

Per ulteriori informazioni sulla gestione dei progetti in Workfront, vedere [Progetti: indice articolo](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Struttura imposta e convenzioni di denominazione

Poiché la revisione e l’approvazione unificate vengono create utilizzando lo storage aziendale Adobe, è necessario tenere presenti alcune convenzioni di denominazione e struttura applicate durante la gestione di progetti e documenti.

* I nomi degli oggetti devono essere univoci e non possono essere duplicati
* Lo storage aziendale Adobe richiede nomi univoci per gli oggetti peer con lo stesso elemento padre nella struttura gerarchica
* I documenti non possono avere lo stesso nome se appartengono allo stesso progetto
* I nomi dei documenti non possono contenere i seguenti caratteri speciali: \ / : * ? &quot; | &lt; >
* I nomi dei documenti non possono superare i 255 caratteri

Tenendo presenti queste limitazioni, Workfront rinomina automaticamente gli oggetti o i documenti in base alle esigenze per evitare conflitti.

### Condivisione e autorizzazioni

Come parte dell&#39;integrazione, le autorizzazioni utente sono controllate in Workfront e si estendono fino a Frame.io. Ciò significa che non è possibile invitare un utente a un progetto in Frame.io o modificare le autorizzazioni utente in Frame.io. Queste azioni devono essere eseguite tramite la finestra modale Condivisione progetto in Workfront.

Nella tabella seguente viene illustrato il mapping delle autorizzazioni di Workfront alle autorizzazioni Frame.io:

<table>
<tr>
<th>Autorizzazione utente di Workfront</th>
<th>Autorizzazione utente Frame.io</th>
</tr>
<tr>
<td>Gestione</td>
<td>Modifica e condividi</td>
</tr>
<tr>
<td>Contribuisci</td>
<td>Modifica e condividi</td>
</tr>
<tr>
<td>Visualizzazione</td>
<td>Solo commento</td>
</tr>
</table>



### Gestione dei documenti in Workfront

I documenti caricati su Workfront vengono memorizzati nello storage aziendale di Adobe e sono accessibili sia in Workfront che in Frame.io. Quando carichi un documento in un’attività o un problema in Workfront, viene creata una cartella generata dal sistema nell’archiviazione aziendale di Adobe che eredita le autorizzazioni dall’attività o dal problema. Tutti i documenti caricati su tale attività o problema sono memorizzati in tale cartella e da essa ereditano le autorizzazioni. Per ulteriori informazioni sui documenti in Workfront, vedere [Panoramica sulla nuova area documenti](/help/quicksilver/documents/managing-documents/documents-area.md) e [Autorizzazioni oggetto e panoramica del livello di accesso per il modello di archiviazione aziendale Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

### Limitazioni dell’esperienza documentale

Le seguenti funzionalità di Document non sono incluse:

<!--* External document providers-->
* Accesso alle bozze in Workfront
* Visualizzatore documenti in Workfront
* Documenti preferiti
* Richiedi documenti










<!--
# Unified Approvals overview

>[!IMPORTANT]
>
>The content of this article refers to updated document approval functionality that is only available for specific accounts. For information on standard approval processes, see the articles listed in [Work approvals](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

Unified Approvals, previously referred to as New Document Approvals, is a holistic redesign of the existing approvals process that is currently in development for Adobe Workfront. Currently available in limited release, it is designed to be a practical and effective solution for businesses requiring comprehensive stakeholder engagement and version-specific document approvals. Its thoughtful design and purposeful new features facilitate collaboration, role clarity, and version control in the approval process, enhancing efficiency and accountability.

## Key differences from Proofing and legacy document approvals

**Differences from Proofing**

* Document approval participants display in the document Summary, not the proofing workflow tab.
* Unified Approvals are not supported in the current reporting tool. 

    You can join the new Canvas Dashboards beta to [Create a report dashboard for review and approvals](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md), or you can use the Document approval metrics widget available in new Home and Canvas Dashboards provides the following details about Unified Approvals:

    * Approvals by decision
    * Average approval time
    * Pending approvals
    * Overdue approvals

**Differences from Legacy document approvals**

With Unified Approvals, you can

* Add reviewers in addition to approvers
* Designate an entire Workfront team as either reviewers or approvers
* Set a deadline for the review or approval
* Create and resuse approval templates
* Utilize new versions 
* View multiple key performance indicators for your approvals in Workfront Home widgets
* Use Canvas Dashboards to view reporting details about Unified Approvals

## Using Unified Approvals

For users looking to create or manage document approvals, see the articles listed in [Set up and manage unified approvals: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/set-up-and-manage-doc-asset-approvals-toc.md)

For users looking to review or approve documents for which they have received a request, see the articles listed in [Approve and review documents: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/review-documents-toc.md).



-->