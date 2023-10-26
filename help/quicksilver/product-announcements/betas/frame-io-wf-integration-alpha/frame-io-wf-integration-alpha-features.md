---
content-type: reference
navigation-topic: betas
title: "Integrazione nativa alfa Adobe Workfront e Frame.io: funzioni"
description: Funzioni pianificate per l'integrazione alfa nativa di Adobe Workfront e Frame.io
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
source-git-commit: 0ad33f377086f71699c550e2300731056a834e72
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---


# Integrazione alfa nativa di Adobe Workfront e Frame.io: funzioni

## Casi d’uso e test delle funzioni

Con questa integrazione, il nostro obiettivo è consentire ai creativi di rimanere nel loro strumento scelto (CC o Frame.io) per condurre la creazione dei contenuti e le revisioni tra pari, mentre i project manager coordinano il lavoro e inizializzano e monitorano il processo di revisione formale dall&#39;interno di Workfront. Ciò può essere ottenuto utilizzando il meglio di entrambe le soluzioni: le nuove approvazioni dei documenti di Workfront per la gestione delle approvazioni dei contenuti, insieme alle funzionalità di revisione dei contenuti offerte da Frame.io. Collettivamente, le nuove approvazioni dei documenti e Frame.io formeranno la nuova esperienza di revisione e approvazione dei contenuti end-to-end. 

Per ulteriori informazioni sul funzionamento dell&#39;alfa e sulle modalità di partecipazione, vedere [Integrazione di Adobe Workfront e Frame.io alfa: panoramica](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>Se vi imbatteste in queste pagine senza che la vostra azienda partecipasse a questo programma alfa, assicuratevi di trattare le informazioni con attenzione e contattate l&#39;amministratore Workfront o Frame.io per ulteriori informazioni.

<!--Initial setup and basic test scenario 

As part of the alpha program, we've provisioned a new test Frame.io account for you and connected it to a new group "Frame.io alpha testing" in your existing Workfront Preview or Sandbox environment. To test the delivered functionality please log in to your Workfront Preview or Sandbox instance and  perform the following steps: 

Coordinators: Within Workfront, create a project with the "Frame.io alpha testing" group assigned as project group 

Coordinators: Within Workfront, assign your creatives to the project or Frame enabled tasks and change the project status to "Current" 

Creatives: Check your emails for an invite to the newly created Frame.io project 

Creatives: Click on the "Join project" button within the invitation email to join the Frame.io project, review the creative brief within the project and start your content creation within your CC tool of choice 

Creatives: Upload your created assets to Frame.io and add them to the linked Workfront project (or assigned Frame enabled tasks)  

Coordinators: Within Workfront, see the linked Frame.io assets in your project and assign reviewers / approvers (new document approvals: More help on this feature) 

Stakeholders: Withing Workfront, view your approval request in Workfront Home or Document Details and review the Frame connected document in the Frame.io Viewer. Leave a comment feedback 

Coordinators: Within Workfront, view the stakeholder created comments within the Updates section of the Frame.io connected document in Workfront 

Stakeholders: Make a decision from within the Frame.io Viewer 

Creatives: Within Frame.io, notice the overall approval decision made for your assets 

Creatives: Within Frame.io, Apply the requested changes by adding the updated version to the version stack of the connected asset 

Coordinators: Within Workfront, assign approvers / reviewers to the new version upload and monitor the progress until it reaches sign-off-->

## Feature plan

Di seguito sono riportate informazioni sui casi d’uso principali che stiamo cercando di affrontare e sulle funzioni che abbiamo pianificato di svolgere. <!--, along with documentation to get you started testing.-->


### Gli amministratori di Workfront possono impostare una connessione tra i gruppi di Workfront e gli account Frame.io

* _In Workfront è possibile collegare un gruppo Workfront a un account Frame.io_

* All&#39;interno di Frame.io verrà creato un nuovo team Frame.io che rappresenta il gruppo Workfront connesso

**Potenziali miglioramenti nelle versioni future:**

* Disconnettere un gruppo Workfront da un account Frame.io

* Collegare un gruppo Workfront a un team Frame.io esistente

### I coordinatori dei progetti possono configurare quali progetti Workfront vengono inviati a Frame.io e far aggiungere al progetto in Frame.io le creatività assegnate in Workfront.

* Possibilità di contrassegnare i progetti Workfront come Frame.io abilitati assegnando un gruppo Frame connesso

