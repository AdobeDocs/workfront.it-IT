---
content-type: api
navigation-topic: general-api
title: API sottoscrizione a eventi
description: API sottoscrizione a eventi
author: Becky
feature: Workfront API
role: Developer
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: 3afa0fbfb8a82a7dc1a2e9c65d04aa1be7b6f1f8
workflow-type: tm+mt
source-wordcount: '3190'
ht-degree: 97%

---


# API sottoscrizione a eventi

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

Quando si verifica un’azione su un oggetto Adobe Workfront supportato dalle sottoscrizioni a eventi, puoi configurare Workfront per inviare una risposta all’endpoint desiderato. Ciò significa che le applicazioni di terze parti possono ricevere aggiornamenti dalle interazioni Workfront tramite l’API Workfront subito dopo che si verificano. In generale, puoi aspettarti di ricevere le notifiche del webhook in meno di 5 secondi dalla registrazione della modifica dei dati. In media, le notifiche dei webhook vengono ricevute in meno di 1 secondo dalla registrazione della modifica dei dati.

Poiché le sottoscrizioni a eventi inviano dati a un altro servizio, vengono gestite tramite comandi anziché tramite l’applicazione Workfront.

Per ricevere i payload delle sottoscrizioni a eventi tramite il firewall, devi aggiungere i seguenti indirizzi IP nell’elenco Consentiti:

**Per clienti in Europa:**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**Per clienti in località diverse dall’Europa:**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

I seguenti argomenti supportano l’API di sottoscrizione a eventi:

## Oggetti supportati dalle sottoscrizioni a eventi

I seguenti oggetti Workfront sono supportati dalle sottoscrizioni a eventi.

* Approvazione
* Fase di approvazione
* Fase di approvazione del partecipante
* Assegnazione
* Azienda
* Dashboard
* Documento
* Versione documento
* Spesa
* Campo
* Ora
* Problema
* Nota
* Portfolio
* Programma
* Progetto
* Approvazione bozza
* Record
* Tipo di record
* Rapporto
* Piano per gestione del personale
* Valore parametro del piano per gestione del personale
* Risorse del piano per gestione del personale
* Valore attributo risorsa del piano per gestione del personale
* Impostazione valore attributo risorsa del piano per gestione del personale
* Valore parametro risorsa del piano per gestione del personale
* Attività
* Modello
* Scheda orario
* Utente
* Area di lavoro

>[!NOTE]
>
>Per un elenco dei campi supportati dagli oggetti di sottoscrizione a eventi, consulta [Campi delle risorse di sottoscrizione a eventi](../../wf-api/api/event-sub-resource-fields.md).

## Autenticazione della sottoscrizione a eventi

Per creare, eseguire query o eliminare una sottoscrizione evento, l’utente di Workfront necessita dei seguenti elementi:

* Un livello di accesso “Amministratore di sistema” per utilizzare le sottoscrizioni a eventi.
* Un’intestazione `sessionID` per utilizzare l’API sottoscrizione a eventi

  Per ulteriori informazioni, consulta [Autenticazione](api-basics.md#authentication) in [Nozioni di base sulle API](api-basics.md).

## Evitare il sovraccarico delle sottoscrizioni a eventi

Il servizio di sottoscrizione a eventi è progettato per fornire una consegna affidabile di eventi a tutti gli utenti. A tal fine, sono state introdotte misure di protezione per impedire la produzione eccessiva di eventi da parte di un singolo utente, che potrebbero causare potenziali problemi di qualità del servizio per tutti gli altri. Di conseguenza, un utente che produce troppi eventi a una frequenza elevata in un breve arco di tempo, potrebbe subire sandboxing e ritardi nella consegna degli eventi.

## Creazione della risorsa di sottoscrizione

La risorsa di sottoscrizione contiene i campi seguenti.

* objId (facoltativo)

   * **Stringa**: ID dell’oggetto objCode specificato per il quale vengono attivati gli eventi. Se questo campo non è specificato, l’utente riceve eventi per tutti gli oggetti del tipo specificato.

* objCode (obbligatorio)

   * **Stringa**: l’objCode dell’oggetto sottoscritto per le modifiche. I valori possibili per objCode sono elencati nella tabella seguente.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <thead> 
       <tr> 
        <th><p>Oggetto</p></th> 
        <th><p>objCode</p></th> 
       </tr> 
      </thead> 
      <tbody> 
       <tr> 
        <td scope="col">Approvazione</td> 
        <td scope="col"><p>approvazione</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Fase di approvazione</td> 
        <td scope="col"><p>approval_stage</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Fase di approvazione del partecipante</td> 
        <td scope="col"><p>approval_stage_participant</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Assegnazione</td> 
        <td scope="col"><p>ASSGN</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Azienda </td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Dashboard</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Documento</p></td> 
        <td scope="col">DOCU </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Versione documento</p></td> 
        <td scope="col">DOCV </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Spesa</p></td> 
        <td scope="col">EXPNS</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Campo</p></td> 
        <td scope="col"><p>CAMPO</p></td> 
       </tr> 
      <tr> 
        <td scope="col"><p>Ora</p></td> 
        <td scope="col">HOUR</td> 
       </tr> 
       <tr> 
        <td scope="col">Problema</td> 
        <td scope="col"><p>OPTASK</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Nota</td> 
        <td scope="col">NOTA</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Portfolio</p></td> 
        <td scope="col"><p>PORT</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Programma</p></td> 
        <td scope="col"><p>PRGM</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Progetto</p></td> 
        <td scope="col"><p>PROJ</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Approvazione bozza</p></td> 
        <td scope="col"><p>PRFAPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Record</p></td> 
        <td scope="col"><p>RECORD</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Tipo di record</p></td> 
        <td scope="col"><p>RECORD_TYPE</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Rapporto</p></td> 
        <td scope="col"><p>PTLSEC</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Piano per gestione del personale</p></td> 
        <td scope="col"><p>STAFFP</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Valore parametro del piano per gestione del personale</p></td> 
        <td scope="col"><p>SPVAL</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Risorse del piano per gestione del personale</p></td> 
        <td scope="col"><p>STAFFR</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Valore attributo risorsa del piano per gestione del personale</p></td> 
        <td scope="col"><p>SPAVAL</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Impostazione valore attributo risorsa del piano per gestione del personale</p></td> 
        <td scope="col"><p>SAVSET</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Valore parametro risorsa del piano per gestione del personale</p></td> 
        <td scope="col"><p>SRPVAL</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Attività</p></td> 
        <td scope="col"><p>ATTIVITÀ</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Modello</p></td> 
        <td scope="col"><p>TMPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Scheda orario</td> 
        <td scope="col">TSHET</td> 
       </tr> 
       <tr> 
        <td scope="col">Utente</td> 
        <td scope="col">UTENTE</td> 
       </tr> 
       <tr> 
        <td scope="col">Area di lavoro</td> 
        <td scope="col">AREA DI LAVORO</td> 
       </tr> 
      </tbody> 
     </table>

* eventType (obbligatorio)

   * **Stringa**: un valore che rappresenta il tipo di evento a cui l’oggetto è sottoscritto. I tipi di evento disponibili includono:

      * CREATE
      * DELETE
      * UPDATE

* URL (obbligatorio)

   * **Stringa**: URL dell’endpoint a cui vengono inviati i payload degli eventi di sottoscrizione tramite HTTP.

* authToken (obbligatorio)

   * **Stringa**: il token Bearer OAuth2 utilizzato per l’autenticazione con l’URL specificato nel campo “URL”.

## Creazione di richieste API per la sottoscrizione a eventi

Dopo aver verificato che l’utente disponga dell’accesso come amministratore e aver creato la risorsa di sottoscrizione, puoi creare le sottoscrizioni a eventi.

Utilizza la sintassi seguente per creare l’URL.

**URL richiesta**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Intestazioni richiesta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nome intestazione</p> </th> 
   <th> <p>Valore intestazione</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tipo di contenuto</p> </td> 
   <td> <p>applicazione/JSON</p> </td> 
  </tr> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>valore sessionID</p> </td> 
  </tr> 
 </tbody> 
</table>

**Esempio di corpo della richiesta:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua",
                "authToken": "EauthTokenWorkfrontRocks1234_"
            }
