---
content-type: release-notes
title: Attività della versione del terzo trimestre 2026 per Adobe Workfront Planning
description: Questa è l’attività di rilascio per il prodotto Adobe Workfront Planning per il terzo trimestre 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: ab1ac1363d6531352e905536218618196651c3b9
workflow-type: tm+mt
source-wordcount: '1448'
ht-degree: 1%

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



<!--

## Planning Designer now available in Beta for all Workfront Planning customers

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 
>[!BADGE In Beta]{type=Neutral}

You can now use the Adobe Planning Designer powered by AI to configure your workspaces and data structures with ease. The Planning Designer supports everything from creating and configuring workspaces to defining fields and formulas, managing records, reviewing change history and building custom views.  

Whether used directly or through the AI Assistant, the Planning Designer provides a flexible, powerful environment for building and maintaining structured, connected information. 

A Workfront administrator can manage the availability of the Planning Designer from the System Preferences area in Setup.   

For information, see [Get started with the Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).

## New Sample workspaces tab added to the Planning landing page

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

We have added the Sample workspaces tab in the Planning landing area where you can view example of best-practice workspaces. The workspaces are not editable and we recommend that you use them as examples to create your own.  

We also recommend that you use the multi-workspace template to create, and edit and share workspaces that result as a use of that template.  The template contains the same workspaces as the Sample workspaces tab.   

Workspace managers can modify views in sample workspaces.     

For information, see Workspaces overview (/help/quicksilver/planning/architecture/workspaces-overview.md). 

-->

## Workfront Planning API versione 2

>[!NOTE]
>
>Disponibile per tutti i clienti: 28 maggio 2026>[!BADGE Sconto pianificato]{type=Neutral}

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
>Anteprima: 28 maggio 2026>Rilascio rapido produzione: 11 giugno 2026>Produzione per tutti: 16 luglio 2026

È ora possibile modificare le autorizzazioni dei singoli record per controllare chi può gestirle all’interno di un tipo di record.

Per impostazione predefinita, gli utenti ereditano le autorizzazioni dei record dall’area di lavoro e dal tipo di record. Per assegnare solo a determinati record determinati utenti con autorizzazioni di tipo record le autorizzazioni di gestione, è possibile disabilitare le autorizzazioni ereditate per determinati record e concedere solo a tali utenti l&#39;accesso di gestione a tali record. È possibile modificare in blocco le autorizzazioni per un record o per più record contemporaneamente.

Puoi assegnare agli utenti i seguenti livelli di autorizzazione:

* Visualizzazione
* Gestione

>[!NOTE]
>
>* Le autorizzazioni a livello di record di un utente non possono superare le autorizzazioni relative al tipo di record. Ad esempio, a un utente con accesso di visualizzazione a un tipo di record non può essere concesso l&#39;accesso di gestione a singoli record di quel tipo.
>* Al momento non è possibile rimuovere le autorizzazioni di un utente da un record. Qualsiasi utente con almeno l&#39;accesso Visualizzazione al tipo di record può visualizzare tutti i record di quel tipo.

Per informazioni, vedere [Condividi record](/help/quicksilver/planning/access/share-records.md).

## Aggiunta semplificata del tipo di record globale

>[!NOTE]
>
>Anteprima: 28 maggio 2026>Rilascio rapido produzione: 11 giugno 2026>Produzione per tutti: 16 luglio 2026

Per ridurre i clic e trovare rapidamente i tipi di record necessari, è stata migliorata l&#39;esperienza per l&#39;aggiunta di record in modo da renderla più rapida e intuitiva quando si aggiungono tipi di record globali a un&#39;altra area di lavoro.

Quando si sceglie di aggiungere un record da tipi di record esistenti, viene immediatamente visualizzato un elenco di tutti i tipi di record globali disponibili.

È possibile selezionare e aggiungere contemporaneamente uno o più tipi di record globali direttamente da questa schermata.

