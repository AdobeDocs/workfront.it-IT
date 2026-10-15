---
product-area: documents
navigation-topic: approvals
title: Differenze nell’archiviazione cloud di Adobe
description: Comprendi le principali differenze sugli oggetti di archiviazione cloud di Adobe, tra cui la nuova area Documenti, il visualizzatore Frame.io, le autorizzazioni per i documenti, le regole di denominazione degli oggetti, la quota di archiviazione e Workfront Fusion.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 4f63b6c4f4c73bedba707aed6b02c9046f9b356c
workflow-type: tm+mt
source-wordcount: '1717'
ht-degree: 0%
---
# Differenze nell’archiviazione cloud di Adobe

Dopo aver aggiornato il contratto per includere la nuova esperienza di revisione e approvazione unificata, l’ambiente può contenere due tipi di oggetti: oggetti sullo storage legacy di Workfront (gli oggetti che hai oggi) e oggetti creati utilizzando lo storage cloud Adobe. La nuova area Documenti, il visualizzatore Frame.io e gli altri comportamenti qui descritti si applicano solo agli oggetti che utilizzano l’archiviazione cloud di Adobe.

Per informazioni sull&#39;orientamento dello spostamento e sulle modalità di attivazione, vedere [Sposta su Workfront nell&#39;archivio cloud Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Comprendere lo storage legacy Workfront e lo storage cloud Adobe

Ad alto livello, i due modelli di archiviazione differiscono per la posizione in cui si trovano i dati, i prodotti Adobe in grado di visualizzarli e le funzionalità disponibili:

|  | Oggetto sullo storage legacy Workfront | Oggetto sull’archiviazione cloud di Adobe |
|---|---|---|
| Back-end di archiviazione | Solo Workfront | Archiviazione cloud Adobe |
| Visibilità tra prodotti | Solo Workfront | Workfront, Frame.io e Creative Cloud |
| Funzionalità | Funzionalità legacy | Nuove funzionalità |

Gli oggetti creati prima dell’archiviazione cloud di Adobe sono di default e rimangono nell’archiviazione Workfront legacy. I comportamenti descritti in questo articolo si applicano solo agli oggetti di archiviazione cloud di Adobe che vengono creati insieme agli utenti una volta che l’archiviazione cloud di Adobe è l’impostazione predefinita.

## Riepilogo delle differenze

La più grande modifica giornaliera con l’archiviazione cloud di Adobe è rappresentata dalla nuova area Documenti e dal visualizzatore Frame.io, che consente la revisione e l’approvazione al suo interno. Esistono altre differenze che influiscono sulla modalità di gestione di oggetti, documenti e revisioni. Ogni area nella tabella seguente è collegata alla sezione dettagliata sottostante.

