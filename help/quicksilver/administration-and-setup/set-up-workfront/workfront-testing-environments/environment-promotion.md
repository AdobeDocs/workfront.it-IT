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
recommendations: noDisplay, noCatalog
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
source-git-commit: 6f5da5ede6bb8c98b26d7d37366670c89ded6c49
workflow-type: tm+mt
source-wordcount: '2095'
ht-degree: 2%

---

# Sposta oggetti tra ambienti [!DNL Workfront] utilizzando l&#39;API di promozione dell&#39;ambiente [!DNL Workfront]

La funzionalità di promozione dell’ambiente consente di spostare gli oggetti relativi alla configurazione da un ambiente all’altro. Puoi spostare questi oggetti utilizzando l’API di Workfront come descritto in questo articolo.

Per istruzioni sullo spostamento di oggetti tra ambienti utilizzando l&#39;applicazione Workfront, vedere:

* [Creare o modificare un pacchetto di promozione dell’ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
* [Installare un pacchetto di promozione dell’ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)


## Requisiti di accesso

Devi avere i seguenti:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] piano</strong>
   </td>
   <td> Prime o Ultimate (solo per i nuovi piani)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenze</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Configurazioni del livello di accesso
   </td>
   <td>Devi essere un amministratore [!DNL Workfront].
   </td>
  </tr>
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisiti

L’endpoint &quot;Crea pacchetto di promozione&quot; presuppone che tu abbia già configurato l’ambiente di origine. Questa chiamata API richiede la creazione manuale di una mappa oggetto di [!DNL Workfront] objCodes e GUID oggetto. La struttura specifica di questa mappa è descritta di seguito.

## Oggetti supportati per la promozione dell’ambiente

La funzionalità di promozione dell’ambiente ha lo scopo di consentire lo spostamento di oggetti correlati alla configurazione da un ambiente all’altro. Non supporta la possibilità di spostare oggetti transazionali (con eccezioni limitate).