```

**Esempio di corpo della risposta**

```
{
    "id": <NEW SUBSCRIPTION ID>,
    "version": <NEW SUBSCRIPTION VERSION>
}
```

| Codice di risposta | Descrizione |
|---|---|
| 201 (creato) | La sottoscrizione a eventi è stata creata correttamente. |
| 400 (richiesta non valida) | Il campo URL della risorsa della sottoscrizione è stato ritenuto non valido. |
| 401 (non autorizzato) | Il sessionID fornito era vuoto o ritenuto non valido. |
| 403 (non consentito) | L’utente che corrisponde al sessionID fornito non dispone dell’accesso come amministratore. |

Il passaggio di una risorsa della sottoscrizione come corpo di una richiesta (con il tipo di contenuto “applicazione/JSON”) determina la creazione di una sottoscrizione evento per l’oggetto specificato. Il codice di risposta 201 (creato) indica che la sottoscrizione è stata creata. Un codice di risposta diverso da 201 indica che la sottoscrizione **NON** è stata creata.

>[!NOTE]
>
> L’intestazione di risposta “Posizione” contiene l’URI della sottoscrizione evento appena creata.

**Esempio di intestazioni di risposta:**

| Intestazioni di risposta | Esempio |
|---|---|
| Lunghezza del contenuto | `→0` |
| Data | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| Posizione | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| Server | `→Apache-Coyote/1.1` |

## Query delle sottoscrizioni a eventi

Quando esegui una query su HTTP di Workfront, utilizza il metodo GET. Esistono due modi per eseguire query per le sottoscrizioni a eventi: eseguire query per ID sottoscrizione (vedi sotto) o eseguire query per tutte le sottoscrizioni a eventi.

### Eseguire query per tutte le sottoscrizioni a eventi

Puoi eseguire una query per tutte le sottoscrizioni a eventi per un cliente oppure utilizzare quanto segue per gestire la risposta. Per gestire la risposta, puoi inoltre utilizzare le seguenti opzioni:

* **page**: opzione del parametro query per specificare il numero di pagine da restituire. Il valore predefinito è 1.
* **limit**: opzione del parametro query per specificare il numero di risultati da restituire per pagina. Il valore predefinito è 100 con un massimo di 1000.

La sintassi della richiesta per elencare tutte le sottoscrizioni a eventi per un cliente specifico è la seguente:

**URL richiesta**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Intestazioni richiesta:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nome intestazione</p> </th> 
   <th> <p>Valore intestazione</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>valore sessionID</p> </td> 
  </tr> 
 </tbody> 
</table>

**Codici di risposta**

| Codice di risposta | Descrizione |
|---|---|
| 200 (OK) | La richiesta restituita con tutte le sottoscrizioni a eventi trovate per il cliente che corrispondono al sessionID fornito. |
| 401 (non autorizzato) | Il valore sessionID fornito era vuoto. |
| 403 (non consentito) | L’utente, che corrisponde al sessionID fornito, non dispone dell’accesso come amministratore. |


**Esempio di intestazioni di risposta**

| Intestazione risposta | Esempio |
|---|---|
| Tipo di contenuto | `→application/json;charset=UTF-8` |
| Data | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| Server | `→Apache-Coyote/1.1` |
| Codifica di trasferimento | `→chunked` |


**Esempio di corpo della risposta**

```
{
    "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
    "date_created": "2024-04-11T17:10:10.305981",
    "date_modified": "2024-04-11T17:10:10.305981",
    "version": "v2",
    "dateVersionUpdated": "2025-01-15T04:04:04.407945"
    "customerId": "504f9640000013401be513579fbebffa",
    "objId": null,
    "objCode": "PROJ",
    "url": "http://requestb.in/ua5hi2ua",
    "eventType": "UPDATE",
    "authToken": "authTokenWorkfrontRocks1234_"
    "subscription_url": {
        "url": "http://requestb.in/ua5hi2ua",
        "date_created": "2024-04-11T15:56:14.169489",
        "successes": 11,
        "failures": 2,
        "disabled_at": null,
        "frozen_at": null
   }
}
```

Dove

* **pagina** e **limite** sono i valori forniti nella richiesta o il valore predefinito se non vengono forniti valori
* **conteggio_pagine** è il numero totale di pagine che è possibile interrogare.
* **conteggio_totale** è il numero totale di sottoscrizioni corrispondenti alla query.

### Eseguire una query in base all’ID sottoscrizione eventi

Puoi eseguire una query per le sottoscrizioni eventi in base all’ID della sottoscrizione eventi. La sintassi della richiesta per l’elenco delle sottoscrizioni eventi è la seguente:

**URL richiesta**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Intestazioni richiesta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nome intestazione</p> </th> 
   <th> <p>Valore intestazione</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>valore sessionID</p> </td> 
  </tr> 
 </tbody> 
</table>

**Codici di risposta**

| Codice di risposta | Descrizione |
|---|---|
| 200 (OK) | La richiesta restituita con la sottoscrizione eventi corrispondente all’ID sottoscrizione fornito. |
| 401 (non autorizzato) | Il valore sessionID fornito era vuoto. |
| 403 (non consentito) | L’utente, che corrisponde al sessionID fornito, non dispone dell’accesso come amministratore. |


**Esempio di corpo della risposta**



```
{
    "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
    "date_created": "2024-04-11T17:10:10.305981",
    "date_modified": "2024-04-11T17:10:10.305981",
    "version": "v2",
    "dateVersionUpdated": "2025-01-15T04:04:04.407945"
    "customerId": "504f9640000013401be513579fbebffa",
    "objId": null,
    "objCode": "PROJ",
    "url": "http://requestb.in/ua5hi2ua",
    "eventType": "UPDATE",
    "authToken": "authTokenWorkfrontRocks1234_"
    "subscription_url": {
        "url": "http://requestb.in/ua5hi2ua",
        "date_created": "2024-04-11T15:56:14.169489",
        "successes": 11,
        "failures": 2,
        "disabled_at": null,
        "frozen_at": null
   }
}
```


## Controllo delle versioni di sottoscrizione eventi

Workfront dispone di due versioni di sottoscrizioni eventi.

La possibilità di aggiornare o eseguire il downgrade delle sottoscrizioni eventi assicura che, quando vengono apportate modifiche alla struttura degli eventi, le sottoscrizioni esistenti non vengano interrotte, consentendo di testarle e aggiornarle alla nuova versione senza interruzioni nella sottoscrizione eventi.

Per ulteriori informazioni sul controllo delle versioni di sottoscrizione eventi, incluse le differenze specifiche tra la versione e le date importanti, consulta [Controllo delle versioni della sottoscrizione eventi](/help/quicksilver/wf-api/general/event-subs-versioning.md).

>[!NOTE]
>
>Quando aggiorni o esegui il downgrade della sottoscrizione eventi a un’altra versione, ricevi eventi duplicati per ogni consegna di eventi per una finestra di cinque minuti dopo la modifica della versione. I duplicati includono una versione 1 e versione 2 per ogni iscrizione eventi. Ciò garantisce che non si perdano eventi a causa della modifica della versione dell’iscrizione eventi.

### Modifica della versione di un’iscrizione singola

La sintassi della richiesta per modificare la versione di una singola sottoscrizione è la seguente:

**URL richiesta**

```
PUT https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>/version 
```

**Corpo della richiesta di esempioi**

```
{
    "version": "v2" 
}
```


**Corpo della risposta di esempio (200)**

```
{
    "id": <SUBSCRIPTION ID>,
    "version": "v2" 
}
```

**Codici di risposta possibili**

* 200
* 400
* 404


### Modifica di più versioni di sottoscrizioni

Questo endpoint modifica la versione di più sottoscrizioni, in base all’elenco delle sottoscrizioni o al flag di tutte le sottoscrizioni del cliente.

La sintassi della richiesta per modificare la versione di una singola sottoscrizione è la seguente:

**URL richiesta**

```
PUT https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/version
```

**Corpi della richiesta di esempio**

* Corpo della richiesta dell’elenco di sottoscrizioni

  ```
  {
      "subscriptionIds": [<SUBSCRIPTION ID 1>, <SUBSCRIPTION ID 2>],
      "version": "v2" 
  }
  ```

* Corpo della richiesta per tutte le sottoscrizioni del cliente

  ```
  {
      "allCustomerSubscriptions": true,
      "version": "v2" 
  }
  ```

**Esempio di corpo della risposta (200)**

```
{
    "subscription_ids": [<SUBSCRIPTION ID 1>, <SUBSCRIPTION ID 2>, ...],
    "version": "v2" 
}
```

**Codici di risposta possibili**

* 200
* 400

## Conferma della sottoscrizione a eventi

Puoi utilizzare il filtro della sottoscrizione a eventi per assicurarti di ricevere solo messaggi pertinenti. La creazione di filtri per le sottoscrizioni può ridurre in modo significativo il numero di messaggi che l’endpoint deve utilizzare.

Ad esempio, puoi impostare una sottoscrizione all’evento **UPDATE - TASK** in modo che si attivi solo quando il **newState** del payload di un evento definisce il **taskStatus** come **current**.

>[!IMPORTANT]
>
>I seguenti attributi vengono applicati al filtro della sottoscrizione eventi

* Quando un campo filtro contiene un valore non vuoto, solo i messaggi con un **newState** contenente le chiavi e i valori del filtro vengono inviati all’URL sottoscritto
* Puoi filtrare in base ai dati personalizzati inclusi in **newState** E/O **oldState** dell’oggetto
* I filtri vengono valutati solo a seconda che siano uguali o meno a un valore specifico
* Se la sintassi del filtro non è corretta o non corrisponde ad alcun dato contenuto nel **newState** del payload, non verrà restituito un messaggio di convalida per indicare che si è verificato un errore
* Non è possibile aggiornare i filtri di una sottoscrizione esistente; è necessario creare una nuova sottoscrizione con nuovi parametri di filtro.
* È possibile applicare più filtri a una singola sottoscrizione e la sottoscrizione verrà consegnata solo quando sono state soddisfatte tutte le condizioni del filtro.
* L’applicazione di più filtri a una singola sottoscrizione equivale a utilizzare un operatore logico **AND**.
* È possibile applicare più sottoscrizioni a eventi a un singolo oggetto, a condizione che uno o più parametri dei campi della sottoscrizione siano diversi tra tutte le sottoscrizioni.
* Quando a un singolo oggetto vengono assegnate più sottoscrizioni a eventi, tutte le sottoscrizioni a eventi associate a tale oggetto possono essere restituite a un singolo endpoint. Questa pratica può essere utilizzata come sostituto equivalente dell’operatore logico **OR** che non può essere impostato utilizzando i parametri di filtro.
* I seguenti campi non sono filtrabili:

   * DOCU.groups
   * RECORD.data
   * RECORD_TYPE.data
   * RECORD_TYPE.fields

### Utilizzo degli operatori di confronto

Puoi specificare un campo di confronto insieme al campo di filtro. Utilizza un operatore di confronto in questo campo per filtrare i risultati comparativi. Ad esempio, puoi creare una sottoscrizione UPDATE - TASK che invia un payload solo se lo stato dell’attività NON è uguale a current. Puoi utilizzare i seguenti operatori di confronto:

#### eq: equal (uguale)

Questo filtro consente la trasmissione dei messaggi se la modifica avvenuta corrisponde esattamente al `fieldValue` nel filtro. Il valore `fieldValue` fa distinzione tra maiuscole e minuscole.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "eq"
        }
    ]
}
```

