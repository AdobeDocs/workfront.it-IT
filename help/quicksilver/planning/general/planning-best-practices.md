---
title: Best practice per la pianificazione Adobe Workfront
description: In qualità di responsabile delle operazioni di marketing, puoi utilizzare Adobe Workfront Planning per organizzare il lavoro nel ciclo di vita di marketing per tutti i team. Di seguito sono riportate alcune best practice consigliate all'avvio di Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6e039b80-e3bf-412c-8c86-8f801f5861e3
source-git-commit: 1926500c76e4f9cfdac829f8d9f0cdfa6231e31d
workflow-type: tm+mt
source-wordcount: '3304'
ht-degree: 0%

---

<!--drafted because Kari Woolf will write something for Field Readiness instead, nothing for ExL, public-facing documentation-->

# Best practice di Adobe Workfront Planning

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

In qualità di responsabile delle operazioni di marketing, puoi utilizzare Adobe Workfront Planning per organizzare il lavoro nel ciclo di vita di marketing per tutti i team.

Questo articolo illustra alcune domande frequenti e best practice consigliate all&#39;avvio di Workfront Planning.

## Best practice di configurazione

### Aree di lavoro

Le aree di lavoro sono posizioni centralizzate in cui i team possono pianificare il lavoro. Un&#39;area di lavoro è una raccolta di tipi di record utilizzati da un team e rappresenta il ciclo di vita del lavoro del team.

Di seguito sono riportate alcune domande frequenti sulla configurazione di Workfront Planning.

#### Come dovrei iniziare?

* ✅ Quando accedi a Planning per la prima volta, segui il nostro processo di onboarding in-app che comunica chiaramente il valore di Planning e ti guida su come navigare e utilizzare il prodotto in modo efficace. In questo modo potrai comprenderne le funzionalità e iniziare facilmente il tuo lavoro.
* ✅ Per iniziare, esplora i nostri modelli di area di lavoro predefiniti per idee su casi d&#39;uso simili esistenti. È possibile utilizzare i tipi di record e i campi predefiniti inclusi in un modello oppure aggiungere record personalizzati.
* ✅ Identificare i principali casi d&#39;uso che si desidera risolvere con Workfront Planning. Ad esempio, la maggior parte delle organizzazioni desidera migliorare la visibilità delle attività strategiche, che può includere la creazione di un &quot;Calendario delle campagne&quot; migliore. Pertanto, per quel caso d’uso, vorresti iniziare rispondendo ad alcune domande:

   * Chi lo sta chiedendo?
   * Come chiamano le cose che vogliono mettere nel calendario?
Campagne? Tattiche? Iniziative? Attività? Eventi?
   * A quali domande si desidera rispondere con questo calendario?
   * Esistono campagne sovrapposte per lo stesso pubblico?
   * Qual è il budget per tale campagna, tattica, attività o evento?

  Le risposte a queste domande determinano ciò che è necessario creare all&#39;interno di Workfront Planning.

  Inoltre, considera che ci potrebbero essere altri planner che al momento non sono utenti di Workfront. Questi planner possono funzionare al di fuori dei fogli di calcolo Excel, documenti Word, PowerPoint, ecc. Esaminare la modalità di accesso alle informazioni in Workfront Planning.

* ✅ Per sfruttare appieno Workfront Planning, è consigliabile sostituire l&#39;utilizzo di portafogli e programmi in Workfront Workflow con altre strutture di livello superiore in Workfront Planning.

  Oggi, i clienti Workfront rappresentano il loro lavoro strategico attraverso portfolio e programmi, in alcuni casi come progetti di diverso tipo. Con l&#39;introduzione di Planning, tutto questo lavoro strategico deve essere gestito attraverso tipi di record personalizzati in Workfront Planning, mentre Workfront sarà centrato intorno alla fase di esecuzione del lavoro rappresentato come progetti e attività.


#### Quando è necessario creare una nuova area di lavoro anziché modificarne una esistente?

* ✅ Progettazione per il volume più basso di aree di lavoro a livello di organizzazione. È possibile creare aree di lavoro per unità organizzative specifiche, in base al funzionamento di ciascuna unità.

  Disporre delle informazioni in un unico Workspace, per garantire che le relazioni tra tutti i dati possano essere gestite facilmente.

  Ad esempio, prova a creare un’unica area di lavoro per tutto il reparto Marketing.

  È possibile creare una nuova area di lavoro per un team con una struttura operativa completamente diversa:

  Ad esempio, un&#39;area di lavoro **Sviluppo prodotto** deve essere distinta da un&#39;area di lavoro **Marketing**.

