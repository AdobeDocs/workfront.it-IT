---
title: Nozioni di base sulle API di Adobe Workfront Planning
description: L’obiettivo per l’API di pianificazione di Adobe Workfront è semplificare la creazione di integrazioni con Planning introducendo un’architettura REST-ful che funziona tramite HTTP. Questo documento presuppone che tu abbia familiarità con le risposte REST e JSON e descrive l’approccio adottato dall’API di Planning.
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: fdbe3945f59306fc26424d7e88b799d9dcaea4da
workflow-type: tm+mt
source-wordcount: '2206'
ht-degree: 3%

---


# Nozioni di base sulle API di pianificazione di Adobe Workfront

{{planning-important-intro}}

<!--

Lilit asked me to hide everything in this current article and replace it with her version of it. I kept just the Field type and search modifier section. The rest of the article is a re-write of the original from Lilit. 

She also said we need to reword how we organize the version features, after we get more versions released but for now, she calls out what's different in V1 than the current (V2) with almost every feature. 

-->

L’obiettivo dell’API di pianificazione di Adobe Workfront è semplificare la creazione di integrazioni con Planning introducendo un’architettura RESTful che funziona tramite HTTP. In questo documento si presuppone che tu abbia familiarità con le risposte REST e JSON.

Per informazioni complete sul riferimento all&#39;endpoint, sugli schemi di richiesta/risposta e sui dettagli specifici della versione, vedere la [documentazione per gli sviluppatori API di Workfront Planning](https://developer.adobe.com/wf-planning).

## Autenticazione

L’API di pianificazione di Workfront utilizza OAuth 2.0 per l’autenticazione. Le credenziali vengono impostate tramite Adobe Developer Console.

A seconda del tipo di integrazione, sono supportati i due flussi seguenti:

* **Autenticazione server-to-server (JWT)**: per integrazioni automatizzate e servizi back-end senza interazione dell&#39;utente. Utilizza le credenziali da server a server OAuth (credenziali client concesse, l&#39;applicazione si autentica direttamente utilizzando il proprio ID client e segreto per ottenere un token di accesso, senza alcun accesso utente o passaggio di consenso).

  Per informazioni, vedere [Autenticazione da server a server](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/).