#### ne: not equal (non uguale a)

Questo filtro consente la trasmissione dei messaggi se la modifica avvenuta non corrisponde esattamente al `fieldValue` nel filtro. Il valore `fieldValue` fa distinzione tra maiuscole e minuscole.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "ne"
        }
    ]
}
```

#### gt: greater than (maggiore di)

Questo filtro consente la trasmissione dei messaggi se l’aggiornamento per `fieldName` specificato è maggiore del valore per `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gt"
        }
    ]
}
```

#### gte: greater than or equal to (maggiore di o uguale a)

Questo filtro consente la trasmissione dei messaggi se l’aggiornamento per `fieldName` specificato è maggiore o uguale al valore per `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gte"
        }
    ]
}
```

#### lt: less than (minore di)

Questo filtro consente la trasmissione dei messaggi se l’aggiornamento per `fieldName` specificato è minore del valore per `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lt"
        }
    ]
}
```

#### lte: less than or equal to (minore di o uguale a)

Questo filtro consente la trasmissione dei messaggi se l’aggiornamento per `fieldName` specificato è minore o uguale al valore per `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lte"
        }
    ]
}
```

#### contiene

Questo filtro consente la trasmissione dei messaggi se la modifica avvenuta contiene il `fieldValue` nel filtro. Il valore `fieldValue` fa distinzione tra maiuscole e minuscole.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        }
    ]
}
```

