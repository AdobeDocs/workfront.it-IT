---
product-area: documents
navigation-topic: approvals
title: Autorizzazioni degli oggetti e panoramica del livello di accesso per il modello di storage aziendale Adobe
description: Autorizzazioni di storage aziendale e panoramica degli accessi ad Adobe
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
source-git-commit: 89dcc972e2e29890763dba6b5f7a44489a2eee5a
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---


# Autorizzazioni degli oggetti e panoramica del livello di accesso per il modello di storage aziendale Adobe

<!--linked in UI -->

Adobe enterprise storage è una soluzione di storage basata su cloud che funge da archivio di storage centrale per le risorse tra i prodotti aziendali Adobe. Gli ambienti Workfront che utilizzano lo storage aziendale Adobe presentano autorizzazioni degli oggetti e comportamenti dei livelli di accesso leggermente diversi rispetto a quelli che utilizzano lo storage dei documenti Workfront legacy.

## Livelli di accesso

I livelli di accesso a Workfront si applicano solo all&#39;interno di Workfront. Le restrizioni per progetti e documenti in Workfront non si applicano sempre ad altre applicazioni Adobe.

### Ambienti che utilizzano sia lo storage aziendale Adobe che lo storage Workfront legacy

L’accesso ai documenti funziona in modo diverso a seconda che il progetto sia basato sullo storage aziendale Adobe o su quello Workfront legacy:

* **Archiviazione Workfront legacy**: i progetti, i programmi, i portfolio e i modelli che utilizzano l&#39;archiviazione Workfront legacy seguono la logica standard del livello di accesso Workfront per l&#39;accesso ai documenti. Quando un livello di accesso ha **Nessun accesso** selezionato per i documenti, non è possibile visualizzare i documenti in Workfront o in altri prodotti Adobe come Frame.io o Creative Cloud.
* **Archiviazione aziendale Adobe**: i progetti, i programmi, i portfolio e i modelli che utilizzano l&#39;archiviazione aziendale Adobe seguono la logica del livello di accesso all&#39;archiviazione aziendale Adobe per altri prodotti Adobe.


   * **Autorizzazioni per oggetti Progetti, programmi, portfolio e modelli**: se per progetti, programmi, portfolio e modelli è selezionato **Nessun accesso** a un livello di accesso, ma l&#39;oggetto è condiviso con gli utenti, questi non possono visualizzare l&#39;oggetto in Workfront, ma possono comunque visualizzare il nome dell&#39;oggetto e qualsiasi documento associato in altri strumenti di Adobe, come Frame.io e Adobe Creative Cloud.
   * **Autorizzazioni documenti**: quando per un livello di accesso è selezionato **Nessun accesso** per i documenti, gli utenti non sono in grado di visualizzare i documenti nei progetti in Workfront, ma possono comunque visualizzare e gestire i documenti per i progetti condivisi con loro in altri strumenti di Adobe, come Frame.io e Adobe Creative Cloud. Questo perché l’accesso ai documenti è determinato dalle autorizzazioni a livello di progetto nello storage aziendale di Adobe, anziché dai soli livelli di accesso di Workfront.

Se nell&#39;ambiente Workfront è abilitato lo storage aziendale Adobe, è possibile creare sia progetti di storage aziendale Adobe che progetti di storage Workfront legacy. I progetti di storage Workfront precedenti presentano un&#39;icona accanto al nome del progetto in qualsiasi punto di Workfront. I progetti Adobe per lo storage aziendale non presentano un&#39;icona.

![icona legacy workfront storage accanto al nome del progetto](assets/legacy-project-icon.png)


### Ambienti che utilizzano solo lo storage aziendale Adobe

Non è possibile modificare le autorizzazioni dei documenti a livello di accesso per progetti, programmi e portfolio che utilizzano lo storage aziendale Adobe.

Tutti i livelli di accesso dispongono dell&#39;accesso in modifica ai documenti. Le autorizzazioni a livello di progetto determinano l’accesso ai documenti in altri strumenti di Adobe.

Non è possibile limitare l&#39;accesso all&#39;ereditarietà dei documenti.


### Ambienti che utilizzano solo storage Workfront legacy

Nessuna modifica ai livelli o al comportamento di accesso ai documenti.


## Progetti

Gli utenti con autorizzazioni a livello di progetto possono visualizzare e gestire i documenti per progetti in altri prodotti Adobe come Frame.io e Adobe Creative Cloud.

I nomi dei progetti sono visibili anche all’esterno di Workfront per i progetti ESM.

I dati finanziari non sono visibili all’esterno di Workfront per i progetti ESM.

## Attività e problemi

I documenti vengono memorizzati a livello di progetto, ma possono essere condivisi con singole attività e problemi, in base alle esigenze. Gli utenti con l’accesso alle attività e ai problemi ereditano automaticamente l’accesso ai documenti dal progetto. Non puoi modificare il loro livello di accesso. Possono gestire l’accesso o non accedervi.