* ⛔ Non creare aree di lavoro univoche per ogni team o processo di un&#39;organizzazione.

  L’organizzazione Marketing deve impegnarsi a mantenere un’unica area di lavoro per mantenere la visibilità e consentire il rollup dei dati a livello di pianificazione globale.

  Evita di creare aree di lavoro simili o duplicate per i team che seguono processi simili (ad esempio, EMEA Marketing e APAC Marketing), soprattutto quando questi team possono svolgere un lavoro che sale fino alle campagne strategiche comuni.

#### Come si utilizzano le sezioni di Workspace?

* ✅ Creare ed etichettare le sezioni per aiutare gli utenti a comprendere come organizzare il ciclo di vita operativo.

  Ad esempio, puoi creare una sezione denominata **Record core** in cui inserire le campagne, le tattiche e i risultati finali nell&#39;area di lavoro.
* ✅ Raggruppa i tipi di record &quot;like&quot;.

  Ad esempio, puoi creare una sezione denominata **Geografie** che contiene tipi di record quali: Regione, Paese e Città.

### Tipi di record

I tipi di record sono i blocchi predefiniti di Workfront Planning Workspace. È possibile definire l&#39;interconnessione dei tipi di record.


#### Come definire i tipi di record nella mia area di lavoro?

* ✅ Identificare le informazioni da tenere traccia (i tipi di record necessari) e il modo in cui tali informazioni devono essere connesse. Parla con le parti interessate che utilizzeranno l’area di lavoro per prendere in considerazione tutte le loro esigenze. È inoltre possibile creare sezioni personalizzate con diversi tipi di record per presentare le informazioni in modo molto fruibile.


* ⛔ Non duplicare i tipi di record per un periodo diverso, ad esempio non creare tipi di record separati per **Campagne 2024** e **Campagne 2025**.

  La creazione di tipi di record diversi interrompe il flusso di dati ogni volta che si desidera confrontare i dati in più anni. Le visualizzazioni odierne sono per tipo di record, quindi non appena l&#39;anno termina, la visualizzazione di quel tipo di record non mostrerà più gli elementi futuri. La best practice prevede di avere un tipo di record per il tipo di lavoro e segmentare i dati utilizzando filtri o archiviandoli, se necessario.

#### Quando utilizzare un campo a selezione singola o multipla rispetto a un tipo di record collegato?

* ✅ Aggiungere un nuovo tipo di record se l&#39;oggetto verrà utilizzato in connessione con più altri tipi di record

  Ad esempio, una campagna può avere una connessione a più tipi di pubblico Target e una tattica può avere una connessione a un singolo pubblico Target. Pertanto, Campaign, Tactic e Audience devono essere tipi di record anziché campi a selezione multipla.

* ✅ Aggiungere un nuovo tipo di record se l&#39;oggetto deve memorizzare valori di metadati aggiuntivi che potrebbero essere utili nelle ricerche

  Ad esempio, un tipo di record di canale come **E-mail** può memorizzare un elenco di risultati finali di supporto come metadati nativi o come connessione a un tipo di record **Risultati finali** autonomo.
* ⛔ Non aggiungere un nuovo tipo di record se i dati memorizzati sono rilevanti solo per un singolo tipo di record.

  Ad esempio, un tipo di record **Campaign** può avere un campo a selezione singola denominato **Dimensione campagna** che è rilevante solo quando è direttamente associato a una campagna specifica.

#### Come etichettare i tipi di record?

* ✅ Creare ed etichettare i tipi di record che rappresentano un singolo costrutto o sostantivo, ad esempio **Campagne**.
* ⛔ Non creare un tipo di record meglio rappresentato come visualizzazione.

  Ad esempio, **Calendario** è una scelta errata per un tipo di record, perché non è il tipo di record stesso, ma una visualizzazione di record.

### Gestione dei campi

I campi sono attributi dei tipi di record e vengono visualizzati come colonne nella visualizzazione tabella. È possibile creare campi personalizzati per i tipi di record e quindi associarli ai record di Workfront Planning per migliorare le informazioni sui record.


#### Quale campo si consiglia di definire come Campo primario?


