---
content-type: api
navigation-topic: general-api
title: API iscrizione agli eventi
description: API iscrizione agli eventi
author: John
feature: Workfront API
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: c52f1839d3d00c71c6d567084dafd586d161d8fb
workflow-type: tm+mt
source-wordcount: '2203'
ht-degree: 3%

---


# API iscrizione agli eventi

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

Quando si verifica un&#39;azione su un oggetto Adobe Workfront supportato dalle sottoscrizioni di eventi, puoi configurare Workfront per inviare una risposta all&#39;endpoint desiderato. Ciò significa che le applicazioni di terze parti possono ricevere aggiornamenti dalle interazioni di Workfront tramite l’API di Workfront subito dopo il loro verificarsi. In generale, si può aspettarsi di ricevere notifiche webhook in meno di 5 secondi dal cambiamento di dati registrato. In media, i clienti ricevono notifiche webhook in meno di 1 secondo dal cambiamento di dati registrato.  

Per ricevere i payload di sottoscrizioni di eventi attraverso il firewall, devi aggiungere i seguenti indirizzi IP al tuo inserire nell&#39;elenco Consentiti:

**Per i clienti europei:**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**Per i clienti in località diverse dall&#39;Europa:**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

I seguenti argomenti supportano l’API di iscrizione agli eventi:

## Oggetti supportati da sottoscrizioni di eventi

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

Per un elenco dei campi supportati dagli oggetti di sottoscrizione degli eventi, consulta [Campi delle risorse della sottoscrizione evento](../../wf-api/api/event-sub-resource-fields.md).

## Autenticazione iscrizione evento

Per creare, eseguire query o eliminare un abbonamento a un evento, l’utente Workfront deve disporre dei seguenti requisiti:

* Livello di accesso di &quot;Amministratore di sistema&quot;
* Un apiKey

   >[!NOTE]
   >
   >Se l’utente utilizza già l’API di Workfront, deve già disporre di un apiKey. Puoi recuperare apiKey tramite la seguente richiesta HTTP:

**URL richiesta:**

```
PUT https://<HOSTNAME>/attask/api/v7.0/USER?action=getApiKey&username=<USERNAME>&password=<PASSWORD>
```

**Intestazioni richieste:**

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
   <td> <p>text/html</p> </td> 
  </tr> 
 </tbody> 
</table>

**Codici di risposta:**

| Codice di risposta | Descrizione |
|---|---|
| 200 (OK) | La richiesta è stata elaborata correttamente e l&#39;apiKey esistente per l&#39;utente deve essere restituito nel corpo della risposta. |
| 401 (Non autorizzato) | Il server riconosce la richiesta ma non è riuscito a elaborarla perché l&#39;apiKey/user richiedente non ha accesso per effettuare questa richiesta. |

{style=&quot;table-layout:auto&quot;}

**Esempio di corpo della risposta:**

```
{
               "data"{
               "result": "rekxqndrw9783j4v79yhdsakl56bu1jn"
               }
      }
```

>[!NOTE]
>
> Se questa è la prima volta che utilizzi l’API Workfront, devi generare un apiKey da eseguire tramite questo collegamento:


```
PUT https://<HOSTNAME>/attask/api/v7.0/USER/generateApiKey?username=<USERNAME>&password=<PASSWORD>
```

## Formazione della risorsa Iscrizione

La risorsa abbonamento contiene i campi seguenti.

* objId (facoltativo)

   * **Stringa** - L&#39;ID dell&#39;oggetto del codice objCode specificato per il quale vengono attivati gli eventi. Se questo campo non viene specificato, l&#39;utente riceve eventi per tutti gli oggetti del tipo specificato.