* **Autenticazione utente (flusso codice di autorizzazione)**: per integrazioni che agiscono per conto di un utente specifico. Utilizza le credenziali dell&#39;app Web OAuth o dell&#39;app a pagina singola (concessione del codice di autorizzazione: l&#39;utente effettua l&#39;accesso e dà il consenso, dopodiché l&#39;applicazione riceve un codice di autorizzazione che scambia per un token di accesso).

  Per informazioni, vedere [Autenticazione utente](https://developer.adobe.com/developer-console/docs/guides/authentication/UserAuthentication/).

Per iniziare, crea un progetto in Adobe Developer Console e aggiungi Workfront Planning API per ottenere le credenziali.

Per impostare le credenziali, crea un’applicazione OAuth2 in Workfront.

Per informazioni, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

>[!NOTE]
>
>L&#39;endpoint `/login` e l&#39;autenticazione della chiave API non sono supportati per Workfront Planning. Non utilizzare `sessionID` o `apiKey` parametri.


## Controllo delle versioni API

Il controllo delle versioni dell’API di Planning viene eseguito tramite il percorso URL.

Di seguito sono elencate le versioni supportate correnti:

| Versione | Data di rilascio |
|-----------|----------------|
| Versione 1 | Luglio 2024 |
| Versione 2 | Maggio 2026 |

<!--

(*****************add deprecation date column above, when we have one*****************)

-->


Per ulteriori informazioni sulle versioni supportate correnti, vedere l&#39;articolo [Documentazione per gli sviluppatori API di Workfront Planning](https://developer.adobe.com/wf-planning).

È consigliabile eseguire esplicitamente il targeting di una versione in tutte le integrazioni:

```
https://{customer-domain}/maestro/api/v2/...
```

Quando viene rilasciata una nuova versione principale, la versione precedente continuerà a essere disponibile fino a quando non viene comunicata una data di rimozione.

Segui le note sulla versione di Workfront per essere sempre informato sulle modifiche API.


## Struttura degli URL e operazioni

Gli oggetti vengono manipolati inviando una richiesta HTTP al relativo URI univoco. Operazione specificata dal metodo HTTP.

| Metodo | Operazione |
|----------|----------------------------------------------------------------------|
| GET | Recuperare un singolo oggetto per ID o oggetti di ricerca/elenco |
| POST | Crea un nuovo oggetto |
| PUT | Sostituire un oggetto esistente (aggiornamento completo) |
| PATCH | Aggiorna parzialmente un oggetto esistente (vengono modificati solo i campi forniti) |
| DELETE | Eliminare un oggetto |

>[!NOTE]
>
>**Nota versione1:** `PATCH` non è supportato nella versione 1. Utilizza `PUT` per tutti gli aggiornamenti.


Per i percorsi di endpoint completi e gli esempi di richieste/risposte, consulta il **riferimento API** in [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning).

## Codici di stato HTTP

L&#39;API Planning restituisce i codici di stato HTTP standard:

| Codice | Significato |
|------------------------|-------------------------------------------------|
| 200 OK | GET, PUT o PATCH riusciti |
| 201 creato | POST riuscito (risorsa creata) |
| 204 Nessun contenuto | DELETE riuscito |
| 207 con più stati | Operazione in blocco completata con risultati misti, in cui alcuni elementi hanno avuto esito positivo e altri non sono riusciti. Per informazioni dettagliate, vedere le risposte dei singoli elementi. |
| 400 - Richiesta non valida | Richiesta non valida. Per ulteriori informazioni consulta la risposta di errore. |
| 401 Non autorizzato | Token di autenticazione mancante o non valido |
| 403 - Non consentito | Autorizzazioni autenticate ma insufficienti |
| 404 Non trovato | La risorsa non esiste |
| Conflitto 409 | Conflitto di scrittura, la risorsa è stata modificata da un’altra richiesta. Riprova con la versione più recente. |
| 429 Troppe richieste | Limite di frequenza superato |

>[!NOTE]
>
>**Nota della versione 1:** La versione 1 restituisce `200 OK` per tutte le operazioni riuscite, inclusi POST e DELETE.


## Gestione degli errori

L’API di Planning restituisce gli errori in un formato coerente. Ogni risposta di errore include un messaggio leggibile dall’utente, un codice di errore leggibile dal computer e un ID richiesta per l’escalation del supporto.

Esempio di risposta di errore:

```
json
{
  "title": "Validation failed",
  "status": 400,
  "detail": "Request validation failed. See 'errors' for details.",
  "errorCode": "VALIDATION_FAILED",
  "requestId": "req-123",
  "errors": [
    { "field": "name", "message": "must not be blank" }
  ]
}
```

Utilizzare `errorCode` (non `status`) per gestire gli errori a livello di programmazione. Fornisce la classificazione più specifica dell’errore.

>[!NOTE]
>
>**Nota della versione 1:** le risposte di errore della versione 1 utilizzano un campo `type` numerico (ad esempio `40001`) invece di una stringa `errorCode` e racchiudono i dettagli in un oggetto `report` anziché in un campo `detail` di primo livello.

## Filtraggio dei record

Utilizzare il parametro `filter` nelle richieste di ricerca dei record per restituire solo i record che corrispondono a criteri specifici. Per le richieste POST, `filter` è una proprietà JSON nel corpo della richiesta. Per le richieste GET, `filter` è un parametro di query contenente un gruppo di filtri con codifica JSON. I filtri utilizzano una struttura composita tipizzata con operatori logici espliciti.

```
json
{
  "filter": {
    "operator": "AND",
    "conditions": [
      { "fieldId": "<fieldId>", "condition": "IS", "value": "Active" },
      { "fieldId": "<fieldId>", "condition": "CONTAINS", "value": "marketing" }
    ]
  }
}
```

I filtri possono essere nidificati utilizzando gli operatori `AND` / `OR` per creare condizioni composte:

```
json
{
  "filter": {
    "operator": "OR",
    "conditions": [
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "BETWEEN", "value": ["2024-03-31T20:00:00.000Z", "2024-04-01T20:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "active" }
        ]
      },
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "IS_BETWEEN", "value": ["2024-04-15T00:00:00.000Z", "2024-04-16T00:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "planned" }
        ]
      }
    ]
  }
}
```

>[!NOTE]
>
>**Nota versione 1:** La versione 1 utilizza operatori non tipizzati Mongo in un oggetto `filters`. Gli operatori hanno il prefisso `$` (ad esempio `$and`, `$or`, `$is`, `$contains`, `$isBetween`). I parametri di impaginazione (`offset`, `limit`) e `recordTypeId` vengono passati nel corpo della richiesta anziché come parametri di query e percorso URL.


## Tipi di campi e modificatori di ricerca

È possibile utilizzare modificatori e filtri con i campi per controllare quali dati verranno restituiti nei risultati.

Per esempi, vedere la [documentazione per gli sviluppatori API di Workfront Planning](https://developer.adobe.com/wf-planning/).

### Utilizzo dei modificatori di ricerca

Workfront Planning supporta i seguenti modificatori di ricerca:


<table style="table-layout:auto"> 
  <colgroup><col class="c1"><col class="c2"><col class="c3"><col class="c4"></colgroup>
  <thead>
    <tr>
      <th>Modificatore</th>
      <th>Esempio</th>
      <th>Descrizione</th>
      <th>Valori possibili</th>
    </tr>
  </thead>
  <tbody>
    <tr><td class="modifier">CONTAINS</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"CONTAINS","value":"product"}</td><td>Restituisce record il cui valore di campo contiene il filtro</td><td class="possible">"Lancio di nuovi prodotti"</td></tr>
    <tr><td class="modifier">DOES_NOT_CONTAIN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"DOES_NOT_CONTAIN","value":"product"}</td><td>Restituisce record in cui il valore del campo non contiene il filtro</td><td class="possible">"Nuovo lancio"</td></tr>
    <tr><td class="modifier">È</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS","value":"new product launch"}</td><td>Restituisce record il cui valore di campo corrisponde esattamente al filtro</td><td class="possible">"Lancio di nuovi prodotti"</td></tr>
    <tr><td class="modifier">IS_NOT</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT","value":"product"}</td><td>Restituisce record il cui valore di campo non corrisponde esattamente al filtro</td><td class="possible">"Lancio di nuovi prodotti"</td></tr>
    <tr><td class="modifier">IS_EMPTY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_EMPTY"}</td><td>Restituisce record il cui valore di campo è vuoto</td><td class="possible">"" o null</td></tr>
    <tr><td class="modifier">IS_NOT_EMPTY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT_EMPTY"}</td><td>Restituisce record il cui valore di campo non è vuoto</td><td class="possible">"Lancio di nuovi prodotti"</td></tr>
    <tr><td class="modifier">GREATER_THAN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"GREATER_THAN","value":"10"}</td><td>Restituisce record il cui valore di campo è maggiore del filtro</td><td class="possible">"11"</td></tr>
    <tr><td class="modifier">GREATER_THAN_OR_EQUAL</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"GREATER_THAN_OR_EQUAL","value":"10"}</td><td>Restituisce record il cui valore di campo è maggiore o uguale al filtro</td><td class="possible">"10", "11"</td></tr>
    <tr><td class="modifier">LESS_THAN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"LESS_THAN","value":"10"}</td><td>Restituisce record il cui valore di campo è minore del filtro</td><td class="possible">"9"</td></tr>
    <tr><td class="modifier">LESS_THAN_OR_EQUAL</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"LESS_THAN_OR_EQUAL","value":"10"}</td><td>Restituisce record il cui valore di campo è minore o uguale al filtro</td><td class="possible">"9", "10"</td></tr>
    <tr><td class="modifier">IS_BETWEEN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_BETWEEN","value":["2024-01-01","2024-12-31"]}</td><td>Restituisce record il cui valore di campo è compreso tra i due valori di filtro</td><td class="possible">["2024-03-01","2024-06-30"]</td></tr>
    <tr><td class="modifier">IS_NOT_BETWEEN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT_BETWEEN","value":["2024-01-01","2024-12-31"]}</td><td>Restituisce record il cui valore di campo non rientra tra i due valori di filtro</td><td class="possible">["2023-01-01","2025-06-30"]</td></tr>
    <tr><td class="modifier">IS_AFTER</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_AFTER","value":"2024-01-01"}</td><td>Restituisce record il cui valore del campo data è successivo al filtro</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_BEFORE</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_BEFORE","value":"2024-12-31"}</td><td>Restituisce record il cui valore del campo data è precedente al filtro</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_ANY_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_ANY_OF","value":["Active","Planned"]}</td><td>Restituisce record il cui valore di campo corrisponde a qualsiasi valore nell'elenco dei filtri</td><td class="possible">["Attivo","Pianificato","Completo"]</td></tr>
    <tr><td class="modifier">IS_NONE_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NONE_OF","value":["Active","Planned"]}</td><td>Restituisce record il cui valore di campo non corrisponde a nessuno dei valori nell'elenco dei filtri</td><td class="possible">["Attivo","Pianificato"]</td></tr>
    <tr><td class="modifier">HAS_ANY_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_ANY_OF","value":["Tag1","Tag2"]}</td><td>Restituisce record il cui campo multivalore contiene uno dei valori del filtro</td><td class="possible">["Tag1","Tag2"]</td></tr>
    <tr><td class="modifier">HAS_ALL_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_ALL_OF","value":["Tag1","Tag2"]}</td><td>Restituisce record il cui campo multivalore contiene tutti i valori del filtro</td><td class="possible">["Tag1","Tag2"]</td></tr>
    <tr><td class="modifier">IS_EXACTLY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_EXACTLY","value":["Tag1"]}</td><td>Restituisce record il cui campo multivalore contiene esattamente i valori del filtro e nessun altro</td><td class="possible">["Tag1"]</td></tr>
    <tr><td class="modifier">HAS_NONE_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_NONE_OF","value":["Tag1"]}</td><td>Restituisce record il cui campo multivalore non contiene nessuno dei valori del filtro</td><td class="possible">["Tag1"]</td></tr>
  </tbody>