* ✅ Utilizzare valori di campo primari univoci per semplificare la ricerca e la selezione di tali record durante l&#39;esecuzione delle connessioni. 

  Quando si effettua una connessione, gli utenti eseguiranno la ricerca in base ai valori del campo Principale e, se non sono univoci, non sapranno quale scegliere. 
* ⛔ Evitare di utilizzare valori non univoci come campo principale, in quanto possono creare confusione per gli utenti che devono eseguire ricerche nel campo principale quando si utilizza il menu del selettore delle connessioni. 

#### Come si utilizzano le formule?

* ✅ Utilizzare i tipi di campo Formula per ridurre l&#39;input manuale. Quando si immettono informazioni in base a dati già presenti nella vista tabella, è possibile calcolare tali informazioni automaticamente utilizzando le formule.

#### Come iniziare a collegare i dati nella mia area di lavoro?

* ✅ La creazione di connessioni è una delle funzionalità più potenti di Workfront Planning. È possibile connettere tipi di record tra loro o tipi di record con tipi di oggetti di altre applicazioni come Adobe Workfront (connessione a progetti, portafogli, programmi, società e gruppi) e con Adobe Experience Manager Assets (connessione a risorse e cartelle).

  Il collegamento di oggetti e tipi di record offre una panoramica completa delle modalità di connessione di tutti gli elementi dell&#39;azienda.

  Ad esempio, si dispone di un tipo di record **Campaign** e di un tipo di record **Tactics** ed è possibile creare una connessione tra questi due tipi di record per vedere quali **Tactics** sono associate a una **Campaign** specifica.

  Dopo aver definito la connessione, tutte le persone nell&#39;area di lavoro possono iniziare ad aggiungere valori per **Campagne** facendo doppio clic nel campo della connessione in cui visualizzeranno un elenco di tutte le **Tattiche** disponibili. Ciò ti consente di trovare rapidamente quali tattiche devono essere associate alle campagne.

#### Come si utilizzano i campi di ricerca?

* ✅ Dopo aver stabilito la connessione tra i record o i tipi di oggetto, è possibile connettere tra loro singoli record e visualizzare i campi del record o dei tipi di oggetto collegati in un record di Workfront Planning. Riduci il numero di posizioni in cui devi aggiornare la stessa informazione e assicurati che corrispondano perfettamente.

  Ad esempio, una volta stabilita una connessione tra un tipo di record **Campaign** e un tipo di record **Tactics**, verranno visualizzate le informazioni del campo principale, ma quando si aggiungono campi di ricerca, sarà possibile inserire ulteriori informazioni da tale tipo di record, come la **Data lancio** per tale **Tactic**. I dati per questi campi di ricerca vengono compilati automaticamente dopo l’aggiunta dei record.

#### Quale tipo di campo è consigliato per gli URL? 

* ✅ Utilizzare un campo di testo a riga singola per aggiungere dati URL a un record.

### Viste

#### Come è possibile decidere cosa deve essere una visualizzazione rispetto a un tipo di record?

* ✅Per gli elementi che rappresentano un singolo costrutto o sostantivo (ad esempio **Campagne**), creare un tipo di record. 

* ⛔ Non creare un tipo di record meglio rappresentato come visualizzazione.

  Ad esempio, **Calendario** è una scelta errata per un tipo di record, perché non è il tipo di record stesso, ma una visualizzazione di record. 

#### È necessario nascondere o eliminare i campi non rilevanti?

* ✅ Nascondere la colonna invece di eliminarla quando queste informazioni potrebbero essere rilevanti per un&#39;altra persona che utilizza lo stesso tipo di record. Se si elimina il campo in una visualizzazione tabella specifica, questo campo verrà eliminato anche nelle altre visualizzazioni del record e in qualsiasi altro punto da cui il tipo di record è collegato.

#### Come si utilizzano i filtri e i raggruppamenti nelle viste tabella e timeline?

* ✅ Utilizzare le visualizzazioni con filtri e raggruppamenti per visualizzare un&#39;istantanea di ciò che è necessario visualizzare. Puoi filtrare e raggruppare i dati in modo da avere un modo più fruibile di capire cosa è pianificato. È possibile raggruppare i record per campi di metadati.

  Ad esempio, puoi avere una visualizzazione della timeline per il tipo di record **Campaign** che puoi raggruppare per **Tipi di pubblico di destinazione** e filtrare per **Data** in modo da mostrare solo l&#39;anno corrente.

