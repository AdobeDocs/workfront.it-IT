---
content-type: release-notes
keywords: note,trimestrale,aggiornamento
navigation-topic: product-releases
title: 21.1 Altri miglioramenti
description: Questa pagina descrive tutti gli altri miglioramenti apportati all’ambiente di anteprima con la versione 21.1. Questi miglioramenti saranno resi disponibili nell'ambiente di produzione la settimana del 15 febbraio 2021.
author: Luke
feature: Product Announcements
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 21.1 Altri miglioramenti

Questa pagina descrive tutti gli altri miglioramenti apportati all’ambiente di anteprima con la versione 21.1. Questi miglioramenti saranno resi disponibili nell&#39;ambiente di produzione la settimana del 15 febbraio 2021.

Per un elenco di tutte le modifiche disponibili con la versione 21.1, vedi [Panoramica sulla versione 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Aggiornamenti ai requisiti di errore della sottoscrizione agli eventi

Sono in corso l’aggiornamento dei requisiti di disattivazione software degli errori di abbonamento agli eventi. Oltre ai requisiti esistenti, gli abbonamenti agli eventi verranno disattivati in modo morbido se non riescono a ottenere una consegna corretta entro 2000 tentativi. Ciò è inteso a rafforzare l&#39;attuale regola del 70% di fallimento che può portare a quantità eccessive di insuccessi, in alcune condizioni.

Inoltre, a partire da febbraio 2021, aggiungeremo i requisiti per la disabilitazione.

Per ulteriori informazioni sui nuovi requisiti di disattivazione software e di disattivazione hardware, vedi [Domande frequenti - Abbonamenti agli eventi](../../../wf-api/general/event-subs-faq.md).

## Nuovi campi Team disponibili per il digest giornaliero

Abbiamo aggiunto i campi di approvazione e assegnazione del team all&#39;e-mail di riepilogo giornaliero necessario per l&#39;azione.

Per ulteriori informazioni, consulta [Notifiche: Azioni necessarie](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## Sostituzione dell’opzione e-mail POP nelle code di richiesta

Stiamo sostituendo l’opzione POP email per le code di richiesta con un nuovo sistema gestito da Workfront. Potrai comunque inviare le richieste via e-mail, ma dovrai impostare un nuovo indirizzo e-mail gestito da Adobe Workfront nell’area Coda richieste .

Queste modifiche sono disponibili per il test in Anteprima.

L’e-mail viene disabilitata automaticamente in tutti gli ambienti di anteprima. Per abilitare le e-mail a scopo di test, vedi [Abilitare la consegna di e-mail dall’ambiente Sandbox di anteprima](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

Per ulteriori informazioni, consulta [Consenti agli utenti di inviare un problema via e-mail a un progetto di coda richieste](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

Per ulteriori informazioni sul motivo per cui stiamo apportando questa modifica, vedi [Nuovo sistema gestito di Adobe Workfront per sostituire le e-mail POP per le code di richiesta con 21.1](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

Questa funzione è ora inclusa nella [Gestione delle code nella nuova esperienza Workfront](https://one.workfront.com/s/learningpath4/queue-management-MCYCJRWK36QZBP7PGMNDMSPRN3LE) percorso di apprendimento su Workfront One.

## Limitare la modifica delle ore sui fogli ore

Per un maggiore controllo sulle schede attività e sulla modifica delle ore, è stata aggiunta un’impostazione che consente di limitare la modifica delle ore ai proprietari delle schede attività e agli amministratori di sistema.

In precedenza, gli utenti con l&#39;opzione Fogli orari e ore abilitata nel livello di accesso potevano modificare le ore su qualsiasi scheda attività.

Per ulteriori informazioni, consulta [Configurare le preferenze relative a schede attività e ora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Filtri e viste migliorati nell’area Timesheets

Sono stati aggiunti i seguenti miglioramenti quando si aggiunge un progetto, un&#39;attività o un problema a una scheda attività:

* Filtri: Sono stati aggiunti filtri per progetti e problemi. Fai clic su Altre opzioni per visualizzare questi filtri. In precedenza, era disponibile solo il filtro Attività .
* Viste: Nella pagina Ricerca sono state aggiunte le opzioni Visualizza e Raggruppamento .

Per ulteriori informazioni, consulta [Tempo di log](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Nascondere la casella del tempo eccessivo nei fogli presenze

Ora è possibile nascondere la casella del tempo eccessivo per semplificare la confusione dell’utente se non si tiene traccia del tempo eccessivo in Workfront. È possibile nascondere la casella del lavoro straordinario per una scheda attività a uso singolo o nel profilo della scheda attività:

* Scheda attività a uso singolo: Quando si sceglie di nascondere la casella del lavoro straordinario in una singola scheda attività, questa viene nascosta solo per tale scheda attività. Per ulteriori informazioni, consulta [Creare una scheda attività a uso singolo](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* Profilo scheda attività: Quando si sceglie di nascondere la casella del lavoro straordinario nel profilo scheda attività, tutte le schede attività future create per gli utenti assegnati a quel profilo non visualizzeranno la casella del lavoro straordinario. Per ulteriori informazioni, consulta [Creare, modificare e assegnare profili della scheda attività](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

In precedenza, non era possibile nascondere la casella del lavoro straordinario sui fogli presenze.

## Espandi o comprimi gli elementi nella navigazione breadcrumb

Per facilitare la visualizzazione dell’intero percorso di breadcrumb, è stata aggiunta una funzionalità di espansione e compressione.

Ora, tutti gli elementi troncati vengono raggruppati prima del Progetto con il testo &quot;altro&quot;. Ad esempio, &quot;3 more&quot; indica che sono presenti 3 oggetti che non vengono visualizzati.

In precedenza era necessario fare clic sui puntini di sospensione per visualizzare gli oggetti troncati in un menu a discesa.

Per visualizzare tutti gli elementi nel breadcrumb, fai clic su &quot;Altro&quot; all’inizio del breadcrumb per espandere gli elementi. Una volta espanso, puoi fare clic su &quot;Meno&quot; per comprimere di nuovo gli elementi.

## Nuovo aspetto per la navigazione nel breadcrumb

Per aiutare gli utenti a identificare meglio dove si trovano in Workfront e a navigare più facilmente tra gli oggetti, sono stati apportati i seguenti miglioramenti alla navigazione nel breadcrumb:

* Ogni elemento della breadcrumb ora include un’etichetta di oggetto.
* La pagina corrente è ora inclusa nel breadcrumb ed è in corsivo.
* La navigazione tramite tastiera e tramite assistenti vocali sono ora disponibili per le breadcrumb.
* Modifiche aggiuntive allo stile minori

