---
content-type: api
navigation-topic: general-api
title: Requisiti di consegna dell’abbonamento agli eventi
description: Requisiti di consegna dell’abbonamento agli eventi
author: Becky
feature: Workfront API
role: Developer
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Requisiti di consegna dell’abbonamento agli eventi

I messaggi di abbonamento agli eventi sono notifiche che possono essere configurate per avvisare gli utenti quando si verificano determinati eventi. Per ulteriori informazioni sulle sottoscrizioni di eventi, consulta [Domande frequenti - Abbonamenti agli eventi](../../wf-api/general/event-subs-faq.md).

## Standard per la consegna dei messaggi di abbonamento agli eventi

Gli endpoint di servizio che utilizzano i messaggi di abbonamento agli eventi di Adobe Workfront devono soddisfare i seguenti requisiti di base, al fine di garantire che i messaggi vengano inviati e ricevuti correttamente:

* L’endpoint del servizio deve accettare le richieste HTTP POST. HTTP POST è il metodo di richiesta utilizzato in tutte le consegne dei messaggi di abbonamento agli eventi, inclusi i messaggi di convalida.

* Affinché il sistema di consegna della sottoscrizione dell’evento possa confermare che il messaggio è stato ricevuto correttamente, l’endpoint deve restituire uno stato HTTP di 200 livelli (ad esempio, 200 OK o 202) per tutti i messaggi in arrivo.

* Se non viene restituito uno stato di 200 livelli, il sistema di sottoscrizione degli eventi presuppone che il messaggio non sia stato recapitato correttamente e inizia ad applicare il criterio appropriato per i nuovi tentativi. Per ulteriori informazioni sui criteri per i nuovi tentativi di Workfront, consulta [Nuovi tentativi di abbonamento agli eventi](../../wf-api/api/event-sub-retries.md).

* Oltre a restituire uno stato di 200 livelli come stato di risposta, la risposta HTTP deve essere ricevuta entro cinque secondi dall’avvio del tentativo di consegna. Questo vincolo assicura che i processi aziendali dei consumatori o le limitazioni dell’infrastruttura non ritardino la consegna di altri messaggi in attesa di consegna.

* Se un processo aziendale a esecuzione prolungata viene attivato da un messaggio di abbonamento a un evento, Workfront consiglia di:

   1. l’endpoint salva le informazioni sul messaggio al momento della ricezione e risponde immediatamente con uno stato di 200 livelli.
   1. Dopo che un endpoint ha risposto a una richiesta di consegna della sottoscrizione dell’evento, è possibile elaborare i messaggi salvati.