#### Perché non vengono visualizzati tutti i record nella visualizzazione della sequenza temporale?

* ✅ Ricorda di definire 2 campi data per i tuoi record. È possibile creare una visualizzazione timeline solo se a un tipo di record sono associati almeno due campi data. Alcuni record potrebbero non essere visualizzati nella visualizzazione della sequenza temporale se le date di inizio e di fine o entrambe non contengono valori e se la data di inizio è successiva alla data di fine.

#### Come si utilizzano le impostazioni della vista timeline

* ✅ Definisci le impostazioni della visualizzazione timeline, come lo stile **Barre** e il **Colore** per ottenere una visualizzazione più ricca dal punto di vista visivo. Puoi personalizzare lo stile **Barra** definendo se desideri visualizzare una miniatura con un&#39;immagine significativa e aggiungere altri campi da visualizzare sulla barra (ad esempio, **Proprietario** o **Stato**).

  Per impostazione predefinita, viene visualizzato solo il campo principale. È inoltre possibile definire il colore della barra in base ai valori dei campi (ad esempio, è possibile personalizzare i colori delle barre confrontandole con il campo Stato) o in base al raggruppamento applicato. Per impostazione predefinita, il colore corrisponde al colore del tipo di record.

  Solo i colori del tipo di record o i campi con opzioni associate ai colori possono influire sui colori delle barre dei record nella timeline.

### Autorizzazioni e condivisione

Utilizzare la funzione di condivisione per assegnare le autorizzazioni appropriate ai dipendenti per le visualizzazioni e le aree di lavoro.

#### Come posso gestire le autorizzazioni per le aree di lavoro?

* ✅ Quando crei un&#39;**area di lavoro**, è disponibile solo per te. Chiunque, a parte gli amministratori di sistema, non sarà in grado di trovarlo. Una volta definita l’area di lavoro e quando sei pronto a coinvolgere il team per avviare la collaborazione, devi condividerla con loro e definirne il livello di autorizzazione.

  Puoi scegliere tra i seguenti livelli di autorizzazione:

   * **Gestisci**: gli utenti possono modificare, eliminare e condividere l&#39;area di lavoro.
   * **Contribute**: gli utenti possono creare, modificare ed eliminare record.
   * **Visualizza**: gli utenti possono visualizzare i record.

* ✅ Anche se molti clienti ritengono che concederebbero le autorizzazioni **Gestisci** alle aree di lavoro alla maggior parte delle persone, limita le autorizzazioni **Gestisci** a un gruppo selezionato di persone attendibili che non elimineranno accidentalmente un tipo di record o creeranno in altro modo tipi di record e campi non necessari. Possono modificare, condividere e persino eliminare l’area di lavoro. Questo livello di autorizzazioni garantisce loro l’accesso amministrativo completo a Workspace.

  È necessaria una licenza utente Standard affinché un utente disponga delle autorizzazioni di gestione per un&#39;area di lavoro.

* ✅ Concedere agli utenti le autorizzazioni **Contribute** se si desidera che possano semplicemente creare, modificare ed eliminare record, ma non modificare la struttura e lo schema dell&#39;area di lavoro. Con le autorizzazioni di **Contribute**, non è possibile creare tipi di record o modificare i campi dei tipi di record esistenti.

  È necessaria una licenza utente Standard affinché un utente disponga di **autorizzazioni Contribute** per un&#39;area di lavoro.

* ✅ Concedi agli utenti le autorizzazioni **Visualizza**, se desideri che visualizzino solo i record.

  >[!NOTE]
  >
  >Al momento non disponiamo di autorizzazioni specifiche per i tipi di record o i record, pertanto tutti i record in uno qualsiasi dei tipi di record sono visibili se si concede a un utente l&#39;accesso **Visualizzazione** all&#39;area di lavoro.


#### Come posso gestire le autorizzazioni per i tipi di record?