* _Miglioramento: possibilità di attivare o disattivare le attività all&#39;interno dei progetti Workfront come attività Frame che, a loro volta, creeranno cartelle di attività all&#39;interno di Frame.io_

* Quando lo stato di un progetto Workfront è impostato su Corrente, viene creato un progetto connesso corrispondente in Frame, gli utenti assegnati a Workfront vengono aggiunti al progetto Frame e viene inviata una notifica e-mail da Frame.io

   * Tutti i membri del progetto Workfront (utenti e team) verranno aggiunti come collaboratori al progetto Frame.io (durante la creazione del progetto e in seguito)

   * _Modifica: utenti e team assegnati ad attività di Workfront abilitate per i frame verranno aggiunti come collaboratori al progetto Frame.io e notificati (durante la creazione del progetto e in seguito)_

* I documenti (Riassunti creativi) aggiunti al progetto e le attività con Frame abilitato verranno inviati al progetto Frame.io (nella rispettiva cartella di lavoro) quando il progetto viene creato (trigger: stato progetto impostato su Corrente)

   * Si consiglia di limitare la quantità di documenti aggiunti al progetto prima di diventare attivi solo nelle descrizioni creative, per evitare di inviare più documenti non necessari a Frame.io

* _Miglioramento: Utenti / team esplicitamente non assegnati a un&#39;attività Workfront abilitata per frame verrà rimossa dal progetto Frame.io_

**Potenziali miglioramenti nelle versioni future:**

* Le attività con frame abilitato possono essere configurate sui modelli di progetto

* La nuova versione caricata in specifiche creative verrà inviata al frame

* Sincronizzazione dei progetti ottimizzata (disconnessione di progetti, risincronizzazione di progetti e documenti, ecc.)

### All’interno di Frame.io, i creativi possono inviare le risorse create al progetto Workfront per una revisione formale

* Possibilità di collegare una singola risorsa Frame.io a un progetto o attività WF. Verrà creato un riferimento a una risorsa in Workfront

* La nuova versione caricata all&#39;interno di Frame.io creerà automaticamente una nuova versione del documento in Workfront sulle risorse collegate

* _Miglioramento: possibilità di contrassegnare le attività Workfront a cui si fa riferimento come completate dall&#39;interno di Frame.io_

* _Miglioramento: nel caso in cui il documento Workfront connesso venga eliminato, rimane all&#39;interno di Frame.io e può essere riconnesso alla stessa o ad altra attività di progetto_

**Potenziali miglioramenti nelle versioni future:**

* Possibilità di inviare contemporaneamente più risorse Frame.io a Workfront

* Registrazione dell&#39;ora per il progetto/attività Workfront da Frame.io

### I coordinatori dei progetti possono assegnare il processo di approvazione formale ai documenti collegati da Frame.io

* Gli utenti e i team di Workfront possono essere aggiunti alle nuove approvazioni di documenti per documenti connessi a Frame.io

* _Miglioramento: quando un utente/team non è più condiviso da un documento abilitato per i frame, perde anche l’accesso alla risorsa nel Visualizzatore Frame.io_

**Potenziali miglioramenti nelle versioni future:**

* Inviare più risorse come una singola revisione

* Assegnazione in blocco di approvatori/revisori a documenti Workfront

### Le parti interessate possono condurre la loro revisione e approvazione all&#39;interno di Frame.io Viewer

* Le parti interessate riceveranno una notifica e potranno visualizzare il documento Frame connected nel visualizzatore Frame.io

* È possibile accedere al visualizzatore Frame.io da posizioni diverse all&#39;interno di Workfront, ad esempio Elenco documenti, Dettagli documento, Home di Workfront

* Possibilità di sfruttare le funzionalità esistenti di revisione e commento fornite dal visualizzatore Frame.io che sarà sincronizzato con il flusso di aggiornamento di Workfront

* _Possibilità di prendere una nuova decisione di approvazione del documento dal visualizzatore Frame.io_

### All&#39;interno di Frame.io, i creativi verranno informati sulle decisioni generali relative alla risorsa Frame.io collegata

* _Miglioramento: lo stato di approvazione generale del documento verrà visualizzato sulla risorsa all&#39;interno di Frame.io_

### I coordinatori dei progetti possono inviare risorse finali all&#39;AEM

* _Miglioramento: i documenti con frame collegato, inclusi i metadati, possono essere inviati all&#39;AEM utilizzando l&#39;attuale connettore Workfront + AEM Asset CS_