#### containsOnly

Questo filtro consente la trasmissione dei messaggi solo quando l’intero set di valori selezionati corrisponde esattamente al valore fieldValue nel filtro, indipendentemente dall’ordine. Non devono essere presenti valori aggiuntivi o mancanti.

>[!NOTE]
>
>Questo è utilizzato per campi di tipo array (a selezione multipla). L’esempio di sottoscrizione di seguito consente la trasmissione dei messaggi solo quando il campo `groups` contiene esattamente “Scelta 3” e “Scelta 4”, senza valori aggiuntivi o mancanti e indipendentemente dall’ordine. Se in `fieldValue` è specificata una stringa o un numero intero anziché un array, la sottoscrizione consente la trasmissione dei messaggi solo quando il campo `groups` contiene esattamente un’opzione e tale opzione corrisponde esattamente alla stringa o al numero intero specificato in `fieldValue`”


```
{
    "objCode": "PROJ",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedProjects",
    "filters": [
        {
            "fieldName": "groups",
            "fieldValue": [
                "Choice 3",
                "Choice 4"
            ],
            "state": "newState",
            "comparison": "containsOnly"
        }
    ]
}
```

#### notContains

Questo filtro consente la trasmissione dei messaggi solo quando il campo specificato (`fieldName`) non contiene il valore specificato (`fieldValue`).

>[!NOTE]
>
>È utilizzato per campi di tipo array (a selezione multipla) o stringa. Se il campo è una stringa, verrà controllato che il valore specificato non sia contenuto nella stringa (ad esempio, “Nuovo” non è nella stringa “Progetto - Aggiornato”). Se il campo è un array e il valore di campo specificato è una stringa o un numero intero, verrà controllato che l’array non contenga il valore specificato (ad esempio, “Scelta 1” non in [“Scelta 2”, “Scelta 3”]). L’esempio di sottoscrizione seguente consente la trasmissione dei messaggi solo quando i campi `groups` non contengono la stringa “Gruppo 2”.

```
{
    "objCode": "PROJ",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedProjects",
    "filters": [
        {
            "fieldName": "groups",
            "fieldValue": "Group 2",
            "state": "newState",
            "comparison": "notContains"
        }
    ]
}
```

#### change

Questo filtro consente la trasmissione dei messaggi solo se nel campo specificato (`fieldName`) è presente un valore diverso in oldstate e newstate. L’aggiornamento di altri campi oltre a quello specificato (`fieldName`) non restituirà la modifica.

