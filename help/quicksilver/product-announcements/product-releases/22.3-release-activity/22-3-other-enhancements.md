---
title: altri aggiornamenti durante l’intervallo di tempo per la versione 22.3
description: altri aggiornamenti durante l’intervallo di tempo per la versione 22.3
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# 22.3 Altri miglioramenti

Questa pagina descrive tutti gli altri miglioramenti apportati all’ambiente di anteprima con la versione 22.3. Questi miglioramenti sono stati resi disponibili nell&#39;ambiente di produzione la settimana dell&#39;11 luglio 2022. Per un elenco di tutte le modifiche disponibili con la versione 22.3, vedi [Panoramica sulla versione 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Schede temporali aggiornate

Continuiamo a migliorare e aggiornare la tua esperienza quando lavori con i fogli presenze. Di seguito sono riportate alcune delle funzioni incluse in questo aggiornamento:

* Un nuovo look per la nuova esperienza Workfront.

* La funzionalità di salvataggio automatico consente di salvare automaticamente le ore e le ore registrate al momento dell&#39;aggiunta dei commenti.

* Layout di pagina più intuitivo per corrispondere alle altre pagine dell’oggetto. Ad esempio, abbiamo aggiunto un pannello a sinistra alla scheda attività. Gli aggiornamenti della scheda attività vengono ora visualizzati nella sezione Aggiornamenti del pannello a sinistra. È inoltre possibile eliminare una scheda attività dalla pagina della scheda attività e aggiungere la scheda attività all&#39;elenco Preferiti.

* Un&#39;esperienza migliore per la ricerca e l&#39;aggiunta di progetti, attività o problemi alla scheda attività. Questo corrisponde all’esperienza in tutti gli altri elenchi in Workfront.

* Il pannello Riepilogo è disponibile per attività e problemi per aggiungere commenti o aggiornare informazioni direttamente dalla scheda attività.


Con l’aggiornamento corrente, sono state disattivate anche le seguenti funzioni:

* La creazione di un&#39;attività da un aggiornamento è stata rimossa. Questa funzione è stata rimossa dalla versione 2018.2 dalle aree Aggiornamenti di tutti gli altri oggetti, ma era ancora disponibile nel flusso di aggiornamento della scheda attività.

* &quot;Aggiungi spese da una scheda attività. &quot;la preferenza è stata rimossa dall&#39;area Preferenze scheda attività e ore di Configurazione e non è più possibile registrare le spese dalla scheda attività. È comunque possibile registrare le spese dalle pagine attività e progetto.


Per ulteriori informazioni, consulta i seguenti articoli:

* [Comprendere il layout del foglio presenze](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [Configurare le preferenze relative a schede attività e ora](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## Miglioramenti al pannello di navigazione a sinistra

Sono stati apportati diversi miglioramenti al pannello di navigazione a sinistra in Adobe Workfront.

* L’aspetto del pannello di navigazione a sinistra è stato aggiornato agli standard di progettazione Adobi, inclusi colori e font.

* Il collegamento &quot;Aggiungi sezione personalizzata&quot; nella parte inferiore del pannello è stato rinominato &quot;Aggiungi dashboard&quot; per spiegarne meglio la funzione.

## Abilitare la rotazione automatica dei token di aggiornamento nelle applicazioni OAuth2 personalizzate

Per consentire un maggiore controllo sulla sicurezza delle applicazioni OAuth2 personalizzate, abbiamo aggiunto l’opzione per abilitare la rotazione dei token di aggiornamento. Quando questa opzione è abilitata, ogni volta che viene utilizzato un token di aggiornamento, l’applicazione crea e invia automaticamente un nuovo token di aggiornamento e disabilita quello precedente.

L&#39;applicazione deve memorizzare il nuovo token di aggiornamento dopo ogni aggiornamento. Workfront non memorizza questo token di aggiornamento.

In precedenza, i token di aggiornamento erano scaduti dopo un periodo di tempo configurato nelle impostazioni personalizzate dell’applicazione OAuth2.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## Utilizzare PKCE nelle integrazioni personalizzate OAuth2 per le applicazioni web a pagina singola

È ora possibile creare applicazioni web a pagina singola nelle integrazioni personalizzate utilizzando PKCE. PKCE è un flusso di autorizzazione sicuro che funziona bene con applicazioni di aggiornamento dinamico come le app mobili, ma è prezioso in tutti i client OAuth2. Invece di un segreto client statico, PKCE utilizza una stringa generata in modo dinamico, eliminando il rischio di una perdita del segreto client.

In precedenza, le opzioni disponibili per le applicazioni OAuth2 personalizzate utilizzavano il nome e la password di un utente o un segreto client.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
