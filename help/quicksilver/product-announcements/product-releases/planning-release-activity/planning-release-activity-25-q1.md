---
content-type: release-notes
title: Attività sulla versione 25.1 di Adobe Workfront Planning
description: Questa è l’attività di rilascio del prodotto Adobe Workfront Planning per il primo trimestre 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: ef0b719c-6d2e-4d3e-9522-da6dbd71c248
source-git-commit: a6104204cae2a2d8fb021da254437008d55a43b6
workflow-type: tm+mt
source-wordcount: '2112'
ht-degree: 0%

---

# Attività della versione del primo trimestre 2025 per Adobe Workfront Planning

Questo articolo descrive le funzioni rilasciate per Workfront Planning durante la versione del primo trimestre 2025.

<!--keep the sentence below for all future quarterly release pages-->

Per un elenco di tutte le funzionalità rilasciate per Adobe Workfront Planning, vedere [Attività di rilascio di Adobe Workfront Planning: indice articolo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## I campi di connessione con le risorse Adobe Experience Manager ora sono supportati nei moduli di richiesta

>[!NOTE]
>
>Versione di anteprima: 20 dicembre 2024; versione di produzione per tutti i clienti: 16 gennaio 2025

È ora possibile aggiungere campi di connessione con risorse AEM a un modulo di richiesta di tipo record in Workfront Planning.

Prima di questo miglioramento, non era possibile aggiungere questi tipi di campi ai moduli di richiesta.

Per informazioni, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Configurare le approvazioni per le richieste di Workfront Planning

>[!NOTE]
>
>Versione di anteprima: 16 dicembre 2024; versione di produzione per tutti i clienti: 16 gennaio 2025

È ora possibile associare un&#39;approvazione a un modulo di richiesta di Workfront Planning. Puoi aggiungere solo utenti come approvatori di una richiesta. Dopo l’invio, la richiesta viene inviata a tutti gli approvatori per approvarla prima di creare un record.

Per informazioni, vedere [Aggiungere un&#39;approvazione a un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/add-approval-to-request-form.md).


## Notifiche per l’invio di richieste, approvazioni e modifiche di stato

>[!NOTE]
>
>Versione di anteprima: 16 dicembre 2024; versione di produzione per tutti i clienti: 16 gennaio 2025

Dopo l’invio di una richiesta in Workfront Planning, ora riceverai una notifica in-app e una notifica e-mail per le seguenti azioni:

* Un richiedente riceve una notifica che indica che una richiesta è stata inviata correttamente

* Un richiedente riceve una notifica di approvazione o rifiuto di una richiesta

* Un approvatore riceve una notifica di invio di una richiesta per l&#39;approvazione.

>[!NOTE]
>
>Per consentire agli utenti di ricevere notifiche e-mail e in-app, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.

Per informazioni sull’invio o l’approvazione delle richieste, consulta i seguenti articoli:

* [Inviare richieste di Adobe Workfront Planning per creare record](/help/quicksilver/planning/requests/submit-requests.md)

* [Approva una richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md).

## Ricerca intelligente durante la ricerca di un tipo di campo

>[!NOTE]
>
>Versione di anteprima: 5 dicembre 2024; versione di produzione per tutti i clienti: 5 dicembre 2024

È stata aggiunta la funzionalità di ricerca intelligente quando si cerca un tipo di campo in Workfront Planning. È ora possibile trovare i tipi di campo durante la digitazione di una parola chiave. Ad esempio, digitando &quot;Prezzo&quot; vengono trovati i tipi di campi Numero e Valuta. Prima di questo miglioramento, era possibile cercare solo il nome del tipo di campo effettivo.

Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

## Selettore colore personalizzato per le opzioni codificate per colore dei campi a selezione singola o multipla

>[!NOTE]
>
>Versione di anteprima: 5 dicembre 2024; produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

Ora è possibile effettuare scelte personalizzate dei colori durante la creazione o la modifica di un campo a selezione singola o multipla. Quando si creano o si modificano campi con opzioni codificate con colori, facendo clic sull&#39;icona del colore viene visualizzata una casella di selezione dei colori. È possibile scegliere tra colori predefiniti o crearne di personalizzati utilizzando codici esadecimali o uno spettro di colori.

Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

## Importare i campi Workfront esistenti nei tipi di record di Workfront Planning

>[!NOTE]
>
>Versione di anteprima: 27 novembre 2024; produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

Ora, quando si aggiungono campi a un tipo di record, è possibile importare campi personalizzati o nativi di Workfront esistenti e associarli al tipo di record selezionato. L&#39;importazione di campi esistenti crea una copia dei campi di Workfront in Workfront Planning. I campi copiati sono indipendenti dalle versioni originali.

Prima di questo miglioramento, era necessario creare manualmente tutti i campi e associarli ai tipi di record.

I campi calcolati non sono al momento supportati.

Per informazioni, vedere [Importa campi da Adobe Workfront](/help/quicksilver/planning/fields/import-fields-from-workfront.md)

## Creare tipi di record, record e campi importando un file CSV o Excel

>[!NOTE]
>
>Versione di anteprima: 27 novembre 2024; produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

È ora possibile importare nuovi tipi di record importando un file CSV o Excel.

Vengono importate le seguenti informazioni:

* Il nome del foglio o del file viene importato come nome del tipo di record.

* La prima riga di ogni colonna viene importata come nuovo campo. È possibile avere fino a 500 campi in ogni foglio importato.

* Ogni riga viene importata come nuovo record. È possibile avere fino a 10.000 record in ogni foglio.

Per ulteriori informazioni, vedere [Creare tipi di record](/help/quicksilver/planning/architecture/create-record-types.md).

## Evitare riferimenti circolari nelle formule

>[!NOTE]
>
>Versione di anteprima: 27 novembre 2024; produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

È stato introdotto un messaggio di avviso durante la modifica o la creazione di un campo formula che potrebbe creare un riferimento circolare a se stesso o a campi condivisi. Non è possibile salvare un campo formula che fa riferimento a se stesso o a elementi a cui viene fatto riferimento nel calcolo.

Per informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

## Aggiungere pagine della visualizzazione Connessione alla pagina di un record per visualizzare i record connessi in una visualizzazione tabella

>[!NOTE]
>
>Versione di anteprima: 27 novembre 2024; produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

È possibile aggiungere pagine all&#39;area dei dettagli di un record per visualizzare i record connessi in una visualizzazione per tabella. È possibile aggiungere una pagina per ogni record connesso.

Le pagine aggiunte sono di sola lettura.

Per informazioni, vedere [Gestire il layout della pagina record](/help/quicksilver/planning/records/manage-the-record-page.md).

## Nuove schede Workfront e Planning nella sezione Inviato dell&#39;area Richieste

>[!NOTE]
>
>Versione di anteprima: 27 novembre 2024; produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

Le richieste di Workfront Planning sono ora disponibili nella sezione Inviato dell&#39;area Richieste di Workfront. Nella sezione Inviata sono ora visualizzate le seguenti schede:

* Workfront: visualizza le richieste inviate in Workfront.
* Planning: visualizza le richieste sottomesse utilizzando un modulo di richiesta Workfront Planning.

Per poter aggiungere richieste a un tipo di record di Workfront Planning, è necessario utilizzare un collegamento al modulo di richiesta. L&#39;invio di una richiesta di Workfront Planning dall&#39;area Richieste di Workfront sarà disponibile in un secondo momento.

L&#39;organizzazione deve acquistare un pacchetto di Workfront Planning prima che la scheda Pianificazione sia disponibile nell&#39;area Richieste.

Per informazioni, vedere [Inviare le richieste di Adobe Workfront Planning per la creazione di record](/help/quicksilver/planning/requests/submit-requests.md).

## Nei moduli di richiesta sono ora supportati tipi di campo aggiuntivi

>[!NOTE]
>
>Versione di anteprima: 27 novembre 2024; produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

È ora possibile aggiungere i seguenti tipi di campo a un modulo di richiesta di tipo di record in Workfront Planning:

* Persone
* Connessioni Workfront

Prima di questo miglioramento, non era possibile aggiungere questi tipi di campi ai moduli di richiesta in Workfront Planning.

Per informazioni, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Limita la condivisione pubblica dei moduli di richiesta che contengono determinati tipi di campi

>[!NOTE]
>
>Versione di anteprima: 27 novembre 2024; produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

Non è più possibile condividere un modulo di richiesta pubblicamente se il modulo contiene uno dei tipi di campo seguenti:

* Formula
* Connessioni Workfront e AEM Assets
* Campi di ricerca
* Persone

Per informazioni, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).


## Visualizza i record nella vista calendario per settimana

>[!NOTE]
>
>Versione di anteprima: 26 novembre 2024; produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

È ora possibile visualizzare i record nella vista calendario per settimana. Prima di questo miglioramento, era possibile visualizzare la vista calendario solo per mese.

Per informazioni, vedere [Gestire la visualizzazione del calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md).

## Ripristina record eliminati

>[!NOTE]
>
>Versione di anteprima: 22 novembre 2024; Produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024); Produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