| Area | Differenze | Cosa bisogna sapere |
|---|---|---|
| [Area nuovi documenti](#the-new-documents-area) | L&#39;area Documenti riprogettata e unificata sostituisce l&#39;area Documenti legacy. | Non esiste un&#39;area Documenti globale. È possibile accedere ai documenti da un programma, portfolio, progetto, attività o problema. |
| [Autorizzazioni documento](#document-permissions) | I documenti ereditano le autorizzazioni dal progetto, dall&#39;attività o dal problema a cui sono collegati. | Impossibile condividere o impostare autorizzazioni per singoli documenti. Puoi gestire tutti gli accessi tramite l’oggetto modale Share in Workfront, che si propaga nelle cartelle di documenti generate dal sistema. |
| [Mappatura autorizzazioni oggetto](#object-permissions-mapping) | Le autorizzazioni Gestisci e Contribuisci vengono mappate su Modifica e condividi in Frame.io. Visualizza le mappe solo per commenti. | Puoi gestire le autorizzazioni in Workfront. Sia gli utenti Manage che Contribute acquisiscono la funzionalità di condivisione esterna in Frame.io. |
| [Visualizzatore recensioni e approvazioni](#review-and-approval-viewer) | Il visualizzatore Frame.io sostituisce il visualizzatore di bozze di Workfront. | È incluso per tutti gli utenti di Workfront, inclusi gli utenti esterni assegnati a una revisione o approvazione. Supporta markup, commenti con marca temporale, cronologia delle versioni, dispositivi mobili, formati 40+ e file fino a 500 GB. |
| [Regole di denominazione degli oggetti](#object-naming-rules) | Si applicano rigide regole di denominazione: nomi univoci all’interno di un portfolio o progetto, nessun carattere speciale, nessun punto o spazio finale e un limite di 255 caratteri. | Workfront rinomina automaticamente gli oggetti in caso di conflitti. Controlla i modelli che generano nuovi nomi e strutture di progetto. |
| [Portabilità oggetto](#object-portability) | Nella maggior parte degli scenari, è possibile spostare, copiare e convertire oggetti solo tra modelli di memorizzazione simili. | Puoi convertire un oggetto legacy in Adobe Cloud Storage in tre casi specifici. I documenti e le cartelle di documenti non vengono spostati dall&#39;archivio legacy durante la conversione. |
| [Funzionalità non disponibili](#capabilities-not-available-on-adobe-cloud-storage-objects) | Workfront Proof, il visualizzatore documenti di Workfront, i documenti preferiti e i documenti di richiesta non fanno parte dell’esperienza. | Gli oggetti legacy mantengono queste funzionalità. Workfront Proof non riceverà un nuovo investimento e verrà ritirato in una versione futura. |
| [Quota di archiviazione](#storage-quota) | Lo storage viene unito per i progetti Workfront precedenti e i progetti di storage cloud Adobe, a 60 GB per utente con licenza senza alcun limite rigido. | Gli amministratori di sistema possono visualizzare l’utilizzo dello storage nella pagina Informazioni cliente di Configurazione. |
| [Limite di revisione video annuale](#annual-video-review-cap) | Le richieste di bozze video sono limitate al 10% delle licenze Workfront a pagamento (Standard e Light). | Una volta raggiunto il limite, non puoi creare nuove recensioni video fino al periodo annuale successivo. Ricevi notifiche in-app all’80% e al 100%. Il limite non si applica ai clienti Frame.io Enterprise. |
| [Workfront Fusion](#workfront-fusion-on-adobe-cloud-storage-projects) | Gli scenari di Fusion basati su bozze esistenti non funzionano automaticamente con i progetti di archiviazione cloud di Adobe. | Gli scenari con ambito di progetti legacy continuano a funzionare. Ogni scenario interessato segue uno dei tre percorsi seguenti: modificare, ricreare o ritirare. |

## La nuova area Documenti

La nuova area Documenti è un’esperienza di documenti unificati progettata per l’archiviazione cloud Adobe. Semplifica la navigazione, consolida l&#39;attività di revisione e approvazione ed è il punto di ingresso per il visualizzatore Frame.io.

L’area Documenti globale non fa parte della nuova esperienza. Nei progetti Adobe di archiviazione cloud, puoi accedere ai documenti da un programma, un portfolio, un progetto, un’attività o un problema.

Per ulteriori informazioni, vedere [Area Documenti](/help/quicksilver/documents/managing-documents/documents-area.md).

## Autorizzazioni documento

Le autorizzazioni per i documenti sono fondamentalmente diverse nei progetti di archiviazione cloud Adobe:

* Impossibile condividere o impostare autorizzazioni per singoli documenti. Le autorizzazioni vengono invece applicate alle cartelle di documenti generate dal sistema che contengono i documenti.
* Le cartelle dei documenti generate dal sistema ereditano le autorizzazioni dal progetto, dall&#39;attività o dal problema principale.
* Le sottocartelle ereditano le autorizzazioni dalla cartella documenti generata dal sistema padre.
* Le sottoattività non ereditano le autorizzazioni dalle attività padre. Per accedere alla cartella dei documenti generata dal sistema, è necessario essere aggiunti direttamente a una sottoattività.

Per ulteriori informazioni sul funzionamento delle autorizzazioni per i documenti, vedere [Autorizzazioni per gli oggetti e panoramica del livello di accesso per il modello di archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Mappatura delle autorizzazioni oggetto

Le autorizzazioni sono impostate in Workfront e scorrono in una direzione fino a Frame.io. Non puoi invitare utenti a un progetto di archiviazione cloud Adobe in Frame.io o modificare le autorizzazioni utente in Frame.io.

>[!TIP]
>
>Forma i coordinatori dei progetti affinché l&#39;accesso a Frame.io rifletta a valle le autorizzazioni di Workfront. Se una parte interessata segnala che non può accedere a una revisione su un progetto di archiviazione cloud Adobe, la correzione si trova in Workfront e non in Frame.io.

Nella tabella seguente le autorizzazioni degli oggetti Workfront vengono associate alle autorizzazioni Frame.io:

| Autorizzazione Workfront | Autorizzazione Frame.io |
|---|---|
| Gestione | Modifica e condividi |
| Contribuisci | Modifica e condividi |
| Visualizzazione | Solo commento |

Mappatura di Gestisci e Contribuisci per la modifica e la condivisione in Frame.io. Esaminando i modelli di condivisione per i progetti di Adobe Cloud Storage, considera se sia adatto al modello di governance per i collaboratori disporre delle stesse funzionalità lato revisione dei manager, inclusa la condivisione esterna.

Per ulteriori informazioni, consulta [Autorizzazioni oggetto e panoramica del livello di accesso per il modello di archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#permission-mapping-to-frameio).

## Visualizzatore recensioni e approvazioni

Sugli oggetti di archiviazione cloud Adobe, il visualizzatore Frame.io è l’area di revisione e approvazione al posto di Workfront Proof. Il visualizzatore Frame.io è incluso per tutti gli utenti di Workfront senza costi aggiuntivi, inclusi gli utenti esterni assegnati a una revisione o approvazione.

Il visualizzatore Frame.io fornisce:

* Strumenti di markup e commento, inclusi disegno a mano libera e forme standard quali cerchi, frecce e quadrati
* Commenti con precisione del frame per le recensioni video
* Cronologia delle versioni e confronto delle versioni
* Accesso mobile per revisioni e approvazioni in movimento
* Supporto per oltre 40 formati di file, inclusi tutti i tipi comuni di video, immagini, audio, PDF e Microsoft Office, con riproduzione nativa per formati video professionali come ProRes, H.265 e DNxHD e supporto per file fino a 500 GB

## Regole di denominazione degli oggetti

L’archiviazione cloud Adobe applica regole strutturali e di denominazione rigorose per mantenere la coerenza del livello di archiviazione tra i vari prodotti Adobe. Queste regole si applicano agli oggetti creati sui progetti di archiviazione cloud Adobe. I progetti legacy esistenti mantengono i nomi correnti.

Ai progetti di archiviazione cloud Adobe si applicano le seguenti regole:

| Regola | Dettaglio |
|---|---|
| Nomi univoci di programmi e progetti | I programmi e i progetti non possono avere lo stesso nome se appartengono allo stesso portfolio. |
| Nomi di documenti univoci | I documenti non possono avere lo stesso nome se appartengono allo stesso progetto. I nomi dei documenti devono essere univoci all&#39;interno dello stesso elemento padre nella gerarchia delle cartelle. |
| Caratteri proibiti | Programmi, portfolio, progetti, modelli, attività, problemi, cartelle di documenti e documenti non possono contenere i seguenti caratteri speciali: `\ / : * ? " \| < >` |
| Caratteri finali | Programmi, portfolio, progetti, modelli, attività, problemi e cartelle di documenti non possono avere nomi che terminano con un punto o uno spazio. |
| Limite lunghezza nome | I nomi degli oggetti sono limitati a 255 caratteri. |

Se un nome è in conflitto con queste regole, Workfront rinomina automaticamente l&#39;oggetto per risolvere il conflitto.

>[!TIP]
>
>Se crei progetti Adobe Cloud Storage da modelli, controlla i modelli esistenti in modo che i nomi e la struttura dei progetti generati siano conformi alle regole precedenti.

## Portabilità degli oggetti

Nella maggior parte degli scenari, è possibile spostare, copiare e convertire oggetti Workfront solo tra modelli di memorizzazione simili. Ad esempio, puoi spostare un’attività da un progetto di archiviazione cloud Adobe a un altro progetto di archiviazione cloud Adobe. In tre casi specifici, puoi convertire un oggetto di archiviazione Workfront legacy in archiviazione cloud Adobe.

Per ulteriori informazioni, consulta [Convertire oggetti legacy in Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/convert-objects-to-adobe-cloud-storage.md).

## Funzionalità non disponibili negli oggetti di archiviazione cloud di Adobe

Le seguenti funzionalità non fanno parte degli oggetti di archiviazione cloud Adobe:

* Workfront Proof
* Visualizzatore documenti di Workfront
* Documenti preferiti
* Richiedi documenti

I progetti legacy mantengono l’accesso a Workfront Proof e alle funzionalità dei documenti legacy elencate in precedenza. Workfront Proof non riceverà un nuovo investimento in futuro e verrà ritirato in una versione futura.

## Quota di archiviazione

L’archiviazione è in pool per gli oggetti Workfront legacy e gli oggetti di archiviazione cloud Adobe. Ogni utente con licenza riceve 60 GB di storage. Non esiste alcun limite all’utilizzo dello storage, ma gli amministratori di Workfront ricevono notifiche e-mail quando l’utilizzo raggiunge il 75%, il 90% e il 100% della quota.

Per visualizzare l&#39;utilizzo e la quota di archiviazione correnti, vai a **Configurazione** > **Sistema** > **Informazioni cliente**.

Per ulteriori informazioni, vedere [Controllare i limiti di archiviazione dei documenti](/help/quicksilver/documents/managing-documents/check-document-storage.md).

## Limite di revisione video annuale

È previsto un limite annuo per le richieste di bozze video, fissato al 10% del totale delle licenze utente Workfront a pagamento dell’organizzazione (Standard e Light). Questo limite viene applicato a livello di organizzazione.

* Gli amministratori di Workfront ricevono notifiche in-app quando l’utilizzo raggiunge l’80% e il 100% del limite.
* Una volta raggiunto il limite, non puoi creare nuove richieste di revisione video fino al periodo annuale successivo.
* Questo limite non si applica ai clienti Frame.io Enterprise. Se la tua organizzazione rivede regolarmente grandi quantità di contenuti video, contatta il rappresentante del tuo account Adobe per scoprire le licenze Enterprise di Frame.io.

Per ulteriori informazioni, consulta le Domande frequenti sulla revisione e l&#39;approvazione di risorse e video in [Panoramica unificata sulla revisione e l&#39;approvazione](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

## Progetti di archiviazione cloud Workfront Fusion su Adobe

Gli scenari Workfront Fusion esistenti basati su prove legacy non funzionano automaticamente con i progetti di archiviazione cloud di Adobe. I moduli specifici della bozza, i webhook e gli endpoint API hanno equivalenti diretti in alcuni casi e cambiamenti significativi in altri. Gli scenari con ambito di progetti legacy continuano a funzionare come fanno attualmente.

Per informazioni dettagliate sull&#39;impatto sui tipi di scenario comuni e su come classificare ogni scenario come Modifica, Ricostruisci o Ritira in base alle funzionalità, consulta [Aggiornare gli scenari di Workfront Fusion per la revisione e l&#39;approvazione unificate](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).