</table>


>[!NOTE]
>
>Nota della versione 1: i nomi dei modificatori V1 utilizzano `$-prefixed camelCase` (ad esempio `$contains`, `$isNot`, `$isEmpty`, `$greaterThan`, `$greaterThanOrEqual`, `$lessThan`, `$lessThanOrEqual`, `$isBetween`, `$isNotBetween`, `$isAnyOf`, `$hasAllOf`). Il comportamento di ciascun modificatore è lo stesso.


## Condizioni di filtro supportate per tipo di campo

| Tipo di campo | Condizioni supportate |
|-----------------------------|--------------------------------------------------------------------------------------------------------------|
| testo, testo lungo | CONTAINS, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY |
| numero, percentuale, valuta | IS, IS_NOT, GREATER_THAN, GREATER_THAN_OR_EQUAL, LESS_THAN, LESS_THAN_OR_EQUAL, IS_EMPTY, IS_NOT_EMPTY |
| data | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY |
| selezione singola | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| selezione multipla, utente | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| booleano | È |
| formula | CONTAINS, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY |
| creato da | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF |
| aggiornato da | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| creato a | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN |
| update-at | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY |
| riferimento | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| ricerca | Dipende dal tipo di campo collegato |

>[!NOTE]
>
>**Nota della versione 1:** La versione 1 utilizza nomi di operatori con prefisso `$` (ad esempio `$contains`, `$greaterThan`, `$isAnyOf`, `$hasAllOf`). Il set di condizioni supportate per tipo di campo è lo stesso.