* ✅ Ricorda che gli utenti con le autorizzazioni di gestione per le aree di lavoro non possono avere le autorizzazioni ridotte per il tipo di record. Erediteranno inoltre le autorizzazioni Manage per il tipo di record. Non è possibile assegnare a un utente le autorizzazioni di gestione per l&#39;area di lavoro, ma le autorizzazioni di Contribute o di visualizzazione per il tipo di record.
* ✅ Se si desidera che gli utenti dispongano di un livello di autorizzazione inferiore (ad esempio le autorizzazioni di visualizzazione) per il tipo di record rispetto a quello dell&#39;area di lavoro, è consigliabile assegnare loro le autorizzazioni Contribute per l&#39;area di lavoro. È quindi possibile assegnare loro le autorizzazioni di visualizzazione per il tipo di record.
* La rimozione di un utente dalle autorizzazioni del tipo di record conferisce comunque a tale utente almeno le autorizzazioni di visualizzazione per l&#39;area di lavoro.

#### Come posso gestire le autorizzazioni per le visualizzazioni?

* ✅ Limitare le autorizzazioni **Gestione** alle persone che si desidera possano modificare, eliminare e condividere la visualizzazione. Ciò significa che possono modificare i filtri, i campi di raggruppamento o alcune configurazioni della vista. Tali modifiche avranno effetto sulla configurazione principale della vista per tutti gli altri utenti che la utilizzano.

  È necessaria una licenza utente Standard affinché un utente disponga delle autorizzazioni di gestione per una visualizzazione.

* ✅ Concedi agli utenti l&#39;accesso **View** per applicare la visualizzazione. Potranno modificare alcuni dei filtri o dei raggruppamenti e l’ordinamento, ma le modifiche saranno solo temporanee; le modifiche non vengono salvate per tutti gli altri utenti che accedono alla visualizzazione. Tali modifiche non influiranno sulla configurazione principale della vista per tutti gli altri utenti che la utilizzano.  Le modifiche apportate sono visibili solo all&#39;utente che le applica. Dopo aver aggiornato la schermata, le modifiche vengono reimpostate sul valore predefinito.

* ✅ Assegna a **Tutti gli utenti dell&#39;area di lavoro possono visualizzare** le autorizzazioni quando desideri che tutti gli utenti che possono visualizzare l&#39;area di lavoro visualizzino i record e i relativi campi in quella visualizzazione specifica. In questo modo, non è necessario aggiungere manualmente alcun utente alla casella delle autorizzazioni di condivisione per la visualizzazione.

  >[!NOTE]
  >
  >Se una visualizzazione non è stata condivisa e si condivide un collegamento con altre persone, queste potranno visualizzare i record nella **Visualizzazione tabella predefinita**. Se dispongono di una licenza Workfront standard, possono creare la propria visualizzazione.


#### In che modo **Condivisione Workspace** è diverso da **Condivisione visualizzazione**?

* **Condivisione Workspace** definisce l&#39;accesso delle persone all&#39;area di lavoro, i relativi tipi di record, i record e i relativi campi.

* **Condivisione visualizzazione** definisce se l&#39;utente può visualizzare la visualizzazione creata e se può modificare il filtro, i campi di raggruppamento o un&#39;altra configurazione della visualizzazione. La visibilità dei record visualizzati nella visualizzazione è controllata dalla condivisione di Workspace e non dalla condivisione di visualizzazione.

#### In che modo i tipi di licenza di Workfront influiscono sulle autorizzazioni di Workfront Planning?

* Per **condivisione Workspace**: gli utenti con licenza Light e Contribute possono accedere solo alla visualizzazione di un&#39;area di lavoro. Per concedere a un utente l&#39;autorizzazione Contribuisci o Gestisci per un&#39;area di lavoro, è necessario disporre di una licenza Standard.

* **Visualizzazioni condivise**: gli utenti con licenza Standard che dispongono di autorizzazioni Gestione per un&#39;area di lavoro potranno creare una visualizzazione. Gli utenti con licenza Light e Contribute possono utilizzare solo le visualizzazioni create e condivise dagli utenti Standard. In caso contrario, se non è stato condiviso nulla, gli utenti potranno visualizzare la **Visualizzazione tabella predefinita**.


#### Cosa devo fare quando un proprietario di Workspace cambia?

* Workfront imposta il creatore dell’area di lavoro come proprietario, ma dal punto di vista delle funzionalità dispone delle stesse autorizzazioni di qualsiasi utente con autorizzazioni di gestione.
* Se il proprietario è disattivato, gli altri membri possono continuare il loro lavoro nell&#39;area di lavoro senza interruzioni.
* Gli amministratori di sistema hanno accesso a qualsiasi area di lavoro, pertanto se il proprietario è l&#39;unica persona con autorizzazioni Gestione, gli amministratori possono aggiungere un&#39;altra persona e concedere loro le autorizzazioni Gestione per gestire la gestione dell&#39;area di lavoro.