* objCode (obbligatorio)

   * **Stringa** - Il codice objCode dell&#39;oggetto che viene sottoscritto alle modifiche. I possibili valori per objCode sono elencati nella tabella seguente.

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
        <td scope="col"><p>ASSEGNARE</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Azienda </td> 
        <td scope="col"><p>CMPY</p></td> 
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
        <td scope="col">TAGLIA</td> 
       </tr> 
       <tr> 
        <td scope="col">Utente</td> 
        <td scope="col">UTENTE</td> 
       </tr> 
      </tbody> 
     </table>

* eventType (obbligatorio)

   * **Stringa** - Un valore che rappresenta il tipo di evento a cui l&#39;oggetto è iscritto. I tipi di evento disponibili includono:

      * CREA
      * ELIMINA 
      * AGGIORNA

* url (obbligatorio)

   * **Stringa** - L’URL dell’endpoint a cui vengono inviati i payload dell’evento di abbonamento tramite HTTP.

* authToken (obbligatorio)

   * **Stringa** - Il token portatore OAuth2 utilizzato per l’autenticazione con l’URL specificato nel campo &quot;URL&quot;. 

## Creazione di richieste API di iscrizione agli eventi

Dopo aver garantito all’utente l’accesso come amministratore e aver formato la risorsa di abbonamento, puoi creare sottoscrizioni di eventi.

Utilizza la sintassi seguente per creare l&#39;URL.

**URL richiesta:**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Intestazioni richieste:**

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
   <td> <p>Autorizzazione</p> </td> 
   <td> <p>valore apiKey</p> </td> 
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
| 201 (Creato) | La sottoscrizione dell&#39;evento è stata creata correttamente. |
| 400 (Richiesta non valida) | Il campo URL della risorsa abbonamento è stato considerato non valido. |
| 401 (Non autorizzato) | L&#39;apiKey fornita è vuota o ritenuta non valida. |
| 403 (proibito) | L&#39;utente, che corrisponde all&#39;apiKey fornito, non dispone dell&#39;accesso amministratore. |

Passando una risorsa di abbonamento come corpo di una richiesta (con il tipo di contenuto &quot;application/json&quot;) si crea una sottoscrizione evento per l’oggetto specificato. Un codice di risposta 201 (Creato) indica che la sottoscrizione è stata creata. Un codice di risposta diverso da 201 indica che l’abbonamento è stato **NOT** creato.

>[!NOTE]
 L&#39;intestazione di risposta &quot;Location&quot; contiene l&#39;URI della nuova sottoscrizione evento creata.

**Esempio di intestazioni di risposta:**

| Intestazioni di risposta | Esempio |
|---|---|
| Lunghezza del contenuto | `→0` |
| Data | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| Posizione | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| Server | `→Apache-Coyote/1.1` |

## Query degli abbonamenti agli eventi

Quando si esegue una query su Workfront HTTP, utilizzare il metodo GET. Esistono due modi per eseguire query per le sottoscrizioni di eventi: Esegui una query per ID sottoscrizione (vedi di seguito) o esegui una query su tutte le sottoscrizioni di eventi.

### Query di tutte le sottoscrizioni di eventi

Puoi eseguire una query su tutte le sottoscrizioni di eventi per un cliente come specificato dal valore apiKey . Per gestire la risposta puoi inoltre utilizzare le seguenti opzioni:

* **page**: opzione del parametro query per specificare il numero di pagine da restituire. Il valore predefinito è 1.
* **limite**: opzione del parametro query per specificare il numero di risultati da restituire per pagina. Il valore predefinito è 100 con un massimo di 1000.

La sintassi di richiesta per l’elenco di tutte le sottoscrizioni di eventi per un cliente specifico è la seguente:

**URL richiesta:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Intestazioni richieste:**

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
   <td> <p>Autorizzazione</p> </td> 
   <td> <p>valore apiKey</p> </td> 
  </tr> 
 </tbody> 
</table>

**Codici di risposta:**

