---
content-type: release-notes
keywords: note,trimestrale,aggiornamento
navigation-topic: product-releases
title: 21.1 Altri miglioramenti
description: Questa pagina descrive tutti gli altri miglioramenti apportati con la versione 21.1 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione la settimana del 15 febbraio 2021.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# 21.1 Altri miglioramenti

Questa pagina descrive tutti gli altri miglioramenti apportati con la versione 21.1 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione la settimana del 15 febbraio 2021.

Per un elenco di tutte le modifiche disponibili con la versione 21.1, consulta [Panoramica sulla versione 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Aggiornamenti ai requisiti di errore della sottoscrizione eventi

Stiamo aggiornando i requisiti di soft-disable per gli errori di abbonamento agli eventi. Oltre ai requisiti esistenti, le sottoscrizioni di eventi verranno ora disabilitate se non riescono a raggiungere una consegna corretta entro 2.000 tentativi. In tal modo si intende rafforzare l&#39;attuale regola del fallimento del 70% che, in determinate condizioni, può portare a un numero eccessivo di fallimenti.

Inoltre, a partire da febbraio 2021 verranno aggiunti requisiti di hard-disable.

Per ulteriori informazioni sui nuovi requisiti di soft-disable e hard-disable, consulta [Domande frequenti - Abbonamenti agli eventi](../../../wf-api/general/event-subs-faq.md).

## Nuovi campi del team disponibili per il riepilogo giornaliero

Abbiamo aggiunto i campi Approvazione team e Assegnazioni all’e-mail Riepilogo giornaliero azioni necessarie.

Per ulteriori informazioni, consulta [Notifiche: azione necessaria](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## Sostituzione dell’opzione POP email nelle code di richiesta

Stiamo sostituendo l’opzione e-mail POP per le code di richieste con un nuovo sistema gestito da Workfront. Potrai comunque inviare le richieste tramite e-mail, ma dovrai impostare invece un nuovo indirizzo e-mail gestito da Adobe Workfront nell’area Coda richieste.

Queste modifiche sono disponibili per il test in Anteprima.

L’e-mail viene disattivata automaticamente in tutti gli ambienti di anteprima. Per abilitare l’e-mail a scopo di test, consulta [Abilitare la consegna di e-mail dall’ambiente Sandbox di anteprima](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

Per ulteriori informazioni, consulta [Consentire agli utenti di inviare un problema tramite e-mail a un progetto della coda richieste](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

Per ulteriori informazioni sulle ragioni di questo cambiamento, consulta [Nuovo sistema gestito da Adobe Workfront per sostituire POP email for Request Queues con 21.1](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

Questa funzione è ora inclusa nel [Gestione delle code nella nuova esperienza Workfront](https://one.workfront.com/s/learningpath4/queue-management-MCYCJRWK36QZBP7PGMNDMSPRN3LE) percorso di apprendimento in Workfront One.

## Limita la modifica delle ore nelle schede orario

Per fornire un maggiore controllo sulle schede orario e sulla modifica delle ore, è stata aggiunta un&#39;impostazione che consente di limitare la modifica delle ore ai proprietari delle schede orario e agli amministratori di sistema.

In precedenza, gli utenti con l’opzione Schede orario e ore abilitata nel loro livello di accesso potevano modificare le ore su qualsiasi scheda orario.

Per ulteriori informazioni, consulta [Configurare le preferenze di orario e scheda orario](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Sono stati migliorati i filtri e le visualizzazioni nell’area Schede orario

Sono stati aggiunti i seguenti miglioramenti quando si aggiunge un progetto, un&#39;attività o un problema a una scheda orario:

* Filtri: sono stati aggiunti i filtri per Progetti e Problemi. Fai clic su Altre opzioni per visualizzare questi filtri. In precedenza, erano disponibili solo i filtri per le attività.
* Visualizzazioni: sono state aggiunte le opzioni Visualizza e Raggruppamento alla pagina Ricerca.

Per ulteriori informazioni, consulta [Tempo di connessione](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Nascondi la casella del lavoro straordinario nelle schede orario

Ora puoi nascondere la casella del lavoro straordinario per semplificare la confusione degli utenti se non tieni traccia del lavoro straordinario in Workfront. Puoi nascondere la casella del lavoro straordinario per una scheda orario monouso o nel Timesheet Ricorrente:

* Scheda orario monouso: quando si sceglie di nascondere la casella del lavoro straordinario in una singola scheda orario, questa viene nascosta solo per tale scheda. Per ulteriori informazioni, consulta [Creare una scheda orario monouso](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* Profilo scheda orario: quando si sceglie di nascondere la casella Lavoro straordinario nel Profilo scheda orario, tutte le schede orario future create per gli utenti assegnati a quel profilo non visualizzeranno la casella Lavoro straordinario. Per ulteriori informazioni, consulta [Creare, modificare e assegnare profili di schede orario](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

In precedenza, non era possibile nascondere la casella del lavoro straordinario nelle schede orario.

## Espandere o comprimere gli elementi nella navigazione delle breadcrumb

Per semplificare la visualizzazione dell’intero percorso della breadcrumb, sono state aggiunte le funzionalità di espansione e compressione.

Ora, tutti gli elementi troncati vengono raggruppati prima del progetto con il testo &quot;altro&quot;. Ad esempio, &quot;3 ulteriori&quot; indica che non vengono visualizzati 3 oggetti.

In precedenza, era necessario fare clic sui puntini di sospensione per visualizzare gli oggetti troncati in un menu a discesa.

Per visualizzare tutti gli elementi nel breadcrumb, fai clic su &quot;altro&quot; all’inizio del breadcrumb per espandere gli elementi. Una volta espansi, puoi fare clic su &quot;Less&quot; (Meno) per comprimere nuovamente gli elementi.

## Nuovo aspetto per la navigazione nel breadcrumb

Per aiutare gli utenti a identificare meglio la loro posizione in Workfront e a navigare più facilmente tra gli oggetti, sono stati apportati i seguenti miglioramenti alla navigazione delle breadcrumb:

* Ogni elemento nella breadcrumb ora include un’etichetta oggetto.
* La pagina corrente è ora inclusa nel breadcrumb ed è in corsivo.
* La navigazione tramite tastiera e la navigazione tramite assistente vocale sono ora disponibili per le breadcrumb.
* Ulteriori modifiche minori allo stile

