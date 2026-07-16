---
content-type: release-notes
title: Attività della versione del terzo trimestre 2026 per Adobe Workfront Planning
description: Questa è l’attività di rilascio per il prodotto Adobe Workfront Planning per il terzo trimestre 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: b186900d58f6a422c787cef881a4d06d6cd7feed
workflow-type: tm+mt
source-wordcount: '3111'
ht-degree: 2%

---

# Attività della versione del terzo trimestre 2026 per Adobe Workfront Planning

<!--

take the next sentence out when we start listing features

-->

<!--
There are no features released during the Third Quarter Release for 2026. When features are released for this quarter, we will document them in this article. 
-->

<!--keep the sentence below for all future quarterly release pages-->

Questo articolo descrive le funzioni rilasciate per Workfront Planning durante la versione del terzo trimestre 2026.

Per un elenco di tutte le funzionalità rilasciate per Adobe Workfront Planning, vedere [Attività di rilascio di Adobe Workfront Planning: indice articolo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).


## Nuovi campi del tipo di licenza per i livelli di accesso

>[!NOTE]
>
>Anteprima e produzione per tutti i clienti: 16 luglio 2026
>[!BADGE Fuori pianificazione]{type=Neutral}


Sono state apportate le seguenti modifiche al campo nella casella Livello di accesso:

* Il campo Tipo di licenza nella casella Livello di accesso è stato rinominato Tipo di licenza flusso di lavoro. Non vi sono modifiche di funzionalità con questa rietichettatura.

  Per informazioni, vedere [Creare e modificare livelli di accesso personalizzati](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Per i clienti che hanno acquistato anche un pacchetto Workfront Planning, è stato aggiunto un nuovo campo Tipo di licenza Planning per illustrare la licenza di un utente in Workfront Planning.
I clienti che hanno acquistato un numero uguale di licenze Workflow e Planning dispongono dei seguenti tipi di licenza disponibili:

   * Standard di pianificazione
   * Collaboratore pianificazione
   * Nessuno

>[!NOTE]
>
>È possibile assegnare agli utenti una combinazione mista di licenze tra Workflow e Planning, ma gli utenti devono disporre di una licenza Workflow a pagamento per disporre di una licenza Planning Standard.
>
>Ad esempio, non è possibile assegnare una licenza di Planning Standard a un utente di Workflow Contributor. A un utente con una licenza Workflow Light è ora possibile concedere una licenza Standard a Planning, gestendo così le aree di lavoro e il relativo contenuto. In precedenza, era possibile accedere ai dati di Planning solo in visualizzazione.
>
>I nuovi clienti possono acquistare licenze Planning e Workflow in quantità diverse e utilizzarle con qualsiasi combinazione. In questo scenario il tipo di licenza Collaboratore di Planning non è disponibile.

Per informazioni, vedere [Panoramica dell&#39;accesso ad Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

## Controllo automatico dell&#39;accesso per Workfront Planning in Snowflake

>[!IMPORTANT]
>
>Anteprima e produzione per tutti i clienti: 16 luglio 2026
>[!BADGE Fuori pianificazione]{type=Neutral}


Questa versione introduce la gestione degli accessi automatizzata e basata sui diritti per i dati di Workfront Planning in Snowflake come parte di Workfront Data Connect.

Si inizia estendendo la generazione di viste sicure alle tabelle di Planning che stabiliscono le basi necessarie per il controllo degli accessi a valle e rendendo possibili le sovvenzioni basate sui diritti.

Sulla base di questo, il provisioning dell’account di lettura ora controlla i diritti TMS al momento della creazione e applica automaticamente o trattiene le sovvenzioni al database Planning, garantendo la correttezza.

Prima di questo miglioramento, questo era disponibile solo per Workfront.

L’aggiornamento include le seguenti funzionalità:

* Un processo giornaliero automatizzato rileva le modifiche di adesione per i clienti esistenti
* I nuovi job concedono, revocano o conservano l&#39;accesso in base ai diritti
* Copertura completa del ciclo di vita per provisioning, creazione di account e modifiche continue dei diritti.

L&#39;articolo del dizionario dati [Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md) verrà aggiornato dopo la data di rilascio.


## Impostare le autorizzazioni predefinite per i record

>[!NOTE]
>
>Anteprima: 7 luglio 2026
>Versione rapida di produzione: 15 luglio 2026
>Produzione per tutti: 16 luglio 2026

I responsabili di Workspace possono ora impostare una regola di autorizzazione predefinita, aperta o limitata, per ogni tipo di record, in modo che i record appena creati vengano automaticamente protetti senza passaggi manuali.

Quando si seleziona Limitato, solo il creatore del record e tutti gli utenti, i gruppi, i team, i ruoli o le aziende specificamente selezionati possono modificare il record, mentre tutti gli altri utenti mantengono l&#39;accesso in sola visualizzazione.

Questa regola si applica automaticamente ai nuovi record, indipendentemente dalla modalità di creazione del record (pulsante Nuovo record, moduli di richiesta, API, utilizzo di un’automazione Fusion o Assistente IA). Le modifiche apportate alla regola interessano solo i record creati in futuro, mai quelli esistenti.

Una volta creato un record, le relative autorizzazioni possono ancora essere aggiornate in modo indipendente senza influire sulla regola predefinita per i record futuri.

Per informazioni, vedere [Impostare le autorizzazioni predefinite per i record](/help/quicksilver/planning/access/set-default-record-permissions.md).

## Layout di raggruppamento corsia per la visualizzazione della timeline

>[!NOTE]
>
>Anteprima: 7 luglio 2026
>Versione rapida di produzione: 15 luglio 2026
>Produzione per tutti: 16 luglio 2026

Le visualizzazioni della timeline che sono raggruppate ora supportano un layout a corsia scorrevole, con i gruppi visualizzati come colonna di intestazione sinistra bloccata invece che come bande orizzontali scorrevoli. Questo tipo di raggruppamento è aggiuntivo rispetto al raggruppamento in pila corrente.

I livelli di raggruppamento nidificati vengono visualizzati come colonne secondarie rientrate e i record all&#39;interno di ogni corsia rimangono sottoimpilati e ordinati.

È possibile trascinare i record nella visualizzazione raggruppata per aggiornare in modo ottimale le informazioni e le date.

Tutti gli utenti che visualizzano la vista possono vedere i raggruppamenti applicati.

Per informazioni, consulta [Gestire la vista timeline](/help/quicksilver/planning/views/manage-the-timeline-view.md).


## Elementi visitati di recente nella casella di ricerca globale

>[!NOTE]
>
>Anteprima e produzione per tutti i clienti: 30 giugno 2026
>[!BADGE Fuori pianificazione]{type=Neutral}

La casella di ricerca globale in Planning ora ricorda le ricerche più recenti: le ultime 7 aree di lavoro visitate, i tipi di record e le visualizzazioni vengono visualizzati in sezioni dedicate e chiaramente etichettate in modo da potervi accedere rapidamente senza dover eseguire nuovamente una query.

I risultati recenti rispettano le autorizzazioni correnti e l’elenco degli elementi più recenti è visivamente diverso dai risultati della ricerca live. Come in precedenza, è possibile accedere alla ricerca dalla pagina di destinazione di Planning o da qualsiasi pagina utilizzando una combinazione di tastiera.

Per ulteriori informazioni, vedere [Panoramica di Workspace](/help/quicksilver/planning/architecture/workspaces-overview.md).


## Supporto per i campi di pianificazione della valuta nei dashboard di Canvas

>[!NOTE]
>
>Anteprima: 25 giugno 2026
>Versione rapida di produzione: 15 luglio 2026
>Produzione per tutti: 16 luglio 2026

È ora possibile includere i campi di pianificazione della valuta nei rapporti di tabella, indicatore KPI e grafico nei dashboard di Canvas.

Prima di questo miglioramento, i campi di valuta non erano supportati nei dashboard di Canvas.

Per informazioni, vedere [Utilizzare i campi di valuta nei dashboard di Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md).

## Miglioramento dell’interfaccia per i controlli del colore delle righe

>[!NOTE]
>
>Anteprima: 22 giugno 2026
>Versione rapida di produzione: 15 luglio 2026
>Produzione per tutti: 16 luglio 2026

È stato aggiornato l&#39;aspetto del controllo Colori riga nella visualizzazione per tabella.

Per ulteriori informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).

## Aggiungere le scelte predefinite per i campi di selezione e di tipo Persone

>[!NOTE]
>
>Anteprima: 18 giugno 2026
>Versione rapida di produzione: 15 luglio 2026
>Produzione per tutti: 16 luglio 2026

Quando si crea un campo a selezione singola o multipla o un campo di tipo Persone, è ora possibile indicare un valore predefinito per questi campi. I valori predefiniti verranno sempre applicati quando il campo è visibile su un record.

È possibile modificare le impostazioni predefinite del campo dopo averlo salvato. È possibile sostituire i valori predefiniti dei campi quando si lavora con i record.

Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

## Miglioramenti dell’interfaccia nella vista a tabella

>[!NOTE]
>
>Anteprima: 11 giugno 2026
>Versione rapida di produzione: 15 luglio 2026
>Produzione per tutti: 16 luglio 2026

È stato aggiornato l&#39;aspetto della vista tabella per le seguenti aree in Workfront Planning:

* Tutte le pagine del tipo di record

* Tutte le pagine dei tipi di record collegate, ad eccezione di Progetti

Oltre ad alcune modifiche di navigazione e a miglioramenti della progettazione, questo aggiornamento include alcuni miglioramenti:

* L&#39;aggiunta di una riga di aggregazione nella parte inferiore della tabella che riepiloga i campi numero, valuta, percentuale e alcuni campi formula utilizzando i seguenti aggregatori: SUM, AVG, MAX, MIN.

* Un formato data più semplice con un numero inferiore di tipi di formato quando si aggiunge un campo Data.

* Possibilità di selezionare un fuso orario visibile a tutti gli utenti, indipendentemente dal fuso orario del loro profilo, quando si aggiunge un campo Data.

* Rimozione della numerazione delle righe per un aspetto più pulito

* Casella di selezione riga persistente, anziché visibile solo quando si passa il puntatore del mouse sulla riga

* Righe separatori di colonna persistenti per una migliore leggibilità

* Un’esperienza di ordinamento più semplice quando si effettua un ordinamento da un’intestazione di colonna

Per ulteriori informazioni, vedere [Gestire la visualizzazione della tabella](/help/quicksilver/planning/views/manage-the-table-view.md).


## È ora possibile aggiungere Marchi GenStudio for Performance Marketing ai moduli di richiesta Planning

>[!NOTE]
>
>Anteprima e produzione per tutti i clienti: 5 giugno 2026
>Disponibile solo per i clienti Adobe Workfront Planning che dispongono anche di Adobe GenStudio for Performance Marketing.
>[!BADGE Fuori pianificazione]{type=Neutral}


Per consentire l’aggiunta di brand alle campagne a partire dall’invio di una richiesta, ora puoi aggiungere il campo record Brands connected a un modulo di richiesta Planning.

Quando un tipo di record Planning è connesso al tipo di record Marchi GenStudio, è possibile aggiungere il campo Marchi connessi a un modulo di richiesta Planning associato al tipo di record Planning.

Per informazioni, vedere [Introduzione all&#39;integrazione di Adobe Workfront Planning e Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).


## Nuova scheda di esempio per le aree di lavoro aggiunta alla pagina di destinazione Planning

>[!NOTE]
>
>Anteprima: 1 giugno 2026
>Versione rapida di produzione: 11 giugno 2026
>Produzione per tutti: 16 luglio 2026


Nell’area di destinazione di Planning è stata aggiunta la scheda Aree di lavoro di esempio, in cui è possibile visualizzare un esempio di aree di lavoro basate sulle best practice. Le aree di lavoro non sono modificabili. I manager di Workspace possono modificare le viste in aree di lavoro di esempio. La scheda è visibile per gli utenti Standard e Amministratore di sistema.

È consigliabile visualizzare le aree di lavoro di esempio come esempi e utilizzare il bundle di modelli per più aree di lavoro per creare, modificare e condividere le aree di lavoro risultanti dall’utilizzo di tale modello.  Il bundle di modelli contiene le stesse aree di lavoro della scheda Aree di lavoro di esempio.

Per informazioni, vedere [Panoramica delle aree di lavoro](/help/quicksilver/planning/architecture/workspaces-overview.md).

>[!NOTE]
>
>La creazione di aree di lavoro da bundle di modelli è disponibile solo per le organizzazioni nei pacchetti Workflow Prime o Ultimate.

## Workfront Planning API versione 2

>[!NOTE]
>
>Disponibile per tutti i clienti: 28 maggio 2026
>[!BADGE Fuori pianificazione]{type=Neutral}

È ora disponibile la versione 2 dell&#39;API di pianificazione di Workfront, che estende in modo significativo le funzionalità della versione 1.

I seguenti miglioramenti sono inclusi nella versione 2:

* Crea, aggiorna ed elimina aree di lavoro, tipi di record e campi a livello di programmazione.

* Gestione completa dei record.
* Sono stati apportati miglioramenti alla struttura degli URL, alla gestione degli errori, all’impaginazione, ai filtri e alle autorizzazioni.
* Include aggiornamenti parziali tramite PATCH
* Include le operazioni di registrazione in blocco.

La versione 1 rimane disponibile, anche se si consiglia di passare all&#39;utilizzo della versione 2.

>[!NOTE]
>
>Il connettore Workfront Planning per Fusion non è stato aggiornato all’API versione 2 e continuerà a utilizzare la versione 1 fino a nuovo avviso.

Per informazioni, vedere [Nozioni di base sulle API di Adobe Workfront Planning](/help/quicksilver/planning/general/planning-api-basics.md).

Per le specifiche API di Workfront Planning, vedere la documentazione per gli sviluppatori [Workfront Planning API](https://developer.adobe.com/wf-planning/).

## Concedere autorizzazioni ai record

>[!NOTE]
>
>Anteprima: 28 maggio 2026
>Versione rapida di produzione: 11 giugno 2026
>Produzione per tutti: 16 luglio 2026


È ora possibile modificare le autorizzazioni dei singoli record per controllare chi può gestirle all’interno di un tipo di record.

Per impostazione predefinita, gli utenti ereditano le autorizzazioni dei record dall&#39;area di lavoro e dal tipo di record. È ora possibile sovrascrivere le autorizzazioni ereditate su record specifici per concedere l’accesso Visualizza o Gestisci a un sottoinsieme di utenti. Le sostituzioni delle autorizzazioni possono essere applicate a singoli record o aggiornate in blocco in più record.

<!-- 
Laurel asked for this to be replaced with the above: 

Users inherit record permissions from the workspace and record type by default. To give only select users with record type permissions Manage permissions to only certain records, you can disable inherited permissions on select records and grant only those users Manage access to those records. You can adjust permissions for one record, or for multiple records at the same time, in bulk.

You can give users the following permissions levels: 

* View 
* Manage 
-->

>[!NOTE]
>
>* Le autorizzazioni a livello di record di un utente non possono superare le autorizzazioni relative al tipo di record. Ad esempio, a un utente con accesso di visualizzazione a un tipo di record non può essere concesso l&#39;accesso di gestione a singoli record di quel tipo.
>* Al momento non è possibile rimuovere le autorizzazioni di un utente da un record. Qualsiasi utente con almeno l&#39;accesso Visualizzazione al tipo di record può visualizzare tutti i record di quel tipo.

Per informazioni, vedere [Condividi record](/help/quicksilver/planning/access/share-records.md).

## Aggiunta semplificata del tipo di record globale

>[!NOTE]
>
>Anteprima: 28 maggio 2026
>Versione rapida di produzione: 11 giugno 2026
>Produzione per tutti: 16 luglio 2026

Per ridurre i clic e trovare rapidamente i tipi di record necessari, è stata migliorata l&#39;esperienza per l&#39;aggiunta di record in modo da renderla più rapida e intuitiva quando si aggiungono tipi di record globali a un&#39;altra area di lavoro.

Quando si sceglie di aggiungere un record da tipi di record esistenti, viene immediatamente visualizzato un elenco di tutti i tipi di record globali disponibili.

È possibile selezionare e aggiungere contemporaneamente uno o più tipi di record globali direttamente da questa schermata.

Per informazioni, vedere [Aggiungere tipi di record esistenti da un&#39;altra area di lavoro](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

## Planning Designer è ora disponibile in Beta per tutti i clienti Workfront Planning

>[!NOTE]
>
>Anteprima: 28 maggio 2026
>Versione rapida di produzione: 11 giugno 2026
>Produzione per tutti: 16 luglio 2026
>[!BADGE In Beta]{type=Neutral}

Ora puoi utilizzare Adobe Planning Designer basato sull’intelligenza artificiale per configurare facilmente le aree di lavoro e le strutture di dati. Il Designer di Planning supporta tutte le operazioni, dalla creazione e configurazione delle aree di lavoro alla definizione di campi e formule, alla gestione dei record, alla revisione della cronologia delle modifiche e alla creazione di viste personalizzate.

Sia che venga utilizzato direttamente o tramite l&#39;Assistente di intelligenza artificiale, Planning Designer offre un ambiente flessibile e potente per la creazione e la manutenzione di informazioni strutturate e connesse.

Un amministratore di Workfront può gestire la disponibilità di Planning Designer dall&#39;area Preferenze di sistema in Configurazione.

Per informazioni, vedere [Introduzione ad Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).


## Sincronizzare i metadati da Planning a AEM Assets

>[!NOTE]
>
>Anteprima e produzione per tutti: 28 maggio 2026
>Disponibile solo per i clienti Adobe Workfront Planning che dispongono anche di Adobe GenStudio for Performance Marketing e Adobe Experience Manager.
>[!BADGE Fuori pianificazione]{type=Neutral}

Per migliorare l’integrità dei dati, è stata rilasciata una sincronizzazione perfetta dei metadati tra i tipi di record di GenStudio for Performance Marketing e AEM Assets quando AEM Assets è collegato ai tipi di record di GenStudio in Workfront Planning.

È possibile collegare ad AEM Assets i seguenti tipi di record di GenStudio for Performance Marketing: Campaign, Product, Persona, Region e Channel.

Le informazioni aggiunte a un tipo di record GenStudio in Workfront Planning vengono visualizzate in una scheda Campaign separata di una risorsa AEM in AEM. Le informazioni su Prodotto, Persona, Area geografica e Canale per tale campagna vengono visualizzate anche in tale scheda, in modalità di sola lettura.

Con questa versione, i metadati chiave sono coerenti tra le due piattaforme e riflettono gli aggiornamenti quasi in tempo reale, riducendo la riconciliazione manuale.

Per informazioni, vedere [Gestire l&#39;area di lavoro di GenStudio in Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).

## Sincronizzare i metadati da Planning a frammenti di contenuto AEM

>[!NOTE]
>
>Anteprima e produzione per tutti: 28 maggio 2026
>Disponibile solo per i clienti Adobe Workfront Planning che dispongono anche di Adobe GenStudio for Performance Marketing e Adobe Experience Manager.
>[!BADGE Fuori pianificazione]{type=Neutral}

Per migliorare l’integrità dei dati, è stata rilasciata una sincronizzazione perfetta dei metadati tra i tipi di record di Planning nell’area di lavoro GenStudio e i frammenti di contenuto di AEM quando questi sono collegati alle campagne GenStudio for Performance Marketing.

Le informazioni sulla campagna GenStudio ora vengono visualizzate nella scheda Metadati di un frammento di contenuto in AEM.  Le informazioni su Prodotto, Persona, Area geografica e Canale per tale campagna vengono visualizzate anche in tale scheda, in modalità di sola lettura.

Con questa versione, i metadati chiave sono coerenti tra le due piattaforme e riflettono gli aggiornamenti quasi in tempo reale, riducendo la riconciliazione manuale.

Per informazioni, vedere [Gestire l&#39;area di lavoro di GenStudio in Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).


## Aggiornamenti della vista a elenco

>[!NOTE]
>
>Anteprima: 27 maggio 2026
>Versione rapida di produzione: 11 giugno 2026
>Produzione per tutti: 16 luglio 2026

Sono stati aggiornati diversi tipi di campo nella vista a elenco per includere la navigazione da tastiera e altri miglioramenti.

I campi Selezione multipla, Selezione singola e Assegnatario ora offrono la navigazione da tastiera nella vista a elenco:

* Utilizza le frecce su e giù sulla tastiera per spostarti nell’elenco delle persone.

* Premere la barra spaziatrice per selezionare una persona o per rimuoverla.

Nei campi a selezione singola e multipla nella vista a elenco:

* Se non viene trovato alcun risultato, puoi aggiungere nuove opzioni direttamente dall’editor. Questa funzione potrebbe non essere disponibile in tutti gli elenchi.

* L’interazione con i campi ora è accessibile da tastiera. Ciò include la navigazione tra i tag, le opzioni di ricerca e l’elenco utilizzando le frecce su e giù. Premere la barra spaziatrice per selezionare o rimuovere un elemento selezionato.

Alcuni miglioramenti all’interfaccia sono stati apportati ai campi di riferimento, come i campi typeahead e i campi di ricerca esterni.

Inoltre, laddove disponibile, l’esperienza di trascinamento e rilascio di colonne è stata migliorata visivamente.

Per ulteriori informazioni, vedere [Gestire la visualizzazione elenco in Adobe Workfront Planning](/help/quicksilver/planning/views/manage-the-list-view.md).

## I campi di riferimento di Workfront sono abilitati come campi di ricerca per le connessioni Planning

>[!NOTE]
>
>Anteprima: 27 maggio 2026
>Versione rapida di produzione: 11 giugno 2026\
>Produzione per tutti: 16 luglio 2026

È ora possibile aggiungere campi di riferimento Workfront come campi di ricerca quando si collega un tipo di record Planning a un tipo di oggetto Workfront.

È ad esempio possibile aggiungere le informazioni relative a Portfolio, Programma, Gruppo o Società dall&#39;oggetto Progetto a un campo di connessione di progetto di una campagna in Planning.

Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).

## Nuovi filtri per la funzione di suddivisione della vista timeline

>[!NOTE]
>
>Anteprima: 27 maggio 2026
>Versione rapida di produzione: 11 giugno 2026
>Produzione per tutti: 16 luglio 2026

È ora possibile filtrare le informazioni nella vista timeline in base a criteri che corrispondono agli oggetti inclusi nella suddivisione dei record.

Prima di questo miglioramento, era possibile applicare filtri solo per i record principali nella vista timeline.

Per informazioni, consulta [Gestire la vista timeline](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Nuova indicazione che i campi modificati ed eliminati influiscono sui moduli di richiesta

>[!NOTE]
>
>Anteprima: 27 maggio 2026
>Versione rapida di produzione: 11 giugno 2026
>Produzione per tutti: 16 luglio 2026

È stato aggiunto un promemoria per ricordarti che i campi record modificati o eliminati potrebbero influire sui moduli di richiesta che li contengono. Ora potrai rivedere i moduli interessati e assicurarti che le modifiche che desideri apportare ai campi non influiscano sulle informazioni esistenti.

Per informazioni, vedere [Modifica impostazioni campo](/help/quicksilver/planning/fields/edit-fields.md).

## Modifica richieste Planning inviate

>[!NOTE]
>
>Anteprima: 27 maggio 2026
>Versione rapida di produzione: 11 giugno 2026
>Produzione per tutti: 16 luglio 2026

È ora possibile modificare le richieste di Planning dopo averle inviate, prima di creare un record dalla richiesta.

I seguenti utenti possono modificare una richiesta inviata:

* Il creatore della richiesta
* Manager Workspace per l’area di lavoro in cui è stata inviata la richiesta
* Amministratori di sistema

Prima di questo miglioramento, non era possibile modificare le richieste inviate.

Per ulteriori informazioni, vedere [Inviare le richieste di Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md).

## Nuova finestra di anteprima per frammenti di contenuto AEM

>[!NOTE]
>
>Anteprima e produzione per tutti i clienti: 14 maggio 2026
>[!BADGE Fuori pianificazione]{type=Neutral}

Per una migliore visibilità durante l’utilizzo dei frammenti di contenuto di AEM connessi ai record di Workfront Planning, è stata aggiunta una finestra di anteprima che visualizza informazioni sui frammenti in Workfront Planning.

Questa funzionalità era precedentemente disponibile per le risorse AEM e ora è stata aggiunta ai frammenti di contenuto.

Per informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

## I campi di ricerca sono ora disponibili per i frammenti di contenuto di AEM in Workfront Planning

>[!NOTE]
>
>Anteprima e produzione per tutti i clienti: 14 maggio 2026
>Disponibile solo per i clienti Adobe Workfront Planning che dispongono anche di Adobe Experience Manager.
>[!BADGE Fuori pianificazione]{type=Neutral}

Ora è possibile aggiungere i seguenti campi di ricerca quando si collega un tipo di record Planning a un frammento di contenuto di AEM:

* Creato da
* Data creazione
* Modificato da
* Modificato

Prima di questo miglioramento, i campi di ricerca erano disponibili solo per le risorse e le cartelle di AEM.

Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).



## Visualizzazioni personalizzate per la pagina Dettagli di un record

>[!NOTE]
>
>Anteprima: 14 maggio 2026
>Versione rapida di produzione: 11 giugno 2026
>Produzione per tutti: 16 luglio 2026

Per consentire una migliore flessibilità nella visualizzazione delle informazioni nella pagina dei dettagli di un record, è stata introdotta la possibilità di creare visualizzazioni personalizzate per questa pagina.

Oltre ad aggiungere due visualizzazioni di pagina dei dettagli già create che contengono tutti i campi dei record o solo i campi visibili nella visualizzazione tabella, è ora possibile creare visualizzazioni personalizzate per le pagine dei dettagli di un record. Le visualizzazioni create sono visibili a tutti coloro che possono accedere al record.

Questo aggiornamento rimuove l&#39;impostazione **Mostra tutti i campi** e la sostituisce con le visualizzazioni dei dettagli personalizzate.

Per informazioni, vedere [Gestire la pagina record](/help/quicksilver/planning/records/manage-the-record-page.md).

## Aggiungere raggruppamenti a una pagina record Progetti connessi

>[!NOTE]
>
>Anteprima: 14 maggio 2026\
>Velocità di produzione: 11 giugno 2026
>Produzione per tutti: 16 luglio 2026

È ora possibile raggruppare le informazioni nella pagina dei record connessi ai progetti di un record in Workfront Planning. Questa funzionalità non esisteva in quest’area prima di questo miglioramento.

Per informazioni, vedere [Gestire la visualizzazione elenco](/help/quicksilver/planning/views/manage-the-list-view.md).