## Filtrare per campi Persone

I filtri dei campi delle persone (`user`, `created-by`, `updated-by`, `approved-by`) accettano sia gli ID utente Adobe IMS che gli ID utente Workfront. Un valore di stringa semplice viene interpretato come un ID utente Adobe IMS.

Per impostare il tipo di identificatore per controllare l&#39;ID utente di Workfront, è necessario trasmettere esplicitamente i parametri `id` e `idType`. I valori supportati per `idType` sono &quot;`WF`&quot; per gli ID utente di Workfront e &quot;`IMS`&quot; per gli ID utente di Adobe IMS.

```
{ 
  "filter": { 
   "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<userFieldId>", 
        "condition": "HAS_ANY_OF", 
        "value": [ 
          { "id": "63e3b13000078c1795146248182d15dc", "idType": "WF" } 
        ] 
      } 
    ] 
  } 
} 
```

>[!NOTE]
>
> Versione 1 nota: la versione 1 supporta solo il filtro per ID IMS degli utenti.

## Filtraggio dei campi di riferimento esterni per ID esterno

I campi di riferimento esterni collegano i record a oggetti in altri sistemi Adobe (come progetti Workfront o AEM Assets). Internamente, Planning assegna gli ID record di Planning a questi oggetti. Per filtrare questi campi direttamente in base al loro ID oggetto originale, aggiungi `"matchExternalId": true` a una condizione di filtro.

