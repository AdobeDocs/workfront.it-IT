---
product-area: documents
navigation-topic: approvals
title: Passare a Workfront sull’archiviazione cloud Adobe
description: Pianifica il rollout di Workfront sull’archiviazione cloud Adobe. Scopri le differenze tra gli oggetti di archiviazione cloud di Adobe, inclusa la nuova area Documenti e l’esperienza di revisione Frame.io, e decidi in che modo l’archiviazione cloud di Adobe viene implementata nel tuo ambiente.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 4821a7db4014b2a73c0466726ba3d239c318d5f0
workflow-type: tm+mt
source-wordcount: '2702'
ht-degree: 0%

---

# Passare a Workfront sull’archiviazione cloud Adobe

Workfront sull’archiviazione cloud di Adobe offre l’esperienza completa di revisione e approvazione unificata: recensioni nel visualizzatore Frame.io, potenti flussi di lavoro di approvazione, visibilità delle risorse tra i prodotti e altro ancora.

Gli oggetti esistenti continuano a funzionare come fanno attualmente. La nuova area Documenti, il visualizzatore Frame.io e altri comportamenti di archiviazione cloud Adobe si applicano solo agli oggetti che utilizzano l’archiviazione cloud Adobe.

Questo articolo è destinato agli amministratori di Workfront che si preparano a eseguire il rollout di Workfront sull’archiviazione cloud Adobe. Vengono illustrate le principali differenze sugli oggetti di archiviazione cloud di Adobe, come scegliere il tipo di rollout e cosa pensare prima di abilitare l’archiviazione cloud di Adobe per i tuoi utenti.

>[!IMPORTANT]
>
>È necessaria una versione di Workfront che supporti l’archiviazione cloud di Adobe. Se la tua organizzazione non utilizza già una versione supportata, contatta il rappresentante del tuo account Adobe.



## Comprendere lo storage legacy Workfront e lo storage cloud Adobe

Dopo aver aggiornato il contratto per includere la nuova esperienza di revisione e approvazione unificata, l’ambiente può contenere due tipi di oggetti: oggetti sullo storage legacy di Workfront (gli oggetti che hai oggi) e oggetti creati utilizzando lo storage cloud Adobe. Ad alto livello, i due modelli di archiviazione differiscono per la posizione in cui si trovano i dati, i prodotti Adobe in grado di visualizzarli e le funzionalità disponibili:

|  | Oggetto sullo storage legacy Workfront | Oggetto sull’archiviazione cloud di Adobe |
|---|---|---|
| Back-end di archiviazione | Solo Workfront | Archiviazione cloud Adobe |
| Visibilità tra prodotti | Solo Workfront | Workfront, Frame.io e Creative Cloud |
| Funzionalità | Funzionalità legacy | Nuove funzionalità |

Gli oggetti creati prima dell’abilitazione dell’archiviazione cloud di Adobe nell’area di configurazione rimangono nell’archiviazione Workfront legacy. I nuovi comportamenti descritti in questo articolo si applicano solo agli oggetti di archiviazione cloud di Adobe che crei insieme agli utenti una volta abilitata l’archiviazione cloud di Adobe.

## Differenze nell’archiviazione cloud di Adobe

La più grande modifica giornaliera con l’archiviazione cloud di Adobe è rappresentata dalla nuova area Documenti e dal visualizzatore Frame.io, che consente la revisione e l’approvazione al suo interno. Esistono altre differenze che influiscono sulla modalità di gestione di oggetti, documenti e revisioni.

La tabella seguente riepiloga le principali differenze quando si passa all’archiviazione cloud di Adobe. Ogni area nella tabella è collegata alla sezione dettagliata seguente.

