---
content-type: api
navigation-topic: general-api
title: API di abbonamento agli eventi
description: API di abbonamento agli eventi
author: Becky
feature: Workfront API
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: e06f6e8ca40da6741982b4ed8c5c53bdbfb253ca
workflow-type: tm+mt
source-wordcount: '2109'
ht-degree: 3%

---


# API di abbonamento agli eventi

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

Quando si verifica un&#39;azione su un oggetto Adobe Workfront supportato dalle sottoscrizioni di eventi, puoi configurare Workfront per inviare una risposta all&#39;endpoint desiderato. Ciò significa che le applicazioni di terze parti possono ricevere aggiornamenti dalle interazioni Workfront tramite l’API Workfront subito dopo che si verificano. In generale, puoi aspettarti di ricevere le notifiche del webhook in meno di 5 secondi dalla registrazione della modifica dei dati. In media, i clienti ricevono le notifiche dei webhook in meno di 1 secondo dalla registrazione della modifica dei dati.  

Per ricevere i payload degli abbonamenti agli eventi tramite il firewall, è necessario aggiungere i seguenti indirizzi IP al inserisco nell&#39;elenco Consentiti di accesso agli eventi:

**Per i clienti in Europa:**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**Per i clienti in località diverse dall’Europa:**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

I seguenti argomenti supportano l’API di abbonamento agli eventi:

## Oggetti supportati dalle sottoscrizioni di eventi

I seguenti oggetti Workfront sono supportati dalle sottoscrizioni di eventi.

* Assegnazione
* Azienda
* Dashboard
* Documento
* Spesa
* Ora
* Problema
* Nota
* Portfolio
* Programma
* Progetto
* Rapporto
* Attività
* Modello
* Scheda orario
* Utente

Per un elenco dei campi supportati dagli oggetti di sottoscrizione degli eventi, vedi [Campi delle risorse di abbonamento agli eventi](../../wf-api/api/event-sub-resource-fields.md).

## Autenticazione sottoscrizione eventi

Per creare, eseguire query o eliminare un abbonamento a un evento, l’utente di Workfront ha bisogno dei seguenti elementi:

* Per utilizzare le sottoscrizioni di eventi è necessario un livello di accesso &quot;Amministratore di sistema&quot;.
* A `sessionID`  L’intestazione è necessaria per utilizzare l’API Sottoscrizioni eventi

   Per ulteriori informazioni, consulta [Autenticazione](api-basics.md#authentication) in [Nozioni di base sulle API](api-basics.md).

## Formazione della risorsa abbonamento

La risorsa abbonamento contiene i campi seguenti.

* objId (facoltativo)

   * **Stringa** : ID dell’oggetto dell’objCode specificato per il quale vengono attivati gli eventi. Se questo campo non è specificato, l&#39;utente riceve eventi per tutti gli oggetti del tipo specificato.

* objCode (obbligatorio)

   * **Stringa** : objCode dell’oggetto abbonato alle modifiche. I valori possibili per objCode sono elencati nella tabella seguente.

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
        <td scope="col">Assegnazione</td> 
        <td scope="col"><p>ASSEGNA</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Azienda </td> 
        <td scope="col"><p>AZIENDA</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Dashboard</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Documento</p></td> 
        <td scope="col">DOCU </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Spesa</p></td> 
        <td scope="col">EXPNS</td> 
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
        <td scope="col"><p>PORTA</p></td> 
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
        <td scope="col"><p>Rapporto</p></td> 
        <td scope="col"><p>PTLSEC</p></td> 
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
        <td scope="col">SCHEDA</td> 
       </tr> 
       <tr> 
        <td scope="col">Utente</td> 
        <td scope="col">UTENTE</td> 
       </tr> 
      </tbody> 
     </table>

* eventType (obbligatorio)

   * **Stringa** - Valore che rappresenta il tipo di evento a cui l&#39;oggetto è abbonato. I tipi di evento disponibili includono:

      * CREA
      * ELIMINA 
      * AGGIORNA

* url (obbligatorio)

   * **Stringa** : URL dell’endpoint al quale vengono inviati i payload dell’evento di abbonamento tramite HTTP.

* authToken (obbligatorio)

   * **Stringa** : token Bearer OAuth2 utilizzato per l’autenticazione con l’URL specificato nel campo &quot;URL&quot;. 

## Creazione di richieste API di abbonamento a eventi

Dopo aver verificato che l’utente disponga dell’accesso di amministratore e aver creato la risorsa dell’abbonamento, puoi creare abbonamenti a eventi.

Utilizza la sintassi seguente per creare l’URL.

**URL richiesta:**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
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
   <td> <p>Tipo di contenuto</p> </td> 
   <td> <p>application/json</p> </td> 
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

| Codice di risposta | Descrizione |
|---|---|
| 201 (creato) | La sottoscrizione dell’evento è stata creata correttamente. |
| 400 (richiesta non valida) | Il campo URL della risorsa abbonamento è stato ritenuto non valido. |
| 401 (non autorizzato) | Il valore sessionID fornito è vuoto o ritenuto non valido. |
| 403 (non consentito) | L’utente che corrisponde al valore sessionID fornito non dispone dell’accesso di amministratore. |

Il passaggio di una risorsa di abbonamento come corpo di una richiesta (con il tipo di contenuto &quot;application/json&quot;) determina la creazione di una sottoscrizione di evento per l’oggetto specificato. Il codice di risposta 201 (Creato) indica che l’abbonamento è stato creato. Un codice di risposta diverso da 201 indica che l’abbonamento è stato **NOT** creato.

>[!NOTE]
>
> L’intestazione di risposta &quot;Location&quot; contiene l’URI della sottoscrizione dell’evento appena creata.

**Esempio di intestazioni di risposta:**

| Intestazioni di risposta | Esempio |
|---|---|
| Content-Length | `→0` |
| Data | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| Posizione | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| Server | `→Apache-Coyote/1.1` |

## Query delle sottoscrizioni eventi

Quando esegui una query su HTTP di Workfront, utilizza il metodo GET. Esistono due modi per eseguire query per le sottoscrizioni di eventi: eseguire query per ID sottoscrizione (vedi sotto) o eseguire query su tutte le sottoscrizioni di eventi.

### Esegui query su tutte le sottoscrizioni eventi

Puoi eseguire query su tutte le sottoscrizioni di eventi per un cliente come specificato dal valore apiKey. Per gestire la risposta, puoi inoltre utilizzare le seguenti opzioni:

* **pagina**: opzione del parametro query per specificare il numero di pagine da restituire. Il valore predefinito è 1.
* **limit**: opzione del parametro query per specificare il numero di risultati da restituire per pagina. Il valore predefinito è 100 con un massimo di 1000.

La sintassi della richiesta per elencare tutte le sottoscrizioni di eventi per un cliente specifico è la seguente:

**URL richiesta:**

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

**Codici di risposta:**

| Codice di risposta | Descrizione |
|---|---|
| 200 (OK) | La richiesta restituita con tutte le sottoscrizioni di eventi trovate per il cliente che corrispondono all’ID sessione fornito. |
| 401 (non autorizzato) | Il valore sessionID fornito è vuoto. |
| 403 (non consentito) | L’utente, che corrisponde all’ID sessione fornito, non dispone dell’accesso di amministratore. |


**Esempio di intestazioni di risposta:**

| Intestazione risposta | Esempio |
|---|---|
| Content-Type | `→application/json;charset=UTF-8` |
| Data | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| Server | `→Apache-Coyote/1.1` |
| Transfer-Encoding | `→chunked` |


**Esempio di corpo della risposta:**

<!-- [Copy](javascript:void(0);) -->

```
                {
                "subscriptions":                
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": "ObjId1234",
                "objCode": "TASK",
                "url": "http://test.test.net/test/1234",
                "eventType": "UPDATE",
                "authToken": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
                ],
                "meta":
                {
                "page": 1,
                "page_count": 2,
                "limit": 100,
                "total_count": 150
                }
                }            
```

Dove

* **pagina** e **limit** sono i valori forniti nella richiesta o il valore predefinito, se non vengono forniti valori
* **page_count** è il numero totale di pagine su cui è possibile eseguire una query.
* **total_count** è il numero totale di sottoscrizioni che corrispondono alla query.

### Eseguire una query in base all’ID sottoscrizione evento

Puoi eseguire una query per le sottoscrizioni di eventi in base all’ID della sottoscrizione di eventi. La sintassi della richiesta per l’elenco delle sottoscrizioni di eventi è la seguente:

**URL richiesta:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
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

**Codici di risposta:**

| Codice di risposta | Descrizione |
|---|---|
| 200 (OK) | La richiesta restituita con l’abbonamento all’evento corrispondente all’ID dell’abbonamento fornito. |
| 401 (non autorizzato) | Il valore sessionID fornito è vuoto. |
| 403 (non consentito) | L’utente, che corrisponde all’ID sessione fornito, non dispone dell’accesso di amministratore. |


**Esempio di corpo della risposta:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
```

## Filtro abbonamento eventi

Puoi utilizzare il filtro dell’abbonamento agli eventi per assicurarti di ricevere solo messaggi pertinenti. La creazione di filtri per gli abbonamenti può ridurre in modo significativo il numero di messaggi che l’endpoint deve utilizzare.

Ad esempio, un’ **AGGIORNA - ATTIVITÀ** è possibile impostare la sottoscrizione dell&#39;evento per l&#39;attivazione solo quando **newState** di un payload dell’evento definisce **taskStatus** as **corrente**.

>[!IMPORTANT]
I seguenti attributi si applicano al filtro di abbonamento agli eventi

* Quando un campo filtro ha un valore non vuoto, vengono inviati solo messaggi con un valore **newState** contenente le chiavi e i valori del filtro vengono inviati all’URL sottoscritto
* Puoi filtrare in base ai dati personalizzati inclusi nella **newState** E/O **oldState** dell’oggetto
* I filtri vengono valutati solo a seconda che siano uguali o meno a un valore specifico
* Se la sintassi del filtro non è corretta o non corrisponde ad alcun dato contenuto nel **newState** del payload, non verrà restituito un messaggio di convalida per indicare un errore
* Non è possibile aggiornare i filtri di una sottoscrizione esistente; è necessario creare una nuova sottoscrizione con nuovi parametri di filtro.
* È possibile applicare più filtri a un singolo abbonamento e l’abbonamento verrà consegnato solo quando sono state soddisfatte tutte le condizioni del filtro.
* L’applicazione di più filtri a un singolo abbonamento equivale a utilizzare un’ **E** operatore logico.
* È possibile applicare più sottoscrizioni di eventi a un singolo oggetto, a condizione che uno o più parametri del campo di sottoscrizione dell’evento siano diversi tra ciascuna sottoscrizione di eventi.
* Quando a un singolo oggetto vengono assegnate più sottoscrizioni di eventi, tutte le sottoscrizioni di eventi associate a tale oggetto possono essere restituite a un singolo endpoint. Questa procedura può essere utilizzata come sostituto equivalente dell’operatore logico **OPPURE** che non può essere impostata utilizzando i parametri del filtro.

### Utilizzo degli operatori di confronto

È possibile specificare un campo di confronto insieme al campo filtro. Utilizza un operatore di confronto in questo campo per filtrare i risultati comparativi. Ad esempio, puoi creare una sottoscrizione UPDATE - TASK che invia un payload solo se lo stato dell’attività NON è uguale a corrente. Puoi utilizzare i seguenti operatori di confronto:

#### eq: equal

Questo filtro consente la trasmissione dei messaggi se la modifica apportata corrisponde a `fieldValue` nel filtro. Il `fieldValue` il valore distingue tra maiuscole e minuscole.

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

#### ne: diverso da

Questo filtro consente la trasmissione dei messaggi se la modifica apportata non corrisponde `fieldValue` nel filtro. Il `fieldValue` il valore distingue tra maiuscole e minuscole.

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

#### gt: maggiore di

Questo filtro consente la trasmissione dei messaggi se l’aggiornamento sulla `fieldName` è maggiore del valore per `fieldValue`.

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

#### gte: maggiore o uguale a

Questo filtro consente la trasmissione dei messaggi se l’aggiornamento sulla `fieldName` è maggiore o uguale al valore per `fieldValue`.

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

Questo filtro consente la trasmissione dei messaggi se l’aggiornamento sulla `fieldName` è minore del valore per `fieldValue`.

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

#### lte: less than or equal to

Questo filtro consente la trasmissione dei messaggi se l’aggiornamento sulla `fieldName` è minore o uguale al valore per `fieldValue`.

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

Questo filtro consente la trasmissione dei messaggi se la modifica apportata contiene `fieldValue` nel filtro. Il `fieldValue` il valore distingue tra maiuscole e minuscole

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

#### cambia

Questo filtro consente la trasmissione dei messaggi solo se il campo specificato (`fieldName`) ha un valore diverso in oldstate e newstate. Aggiornamento di altri campi oltre a quello specificato (`fieldName`) non restituirà la modifica.

>[!NOTE]
`fieldValue` nell’array filters qui sotto non ha alcun effetto.

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

#### stato

Questo connettore applica il filtro al nuovo stato o al vecchio stato dell’oggetto creato o aggiornato. Questa funzione è utile quando si desidera sapere dove è stata apportata una modifica da un elemento all’altro.
`oldState` non è possibile su CREATE `eventTypes`.

>[!NOTE]
La sottoscrizione seguente con il filtro specificato restituirà solo messaggi in cui il nome dell’attività contiene `again` il `oldState`, precedente a un aggiornamento dell&#39;attività.
Un caso d’uso per questo potrebbe essere quello di trovare i messaggi objCode che sono cambiati da una cosa all’altra. Ad esempio, per individuare tutte le attività che sono cambiate da &quot;Cerca nome&quot; a &quot;Cerca nome team&quot;

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

### Utilizzo dei campi del connettore

Il `filterConnector` sul payload dell’abbonamento consente di scegliere come applicare i filtri. Il valore predefinito è &quot;AND&quot;, dove tutti i filtri devono essere `true` affinché venga trasmesso il messaggio di abbonamento. Se si specifica &quot;OR&quot;, solo un filtro deve corrispondere per consentire il completamento del messaggio di abbonamento.

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

## Eliminazione di sottoscrizioni di eventi

Quando si elimina il codice HTTP di Workfront, utilizzare il metodo DELETE. La sintassi della richiesta per l’eliminazione di una singola sottoscrizione di evento per ID sottoscrizione è la seguente:

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
   <th> Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (nessun contenuto)</td> 
   <td>Il server ha rimosso correttamente la sottoscrizione dell'evento corrispondente all'subscriptionID fornito.</td> 
  </tr> 
  <tr> 
   <td>401 (non autorizzato)</td> 
   <td>Il valore sessionID fornito è vuoto.</td> 
  </tr> 
  <tr> 
   <td>403 (non consentito)</td> 
   <td>L’utente che corrisponde al valore sessionID fornito non dispone dell’accesso di amministratore.</td> 
  </tr> 
  <tr> 
   <td>404 (non trovato)</td> 
   <td>Il server non è stato in grado di trovare una sottoscrizione di eventi corrispondente all'subscriptionID fornito per l'eliminazione.</td> 
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

Il payload ricevuto da un utente varia a seconda del tipo di oggetto, ma esiste un formato coerente per il quale vengono consegnati i payload variabili.

Ad esempio, le seguenti proprietà rimangono coerenti in tutti i payload dell’evento:

* eventType
* subscriptionId
* oldState
* newState
* eventTime

Sebbene siano coerenti nel formato, i valori contenuti all&#39;interno delle proprietà variano tra oggetti e tipi di oggetto diversi.

Di seguito sono riportati esempi di payload per un evento UPDATE e un evento CREATE. Nell&#39;esempio UPDATE gli oggetti oldState e newState sono gli stessi, mentre nell&#39;esempio CREATE l&#39;oggetto oldState è vuoto (non NULL).

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

Se un abbonamento a un evento viene rifiutato a causa di un conflitto tra i caratteri speciali contenuti negli abbonamenti agli eventi e le impostazioni di rete, è possibile utilizzare la codifica Base64 per trasmettere gli abbonamenti agli eventi. Base64 è un insieme di schemi di codifica in grado di tradurre qualsiasi dato arbitrario in un formato di stringa ASCII. È importante notare che Base64 non è una forma di crittografia di sicurezza.

### Campo di codifica Base 64

Il campo base64Encoding è un campo facoltativo utilizzato per abilitare la codifica Base64 dei payload di abbonamento agli eventi. Il valore predefinito è false e i valori possibili sono: true, false e &quot; &quot; (vuoto).

### Esempio di richiesta tramite il campo base64Encoding

Se viene effettuata una richiesta utilizzando il campo base64Encoding impostato su true, il **newState** e **oldState** gli oggetti nel payload vengono consegnati come stringhe di codifica in base 64. Se il campo base64Encoding è impostato su false, lasciato vuoto o non incluso nella richiesta, il payload restituito non verrà codificato in base 64.

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
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## Metodo obsoleto per la query di tutte le sottoscrizioni di eventi

Il seguente endpoint API è obsoleto e non deve essere utilizzato per le nuove implementazioni. Consigliamo inoltre di passare dalle vecchie implementazioni al metodo in **Query delle sottoscrizioni eventi** sezione sopra descritta.

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
   <th> Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (nessun contenuto)</td> 
   <td>La richiesta ha restituito tutte le sottoscrizioni di eventi trovate per l'utente.</td> 
  </tr> 
  <tr> 
   <td>401 (non autorizzato)</td> 
   <td>Il valore sessionID fornito è vuoto.</td> 
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
