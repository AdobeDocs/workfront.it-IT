---
product-area: documents
navigation-topic: approvals
title: Passare a Workfront sullo storage aziendale Adobe
description: Pianifica il rollout di Workfront sullo storage aziendale Adobe. Scopri le differenze tra gli oggetti di storage aziendale Adobe, inclusa la nuova area Documenti e l’esperienza di revisione Frame.io, e decidi come lo storage aziendale Adobe viene implementato nel tuo ambiente.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 722ba7f6617e3ccc1a1dcbf51f5d539c550617ab
workflow-type: tm+mt
source-wordcount: '2360'
ht-degree: 0%

---

# Passare a Workfront sullo storage aziendale Adobe

Lo storage aziendale Workfront on Adobe offre l&#39;esperienza completa di revisione e approvazione unificata: revisioni nel visualizzatore Frame.io, potenti flussi di lavoro di approvazione, visibilità delle risorse tra i prodotti e altro ancora.

Gli oggetti esistenti continuano a funzionare come fanno attualmente. La nuova area Documenti, il visualizzatore Frame.io e altri comportamenti di archiviazione aziendale di Adobe si applicano solo agli oggetti che utilizzano l’archiviazione aziendale di Adobe.

Questo articolo è destinato agli amministratori di Workfront che si preparano a implementare Workfront sullo storage aziendale Adobe. Vengono illustrate le principali differenze relative agli oggetti di storage aziendale Adobe, alla scelta del tipo di rollout e a cosa pensare prima di abilitare lo storage aziendale Adobe per gli utenti.

