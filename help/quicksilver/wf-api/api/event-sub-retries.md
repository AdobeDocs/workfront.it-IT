---
content-type: api
navigation-topic: api-navigation-topic
title: Nuovi tentativi di abbonamento agli eventi
description: Nuovi tentativi di abbonamento agli eventi
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Nuovi tentativi di abbonamento agli eventi

Quando si implementa un sistema di consegna dei messaggi, è necessario porre alcune avvertenze per garantire stabilità, coerenza e buona esperienza utente. Una delle carenze di un sistema di consegna dei messaggi consiste nel garantire che i messaggi raggiungano correttamente la destinazione e nel sapere cosa fare in caso di mancato arrivo dei messaggi.

Alcune integrazioni possono accettare un errore di consegna, quindi rilascia il messaggio e passa al messaggio successivo.  In altre integrazioni, l’impossibilità di recapitare un messaggio non può essere ignorata. Ad esempio, un’integrazione finanziaria potrebbe tentare di recapitare un messaggio, ma riceve invece un codice di stato HTTP 404, che indica che il server non è riuscito a trovare l’endpoint al quale il messaggio doveva essere recapitato. In tali casi, un messaggio mancante potrebbe significare che qualcuno non viene pagato per il tempo che ha dedicato o che un&#39;organizzazione supera il budget con risorse contrattuali.

## Strategia di Adobe Workfront per i tentativi di abbonamento agli eventi

Poiché i clienti sfruttano la piattaforma Workfront come parte fondamentale del loro lavoro quotidiano, il framework Workfront Event Subscription fornisce un meccanismo per garantire che la consegna di ogni messaggio venga tentata nella massima misura possibile.

I messaggi in uscita attivati dagli eventi che non vengono consegnati agli endpoint del cliente vengono inviati nuovamente fino alla consegna corretta, per un periodo massimo di 48 ore. Durante questo periodo, i nuovi tentativi si verificano con una frequenza ridotta in modo incrementale fino alla riuscita della consegna o allo scadere di 48 ore.

I clienti devono assicurarsi che tutti gli endpoint che utilizzano messaggi in uscita da Abbonamenti eventi di Workfront siano configurati per restituire a Workfront un messaggio di risposta di 200 livelli quando la consegna ha esito positivo.

## Gestione dei messaggi in uscita attivati da eventi non riusciti

Il diagramma di flusso seguente mostra la strategia per ritentare le consegne dei messaggi con le sottoscrizioni di eventi di Workfront:

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

Le seguenti spiegazioni corrispondono ai passaggi descritti nel diagramma di flusso:

1. Impossibile recapitare il messaggio.
1. Le informazioni sull’errore di consegna del messaggio sono state registrate.

   Tutti i tentativi non riusciti di recapitare un messaggio vengono registrati in modo da poter eseguire il debug per determinare la causa principale di un determinato errore o di una serie di errori.

1. Errori URL incrementati.
1. Il conteggio dei tentativi di messaggio viene incrementato.
1. Calcola il ritardo fino al successivo tentativo di consegna del messaggio.
1. Il messaggio viene inserito nella coda dei nuovi tentativi del messaggio.

   Come mostrato nel diagramma di flusso precedente, la coda di messaggi utilizzata per l’elaborazione dei nuovi tentativi di consegna dei messaggi è una coda separata da quella che elabora il tentativo di consegna iniziale per ciascun messaggio. Questo consente al flusso di messaggi in tempo reale di continuare senza ostacoli a causa del fallimento di qualsiasi sottoinsieme di messaggi.

1. Lo stato del circuito URL viene valutato. Si verifica una delle seguenti situazioni:

   * Se il circuito è aperto e non consente consegne in questo momento, riavviare il processo al punto 5.
   * Se il circuito è semi-aperto, ciò significa che il nostro circuito è attualmente aperto, ma è trascorso abbastanza tempo per consentire il test dell’URL per vedere se il problema con la consegna ad esso è stato risolto.
   * Se sono stati raggiunti i limiti di tentativi di consegna del messaggio (48 ore di un nuovo tentativo), il messaggio viene eliminato

1. Se il circuito URL è chiuso e le consegne sono consentite, prova a consegnare il messaggio. Se questa consegna non riesce, il messaggio verrà riavviato al passaggio 1

1. Se il circuito URL è chiuso e le consegne sono consentite, prova a consegnare il messaggio. Se questa consegna non riesce, il messaggio verrà riavviato al passaggio 1.

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront disables Event Subscriptions when both of the following criteria are met:
   <ul>
   <!--
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The Event Subscription has failed 1000 delivery attempts consecutively</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">48 hours have passed since the last successful delivery</li>
   </ul></li>
   -->