### Invio di richieste in Workfront Planning

È possibile creare un modulo di richiesta per ogni tipo di record quando si desidera che gli utenti aggiungano record all&#39;esterno della pagina di un tipo di record. L&#39;invio della maschera aggiunge un nuovo record al tipo di record.

#### Quando devo iniziare a creare un modulo di richiesta per un tipo di record?

* ✅ Assicurarsi che la struttura del tipo di record sia impostata prima aggiungendo i campi necessari alla tabella. Questi campi descrivono i record e saranno accessibili nel generatore di moduli.

  È consigliabile creare la richiesta o il modulo di assegnazione dopo aver finalizzato la struttura del tipo di record per evitare di perdere campi chiave.

#### Chi può creare i moduli di richiesta?

* ✅ Qualsiasi utente con accesso Gestisci all&#39;area di lavoro può creare o modificare un modulo di richiesta. Assicurati che le autorizzazioni dell’utente siano correttamente assegnate per consentire questa funzionalità.

#### Come creare o modificare un modulo di richiesta per un tipo di record?

* ✅ Qualsiasi utente con accesso di gestione all&#39;area di lavoro può seguire i passaggi descritti nell&#39;articolo [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).


#### Chi sarà in grado di inviare nuovi record utilizzando il modulo di richiesta?

* ✅ Le autorizzazioni di invio dipendono dalle impostazioni configurate per ciascun modulo.

  Nel generatore di moduli, dopo aver pubblicato il modulo, puoi gestire le autorizzazioni per controllare chi può inviare le richieste.

  È possibile scegliere tra le tre opzioni di condivisione seguenti:

   * **Tutti gli utenti con accesso di visualizzazione o superiore all&#39;area di lavoro:** Consente a tutti gli utenti con autorizzazioni di visualizzazione o superiori all&#39;area di lavoro di inviare una richiesta che crea un record.
   * **Qualsiasi utente con accesso di tipo Contribute o di livello superiore all&#39;area di lavoro**: limita gli invii agli utenti con autorizzazioni Contribute o di livello superiore all&#39;area di lavoro.
   * **Chiunque disponga del collegamento:** Consente a chiunque disponga del collegamento al modulo di inviare una richiesta.
   * **Data di scadenza:** Assicurarsi di impostare una data di scadenza per il collegamento pubblico per migliorare la sicurezza.

### Best practice per la gestione dei moduli di richiesta

Di seguito sono riportati alcuni consigli per la gestione dei moduli di richiesta:

* Pianifica in anticipo: definisci chiaramente quali informazioni sono necessarie o richieste ai richiedenti prima di creare il modulo per evitare revisioni eccessive in un secondo momento.
* Utilizza etichette chiare: assicurati che le etichette e le descrizioni dei campi siano chiare e comprensibili per tutti gli utenti.
* Test dei moduli: prima di distribuirne di nuovi a un pubblico più ampio, esegui il test utilizzando l’opzione Collegamento modulo e Anteprima modulo per garantire che tutti i campi e la logica funzionino come previsto.
* Mantieni moduli aggiornati: rivedi periodicamente i moduli e aggiornali per riflettere eventuali modifiche nella struttura del tipo di record o nei processi operativi.

<!-- this is hidden, per Andrea:  

2.2 Migration  

Migrating your data from external <span style="text-decoration:underline;">s~~S~~</span>ystems to Workfront Planning unlocks new ways to create important connections in your workflow and uncover insights that you might not have been able to identify with your previous tools. 

By having all your data in one central location, you can more easily form connections between your Workfront data than if they all existed in separate tools. 

We have some options that will help you to accelerate the migration process:  