>[!IMPORTANT]
>
>Per utilizzare il visualizzatore Frame.io e lo storage aziendale Adobe, il contratto Workfront deve includere una SKU Workfront V2. Per ulteriori informazioni, vedere le domande frequenti in [Panoramica unificata su revisione e approvazione](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md#getting-started-with-unified-review-and-approval).



## Comprendere lo storage legacy Workfront e lo storage aziendale Adobe

Dopo aver aggiornato il contratto per includere la nuova esperienza di revisione e approvazione unificata, l’ambiente può contenere due tipi di oggetti: oggetti sullo storage legacy di Workfront (gli oggetti attualmente disponibili) e oggetti creati utilizzando lo storage aziendale di Adobe. Ad alto livello, i due modelli di archiviazione differiscono per la posizione in cui si trovano i dati, i prodotti Adobe in grado di visualizzarli e le funzionalità disponibili:

|  | Oggetto sullo storage legacy Workfront | Oggetto sullo storage aziendale Adobe |
|---|---|---|
| Back-end di archiviazione | Solo Workfront | Storage aziendale Adobe |
| Visibilità tra prodotti | Solo Workfront | Workfront, Frame.io e Creative Cloud |
| Funzionalità | Funzionalità legacy | Nuove funzionalità |

Gli oggetti creati prima dell&#39;attivazione dello storage aziendale Adobe nell&#39;area di configurazione rimangono sullo storage Workfront legacy. I nuovi comportamenti descritti in questo articolo si applicano solo agli oggetti di storage aziendale di Adobe creati dall&#39;utente una volta abilitato lo storage aziendale di Adobe.

## Differenze nello storage aziendale Adobe

La più grande modifica quotidiana con lo storage aziendale Adobe è rappresentata dalla nuova area Documenti e dal visualizzatore Frame.io, che consente la revisione e l&#39;approvazione al suo interno. Esistono altre differenze che influiscono sulla modalità di gestione di oggetti, documenti e revisioni.

Nella tabella seguente sono riepilogate le principali differenze quando si passa allo storage aziendale Adobe. Ogni area nella tabella è collegata alla sezione dettagliata seguente.

| Area | Differenze | Cosa bisogna sapere |
|---|---|---|
| [Area nuovi documenti](#the-new-documents-area) | L&#39;area Documenti riprogettata e unificata sostituisce l&#39;area Documenti legacy. | Area Documenti non globale. Accedere ai documenti da un programma, portfolio, progetto, attività o problema. |
| [Autorizzazioni documento](#document-permissions) | I documenti ereditano le autorizzazioni dal progetto, dall&#39;attività o dal problema a cui sono collegati. | Impossibile condividere o impostare autorizzazioni per singoli documenti. Puoi gestire tutti gli accessi tramite l’oggetto modale Share in Workfront, che si propaga nelle cartelle di documenti generate dal sistema. |
| [Mappatura autorizzazioni oggetto](#object-permissions-mapping) | Le autorizzazioni Gestione e Contribuisci di Workfront sono mappate su Modifica e condividi in Frame.io. Visualizza le mappe solo per commenti. | Le autorizzazioni vengono gestite in Workfront. Sia gli utenti Manage che Contribute acquisiscono la funzionalità di condivisione esterna in Frame.io. |
| [Visualizzatore recensioni e approvazioni](#review-and-approval-viewer) | Il visualizzatore Frame.io sostituisce il visualizzatore di bozze di Workfront. | Incluso per tutti gli utenti di Workfront con una licenza a pagamento. Supporta markup, commenti con marca temporale, cronologia delle versioni, dispositivi mobili, formati 40+, file fino a 500 GB. |
| [Regole di denominazione degli oggetti](#object-naming-rules) | Si applicano rigide regole di denominazione: nomi univoci all’interno di un portfolio o progetto, nessun carattere speciale, nessun punto finale o spazio, limite di 255 caratteri. | Workfront rinomina automaticamente gli oggetti in caso di conflitti. Modelli di audit che generano nuovi nomi e strutture di progetto. |
| [Portabilità oggetto](#object-portability) | È possibile spostare, copiare e convertire oggetti solo tra modelli di memorizzazione simili. | Gli oggetti di storage aziendale Adobe non possono essere spostati su progetti legacy o viceversa. Se si sposta un progetto di storage aziendale Adobe in un portfolio o programma legacy, lo storage principale viene convertito in storage aziendale Adobe. |
| [Funzionalità non disponibili](#capabilities-not-available-on-adobe-enterprise-storage-objects) | Workfront Proof, il visualizzatore documenti di Workfront, i documenti preferiti e i documenti di richiesta non fanno parte dell’esperienza. | Gli oggetti legacy mantengono queste funzionalità. Workfront Proof non riceverà un nuovo investimento e verrà ritirato in una versione futura. |
| [Quota di archiviazione](#storage-quota) | Lo storage è in pool per i progetti legacy Workfront e Adobe Enterprise. 60 GB per utente con licenza. Nessun cappuccio rigido. | Gli amministratori di sistema possono visualizzare l’utilizzo dello storage nella pagina Informazioni cliente di Configurazione. |
| [Limite di revisione video annuale](#annual-video-review-cap) | Limite a livello organizzativo per le richieste di bozze video al 10% delle licenze utente Workfront a pagamento (Standard e Light). | Una volta raggiunto, non ci saranno nuove recensioni video fino al prossimo periodo annuale. Notifiche in-app all’80% e al 100%. Non si applica ai clienti Frame.io Enterprise. |
| [Workfront Fusion](#workfront-fusion-on-adobe-enterprise-storage-projects) | Gli scenari di Fusion basati su bozze esistenti non funzionano automaticamente con i progetti di storage aziendale Adobe. | Gli scenari con ambito di progetti legacy continuano a funzionare. Ogni scenario interessato ottiene uno dei tre percorsi seguenti: modifica, ricostruzione o ritiro. Nuovi connettori previsti per il terzo trimestre 2026. |

### La nuova area Documenti

La nuova area Documenti è un&#39;esperienza di documenti unificati progettata per lo storage aziendale Adobe. Semplifica la navigazione, consolida l&#39;attività di revisione e approvazione ed è il punto di ingresso per il visualizzatore Frame.io.

L’area Documenti globale non fa parte della nuova esperienza. Nei progetti di storage aziendale Adobe, è possibile accedere ai documenti da un programma, un portfolio, un progetto, un&#39;attività o un problema.

Per ulteriori informazioni, vedere [Area Documenti](/help/quicksilver/documents/managing-documents/documents-area.md).

### Autorizzazioni documento

Le autorizzazioni per i documenti sono fondamentalmente diverse nei progetti di storage aziendale Adobe:

* Impossibile condividere o impostare autorizzazioni per singoli documenti. Le autorizzazioni vengono invece applicate alle cartelle di documenti generate dal sistema che contengono i documenti.
* Le cartelle dei documenti generate dal sistema ereditano le autorizzazioni dal progetto, dall&#39;attività o dal problema principale.
* Le sottocartelle ereditano le autorizzazioni dalla cartella documenti generata dal sistema padre.
* Le sottoattività non ereditano le autorizzazioni dalle attività padre. Per accedere alla cartella dei documenti generata dal sistema, è necessario essere aggiunti direttamente a una sottoattività.


Per ulteriori informazioni sul funzionamento delle autorizzazioni per i documenti, vedere [Autorizzazioni per gli oggetti e panoramica del livello di accesso per il modello di archiviazione aziendale Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).


### Mappatura delle autorizzazioni oggetto

Le autorizzazioni sono impostate in Workfront e scorrono in una direzione fino a Frame.io. Non puoi invitare utenti a un progetto di archiviazione aziendale Adobe in Frame.io o modificare le autorizzazioni utente in Frame.io.

>[!TIP]
>
>Forma i coordinatori dei progetti affinché l&#39;accesso a Frame.io rifletta a valle le autorizzazioni di Workfront. Se una delle parti interessate segnala di non poter accedere a una revisione su un progetto di storage aziendale Adobe, la correzione si trova in Workfront e non in Frame.io.

Nella tabella seguente le autorizzazioni degli oggetti Workfront vengono associate alle autorizzazioni Frame.io:

| Autorizzazione Workfront | Autorizzazione Frame.io |
|---|---|
| Gestione | Modifica e condividi |
| Contribuisci | Modifica e condividi |
| Visualizzazione | Solo commento |

Sia Gestisci che Contribuisci mappano a **Modifica e condividi** in Frame.io. Quando si esaminano i modelli di condivisione per i progetti di storage aziendale Adobe, valutare se sia adatto al modello di governance per i collaboratori disporre delle stesse funzionalità lato revisione dei manager, inclusa la condivisione esterna.

Per ulteriori informazioni, vedere [Autorizzazioni degli oggetti e panoramica del livello di accesso per il modello di storage aziendale Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#permission-mapping-to-frameio).


### Visualizzatore recensioni e approvazioni

Sugli oggetti di archiviazione aziendale Adobe, il visualizzatore Frame.io è la superficie di revisione e approvazione al posto di Workfront Proof. Il visualizzatore Frame.io è incluso per tutti gli utenti di Workfront con una licenza a pagamento.

Il visualizzatore Frame.io fornisce:

* Strumenti di markup e commento, inclusi disegno a mano libera e forme standard quali cerchi, frecce e quadrati
* Commenti con precisione del frame per le recensioni video
* Cronologia delle versioni e confronto delle versioni
* Accesso mobile per revisioni e approvazioni in movimento
* Supporto per oltre 40 formati di file, inclusi tutti i tipi comuni di video, immagini, audio, PDF e Microsoft Office, con riproduzione nativa per formati video professionali come ProRes, H.265 e DNxHD e supporto per file fino a 500 GB


### Regole di denominazione degli oggetti

Lo storage aziendale Adobe applica regole rigorose di denominazione e struttura per mantenere coerente il livello di storage tra i prodotti Adobe. Queste regole si applicano agli oggetti creati nei progetti di storage aziendale Adobe. I progetti legacy esistenti mantengono i nomi correnti.

Le seguenti regole si applicano ai progetti di storage aziendale Adobe:

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
>Se si creano progetti di archiviazione aziendale Adobe da modelli, esaminare i modelli esistenti in modo che i nomi e la struttura dei progetti generati siano conformi alle regole precedenti.


### Portabilità degli oggetti

È possibile spostare, copiare e convertire oggetti Workfront tra modelli di memorizzazione simili. È ad esempio possibile spostare un&#39;attività da un progetto di storage aziendale Adobe a un altro progetto di storage aziendale Adobe. Non è possibile spostare o copiare un&#39;attività o un problema da un progetto di storage aziendale Adobe a un progetto legacy o viceversa.

Oggi, quando si crea o si sposta un progetto di storage aziendale Adobe in un portfolio o programma legacy, il portfolio o il programma viene automaticamente convertito in un oggetto di storage aziendale Adobe. Una versione futura offrirà agli amministratori di sistema un maggiore controllo sugli oggetti che verranno automaticamente convertiti.

### Funzionalità non disponibili sugli oggetti di storage aziendale Adobe

Le seguenti funzionalità non fanno parte degli oggetti di storage aziendale di Adobe:

* Workfront Proof
* Visualizzatore documenti di Workfront
* Documenti preferiti
* Richiedi documenti

I progetti legacy mantengono l’accesso a Workfront Proof e alle funzionalità dei documenti legacy elencate in precedenza. Workfront Proof non riceverà un nuovo investimento in futuro e verrà ritirato in una versione futura.

### Quota di archiviazione

Lo storage è in pool per gli oggetti Workfront legacy e per gli oggetti di storage aziendale Adobe. Ogni utente con licenza riceve 60 GB di storage. Non esiste alcun limite all’utilizzo dello storage, ma gli amministratori di Workfront ricevono notifiche e-mail quando l’utilizzo raggiunge il 75%, il 90% e il 100% della quota.

Gli amministratori di sistema possono passare a **Configurazione** > **Sistema** > **Informazioni cliente** per visualizzare l&#39;utilizzo e la quota di archiviazione correnti.

Per ulteriori informazioni, vedere [Controllare i limiti di archiviazione dei documenti](/help/quicksilver/documents/managing-documents/check-document-storage.md).


### Limite di revisione video annuale

È previsto un limite annuo per le richieste di bozze video, fissato al 10% del totale delle licenze utente Workfront a pagamento dell’organizzazione (Standard e Light). Questo limite viene applicato a livello di organizzazione.

* Gli amministratori di Workfront ricevono notifiche in-app quando l’utilizzo raggiunge l’80% e il 100% del limite.
* Una volta raggiunto il limite, non puoi creare nuove richieste di revisione video fino al periodo annuale successivo.
* Questo limite non si applica ai clienti Frame.io Enterprise. Se la tua organizzazione rivede regolarmente grandi quantità di contenuti video, contatta il rappresentante del tuo account Adobe per scoprire le licenze Enterprise di Frame.io.

Per ulteriori informazioni, consulta le Domande frequenti sulla revisione e l&#39;approvazione di risorse e video in [Panoramica unificata sulla revisione e l&#39;approvazione](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

### Workfront Fusion sui progetti di storage aziendale Adobe

Gli scenari Workfront Fusion esistenti basati su prove legacy non funzionano automaticamente con i progetti di storage aziendale Adobe. I moduli specifici della bozza, i webhook e gli endpoint API hanno equivalenti diretti in alcuni casi e cambiamenti significativi in altri. Gli scenari con ambito di progetti legacy continuano a funzionare come fanno attualmente.

I connettori di fusione con supporto nativo per revisione e approvazione unificate saranno disponibili nel terzo trimestre del 2026.

Per informazioni dettagliate sull&#39;impatto sui tipi di scenario comuni e su come classificare ogni scenario come Modifica, Ricostruisci o Ritira in base alle funzionalità, consulta [Aggiornare gli scenari di Workfront Fusion per la revisione e l&#39;approvazione unificate](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).


## Scegli il modo in cui viene implementato lo storage aziendale Adobe

È possibile decidere in che modo lo storage aziendale Adobe viene visualizzato agli utenti. Esistono due configurazioni e ciascuna può essere applicata all’intera organizzazione o a gruppi Workfront specifici.

Per istruzioni dettagliate, consulta [Abilitare l&#39;archiviazione aziendale Adobe per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

* **Solo archiviazione aziendale Adobe**: per impostazione predefinita, i nuovi progetti utilizzano l&#39;archiviazione aziendale Adobe. Gli utenti non possono creare progetti legacy.
* **Archiviazione aziendale Adobe e archiviazione Workfront legacy**: durante la creazione di un progetto, gli utenti possono scegliere tra lo storage aziendale Adobe (denominato &quot;Nuovo progetto&quot;) e lo storage Workfront legacy (denominato &quot;Archiviazione legacy&quot;).

  ![scegli un tipo di progetto](assets/choose-project-type.png)



>[!TIP]
>
>Per mettere lo storage aziendale Adobe davanti a un team più piccolo, applicare una delle due configurazioni a un singolo gruppo Workfront. Questo consente di eseguire un programma pilota mirato prima di implementarlo in modo più ampio. Per una valutazione controllata, consigliamo di iniziare con un rollout a livello di gruppo, quindi di espanderlo all’intera organizzazione una volta che il gruppo pilota avrà convalidato l’esperienza.

Gli oggetti esistenti mantengono il modello di archiviazione con cui sono stati creati. La modifica della preferenza di archiviazione predefinita non comporta la modifica di alcun oggetto esistente.

## Pianificare il rollout

Ogni ambiente Workfront è diverso. Prima di abilitare lo storage aziendale Adobe per i tuoi utenti, pianifica l’aspetto di un rollout di successo per la tua organizzazione. I suggerimenti riportati di seguito non sono un elenco di controllo, ma un punto di partenza per il tuo piano.

**1. Selezionare un gruppo pilota.** Un rollout con ambito di gruppo consente di mettere lo storage aziendale Adobe davanti a un team più piccolo, raccogliere feedback e apportare le modifiche necessarie prima di un rollout più ampio. Scegli un gruppo i cui modelli di lavoro siano sufficientemente rappresentativi da far emergere i problemi che desideri conoscere in anticipo.

**2. Comunicare la modifica agli utenti finali.** La più grande modifica visibile per revisori, approvatori e proprietari di progetti è la nuova area Documenti e il visualizzatore Frame.io che consente la revisione e l&#39;approvazione sui progetti di storage aziendale Adobe. Pianifica come presentarli in modo che gli utenti sappiano cosa aspettarsi quando incontrano il loro primo progetto di storage aziendale Adobe. L&#39;articolo [Introduzione a revisione e approvazione unificate](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) è un utile punto di partenza per il materiale rivolto all&#39;utente finale.

**3. Pianifica la disponibilità del connettore Workfront Fusion.** I connettori di fusione con supporto nativo per revisione e approvazione unificate saranno disponibili nel terzo trimestre del 2026. Gli scenari di Fusion basati su bozze esistenti continuano a funzionare sui progetti legacy. Prima di inserire i team che dipendono da tali scenari nel progetto pilota per lo storage aziendale di Adobe, decidi se attendere i nuovi connettori, se eseguire la ricostruzione in base all’API corrente o se sostituire tali scenari con funzioni native di revisione e approvazione unificate.

Per informazioni dettagliate sull&#39;impatto sui tipi di scenario comuni e su come classificare ogni scenario come Modifica, Ricostruisci o Ritira in base alle funzionalità, consulta [Aggiornare gli scenari di Workfront Fusion per la revisione e l&#39;approvazione unificate](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).


## Articoli correlati

* [Panoramica sull’archiviazione aziendale Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md)
* [Abilitare lo storage aziendale Adobe per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)
* [Panoramica sulla revisione e sull’approvazione unificata](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Introduzione a revisione e approvazione unificate](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [L’area Documenti](/help/quicksilver/documents/managing-documents/documents-area.md)
* [Autorizzazioni degli oggetti e panoramica del livello di accesso per il modello di storage aziendale Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)