Questo flag è valido solo per i campi di riferimento in cui `referenceOptions.isExternal` è `true`; viene ignorato per i campi di riferimento non esterni. Se non è possibile risolvere un singolo valore stringa, la richiesta non riesce con `400 Bad Request`. Se viene fornito un valore di elenco, le voci non risolte passano attraverso invariate e semplicemente non corrispondono.

```
{ 
  "filter": { 
    "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<externalReferenceFieldId>", 
        "condition": "IS_ANY_OF", 
        "value": [ 
          "5f6a4f6e00000123456789abcdef0123", 
          "/content/dam/wknd/en/adventures/bali-surf-camp" 
        ], 
        "matchExternalId": true 
      } 
    ] 
  } 
} 
```

>[!NOTE]
>
>Versione 1 Nota: la versione 1 non supporta il filtro in base agli ID di oggetti esterni.

## Campi di connessione esterna

I tipi di record di Planning possono ospitare campi di riferimento esterni che collegano i record a oggetti in altri sistemi Adobe anziché ad altri tipi di record di Planning.

Per creare un campo di riferimento esterno tramite API, impostare `referenceOptions.recordTypeId` su un nuovo campo `REFERENCE` sull&#39;ID del tipo di record esterno desiderato. Il server deriva automaticamente `referenceOptions.isExternal=true` e i metadati di connessione (`connectionName, objectName`) dal tipo di record di destinazione.

I tipi di oggetti esterni supportati includono oggetti Workfront (progetti, attività, programmi, portfolio, aziende, gruppi, team, utenti) e AEM Assets (risorse, frammenti di contenuto).

>[!NOTE]
>
>Versione 1 Nota: la versione 1 non supporta la creazione di campi di connessione esterni.


## Ordinamento

Ordinare i risultati in base a qualsiasi campo includendo un array `sort` nella richiesta:

```
json
{
  "sort": [
    { "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" },
    { "fieldId": "F658afcbd4a0273c67c346fd5", "direction": "desc" }
  ]
}
```

Più campi di ordinamento vengono valutati in ordine. Applica sempre un ordinamento durante la paginazione per garantire un ordinamento coerente tra le pagine.

Per raggruppare i risultati, includere una matrice di gruppi insieme all&#39;ordinamento:

```
{ 
  "sort": [{ "fieldId": "F001", "direction": "asc" }], 
  "group": [{ "fieldId": "F002", "direction": "asc" }] 
} 
```

>[!NOTE]
>
>Versione 1 Nota: la versione 1 utilizza `sorting` (non `sort`), `groupingFieldIds` (array di ID campo, non `group` oggetti) e l&#39;ora obsoleto `rowOrderViewId` per applicare l&#39;ordine di riga di una visualizzazione esistente. Nessuno di questi parametri V1 è supportato nella versione

