---
content-type: api;faq
navigation-topic: general-api
title: Domande frequenti - Abbonamenti agli eventi
description: Domande frequenti - Abbonamenti agli eventi
author: Becky
feature: Workfront API
role: Developer
exl-id: a6120939-5d76-4f46-a304-125de6b22502
source-git-commit: 77c07c7c7104d37360cc7630a89dd72836da477c
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 0%

---

# Domande frequenti - Abbonamenti agli eventi

<!--
{{highlighted-preview}}
-->

Di seguito sono riportate le domande frequenti relative agli abbonamenti agli eventi:

## Che cos’è un abbonamento?

Una sottoscrizione è un set di dati utilizzati per associare e inviare eventi Adobe Workfront all’endpoint HTTP di un cliente. Questa risorsa è composta da 4 attributi principali:

* customer_id
* obj_code
* obj_id
* url

Un abbonamento può avere anche altri attributi, come il proprio ID univoco e la data di creazione, ma gli attributi elencati sopra vengono utilizzati principalmente per far corrispondere gli eventi e distribuirli ai clienti.

## È possibile selezionare gli eventi da inviare a un endpoint in base a determinati criteri all’interno di un payload di eventi?

I filtri di abbonamento agli eventi consentono di ordinare i sottoeventi in base a criteri specifici. È consigliabile applicare filtri alle sottoscrizioni di eventi, in quanto ciò potrebbe ridurre in modo significativo il numero di messaggi che un endpoint deve utilizzare. Per ulteriori informazioni, vedere [Filtro sottoscrizioni eventi](../../wf-api/general/event-subs-api.md#event).

## Perché l’API restituisce un codice di risposta ai conflitti 409?

Se tenti di creare una sottoscrizione evento e ricevi un codice di risposta: conflitto 409, la sottoscrizione che hai tentato di creare è un duplicato. Workfront non consente la creazione di abbonamenti duplicati.

## Cosa devo fare se i miei messaggi non vengono recapitati all&#39;endpoint?

Cerca i seguenti scenari e utilizza la soluzione consigliata:

* Verifica che l&#39;endpoint della sottoscrizione, definito dal campo **url**, restituisca un codice di risposta HTTP 2XX. In caso contrario, contattare il supporto tecnico Workfront o vedere [Requisiti di consegna dell&#39;abbonamento agli eventi](../../wf-api/general/setup-event-sub-endpoint.md).

* Timeout della richiesta di consegna dell’evento prima del completamento. Assicurati che l’endpoint risponda in modo coerente entro 5 secondi. Timeout predefinito impostato per la richiesta HTTP per la consegna di un messaggio di abbonamento agli eventi. Se l&#39;endpoint non risponde entro 5 secondi, contatta il supporto Workfront o vedi [Requisiti di consegna dell&#39;abbonamento agli eventi](../../wf-api/general/setup-event-sub-endpoint.md).
* Gli eventi potrebbero non generare il modo in cui pensi. Assicurati di non fare supposizioni su come e quando attivare gli eventi. Ad esempio, si potrebbe pensare che l&#39;aggiornamento di un documento su un&#39;attività generi un evento di aggiornamento dell&#39;attività, ma genera invece un evento di creazione o aggiornamento del documento.
* L’abbonamento potrebbe non essere configurato come previsto. Puoi creare sottoscrizioni di eventi in ambienti diversi e aspettarti che vengano trasferite come fanno gli altri dati di Workfront. Tuttavia, i dati di abbonamento agli eventi non sono configurati per essere copiati o promossi in altri ambienti. Assicurati di inviare richieste API all’ambiente corretto e che gli abbonamenti in tale ambiente siano configurati come previsto.
* Il payload non è stato ricevuto perché l&#39;indirizzo IP di Workfront necessario non è stato aggiunto al inserisco nell&#39;elenco Consentiti di sul firewall. Gli eventi di abbonamento agli eventi vengono inviati solo da alcuni indirizzi IP. Assicurati che la rete di destinazione disponga di tutte le eccezioni IP necessarie per ricevere payload da Workfront Event Subscriptions.
* Payload non ricevuto perché superiore a 1 MB. I messaggi o l&#39;oggetto di sottoscrizione degli eventi non possono superare 1 MB.

## Perché i miei messaggi richiedono un tempo eccessivo per raggiungere il mio endpoint?

Alcuni dei seguenti scenari potrebbero essere responsabili:

* Un’operazione di grandi dimensioni, ad esempio un aggiornamento in blocco, nel sistema può causare l’accodamento di un grande volume di messaggi in una sola volta, operazione che può richiedere un po’ di tempo.
* Calcoli a esecuzione prolungata o calcoli della sequenza temporale su progetti di grandi dimensioni potrebbero causare un ritardo nella pubblicazione dei messaggi alle sottoscrizioni di eventi da utilizzare.
* La sottoscrizione potrebbe essere stata disabilitata.

   * Dopo un periodo di tolleranza di 100 messaggi, se un particolare URL, che potrebbe essere associato a uno o più abbonamenti, genera un errore più del 70% del tempo o se l’URL non riesce a consegnare dopo 2.000 tentativi consecutivi, tutti i messaggi che corrispondono agli abbonamenti allo stesso URL non vengono tentati per la consegna. Al contrario, questi messaggi vengono immediatamente messi in coda per un nuovo tentativo.

     Ogni 10 minuti dopo la disabilitazione di un URL, tentiamo di inviare il messaggio successivo che arriva per l’elaborazione. Se il messaggio ha esito positivo, riattiviamo l’URL e successivamente tutti gli abbonamenti corrispondenti. Se l’invio del messaggio non riesce, il timer di 10 minuti viene ripristinato e riproviamo dopo la scadenza.

     Questo comportamento può essere percepito come una consegna incoerente o ritardata, ma si limita a seguire i nostri criteri per la gestione dei messaggi di abbonamento agli eventi.

   * Un URL di abbonamento a un evento verrà disabilitato se viene soddisfatta una delle seguenti condizioni:

      * L’URL dell’abbonamento non è stato consegnato per 7 giorni e ha avuto esito negativo in almeno 2.000 tentativi di consegna consecutivi nelle ultime 72 ore.
      * L’URL dell’abbonamento non è riuscito a fornire 50.000 tentativi consecutivi.

## Cosa devo fare se ricevo uno stato di risposta 500 quando tento di chiamare l’API di abbonamento agli eventi?

Contatta il supporto Workfront. Per informazioni su come contattare il supporto, vedere [Contattare l&#39;Assistenza clienti](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## Quali diversi tipi di autenticazione è possibile utilizzare con gli abbonamenti agli eventi di Workfront?

Puoi utilizzare qualsiasi autenticazione che utilizza un token Bearer. Il campo **authToken** di una sottoscrizione è una stringa che rappresenta un token Bearer OAuth2 utilizzato per l&#39;autenticazione con l&#39;URL specificato nel campo **url**. In teoria, questo valore di token potrebbe essere qualsiasi cosa, purché l&#39;endpoint di destinazione sia consapevole di come gestire la propria codifica, che è **utf-8**.

## Quanto tempo deve trascorrere prima che io riceva il payload dell’evento da Workfront Event Subscriptions?

In generale, puoi aspettarti di ricevere le richieste di consegna degli eventi di abbonamento agli eventi in meno di 5 secondi dalla registrazione della modifica dei dati. In media, le notifiche dei webhook vengono ricevute in meno di 1 secondo dal momento in cui viene apportata la modifica ai dati. Tuttavia, il servizio può ricevere messaggi in quantità talmente elevate da richiedere anche più tempo.

## Risorse aggiuntive

* **Documentazione API**: [API sottoscrizione evento](../../wf-api/general/event-subs-api.md)

* **Best practice**: [Best practice per l&#39;abbonamento agli eventi](../../wf-api/general/event-sub-best-practice.md)

* **Campi che attivano i payload della sottoscrizione eventi**: [Campi delle risorse della sottoscrizione eventi](../../wf-api/api/event-sub-resource-fields.md)

* **Informazioni sui nuovi tentativi di sottoscrizione eventi**: [Nuovi tentativi di sottoscrizione eventi](../../wf-api/api/event-sub-retries.md)

* **Configurazione del firewall per Workfront**: [Configurazione del inserisco nell&#39;elenco Consentiti di configurazione del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)
