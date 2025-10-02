---
product-area: documents
navigation-topic: approvals
title: Panoramica dell’integrazione Frame.io
description: Panoramica dell’integrazione Frame.io
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b5f0150b-40b5-4386-98bc-374e7ca65b74
source-git-commit: f8d81996846f7b719bf3e5e8aaa2ad9ba1805cff
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 0%

---

# Panoramica dell’integrazione Frame.io

L’integrazione Workfront e Frame.io consente ai coordinatori dei progetti di gestire i progetti e pianificare il lavoro in Workfront, mentre i creativi, gli esperti di marketing e le parti interessate possono rivedere e approvare le risorse in Frame.io.

## Requisiti di integrazione

Adobe Professional Services deve abilitare l&#39;integrazione di Workfront e Frame.io.

<!--
* Workfront and Frame.io must be deployed to the same Identity Management system (IMS) organization.

* Users can belong to only one Workfront instance within the IMS organization.

* The Workfront instance must be enabled on the Adobe Unified Experience.

* The integration is configured by Adobe Professional Services. 
-->

## Basato sullo storage aziendale Adobe

Il nucleo di questa integrazione è lo storage aziendale Adobe, una soluzione di storage basata su cloud che funge da archivio centrale per le risorse dei prodotti aziendali Adobe, inclusi Workfront e Frame.io. <!--, and Creative Cloud.-->

I principali vantaggi dello storage aziendale Adobe includono:

* Livello di storage unificato per risorse creative e di gestione del lavoro
* Autorizzazioni centralizzate tramite Adobe IMS per il controllo sicuro degli accessi
* Visibilità completa delle risorse in Workfront e Frame.io <!--, and Creative Cloud apps -->
* Storage scalabile e gestione delle quote per le esigenze aziendali

Per ulteriori dettagli, consulta [Panoramica sull&#39;archiviazione aziendale di Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

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

#### Limiti di revisione video

Per le richieste di bozze video, il limite massimo annuale è fissato al 10% del totale delle licenze Workfront a pagamento di un&#39;organizzazione: Standard e Light. Questo limite viene applicato a livello di organizzazione.

Gli amministratori di Workfront riceveranno notifiche quando l’utilizzo raggiunge l’80% e il 100% del limite.

Questo limite non si applica ai clienti Frame.io Enterprise.

#### Tipi di file supportati nel visualizzatore Frame.io

Il visualizzatore Frame.io supporta tutti i tipi comuni di video, immagini, audio, PDF e MS® Office. Per un elenco dettagliato dei file supportati, vedere [Tipi in Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Accesso e licenze per il visualizzatore Frame.io

Il visualizzatore Frame.io è il visualizzatore predefinito per tutti i flussi di lavoro di revisione e approvazione di Workfront. È incluso automaticamente per tutti gli utenti di Workfront con una licenza a pagamento. Non è richiesta alcuna licenza Frame.io aggiuntiva per utilizzare il visualizzatore Frame.io per le revisioni e le approvazioni.

Se la tua organizzazione desidera sfruttare le funzionalità Frame.io aggiuntive disponibili con questa integrazione, ad esempio per caricare le risorse direttamente nei progetti in Frame.io, puoi acquistare una licenza Enterprise Frame.io. Contatta il rappresentante del tuo account Adobe per pianificare una demo ed esplorare i vantaggi della soluzione Frame.io completa.

La funzionalità Workfront Proofing non è disponibile con questa integrazione.

## Potente gestione dei progetti in Workfront

Con l&#39;integrazione Workfront e Frame.io, i coordinatori dei progetti possono sfruttare le potenti funzionalità di gestione dei progetti di Workfront per pianificare, tracciare e gestire il lavoro.

Per ulteriori informazioni sulla gestione dei progetti in Workfront, vedere [Progetti: indice articolo](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Struttura imposta e convenzioni di denominazione

Poiché questa integrazione viene creata utilizzando ESM, esistono alcune convenzioni di denominazione e struttura applicate di cui tenere conto durante la gestione di progetti e documenti.

* I nomi degli oggetti devono essere univoci e non possono essere duplicati
* ESM richiede nomi univoci per gli oggetti peer con lo stesso padre nella struttura gerarchica
* I documenti non possono avere lo stesso nome se appartengono allo stesso progetto

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
<td>Gestisci</td>
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

I documenti vengono gestiti a livello di progetto con questa integrazione e non possono essere caricati sulle attività o sui problemi in questo momento.

L’accesso ai documenti viene gestito anche a livello di progetto. Se un utente ha accesso a un progetto, può accedere a tutti i documenti associati a tale progetto.

### Limitazioni dell’esperienza documentale

Poiché questa integrazione viene creata utilizzando lo storage aziendale di Adobe, esistono alcune limitazioni all’esperienza con i documenti originali in Workfront:

#### Limitazioni

Le seguenti funzionalità non saranno incluse in questa integrazione:

<!--* External document providers-->
* Accesso alle bozze in Workfront
* Visualizzatore documenti in Workfront
* Documenti preferiti
* Richiedi documenti


<!--#### Temporary limitations

For now, the following capabilities are not available:

* Send documents to Adobe Experience Manager Assets
* Multi-stage approvals
* Upload documents to comments or updates in Workfront
* Upload documents to tasks or issues in Workfront-->