| Codice di risposta | Descrizione |
|---|---|
| 200 (OK) | La richiesta restituita con tutte le sottoscrizioni di eventi trovate per il cliente che corrispondono all&#39;apiKey fornito. |
| 401 (Non autorizzato) | L&#39;apiKey fornito era vuoto. |
| 403 (proibito) | L&#39;utente, che corrisponde all&#39;apiKey fornito, non dispone dell&#39;accesso amministratore. |


**Esempio di intestazioni di risposta:**

| Intestazione di risposta | Esempio |
|---|---|
| Content-Type | `→application/json;charset=UTF-8` |
| Data | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| Server | `→Apache-Coyote/1.1` |
| Codifica trasferimento | `→chunked` |


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

* **page** e **limite** sono i valori forniti nella richiesta o i valori predefiniti se non vengono forniti valori
* **page_count** è il numero totale di pagine su cui è possibile eseguire una query.
* **total_count** è il numero totale di sottoscrizioni corrispondenti alla query.

### Query per ID sottoscrizione evento

Puoi eseguire una query per le sottoscrizioni di eventi in base all’ID della sottoscrizione dell’evento. La sintassi della richiesta per l&#39;elenco degli abbonamenti agli eventi è la seguente:

**URL richiesta:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Intestazioni richieste:**

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
   <td> <p>Autorizzazione</p> </td> 
   <td> <p>valore apiKey</p> </td> 
  </tr> 
 </tbody> 
</table>

**Codici di risposta:**

| Codice di risposta | Descrizione |
|---|---|
| 200 (OK) | La richiesta restituita con la sottoscrizione dell’evento corrispondente all’ID di sottoscrizione fornito. |
| 401 (Non autorizzato) | L&#39;apiKey fornito era vuoto. |
| 403 (proibito) | L&#39;utente, che corrisponde all&#39;apiKey fornito, non dispone dell&#39;accesso amministratore. |


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

## Filtro della sottoscrizione degli eventi

È possibile utilizzare il filtro dell’abbonamento agli eventi per garantire che vengano ricevuti solo messaggi rilevanti. La creazione di filtri per le sottoscrizioni potrebbe ridurre notevolmente il numero di messaggi che l’endpoint deve utilizzare.

Ad esempio, un **AGGIORNAMENTO - ATTIVITÀ** la sottoscrizione di un evento può essere impostata in modo da attivarsi solo quando **newState** di un payload evento definisce il **taskStatus** come **attuale**.

>[!IMPORTANT]
I seguenti attributi si applicano al filtro della sottoscrizione degli eventi

* Quando un campo filtro presenta un solo valore non vuoto, viene visualizzato un messaggio con un **newState** contenente le chiavi e i valori del filtro vengono inviati all’URL con sottoscrizione
* Puoi filtrare in base ai dati personalizzati inclusi nella **newState** E/O **oldState** dell&#39;oggetto
* I filtri vengono valutati solo se sono uguali o meno a un valore specifico
* Se la sintassi del filtro non è corretta o non corrisponde ad alcun dato contenuto in **newState** del payload, non verrà restituito un messaggio di convalida per indicare che si è verificato un errore
* Impossibile aggiornare i filtri in una sottoscrizione attualmente esistente; è necessario creare una nuova sottoscrizione con nuovi parametri di filtro.
* Puoi applicare più filtri a un singolo abbonamento e l’abbonamento verrà consegnato solo quando sono state soddisfatte tutte le condizioni del filtro.
* L’applicazione di più filtri a un singolo abbonamento è una pratica equivalente all’utilizzo di un **E** operatore logico.
* È possibile applicare più abbonamenti agli eventi a un singolo oggetto, purché uno o più parametri di campo di abbonamento agli eventi siano diversi tra le sottoscrizioni di eventi.
* Quando più sottoscrizioni di eventi vengono assegnate a un singolo oggetto, tutte le sottoscrizioni di eventi associate a tale oggetto possono essere restituite a un singolo endpoint. Questa pratica può essere utilizzata come sostituto equivalente dell’operatore logico **O** che non può essere impostata utilizzando i parametri del filtro.

