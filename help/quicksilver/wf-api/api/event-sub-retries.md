---
content-type: api
navigation-topic: api-navigation-topic
title: Nuovi tentativi di abbonamento agli eventi
description: Nuovi tentativi di abbonamento agli eventi
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Nuovi tentativi di abbonamento agli eventi

Quando si implementa un sistema di consegna dei messaggi, è necessario porre alcune avvertenze per garantire stabilità, coerenza e buona esperienza utente. Una delle carenze di un sistema di consegna dei messaggi consiste nel garantire che i messaggi raggiungano correttamente la destinazione e nel sapere cosa fare in caso di mancato arrivo dei messaggi.

Alcune integrazioni possono accettare un errore di consegna, quindi rilascia il messaggio e passa al messaggio successivo.  In altre integrazioni, l’impossibilità di recapitare un messaggio non può essere ignorata. Ad esempio, un’integrazione finanziaria potrebbe tentare di recapitare un messaggio, ma riceve invece un codice di stato HTTP 404, che indica che il server non è riuscito a trovare l’endpoint al quale il messaggio doveva essere recapitato. In tali casi, un messaggio mancante potrebbe significare che qualcuno non viene pagato per il tempo che ha dedicato o che un&#39;organizzazione supera il budget con risorse contrattuali.

## Strategia di Adobe Workfront per i tentativi di abbonamento agli eventi

Poiché i clienti sfruttano la piattaforma Workfront come parte fondamentale del loro lavoro quotidiano, il framework Workfront Event Subscription fornisce un meccanismo per garantire che la consegna di ogni messaggio venga tentata nella massima misura possibile.

I messaggi in uscita attivati dagli eventi che non vengono consegnati agli endpoint del cliente vengono inviati nuovamente fino alla consegna corretta, per un periodo massimo di 48 ore. Durante questo periodo, i nuovi tentativi si verificano con una frequenza incrementale fino a quando la consegna non ha esito positivo o fino a quando non sono stati effettuati 11 tentativi.

La formula per questi nuovi tentativi è:

`((2^attempt) - 1) * 84800ms`

Il primo nuovo tentativo si verifica dopo 1,5 minuti, il secondo dopo quasi 5 minuti e l’undicesimo dopo circa 48 ore.

I clienti devono assicurarsi che tutti gli endpoint che utilizzano messaggi in uscita da Abbonamenti eventi di Workfront siano configurati per restituire a Workfront un messaggio di risposta di 200 livelli quando la consegna ha esito positivo.

## Regole di abbonamento disabilitate e congelate

* L&#39;URL di una sottoscrizione è **disabilitato** se ha una percentuale di errori superiore al 70% con oltre 100 tentativi OPPURE se ha 2.000 errori consecutivi
* Un URL di abbonamento è **bloccato** se ha più di 2.000 errori consecutivi e l&#39;ultimo successo è stato più di 72 ore fa OPPURE se ha 50.000 errori consecutivi in qualsiasi arco temporale.
* Un URL di abbonamento **disabled** continuerà a tentare la consegna ogni 10 minuti e verrà riabilitato con una consegna riuscita.
* Un URL di abbonamento **congelato** non tenterà mai la consegna a meno che non venga abilitato manualmente effettuando una richiesta API.




<!--

## Handling Failed Event-Triggered Outbound Messages

The following flowchart shows the strategy for reattempting message deliveries with Workfront Event Subscriptions:

![Event sub retries](assets/event-subscription-circuit-breaker-retries-350x234.png)

The following explanations correspond with the steps depicted in the flowchart:

1. Message fails to be delivered. 
1. Message delivery failure information is logged.

   All failed attempts to deliver a message are logged so that debugging may be performed to determine the root cause of a given failure or series of failures. 

1. URL failures incremented. 
1. Message attempt count is incremented. 
1. Calculate the delay until this message's delivery will be attempted again. 
1. Message is placed onto the message retry queue.

   As shown in the preceding flowchart, the message queue used for processing message delivery retries is a separate queue from the one that processes the initial delivery attempt for each message. This allows the near real-time flow of messages to continue unimpeded by the failure of any subset of messages. 

1. URL circuit status is evaluated. One of the following occurs:

   * If the circuit is open and not allowing deliveries at this time, restart the process at step 5.
   * If the circuit is half-open, this implies that our circuit is currently open, but enough time has passed to allow testing of the URL to see if the problem with delivering to it has been resolved.
   * If the message delivery attempt limits have been reached (48 hours of retrying) then the message is dropped

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1 

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1.
   -->
