---
title: Compilazione automatica di una richiesta tramite IA
content-type: reference
description: Puoi utilizzare l’intelligenza artificiale per compilare automaticamente i campi della richiesta.
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
source-git-commit: 9e1a5718092092bb9ca98cf92ddd2a1a07f32f51
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Compilazione automatica di una richiesta tramite IA

L’intelligenza artificiale può aiutarti a compilare automaticamente i campi della richiesta. Può suggerire valori di campo in base alle richieste precedenti o analizzarli da testo come le e-mail.

È possibile approvare o rifiutare questi invii prima di inviare la richiesta.

La funzione di riempimento automatico non sovrascrive i campi già compilati.

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

La funzione di riempimento automatico può suggerire i valori dei campi in base al testo, ad esempio le e-mail. Incollando in un blocco di testo, Workfront ha elaborato il testo per suggerire i valori dei campi in base al testo.

Ad esempio, se l’e-mail include &quot;Scadenza 1 giugno&quot; e il modulo di richiesta ha un campo per la data di scadenza, Workfront consiglia 1 giugno per tale valore di campo.

Questo tipo di suggerimento controlla anche le richieste precedenti per contesti simili. Ad esempio, se il prompt indica che la richiesta è per un determinato client, Workfront può individuare e immettere automaticamente l’indirizzo di fatturazione per tale client, in base alle richieste precedenti.

È possibile incollare il testo da applicare all&#39;intero modulo o a una singola sezione del modulo.

Per utilizzare i suggerimenti basati su un prompt di testo incollato:

1. Inizia a creare una richiesta.

   Per istruzioni, vedere [Creare e inviare richieste](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Per applicare il prompt di testo all&#39;intero modulo, fare clic su **Compilazione automatica con IA** nell&#39;angolo superiore destro dello schermo.

   Oppure

   Per applicare il prompt di testo per una singola sezione, fai clic sull&#39;icona IA ![icona IA](assets/request-prompt-icon.png) accanto al nome della sezione.

1. Incollare il testo nella casella del prompt.
1. Fai clic su **Compila il modulo**.

   Workfront genera suggerimenti per il modulo.
1. Per ogni suggerimento di campo, selezionare **Accetta** o **Rifiuta** sotto il campo.

   Oppure

   Selezionare **Accetta tutti** o **Rifiuta tutti** nella parte superiore della pagina per accettare o rifiutare tutti i suggerimenti.

