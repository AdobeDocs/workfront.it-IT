---
content-type: reference
navigation-topic: betas
title: "Integrazione nativa alfa Adobe Workfront e Frame.io: funzioni"
description: Funzioni pianificate per l'integrazione alfa nativa di Adobe Workfront e Frame.io
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
source-git-commit: 31adfeffeda9fc6aa4e76ceae7ef410d9c4c178c
workflow-type: tm+mt
source-wordcount: '1246'
ht-degree: 0%

---

# Integrazione nativa alfa di Adobe Workfront e Frame.io: funzioni e test

Con questa integrazione, il nostro obiettivo è consentire ai creativi di rimanere nel loro strumento scelto (CC o Frame.io) per condurre la creazione dei contenuti e le revisioni tra pari, mentre i project manager coordinano il lavoro e inizializzano e monitorano il processo di revisione formale dall&#39;interno di Workfront. Ciò può essere ottenuto utilizzando il meglio di entrambe le soluzioni: le nuove approvazioni dei documenti di Workfront per la gestione delle approvazioni dei contenuti, insieme alle funzionalità di revisione dei contenuti offerte da Frame.io. Collettivamente, le nuove approvazioni dei documenti e Frame.io formeranno la nuova esperienza di revisione e approvazione dei contenuti end-to-end. 

Per ulteriori informazioni sul funzionamento dell&#39;alfa e sulle modalità di partecipazione, vedere [Integrazione di Adobe Workfront e Frame.io alfa: panoramica](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>Se vi imbatteste in queste pagine senza che la vostra azienda partecipasse a questo programma alfa, assicuratevi di trattare le informazioni con attenzione e contattate l&#39;amministratore Workfront o Frame.io per ulteriori informazioni.

## Scenario di test di base

Per consentire di testare facilmente le nuove funzioni del programma alfa, abbiamo creato un nuovo account test Frame.io e lo abbiamo collegato a un nuovo gruppo chiamato `Frame.io alpha testing` nell’ambiente Workfront Preview o Sandbox esistente.

Per testare la funzionalità, accedi all’istanza Workfront Preview o Sandbox ed esegui i seguenti passaggi:

>[!NOTE]
>
><span class="preview">Testo evidenziato</span> di seguito sono riportate le funzioni non ancora implementate per il test, ma che verranno incluse in una versione successiva.
>

1. **Coordinatori:** In Workfront, crea un progetto con `Frame.io alpha testing` gruppo assegnato come gruppo di progetto.

1. **Coordinatori:** In Workfront, assegna i tuoi creativi al progetto <span class="preview">o le attività con frame abilitato (si noti che le sottoattività non possono essere contrassegnate come abilitate per frame)</span> e cambia lo stato del progetto in &quot;Corrente&quot;.

1. **Creatività:** Controlla le e-mail per un invito al progetto Frame.io appena creato

1. **Creatività:** Fai clic sul pulsante &quot;Partecipa al progetto&quot; nell’e-mail di invito per partecipare al progetto Frame.io, rivedi il documento creativo all’interno del progetto e avvia la creazione dei contenuti all’interno dello strumento Creative Cloud desiderato.

1. **Creatività:** Carica le risorse create in Frame.io e aggiungile al progetto Workfront collegato <span class="preview">(o attività assegnate abilitate per i fotogrammi).</span>

1. **Coordinatori:** In Workfront, trova le risorse Frame.io collegate nel tuo progetto e assegna revisori/approvatori (per ulteriori informazioni sull’assegnazione di revisioni/approvatori, consulta [Aggiungere altri approvatori o revisori a un documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)).

1. **Parti interessate:** In Workfront, visualizzare la richiesta di approvazione in Dettagli pagina principale o Documento, esaminare il documento Frame connected nel visualizzatore Frame.io e lasciare un commento contenente il feedback.

1. <span class="preview">**Coordinatori:** In Workfront, visualizzare i commenti creati dalle parti interessate nella sezione Aggiornamenti del documento connesso Frame.io.</span>

1. <span class="preview">**Parti interessate:** Decidere dall&#39;interno del visualizzatore Frame.io.</span>

1. <span class="preview">**Creatività:** In Frame.io, notate la decisione di approvazione complessiva presa per le vostre risorse.</span>

1. **Creatività:** All’interno di Frame.io, applica le modifiche richieste aggiungendo la versione aggiornata allo stack delle versioni della risorsa connessa.

1. **Coordinatori:** In Workfront, assegna approvatori/revisori alla versione appena caricata e monitora l’avanzamento fino al momento dell’approvazione.

## Scenario di test dettagliato

Abbiamo creato uno scenario di test più complesso per i partecipanti che desiderano testare funzionalità aggiuntive. Una guida per questo scenario di test dettagliato può essere scaricata qui: [Scenario di test dettagliato WF + Frame.io](/help/quicksilver/product-announcements/betas/assets/WF-Frame-Detailed-Test-Scenario-Walkthrough.pdf).

## Feature plan

Di seguito sono riportate informazioni sui casi d’uso principali che stiamo cercando di affrontare e sulle funzioni che abbiamo pianificato di svolgere. <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
><span class="preview">Testo evidenziato</span> di seguito si fa riferimento alle funzioni non ancora implementate, ma che verranno incluse in una versione successiva.
>
>Punti elenco sotto a **&quot;Potenziali miglioramenti nelle versioni future&quot;** l’intestazione potrebbe essere inclusa o meno in una versione futura, a seconda del feedback alfa e dei nostri piani di sviluppo in evoluzione.
>


