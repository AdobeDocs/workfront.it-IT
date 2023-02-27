---
content-type: api
navigation-topic: general-api
title: Requisiti di consegna abbonamento agli eventi
description: Requisiti di consegna abbonamento agli eventi
author: Becky
feature: Workfront API
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Requisiti di consegna abbonamento agli eventi

I messaggi di abbonamento agli eventi sono notifiche che possono essere configurate per avvisare gli utenti quando si verificano determinati eventi. Per ulteriori informazioni sugli abbonamenti agli eventi, consulta [Domande frequenti - Abbonamenti agli eventi](../../wf-api/general/event-subs-faq.md).

## Standard per la consegna dei messaggi di abbonamento agli eventi

Per garantire che i messaggi vengano inviati e ricevuti correttamente, gli endpoint di servizio che utilizzano i messaggi di abbonamento agli eventi di Adobe Workfront devono soddisfare i seguenti requisiti di base:

* L&#39;endpoint del servizio deve accettare richieste HTTP POST. HTTP POST è il metodo di richiesta utilizzato in tutte le consegne di messaggi di abbonamento a eventi, inclusi i messaggi di convalida.

* Affinché il sistema di consegna della sottoscrizione dell’evento riconosca che il messaggio è stato ricevuto correttamente, l’endpoint deve restituire uno stato HTTP a 200 livelli (ad esempio, 200 OK o 202) per tutti i messaggi in arrivo.

* Se non viene restituito uno stato a 200 livelli, il sistema di sottoscrizione dell’evento presuppone che il messaggio non sia stato consegnato correttamente e inizia ad applicare il criterio di esecuzione dei nuovi tentativi appropriato. Per ulteriori informazioni sui criteri per i nuovi tentativi di Workfront, consulta [Tentativi di abbonamento agli eventi](../../wf-api/api/event-sub-retries.md).

* Insieme alla restituzione di uno stato a 200 livelli come stato di risposta, la risposta HTTP deve essere ricevuta entro cinque secondi dall&#39;avvio del tentativo di consegna.Questo vincolo garantisce che i processi aziendali dei consumatori o le limitazioni dell&#39;infrastruttura non ritardano la consegna di altri messaggi in attesa di consegna.

* Se un processo aziendale di lunga durata viene attivato da un messaggio di abbonamento a un evento, Workfront consiglia di:

   1. l’endpoint salva le informazioni sul messaggio al momento della ricezione e risponde immediatamente con uno stato di 200 livelli.
   1. Dopo che un endpoint ha risposto a una richiesta di consegna della sottoscrizione di un evento, i messaggi salvati possono essere elaborati.