## Proiezione sul campo

Per limitare i campi restituiti in una risposta, utilizzare i parametri di query `fieldIds` o `fieldAliases` con un elenco separato da virgole. Questo riduce le dimensioni del payload di risposta ed è consigliato per integrazioni con volumi elevati o sensibili alla latenza.

>[!NOTE]
>
>**Nota della versione 1:** La versione 1 utilizza `?attributes=` per la proiezione (ad esempio `?attributes=data,createdBy`) anziché `?fieldIds=` o `?fieldAliases=`.

## Paginazione

L’API di Planning supporta risposte impaginate per gestire set di dati di grandi dimensioni.

* **L&#39;impaginazione basata su cursore** viene utilizzata per aree di lavoro, tipi di record, campi e visualizzazioni. Passa un valore `cursor` dalla risposta precedente per recuperare la pagina successiva. Le risposte basate sul cursore includono un flag hasMore per indicare se sono presenti più pagine o meno.
* **La paginazione basata su pagina** è utilizzata per la ricerca dei record. Utilizzare `page` e `size` come parametri di query. Applica sempre un ordinamento durante la paginazione per garantire un ordinamento coerente tra le pagine. Si noti che l&#39;impaginazione è basata su zero, quindi per recuperare i risultati della seconda pagina, utilizzare &quot;`page=1`&quot; come parametro.

Ad esempio, utilizza la seguente richiesta per recuperare la seconda pagina di 500 record da una ricerca record:

```
POST /v2/record-types/{recordTypeId}/records/search?page=1&size=500 
{ 
  "sort": [{ "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" }], 
  "filter": { "operator": "AND", "conditions": [ 
    { "fieldId": "<fieldId>", "condition": "IS", "value": "active" } 
  ] } 
} 
```

Tutte le risposte impaginate includono una busta strutturata che indica se sono disponibili più risultati. Applica sempre un ordinamento durante la paginazione per garantire un ordinamento coerente tra le pagine.

>[!NOTE]
>
> **Nota della versione 1:** la versione 1 utilizza `offset` e `limit` sono stati passati nel corpo della richiesta (valore predefinito: 500, massimo 2.000). Per recuperare i record 2001-4000, impostare &quot;`offset`&quot;: &quot;`2000`&quot;, &quot;`limit`&quot;: &quot;`2000`&quot; nel corpo della richiesta. La risposta restituisce una matrice di record flat con un campo `totalCount`.

## Operazioni in blocco

L’API Planning supporta la creazione, l’aggiornamento, la correzione e l’eliminazione in blocco di record in una singola richiesta. Per i percorsi degli endpoint, i formati di richiesta e i limiti di record per operazione, fare riferimento al **riferimento API** in [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning).

>[!NOTE]
>
>**Nota versione 1:** le operazioni in blocco non sono disponibili nella versione 1.


## Autorizzazioni

Le autorizzazioni per le entità vengono gestite tramite un’API di autorizzazioni dedicata, separata dagli endpoint di risorsa stessi. Questo consente di leggere le autorizzazioni correnti, gestire l’elenco di condivisione e gestire le richieste di accesso indipendentemente dalle operazioni sui dati. Per ulteriori informazioni, vedere la sezione &quot;Riferimenti API&quot; nell&#39;articolo [Workfront Planning API](https://developer.adobe.com/wf-planning).

>[!NOTE]
>
>**Nota della versione 1:** la versione 1 non espone un&#39;API di autorizzazioni pubblica. Il livello di autorizzazione è incorporato direttamente nei DTO di risposta delle risorse.

## Utilizzo dell’API di Planning con i moduli personalizzati di Workfront

È possibile chiamare l&#39;API Planning da un campo di ricerca Esterna in un modulo personalizzato Workfront per rendere visibili i dati di Planning direttamente all&#39;interno di oggetti Workfront. Per ulteriori informazioni, vedere [Esempi del campo di ricerca esterna in un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

## Risorse correlate

Per ulteriore documentazione relativa all’API, consulta anche i seguenti articoli:

* Documentazione e riferimento per gli sviluppatori di [Workfront Planning API](https://developer.adobe.com/wf-planning)
* [Introduzione alla Pianificazione di Adobe Workfront](/help/quicksilver/planning/general/planning-overview.md)
* [Panoramica sull’accesso a Pianificazione di Adobe Workfront](/help/quicksilver/planning/access/access-overview.md)
* [Creare applicazioni OAuth2 per le integrazioni Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)

<!--

Our version of this article before Lilit replaced it with the above: 

The goal for the Adobe Workfront Planning API is to simplify building integrations with Planning by introducing a REST-ful architecture that operates over HTTP. This document assumes you are familiar with REST and JSON responses and describes the approach taken by the Planning API.  

A familiarity with the Workfront Planning schema will assist you in understanding the database relationships that can be utilized to pull data out of Workfront Planning for integration purposes. 

You can call the planning API from an External lookup field in a Workfront custom form.

For more information on External lookup fields, see [Examples of the External lookup field in a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>When using the Planning API, all user-related information will be returned using the Adobe Identity Management System (IMS) user ID, and not the Workfront user ID.
>
>For information, see [Manage users in the Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).  

## Workfront Planning API versions

* Version 1 - released in July 2024 

  For more information, see the section [Workfront Planning API Version 1](#workfront-planning-api-version-1) in this article. 

* Version 2 - released in May 2026

  For more information, see the section [Workfront Planning API Version 2](#workfront-planning-api-version-2) in this article.


## Workfront Planning API Version 1

Workfront Planning API Version 1 was released in July 2024.

The following sections described functionality that was made available in the Workfront API Version 1. 

All future API version will contain the same functionality, unless otherwise specified. 

### Operations 

Objects are manipulated by sending an HTTP request to their unique URI. The operation to be performed is specified by the HTTP method. 

The standard HTTP methods correspond to the following operations: 

* **GET** - Retrieves an object by ID, searches for all objects by a query 
* **POST** - Inserts a new object 
* **PUT** - Edits an existing object 
* **DELETE** - Deletes an object 

For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

### Field types and search modifiers used with them 

You can use modifiers and filters with fields to control what data will be returned in results. 

For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

#### Using search modifiers 

Workfront Planning supports the following search modifiers: 

<table>
    <tr>
        <td><b>Modifier</b></td>
        <td><b>Example</b></td>
        <td><b>Description</b></td>
        <td><b>Possible Values</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Returns records whose field value contains the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Returns records where the field value does not contain the filter  </td>
        <td>"New Launch"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Returns records whose field value exactly match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Returns records whose field value exactly is not match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is empty  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is not empty  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Returns records whose field value is greater than the filter  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is greater than or equal the filter  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Returns records whose field value is less than the filter  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is less than or equal the filter </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is after the filter  </td>
        <td>"2024-05-15T20:00:00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is before the filter </td>
        <td>"2024-05-12T20:00:00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is between the filter  </td>
        <td><ul><li>"2024-05-12T20:00:00.000Z" </li><li>"2024-05-14T20:00:00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is not between the filter  </td>
        <td><ul><li>"2024-05-09T20:00:00.000Z"  </li><li>"2024-05-17T20:00:00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is any of the filter  </td>
        <td><ul><li>"active" </li><li>"completed" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is none of the filter </td>
        <td><ul><li>"finished"  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has any of the filter  </td>
        <td><ul><li>["active", "fixed"]  </li><li>["fixed", "completed", "finished"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has all of the filter  </td>
        <td><ul><li>["active", "completed"]   </li><li>["active", "completed", "finished"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has none of the filter </td>
        <td>["fixed", "finished"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is exactly the filter  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>
 
#### Field types 

Below is the list of supported field types and what search modifiers can be used with each of those field types  

| Field Type | Supported search modifiers |
|---|---|
| text |$contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| long-text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| number | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| percentage | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| currency | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| date | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| single-select | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| multi-select | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| boolean | $is |
| user | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| formula | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| created-by | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| updated-by | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| updated-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| reference | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| lookup | Depends on the linked field |

### Using "And" and "Or" statements 

In the API call you can have filters that are based on several criteria combined by $and" and "$or" statements  

```
{
  "recordTypeId": "recordTypeId",
  "offset": "integer",
  "limit": "integer",
  "filters": [
    {
      "$or": [
        {
          "launch_date": {
            "$isBetween": [
              "2024-03-31T20:00:00.000Z",
              "2024-04-01T20:00:00.000Z"
            ]
          }
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-03-31T20:00:00.000Z",
                  "2024-04-01T20:00:00.000Z"
                ]
              }
            },
            {
              "status": "active"
            }
          ]
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-04-15T00:00:00.000Z",
                  "2024-04-16T00:00:00.000Z"
                ]
              }
            },
            {
              "status": "planned"
            }
          ]
        }
      ]
    }
  ]
}
```

### Using the fields request parameter 

You can use the fields request parameter to specify a comma-separated list of specific fields that should be returned. These field names are case-sensitive.  

For example, the request 

`/v1/records/search?attributes=data,createdBy`

```
{
    "records": [
        {
            "id": "Rc6527ecb35df57c441d92ba00",
            "createdBy": "61a9cc0500002f9fdaa7a6f824f557e1",
            "createdAt": null,
            "updatedBy": null,
            "updatedAt": null,
            "customerId": null,
            "imsOrgId": null,
            "recordTypeId": null,
            "data": {
                "F666c0b58b6fee61a2ea6ea81": [
                    {
                        "externalId": null,
                        "id": "Rc665728ff95730b58bc757b13",
                        "value": null
                    },
..
```

returns a response similar to the following: 

  
```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Sorting query results in the API 

You can sort your results by any field if you append the following to your API call: 


`/v1/records/search`

Request body:

```
{
    "recordTypeId": "Rt6527ecb25df57c441d92b9fa",
    "filters": [],
    "sorting": [
        {
            "fieldId": "F6527ecb25df57c441d92b9fc",
            "direction": "asc"
        },
        {
            "fieldId": "F658afcbd4a0273c67c346fd5",
            "direction": "desc"
        }
    ],
    "limit": 500,
    "offset": 0,
    "rowOrderViewId": "V6527ecb75df57c441d92ba03",
    "groupingFieldIds": []
}
```

### Query limits and paginated responses 

By default, Planning API requests return 500 results, starting from the beginning of the list. To override the default limitation for number of results, you can use the `limit` parameter in your requests and set it to a different number, up to 2000 results.  

We recommend that you consider using paginated responses for large datasets by adding the `offset` parameter to your requests. Paginated responses allow you to specify the location of the first result that should be returned. 

For example, if you want to return the results 2001-4000, you can use the following request. This example returns 2000 records that are in active status, starting from the 2001st result: 

`POST /v1/records/search`


Request body: 

```
{ 
    "recordTypeId": "recordTypeId", 
    "offset": "2001", 
    "limit": "2000", 
    "filters": [ 
        { "status": "active" } 
    ] 
} 
```

To make sure your results are properly paginated, use a sorting parameter. This allows the results to be returned in the same order, so that the pagination does not repeat or skip results. 

For more information on sorting, see [Sorting query results in the API](#sorting-query-results-in-the-api) in this article.


Lilit did not want this organized like this - keeping this for reference: 

## Workfront Planning API Version 2

Version of the Workfront Planning API was released in May 2026. 

In addition to all the information contained in Version 1, the following enhancements were added in Version 2: 

* Search by the user's Workfront ID field instead of the user's IMS ID.

    This is applicable to custom People fields, as well as system fields such as Created By and Last Updated By fields.

* Ability to search by external connections (Workfront or AEM objects) via the API.

* Ability to link cross-workspace shared records through API. 

* Support all CRUD operations for workspaces, record types, fields, and views. 

* Enable permissions sharing for all sharable entities via API. 

    This includes workspaces, record types, and views. (***********and in the future also records and fields.*********)

* Support for uploading record thumbnail through API. 

-->