### Utilizzo degli operatori di confronto

Puoi specificare un campo di confronto insieme al campo del filtro. Utilizza un operatore di confronto in questo campo per filtrare i risultati comparativi. Ad esempio, è possibile creare una sottoscrizione UPDATE - TASK che invia un payload solo se lo stato dell’attività NON è uguale a quello corrente. Puoi utilizzare i seguenti operatori di confronto:

#### eq: uguale

Questo filtro consente ai messaggi di essere visualizzati se la modifica apportata corrisponde a `fieldValue` nel filtro esattamente. La `fieldValue` è sensibile a maiuscole e minuscole.

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

#### n: diverso

Questo filtro consente ai messaggi di essere visualizzati se la modifica apportata non corrisponde a `fieldValue` nel filtro esattamente. La `fieldValue` è sensibile a maiuscole e minuscole.

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

Questo filtro consente la visualizzazione dei messaggi se l&#39;aggiornamento sul `fieldName` è maggiore del valore di `fieldValue`.

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

Questo filtro consente la visualizzazione dei messaggi se l&#39;aggiornamento sul `fieldName` è maggiore o uguale al valore di `fieldValue`.

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

#### lt: inferiore a

Questo filtro consente la visualizzazione dei messaggi se l&#39;aggiornamento sul `fieldName` è minore del valore di `fieldValue`.

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

#### lte: minore o uguale a

Questo filtro consente la visualizzazione dei messaggi se l&#39;aggiornamento sul `fieldName` è minore o uguale al valore di `fieldValue`.

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

Questo filtro consente ai messaggi di essere visualizzati se la modifica apportata contiene la variabile `fieldValue` nel filtro. La `fieldValue` è sensibile a maiuscole e minuscole

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

Questo filtro consente ai messaggi di passare solo se il campo specificato (`fieldName`) ha un valore diverso in oldstate e newstate. Aggiornamento di altri campi oltre a quello specificato (`fieldName`) non restituirà tale modifica.

>[!NOTE]
`fieldValue` nella matrice dei filtri seguente non ha alcun effetto.

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

Questo connettore applica il filtro al nuovo stato o allo stato precedente dell’oggetto creato o aggiornato. È utile quando desideri sapere dove è stata apportata una modifica da un elemento all’altro.
`oldState` non è possibile su CREATE `eventTypes`.

>[!NOTE]
La sottoscrizione seguente con il filtro specificato restituirà solo messaggi in cui il nome dell’attività contiene `again` sulla `oldState`, ovvero prima dell’esecuzione di un aggiornamento sull’attività.
Un caso d&#39;uso per questo potrebbe essere quello di trovare i messaggi objCode che sono cambiati da una cosa all&#39;altra. Ad esempio, per scoprire tutte le attività che sono state modificate da &quot;Ricerca un nome&quot; a &quot;Ricerca un nome del team&quot; a &quot;Nome del team di ricerca un nome&quot;

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

### Uso dei campi del connettore

La `filterConnector` Il campo sul payload dell’abbonamento ti consente di scegliere come applicare i filtri. Il valore predefinito è &quot;AND&quot;, dove i filtri devono essere tutti `true` affinché venga trasmesso il messaggio di abbonamento. Se è specificato &quot;OR&quot;, per il messaggio di abbonamento deve corrispondere un solo filtro.

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

Quando si elimina Workfront HTTP, utilizzare il metodo DELETE. La sintassi di richiesta per l’eliminazione di una singola sottoscrizione evento per ID sottoscrizione è la seguente:

**URL richiesta:**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Intestazioni richieste:**

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
   <td> <p>Autorizzazione</p> </td> 
   <td> <p> apiKey dell’utente </p> </td> 
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
   <td>Il server ha rimosso correttamente la sottoscrizione dell’evento corrispondente all’ID sottoscrizione fornito.</td> 
  </tr> 
  <tr> 
   <td>401 (Non autorizzato)</td> 
   <td>L'apiKey fornito era vuoto.</td> 
  </tr> 
  <tr> 
   <td>403 (proibito)</td> 
   <td>L'utente che corrisponde all'apiKey fornito non dispone dell'accesso di amministratore.</td> 
  </tr> 
  <tr> 
   <td>404 (non trovato)</td> 
   <td>Impossibile trovare una sottoscrizione evento corrispondente all'ID sottoscrizione fornito per l'eliminazione.</td> 
  </tr> 
 </tbody> 
</table>

**Esempio di intestazioni di risposta:**

| Intestazione di risposta | Esempio |
|---|---|
| Data | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| Server | `→Apache-Coyote/1.1` |


**Esempio di corpo della risposta:** N/D

## Esempi di payload di eventi

Il payload ricevuto da un utente varia a seconda del tipo di oggetto, ma esiste un formato coerente per il quale vengono distribuiti i payload variabili.

Ad esempio, le seguenti proprietà rimangono coerenti per tutti i payload dell’evento:

* eventType
* subscriptionId
* oldState
* newState
* eventTime

Anche se coerenti in formato, i valori contenuti nelle proprietà variano a seconda degli oggetti e dei tipi di oggetto.

Di seguito sono riportati alcuni esempi di payload per un evento UPDATE e un evento CREATE . Nell&#39;esempio UPDATE gli oggetti oldState e newState sono gli stessi, mentre nell&#39;esempio CREATE l&#39;oggetto oldState è vuoto (non NULL).

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

Di seguito è riportato un payload di esempio per un evento CREATE :

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

## Codifica base 64

Se un abbonamento a un evento viene rifiutato a causa di un conflitto tra i caratteri speciali contenuti nelle sottoscrizioni dell&#39;evento e le impostazioni di rete, è possibile utilizzare la codifica Base64 per trasmettere le sottoscrizioni dell&#39;evento. Base64 è un insieme di schemi di codifica in grado di tradurre qualsiasi dato arbitrario in un formato stringa ASCII. È importante notare che Base64 non è una forma di crittografia di sicurezza.

### Campo di codifica Base 64

Il campo base64Encoding è un campo facoltativo utilizzato per abilitare la codifica Base64 dei payload di abbonamento agli eventi. Il valore predefinito è false e i possibili valori sono: true, false e &quot; &quot; (vuoto).

### Esempio di richiesta utilizzando il campo base64Encoding

Se una richiesta viene effettuata utilizzando il campo base64Encoding impostato su true, allora il **newState** e **oldState** gli oggetti nel payload vengono consegnati come stringhe di codifica base 64. Se il campo base64Encoding è impostato su false, left blank o not included in the request, il payload restituito non verrà codificato in base 64.

Di seguito è riportato un esempio di richiesta che utilizza il campo base64Encoding :

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

### Esempi di payload di risposta nella codifica base 64

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

Il seguente endpoint API è obsoleto e non deve essere utilizzato per nuove implementazioni. Consigliamo inoltre di transitare vecchie implementazioni al metodo in **Query degli abbonamenti agli eventi** sezione sopra descritta.

Puoi eseguire una query su tutte le sottoscrizioni di eventi per un cliente come specificato dal valore apiKey . La sintassi di richiesta per l&#39;elenco di tutte le sottoscrizioni di eventi per un cliente specifico è il seguente URL:

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**Intestazioni richieste:**

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
   <td> <p>Autorizzazione</p> </td> 
   <td> <p> apiKey dell’utente </p> </td> 
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
   <td>401 (Non autorizzato)</td> 
   <td>L'apiKey fornito era vuoto.</td> 
  </tr> 
  <tr> 
   <td>403 (proibito)</td> 
   <td>L'utente che corrisponde all'apiKey fornito non dispone dell'accesso di amministratore.</td> 
  </tr> 
 </tbody> 
</table>

 

### Esempio del corpo della risposta

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
