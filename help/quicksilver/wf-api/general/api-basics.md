---
content-type: api
navigation-topic: general-api
title: Nozioni di base sulle API
description: Nozioni di base sulle API
author: Becky
feature: Workfront API
role: Developer
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: be11c7417023ce2f310fce3e0cf77724d101b89e
workflow-type: tm+mt
source-wordcount: '4461'
ht-degree: 96%

---


# Nozioni di base sulle API

L’obiettivo dell’API Adobe Workfront è semplificare la creazione di integrazioni con Workfront introducendo un’architettura RESTful che funziona tramite HTTP. Questo documento presuppone una familiarità con le risposte REST e JSON e descrive l’approccio adottato dall’API Workfront.

Acquisire familiarità con lo schema Workfront ti aiuterà a comprendere le relazioni tra database che possono essere utilizzate per estrarre dati da Workfront a scopo di integrazione.

## Limiti e linee guida

Per garantire prestazioni coerenti del sistema Workfront on demand, l’API Workfront limita i thread API simultanei. Questo guardrail impedisce i problemi di sistema causati da chiamate API offensive. L’ambiente sandbox dispone dello stesso limite di thread API simultanei, che consente a clientela e partner di testare con precisione le chiamate API prima di rilasciare il codice in produzione.

Per gli ambienti di produzione, anteprima e test delle unità, le richieste degli utenti finali hanno una lunghezza URI massima di 8892 byte, in quanto vengono instradate tramite la rete CDN di Workfront (Akamai). Questo limite si applica solo agli URI instradati attraverso la rete CDN.

### Liberatoria

Qualsiasi utilizzo dell’API deve essere testato nell’ambiente Beta di Workfront prima di essere eseguito nell’ambiente di produzione. Se un cliente utilizza l’API per un processo che Workfront ritiene ragionevolmente oneroso per il software on demand (ovvero, il processo causa un effetto sostanzialmente negativo sulle prestazioni del software per altra clientela), Workfront si riserva il diritto di richiedere che il cliente interrompa tale processo. Se il cliente non si conforma e il problema persiste, Workfront si riserva il diritto di terminare il processo.

## URL API Workfront

Per informazioni sull’URL che utilizzerai per chiamare l’API Workfront, consulta [Formato dominio per le chiamate API Adobe Workfront](/help/quicksilver/wf-api/tips-tricks-and-troubleshooting/locate-domain-for-api.md).

## Nozioni di base su REST

Questa sezione fornisce un’introduzione di alto livello su come interagire con l’API REST di Workfront per i seguenti principi REST:

### URI oggetto

A ogni oggetto nel sistema viene assegnato un URI univoco costituito dal tipo di oggetto e dall’ID. Gli esempi seguenti mostrano gli URI che descrivono tre oggetti univoci:

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

Il tipo di oggetto non distingue tra maiuscole e minuscole e può essere l’abbreviazione ObjCode (ad esempio proj) o il nome dell’oggetto alternativo (project).