### Gli amministratori di Workfront possono impostare una connessione tra i gruppi di Workfront e gli account Frame.io

* <span class="preview">In Workfront è possibile collegare un gruppo Workfront a un account Frame.io</span>

* All&#39;interno di Frame.io verrà creato un nuovo team Frame.io che rappresenta il gruppo Workfront connesso

**Potenziali miglioramenti nelle versioni future:**

* Disconnettere un gruppo Workfront da un account Frame.io

* Collegare un gruppo Workfront a un team Frame.io esistente

### I coordinatori dei progetti possono configurare quali progetti Workfront vengono inviati a Frame.io e far aggiungere al progetto in Frame.io le creatività assegnate in Workfront.

* Possibilità di contrassegnare i progetti Workfront come Frame.io abilitati assegnando un gruppo Frame connesso

* <span class="preview">Miglioramento: possibilità di attivare o disattivare le attività all&#39;interno dei progetti Workfront come attività Frame che, a loro volta, creeranno cartelle di attività all&#39;interno di Frame.io</span>

* Quando lo stato di un progetto Workfront è impostato su Corrente, viene creato un progetto connesso corrispondente in Frame, gli utenti assegnati a Workfront vengono aggiunti al progetto Frame e viene inviata una notifica e-mail da Frame.io

   * Tutti i membri del progetto Workfront (utenti e team) verranno aggiunti come collaboratori al progetto Frame.io (durante la creazione del progetto e in seguito)

   * <span class="preview">Modifica: utenti e team assegnati ad attività di Workfront abilitate per i frame verranno aggiunti come collaboratori al progetto Frame.io e notificati (durante la creazione del progetto e in seguito)</span>

* I documenti (Riassunti creativi) aggiunti al progetto e le attività con Frame abilitato verranno inviati al progetto Frame.io (nella rispettiva cartella di lavoro) quando il progetto viene creato (trigger: stato progetto impostato su Corrente)

   * Si consiglia di limitare la quantità di documenti aggiunti al progetto prima di diventare attivi solo nelle descrizioni creative, per evitare di inviare più documenti non necessari a Frame.io

* <span class="preview">Miglioramento: Utenti / team esplicitamente non assegnati a un&#39;attività Workfront abilitata per frame verrà rimossa dal progetto Frame.io</span>

**Potenziali miglioramenti nelle versioni future:**

* Le attività con frame abilitato possono essere configurate sui modelli di progetto

* La nuova versione caricata in specifiche creative verrà inviata al frame

* Sincronizzazione dei progetti ottimizzata (disconnessione di progetti, risincronizzazione di progetti e documenti, ecc.)

### All’interno di Frame.io, i creativi possono inviare le risorse create al progetto Workfront per una revisione formale

* Possibilità di collegare una singola risorsa Frame.io a un progetto o attività WF. Verrà creato un riferimento a una risorsa in Workfront

* La nuova versione caricata all&#39;interno di Frame.io creerà automaticamente una nuova versione del documento in Workfront sulle risorse collegate

* <span class="preview">Miglioramento: possibilità di contrassegnare le attività Workfront a cui si fa riferimento come completate dall&#39;interno di Frame.io</span>

* <span class="preview">Miglioramento: nel caso in cui il documento Workfront connesso venga eliminato, rimane all&#39;interno di Frame.io e può essere riconnesso alla stessa o ad altra attività di progetto</span>

**Potenziali miglioramenti nelle versioni future:**

* Possibilità di inviare contemporaneamente più risorse Frame.io a Workfront

* Registrazione dell&#39;ora per il progetto/attività Workfront da Frame.io

### I coordinatori dei progetti possono assegnare il processo di approvazione formale ai documenti collegati da Frame.io

* Gli utenti e i team di Workfront possono essere aggiunti alle nuove approvazioni di documenti per documenti connessi a Frame.io

* <span class="preview">Miglioramento: quando un utente/team non è più condiviso da un documento abilitato per i frame, perde anche l’accesso alla risorsa nel Visualizzatore Frame.io</span>

**Potenziali miglioramenti nelle versioni future:**

* Inviare più risorse come una singola revisione

* Assegnazione in blocco di approvatori/revisori a documenti Workfront

### Le parti interessate possono condurre la loro revisione e approvazione all&#39;interno di Frame.io Viewer

* Le parti interessate riceveranno una notifica e potranno visualizzare il documento Frame connected nel visualizzatore Frame.io

* È possibile accedere al visualizzatore Frame.io da posizioni diverse all&#39;interno di Workfront, ad esempio Elenco documenti, Dettagli documento, Home di Workfront

* Possibilità di sfruttare le funzionalità esistenti di revisione e commento fornite dal visualizzatore Frame.io che sarà sincronizzato con il flusso di aggiornamento di Workfront

* <span class="preview">Possibilità di prendere una nuova decisione di approvazione del documento dal visualizzatore Frame.io</span>

### All&#39;interno di Frame.io, i creativi verranno informati sulle decisioni generali relative alla risorsa Frame.io collegata

* <span class="preview">Miglioramento: lo stato di approvazione generale del documento verrà visualizzato sulla risorsa all&#39;interno di Frame.io</span>

### I coordinatori dei progetti possono inviare risorse finali all&#39;AEM

* <span class="preview">Miglioramento: i documenti con frame collegato, inclusi i metadati, possono essere inviati all&#39;AEM utilizzando l&#39;attuale connettore Workfront + AEM Asset CS</span>