>[!NOTE]
>
>`fieldValue` nell’array di filtri seguente non ha alcun effetto.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "",
            "comparison": "changed"
        }
    ]
}
```

#### state

Questo connettore applica il filtro al nuovo stato o allo stato precedente dell’oggetto creato o aggiornato. Questo è utile quando si desidera sapere dove è stata effettuata una modifica da un valore a un altro.
`oldState` non è possibile in CREATE `eventTypes`.

>[!NOTE]
>
>La sottoscrizione seguente con il filtro specificato restituirà solo i messaggi in cui il nome dell’attività contiene `again` per `oldState`, ovvero come era prima che venisse effettuato un aggiornamento dell’attività.
>Un caso d’uso potrebbe essere quello di trovare i messaggi objCode che sono cambiati da un valore a un altro. Ad esempio, per individuare tutte le attività modificate da “Cerca nome” a “Cerca nome team”

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains",
            "state": "oldState"
        }
    ]
}
```

### Utilizzo di filtri nidificati

La sottoscrizione a eventi supporta il filtro sui campi nidificati degli eventi utilizzando i nomi dei campi nidificati. Ad esempio, per filtrare un messaggio in cui `newState.data.customField1 = 'myCustomFieldValue'`, è possibile creare la seguente sottoscrizione con filtro:

```
{
    "objCode": "RECORD",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedRecords",
    "filters": [
        {
            "fieldName": "data",
            "fieldValue": {
                    "customField1": "myCustomFieldValue"
            },
            "comparison": "eq",
            "state": "newState"
        }
    ]
}
```

È possibile gestire anche i filtri nidificati due volte.

```
"filters": [
    {
        "fieldName": "data",
        "fieldValue": {
            "fields": {
                "children": {
                    "customerId":"customer1234",
                    "name":"New Campaign"
                }
            }
        },
        "comparison": "eq",
        "state": "newState"
    }
],
"filterConnector": 'AND'
```


#### Prestazioni e limiti

Per garantire prestazioni e manutenibilità coerenti:

* Ogni sottoscrizione supporta fino a 10 gruppi di filtri (ogni gruppo contiene più filtri).
* Ogni gruppo di filtri può includere fino a 5 filtri per evitare un potenziale deterioramento delle prestazioni durante l’elaborazione degli eventi.
* È supportato un massimo di 10 gruppi di filtri (ciascuno con 5 filtri), ma un numero elevato di abbonamenti attivi con logica di filtro complessa potrebbe causare un ritardo durante la valutazione dell’evento.

Se superi questi limiti, prova a semplificare la logica o a suddividere l’abbonamento in più limiti più piccoli.

### Utilizzo dei campi del connettore