Per un elenco di oggetti, ObjCodes validi, e campi oggetto, consulta  [API Explorer](../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Nel contesto dell’API Workfront, un modulo personalizzato è un oggetto `Category` e un campo personalizzato è un oggetto `Parameter`.

### Operazioni

Gli oggetti vengono manipolati inviando una richiesta HTTP al relativo URI univoco. L’operazione da eseguire è specificata dal metodo HTTP.

I metodi HTTP standard corrispondono alle operazioni seguenti:

* **GET**: recupera un oggetto in base all’ID, cerca tutti gli oggetti in base a una query, esegue rapporti o esegue query denominate
* **POST**: inserisce un nuovo oggetto
* **PUT**: modifica un oggetto esistente
* **DELETE**: elimina un oggetto

Per ovviare alle carenze dei client o ai limiti di lunghezza del protocollo, il parametro di metodo può essere utilizzato per sostituire il comportamento HTTP. Ad esempio, un’operazione GET può essere implementata inserendo il seguente URI:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=get<br>GET /attask/api/v15.0/project/4c78...54d0?method=get</pre>

### Risposta

A ogni richiesta viene fornita una risposta in formato JSON. La risposta dispone di un attributo dati se la richiesta ha avuto esito positivo o di un attributo errore se si è verificato un problema. Ad esempio, la richiesta

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

restituisce una risposta JSON simile alla seguente:


<pre>{<br>    "data": [<br>        {<br>            "percentComplete": 0,<br>            "status": "CUR",<br>            "priority": 2,<br>            "name": "Progetto appena creato",<br>            "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>Quando si esegue una richiesta GET tramite la barra degli indirizzi del browser, non è necessario includere sessionID come parte della richiesta.

È stata aggiunta una protezione speciale per le richieste PUT, POST e DELETE. Qualsiasi richiesta che determini la scrittura o l’eliminazione dal database può essere eseguita solo se l’**sessionID=abc123** è incluso nell’URI. Gli esempi seguenti mostrano come questo dovrebbe cercare una richiesta DELETE:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET /attask/api/v15.0/project/4c78...54d0?method=delete&amp;sessionID=abc123</pre>

### Autenticazione

L’API autentica ciascuna richiesta per garantire che il client abbia accesso alla visualizzazione o alla modifica di un oggetto richiesto.

L’autenticazione viene eseguita trasmettendo un ID sessione che può essere assegnato utilizzando uno dei seguenti metodi:

#### Autenticazione tramite intestazione della richiesta

Il metodo preferito per l’autenticazione consiste nel trasmettere un’intestazione di richiesta denominata SessionID contenente il token di sessione. Questo presenta il vantaggio di essere progetto dagli attacchi di [Cross-Site Request Forgery (CSRF, Falsificazione di richieste tra siti)](https://it.wikipedia.org/wiki/Cross-site_request_forgery) e di non interferire con l’URI ai fini della memorizzazione in cache.

Di seguito è riportato un esempio di intestazione di richiesta:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### Autenticazione basata su cookie

L’API utilizza la stessa autenticazione basata su cookie usata dall’interfaccia utente web per il sistema. In questo modo, se un client accede a Workfront utilizzando l’interfaccia utente web, tutte le chiamate AJAX effettuate all’interno dello stesso browser utilizzano la stessa autenticazione.

>[!NOTE]
>
>Al fine di proteggere da possibili attacchi CSRF (Cross Site Request Forgery), questo metodo di autenticazione è disponibile solo per le operazioni di sola lettura.

## Accesso

>[!IMPORTANT]
>
>Workfront non consiglia più di utilizzare l’endpoint `/login` o le chiavi API. Utilizza invece uno dei seguenti metodi di autenticazione:
>
>* Autenticazione server con JWT
>* Autenticazione utente con OAuth2
>
>Per istruzioni sulla configurazione di questi metodi di autenticazione, consulta [Creare applicazioni OAuth2 per le integrazioni Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>
>Per istruzioni sull’utilizzo dell’autenticazione server in Workfront, consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso JWT](../../wf-api/api/oauth-app-jwt-flow.md)
>
>Per istruzioni sull’utilizzo dell’autenticazione utente in Workfront, consulta [Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso del codice di autorizzazione](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
>
>La procedura descritta in questa sezione si applicava solo alle organizzazioni che non erano ancora state caricate su Adobe Business Platform. Poiché tutte le organizzazioni sono ora state integrate in Adobe Business Platform, **l&#39;accesso a Workfront tramite l&#39;API Workfront non è più disponibile**.
>
>Per un elenco delle procedure che differiscono a seconda che l&#39;organizzazione sia stata integrata o meno in Adobe Business Platform, vedi [Differenze di amministrazione tra Adobe Workfront e Adobe Business Platform](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Utilizzando un nome utente e una password validi, puoi utilizzare la seguente richiesta per ottenere un ID sessione:

```
POST /attask/api/v15.0/login?username=admin&password=user
```

Questa operazione imposta un cookie per autenticare le richieste future e restituire inoltre una risposta JSON con il sessionID appena creato, l’userID dell’utente connesso e altri attributi di sessione.

>[!NOTE]
>
>Se disponi di un utente API designato che è anche un amministratore, Workfront ti consiglia vivamente di utilizzare una chiave API per accedere.

**Generazione di una chiave API**

Puoi generare una chiave API quando accedi al sistema come tale utente, come illustrato nell’esempio seguente:


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**Recupero di una chiave API generata in precedenza**

Puoi anche recuperare una chiave API che è stata generata in precedenza per un particolare utente eseguendo getApiKey:


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

Puoi quindi utilizzare questo risultato per autenticare qualsiasi chiamata API aggiungendo “apiKey” come parametro di richiesta, in sostituzione di sessionID o di nome utente e password. Questo è vantaggioso dal punto di vista della sicurezza.

La seguente richiesta è un esempio di recupero di dati da un progetto utilizzando apiKey:

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**Annullamento della validità di una chiave API**

Se il valore apiKey è stato compromesso, puoi eseguire “clearApiKey”, che invalida la chiave API corrente, come illustrato nell’esempio seguente:

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

Una volta annullata, puoi eseguire nuovamente getApiKey per generare una nuova chiave API.

### Disconnessione

Al termine di una sessione, puoi utilizzare la seguente richiesta per disconnettere l’utente, impedendo qualsiasi ulteriore accesso con sessionID.

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

Il valore sessionID da disconnettere può essere specificato come cookie, intestazione di richiesta o parametro di richiesta.

Per disconnettere un utente:

1. Passa alla schermata di accesso, senza però accedere.
1. Modifica l’URL in /attask/api/v15.0/project/search.\
   Nota che la pagina non può essere trovata.
1. Sostituisci la parola *search* con login?username=admin&amp;password=user, sostituendo il tuo nome utente e la tua password con *admin* e *user\
   *Questa sessione viene memorizzata nel browser come cookie e non deve essere ripetuta in ogni richiesta GET successiva.

1. Modifica nuovamente l’URL **/attask/api/v15.0/project/search**.
1. Osserva la risposta fornita.

Quando esegui richieste PUT, POST e DELETE, devi sempre includere l’ID sessione fornito dopo l’accesso.

## Comportamento di GET

Utilizza il metodo HTTP GET per recuperare uno o più oggetti ed eseguire i rapporti.

### Recupero di oggetti

Puoi migliorare la ricerca di oggetti utilizzando modificatori e filtri.

#### Recupero di un oggetto mediante l’ID oggetto

Se conosci l’ID di un oggetto, puoi recuperarlo accedendo al relativo URI univoco. Ad esempio, la richiesta

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

restituisce una risposta simile a quanto segue:

<pre>{<br>    "percentComplete": 0,<br>    "status": "CUR",<br>    "priority": 2,<br>    "name": "Brand New Project",<br>    "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>}</pre>


Puoi recuperare più oggetti nella stessa richiesta specificando il parametro di richiesta ID e fornendo un elenco ID separato da virgole, come mostrato nell’esempio seguente:


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

La richiesta /attask/api/v15.0/project?id=... corrisponde alla richiesta `/attask/api/v15.0/project/...`.

#### Recupero di un oggetto tramite l’URI

Se desideri recuperare un oggetto in base a criteri diversi dall’ID, puoi cercare l’URI.

Ad esempio, puoi utilizzare la seguente richiesta per restituire un elenco di tutti i progetti nel sistema:

```
GET /attask/api/v15.0/project/search
```

Puoi specificare i filtri utilizzando i parametri della richiesta come coppie nome-valore. Ad esempio, l’esempio seguente mostra una richiesta per individuare tutti i progetti correnti:

```
GET /attask/api/v15.0/project/search?status=CUR
```

La richiesta seguente individua tutte le attività non ancora completate e assegnate a un utente di nome John.

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### Utilizzo dei modificatori di ricerca

Nella tabella seguente sono elencati alcuni dei modificatori che è possibile utilizzare con l’API Workfront.

| **Modificatore** | **Descrizione** | **Esempio** |
| --- | --- | --- |
| eq | restituisce risultati con stato chiuso | <pre>...status=cls&amp;status_Mod=eq...</pre> |
| ne | restituisce risultati che non sono nello stato chiuso | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| gte | restituisce risultati con una percentuale di completamento maggiore o uguale a 50 | <pre>...percentComplete=50&amp;percentComplete_Mod=get...</pre> |
| lte | restituisce risultati con una percentuale di completamento minore o uguale a 50 | <pre>...percentComplete=50&amp;percentComplete_Mod=lte...</pre> |
| isnull | restituisce risultati in cui la descrizione è Null | <pre>...description_Mod=isnull...</pre> |
| notnull | restituisce risultati in cui la descrizione non è Null | <pre>...description_Mod=notnull...</pre> |
| contiene | restituisce i risultati in cui il nome contiene “Workfront” | <pre>...name=Workfront&amp;name_Mod=contains</pre> |
| tra | restituisce risultati con una data di inserimento compresa negli ultimi 7 giorni | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between...</pre> |

{style="table-layout:auto"}

>[!NOTE]
>
>Le richieste di ricerca fanno distinzione tra maiuscole e minuscole. Se ricevi un errore, assicurati che  **_Mod** e **_Range** abbiano le maiuscole corrette.

#### Utilizzo delle istruzioni OR

Puoi migliorare una ricerca aggiungendo un parametro che includa “OR” e un numero per indicare il livello di un filtro o di una serie di filtri.

Un’istruzione OR restituisce solo i record nella chiamata API che soddisfano i criteri di filtro dell’istruzione OR. I filtri non sono impliciti tra i livelli di istruzione OR.

Ad esempio, se desideri filtrare per

* Attività il cui nome contiene “Pianificazione” OR
* Attività in un portfolio denominato “FixedAssets” AND assegnate a qualcuno con un nome contenente “Steve” OR
* Attività con un’attività principale denominata “Attività finale”

quindi utilizza la seguente chiamata API con le relative istruzioni OR multiple:
<pre>GET /attask/api/v15.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>&amp;OR:1:portfolio:name=FixedAssets<br>&amp;OR:1:portfolio:name_Mod=eq<br>&amp;OR:1:assignedTo:name=Steve<br>&amp;OR:1:assignedTo:name_Mod=cicontains<br>&amp;OR:2:parent:name=Final Task<br>&amp;OR:2:parent:name_Mod=eq
</pre>

#### Utilizzo dei parametri del filtro

Un potenziale problema nell’utilizzo dei parametri URL per i filtri di ricerca è che Workfront analizza alcuni parametri prima di verificare la presenza di diversi metodi di autenticazione (ad esempio nome utente, password, apiKey, cookie). In questo caso, i parametri non vengono utilizzati come filtri nella chiamata. 

Per evitare questo problema, puoi inserire questi valori nei parametri del filtro con formattazione JSON. Ad esempio, se desideri filtrare in base al nome utente testuser, anziché utilizzare 
<pre>/attask/api/v15.0/user/search?username=testuser@workfront.com</pre>passa il parametro URL in un filtro, come illustrato nell’esempio seguente:
<pre>/attask/api/v15.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### Utilizzo del parametro di richiesta mappa

Per impostazione predefinita, i dati restituiti da una ricerca sono un array JSON. A seconda del caso d’uso, potrebbe essere più efficiente ottenere il risultato come oggetto JSON indicizzato per ID. Questa operazione può essere eseguita utilizzando il parametro della richiesta mappa. Ad esempio, la richiesta 
<pre>/attask/api/v15.0/task/search?map=true</pre>restituisce una risposta indicizzata per ID simile alla seguente:
<pre>{<br>    "data": {<br>        "4c9a97db0000000f13ee4446b9aead9b": {<br>            "percentComplete": 0,<br>            "status": "NUOVo",<br>            "name": "prima attività",<br>            "ID": "4c9a97db0000000f13ee4446b9aead9b",<br>            "taskNumber": 1 <br>        },<br>        "4ca28ba600002024cd49e75bd43cf601": {<br>            "percentComplete": 0,<br>            "status": "INP:A",<br>            "name": "seconda attività",<br>            "ID": "4ca28ba600002024cd49e75bd43cf601",<br>            "taskNumber": 2 <br>        } <br>    } <br>}</pre>

#### Utilizzo del parametro di richiesta campi

Per impostazione predefinita, il recupero di un oggetto restituisce solo il sottoinsieme di campi più comunemente utilizzato.

Puoi utilizzare il parametro di richiesta campi per specificare che venga restituito un elenco separato da virgole di campi specifici. Ad esempio, la richiesta
<pre>/attask/api/v15.0/task/search?fields=plannedStartDate,priority</pre>restituisce una risposta simile a quanto segue:
<pre>{<br>    "priority": 2,<br>    "name": "first task",<br>    "ID": "4c7c08fa0000002ff924e298ee148df4",<br>    "plannedStartDate": "2010-08-30T09:00:00:000-0600" <br>}</pre>

>[!NOTE]
>
>Questi nomi di campo fanno distinzione tra maiuscole e minuscole.

Per un elenco dei possibili riferimenti ai campi, consulta [API Explorer](../../wf-api/general/api-explorer.md)

#### Ricerca di oggetti nidificati

È possibile cercare oggetti nidificati. Per impostazione predefinita, gli oggetti nidificati vengono restituiti solo con il nome e l’ID. Ad esempio, per ottenere tutti i problemi insieme ai relativi proprietari, utilizza la seguente richiesta:
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>Se sono necessarie ulteriori informazioni, puoi richiedere un campo nidificato utilizzando la sintassi dei due punti. Ad esempio, la richiesta seguente cerca tutti i problemi insieme al nome, all’ID, al titolo e al numero di telefono del proprietario
<pre>/attask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>e restituisce quanto segue: 
<pre>{<br>    "name": "un problema importante",<br>    "ID": "4c78285f00000908ea8cfd66e084939f",<br>    "owner": {<br>        "title": "Specialista delle operazioni",<br>        "phoneNumber": "555-1234",<br>        "name": "Utente amministratore",<br>        "ID": "4c76ed7a0000054c172b2c2d9f7f81c3" <br>    } <br>}</pre>

#### Recupero raccolte nidificate

È possibile recuperare raccolte nidificate di oggetti. Ad esempio, per ottenere un progetto con tutte le relative attività, utilizza la seguente richiesta:
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>La richiesta seguente ottiene le assegnazioni delle attività:
<pre>/attask/api/v15.0/task/search?fields=assignments</pre>

#### Ricerca di più campi nidificati

Per impostazione predefinita, vengono restituiti solo il nome e l’ID di ciascuna attività, ma è possibile specificare ulteriori campi nidificati con la sintassi dei due punti. Per visualizzare tutti i campi disponibili per un oggetto o una raccolta correlata, è sufficiente aggiungere due punti e un asterisco al riferimento all’oggetto o alla raccolta.
<pre>/attask/api/v15.0/task/search?fields=assegnazioni:*</pre>

#### Recupero di dati personalizzati

Puoi recuperare campi dati personalizzati con il prefisso “DE:”. Ad esempio, per richiedere un progetto con un parametro denominato “CustomText”, utilizza la seguente richiesta:
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>che restituirebbe
<pre>{<br>    "name": "progetto dati personalizzati",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    "DE:CustomText": "attività b" <br>}</pre>Inoltre puoi recuperare tutti i dati personalizzati per un oggetto richiedendo il campo parameterValues. Ad esempio, 
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>restituisce dati simili ai seguenti:
<pre>{<br>    "name": "custom data project",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    parameterValues: { <br>        "DE:CustomText": "task b", <br>        "DE:CustomNumber": 1.4, <br>        "DE:CustomCheckBoxes": ["first", "second", "third"] <br>    } <br>}</pre>

#### Utilizzo di query denominate

Alcuni tipi di oggetto dispongono di ricerche denominate che vengono comunemente eseguite e sono disponibili aggiungendo il nome della query alla fine dell’URI del tipo di oggetto. Ad esempio, la seguente richiesta recupera gli elementi di lavoro (attività e problemi) a cui l’utente è attualmente assegnato:
<pre>/attask/api/v15.0/work/myWork</pre>Le query denominate supportano la richiesta del parametro fields per recuperare campi aggiuntivi. Alcune query denominate accettano anche filtri aggiuntivi. Per un elenco delle query denominate consentite per un oggetto, consulta la scheda Azione per l’oggetto nella [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

#### Utilizzo di `Count`

Puoi utilizzare `count` per restituire il numero di risultati corrispondenti alla query. Questo può essere utile quando non hai bisogno dei dati nei risultati. Restituendo solo il conteggio, il server può elaborare la richiesta più rapidamente e risparmiare larghezza di banda. Ad esempio, la richiesta
<pre>GET /attask/api/v15.0/project/count?status=CUR</pre>restituisce il numero di risultati nel formato seguente:
<pre>{<br>    "count": 3 <br>}</pre>La restituzione di un conteggio è un trasferimento di dati molto più piccolo rispetto a quando vengono restituiti gli oggetti completi. La sintassi è identica al comando di ricerca.

### Richiedere un rapporto

Puoi eseguire una richiesta di rapporto di cui desideri ottenere solo l’aggregato di alcuni campi con uno o più raggruppamenti. Come mostrato nell’esempio seguente, la sintassi del rapporto è la stessa della sintassi per l’API SOAP:
<pre>GET /attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>che restituisce il seguente risultato
<pre>{<br>    "Primo progetto": { <br>        "sum_hours": 15 <br>    }, <br>     "Secondo progetto": { <br>        "sum_hours": 30 <br>    } <br>}</pre>L’aggiunta del parametro $$ROLLUP=true include un totale a ciascun livello di raggruppamento:
<pre>{<br>    "Primo progetto": { <br>        "sum_hours": 15 <br>    }, <br>    "Secondo progetto": { <br>        "sum_hours": 30 <br>    }, <br>    "$$ROLLUP": { <br>        "sum_hours": 45 <br>    } <br>}</pre>

### Ordinamento dei risultati della query nell’API

Puoi ordinare i risultati in base a qualsiasi campo aggiungendo quanto segue alla chiamata API:

&amp;entryDate_Sort=asc

Se ad esempio desideri ordinare in base all’attività Data inizio pianificata, rimuovi entryDate e sostituiscilo con plannedCompletionDate.

Questa operazione funziona per la maggior parte dei campi in Workfront.

### Considerazione dei limiti delle query

Quando esegui una query su un oggetto, è necessario prestare particolare attenzione alla relazione tra oggetti correlati e limitazioni della ricerca. Ad esempio, come illustrato nella tabella seguente, una query per progetti può restituire non più di 2.000 progetti. Questi 2.000 progetti sono considerati “oggetti principali”. Se esegui una query per il campo Attività dei progetti, il campo Attività, che è una raccolta, diventa un oggetto secondario dell’oggetto principale Progetto. Una query per il campo Attività può includere migliaia di attività nei progetti. In totale, il numero combinato di oggetti (progetti e attività) restituiti non può superare il massimo di 50.000.

Per garantire prestazioni ottimali, la tabella seguente mostra le limitazioni imposte alle richieste di ricerca. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Risultato della query</th> 
   <th>Limitazione</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td width="200">Numero predefinito di risultati</td> 
   <td>100</td> 
   <td> Se nel filtro della query non è specificato alcun limite (ad esempio, $$LIMIT), il risultato non può contenere più di 100 oggetti principali. <br>Per istruzioni su come ignorare questa limitazione, consulta <a href="#using-paginated-responses" class="MCXref xref">Utilizzo di risposte paginate</a>. </td> 
  </tr> 
  <tr> 
   <td>Numero massimo di risultati</td> 
   <td>2.000</td> 
   <td>Il filtro della query (ovvero $$LIMIT) può restituire non più di 2.000 risultati. Per ulteriori informazioni, consulta “Risposte paginate”.</td> 
  </tr> 
  <tr> 
   <td>Profondità massima campo</td> 
   <td>4</td> 
   <td>Durante l’identificazione dei campi che desideri visualizzare, non puoi spostarti di oltre quattro livelli dall’oggetto di cui esegui la query.</td> 
  </tr> 
  <tr> 
   <td>Numero massimo di oggetti</td> 
   <td>50.000</td> 
   <td>Il set di risultati non può includere 50.000 oggetti principali e secondari.</td> 
  </tr> 
  <tr> 
   <td>Numero massimo di campi</td> 
   <td nowrap>1.000.000</td> 
   <td>Se il set di risultati è inferiore a 50.000 oggetti, i risultati possono includere al massimo 1.000.000 campi.</td> 
  </tr> 
  <tr> 
   <td>Numero massimo di creazioni/aggiornamenti batch</td> 
   <td>100</td> 
   <td>Il limite massimo per la creazione o l’aggiornamento batch è 100.</td> 
  </tr> 
 </tbody> 
</table>

### Utilizzo di risposte paginate {#using-paginated-responses}

Per ignorare il limite predefinito di query per il numero di risultati e consentirne 200, puoi includere il filtro `$$LIMIT=200` nella query, come illustrato nell’esempio seguente:
<pre>GET /attask/api/v15.0/project/search?$$LIMIT=200</pre>

Per garantire affidabilità e prestazioni per altri tenant nel sistema, il limite massimo di risultati consentito per query è di 2.000 oggetti. Se tenti di specificare un limite maggiore, verrà visualizzato un messaggio di errore `IllegalArgumentException`. 

Pertanto, è consigliabile considerare l’utilizzo di risposte paginate per set di dati di grandi dimensioni. Per specificare il primo risultato da restituire, aggiungi il filtro `$$FIRST`. Ad esempio, la seguente richiesta restituisce i risultati 201-250 per una query:
<pre>GET /attask/api/v15.0/project/search?$$FIRST=200&amp;$$LIMIT=50</pre>

Nell’esempio precedente, `$$FIRST=200` restituisce il 201° risultato. `$$FIRST=0` restituirebbe il primo risultato. Può essere utile considerare il valore $$FIRST come il numero di risultati che desideri ignorare prima di restituire i risultati.

Per assicurarti che i risultati siano paginati correttamente, utilizza un parametro di ordinamento. Questo consente di restituire i risultati nello stesso ordine, in modo che la paginazione non ripeta né ignori dei risultati. Ad esempio, per ordinare utilizzando l’ID oggetto, utilizza `ID_Sort=asc`.

### Creazione di una regola di accesso

Puoi creare una regola di accesso per determinare chi può accedere a un oggetto. Di seguito sono riportati alcuni esempi di regole di accesso che puoi impostare:

Per impostare un progetto in modo che venga condiviso solo con un utente con ID “abc123”, utilizza la seguente richiesta:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=put &amp;updates={ accessRules: [ {accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'} ] }</pre>In alternativa, per condividere solo con una nuova persona e mantenere intatte le autorizzazioni esistenti:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>Per recuperare le regole di accesso esistenti:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## Comportamento delle richieste POST

La richiesta POST inserisce un nuovo oggetto. La sintassi è identica alla richiesta PUT, ma con alcune eccezioni. Poiché il nuovo oggetto non esiste ancora, non dispone di un ID. Per questo motivo, l’URI non include l’ID.

### Creazione di un oggetto

Di seguito è riportato un esempio di richiesta di creazione di un nuovo progetto:
<pre>POST /attask/api/v15.0/project?name=New Project</pre>La risposta include il progetto appena creato, il nuovo ID e tutti gli altri campi specificati.

### Copia di un oggetto

Alcuni oggetti supportano la copia. Per questi tipi di oggetto, è possibile creare nuovi oggetti pubblicandoli con un parametro copySourceID. Ad esempio, la richiesta seguente copia il progetto specificato e gli assegna un nuovo nome:

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### Caricamento di documenti

Puoi caricare i documenti tramite il seguente URL API:
<pre>POST /attask/api/v15.0/upload</pre>L’API prevede che il tipo di contenuto sia multipart/form-data. Il nome del parametro per il file deve essere uploadedFile. Il server restituisce i seguenti dati JSON:
<pre>{<br>    "handle": "4c7c08fa0000002ff924e298ee148df4"<br>}</pre>Durante la creazione di un documento Workfront, puoi utilizzare l’handle e pubblicare il seguente URL:
<pre>POST /attask/api/v15.0/document?updates={<br>    name: aFileName,<br>    handle: abc...123, (handle ottenuto dal caricamento del file)<br>    docObjCode: PROJ, (o TASK, OPTASK, ecc.)<br>    objID: abc...123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br>}</pre>

## Comportamento delle richieste PUT

Le richieste PUT vengono utilizzate per aggiornare un oggetto esistente.

La risposta per una richiesta PUT è identica a una richiesta GET. In entrambi i casi, il server restituisce il nuovo stato dell’oggetto dopo l’aggiornamento. Tutte le regole utilizzate per modificare una risposta a una richiesta GET funzionano anche con la richiesta PUT, ad esempio specificando campi aggiuntivi da restituire, dati personalizzati e così via.

### Modifica di oggetti

Gli aggiornamenti agli oggetti vengono sempre eseguiti per ID utilizzando l’URI univoco dell’oggetto. I campi da aggiornare vengono specificati come parametri di richiesta. Ad esempio, per modificare il nome di un progetto puoi inviare una richiesta simile alla seguente:
<pre>PUT /attask/api/v15.0/project/4c7...?name=Nome nuovo progetto <br>PUT /attask/api/v15.0/project?id=4c7..&amp;name=Nuovo nome progetto</pre>Poiché l’aggiornamento richiede un ID, questa operazione non riuscirà (senza inserimento) se l’oggetto non esiste sul server.

### Specificare le modifiche JSON

Come mostrato nell’esempio seguente, puoi utilizzare il parametro della richiesta degli aggiornamenti per specificare i campi da aggiornare utilizzando la sintassi JSON:
<pre>PUT /attask/api/v15.0/project/4c7...?updates= <br>{<br>     nome: "Nuovo nome progetto", <br>     stato: "CUR", <br>     ... <br></pre>

### Esecuzione di aggiornamenti nidificati

Alcuni oggetti dispongono di raccolte private che possono essere aggiornate. Nell’esempio seguente viene illustrato come sovrascrivere le assegnazioni esistenti per una determinata attività:
<pre>PUT /attask/api/v15.0/task/4c7...?updates= <br>{<br>    assegnazioni: [ <br>        { <br>            assignedToID: "2222...54d0, <br>            assignmentPercent: 50,0 <br>        },{ <br>            roleID: "1111...54d0"<br>        } <br>    ] <br></pre>

>[!NOTE]
>
>Mentre gli aggiornamenti apportati al livello superiore sono parziali, gli aggiornamenti a una raccolta o a un oggetto nidificato sostituiscono completamente la raccolta esistente. Per modificare una singola assegnazione su un’attività senza interessare gli oggetti, utilizza una richiesta PUT sull’assegnazione anziché sull’attività.

Nell’esempio seguente un progetto diventa una coda pubblica dell’help-desk. Le proprietà della coda esistenti vengono sostituite.
<pre>PUT /attask/api/v15.0/project/4c7...?updates= <br>{ <br>    queueDef: { <br>        isPublic: 1 <br>    } <br></pre>

### Utilizzo del parametro della richiesta di azione

Alcuni oggetti supportano azioni aggiuntive che possono essere eseguite in aggiunta a semplici modifiche. Puoi specificare queste azioni utilizzando il parametro della richiesta di azione. Ad esempio, la richiesta seguente ricalcola la timeline per un determinato progetto:
<pre>PUT /attask/api/v15.0/project/4c7...?action=calculattimeline<br><br>or<br><br>PUT /attask/api/v15.0/project/4c7.../calculattimeline </pre>

### Spostare gli di oggetti

Di seguito viene illustrata la sintassi per lo spostamento di un’attività da un progetto a un altro:
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8..</pre>Un esempio per ogni tipo di azione è fornito qui: (??)
<pre>PUT /attask/api/v15.0/project/1234/approveApproval<br><br>PUT /attask/api/v15.0/project/1234/calculateFinance<br><br>PUT /attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT /attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT /attask/api/v15.0/project/1234/recallApproval<br><br>PUT /attask/api/v15.0/project/1234/rejectApproval<br><br>PUT /attask/api/v15.0/task/1234/move<br><br>PUT /attask/api/v15.0/workitem/1234/markViewed</pre>Solo l’azione Sposta richiede l’identificazione di attributi aggiuntivi per specificare il progetto in cui deve essere spostato l’elemento di lavoro.

Di seguito è riportato un esempio di ciascun tipo di azione: 
<pre>PUT /attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'}]}</pre>

### Condividere di oggetti

L’esempio seguente illustra la sintassi per la condivisione di un progetto con un team:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>Durante la modifica di un oggetto, puoi sostituire tutte le regole di accesso su un oggetto eseguendo una richiesta PUT e inviando aggiornamenti simili a quelli riportati di seguito:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',coreAction:'VIEW'}]}</pre>Nell’esempio seguente viene illustrata la sintassi per lo spostamento di un’attività da un progetto a un altro:
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8..</pre>

## Comportamento del metodo DELETE

Il metodo DELETE rimuove un oggetto. In tutti i casi, l’URI può includere il parametro force=true per fare in modo che il server rimuova i dati specificati e le relative dipendenze. Nell’esempio seguente, un’attività viene eliminata eseguendo il metodo HTTP DELETE su un URI:
<pre>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0?force=true <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0?force=true</pre>

## Aggiornamenti in blocco

Un’istruzione di aggiornamento in blocco aggiorna più oggetti contemporaneamente all’interno di una singola chiamata API. Una chiamata API per la creazione in blocco viene generata in modo simile a una normale chiamata di aggiornamento, come mostrato negli esempi seguenti:
<pre>PUT /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>oppure <pre>PUSH /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>che produce un risultato simile al seguente:
<pre>data: [{<br>    ID: "53ff8d3d003b438b57a8a784df38f6b3",<br>    name: "Test_Project_1",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>},<br>{<br>    ID: "53ff8d49003b43a2562aa34eea3b6b10",<br>    name: "Test_Project_2",<br>    objCode: "PROJ",<br>    percentComplete: 0usi,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>}]</pre>Puoi anche eseguire un aggiornamento in blocco simile al seguente:
<pre>PUT /attask/api/v15.0/proj?Umethod=PUT&amp;updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Edit"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_2_Edit"}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>che produce un risultato simile al seguente:
<pre>data: [{<br>     ID: "53ff8e15003b461d4560f7f65a440078",<br>     nome: "Test_Project_1_Edit",<br>     objCode: "PROJ",<br>     percentComplete: 0,<br>     plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>     plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>     priority: 0,<br>     projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>     status: "CUR"<br>},<br>{<br>    ID: "53ff8e19003b46238a58d303608de502",<br>    name: "Test_Project_2_Edit",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priorità: 0,<br>    projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>    status: "CUR"<br>}]</pre>Se desideri che tutte le operazioni vengano eseguite nella stessa transazione, aggiungi “atomic=true” alla chiamata API batch come parametro della richiesta. In questo modo, se una qualsiasi delle operazioni non riesce, tutte le operazioni vengono ripristinate.

>[!NOTE]
>
>Le operazioni batch atomiche possono restituire solo “success: true” o un errore.