| Area | Differenze | Cosa bisogna sapere |
|---|---|---|
| [Area nuovi documenti](#the-new-documents-area) | L&#39;area Documenti riprogettata e unificata sostituisce l&#39;area Documenti legacy. | Area Documenti non globale. Accedere ai documenti da un programma, portfolio, progetto, attività o problema. |
| [Autorizzazioni documento](#document-permissions) | I documenti ereditano le autorizzazioni dal progetto, dall&#39;attività o dal problema a cui sono collegati. | Impossibile condividere o impostare autorizzazioni per singoli documenti. Puoi gestire tutti gli accessi tramite l’oggetto modale Share in Workfront, che si propaga nelle cartelle di documenti generate dal sistema. |
| [Mappatura autorizzazioni oggetto](#object-permissions-mapping) | Le autorizzazioni Gestione e Contribuisci di Workfront sono mappate su Modifica e condividi in Frame.io. Visualizza le mappe solo per commenti. | Le autorizzazioni vengono gestite in Workfront. Sia gli utenti Manage che Contribute acquisiscono la funzionalità di condivisione esterna in Frame.io. |
| [Visualizzatore recensioni e approvazioni](#review-and-approval-viewer) | Il visualizzatore Frame.io sostituisce il visualizzatore di bozze di Workfront. | Incluso per tutti gli utenti di Workfront, inclusi gli utenti esterni assegnati a una revisione o approvazione. Supporta markup, commenti con marca temporale, cronologia delle versioni, dispositivi mobili, formati 40+, file fino a 500 GB. |
| [Regole di denominazione degli oggetti](#object-naming-rules) | Si applicano rigide regole di denominazione: nomi univoci all’interno di un portfolio o progetto, nessun carattere speciale, nessun punto finale o spazio, limite di 255 caratteri. | Workfront rinomina automaticamente gli oggetti in caso di conflitti. Modelli di audit che generano nuovi nomi e strutture di progetto. |
| [Portabilità oggetto](#object-portability) | Nella maggior parte degli scenari, è possibile spostare, copiare e convertire oggetti solo tra modelli di memorizzazione simili. | Puoi convertire un oggetto legacy in Adobe Cloud Storage in tre casi specifici. I documenti e le cartelle di documenti non vengono spostati dall&#39;archivio legacy durante la conversione. |
| [Funzionalità non disponibili](#capabilities-not-available-on-adobe-cloud-storage-objects) | Workfront Proof, il visualizzatore documenti di Workfront, i documenti preferiti e i documenti di richiesta non fanno parte dell’esperienza. | Gli oggetti legacy mantengono queste funzionalità. Workfront Proof non riceverà un nuovo investimento e verrà ritirato in una versione futura. |
| [Quota di archiviazione](#storage-quota) | L’archiviazione è in pool per i progetti legacy di Workfront e i progetti di archiviazione cloud Adobe. 60 GB per utente con licenza. Nessun cappuccio rigido. | Gli amministratori di sistema possono visualizzare l’utilizzo dello storage nella pagina Informazioni cliente di Configurazione. |
| [Limite di revisione video annuale](#annual-video-review-cap) | Limite a livello organizzativo per le richieste di bozze video al 10% delle licenze utente Workfront a pagamento (Standard e Light). | Una volta raggiunto, non ci saranno nuove recensioni video fino al prossimo periodo annuale. Notifiche in-app all’80% e al 100%. Non si applica ai clienti Frame.io Enterprise. |
| [Workfront Fusion](#workfront-fusion-on-adobe-cloud-storage-projects) | Gli scenari di Fusion basati su bozze esistenti non funzionano automaticamente con i progetti di archiviazione cloud di Adobe. | Gli scenari con ambito di progetti legacy continuano a funzionare. Ogni scenario interessato ottiene uno dei tre percorsi seguenti: modifica, ricostruzione o ritiro. Nuovi connettori previsti per il terzo trimestre 2026. |

### La nuova area Documenti

La nuova area Documenti è un’esperienza di documenti unificati progettata per l’archiviazione cloud Adobe. Semplifica la navigazione, consolida l&#39;attività di revisione e approvazione ed è il punto di ingresso per il visualizzatore Frame.io.

L’area Documenti globale non fa parte della nuova esperienza. Nei progetti Adobe di archiviazione cloud, puoi accedere ai documenti da un programma, un portfolio, un progetto, un’attività o un problema.

Per ulteriori informazioni, vedere [Area Documenti](/help/quicksilver/documents/managing-documents/documents-area.md).

### Autorizzazioni documento

Le autorizzazioni per i documenti sono fondamentalmente diverse nei progetti di archiviazione cloud Adobe:

* Impossibile condividere o impostare autorizzazioni per singoli documenti. Le autorizzazioni vengono invece applicate alle cartelle di documenti generate dal sistema che contengono i documenti.
* Le cartelle dei documenti generate dal sistema ereditano le autorizzazioni dal progetto, dall&#39;attività o dal problema principale.
* Le sottocartelle ereditano le autorizzazioni dalla cartella documenti generata dal sistema padre.
* Le sottoattività non ereditano le autorizzazioni dalle attività padre. Per accedere alla cartella dei documenti generata dal sistema, è necessario essere aggiunti direttamente a una sottoattività.


Per ulteriori informazioni sul funzionamento delle autorizzazioni per i documenti, vedere [Autorizzazioni per gli oggetti e panoramica del livello di accesso per il modello di archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).


### Mappatura delle autorizzazioni oggetto

Le autorizzazioni sono impostate in Workfront e scorrono in una direzione fino a Frame.io. Non puoi invitare utenti a un progetto di archiviazione cloud Adobe in Frame.io o modificare le autorizzazioni utente in Frame.io.

>[!TIP]
>
>Forma i coordinatori dei progetti affinché l&#39;accesso a Frame.io rifletta a valle le autorizzazioni di Workfront. Se una parte interessata segnala che non può accedere a una revisione su un progetto di archiviazione cloud Adobe, la correzione è in Workfront e non in Frame.io.

Nella tabella seguente le autorizzazioni degli oggetti Workfront vengono associate alle autorizzazioni Frame.io:

| Autorizzazione Workfront | Autorizzazione Frame.io |
|---|---|
| Gestione | Modifica e condividi |
| Contribuisci | Modifica e condividi |
| Visualizzazione | Solo commento |

Sia Gestisci che Contribuisci mappano a **Modifica e condividi** in Frame.io. Esaminando i modelli di condivisione per i progetti di Adobe Cloud Storage, considera se sia adatto al modello di governance per i collaboratori disporre delle stesse funzionalità lato revisione dei manager, inclusa la condivisione esterna.

Per ulteriori informazioni, consulta [Autorizzazioni oggetto e panoramica del livello di accesso per il modello di archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#permission-mapping-to-frameio).


### Visualizzatore recensioni e approvazioni

Sugli oggetti di archiviazione cloud Adobe, il visualizzatore Frame.io è l’area di revisione e approvazione al posto di Workfront Proof. Il visualizzatore Frame.io è incluso per tutti gli utenti di Workfront senza costi aggiuntivi, inclusi gli utenti esterni assegnati a una revisione o approvazione.

Il visualizzatore Frame.io fornisce:

* Strumenti di markup e commento, inclusi disegno a mano libera e forme standard quali cerchi, frecce e quadrati
* Commenti con precisione del frame per le recensioni video
* Cronologia delle versioni e confronto delle versioni
* Accesso mobile per revisioni e approvazioni in movimento
* Supporto per oltre 40 formati di file, inclusi tutti i tipi comuni di video, immagini, audio, PDF e Microsoft Office, con riproduzione nativa per formati video professionali come ProRes, H.265 e DNxHD e supporto per file fino a 500 GB


### Regole di denominazione degli oggetti

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


### Portabilità degli oggetti

Nella maggior parte degli scenari è possibile spostare, copiare e convertire oggetti Workfront tra modelli di memorizzazione simili. Ad esempio, puoi spostare un’attività da un progetto di archiviazione cloud Adobe a un altro progetto di archiviazione cloud Adobe. In tre casi specifici, puoi convertire un oggetto di archiviazione Workfront legacy in archiviazione cloud Adobe:

* Convertire un’attività di archiviazione Workfront legacy in un progetto di archiviazione cloud Adobe
* Conversione di un portfolio di storage Workfront legacy in un portfolio di storage cloud Adobe
* Creare un progetto di archiviazione cloud Adobe da un modello di archiviazione Workfront legacy

>[!NOTE]
>
>In tutti e tre gli scenari di conversione, i documenti e le cartelle di documenti non vengono spostati dallo storage legacy di Workfront allo storage cloud Adobe. I documenti esistenti sull’oggetto legacy prima della conversione rimangono nell’archiviazione legacy.

#### Convertire un’attività legacy in un progetto di archiviazione cloud Adobe

Per convertire un’attività di archiviazione Workfront legacy in un progetto di archiviazione cloud Adobe, utilizza il flusso di conversione in progetto esistente per l’attività. Durante la conversione:

* Le sottoattività e i problemi vengono spostati nel nuovo progetto.
* I documenti allegati all&#39;attività e i relativi flussi di lavoro di approvazione rimangono sul progetto originale.
* Le approvazioni del lavoro e i collegamenti agli oggetti di risoluzione vengono rimossi.
* L&#39;attività originale viene eliminata.

<!--
For more information, see [Convert a task to a project](/help/quicksilver/manage-work/tasks/convert-tasks/convert-task-to-project.md).
-->

#### Convertire un portfolio legacy in un portfolio di archiviazione cloud Adobe

Un amministratore Workfront può convertire un portfolio di archiviazione Workfront legacy in un portfolio di archiviazione cloud Adobe dall’area di configurazione. Dopo la conversione:

* Non è più possibile spostare i progetti di storage Workfront legacy nel portfolio.
* Tutti i nuovi progetti creati nel portfolio utilizzano l’archiviazione cloud Adobe.
* Frame.io è il visualizzatore di documenti nei progetti di archiviazione cloud Adobe del portfolio.
* I progetti secondari che utilizzano lo storage legacy Workfront rimangono sullo storage legacy.
* I programmi secondari rimangono nell&#39;archiviazione legacy.

  >[!NOTE]
  >
  >Un programma legacy secondario viene convertito automaticamente in Adobe Cloud Storage solo quando qualcuno vi aggiunge manualmente un progetto Adobe Cloud Storage.

Per ulteriori informazioni, consulta [Convertire i portfolio legacy in Adobe Cloud Storage](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md).

#### Creare un progetto di archiviazione cloud Adobe da un modello legacy

Quando crei un progetto da un modello di archiviazione Workfront legacy, la casella di controllo **Crea il progetto nell&#39;archiviazione cloud Adobe** nella finestra di dialogo di creazione del progetto determina il tipo di archiviazione del nuovo progetto. Il comportamento della casella di controllo dipende dalla posizione in cui viene creato il progetto:

* **Esterno a un portfolio**: la casella di controllo è disponibile e deselezionata per impostazione predefinita. Selezionala per creare il nuovo progetto sull’archiviazione cloud Adobe.
* **All&#39;interno di un portfolio di archiviazione cloud Adobe**: la casella di controllo è selezionata e bloccata. Il nuovo progetto deve corrispondere al tipo di archiviazione del portfolio.
* **In un portfolio di archiviazione legacy di Workfront**: la casella di controllo non è disponibile. Il nuovo progetto utilizza lo storage legacy Workfront.

Per ulteriori informazioni, vedere [Creare progetti](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Funzionalità non disponibili negli oggetti di archiviazione cloud di Adobe

Le seguenti funzionalità non fanno parte degli oggetti di archiviazione cloud Adobe:

* Workfront Proof
* Visualizzatore documenti di Workfront
* Documenti preferiti
* Richiedi documenti

I progetti legacy mantengono l’accesso a Workfront Proof e alle funzionalità dei documenti legacy elencate in precedenza. Workfront Proof non riceverà un nuovo investimento in futuro e verrà ritirato in una versione futura.

### Quota di archiviazione

L’archiviazione è in pool per gli oggetti Workfront legacy e gli oggetti di archiviazione cloud Adobe. Ogni utente con licenza riceve 60 GB di storage. Non esiste alcun limite all’utilizzo dello storage, ma gli amministratori di Workfront ricevono notifiche e-mail quando l’utilizzo raggiunge il 75%, il 90% e il 100% della quota.

Gli amministratori di sistema possono passare a **Configurazione** > **Sistema** > **Informazioni cliente** per visualizzare l&#39;utilizzo e la quota di archiviazione correnti.

Per ulteriori informazioni, vedere [Controllare i limiti di archiviazione dei documenti](/help/quicksilver/documents/managing-documents/check-document-storage.md).


### Limite di revisione video annuale

È previsto un limite annuo per le richieste di bozze video, fissato al 10% del totale delle licenze utente Workfront a pagamento dell’organizzazione (Standard e Light). Questo limite viene applicato a livello di organizzazione.

* Gli amministratori di Workfront ricevono notifiche in-app quando l’utilizzo raggiunge l’80% e il 100% del limite.
* Una volta raggiunto il limite, non puoi creare nuove richieste di revisione video fino al periodo annuale successivo.
* Questo limite non si applica ai clienti Frame.io Enterprise. Se la tua organizzazione rivede regolarmente grandi quantità di contenuti video, contatta il rappresentante del tuo account Adobe per scoprire le licenze Enterprise di Frame.io.

Per ulteriori informazioni, consulta le Domande frequenti sulla revisione e l&#39;approvazione di risorse e video in [Panoramica unificata sulla revisione e l&#39;approvazione](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

### Progetti di archiviazione cloud Workfront Fusion su Adobe

Gli scenari Workfront Fusion esistenti basati su prove legacy non funzionano automaticamente con i progetti di archiviazione cloud di Adobe. I moduli specifici della bozza, i webhook e gli endpoint API hanno equivalenti diretti in alcuni casi e cambiamenti significativi in altri. Gli scenari con ambito di progetti legacy continuano a funzionare come fanno attualmente.

I connettori di fusione con supporto nativo per revisione e approvazione unificate saranno disponibili nel terzo trimestre del 2026.

Per informazioni dettagliate sull&#39;impatto sui tipi di scenario comuni e su come classificare ogni scenario come Modifica, Ricostruisci o Ritira in base alle funzionalità, consulta [Aggiornare gli scenari di Workfront Fusion per la revisione e l&#39;approvazione unificate](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).


## Scegli come viene eseguito il rollout dell’archiviazione cloud di Adobe

Decidi in che modo l’archiviazione cloud di Adobe viene visualizzata dagli utenti. Esistono due configurazioni e ciascuna può essere applicata all’intera organizzazione o a gruppi Workfront specifici.

Per istruzioni dettagliate, consulta [Abilitare l&#39;archiviazione cloud Adobe per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

* **Solo archiviazione cloud Adobe**: per impostazione predefinita, i nuovi progetti utilizzano l&#39;archiviazione cloud Adobe. Gli utenti non possono creare progetti legacy.
* **Archiviazione cloud Adobe e archiviazione Workfront legacy**: quando gli utenti creano un progetto, scelgono tra l&#39;archiviazione cloud Adobe (con etichetta &quot;Nuovo progetto&quot;) e l&#39;archiviazione Workfront legacy (con etichetta &quot;Archiviazione legacy&quot;).

  ![scegli un tipo di progetto](assets/choose-project-type.png)



>[!TIP]
>
>Per mettere l’archiviazione cloud di Adobe prima di un team più piccolo, applica una delle due configurazioni a un singolo gruppo Workfront. Questo consente di eseguire un programma pilota mirato prima di implementarlo in modo più ampio. Per una valutazione controllata, consigliamo di iniziare con un rollout a livello di gruppo, quindi di espanderlo all’intera organizzazione una volta che il gruppo pilota avrà convalidato l’esperienza.

Gli oggetti esistenti mantengono il modello di archiviazione con cui sono stati creati. La modifica della preferenza di archiviazione predefinita non comporta la modifica di alcun oggetto esistente.

## Pianificare il rollout

Ogni ambiente Workfront è diverso. Prima di abilitare l’archiviazione cloud di Adobe per i tuoi utenti, pianifica l’aspetto di un rollout di successo per la tua organizzazione. I suggerimenti riportati di seguito non sono un elenco di controllo, ma un punto di partenza per il tuo piano.

**1. Selezionare un gruppo pilota.** Un rollout con ambito di gruppo consente di mettere l’archiviazione cloud Adobe prima di un team più piccolo, raccogliere feedback e apportare le modifiche necessarie prima di un rollout più ampio. Scegli un gruppo i cui modelli di lavoro siano sufficientemente rappresentativi da far emergere i problemi che desideri conoscere in anticipo.

**2. Comunicare la modifica agli utenti finali.** La più grande modifica visibile per revisori, approvatori e proprietari di progetti è la nuova area Documenti e il visualizzatore Frame.io che consente la revisione e l’approvazione sui progetti di archiviazione cloud Adobe. Pianifica come presentarli in modo che gli utenti sappiano cosa aspettarsi quando incontrano il loro primo progetto di archiviazione cloud Adobe. L&#39;articolo [Introduzione a revisione e approvazione unificate](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) è un utile punto di partenza per il materiale rivolto all&#39;utente finale.

**3. Pianifica la disponibilità del connettore Workfront Fusion.** I connettori di fusione con supporto nativo per revisione e approvazione unificate saranno disponibili nel terzo trimestre del 2026. Gli scenari di Fusion basati su bozze esistenti continuano a funzionare sui progetti legacy. Prima di inserire i team che dipendono da tali scenari nel programma pilota per l’archiviazione cloud di Adobe, decidi se attendere i nuovi connettori, ricostruisci in base all’API corrente o sostituisci tali scenari con funzioni native di revisione e approvazione unificate.

Per informazioni dettagliate sull&#39;impatto sui tipi di scenario comuni e su come classificare ogni scenario come Modifica, Ricostruisci o Ritira in base alle funzionalità, consulta [Aggiornare gli scenari di Workfront Fusion per la revisione e l&#39;approvazione unificate](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).


## Articoli correlati

* [Panoramica dell’archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md)
* [Abilitare l’archiviazione cloud Adobe per la tua organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)
* [Panoramica sulla revisione e sull’approvazione unificata](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Introduzione a revisione e approvazione unificate](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [L’area Documenti](/help/quicksilver/documents/managing-documents/documents-area.md)
* [Autorizzazioni di oggetto e panoramica del livello di accesso per il modello di archiviazione cloud Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)

