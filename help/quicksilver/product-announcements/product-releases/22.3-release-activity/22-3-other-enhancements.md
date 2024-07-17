---
title: altri aggiornamenti durante il periodo di rilascio della versione 22.3
description: altri aggiornamenti durante il periodo di rilascio della versione 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 22.3 Altri miglioramenti

Questa pagina descrive tutti gli altri miglioramenti apportati con la versione 22.3 all’ambiente di anteprima. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione la settimana dell’11 luglio 2022. Per un elenco di tutte le modifiche disponibili con la versione 22.3, vedere [Panoramica sulla versione 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Schede orario aggiornate

Continuiamo a migliorare e aggiornare la tua esperienza quando lavori con le schede orario. Di seguito sono riportate alcune delle funzioni incluse in questo aggiornamento:

* Un nuovo look in linea con la nuova esperienza Workfront.

* Salvataggio automatico per salvare automaticamente le ore registrate e i commenti alle ore non appena vengono aggiunti.

* Un layout di pagina più intuitivo per far corrispondere le altre pagine oggetto. Ad esempio, abbiamo aggiunto un pannello a sinistra alla scheda orario. Gli aggiornamenti delle schede orario vengono ora visualizzati nella sezione Aggiornamenti nel pannello a sinistra. È inoltre possibile eliminare una scheda attività dalla pagina della scheda attività e aggiungerla all&#39;elenco Preferiti.

* Migliora l’esperienza di ricerca e aggiunta di progetti, attività o problemi alla scheda orario. Corrisponde all’esperienza in tutti gli altri elenchi in Workfront.

* Il pannello Riepilogo è disponibile per attività e problemi, per aggiungere commenti o aggiornare informazioni direttamente dalla scheda orario.


Con l’aggiornamento corrente, sono state rese obsolete anche le seguenti funzioni:

* La creazione di un&#39;attività da un aggiornamento è stata rimossa. Questa funzione è stata rimossa a partire dalla versione 2018.2 dalle aree Aggiornamenti di tutti gli altri oggetti, ma era ancora disponibile nel flusso di aggiornamento della scheda orario.

* La sezione &quot;Aggiungi spese da una scheda orario. &quot;La preferenza è stata rimossa dall’area Preferenze scheda orario e ore di Configura e non è più possibile registrare le spese dalla scheda orario. Puoi comunque registrare le spese dalle pagine delle attività e del progetto.


Per ulteriori informazioni, consulta i seguenti articoli:

* [Comprendere il layout della scheda orario](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [Configurare le preferenze di orario e scheda orario](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## Miglioramenti al pannello di navigazione a sinistra

Sono stati apportati diversi miglioramenti al pannello di navigazione a sinistra in Adobe Workfront.

* L’aspetto del pannello di navigazione a sinistra è stato aggiornato agli standard di progettazione Adobi, inclusi colori e font.

* Il collegamento &quot;Aggiungi sezione personalizzata&quot; nella parte inferiore del pannello è stato rinominato &quot;Aggiungi dashboard&quot; per spiegare meglio la sua funzione.

## Abilitare la rotazione automatica dei token di aggiornamento nelle applicazioni OAuth2 personalizzate

Per consentire un maggiore controllo sulla sicurezza delle applicazioni OAuth2 personalizzate, è stata aggiunta l’opzione per abilitare la rotazione dei token di aggiornamento. Quando questa opzione è abilitata, ogni volta che viene utilizzato un token di aggiornamento, l’applicazione crea e invia automaticamente un nuovo token di aggiornamento e disabilita quello precedente.

L’applicazione deve memorizzare il nuovo token di aggiornamento dopo ogni aggiornamento. Workfront non memorizza questo token di aggiornamento.

In precedenza, i token di aggiornamento scadevano dopo un periodo di tempo impostato configurato nelle impostazioni personalizzate dell’applicazione OAuth2.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## Utilizzare PKCE nelle integrazioni OAuth2 personalizzate per le applicazioni web a pagina singola

Ora puoi creare applicazioni web a pagina singola nelle integrazioni personalizzate utilizzando PKCE. PKCE è un flusso di autorizzazione sicuro che funziona bene con le applicazioni di aggiornamento dinamico come le app mobili, ma è prezioso per tutti i client OAuth2. Invece di un segreto client statico, PKCE utilizza una stringa generata dinamicamente, eliminando il rischio di perdita di un segreto client.

In precedenza, le opzioni disponibili per le applicazioni OAuth2 personalizzate utilizzavano il nome e la password di un utente o un segreto client.

Per ulteriori informazioni, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
