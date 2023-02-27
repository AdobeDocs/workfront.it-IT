---
content-type: api;faq
navigation-topic: general-api
title: Domande frequenti - Abbonamenti agli eventi
description: Domande frequenti - Abbonamenti agli eventi
author: Becky
feature: Workfront API
exl-id: a6120939-5d76-4f46-a304-125de6b22502
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 0%

---

# Domande frequenti - Abbonamenti agli eventi

<!--
{{highlighted-preview}}
-->

Di seguito sono riportate le domande frequenti sugli abbonamenti agli eventi:

## Che cos’è un abbonamento?

Una sottoscrizione è un set di dati utilizzati per associare e distribuire eventi Adobe Workfront all’endpoint HTTP di un cliente. Questa risorsa è composta da 4 attributi principali:

* customer_id
* obj_code
* obj_id
* url

Una sottoscrizione può anche avere altri attributi, ad esempio il proprio ID univoco e la data di creazione, ma gli attributi elencati sopra vengono principalmente utilizzati per far corrispondere gli eventi e consegnarli ai clienti.

## Sono in grado di selezionare gli eventi che vengono inviati a un endpoint in base a determinati criteri all’interno di un payload dell’evento?

I filtri di abbonamento agli eventi consentono di ordinare i sottomoduli di eventi in base a criteri specifici. Si consiglia di applicare filtri alle sottoscrizioni di eventi in quanto potrebbe ridurre notevolmente il numero di messaggi che un endpoint deve utilizzare. Per ulteriori informazioni consulta [Filtro della sottoscrizione degli eventi](../../wf-api/general/event-subs-api.md#event).

## Perché l&#39;API restituisce un codice di risposta in conflitto 409?

Se tenti di creare un abbonamento a un evento e ricevi un codice di risposta: 409 in conflitto, l&#39;abbonamento che si è tentato di creare è un duplicato. Workfront non consente la creazione di sottoscrizioni duplicate.

## Cosa devo fare se i miei messaggi non vengono recapitati all’endpoint?

Cerca i seguenti scenari e utilizza la soluzione consigliata:

* Assicurati che l&#39;endpoint di sottoscrizione—definito da **url** field - restituisce un codice di risposta HTTP 2XX. In caso contrario, contatta il supporto Workfront o consulta [Requisiti di consegna abbonamento agli eventi](../../wf-api/general/setup-event-sub-endpoint.md).

* La richiesta di consegna dell’evento potrebbe essere scaduta per timeout prima del completamento. Assicurati che l&#39;endpoint risponda in modo coerente entro 5 secondi. Questo è il timeout predefinito impostato per la richiesta HTTP di consegna di un messaggio di abbonamento a un evento. Se l&#39;endpoint non risponde entro 5 secondi, contatta il supporto Workfront o consulta [Requisiti di consegna abbonamento agli eventi](../../wf-api/general/setup-event-sub-endpoint.md).
* Gli eventi potrebbero non generare il tuo modo di pensare. Assicurati di non fare supposizioni su come o quando gli eventi dovrebbero e attivarsi. Ad esempio, si potrebbe pensare che l&#39;aggiornamento di un documento su un&#39;attività generi un evento di aggiornamento dell&#39;attività, ma invece genera un evento di creazione o aggiornamento del documento.
* L’abbonamento potrebbe non essere configurato come previsto. Puoi creare abbonamenti a eventi in ambienti diversi e aspettarti che vengano trasferiti come gli altri dati di Workfront. Tuttavia, i dati di abbonamento agli eventi non sono configurati per essere copiati o promossi ad altri ambienti. Assicurati di inviare richieste API all’ambiente corretto e che le sottoscrizioni in tale ambiente siano configurate come previsto.
* Il payload non è stato ricevuto perché l&#39;indirizzo IP Workfront necessario non è stato aggiunto all&#39;inserire nell&#39;elenco Consentiti del firewall. Gli eventi di abbonamento agli eventi vengono inviati solo da alcuni indirizzi IP. Assicurati che la rete di destinazione disponga di tutte le eccezioni IP necessarie per ricevere payload da Workfront Event Subscriptions.

## Perché i miei messaggi devono avere un tempo eccessivo per raggiungere l’endpoint?

Alcuni dei seguenti scenari potrebbero essere responsabili:

* Un&#39;operazione di grandi dimensioni, ad esempio un aggiornamento collettivo, nel sistema può causare l&#39;accodamento di un gran numero di messaggi contemporaneamente, il che può richiedere del tempo per l&#39;elaborazione.
* I calcoli a lungo termine o i calcoli della cronologia sui progetti di grandi dimensioni potrebbero causare un ritardo nella pubblicazione dei messaggi in Sottoscrizioni evento da utilizzare.
* La sottoscrizione potrebbe essere stata disabilitata.

   * Dopo un periodo di tolleranza di 100 messaggi, se un particolare URL (che potrebbe essere associato a una o più sottoscrizioni) non riesce più del 70% del tempo o se l’URL non riesce a recapitare dopo 2000 tentativi consecutivi, non viene effettuato alcun tentativo di consegna per tutti i messaggi che corrispondono alle sottoscrizioni con lo stesso URL. Al contrario, tali messaggi vengono immediatamente messi in coda per un nuovo tentativo.

      Ogni 10 minuti dopo che un URL è disabilitato, tentiamo di inviare il messaggio successivo che viene inviato per l’elaborazione. Se il messaggio ha esito positivo, riattiveremo tale URL e successivamente tutte le sottoscrizioni corrispondenti. Se l&#39;invio del messaggio non riesce, il timer di 10 minuti viene reimpostato e riproveremo dopo la scadenza.

      Questo comportamento può essere percepito come consegne incoerenti o ritardate, ma segue semplicemente i nostri criteri per la gestione dei messaggi di abbonamento agli eventi.

   * L’URL di abbonamento a un evento verrà disabilitato se viene soddisfatta una delle seguenti condizioni:

      * L’URL di abbonamento non è riuscito a consegnare per 7 giorni e non ha superato almeno 2000 tentativi di consegna consecutivi nelle ultime 72 ore.
      * L&#39;URL di abbonamento non è riuscito a fornire 50.000 tentativi consecutivi.

## Cosa devo fare se ricevo uno stato di risposta 500 quando si tenta di chiamare l’API di abbonamento agli eventi?

Contattare il supporto Workfront. Per informazioni su come contattare il supporto, consulta [Contatta l’Assistenza clienti](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## Quali diversi tipi di autenticazione è possibile utilizzare con gli abbonamenti agli eventi di Workfront?

Puoi utilizzare qualsiasi autenticazione che utilizza un token portatore. La **authToken** il campo di una sottoscrizione è una stringa che rappresenta un token portatore OAuth2 utilizzato per l’autenticazione con l’URL specificato in **url** campo . In teoria, questo valore del token potrebbe essere qualsiasi cosa purché l’endpoint di destinazione sia consapevole di come gestire la relativa codifica, ovvero **utf-8**.

## Quanto tempo devo trascorrere prima di ricevere il payload dell’evento da Workfront Event Subscriptions?

In generale, puoi aspettarti di ricevere le richieste di consegna degli eventi di abbonamento agli eventi in meno di 5 secondi dalla registrazione della modifica dei dati. In media, le notifiche webhook vengono ricevute in meno di 1 secondo dal momento in cui viene apportata la modifica dei dati. Tuttavia, il servizio può ricevere messaggi in quantità tali da richiedere anche più tempo.

## Risorse aggiuntive

* **Documentazione API**: [API iscrizione agli eventi](../../wf-api/general/event-subs-api.md)

* **Best practice**: [Best practice per l’abbonamento agli eventi](../../wf-api/general/event-sub-best-practice.md)

* **Campi che attivano i payload della sottoscrizione evento**: [Campi delle risorse della sottoscrizione evento](../../wf-api/api/event-sub-resource-fields.md)

* **Informazioni sui nuovi tentativi di abbonamento agli eventi**: [Tentativi di abbonamento agli eventi](../../wf-api/api/event-sub-retries.md)

* **Configurazione del firewall per Workfront**: [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)
