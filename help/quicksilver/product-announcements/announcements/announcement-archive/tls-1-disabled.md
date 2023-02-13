---
content-type: reference
navigation-topic: announcements
title: TLS 1.2 da richiedere in Adobe Workfront
description: Per garantire una sicurezza ottimale, Adobe Workfront richiede che tutte le connessioni al browser e le integrazioni API che si basano su TLS 1.0 o versioni precedenti siano aggiornate per utilizzare TLS 1.2. Nell’ambiente di anteprima, TLS 1.0 è già disabilitato.
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# TLS 1.2 da richiedere in Adobe Workfront

Per garantire una sicurezza ottimale, Adobe Workfront richiede che tutte le connessioni al browser e le integrazioni API che si basano su TLS 1.0 o versioni precedenti siano aggiornate per utilizzare TLS 1.2. Nell’ambiente Anteprima, TLS 1.0 è già disabilitato.

Workfront ha ufficialmente terminato il supporto per TLS 1.0 a marzo 2018. Tutte le integrazioni che sfruttano TLS 1.0 cessano di funzionare a partire dal 9 gennaio 2019.  TLS 1.1 verrà disattivato nel quarto trimestre del 2019.

Le sezioni seguenti forniscono informazioni dettagliate su queste tappe importanti e su come prepararsi a questo aggiornamento nell’organizzazione:

## Workfront interrompe il supporto ufficiale di TLS 1.0 (5 marzo 2018)

Workfront ha terminato il supporto ufficiale per TLS 1.0 a marzo 2018.

Le connessioni browser e le integrazioni API che sfruttano TLS 1.0 sono ancora operative, ma Workfront non risolverà i problemi nell’applicazione Workfront relativi a TLS 1.0.

## Integrazioni Workfront con TLS 1.0 disattivato (9 gennaio 2019)

Il 9 gennaio 2019, tutte le connessioni al browser Workfront e le integrazioni API che sfruttano TLS 1.0 devono essere aggiornate per utilizzare TLS 1.1 o versione successiva. Le connessioni browser e le integrazioni API che continuano a utilizzare TLS 1.0 (connessioni in entrata o in uscita) non saranno più in grado di comunicare con l’applicazione Workfront in seguito a questo passaggio. 

## TLS 1.1 da disabilitare nel quarto trimestre 2019

Nell’ambiente di produzione, TLS 1.1 è stato disattivato il 21 ottobre 2019. Dopo questo periodo, tutte le integrazioni che utilizzano TLS 1.1 non funzioneranno più.

Questa modifica entrerà in vigore negli ambienti Preview e Sandbox il 7 agosto per aiutare le organizzazioni a prepararsi per lo spegnimento.

## Preparazione all’aggiornamento TLS

* [Accesso a Workfront tramite il browser](#when-accessing-workfront-via-the-browser)
* [Quando ci si connette a Workfront tramite API](#when-connecting-to-workfront-via-the-api)

### Accesso a Workfront tramite il browser {#when-accessing-workfront-via-the-browser}

Assicurati che gli utenti della tua organizzazione accedano a Workfront tramite un browser supportato. (Per informazioni sui browser supportati consulta [Requisiti del browser Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).)

Tutti i browser supportati da Workfront sono compatibili con TLS 1.2.

### Quando ci si connette a Workfront tramite API {#when-connecting-to-workfront-via-the-api}

Se stai integrando applicazioni di terze parti a Workfront tramite l’API (in entrata o in uscita), assicurati che TLS 1.2 (e i protocolli di crittografia TLS 1.2) siano abilitati nelle tue integrazioni.
