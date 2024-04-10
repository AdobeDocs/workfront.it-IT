---
content-type: reference
navigation-topic: betas
title: "Integrazione nativa di Adobe Workfront e Frame.io beta: funzioni"
description: Funzioni pianificate per l'integrazione nativa beta di Adobe Workfront e Frame.io
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
source-git-commit: b7a0fe333f0d8f17bc2d6c612d8cff6ee484c935
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 0%

---

# Integrazione nativa beta di Adobe Workfront e Frame.io: funzioni e test

Con questa integrazione, il nostro obiettivo è consentire ai creativi di rimanere nel loro strumento scelto (CC o Frame.io) per condurre la creazione dei contenuti e le revisioni tra pari, mentre i project manager coordinano il lavoro e inizializzano e monitorano il processo di revisione formale dall&#39;interno di Workfront. Ciò può essere ottenuto utilizzando il meglio di entrambe le soluzioni: le nuove approvazioni dei documenti di Workfront per la gestione delle approvazioni dei contenuti, insieme alle funzionalità di revisione dei contenuti offerte da Frame.io. Collettivamente, le nuove approvazioni dei documenti e Frame.io formeranno la nuova esperienza di revisione e approvazione dei contenuti end-to-end. 

Per ulteriori informazioni sul funzionamento della versione beta e sulle modalità di partecipazione, consulta [Integrazione beta di Adobe Workfront e Frame.io: panoramica](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md).

>[!NOTE]
>
>Nel caso in cui ti imbattessi in queste pagine senza che la tua azienda partecipasse a questo programma beta, assicurati di trattare le informazioni con attenzione e rivolgiti al tuo amministratore Workfront o Frame.io per ulteriori informazioni.
>

## Video dimostrativo