* **Fusion** – You can create a Scenario in Fusion that runs after certain criteria and connects objects. 
* **Bulk Data Operations** _through the new functionality -[ [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE)  (Q3 2024)_ -  
* **Copy and paste – **You can copy and paste directly from a spreadsheet. This is best suited to a simple table of data from tools like Excel or Google Sheets.  
* **Upload a C<span style="text-decoration:underline;">SV~~VS~~</span> or Excel **- The CSV (comma-separated values) format or Excel is one of the most common ways to move data between applications, and tools. This functionality is not available yet, but we are planning to work on it in Q4 2024.  

-->

<!--
     

1. Data Flow  

Currently the metadata modelling in Workfront Planning is done by Ops Admins through adding various data points to the record type from the table view, including: 



* Fields added directly on the current record type 
* Connections with custom defined operational and taxonomical record types 
* Connections with execution work captured in Workfront 
* Connections with deliverables stored as assets in AEM 
* Any lookup fields captured in any of the above connections. 

Here is a summary of how you can define the data flow within Workfront Planning and other applications.  


     



* **Connections and Lookup fields. **Creating **connections** is one of the most powerful features of Workfront Planning. You can connect record types to one another or record types with object types from other applications like Adobe Workfront (connection to Project, Portfolios, Programs, Companies, and Groups) or Adobe Experience Manager Assets (connection to assets and folders).  Connections give you a full overview of how everything in your company is connected.  

    - e.g.: You have a Campaign record type, and a Tactics record type, then you can create a connection between these two record types to see to see which Tactics are associated to a specific Campaign. After defining the connection, all the people in the workspace can start adding values by double-clicking into the connection field that displays the tactic where they will see a list of all the Tactics available and you can quickly select the tactics to be associated with each campaign. 


    After you establish the connection between records or object types, you can connect individual records to one another, and display fields from the linked record or object types on a Workfront Planning record. The connected fields are called **Lookup fields**. You will reduce the number of places you have to update the same piece of information and ensure that they match perfectly.  


    - e.g.: Once you have a connection between a Campaign record type and a Tactics record type, you will see the primary field information when you add the tactic, but when you add lookup fields, you will be able to bring additional information from the tactic, like the Launch date for that Tactic. The data for these lookup fields is auto populated. Find more information in the Adobe Experience League documentation in the article about Connecting records.  


     

* **Planning (or Connections) tab** **in Workfront _-[ [E] Global Connect capability in Planning connections area](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6617d7760001e250f5ffb9ebf04baacc/overview?source-id=unifiedShareMFE)_** 

    When you go to the Planning section of Adobe Workfront objects, you can display both connections with linked records or any available connections with Planning record types. With that, you can view and edit any connection field without having to navigate away from the current section in Workfront to other areas. The Planning section is available for the following Workfront objects: Project, Portfolio and Program. For more information, see [Manage records in the Planning section of Adobe Workfront objects](https://experienceleague.adobe.com/it/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/manage-records-in-planning-section).   


* Create new records within the connection fields - In-context creation of connected records https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6656c1a30026b903c6edf0210b8cbb23/overview?source-id=unifiedShareMFE  When you need to link records through a connection field but cannot find the required records in the connected record type, you can also create new records in the connected record type directly within the connection fields, with that you can efficiently establish necessary links without having to leave the current record type context. For more information, see Create records https://experienceleague.adobe.com/it/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/create-records.   

     

* **Field on Customer Form** (CF)[ - [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE) _(Planned completion date Sep 15, 2024 10:00 PM)._ Considering that the Workfront Project metadata modeling is done through forms, you are also able to add Planning connections to your custom forms. You can embed any lookup field value from the connected Planning record types within the custom form of your Workfront object. With that capability, when you are managing objects in Workfront, you can present any taxonomies or operational records connected to the Workfront object in custom forms, alongside other details, so that your teams can easily consume and update all the relevant information through a unified interface.  They should not need to navigate to different areas to view and update the information relevant for their work.  

     

* **Connection between Workspaces with Record types accessible from multiple workspaces** – ~~Epic – "[Connect to record types across workspaces](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/64dfad3100027190324dcc35b2176e76/overview?source-id=unifiedShareMFE)"~~ When you are creating a workspace in Planning, you can define certain record types once and then configure them to be accessible from multiple workspaces so you can create connections with them from anywhere. This way, you can streamline the data management process, eliminate duplicative work, and ensure data consistency across teams. As a result, your teams can tag their records with common taxonomies and unlock better visualization, filtering, grouping, and reporting of cross-team work.  For more information, see [Edit record types](https://experienceleague.adobe.com/it/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/edit-record-types). 

     

* **Fusion connector – You can create a connection to your Workfront Planning account from inside a Workfront Fusion module. **With this connector, you can trigger a scenario when events occur in Workfront Planning. You can also create, read, update, and delete records, or perform a custom API call to your Adobe Workfront Planning account. More information in Experience League in[ Adobe Workfront Planning modules](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-moduleshttps:/experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-modules) article.  

-->
