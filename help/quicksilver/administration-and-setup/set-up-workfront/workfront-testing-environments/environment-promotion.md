---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Spostare gli oggetti da un ambiente a un altro
description: La funzionalità di promozione dell’ambiente ha lo scopo di consentire lo spostamento di oggetti correlati alla configurazione da un ambiente all’altro. Non supporta la possibilità di spostare oggetti transazionali (con eccezioni limitate).
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
source-git-commit: 68c3a66a91f4c0936d256398b5d30518226396a6
workflow-type: tm+mt
source-wordcount: '2346'
ht-degree: 3%

---

# Sposta oggetti da uno [!DNL Workfront] ambiente in un altro

<!-- 
TO DO

Overview of value
Check for any code changes
Fix {}
Add to tocs
-->

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] piano</td> 
   <td> <p>Enterprise, Prime o Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] licenza</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>Devi essere un [!DNL Workfront] amministratore. Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Autorizzazioni oggetto</p> </td> 
   <td> <p>Tutti</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pacchetto di supporto</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred] o [!UICONTROL Enterprise]</p> <p>Il pacchetto di supporto standard non ha accesso alla sandbox di aggiornamento personalizzata, ma alla sandbox di anteprima.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisiti

L’endpoint &quot;Crea pacchetto di promozione&quot; presuppone che tu abbia già configurato l’ambiente di origine. Questa chiamata API richiede la creazione manuale di una mappa oggetto di [!DNL Workfront] objCodes e GUID oggetto. La struttura specifica di questa mappa è descritta di seguito.

## Oggetti supportati per la promozione dell’ambiente

La funzionalità di promozione dell’ambiente ha lo scopo di consentire lo spostamento di oggetti correlati alla configurazione da un ambiente all’altro. Non supporta la possibilità di spostare oggetti transazionali (con eccezioni limitate).