>[!VIDEO](https://video.tv.adobe.com/v/3426406/)

## Scenario di test di base

Per consentirti di testare facilmente le nuove funzioni del programma beta, abbiamo creato un nuovo account test Frame.io e lo abbiamo collegato a un nuovo gruppo denominato `Frame.io testing` nell’ambiente Workfront Preview o Sandbox esistente.

Per testare la funzionalità, accedi all’istanza Workfront Preview o Sandbox ed esegui i seguenti passaggi:

1. **Coordinatori:** In Workfront, crea un progetto con `Frame.io testing` gruppo assegnato come gruppo di progetto.

1. **Coordinatori:** In Workfront, contrassegna le attività che richiedono un lavoro creativo come abilitate per i fotogrammi (in dettagli attività) e assegna i tuoi creativi a esso (assegnali anche se desideri testare l’intero flusso di lavoro).

>[!NOTE]
>
>Le sottoattività non possono essere contrassegnate come abilitate per fotogrammi.
>

1. **Coordinatori:** Carica il resoconto creativo e cambia lo stato del progetto in &quot;Corrente&quot;.

1. **Creatività:** Controlla le e-mail per un invito al progetto Frame.io appena creato

1. **Creatività:** Fai clic sul pulsante &quot;Partecipa al progetto&quot; nell’e-mail di invito per partecipare al progetto Frame.io, rivedi il documento creativo all’interno del progetto e avvia la creazione dei contenuti all’interno dello strumento Creative Cloud desiderato.

1. **Creatività:** Carica le risorse create in Frame.io e aggiungetele al progetto Workfront collegato selezionando una delle attività con Frame abilitato assegnate. Selezionare l&#39;opzione per contrassegnare l&#39;attività come completata.

1. **Coordinatori:** In Workfront, individua le risorse Frame.io collegate nell’attività con frame abilitato e verifica che lo stato dell’attività sia stato modificato in &quot;completato&quot;.

1. **Coordinatori:** Assegna revisori/approvatori alla risorsa Frame.io collegata. Assegnati anche a te stesso come approvatore se desideri testare l’intero flusso di lavoro. (Per ulteriori informazioni sull&#39;assegnazione di revisioni/approvatori, vedere [Aggiungere altri approvatori o revisori a un documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)).

1. **Parti interessate:** In Workfront, puoi visualizzare la richiesta di approvazione in Home, Document Details (Dettagli documento) o nella notifica e-mail ricevuta. Apri la risorsa nel visualizzatore Frame.io, lascia un commento contenente feedback e prendi una decisione.

1. **Coordinatori:** In Workfront, visualizzare i commenti creati dalle parti interessate nella sezione Aggiornamenti del documento connesso Frame.io, nonché la decisione nella sezione Approvazione o nel riquadro di riepilogo del documento.

1. **Creatività:** In Frame.io, notate la decisione di approvazione complessiva presa per le vostre risorse.

1. **Creatività:** All’interno di Frame.io, applica le modifiche richieste aggiungendo la versione aggiornata allo stack delle versioni della risorsa connessa.

1. **Coordinatori:** In Workfront, assegna approvatori/revisori alla versione appena caricata e monitora l’avanzamento fino al momento dell’approvazione.

## Scenario di test dettagliato

Abbiamo creato uno scenario di test più complesso per i partecipanti che desiderano testare funzionalità aggiuntive. Una guida per questo scenario di test dettagliato può essere scaricata qui: [Scenario di test dettagliato WF + Frame.io](/help/quicksilver/product-announcements/betas/assets/MVP-WF-Frame-Detailed-Walk-Through.pdf).



## Feature plan

Di seguito sono riportate informazioni sui casi d’uso principali che stiamo cercando di affrontare e sulle funzioni che abbiamo pianificato di svolgere. <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
>Punti elenco sotto a **&quot;Potenziali miglioramenti nelle versioni future&quot;** l’intestazione potrebbe essere inclusa o meno in una versione futura, a seconda del feedback beta e dei nostri piani di sviluppo in evoluzione.
>

### Gli amministratori di Workfront possono impostare una connessione tra i gruppi di Workfront e gli account Frame.io

* In Workfront è possibile collegare un gruppo Workfront a un account Frame.io

* All’interno di Frame.io verrà creato un nuovo team Frame.io che rappresenterà il gruppo Workfront connesso. Questa funzione è stata abilitata solo per i clienti che utilizzano l’integrazione in produzione. I clienti ancora in fase di test su Sandbox o Anteprima avranno la connessione configurata dal team di Adobi.)

**Potenziali miglioramenti nelle versioni future:**

* Disconnettere un gruppo Workfront da un account Frame.io

* Collegare un gruppo Workfront a un team Frame.io esistente

### I coordinatori dei progetti possono configurare quali progetti Workfront vengono inviati a Frame.io e far aggiungere al progetto in Frame.io le creatività assegnate in Workfront.

* Possibilità di contrassegnare i progetti Workfront come Frame.io abilitati assegnando un gruppo Frame connesso

* Possibilità di attivare o disattivare le attività all&#39;interno dei progetti Workfront come attività Frame che a loro volta creeranno cartelle di attività all&#39;interno di Frame.io

* Dato che a un progetto Workfront è assegnato un gruppo con connessione Frame e almeno un&#39;attività con connessione Frame, quando lo stato del progetto Workfront è impostato su Corrente, viene creato un progetto con connessione corrispondente in Frame, gli utenti assegnati a Workfront vengono aggiunti al progetto Frame e viene inviata loro una notifica e-mail da Frame.io

   * Gli utenti e i team assegnati ad attività di Workfront abilitate per i frame verranno aggiunti come collaboratori al progetto Frame.io e notificati (durante la creazione del progetto e in seguito)

* I documenti (Riassunti creativi) aggiunti al progetto e le attività con Frame abilitato verranno inviati al progetto Frame.io (nella rispettiva cartella di lavoro) quando il progetto viene creato (trigger: stato progetto impostato su Corrente)

   * Si consiglia di limitare la quantità di documenti aggiunti al progetto prima di diventare attivi solo nelle descrizioni creative, per evitare di inviare più documenti non necessari a Frame.io

   * I documenti e le attività aggiunti dopo la sincronizzazione iniziale del progetto non verranno inviati a Frame.io, solo gli utenti e i team

**Potenziali miglioramenti nelle versioni future:**

* Le attività con frame abilitato possono essere configurate sui modelli di progetto

* La nuova versione caricata in specifiche creative verrà inviata al frame

* Sincronizzazione dei progetti ottimizzata (disconnessione di progetti, risincronizzazione di progetti e documenti, ecc.)

### All’interno di Frame.io, i creativi possono inviare le risorse create al progetto Workfront per una revisione formale

* Possibilità di collegare una singola risorsa Frame.io a un progetto o attività WF. Verrà creato un riferimento a una risorsa in Workfront

* La nuova versione caricata all&#39;interno di Frame.io creerà automaticamente una nuova versione del documento in Workfront sulle risorse collegate

* Possibilità di contrassegnare le attività Workfront di riferimento come completate dall&#39;interno di Frame.io

* Nel caso in cui il documento Workfront connesso venga eliminato, rimane all&#39;interno di Frame.io e può essere riconnesso alla stessa o ad altra attività di progetto

**Potenziali miglioramenti nelle versioni future:**

* Possibilità di inviare contemporaneamente più risorse Frame.io a Workfront

* Registrazione dell&#39;ora per il progetto/attività Workfront da Frame.io

### I coordinatori dei progetti possono assegnare il processo di approvazione formale ai documenti collegati da Frame.io

* Gli utenti e i team di Workfront possono essere aggiunti alle nuove approvazioni di documenti per documenti connessi a Frame.io

* Quando un utente/team non è più condiviso da un documento abilitato per Frame, perde anche l’accesso alla risorsa nel Visualizzatore Frame.io

**Potenziali miglioramenti nelle versioni future:**

* Inviare più risorse come una singola revisione

* Assegnazione in blocco di approvatori/revisori a documenti Workfront

### Le parti interessate possono condurre la loro revisione e approvazione all&#39;interno di Frame.io Viewer

* Le parti interessate riceveranno una notifica e potranno visualizzare il documento Frame connected nel visualizzatore Frame.io

* È possibile accedere al visualizzatore Frame.io da posizioni diverse all&#39;interno di Workfront, ad esempio Elenco documenti, Dettagli documento, Home di Workfront

* Possibilità di sfruttare le funzionalità esistenti di revisione e commento fornite dal visualizzatore Frame.io che sarà sincronizzato con il flusso di aggiornamento di Workfront

* Possibilità di prendere una nuova decisione di approvazione del documento dal visualizzatore Frame.io