Una volta eliminati, i record vengono temporaneamente spostati in un raccoglitore Eliminato di recente per 30 giorni. È possibile accedere al contenitore eliminato di recente dalla pagina del tipo di record e contiene solo record di un tipo specifico.

I responsabili di Workspace possono ripristinare i record dal cestino per un massimo di 30 giorni dopo l&#39;eliminazione. Vengono ripristinati anche i record collegati e le relative informazioni di campo.

Prima di questo miglioramento, non era possibile ripristinare i record eliminati.

Per ulteriori informazioni, vedere [Ripristinare i record eliminati](/help/quicksilver/planning/records/records-information.md).

## Assistente AI di Adobe disponibile nelle aree dei dettagli del record

>[!NOTE]
>
>Versione di anteprima: 21 novembre 2024; produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

Per semplificare l&#39;esecuzione del lavoro, abbiamo aggiunto l&#39;Assistente AI di Adobe alla pagina di anteprima dei dettagli o alla pagina del record. È possibile utilizzare l&#39;Assistente AI all&#39;interno di una pagina di record per aggiornare le informazioni sul record.

Per informazioni, vedere [Panoramica dell&#39;Assistente di Adobe Workfront Planning AI](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

## Nuova esperienza durante l’aggiunta di una miniatura e di una copertina a una pagina di record

>[!NOTE]
>
>Versione di anteprima: 20 novembre 2024; produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

Quando si apre l&#39;anteprima o la pagina di un record e il record non contiene una miniatura o un&#39;immagine di copertina, è necessario passare il puntatore sull&#39;area sopra il nome del record nell&#39;intestazione per visualizzare le opzioni per aggiungere una copertina e un&#39;immagine di miniatura al record. Prima di questo miglioramento, le immagini segnaposto vuote per la miniatura e la copertina mostrate sopra il nome del record.

Per ulteriori informazioni, consulta i seguenti articoli:

* [Aggiungere una copertina a un record](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
* [Aggiungere una miniatura a un record](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

## Nuovi tipi di visualizzazione per i campi di tipo percentuale nella visualizzazione Tabella

>[!NOTE]
>
>Versione di anteprima: 7 novembre 2024; produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

Per semplificare la lettura dei numeri nella visualizzazione Tabella, è ora possibile scegliere tra le seguenti opzioni per modificare la modalità di visualizzazione di un campo di tipo Percentuale nella visualizzazione Tabella:

* Numero
* Barra
* Cerchio

Questo tipo di visualizzazione è supportato solo nella vista tabella.

Prima di questo miglioramento, era possibile visualizzare i valori percentuali solo come numeri.

Per ulteriori informazioni, vedere [Creare i campi](/help/quicksilver/planning/fields/create-fields.md).

## I campi di connessione sono ora supportati nei moduli di richiesta

>[!NOTE]
>
>Versione di anteprima: 31 ottobre 2024; produzione per rilascio rapido: con la versione 24.11 (14 novembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

È ora possibile aggiungere campi collegati per i record di Workfront Planning a un modulo di richiesta di tipo record.

Non è possibile aggiungere campi di ricerca connessione o campi connessi per oggetti Workfront nel modulo di richiesta.

Prima di questo miglioramento, non era possibile aggiungere questi tipi di campi ai moduli di richiesta in Workfront Planning.

Per informazioni, vedere [Creare e gestire un modulo di richiesta in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Avviso di connessione durante la connessione di record già collegati ad altri record

>[!NOTE]
>
>Versione di anteprima: 31 ottobre 2024; produzione per rilascio rapido: con la versione 24.11 (14 novembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

Quando si tenta di connettere record già connessi altrove e appartenenti a un tipo di record connesso tramite un tipo di connessione Uno a molti o Uno a uno, viene visualizzato un messaggio di avviso che indica che i record sono già connessi. Se si conferma che si desidera procedere con la connessione, i record selezionati vengono rimossi dal record originale e aggiunti al record che si sta modificando.

Per informazioni sui tipi di connessione, vedere [Panoramica sui tipi di record connessi](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Icona delle nuove informazioni con la descrizione dei campi nella pagina dei dettagli del record

>[!NOTE]
>
>Versione di anteprima: 30 ottobre 2024; produzione per rilascio rapido: con la versione 24.11 (14 novembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

È stata aggiunta un&#39;icona di informazioni a destra dei nomi dei campi in una pagina record. Facendo clic sull’icona delle informazioni viene visualizzata la descrizione del campo, quando esiste già una descrizione. Prima di questo miglioramento, la descrizione del campo visualizzata quando passi il cursore sul nome del campo.

Per informazioni, vedere [Modifica record](/help/quicksilver/planning/records/edit-records.md).

## Nuovo tipo di campo Workfront per le connessioni Planning

>[!NOTE]
>
>Versione di anteprima: 24 ottobre 2024; produzione per rilascio rapido: con la versione 24.11 (14 novembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (gennaio 2025)

Per continuare a collegare gli oggetti di Workfront ai record di Workfront Planning, è stato aggiunto un nuovo tipo di campo nei moduli personalizzati di Workfront denominato Connessione Planning. Aggiungendo questo tipo di campo a un modulo personalizzato di Workfront e, in ultima analisi, a un oggetto Workfront, è possibile effettuare le seguenti operazioni:

* Visualizza i record connessi a un oggetto Workfront nel modulo personalizzato.

* Connettere e disconnettere i record di Workfront Planning da un oggetto Workfront.

È possibile aggiungere il nuovo campo ai moduli per tutti i tipi di oggetto. È tuttavia possibile modificare le informazioni nel campo solo dai moduli allegati ai seguenti oggetti di Workfront che possono essere connessi dai tipi di record di Workfront Planning: Portfolio, Programma, Progetto, Società, Gruppo.

La modifica in blocco dei campi di connessione di Planning per gli oggetti Workfront non è ancora disponibile.

Per informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[Visualizza una dimostrazione video di questa funzionalità](https://video.tv.adobe.com/v/3435633/){target=_blank}