Per informazioni, vedere [Aggiungere tipi di record esistenti da un&#39;altra area di lavoro](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).


## Sincronizzare i metadati da Planning a AEM Assets

>[!NOTE]
>
>Anteprima: 28 maggio 2026>Rilascio rapido produzione: 28 maggio 2026>Produzione per tutti: 28 maggio 2026>[!BADGE Pianificazione off]{type=Neutral}

Per migliorare l’integrità dei dati, è stata rilasciata una sincronizzazione perfetta dei metadati tra i tipi di record di GenStudio for Performance Marketing e AEM Assets quando AEM Assets è collegato ai tipi di record di GenStudio in Workfront Planning.

È possibile collegare ad AEM Assets i seguenti tipi di record di GenStudio for Performance Marketing: Campaign, Product, Persona, Region e Channel.

Le informazioni aggiunte a un tipo di record GenStudio in Workfront Planning vengono visualizzate in una scheda Campaign separata di una risorsa AEM in AEM. Le informazioni su Prodotto, Persona, Area geografica e Canale per tale campagna vengono visualizzate anche in tale scheda, in modalità di sola lettura.

Con questa versione, i metadati chiave sono coerenti tra le due piattaforme e riflettono gli aggiornamenti quasi in tempo reale, riducendo la riconciliazione manuale.

Per informazioni, vedere [Gestire l&#39;area di lavoro di GenStudio in Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).

## Sincronizzare i metadati da Planning a frammenti di contenuto AEM

>[!NOTE]
>
>Anteprima: 28 maggio 2026>Rilascio rapido produzione: 28 maggio 2026>Produzione per tutti: 28 maggio 2026>[!BADGE Pianificazione off]{type=Neutral}

Per migliorare l’integrità dei dati, è stata rilasciata una sincronizzazione perfetta dei metadati tra i tipi di record di Planning nell’area di lavoro GenStudio e i frammenti di contenuto di AEM quando questi sono collegati alle campagne GenStudio for Performance Marketing.

Le informazioni sulla campagna GenStudio ora vengono visualizzate nella scheda Metadati di un frammento di contenuto in AEM.  Le informazioni su Prodotto, Persona, Area geografica e Canale per tale campagna vengono visualizzate anche in tale scheda, in modalità di sola lettura.

Con questa versione, i metadati chiave sono coerenti tra le due piattaforme e riflettono gli aggiornamenti quasi in tempo reale, riducendo la riconciliazione manuale.

Per informazioni, vedere [Gestire l&#39;area di lavoro di GenStudio in Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).


## Aggiornamenti della vista a elenco

>[!NOTE]
>
>Anteprima: 27 maggio 2026>Rilascio rapido produzione: 11 giugno 2026>Produzione per tutti: 16 luglio 2026

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
>Anteprima: 27 maggio 2026>Versione rapida di produzione: 11 giugno 2026\
>Produzione per tutti: 16 luglio 2026

È ora possibile aggiungere campi di riferimento Workfront come campi di ricerca quando si collega un tipo di record Planning a un tipo di oggetto Workfront.

È ad esempio possibile aggiungere le informazioni relative a Portfolio, Programma, Gruppo o Società dall&#39;oggetto Progetto a un campo di connessione di progetto di una campagna in Planning.

Per informazioni, vedere [Tipi di record di connessione](/help/quicksilver/planning/architecture/connect-record-types.md).

## Nuovi filtri per la funzione di suddivisione della vista timeline

>[!NOTE]
>
>Anteprima: 27 maggio 2026>Rilascio rapido produzione: 11 giugno 2026>Produzione per tutti: 16 luglio 2026

È ora possibile filtrare le informazioni nella vista timeline in base a criteri che corrispondono agli oggetti inclusi nella suddivisione dei record.

Prima di questo miglioramento, era possibile applicare filtri solo per i record principali nella vista timeline.

Per informazioni, consulta [Gestire la vista timeline](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Nuova indicazione che i campi modificati ed eliminati influiscono sui moduli di richiesta

>[!NOTE]
>
>Anteprima: 27 maggio 2026>Rilascio rapido produzione: 11 giugno 2026>Produzione per tutti: 16 luglio 2026

È stato aggiunto un promemoria per ricordarti che i campi record modificati o eliminati potrebbero influire sui moduli di richiesta che li contengono. Ora potrai rivedere i moduli interessati e assicurarti che le modifiche che desideri apportare ai campi non influiscano sulle informazioni esistenti.

Per informazioni, vedere [Modifica impostazioni campo](/help/quicksilver/planning/fields/edit-fields.md).

## Modifica richieste Planning inviate

>[!NOTE]
>
>Anteprima: 27 maggio 2026>Rilascio rapido produzione: 11 giugno 2026>Produzione per tutti: 16 luglio 2026

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
>Anteprima: 14 maggio 2026>Rilascio rapido produzione: 14 maggio 2026>Produzione per tutti: 14 maggio 2026>[!BADGE Pianificazione off]{type=Neutral}

Per una migliore visibilità durante l’utilizzo dei frammenti di contenuto di AEM connessi ai record di Workfront Planning, è stata aggiunta una finestra di anteprima che visualizza informazioni sui frammenti in Workfront Planning.

Questa funzionalità era precedentemente disponibile per le risorse AEM e ora è stata aggiunta ai frammenti di contenuto.

Per informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

## I campi di ricerca sono ora disponibili per i frammenti di contenuto di AEM in Workfront Planning

>[!NOTE]
>
>Anteprima: 14 maggio 2026>Rilascio rapido produzione: 14 maggio 2026>Produzione per tutti: 14 maggio 2026>[!BADGE Pianificazione off]{type=Neutral}

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
>Anteprima: 14 maggio 2026>Rilascio rapido produzione: 11 giugno 2026>Produzione per tutti: 16 luglio 2026

Per consentire una migliore flessibilità nella visualizzazione delle informazioni nella pagina dei dettagli di un record, è stata introdotta la possibilità di creare visualizzazioni personalizzate per questa pagina.

Oltre ad aggiungere due visualizzazioni di pagina dei dettagli già create che contengono tutti i campi dei record o solo i campi visibili nella visualizzazione tabella, è ora possibile creare visualizzazioni personalizzate per le pagine dei dettagli di un record. Le visualizzazioni create sono visibili a tutti coloro che possono accedere al record.

Questo aggiornamento rimuove l&#39;impostazione **Mostra tutti i campi** e la sostituisce con le visualizzazioni dei dettagli personalizzate.

Per informazioni, vedere [Gestire la pagina record](/help/quicksilver/planning/records/manage-the-record-page.md).

## Aggiungere raggruppamenti a una pagina record Progetti connessi

>[!NOTE]
>
>Anteprima: 14 maggio 2026\
>Velocità di produzione: 11 giugno 2026>Produzione per tutti: 16 luglio 2026

È ora possibile raggruppare le informazioni nella pagina dei record connessi ai progetti di un record in Workfront Planning. Questa funzionalità non esisteva in quest’area prima di questo miglioramento.

Per informazioni, vedere [Gestire la visualizzazione elenco](/help/quicksilver/planning/views/manage-the-list-view.md).