* [Oggetti di lavoro](#work-objects)
* [Oggetti di reporting](#reporting-objects)
* [Oggetti dati personalizzati](#custom-data-objects)
* [Oggetti organizzazione](#organization-objects)
* [Altri oggetti di configurazione](#other-configuration-objects)


### Oggetti di lavoro

| Oggetto promovibile | Inclusi oggetti secondari promozionali |
| --- | --- |
| Progetto (PROJ) | Progetto<br>Attività<br>Assegnazione<br>Predecessore<br>Azienda<br>Percentuale sostituzione<br>Gruppo<br>Ruolo<br>Team<br>Processo di approvazione<br>Percorso di approvazione<br>Passaggio di approvazione<br>Approvatore passaggio<br>Pianificazione<br>Giorno non feriale<br>Definizione coda<br>Gruppo di argomenti coda<br>Argomento Coda<br>Regola di Instradamento<br>Percorso milestone<br>Milestone<br>Tipo di Ora<br>Pool di Risorse<br>Categoria<br>Parametro di Categoria<br>Parametro<br>Raggruppa parametri<br>Opzione Parametro<br>Logica di visualizzazione della categoria |
| Modello (TMPL) | Modello<br>Attività modello<br>Assegnazione attività modello<br>Predecessore attività modello<br>Azienda<br>Percentuale sostituzione<br>Gruppo<br>Ruolo<br>Team<br>Processo di approvazione<br>Percorso di approvazione<br>Passaggio di approvazione<br>Approvatore passaggio<br>Pianificazione<br>Giorno non feriale<br>Definizione coda<br>Gruppo di argomenti coda<br>Argomento Coda<br>Regola di Instradamento<br>Percorso milestone<br>Milestone<br>Tipo di Ora<br>Pool di Risorse<br>Categoria<br>Parametro di Categoria<br>Parametro<br>Raggruppa parametri<br>Opzione Parametro<br>Logica di visualizzazione della categoria |

### Oggetti di reporting

| Oggetto promovibile | Inclusi oggetti secondari promozionali |
| --- | --- |
| Modello di layout (UITMPL) | Modello di layout<br>Dashboard<br>Calendario<br>Sezione calendario<br>Pagina esterna<br>Report<br>Filtro<br>Raggruppamento<br>Visualizza<br>Parametro |
| Dashboard (PTLTAB) | Dashboard<br>Calendario<br>Sezione calendario<br>Pagina esterna<br>Report<br>Filtro<br>Raggruppamento<br>Visualizza<br>Parametro |
| Calendario (calendario) | Calendario<br>Sezione calendario |
| Pagina esterna (EXTSEC) | Pagina Esterna |
| Rapporto (PTLSEC) | Report<br>Filtro<br>Raggruppamento<br>Visualizza<br>Parametro |
| Filtro (UIFT) | Filtro<br>Parametro |
| Raggruppamento (UIGB) | Raggruppamento<br>Parametro |
| Visualizza (UIVW) | Visualizza<br>Parametro |

### Oggetti dati personalizzati

| Oggetto promovibile | Inclusi oggetti secondari promozionali |
| --- | --- |
| Categoria (CTGY) | Categoria<br>Parametro di Categoria<br>Parametro<br>Raggruppa parametri<br>Opzione Parametro<br>Logica di visualizzazione della categoria<br>Gruppo |
| Parametro (PARAM) | Parametro<br>Opzione Parametro |
| Raggruppa Parametri (PGRP) | Gruppo di parametri |

### Oggetti organizzazione

| Oggetto promovibile | Inclusi oggetti secondari promozionali |
| --- | --- |
| Gruppo (GROUP) | Gruppo <br>Sottogruppi (fino a 5 livelli)<br>Categoria<br>Parametro di Categoria<br>Parametro<br>Raggruppa parametri<br>Opzione Parametro<br>Logica di visualizzazione della categoria |
| Ruolo (ROLE) | Ruolo |
| Team (TEAM) | Team<br>Gruppo |
| Società (CMPY) | Azienda<br>Percentuale sostituzione<br>Categoria<br>Parametro di Categoria<br>Parametro<br>Raggruppa parametri<br>Parametro <br>Logica di visualizzazione della categoria<br>Gruppo |
| Portfolio (PORTA) | Portfolio<br>Programma<br>Gruppo<br>Categoria<br>Parametro di Categoria<br>Parametro<br>Raggruppa parametri<br>Opzione Parametro<br>Logica di visualizzazione della categoria |
| Programma (PRGM) | Programma<br>Portfolio<br>Gruppo<br>Categoria<br>Parametro di Categoria<br>Parametro<br>Raggruppa parametri<br>Opzione Parametro<br>Logica di visualizzazione della categoria |

### Altri oggetti di configurazione

| Oggetto promovibile | Inclusi oggetti secondari promozionali |
| --- | --- |
| Processo di approvazione (ARVPRC) | Processo di approvazione<br>Percorso di approvazione<br>Passaggio di approvazione<br>Approvatore passaggio<br>Ruolo<br>Team<br>Gruppo |
| Pianificazione (SCHED) | Pianificazione<br>Giorno non feriale<br>Gruppo |
| Percorso milestone (MPATH) | Percorso milestone<br>Milestone |
| Timesheet Ricorrente (TSPRO) | Timesheet Ricorrente<br>Tipo di Ora |
| Tipo di Ora (HOURT) | Tipo di ora |
| Tipo di spesa (EXPTYP) | Tipo di Spesa |
| Tipo di rischio (RSKTYP) | Tipo Rischio |
| Pool di Risorse (RSPL) | Gruppo di risorse |

## Autenticazione

L’API autentica ogni richiesta per garantire che il client abbia accesso alla visualizzazione o alla modifica di un oggetto richiesto.

L’autenticazione viene eseguita trasmettendo un ID sessione o una chiave API, che può essere fornita utilizzando il seguente metodo:

### Autenticazione intestazione richiesta

Il metodo preferito per l’autenticazione consiste nel trasmettere un’intestazione di richiesta denominata SessionID contenente il token di sessione. Questo ha il vantaggio di essere al sicuro [CSRF (Cross-Site Request Forgery)](http://en.wikipedia.org/wiki/Cross-site_request_forgery) attacchi e non interferire con l’URI a scopo di caching.

Di seguito è riportato un esempio di intestazione di richiesta:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## Endpoint API

* [Creare un pacchetto](#create-a-package)
* [Ottieni un elenco di pacchetti](#get-a-list-of-packages)
* [Ottenere un pacchetto per ID](#get-a-package-by-id)
* [Ottenere la definizione di configurazione di un pacchetto](#get-a-packages-configuration-definition)
* [Sostituisci dettagli e definizione pacchetto](#replace-package-details-and-definition)
* [Aggiornare proprietà specifiche di un pacchetto](#update-specific-properties-of-a-package)
* [Eliminare un pacchetto](#delete-a-package)
* [Eseguire una](#execute-a-pre-run)
* [Eseguire un’installazione](#execute-an-installation)
* [Ottieni un elenco di installazioni per un pacchetto specifico](#get-a-list-of-installations-for-a-specific-package)
* [Ottenere i dettagli di installazione per un&#39;installazione](#get-the-installation-details-for-an-installation)

### Creare un pacchetto

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Questa chiamata esegue un processo con più passaggi.

Il primo passaggio comporta la creazione di un pacchetto di promozione vuoto con lo stato &quot;ASSEMBLAGGIO&quot;.

Il secondo passaggio utilizza il `objectCollections` fornito nel corpo del POST per assemblare i record richiesti da Workfront. Questo passaggio potrebbe richiedere alcuni minuti, a seconda del numero di record richiesti e della configurazione di Workfront. Al termine di questo processo, il pacchetto di promozione vuoto viene aggiornato con `packageEntities` e lo stato viene impostato automaticamente su &quot;DRAFT&quot; (BOZZA).


>[!NOTE]
>
>Osserva la struttura del `objectCollections`  array.
>
>Ogni elemento dell’array contiene un `objCode` chiave che corrisponde al codice oggetto documentato in Workfront API Explorer.
>
>Ogni elemento contiene anche un `entities` raccolta. Questo prevede che `ID` campo. Può inoltre accettare un `name` per rendere più facile sapere quale `ID` rappresenta.
>
>Per l’elenco dei codici oggetto consentiti da richiedere in `objectCollections` , vedere la [Oggetti supportati per la promozione dell’ambiente](#supported-objects-for-environment-promotion) in questo articolo.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### Intestazioni

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Oppure

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Corpo

```json
{
    "name": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes...",
    "source": "https://{domain}.{environment}.workfront.com",
    "objectCollections": [
        {
            "objCode": "PROJ",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597ba1",
                    "name": "Agency Request"
                }
            ]
        },
        {
            "objCode": "TMPL",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597bb2",
                    "name": "New Agency Onboarding"
                },
                {
                    "ID": "6419b8b9001151ee258921a4f7597bc3",
                    "name": "New Agency Offboarding"
                }
            ]
        },
        {
            "objCode": "PTLTAB",
            "entities": [
                {
                    "ID": "645e6435000b4aaebe4776f4a42ed5ad",
                    "name": "Agency Performance and Readiness"
                }
            ]
        }
    ]
}
```

#### risposta

```json
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "ASSEMBLING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
}
```

### Ottieni un elenco di pacchetti

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Questa chiamata restituisce un elenco non filtrato di pacchetti promozionali appartenenti al cliente.

La risposta includerà tutti i pacchetti creati da una qualsiasi delle istanze sandbox, anteprima o produzione del cliente di Workfront.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### Intestazioni

```json
{
    "apikey": "**********"
}
```

Oppure

```json
{
    "sessionID": "*****************"
}
```

#### Corpo

_Vuoto_

#### risposta

```
200
```

```json
{
    "data": [
        {
            "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
            "name": "Agency Onboarding - 2023-06-06",
            "description": "This promotion package contains configuration to support the agency onboarding processes...",
            "status": "ASSEMBLING",
            "version": 1,
            "installationCounts": {},
            "createdAt": "2023-06-06T17:29:21.600Z",
            "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
            "publishedAt": null,
            "customerId": "61aa9d090005fa42152c1cb66659f38d"
        },
        {...}
    ]
}
```

### Ottenere un pacchetto per ID

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Questa chiamata restituisce i dettagli di un pacchetto di promozione richiesto.

La richiesta può essere effettuata tramite qualsiasi ambiente indipendentemente dall’origine del pacchetto promozionale.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Intestazioni

```json
{
    "apikey": "**********"
}
```

Oppure

```json
{
    "sessionID": "*****************"
}
```

#### Corpo

_Vuoto_

#### risposta

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "DRAFT",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "null"
                   - or -
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Ottenere la definizione di configurazione di un pacchetto

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}/definition</code></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/definition
```

#### Intestazioni

```json
{
    "apikey": "**********"
}
```

Oppure

```json
{
    "sessionID": "*****************"
}
```

#### Corpo

_Vuoto_

#### risposta

```
200
```

```json
{
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID": null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
}
```

### Sostituisci dettagli e definizione pacchetto

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PUT /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Questa chiamata sostituisce tutti i contenuti del pacchetto promozionale.

La richiesta prevede che vengano forniti tutti i campi modificabili.

Gli attributi modificabili sono:

1. nome (stringa)
1. descrizione (stringa)
1. origine (stringa con convalida URL)
1. stato (stringa con convalida del valore)
1. version (numero intero)
1. packageEntities (insieme)

Le opzioni di stato includono:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>ASSEMBLAGGIO</td> 
   <td><p>Questo stato viene assegnato automaticamente durante il montaggio degli oggetti.</p><p>Questo stato non può essere impostato direttamente da un cliente.</p></td> 
  </tr> 
  <tr> 
   <td>BOZZA</td> 
   <td><p>Questo stato viene assegnato al termine di un processo di assemblaggio o durante la creazione di un pacchetto di promozione vuoto.</p><p>Il cliente può ripristinare lo stato attuale del pacchetto promozionale.</p><p>In questo stato, il pacchetto promozionale non può essere installato in alcun ambiente.</p></td> 
  </tr> 
  <tr> 
   <td>TEST</td> 
   <td><p>Questo stato consente di installare un pacchetto di promozione in qualsiasi sandbox di anteprima o di aggiornamento personalizzato. In questo stato il pacchetto non può essere installato in produzione.</p></td> 
  </tr> 
  <tr> 
   <td>ATTIVO</td> 
   <td><p>Questo stato consente di installare un pacchetto promozionale in qualsiasi ambiente, inclusa la produzione.</p><p>Quando lo stato di un pacchetto è impostato su ACTIVE, <code>publishedAt</code> La data viene impostata automaticamente sulla marca temporale corrente della richiesta.</p></td> 
  </tr> 
  <tr> 
   <td>DISABILITATO</td> 
   <td><p>Questo stato verrà utilizzato per nascondere i pacchetti promozionali utilizzati in precedenza che non verranno installati in alcun ambiente in futuro.</p><p>Quando un pacchetto si trova in questo stato, non può essere installato in alcun ambiente.</p><p>Quando lo stato di un pacchetto è impostato su DISABLED, il <code>retiredAt</code> La data viene impostata automaticamente sulla marca temporale corrente della richiesta.</p><p>Si consiglia di utilizzare questo stato anziché il<code>DELETE /package</code> endpoint perché è recuperabile e la cronologia di installazione viene mantenuta per tutte le distribuzioni effettuate con questo pacchetto.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLAGGIO NON RIUSCITO</td> 
   <td><p>Se la fase ASSEMBLING non riesce, il pacchetto promozionale viene automaticamente posto in questo stato.</p><p>Per riportare il pacchetto alla fase ASSEMBLING, è necessario attivare nuovamente il processo di estrazione.</p></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
PUT https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Intestazioni

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Corpo

```json
{
    "name": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes... with a description change",
    "source": "https://{domain}.{environment}.workfront.com",
    "status": "TESTING",
    "version": 1,
    "metadata": {
        "displayOrder": ["GROUP","ROLE","TMPL","PROJ","PTLTAB"],
        "historyOrder": ["GROUP","ROLE","TMPL","TTSK","PROJ","PTLTAB"], 
        "installOrder": ["GROUP","ROLE","TMPL","TTSK","TPRED","TASSGN","PROJ","QUED","RRUL","QUET","UIFT","UIGB","UIVW","PTLTAB"], 
        "summaryOrder": ["GROUP","ROLE","TMPL"], 
        "shapeVersion": 2
    },
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID": null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
}
```

#### risposta

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "TESTING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Aggiornare proprietà specifiche di un pacchetto

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PATCH /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Questa chiamata aggiorna qualsiasi contenuto del pacchetto promozionale fornito nel corpo del PATCH.

Gli attributi modificabili sono:

1. nome (stringa)
1. descrizione (stringa)
1. origine (stringa con convalida URL)
1. stato (stringa con convalida del valore)
1. version (numero intero)
1. packageEntities (insieme)

   oppure

   objectCollections (array)

Fornire `packageEntities` aggiorna il pacchetto di promozione con la definizione di configurazione fornita.

Fornire `objectCollections` avvierà una riestrazione dal `source` ambiente associato al pacchetto di promozione. Il `source` deve essere fornito quando `objectCollections` viene fornito.

#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### Intestazioni

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Oppure

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Corpo

```json
{
    "status": "ACTIVE"
}
```

#### risposta

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "ACTIVE",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Eliminare un pacchetto

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>DELETE /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Questa chiamata elimina il record del pacchetto di promozione. Questa azione è irreversibile.

>[!NOTE]
>
>Invece di eliminare un pacchetto di promozione, si consiglia di modificarne lo stato in DISABILITATO. In questo modo il pacchetto potrà essere recuperato e verrà mantenuta la cronologia di installazione della posizione in cui è stato distribuito.

#### URL

```
DELETE https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Intestazioni

```json
{
    "apikey": "**********"
}
```

Oppure

```json
{
    "sessionID": "*****************"
}
```

#### Corpo

_Vuoto_

#### risposta

```
200
```

```
Deleted
```

### Eseguire una

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST  {customer-domain}/environment-promotion/api/v1/packages/{id}/prepare-installation</code></td> 
  </tr> 
  </tbody> 
</table>

Questa chiamata esegue un confronto tra la definizione del pacchetto e l’ambiente di destinazione identificato nell’URL.

Il risultato è un corpo JSON che identifica se un oggetto di promozione viene trovato o meno nell’ambiente di destinazione.

Per ogni oggetto promozione, effettuare una delle seguenti operazioni `actions`  verrà impostato:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>CREA</td> 
   <td><p>Quando non è possibile trovare un record corrispondente nell’ambiente di destinazione, l’azione viene impostata su CREATE.</p><p>Quando questa azione è impostata in <code>translationmap</code> che viene fornito al <code>/install</code> il servizio di installazione creerà il record.</p></td> 
  </tr> 
  <tr> 
   <td>USA ESISTENTE</td> 
   <td><p>Quando un record corrispondente viene trovato nell’ambiente di destinazione, l’azione è impostata su USEEXISTING e su <code>targetId</code> viene anche acquisito nel <code>translationmap</code>.</p><p>Quando questa azione è impostata in <code>translationmap</code> che viene fornito al <code>/install</code> il servizio di installazione non creerà il record. Tuttavia, utilizzerà il <code>targetId</code> incluso nella voce mappa per altri oggetti che potrebbero avere un riferimento a questo record.</p><p>Ad esempio, nell’ambiente di destinazione in cui viene distribuito un pacchetto è possibile trovare un "Gruppo predefinito". Non è possibile avere due record "Gruppo predefinito", pertanto il servizio di installazione utilizzerà il GUID per il gruppo esistente in qualsiasi altra azione di creazione dell'oggetto che includa un riferimento al "Gruppo predefinito", ad esempio un progetto, un modulo o qualsiasi altra entità correlata al gruppo.</p><p><b>Nota:</b> <ul><li><p>Quando viene assegnata l’azione USEEXISTING, il record esistente nell’ambiente di destinazione non viene modificato. </p><p>Ad esempio, se la descrizione del "Gruppo predefinito" è cambiata nella sandbox da cui è stato creato il pacchetto e il valore della descrizione è diverso nell’ambiente di destinazione, il valore rimarrà invariato dopo un’installazione con questo <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>IGNORA</td> 
   <td><p>Questa azione non verrà impostata automaticamente.</p><p>Consente di eseguire una sostituzione manuale di un'azione CREATE o USEEXISTING assegnata prima di eseguire <code>/install</code> chiamare.</p><p><b>Note: </b><ul><li><p>Se un record originariamente impostato su CREATE è impostato su IGNORE, anche tutti i record figlio devono essere impostati su IGNORE.</p><p>Ad esempio, se un record Modello è stato mappato con un’azione CREA e l’utente che esegue l’installazione desidera escluderlo dalla distribuzione, può impostare l’azione Modello su IGNORA.</p><p>In questo caso, se l’utente che esegue l’installazione non imposta anche le attività modello, le assegnazioni delle attività modello, i predecessori delle attività modello, la definizione della coda, gli argomenti della coda, le regole di indirizzamento e così via su IGNORA, la distribuzione provocherà un tentativo di installazione non riuscito.</p></li><li><p>Se un record originariamente impostato su USEEXISTING è impostato su IGNORE, potrebbero verificarsi alcuni effetti negativi durante il processo di installazione.</p><p>Ad esempio, se un record Gruppo è stato mappato con l'azione USEEXISTING e l'utente che esegue l'installazione modifica l'azione in IGNORA, per gli oggetti che richiedono un gruppo (ad esempio, un progetto non può esistere senza un gruppo assegnato), il gruppo predefinito del sistema verrà assegnato a tale progetto.</p></li><li><p>Se un record originariamente impostato su USEEXISTING è impostato su CREATE, potrebbero verificarsi alcuni effetti negativi durante il processo di installazione perché molte entità Workfront hanno vincoli di nome univoco.</p><p>Ad esempio, se un record "Gruppo predefinito" è stato mappato con l’azione USEEXISTING e l’utente che esegue l’installazione modifica l’azione in CREATE, poiché esiste già un "Gruppo predefinito", il tentativo di installazione non riuscirà a completare tutti i passaggi. I nomi dei gruppi devono essere univoci.</p><p>Alcune entità non hanno un vincolo di nome univoco. Per tali oggetti, questa modifica determinerà due record con lo stesso nome. Ad esempio, Modelli, Progetti, Viste, Filtri, Raggruppamenti, Rapporti e Dashboard non richiedono vincoli di nome univoci. È consigliabile utilizzare nomi univoci per questi record, ma non è possibile applicarli.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

Non è attualmente supportato alcun aggiornamento `action` nelle funzionalità alfa di questo servizio. Opzione per consentire un aggiornamento `action` è qualcosa su cui stiamo facendo ricerche.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/:id/prepare-installation
```

#### Intestazioni

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Oppure

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Corpo

```json
{}
```

#### risposta

```
200
```

```json
{}
```

### Eseguire un’installazione

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

Questa chiamata avvia un tentativo di installazione di un pacchetto di promozione nell’ambiente di destinazione identificato nell’URL di POST.

#### Opzioni

Se un `translationmap` non viene fornito nel corpo del POST, il processo avvierà automaticamente il `/prepare-installation` chiamare. Il `translationmap` che viene restituito verrà utilizzato così com’è, senza la possibilità di rivederlo o modificarlo.

Se un `translationmap` è fornito nel corpo del POST, il processo di installazione utilizzerà la mappatura fornita. In questo modo, l&#39;utente che esegue l&#39;installazione può rivedere e apportare le modifiche necessarie prima di eseguire un tentativo di installazione.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}/install
```

#### Intestazioni

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Oppure

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Corpo

```json
{
}
```

#### risposta

```
200
```


```json
{}
```

### Ottieni un elenco di installazioni per un pacchetto specifico

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
</code></td> 
  </tr> 
  </tbody> 
</table>

I risultati includono gli eventi di installazione da tutti gli ambienti in cui è stato distribuito il pacchetto. Non si limitano alle installazioni per l’ambiente attraverso cui viene effettuata la richiesta. Questo consente di identificare gli ambienti che hanno ricevuto questo pacchetto.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
```

#### Intestazioni

```json
{
    "apikey": "**********"
}
```

Oppure

```json
{
    "sessionID": "*****************"
}
```

#### Corpo

_Vuoto_

#### risposta

```
200
```

```json
[
    {
        "id": "2892b936-e09e-455a-935f-e1462ab9753c",
        "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
        "environmentPromotionPackageVersion": 1,
        "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
        "customerId": "54286d78b064451096752b99bf968481",
        "status": "COMPLETED",
        "environment": "https://{domain}.{environment}.workfront.com",
        "registeredAt": "2021-03-16T02:21:31.908Z",
        "updatedAt": null,
        "translationMap": {
            "ROLE": {
                "5f6d114f006883209828ddd9088e63b3": {
                    "name": "DAM Curator",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f4bed00028a718599f29575840053"
                },
                "ad535a9ebe647361e053a7656a0a1575": {
                    "name": "Copywriter",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f162700001ca051081c06667b14a4"
                },
                ...
            },
            "TMPL": {
                "5f9b317c00b3db5af69abcd1ed5f82aa": {
                    "name": "Digital Asset Production (Integrated)",
                    "action": "CREATE",
                    "isValid": true,
                    "targetId": "6054cda40000d5af63dc811d9c2b3a07"
                },
                ...
            },
            ...
        }
    },
    {...}
]
```

### Ottenere i dettagli di installazione per un&#39;installazione

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /installations/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Questa chiamata restituirà il finale `translationMap` prodotto dal servizio di installazione per un&#39;installazione specifica.

Ogni documento indicherà il tipo di `action` e se tale azione sia stata eseguita con successo o meno.

Per i record con un valore CREATE `action` il `targetId` verrà impostato con il valore del record appena creato nel sistema di destinazione. Inoltre, il `installationStatus` verrà impostato su INSTALLATO.

Per i record con USEEXISTING `action` il `targetId` verrà impostato anche il campo e `installationStatus` verrà impostato su REGISTRATO. Ciò significa che il processo di mappatura è stato completato e che il servizio di installazione riconosce di aver valutato il record e non c&#39;è nulla su cui intervenire.

Se il record ha un valore CREATE `action` ma non riesce a creare il record, quindi il `installationStatus` verrà impostato su FAILED (NON RIUSCITO) e verrà indicato anche il motivo dell’errore.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}
```

#### Intestazioni

```json
{
    "apikey": "**********"
}
```

Oppure

```json
{
    "sessionID": "*****************"
}
```

#### Corpo

_Vuoto_

#### risposta

```
200
```

```json
{
    "id": "2892b936-e09e-455a-935f-e1462ab9753c",
    "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
    "environmentPromotionPackageVersion": 1,
    "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
    "customerId": "54286d78b064451096752b99bf968481",
    "status": "COMPLETED",
    "environment": "https://{domain}.{environment}.workfront.com",
    "registeredAt": "2021-03-16T02:21:31.908Z",
    "updatedAt": null,
    "translationMap": {
        "ROLE": {
            "5f6d114f006883209828ddd9088e63b3": {
                "name": "DAM Curator",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "600f4bed00028a718599f29575840053"
            },
            ...
        },
        "TMPL": {
            "5f9b317c00b3db5af69abcd1ed5f82aa": {
                "name": "Digital Asset Production (Integrated)",
                "action": "CREATE",
                "isValid": true,
                "targetId": "6054cda40000d5af63dc811d9c2b3a07"
            },
            ...
        },
        ...
    }
}
```



<!--table templates

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

<table style="table-layout:fixed"> 
 <col> 
 <tbody> 
  <tr> 
   <td><b></b></td> 
  </tr> 
  <tr> 
   <td><pre></pre></td> 
  </tr> 
  </tbody> 
</table>
-->