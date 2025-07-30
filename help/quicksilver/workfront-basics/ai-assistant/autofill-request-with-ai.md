---
title: Compilazione automatica di una richiesta tramite IA
content-type: reference
description: Puoi utilizzare l’intelligenza artificiale per compilare automaticamente i campi della richiesta.
author: Becky
feature: Get Started with Workfront
exl-id: d053e604-5a28-4fd3-8f89-4467b6e46f02
source-git-commit: d890d467dfdade676a5c93f061a5cbeda53556b6
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 1%

---

# Compilazione automatica di una richiesta tramite IA

>[!NOTE]
>
>Questa funzionalità fa attualmente parte di una versione beta chiusa. Per abilitare questa funzionalità, contattare `sargism@adobe.com`.
>
>Per qualificarsi per la versione beta chiusa, l’organizzazione deve soddisfare i requisiti per utilizzare l’Assistente di intelligenza artificiale di Workfront. Per informazioni dettagliate, vedere [Prerequisiti per l&#39;Assistente IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

L’intelligenza artificiale può aiutarti a compilare automaticamente i campi della richiesta. Può suggerire valori di campo in base a richieste precedenti, o analizzarli da testo come e-mail o documenti caricati.

Puoi approvare o rifiutare questi suggerimenti prima di inviare la richiesta.

La funzione di riempimento automatico non sovrascrive i campi già compilati.

Gli utenti non ricevono suggerimenti di dati a cui non hanno altrimenti accesso.

## Ottieni suggerimenti durante la compilazione del modulo

La compilazione automatica può suggerire i valori dei campi durante la compilazione del modulo. Quando si immettono valori nei campi della richiesta, Workfront li confronta con le richieste precedenti. Se il valore immesso è strettamente correlato con altri valori di campo in contesti simili in richieste precedenti, Workfront consiglia tali valori.

Ad esempio, se una clinica utilizza sempre lo stesso codice di fatturazione, Workfront suggerisce che il codice di fatturazione venga inserito nel campo appropriato quando viene inserito il nome della clinica.

Per utilizzare i suggerimenti basati sulle richieste precedenti:

1. Inizia a creare una richiesta.

   Per istruzioni, vedere [Creare e inviare richieste](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Inizia a compilare i campi.

   Durante la compilazione dei campi, è possibile che in altri campi vengano visualizzati suggerimenti.

1. Per ogni suggerimento di campo, selezionare **Accetta** o **Rifiuta** sotto il campo.

   Oppure

   Selezionare **Accetta tutti** o **Rifiuta tutti** nella parte superiore della pagina per accettare o rifiutare tutti i suggerimenti.

## Ottieni suggerimenti da un prompt di testo

La funzione di riempimento automatico può suggerire i valori dei campi in base al testo, ad esempio le e-mail. Si incolla in un blocco di testo e Workfront elabora il testo per suggerire i valori dei campi in base al testo.

Ad esempio, se l’e-mail include &quot;Scadenza 1 giugno&quot; e il modulo di richiesta ha un campo per la data di scadenza, Workfront consiglia 1 giugno per tale valore di campo.

Questo tipo di suggerimento controlla anche le richieste precedenti per contesti simili. Ad esempio, se il prompt indica che la richiesta è per un determinato client, Workfront può individuare e immettere automaticamente l’indirizzo di fatturazione per tale client, in base alle richieste precedenti.

È possibile incollare il testo da applicare all&#39;intero modulo o a una singola sezione del modulo.

Per utilizzare i suggerimenti basati su un prompt di testo incollato:

1. Inizia a creare una richiesta.

   Per istruzioni, vedere [Creare e inviare richieste](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Per applicare il prompt di testo all&#39;intero modulo, fare clic sull&#39;icona IA ![Icona IA](assets/request-prompt-icon.png) sotto il nome del modulo.

   Oppure

   Per applicare il prompt di testo per una singola sezione, fai clic sull&#39;icona IA ![icona IA](assets/request-prompt-icon.png) accanto al nome della sezione.

1. Incollare il testo nella casella del prompt.
1. Fai clic su **Compila il modulo**.

   Workfront genera suggerimenti per il modulo.
1. Per ogni suggerimento di campo, selezionare **Accetta** o **Rifiuta** sotto il campo.

   Oppure

   Selezionare **Accetta tutti** o **Rifiuta tutti** nella parte superiore della pagina per accettare o rifiutare tutti i suggerimenti.

## Ottieni suggerimenti in base a un documento caricato

La funzione di riempimento automatico può suggerire i valori dei campi in base a un documento caricato.

Questo tipo di suggerimento controlla anche le richieste precedenti per contesti simili. Ad esempio, se il prompt indica che la richiesta è per un determinato client, Workfront può individuare e immettere automaticamente l’indirizzo di fatturazione per tale client, in base alle richieste precedenti.

### Guardrail di caricamento documenti

#### Tipi di file supportati

Sono supportati i seguenti tipi di file:

* BMP
* CSV
* DOC
* DOCX
* GIF
* JPEG
* JPG
* ODP
* ODS
* ODT
* PDF
* PNG
* PPT
* PPTX
* RTF
* TIFF
* TXT
* XLS
* XLSX

#### Dimensione file supportata

Ogni file può avere dimensioni fino a 100 MB

#### Numero di file

È possibile caricare fino a 50 file (pagine, diapositive o fogli).

>[!IMPORTANT]
>
>I documenti vengono convertiti in una serie di immagini, ognuna delle quali viene considerata un file separato.
>
>Ad esempio, è possibile caricare un PowerPoint con 50 diapositive o 5 documenti Word, ciascuno con 10 pagine.

#### Altre best practice

Quando si carica un documento per la richiesta di compilazione automatica, considera quanto segue:

* Il riempimento automatico è attualmente ottimizzato per l&#39;alfabeto latino.
* È consigliabile utilizzare una dimensione di testo di 8 punti o superiore.
* La funzione di riempimento automatico può avere difficoltà con le immagini del documento, ad esempio immagini ruotate o distorte, grafici e il conteggio o l&#39;utilizzo di motivi spaziali sugli oggetti nelle immagini.
* Come sempre, si consiglia di verificare la precisione dei risultati prima di inviare la richiesta.

### Caricare un documento per compilare automaticamente una richiesta

È possibile caricare un documento da applicare all&#39;intero modulo o a una singola sezione del modulo.

1. Inizia a creare una richiesta.

   Per istruzioni, vedere [Creare e inviare richieste](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Per applicare il documento all&#39;intero modulo, fare clic sull&#39;icona IA ![Icona IA](assets/request-prompt-icon.png) sotto il nome del modulo.

   Oppure

   Per applicare il documento a una singola sezione, fai clic sull&#39;icona IA ![icona IA](assets/request-prompt-icon.png) accanto al nome della sezione.

1. Fai clic su **Carica file**, quindi seleziona il file dal file manager.

   Oppure

   Trascina il documento dal gestore di file nella casella **Carica file nel modulo di richiesta di compilazione automatica**.
1. Fai clic su **Compila il modulo** di **Compila la sezione**.

   Workfront genera suggerimenti per il modulo.
1. Per ogni suggerimento di campo, selezionare **Accetta** o **Rifiuta** sotto il campo.

   Oppure

   Selezionare **Accetta tutti** o **Rifiuta tutti** nella parte superiore della pagina per accettare o rifiutare tutti i suggerimenti.

## Risoluzione dei problemi

Se non ricevi i suggerimenti previsti, la causa potrebbe essere una delle seguenti:

* È necessario disporre di almeno un mese di dati della richiesta nel sistema prima che possa suggerire valori di campo da richieste precedenti.
* Un elemento di dati della richiesta deve trovarsi nel sistema da più di 24 ore prima di poter essere suggerito in un’altra richiesta.
* Potresti non aver seguito i guardrail di caricamento del documento durante il caricamento di un documento da cui estrarre i suggerimenti. Per ulteriori informazioni, vedi [Guardrail di caricamento documenti](#document-upload-guardrails) in questo articolo.