Il campo `filterConnector` nel payload della sottoscrizione ti consente di scegliere come applicare i filtri. Il valore predefinito è “AND”, dove i filtri devono essere tutti `true` affinché il messaggio della sottoscrizione venga trasmesso. Se viene specificato “OR”, affinché il messaggio di sottoscrizione venga trasmesso è necessario che solo uno dei filtri corrisponda.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        },
        {
            "fieldName": "name",
            "fieldValue": "also",
            "comparison": "contains"
        }
    ],
    "filterConnector": "AND"
}
```

### Utilizzo dei gruppi di filtri

I gruppi di filtri ti consentono di creare condizioni logiche (AND/OR) nidificate all’interno dei filtri di sottoscrizione a eventi.

Ciascun gruppo di filtri può avere i seguenti elementi:

* Il proprio connettore (AND o OR).
* Più filtri, ciascuno dei quali segue la stessa sintassi e lo stesso comportamento dei filtri autonomi.

>[!IMPORTANT]
>
>Un gruppo deve avere almeno 2 filtri.


Tutti i filtri all’interno di un gruppo supportano quanto segue:

* Operatori di confronto: eq, ne, gt, gte, lt, lte, contains, notContains, containsOnly, changed.
* Opzioni stato: newState, oldState.
* Targeting del campo: qualsiasi nome di campo oggetto valido.

```
{
  "objCode": "TASK",
  "eventType": "UPDATE",
  "authToken": "token",
  "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
  "filters": [
    {
      "fieldName": "percentComplete",
      "fieldValue": "100",
      "comparison": "lt"
    },
    {
      "type": "group",
      "connector": "OR",
      "filters": [
        {
          "fieldName": "status",
          "fieldValue": "CUR",
          "comparison": "eq"
        },
        {
          "fieldName": "priority",
          "fieldValue": "1",
          "comparison": "eq"
        }
      ]
    }
  ],
  "filterConnector": "AND"
}
```

L’esempio precedente contiene i seguenti componenti:

1. Filtro del livello principale (esterno al gruppo):

   * `{ "fieldName": "percentComplete", "fieldValue": "100", "comparison": "lt" }`
   * Questo filtro controlla se il campo percentComplete dell’attività aggiornata è inferiore a 100.

1. Gruppo di filtri (filtri nidificati con OR):

   * `{ "type": "group", "connector": "OR", "filters": [ { "fieldName": "status", "fieldValue": "CUR", "comparison": "eq" }, { "fieldName": "priority", "fieldValue": "1", "comparison": "eq" } ] }`
   * Questo gruppo valuta due filtri interni:

      * Il primo controlla se lo stato dell’attività è uguale a “CUR” (corrente).
      * Il secondo controlla se la priorità è uguale a “1” (priorità alta).
   * Poiché il connettore è “OR”, questo gruppo passerà se una delle due condizioni è vera.

1. Connettore del livello principale (filterConnector: AND):
   * Il connettore più esterno tra i filtri di livello superiore è “AND”. Questo significa che sia il filtro del livello principale che il gruppo devono passare affinché l’evento corrisponda.

1. La sottoscrizione viene attivata quando vengono soddisfatte le seguenti condizioni:
   * La percentComplete è inferiore a 100.
   * Lo stato è “CUR” oppure la priorità è uguale a “1”.

>[!NOTE]
>
>Esistono dei limiti per garantire prestazioni di sistema coerenti quando si utilizzano i gruppi di filtri, tra cui:
>
>* Ogni sottoscrizione supporta fino a 10 gruppi di filtri (ogni gruppo contiene più filtri).
>* Ogni gruppo di filtri può includere fino a 5 filtri per evitare un potenziale deterioramento delle prestazioni durante l’elaborazione degli eventi.
>* Pur disponendo di un massimo di 10 gruppi di filtri (ciascuno con 5 filtri), un numero elevato di sottoscrizioni attive con logica di filtro complessa può causare un ritardo durante la valutazione dell’evento.

## Eliminazione di sottoscrizioni eventi

Durante l’eliminazione di HTTP di Workfront, utilizza il metodo DELETE. La sintassi della richiesta per l’eliminazione di una singola sottoscrizione eventi per ID sottoscrizione è la seguente:

**URL richiesta:**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Intestazioni richiesta:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nome intestazione</p> </th> 
   <th> <p>Valore intestazione</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> valore sessionID </p> </td> 
  </tr> 
 </tbody> 
</table>

**Codici di risposta:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Codice di risposta</p> </th> 
   <th> Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (nessun contenuto)</td> 
   <td>Il server ha rimosso correttamente la sottoscrizione eventi corrispondente al subscriptionID fornito.</td> 
  </tr> 
  <tr> 
   <td>401 (non autorizzato)</td> 
   <td>Il valore sessionID fornito era vuoto.</td> 
  </tr> 
  <tr> 
   <td>403 (non consentito)</td> 
   <td>L’utente che corrisponde al sessionID fornito non dispone dell’accesso come amministratore.</td> 
  </tr> 
  <tr> 
   <td>404 (Non trovato)</td> 
   <td>Il server non è stato in grado di trovare una sottoscrizione eventi corrispondente al subscriptionID fornito per l’eliminazione.</td> 
  </tr> 
 </tbody> 
</table>

**Esempio di intestazioni di risposta:**

| Intestazione risposta | Esempio |
|---|---|
| Data | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| Server | `→Apache-Coyote/1.1` |


**Esempio di corpo della risposta:** N/D

## Esempi di payload di eventi

Il payload che un utente riceve varia a seconda del tipo di oggetto, ma esiste un formato coerente per il quale vengono consegnati i payload variabili.

Ad esempio, le seguenti proprietà rimangono coerenti in tutti i payload evento:

* eventType
* subscriptionId
* oldState
* newState
* eventTime

Sebbene coerenti nel formato, i valori contenuti all’interno delle proprietà variano tra oggetti e tipi di oggetto diversi.

Di seguito vengono visualizzati esempi di payload per un evento UPDATE e un evento CREATE. Nell’esempio UPDATE gli oggetti oldState e newState sono gli stessi, mentre nell’esempio CREATE l’oggetto oldState è vuoto (non NULL).

Di seguito è riportato un payload di esempio per un evento UPDATE:

<!-- [Copy](javascript:void(0);) -->

```
{
                  "eventType": "UPDATE",
                   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                   "eventTime": {
                       "nano": 998000000,
                       "epochSecond": 1507319336
                   },
                   "eventVersion": "v2",
                   "subscriptionVersion": "v2",
                   "newState": {
                "ID": "59d7ddf7000002322d791eb08bafddfb", 
                       "name": "EventSub Test updated",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:56.980-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,       "categoryID": null,
                      "status": "CUR",
                      "parameterValues": {}
                   },
                   "oldState": {
                       "ID": "59d7ddf7000002322d791eb08bafddfb",
                       "name": "EventSub Test 180fd595-63fb-4fa9-bd47-58bf6e53d964",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:07.792-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,<
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,
                       "categoryID": null,
                       "status": "CUR",
                       "parameterValues": {}
                   }
                }