Per un elenco degli oggetti promozionali e dei relativi oggetti secondari promozionali inclusi, vedere [Oggetti supportati per la promozione dell&#39;ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) nell&#39;articolo [Panoramica sullo spostamento di oggetti tra ambienti Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).

## Autenticazione

L’API autentica ogni richiesta per garantire che il client abbia accesso alla visualizzazione o alla modifica di un oggetto richiesto.

L’autenticazione viene eseguita trasmettendo un ID sessione o una chiave API, che può essere fornita utilizzando il seguente metodo:

### Autenticazione intestazione richiesta

Il metodo preferito per l’autenticazione consiste nel trasmettere un’intestazione di richiesta denominata SessionID contenente il token di sessione. Questo ha il vantaggio di essere sicuro contro gli attacchi di [Cross-Site Request Forgery (CSRF)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) e di non interferire con l&#39;URI a scopo di caching.

Di seguito è riportato un esempio di intestazione di richiesta:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## Endpoint API

* [Creare un pacchetto](#create-a-package)
* [Ottieni un elenco di pacchetti](#get-a-list-of-packages)
* [Ottenere un pacchetto per ID](#get-a-package-by-id)
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

Nel secondo passaggio viene utilizzato l&#39;array `objectCollections` fornito nel corpo del POST per assemblare i record richiesti da Workfront. Questo passaggio potrebbe richiedere alcuni minuti, a seconda del numero di record richiesti e della configurazione di Workfront. Al termine di questo processo, il pacchetto di promozione vuoto viene aggiornato con `packageEntities` e lo stato viene impostato automaticamente su &quot;BOZZA&quot;.


>[!NOTE]
>
>Prendere nota della struttura dell&#39;array `objectCollections`.
>
>Ogni elemento nell&#39;array contiene una chiave `objCode` che corrisponde al codice oggetto documentato in Esplora API di Workfront.
>
>Ogni elemento contiene anche una raccolta `entities`. È previsto il campo `ID`. Può inoltre accettare un attributo `name` facoltativo per semplificare la conoscenza di ciò che rappresenta `ID`.
>
>Per l&#39;elenco dei codici oggetto consentiti da richiedere nell&#39;elenco `objectCollections`, vedere la sezione [Oggetti supportati per la promozione dell&#39;ambiente](#supported-objects-for-environment-promotion) in questo articolo.

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

#### Risposta

```json
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ASSEMBLING",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
    }
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

#### Risposta

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
            "createdAt": "2023-06-06T17:29:21.600Z",
            "deletedAt": null
},
        {...}
    ]
}
```

&lt;!—Controllare &quot;status&quot; sopra—è stato aggiunto?—>

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

#### Risposta

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "DRAFT",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
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
1. stato (stringa con convalida del valore)

Per una descrizione dettagliata degli stati disponibili, vedere [Stati di promozione dell&#39;ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) nell&#39;articolo [Panoramica sullo spostamento di oggetti tra ambienti Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).


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

#### Risposta

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ACTIVE",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
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

#### Risposta

```
200
```

```
Deleted
```

### Eseguire una

>[!IMPORTANT]
>
>Prima di poter eseguire un&#39;installazione, è necessario eseguire questa pre-esecuzione. Quando esegui l’installazione, utilizzerai l’ID generato da questa chiamata.

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

Per ogni oggetto promozione verrà impostato uno dei seguenti `actions`:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>CREA</td> 
   <td><p>Quando non è possibile trovare un record corrispondente nell’ambiente di destinazione, l’azione viene impostata su CREATE.</p><p>Quando questa azione viene impostata in <code>translationmap</code> fornito all'endpoint <code>/install</code>, il servizio di installazione creerà il record.</p></td> 
  </tr> 
  <tr> 
   <td>USA ESISTENTE</td> 
   <td><p>Quando viene trovato un record corrispondente nell'ambiente di destinazione, l'azione viene impostata su USEEXISTING e un <code>targetId</code> viene acquisito anche in <code>translationmap</code>.</p><p>Se questa azione è impostata in <code>translationmap</code> fornito all'endpoint <code>/install</code>, il servizio di installazione non creerà il record. Tuttavia, utilizzerà <code>targetId</code> incluso nella voce mappa per altri oggetti che potrebbero avere un riferimento a questo record.</p><p>Ad esempio, nell’ambiente di destinazione in cui viene distribuito un pacchetto è possibile trovare un "Gruppo predefinito". Non è possibile avere due record "Gruppo predefinito", pertanto il servizio di installazione utilizzerà il GUID per il gruppo esistente in qualsiasi altra azione di creazione dell'oggetto che includa un riferimento al "Gruppo predefinito", ad esempio un progetto, un modulo o qualsiasi altra entità correlata al gruppo.</p><p><b>Nota:</b> <ul><li><p>Quando viene assegnata l’azione USEEXISTING, il record esistente nell’ambiente di destinazione non viene modificato. </p><p>Ad esempio, se la descrizione del "Gruppo predefinito" è stata modificata nella sandbox da cui è stato creato il pacchetto e il valore della descrizione è diverso nell'ambiente di destinazione, il valore rimarrà invariato dopo un'installazione con questo <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>SOVRASCRITTURA</td> 
   <td><p>Questa azione non verrà impostata automaticamente.</p><p>Questa azione consente di aggiornare un oggetto esistente nell’ambiente di destinazione. Consente di eseguire una sostituzione manuale di un'azione CREATE o USEEXISTING assegnata prima di eseguire la chiamata <code>/install</code>.<ul><li>Un utente può aggiornare un oggetto nell’ambiente di test, quindi utilizzare l’azione di sovrascrittura per aggiornare tale oggetto nell’ambiente di destinazione.</p></li><li><p>Se l’utente installa inizialmente un pacchetto di promozione e successivamente un nuovo pacchetto (o aggiornato) contiene modifiche agli oggetti nel pacchetto iniziale, può utilizzare la funzione SOVRASCRITTURA per sostituire (sostituire) gli oggetti installati in precedenza. </p><p>Per ulteriori informazioni sulla sovrascrittura, vedere la sezione [Sovrascrittura](#overwriting) in questo articolo.</li><ul></td> 
  </tr> 
  <tr> 
   <td>IGNORA</td> 
   <td><p>Questa azione non verrà impostata automaticamente.</p><p>Consente di eseguire una sostituzione manuale di un'azione CREATE o USEEXISTING assegnata prima di eseguire la chiamata <code>/install</code>.</p><p><b>Note: </b><ul><li><p>Se un record originariamente impostato su CREATE è impostato su IGNORE, anche tutti i record figlio devono essere impostati su IGNORE.</p><p>Ad esempio, se un record Modello è stato mappato con un’azione CREA e l’utente che esegue l’installazione desidera escluderlo dalla distribuzione, può impostare l’azione Modello su IGNORA.</p><p>In questo caso, se l’utente che esegue l’installazione non imposta anche le attività modello, le assegnazioni delle attività modello, i predecessori delle attività modello, la definizione della coda, gli argomenti della coda, le regole di indirizzamento e così via su IGNORA, la distribuzione provocherà un tentativo di installazione non riuscito.</p></li><li><p>Se un record originariamente impostato su USEEXISTING è impostato su IGNORE, potrebbero verificarsi alcuni effetti negativi durante il processo di installazione.</p><p>Ad esempio, se un record Gruppo è stato mappato con l'azione USEEXISTING e l'utente che esegue l'installazione modifica l'azione in IGNORA, per gli oggetti che richiedono un gruppo (ad esempio, un progetto non può esistere senza un gruppo assegnato), il gruppo predefinito del sistema verrà assegnato a tale progetto.</p></li><li><p>Se un record originariamente impostato su USEEXISTING è impostato su CREATE, potrebbero verificarsi alcuni effetti negativi durante il processo di installazione perché molte entità Workfront hanno vincoli di nome univoco.</p><p>Ad esempio, se un record "Gruppo predefinito" è stato mappato con l’azione USEEXISTING e l’utente che esegue l’installazione modifica l’azione in CREATE, poiché esiste già un "Gruppo predefinito", il tentativo di installazione non riuscirà a completare tutti i passaggi. I nomi dei gruppi devono essere univoci.</p><p>Alcune entità non hanno un vincolo di nome univoco. Per tali oggetti, questa modifica determinerà due record con lo stesso nome. Ad esempio, Modelli, Progetti, Viste, Filtri, Raggruppamenti, Rapporti e Dashboard non richiedono vincoli di nome univoci. È consigliabile utilizzare nomi univoci per questi record, ma non è possibile applicarli.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

Non è attualmente supportato un aggiornamento `action` nelle funzionalità alfa di questo servizio. Si sta ricercando l&#39;opzione per consentire un aggiornamento `action`.

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

#### Risposta

```
200
```

```json
{
    "environmentPromotionPackageId": "45f2ae94-76c0-4b13-8f3b-f688de83043d",
    "environmentPromotionPackageVersion": 1,
    "id": "c0bc79bd-c9c1-4b5b-b118-b1241392de0e",
    "userId": "5ba38da500b752fd66439d4f6a9999a1",
    "customerId": "5ba38d9d00b74f0c7a38b1b487fc9710",
    "status": "PREPARING",
    "environment": "mmi.my.workfront.com",
    "registeredAt": "2023-10-19T20:00:16.697Z",
    "updatedAt": "2023-10-19T20:00:16.701Z",
    "translationMap": {
        "CTGY": {
            "62d9c9a0000013aeeefe7242a0a5fdb2": {
                "name": "Example Document Form",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9a0000013aeeefe7242a0a5fdb2"
            }
        },
        "PGRP": {
            "62d1eee4001c6618e6b9f9a588ba1598": {
                "name": "Asset Detail",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee4001c6618e6b9f9a588ba1598"
            }
        },
        "GROUP": {
            "5ba38da500b752b0f46d13186030b7ad": {
                "name": "Default Group",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "5ba38da500b752b0f46d13186030b7ad"
            }
        },
        "PARAM": {
            "62d1eee400f8578895166ee91a83f97a": {
                "name": "Asset Type",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee400f8578895166ee91a83f97a"
            },
            "62d1eee50001407c713514a8970b58e4": {
                "name": "Keywords",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee50001407c713514a8970b58e4"
            },
            "62d1eee5000333ac3981ea4f3df6d88e": {
                "name": "Permitted Uses",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000333ac3981ea4f3df6d88e"
            },
            "62d1eee5000b188e9ec8039a097fc7ab": {
                "name": "File Format",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000b188e9ec8039a097fc7ab"
            },
            "62d1eee500100c159fd5f838ce560507": {
                "name": "CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee500100c159fd5f838ce560507"
            },
            "62d9c988001c1f23954dbb9d646335b5": {
                "name": "Other CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c988001c1f23954dbb9d646335b5"
            },
            "62d9c9880070f546cf4c798ea6c3eaa4": {
                "name": "Other Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9880070f546cf4c798ea6c3eaa4"
            },
            "62d9c990006258baf1b40f2569c3eab7": {
                "name": "Target Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c990006258baf1b40f2569c3eab7"
            }
        }
    }
}
```

>[!NOTE]
>
>L&#39;ID necessario per eseguire l&#39;installazione è il campo `id`. In questo esempio, il campo `id` è terzo dall&#39;alto e ha un valore che inizia con `c0bc79bd`.

### Eseguire un’installazione

>[!IMPORTANT]
>
>Prima di eseguire un&#39;installazione, è necessario eseguire una pre-esecuzione. Quando esegui l’installazione, utilizzerai l’ID generato dalla pre-esecuzione.
>
>Se sono state apportate modifiche all’ambiente di destinazione (l’ambiente in cui viene distribuito il pacchetto) dopo l’esecuzione della pre-esecuzione, si consiglia di eseguirla di nuovo. Se non esegui nuovamente la pre-esecuzione, l’esecuzione potrebbe non essere completata con precisione o l’installazione potrebbe non riuscire.
>
>Per istruzioni sull&#39;esecuzione di una pre-esecuzione, vedere [Eseguire una pre-esecuzione](#execute-a-pre-run).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

Questa chiamata avvia un tentativo di installazione di un pacchetto di promozione nell’ambiente di destinazione identificato nell’URL di POST.

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

#### Risposta

```
202
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

#### Risposta

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
        "status": "INSTALLED",
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

Questa chiamata restituirà il `translationMap` finale prodotto dal servizio di installazione per un&#39;installazione specifica.

Ogni record indicherà quale era il `action` prescritto e se l&#39;azione è stata eseguita correttamente o meno.

Per i record con CREATE `action` il campo `targetId` verrà impostato con il valore del record appena creato nel sistema di destinazione. Inoltre, il campo `installationStatus` verrà impostato su INSTALLATO.

Per i record con USEEXISTING `action` verrà impostato anche il campo `targetId` e il campo `installationStatus` verrà impostato su REGISTERED. Ciò significa che il processo di mappatura è stato completato e che il servizio di installazione riconosce di aver valutato il record e non c&#39;è nulla su cui intervenire.

Se il record contiene un elemento CREATE `action` ma la creazione del record non riesce, `installationStatus` verrà impostato su FAILED e verrà fornito anche il motivo dell&#39;errore.

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

#### Risposta

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
    "status": "INSTALLED",
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

## Sovrascrittura

Si tratta di un processo in tre fasi.

1. Creare una mappa di traduzione (analogamente alla fase di &quot;preparazione dell’installazione&quot;)
1. Modificare la mappa di traduzione generata, impostando i campi `action` e `targetId` per qualsiasi oggetto che si desidera sovrascrivere. L&#39;azione deve essere `OVERWRITING` e `targetId` deve essere l&#39;UUID dell&#39;oggetto da sovrascrivere
1. Eseguire l&#39;installazione.

* [Passaggio 1: creare una mappa di traduzione](#step-1---create-a-translation-map)
* [Passaggio 2: modificare la mappa di traduzione](#step-2---modify-the-translation-map)
* [Passaggio 3: installare](#step-3---install)

### **Passaggio 1 - Creare una mappa di traduzione**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/translation-map
```

#### Corpo

Nessuno

#### Risposta

Mappa di traduzione con stato `202 - OK`

```json
{
    {objcode}: {
        {object uuid}: {
            "targetId": {uuid of object in destination},
            "action": {installation action},
            "name": {name of the object},
            "isValid": true
        },
        {...more objects}
    },
    {...more objcodes}
}
```


#### Esempio

```json
{
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "CREATE",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
```

### Passaggio 2: modificare la mappa di traduzione

Nessun endpoint per questo passaggio.

1. Nella mappa di traduzione restituita nel [Passaggio 1 - Creare una mappa di traduzione](#step-1---create-a-translation-map), controllare l&#39;elenco degli oggetti che verranno installati.
1. Aggiornare il campo di azione di ogni oggetto all&#39;azione di installazione desiderata.
1. Convalida `targetId` su ciascun oggetto. Se l&#39;azione impostata è `USEEXISTING` o `OVERWRITING`, `targetId` deve essere impostato sull&#39;UUID dell&#39;oggetto di destinazione nell&#39;ambiente di destinazione. Per qualsiasi altra azione, targetId deve essere una stringa vuota.

   >[!NOTE]
   >
   >`targetId` è già popolato se è stato rilevato un conflitto.

### **Passaggio 3 - Installa**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/install
```

#### Corpo

Questo è un oggetto con un singolo campo `translationMap`, che deve corrispondere alla mappa di traduzione modificata da [Passaggio 2 - Modifica la mappa di traduzione](#step-2---modify-the-translation-map).

```json
{
    "translationMap": {
        {objcode}: {
            {object uuid}: {
                "targetId": {uuid of object in destination},
                "action": {installation action},
                "name": {name of the object},
                "isValid": true
            },
            {...more objects}
        },
        {...more objcodes}
    }
}
```


#### Esempio

```json
{
    "translationMap": {
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "OVERWRITING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
}
```

#### Risposta

La risposta include lo stato `{uuid of the created installation}` e `202 - ACCEPTED`.

Esempio: `b6aa0af8-3520-4b25-aca3-86793dff44a6`

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