```

Di seguito è riportato un payload di esempio per un evento CREATE:

<!-- [Copy](javascript:void(0);) -->

```
{
                "eventType": "CREATE",
                "subscriptionId": "4028e3815ebf03a7015ebfa53b6d0002",
                "eventTime": {
                "nano": 232000000,
                "epochSecond": 1506453831
                },
                "eventVersion": "v2",
                "subscriptionVersion": "v2",
                "newState": {
                "ID": "59caa946000000e07b0afc3383230c67",
                "name": "EventSub Test fe16d470-0a40-4290-92f4-6a0389fb536c",
                "objCode": "PROJ",
                "entryDate": "2017-09-26T13:23:50.746-0600",
                "accessorIDs": ["544820df0000142362741fc0c368de19"],
                "lastUpdateDate": "2017-09-26T13:23:50.927-0600",
                "groupID": "544820df0000140f6a9c1faa7cacadd3",
                "sponsorID": null,
                "description": null,
                "plannedCompletionDate": "2017-09-26T09:00:00.000-0600",
                "enteredByID": "544820df0000142362741fc0c368de19",
                "ownerID": "544820df0000142362741fc0c368de19",
                "templateID": null,
                "priority": 0,
                "companyID": null,
                "portfolioID": null,
                "referenceNumber": 1750,
                "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                "customerID": "544820df0000135b7719dcca654391f6",
                "currency": null,
                "categoryID": null,
                "status": "CUR",
                "parameterValues": {}
                },
                "oldState": {}
            }
```

## Codifica Base 64

Se una sottoscrizione eventi viene rifiutata a causa di un conflitto tra i caratteri speciali contenuti nelle sottoscrizioni eventi e le impostazioni di rete, puoi utilizzare la codifica Base64 per trasmettere le sottoscrizioni eventi. Base64 è un insieme di schemi di codifica in grado di tradurre qualsiasi dato arbitrario in un formato di stringa ASCII. È importante notare che Base64 non è una forma di crittografia di sicurezza.

### Campo di codifica Base 64

Il campo base64Encoding è facoltativo, utilizzato per abilitare la codifica Base64 dei payload di sottoscrizione agli eventi. Il valore predefinito è falso e i valori possibili sono: vero, falso e “ ” (vuoto).

### Esempio di richiesta tramite il campo base64Encoding

Se viene effettuata una richiesta utilizzando il campo base64Encoding impostato su vero, gli oggetti **newState** e **oldState** nel payload vengono consegnati come stringhe di codifica base 64. Se il campo base64Encoding è impostato su falso, lasciato vuoto o non incluso nella richiesta, il payload restituito non verrà codificato in base 64.

Di seguito è riportato un esempio di richiesta che utilizza il campo base64Encoding:

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua"",
                "authToken": "EauthTokenWorkfrontRocks1234_",
                "base64Encoding": "true"
            }
```

### Esempi di payload di risposta con codifica base 64

<!-- [Copy](javascript:void(0);) -->

```
                {
                "eventType": "UPDATE",
                "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                "eventTime": {
                "nano": 998000000,
                "epochSecond": 1507319336
                },
                "eventVersion": "v2",
                "subscriptionVersion": "v2",
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## Metodo obsoleto per la query di tutte le sottoscrizioni di eventi

Il seguente endpoint API è obsoleto e non deve essere utilizzato per le nuove implementazioni. È inoltre consigliabile eseguire la transizione delle implementazioni precedenti al metodo nella sezione **Query delle sottoscrizioni di eventi** descritta sopra.

Puoi eseguire una query su tutte le sottoscrizioni di eventi per un cliente come specificato dal valore sessionID. La sintassi della richiesta per elencare tutte le sottoscrizioni di eventi per un cliente specifico è il seguente URL:

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**Intestazioni richiesta:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nome intestazione</p> </th> 
   <th> <p>Valore intestazione</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> valore sessionID </p> </td> 
  </tr> 
 </tbody> 
</table>

**Codici di risposta:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Codice di risposta</p> </th> 
   <th> Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (nessun contenuto)</td> 
   <td>La richiesta ha correttamente restituito tutte le sottoscrizioni di eventi trovate per l’utente.</td> 
  </tr> 
  <tr> 
   <td>401 (non autorizzato)</td> 
   <td>Il valore sessionID fornito era vuoto.</td> 
  </tr> 
  <tr> 
   <td>403 (non consentito)</td> 
   <td>L’utente che corrisponde al valore sessionID fornito non dispone dell’accesso di amministratore.</td> 
  </tr> 
 </tbody> 
</table>



### Esempio di corpo della risposta

<!-- [Copy](javascript:void(0);) -->

```
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customer_id": "504f9640000013401be513579fbebffa",
                "obj_id": "ObjId1234",
                "obj_code": "TASK",
                "url": "http://test.test.net/test/1234",
                "event_type": "UPDATE",
                "auth_token": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customer_d": "504f9640000013401be513579fbebffa",
                "obj_id": null,
                "obj_code": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "event_type": "UPDATE",
                "auth_token": "authTokenWorkfrontRocks1234_"
                }                
                ]
```
