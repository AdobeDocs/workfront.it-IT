---
content-type: api
navigation-topic: general-api
title: Nozioni di base sulle API
description: Nozioni di base sulle API
author: John
feature: Workfront API
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: 4c3997f17c4d563849c475d3c0a080129a2b91eb
workflow-type: tm+mt
source-wordcount: '4405'
ht-degree: 0%

---


# Nozioni di base sulle API

L’obiettivo dell’API Adobe Workfront è semplificare la creazione di integrazioni con Workfront introducendo un’architettura REST-ful che opera tramite HTTP. Questo documento presuppone che tu abbia familiarità con le risposte REST e JSON e descrive l’approccio seguito dall’API Workfront.

Una familiarità con lo schema Workfront ti aiuterà a comprendere le relazioni del database che possono essere utilizzate per estrarre i dati da Workfront a scopo di integrazione.

## Limiti e linee guida

Per garantire prestazioni di sistema coerenti su richiesta di Workfront, ogni cliente è limitato a 10 thread API simultanei. L’ambiente Sandbox ha lo stesso limite in vigore, consentendo a clienti e partner di testare accuratamente le chiamate API prima di rilasciare il codice alla produzione.

Per gli ambienti di produzione, anteprima e test dell&#39;unità, le richieste degli utenti finali hanno una lunghezza massima URI di 8892 byte perché vengono instradate attraverso la rete CDN Workfront (Akamai). Questo limite si applica solo agli URI instradati attraverso la rete CDN.

>[!NOTE]
>
>questo limite non è applicabile agli ambienti sandbox perché gli ambienti sandbox non vengono instradati attraverso la rete CDN.

### Disclaimer

Qualsiasi utilizzo dell’API deve essere testato nell’ambiente beta di Workfront prima di essere eseguito nell’ambiente di produzione. Se un cliente utilizza l’API per un processo che Workfront ritiene ragionevolmente oneroso per il software on-demand (ovvero, il processo causa un effetto sostanzialmente negativo sulle prestazioni del software per altri clienti), Workfront si riserva il diritto di richiedere che il cliente interrompa tale processo. Se il cliente non si conforma e il problema persiste, Workfront si riserva il diritto di interrompere il processo.

## Nozioni di base su REST

Questa sezione fornisce un’introduzione di alto livello su come interagire con l’API REST di Workfront per i seguenti principi REST:

### URI oggetto

A ogni oggetto del sistema viene assegnato un URI univoco composto dal tipo di oggetto e dall&#39;ID. Gli esempi seguenti mostrano gli URI che descrivono tre oggetti univoci:

```
/attask/api/v9.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v9.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v9.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

Il tipo di oggetto non distingue tra maiuscole e minuscole e può essere l’oggetto ObjCode abbreviato (ad esempio proj) o il nome dell’oggetto alternativo (progetto).

Per un elenco dei codici ObjCode validi, vedi  [Esplora API](../../wf-api/general/api-explorer.md).

### Operazioni

Gli oggetti vengono manipolati inviando una richiesta HTTP al proprio URI univoco. L&#39;operazione da eseguire è specificata dal metodo HTTP .

I metodi HTTP standard corrispondono alle seguenti operazioni:

* **GET** - Recupera un oggetto per ID, cerca tutti gli oggetti in base a una query, esegue rapporti o esegue query con nome
* **POST** - Inserisce un nuovo oggetto
* **PUT** - Modifica un oggetto esistente
* **DELETE** - Elimina un oggetto

Per ovviare alle carenze del client o ai limiti di lunghezza del protocollo, il parametro del metodo può essere utilizzato per ignorare il comportamento HTTP. Ad esempio, un’operazione GET può essere implementata pubblicando il seguente URI:
<pre>GET /attask/api/v9.0/project?id=4c78...54d0&amp;method=get<br>GET /attask/api/v9.0/project/4c78...54d0?method=get</pre>

### risposta

A ogni richiesta viene data una risposta in formato JSON. La risposta dispone di un attributo di dati se la richiesta è riuscita o di un attributo di errore in caso di problemi. Ad esempio, la richiesta

```
GET /attask/api/v9.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

restituisce una risposta JSON simile alla seguente:


<pre>{<br>    "data": [<br>        {<br>            "percentComplete": 0,<br>            "status": "CUR",<br>            "priorità": 2.<br>            "name": "Nuovo progetto di marchio",<br>            "ID": "4c7c08b2000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>Quando esegui una richiesta di GET tramite la barra degli indirizzi del browser, non è necessario includere sessionID come parte della richiesta.

È stata aggiunta una protezione speciale intorno alle richieste PUT, POST e DELETE. Qualsiasi richiesta che comporti la scrittura o l&#39;eliminazione dal database può essere eseguita solo se **sessionID=abc123** è incluso nell’URI. Gli esempi seguenti mostrano come cercare una richiesta DELETE:
<pre>GET /attask/api/v9.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET /attask/api/v9.0/project/4c78...54d0?method=delete&amp;sessionID=abc123</pre>

### Autenticazione

L’API autentica ogni richiesta per garantire che il client abbia accesso per visualizzare o modificare un oggetto richiesto.

L&#39;autenticazione viene eseguita passando un ID sessione che può essere assegnato utilizzando uno dei metodi seguenti:

#### Richiedi autenticazione intestazione

Il metodo di autenticazione preferito consiste nel passare un’intestazione di richiesta denominata SessionID contenente il token di sessione. Questo ha il vantaggio di essere al sicuro contro [Raccolta richieste intersito (CSRF)](http://en.wikipedia.org/wiki/Cross-site_request_forgery) attacca e non interferisce con l’URI a scopo di caching.

Esempio di intestazione di richiesta:

```
GET /attask/api/v9.0/project/search
SessionID: abc1234
```

#### Autenticazione dei parametri di richiesta

Puoi eseguire l’autenticazione passando un parametro di richiesta denominato sessionID, come illustrato nell’esempio seguente: 

```
GET /attask/api/v9.0/project/4c78821c0000d6fa8d5e52f07a1d54d0?sessionID=abc1234
```

#### Autenticazione basata su cookie

L’API utilizza la stessa autenticazione basata su cookie utilizzata dall’interfaccia utente Web per il sistema. Se un client accede a Workfront utilizzando l’interfaccia utente web, tutte le chiamate AJAX effettuate dallo stesso browser utilizzano la stessa autenticazione.

>[!NOTE]
>
>Al fine di proteggere dalla possibilità di attacchi CSRF (Cross Site Request Forgery), questo metodo di autenticazione è disponibile solo per operazioni di sola lettura.

## Accedi

>[!IMPORTANT]
Workfront sconsiglia più l&#39;utilizzo del `/login` chiavi endpoint o API. Utilizza invece uno dei seguenti metodi di autenticazione:
* Autenticazione server con JWT
* Autenticazione utente con OAuth2
>
Per istruzioni su come impostare questi metodi di autenticazione, vedi [Creare applicazioni OAuth2 per le integrazioni Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)
Per istruzioni sull&#39;utilizzo dell&#39;autenticazione server in Workfront, vedi [Configura e utilizza le applicazioni personalizzate OAuth 2 della tua organizzazione utilizzando il flusso JWT](../../wf-api/api/oauth-app-jwt-flow.md)
Per istruzioni sull’utilizzo dell’autenticazione utente in Workfront, consulta [Configura e utilizza le applicazioni personalizzate OAuth 2 della tua organizzazione utilizzando il flusso di codice di autorizzazione](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
La procedura descritta in questa sezione si applica solo alle organizzazioni che non sono ancora state integrate nell’Adobe Business Platform. L’accesso a Workfront tramite l’API Workfront non è disponibile se l’organizzazione è stata caricata su Adobe Business Platform.
Per un elenco delle procedure che differiscono a seconda che l’organizzazione sia stata imbarcata in Adobe Business Platform, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Utilizzando un nome utente e una password validi, puoi utilizzare la seguente richiesta per ottenere un ID sessione:

```
POST /attask/api/v9.0/login?username=admin&password=user
```

Questo imposta un cookie per autenticare le richieste future e restituisce una risposta JSON con l’ID sessione appena creato, l’ID utente dell’utente connesso e altri attributi di sessione.

>[!NOTE]
Se hai un utente API designato che è anche un amministratore, Workfront consiglia vivamente di utilizzare una chiave API per accedere.

**Generazione di una chiave API**

Puoi generare una chiave API quando accedi al sistema come utente, come illustrato nell’esempio seguente:


```
PUT /attask/api/v9.0/user?action=generateApiKey&username= username&password=password&method=put
```

**Recupero di una chiave API generata in precedenza**

Puoi anche recuperare una chiave API generata in precedenza per un particolare utente eseguendo getApiKey:


```
PUT /attask/api/v9.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

Puoi quindi utilizzare questo risultato per autenticare qualsiasi chiamata API aggiungendo &quot;apiKey&quot; come parametro di richiesta con questo valore al posto di sessionID o nome utente e password. Ciò è vantaggioso dal punto di vista della sicurezza.

La seguente richiesta è un esempio di recupero di dati da un progetto utilizzando apiKey:

```
GET /attask/api/v9.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**Annullare la validità di una chiave API**

Se il valore apiKey è stato compromesso, puoi eseguire &quot;clearApiKey&quot; che invalida la chiave API corrente, come mostrato nell’esempio seguente:

```
GET /attask/api/v9.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

Una volta cancellato, puoi eseguire nuovamente getApiKey per generare una nuova chiave API.

### Esci

Al termine di una sessione, puoi utilizzare la seguente richiesta per disconnettere l’utente, impedendo ulteriori accessi con sessionID.

```
GET /attask/api/v9.0/logout?sessionID=abc1234
```

L&#39;ID sessione da disconnettere può essere specificato come cookie, intestazione di richiesta o parametro di richiesta.

Per disconnettersi da un utente:

1. Passa alla schermata di accesso, ma non accedi.
1. Modifica l’URL in /attask/api/v9.0/project/search.\
   Impossibile trovare la pagina.
1. Sostituisci la parola *ricerca* con login?username=admin&amp;password=user, sostituendo nome utente e password *admin* e *utente\
   *Questa sessione viene memorizzata nel browser come cookie e non deve essere ripristinata in ogni richiesta di GET successiva.

1. Cambia di nuovo l’URL in **/attask/api/v9.0/project/search**.
1. Osserva la risposta fornita.

È sempre necessario includere sessionID fornito dopo l’accesso quando si eseguono richieste di PUT, POST e DELETE.

## Comportamento GET

Utilizzare il metodo HTTP GET per recuperare uno o più oggetti ed eseguire rapporti.

### Recupero oggetti

È possibile migliorare la ricerca di oggetti utilizzando modificatori e filtri.

#### Recupero di un oggetto con l’ID oggetto

Se si conosce l’ID di un oggetto, è possibile recuperare l’oggetto accedendo al relativo URI univoco. Ad esempio, la richiesta

```
GET /attask/api/v9.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

restituisce una risposta simile alla seguente:

<pre>{<br>    "percentComplete": 0,<br>    "status": "CUR",<br>    "priorità": 2.<br>    "name": "Nuovo progetto di marchio",<br>    "ID": "4c7c08b2000002de5ca1ebc19edf2d5" <br>}</pre>


È possibile recuperare più oggetti nella stessa richiesta specificando il parametro della richiesta id e fornendo un elenco di ID separati da virgole, come illustrato nell&#39;esempio seguente:


```
GET /attask/api/v9.0/project?id=4c78...54d0,4c78...54d1
```

Nota che la richiesta /attask/api/v9.0/project?id=... è la stessa della richiesta `/attask/api/v9.0/project/...` richiesta.

#### Recupero di un oggetto utilizzando l’URI

Se si desidera recuperare un oggetto in base a criteri diversi dall’ID, è possibile cercare l’URI.

Ad esempio, puoi utilizzare la seguente richiesta per restituire un elenco di tutti i progetti nel sistema:

```
GET /attask/api/v9.0/project/search
```

Puoi specificare i filtri utilizzando i parametri della richiesta come coppie nome-valore. Ad esempio, l’esempio seguente mostra una richiesta per trovare tutti i progetti correnti:

```
GET /attask/api/v9.0/project/search?status=CUR
```

La seguente richiesta trova tutte le attività non ancora completate e assegnate a un utente di nome John.

```
GET /attask/api/v9.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### Utilizzo dei modificatori di ricerca

Nella tabella seguente sono elencati alcuni dei modificatori utilizzabili con l’API Workfront.

| **Modificatore** | **Descrizione** | **Esempio** |
|---|---|---|
| eq | restituisce i risultati che si trovano nello stato di chiuso | <pre>...status=cls&amp;status_Mod=eq..</pre> |
| ne | restituisce risultati che non sono nello stato di chiuso | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| get | restituisce risultati con una percentuale di completamento maggiore o uguale a 50 | <pre>...percentComplete=50&amp;percentComplete_Mod=gte...</pre> |
| lite | restituisce risultati con una percentuale di completamento inferiore o uguale a 50 | <pre>...percentComplete=50&amp;percentComplete_Mod=lte...</pre> |
| isnull | restituisce i risultati in cui la descrizione è Null | <pre>...description_Mod=isnull...</pre> |
| notnull | restituisce risultati in cui la descrizione non è Null | <pre>...description_Mod=nonnull..</pre> |
| contiene | restituisce i risultati in cui il nome contiene &quot;Workfront&quot; | <pre>...name=Workfront&amp;name_Mod=contains...</pre> |
| tra | restituisce i risultati con una data di ingresso negli ultimi 7 giorni | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=tra...</pre> |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
Le richieste di ricerca sono sensibili all’uso di maiuscole e minuscole. Se ricevi un errore, assicurati  **_Mod** e **_Intervallo** avere la capitalizzazione corretta.

#### Utilizzo di istruzioni OR

Puoi migliorare una ricerca aggiungendo un parametro che include &quot;OR&quot; e un numero che indica il livello di un filtro o una serie di filtri.

Un&#39;istruzione OR restituisce solo i record nella chiamata API che soddisfano i criteri di filtro dell&#39;istruzione OR. I filtri non sono impliciti tra i livelli di istruzione OR.

Ad esempio, per filtrare

* Attività che hanno un nome contenente &quot;Planning&quot; OR
* Attività in un portfolio denominato &quot;FixedAssets&quot; E assegnate a qualcuno con un nome contenente &quot;Steve&quot; OR
* Attività che hanno un&#39;attività padre denominata &quot;Attività finale&quot;

quindi utilizza la seguente chiamata API con le relative istruzioni OR multiple:
<pre>GET /attask/api/v9.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>&amp;OR:1:portfolio:name=FixedAssets<br>&amp;OR:1:portfolio:name_Mod=eq<br>&amp;OR:1:assignedTo:name=Steve<br>&amp;OR:1:assignedTo:name_Mod=cicontains<br>&amp;OR:2:parent:name=Attività finale<br>&amp;OR:2:parent:name_Mod=eq
</pre>

#### Utilizzo dei parametri del filtro

Un potenziale insider nell’utilizzo dei parametri URL per i filtri di ricerca è che Workfront analizza alcuni parametri prima di verificare la presenza di diversi metodi di autenticazione (ad esempio, nome utente, password, apiKey, cookie). In questo caso, i parametri non vengono utilizzati come filtri nella chiamata di . 

Per evitare questo problema, puoi inserire questi valori nei parametri del filtro con formattazione JSON. Ad esempio, se desideri filtrare il nome utente testuser, invece di utilizzare 
<pre>/attask/api/v9.0/user/search?username=testuser@workfront.com</pre>passa il parametro URL in un filtro, come illustrato nell’esempio seguente:
<pre>/attask/api/v9.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### Utilizzo del parametro della richiesta di mappa

Per impostazione predefinita, i dati restituiti da una ricerca sono array JSON. A seconda del caso d’uso, potrebbe essere più efficiente ottenere il risultato come oggetto JSON indicizzato dall’ID. Questo può essere fatto utilizzando il parametro della richiesta di mappa. Ad esempio, la richiesta 
<pre>/attask/api/v9.0/task/search?map=true</pre>restituisce una risposta indicizzata da ID simile al seguente:
<pre>{<br>    "data": {<br>        "4c9a97db000000f13ee4446b9aead9b": {<br>            "percentComplete": 0,<br>            "status": "NEW",<br>            "name": "primo compito",<br>            "ID": "4c9a97db000000f13ee4446b9aead9b",<br>            "taskNumber": 1 <br>        },<br>        "4ca28ba60002024cd49e75bd43cf601": {<br>            "percentComplete": 0,<br>            "status": "INP:A",<br>            "name": "secondo compito",<br>            "ID": "4ca28ba60002024cd49e75bd43cf601",<br>            "taskNumber": 2 <br>        } <br>    } <br>}</pre>

#### Utilizzo del parametro di richiesta dei campi

Per impostazione predefinita, il recupero di un oggetto restituisce solo il sottoinsieme di campi più comunemente utilizzato.

È possibile utilizzare il parametro di richiesta dei campi per specificare un elenco separato da virgole di campi specifici restituiti. Ad esempio, la richiesta
<pre>/attask/api/v9.0/task/search?fields=ScheduledStartDate,priority</pre>restituisce una risposta simile alla seguente:
<pre>{<br>    "priorità": 2.<br>    "name": "primo compito",<br>    "ID": "4c7c08fa000002ff924e298ee148df4",<br>    "scheduledStartDate": "2010-08-30T09:00:00:000-0600" <br>}</pre>

>[!NOTE]
Per questi nomi di campo viene fatta distinzione tra maiuscole e minuscole.

Per un elenco dei possibili riferimenti di campo, consulta  [Esplora API](../../wf-api/general/api-explorer.md)

#### Ricerca di oggetti nidificati

È possibile cercare oggetti nidificati. Per impostazione predefinita, gli oggetti nidificati vengono restituiti solo con il nome e l’ID. Ad esempio, per ottenere tutti i problemi insieme ai loro proprietari, utilizza la seguente richiesta:
<pre>/attask/api/v9.0/issue/search?fields=owner</pre>Se sono necessarie ulteriori informazioni, è possibile richiedere un campo nidificato utilizzando la sintassi dei due punti. Ad esempio, la seguente richiesta cerca tutti i problemi insieme al nome, all’ID, al titolo e al numero di telefono del proprietario
<pre>/attask/api/v9.0/issue/search?fields=owner:phoneNumber</pre>e restituisce quanto segue: 
<pre>{<br>    "name": "una questione importante",<br>    "ID": "4c78285f0000908ea8cfd66e084939f",<br>    "proprietario": {<br>        "title": "Specialista delle operazioni",<br>        "phoneNumber": "555-1234",<br>        "name": "Utente amministratore",<br>        "ID": "4c76ed7a000054c172b2c2d9f7f81c3" <br>    } <br>}</pre>

#### Recupero raccolte nidificate

È possibile recuperare raccolte nidificate di oggetti. Ad esempio, per ottenere un progetto con tutte le relative attività, utilizza la richiesta seguente:
<pre>/attask/api/v9.0/project/search?fields=attività</pre>La richiesta seguente ottiene le assegnazioni delle attività:
<pre>/attask/api/v9.0/task/search?fields=assegnazioni</pre>

#### Ricerca di più campi nidificati

Per impostazione predefinita, vengono restituiti solo il nome e l’ID di ogni attività, ma è possibile specificare campi nidificati aggiuntivi con sintassi a due punti. Per visualizzare tutti i campi disponibili per un oggetto o una raccolta correlati, è sufficiente aggiungere un segno di due punti e un asterisco al riferimento a oggetto/raccolta.
<pre>/attask/api/v9.0/task/search?fields=assegnazioni:*</pre>

#### Recupero dati personalizzati

Puoi recuperare i campi dati personalizzati utilizzando il prefisso &quot;DE:&quot;. Ad esempio, per richiedere un progetto con un parametro chiamato &quot;CustomText&quot;, utilizza la seguente richiesta:
<pre>/attask/api/v9.0/project/search?fields=DE:CustomText</pre>che restituiscono
<pre>{<br>    "name": "progetto dati personalizzato",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    "DE:CustomText": "compito b" <br>}</pre>È inoltre possibile recuperare tutti i dati personalizzati per un oggetto richiedendo il campo parameterValues. Ad esempio, 
<pre>/attask/api/v9.0/project/search?fields=parameterValues</pre>restituisce dati simili ai seguenti:
<pre>{<br>    "name": "progetto dati personalizzato",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    parameterValues: { <br>        "DE:CustomText": "compito b", <br>        "DE:CustomNumber": 1.4 <br>        "DE:CustomCheckBoxes": ["primo", "secondo", "terzo"] <br>    } <br>}</pre>

#### Utilizzo di query con nome

Alcuni tipi di oggetti dispongono di ricerche con nome che vengono comunemente eseguite e sono disponibili aggiungendo il nome della query alla fine dell’URI del tipo di oggetto. Ad esempio, la richiesta seguente recupera gli elementi di lavoro (attività e problemi) a cui l&#39;utente è attualmente assegnato:
<pre>/attask/api/v9.0/work/myWork</pre>Le query denominate supportano la richiesta del parametro fields per recuperare campi aggiuntivi. Alcune query con nome accettano anche filtri aggiuntivi. Per un elenco delle query con nome consentite e di un oggetto, vedere la scheda Azione relativa all'oggetto in [API Explorer](../../wf-api/general/api-explorer.md).

#### Utilizzo del filtro di conteggio

È possibile specificare il numero di risultati che si desidera restituire da una determinata ricerca. Questo consente al server di elaborare la richiesta più rapidamente e di risparmiare larghezza di banda. Ad esempio, la richiesta
<pre>GET /attask/api/v9.0/project/count?status=CUR</pre>restituisce il numero di risultati nel formato seguente:
<pre>{<br>    "count": 3 <br>}</pre>Questo risultato è un download molto più piccolo rispetto a se gli oggetti completi vengono inviati. La sintassi del filtro è identica al comando di ricerca.

### Richiesta di un rapporto

Puoi eseguire una richiesta di rapporto, in cui desideri solo l’aggregato di alcuni campi con uno o più raggruppamenti. Come mostrato nell’esempio seguente, la sintassi del report è la stessa dell’API SOAP:
<pre>GET /attask/api/v9.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>che restituisce il risultato seguente
<pre>{<br>    "Primo progetto": { <br>        "sum_hours": 15 <br>    }, <br>     "Secondo progetto": { <br>        "sum_hours": 30 <br>    } <br>}</pre>L'aggiunta del parametro $$ROLLUP=true include un totale a ogni livello di raggruppamento:
<pre>{<br>    "Primo progetto": { <br>        "sum_hours": 15 <br>    }, <br>    "Secondo progetto": { <br>        "sum_hours": 30 <br>    }, <br>    "$$ROLLUP": { <br>        "sum_hours": 45 <br>    } <br>}</pre>

### Ordinamento dei risultati della query nell’API

Puoi ordinare i risultati in base a qualsiasi campo se aggiungi quanto segue alla chiamata API:

&amp;entryDate_Sort=asc

Ad esempio, se si desidera ordinare per attività Data inizio pianificata, rimuovere entryDate e sostituirlo con ScheduledCompletionDate.

Questo funziona per la maggior parte dei campi in Workfront.

### Considerazione dei limiti delle query

Quando si esegue una query su un oggetto, è necessario prestare particolare attenzione alla relazione tra gli oggetti correlati e alle limitazioni di ricerca. Ad esempio, come illustrato nella tabella seguente, una query per progetti non può restituire più di 2.000 progetti. Questi 2.000 progetti sono considerati &quot;oggetti primari&quot;. Se si esegue una query per il campo Attività nei progetti, il campo Attività, che è un insieme, diventa un oggetto secondario dell&#39;oggetto principale Progetto. Una query per il campo Attività può includere migliaia di attività nei progetti. In totale, il numero complessivo di oggetti (progetti e attività) restituiti non può superare il massimo di 50.000.

Per garantire prestazioni ottimali, la tabella seguente mostra i limiti inseriti nelle richieste di ricerca. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Risultato query</th> 
   <th>Limitazione</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td width="200">Numero predefinito di risultati</td> 
   <td>100</td> 
   <td> Se nel filtro query non è specificato alcun limite (ovvero $$LIMIT), il risultato può contenere non più di 100 oggetti primari. <br>Vedi <a href="#using-paginated-responses" class="MCXref xref">Utilizzo delle risposte impaginate</a> istruzioni su come ignorare questa limitazione. </td> 
  </tr> 
  <tr> 
   <td>Numero massimo di risultati</td> 
   <td>2,000</td> 
   <td>Il filtro query (ovvero $$LIMIT) può restituire non più di 2000 risultati. Per ulteriori informazioni, consulta "Risposte impaginate".</td> 
  </tr> 
  <tr> 
   <td>Profondità massima del campo</td> 
   <td>4</td> 
   <td>Quando si identificano i campi che si desidera visualizzare, non è possibile allontanare più di quattro livelli dall’oggetto oggetto oggetto da interrogare.</td> 
  </tr> 
  <tr> 
   <td>Numero massimo di oggetti</td> 
   <td>50,000</td> 
   <td>Il set di risultati non può includere 50000 oggetti primari e secondari.</td> 
  </tr> 
  <tr> 
   <td>Numero massimo di campi</td> 
   <td nowrap>1,000,000</td> 
   <td>Quando il set di risultati è inferiore a 50000 oggetti, i risultati possono includere al massimo 1000.000 campi.</td> 
  </tr> 
  <tr> 
   <td>Numero massimo di creazione/aggiornamenti batch</td> 
   <td>100</td> 
   <td>Il limite massimo di creazione o aggiornamento batch è 100.</td> 
  </tr> 
 </tbody> 
</table>

### Utilizzo delle risposte impaginate {#using-paginated-responses}

Per ignorare la limitazione predefinita del numero di risultati della query e consentire 200 risultati, è possibile includere nella query il filtro $$LIMIT=200, come illustrato nell&#39;esempio seguente:
<pre>GET /attask/api/v9.0/project/search?$$LIMIT=200</pre>Al fine di garantire l'affidabilità e le prestazioni per gli altri tenant del sistema, il limite massimo di risultati consentiti per query è di 2000 oggetti. Se si tenta di specificare un limite più grande, si verifica un messaggio di errore IllegalArgumentException . 

Pertanto, ti consigliamo di utilizzare risposte impaginate per set di dati di grandi dimensioni. Per specificare il primo risultato da restituire, aggiungere il filtro $$FIRST. Ad esempio, la richiesta seguente restituisce i risultati 201-250 per una query:
<pre>GET /attask/api/v9.0/project/search?$$FIRST=201&amp;$$LIMIT=50</pre>

### Creazione di una regola di accesso

È possibile creare una regola di accesso per determinare chi può accedere a un oggetto. Di seguito sono riportati alcuni esempi di regole di accesso che è possibile impostare:

Per impostare un progetto in modo che venga condiviso solo con un utente con ID &quot;abc123&quot;, utilizza la seguente richiesta:
<pre>GET /attask/api/v9.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=put &amp;Updates={ accessRules: [ {accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'} ] }</pre>In alternativa, per condividere solo con una nuova persona e mantenere intatti i permessi esistenti:
<pre>GET /attask/api/v9.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>Per recuperare le regole di accesso esistenti:
<pre>GET /attask/api/v9.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## Comportamento di POST

POST inserisce un nuovo oggetto. La sintassi è identica a PUT, ma con alcune eccezioni. Poiché il nuovo oggetto non esiste ancora, non dispone di un ID. Per questo motivo, l’URI non include l’ID.

### Creazione di un oggetto

Esempio di richiesta per creare un nuovo progetto:
<pre>POST /attask/api/v9.0/project?name=Nuovo progetto</pre>La risposta include il progetto appena creato, il relativo nuovo ID e tutti gli altri campi specificati.

### Copia di un oggetto

Alcuni oggetti supportano la copia. Per questi tipi di oggetti, è possibile creare nuovi oggetti pubblicandoli con un parametro copySourceID . Ad esempio, la richiesta seguente copia il progetto specificato e gli dà un nuovo nome:

```
POST /attask/api/v9.0/project?copySourceID=4c7...&name=Copied Project
```

### Caricamento di documenti

Puoi caricare i documenti tramite il seguente URL API:
<pre>POST /attask/api/v9.0/upload</pre>L’API prevede che il tipo di contenuto sia multipart/form-data. Il nome del parametro per il file deve essere uploadedFile. Il server restituisce i seguenti dati JSON:
<pre>{<br>    "handle": "4c7c08fa000002ff924e298ee148df4"<br>}</pre>Quando crei un documento Workfront, puoi utilizzare l'handle e inviare il messaggio al seguente URL:
<pre>POST /attask/api/v9.0/document?Updates={<br>    nome: aFileName,<br>    maniglia: abc...123, (handle dal caricamento del file)<br>    docObjCode: PROJ, (o ATTIVITÀ, OPTASK, ecc.)<br>    objID: abc...123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br>}</pre>

## Comportamento di PUT

PUT viene utilizzato per aggiornare un oggetto esistente.

La risposta per un PUT è identica a un GET. In entrambi i casi, il server restituisce il nuovo stato dell&#39;oggetto dopo l&#39;aggiornamento. Tutte le regole utilizzate per modificare una risposta a una richiesta GET funzionano anche con PUT, ad esempio per specificare campi aggiuntivi da restituire, dati personalizzati e così via.

### Modifica degli oggetti

Gli aggiornamenti agli oggetti vengono sempre eseguiti tramite ID utilizzando l’URI univoco dell’oggetto. I campi da aggiornare sono specificati come parametri di richiesta. Ad esempio, per modificare il nome di un progetto, puoi inviare una richiesta simile alla seguente:
<pre>PUT /attask/api/v9.0/project/4c7..?name=Nome nuovo progetto <br>PUT /attask/api/v9.0/project?id=4c7...&amp;name=Nuovo nome del progetto</pre>Poiché l'aggiornamento richiede un ID, l'operazione avrà esito negativo (senza inserimento) se l'oggetto non esiste sul server.

### Specifica delle modifiche JSON

Come mostrato nell’esempio seguente, puoi utilizzare il parametro della richiesta di aggiornamenti per specificare i campi da aggiornare utilizzando la sintassi JSON:
<pre>PUT /attask/api/v9.0/project/4c7..?Updates= <br>{<br>     nome: "Nome nuovo progetto", <br>     stato: "CUR", <br>     ... <br>}</pre>

### Aggiornamenti nidificati

Alcuni oggetti dispongono di raccolte private che possono essere aggiornate. Nell&#39;esempio seguente viene illustrato come sovrascrivere le assegnazioni esistenti per una determinata attività:
<pre>PUT /attask/api/v9.0/task/4c7..?Updates= <br>{<br>    assegnazioni: [ <br>        { <br>            assignedToID: "2222...54d0, <br>            Percentuale assegnazione: 50,0 <br>        },{ <br>            roleID: "1111...54d0"<br>        } <br>    ] <br>}</pre>

>[!NOTE]
Mentre gli aggiornamenti apportati al livello superiore sono sparsi, gli aggiornamenti a una raccolta o a un oggetto nidificato sostituiscono completamente la raccolta esistente. Per modificare una singola assegnazione di un&#39;attività senza influire sugli oggetti, utilizzare PUT nell&#39;assegnazione anziché sull&#39;attività.

Nell’esempio seguente un progetto viene reso una coda dell’help desk pubblico. Le proprietà della coda esistenti vengono sostituite.
<pre>PUT /attask/api/v9.0/project/4c7..?Updates= <br>{ <br>    queueDef: { <br>        isPublic: 1 <br>    } <br>}</pre>

### Utilizzo del parametro della richiesta di azione

Alcuni oggetti supportano azioni aggiuntive che possono essere eseguite oltre a semplici modifiche. Puoi specificare queste azioni utilizzando il parametro della richiesta di azione. Ad esempio, la richiesta seguente ricalcola la timeline di un determinato progetto:
<pre>PUT /attask/api/v9.0/project/4c7..?action=calculateTimeline<br><br>o<br><br>PUT /attask/api/v9.0/project/4c7../calculateTimeline </pre>

### Spostamento di oggetti

Di seguito viene illustrata la sintassi per lo spostamento di un&#39;attività da un progetto all&#39;altro:
<pre>PUT /attask/api/v9.0/task/4c7../move?projectID=5d8..</pre>Ecco un esempio per ogni tipo di azione: (??)
<pre>PUT /attask/api/v9.0/project/1234/authorization<br><br>PUT /attask/api/v9.0/project/1234/calculateFinance<br><br>PUT /attask/api/v9.0/project/1234/calculateTimeline<br><br>PUT /attask/api/v9.0/project/1234/calculateDataExtension<br><br>PUT /attask/api/v9.0/project/1234/richiamoApprovazione<br><br>PUT /attask/api/v9.0/project/1234/rifiutoApprovazione<br><br>PUT /attask/api/v9.0/task/1234/move<br><br>PUT /attask/api/v9.0/workitem/1234/markViewed</pre>Solo l’azione Sposta richiede l’identificazione di attributi aggiuntivi per specificare il progetto in cui spostare l’elemento di lavoro.

Di seguito è riportato un esempio di ogni tipo di azione: 
<pre>PUT /attask/api/v9.0/project/1234?method=put&amp;Updates={accessRules:[{accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'}]}</pre>

### Condivisione di oggetti

L&#39;esempio seguente illustra la sintassi per la condivisione di un progetto con un team:
<pre>PUT /attask/api/v9.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>Durante la modifica di un oggetto, è possibile sostituire tutte le regole di accesso di un oggetto effettuando un PUT e inviando aggiornamenti simili all'esempio seguente:
<pre>PUT /attask/api/v9.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;Updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',coreAction:'VIEEGOX W'}]}</pre>L'esempio seguente illustra la sintassi per lo spostamento di un'attività da un progetto all'altro:
<pre>PUT /attask/api/v9.0/task/4c7../move?projectID=5d8..</pre>

## Comportamento di DELETE

DELETE rimuove un oggetto. In ogni caso, l&#39;URI può includere il parametro force=true per fare in modo che il server rimuova i dati specificati e le relative dipendenze. Nell’esempio seguente, un’attività viene eliminata eseguendo il metodo HTTP DELETE su un URI:
<pre>DELETE /attask/api/v9.0/task/4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v9.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v9.0/task/4c78821c0000d6fa8d5e52f07a1d54d0?force=true <br>DELETE /attask/api/v9.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0?force=true</pre>

## Aggiornamenti in blocco

Un’istruzione di aggiornamento collettivo aggiorna più oggetti contemporaneamente all’interno di una singola chiamata API. Una chiamata API per la creazione in massa viene generata in modo simile a una normale chiamata di aggiornamento, come illustrato negli esempi seguenti:
<pre>PUT /attask/api/v9.0/proj?Updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>che restituisce un risultato simile al seguente:
<pre>dati: [{<br>    ID: "53ff8d3d003b438b57a8a784df38f6b3",<br>    nome: "Test_Project_1",<br>    objCode: "PROJ",<br>    percentualeCompleta: 0,<br>    scheduledCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    scheduledStartDate: "2014-08-28T11:00:00:000-0400",<br>    priorità: 0,<br>    proiettatoCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    stato: "CUR"<br>},<br>{<br>    ID: "53ff8d49003b43a2562aa34eea3b6b10",<br>    nome: "Test_Project_2",<br>    objCode: "PROJ",<br>    percentualeCompleta: 0usi,<br>    scheduledCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    scheduledStartDate: "2014-08-28T11:00:00:000-0400",<br>    priorità: 0,<br>    proiettatoCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    stato: "CUR"<br>}]</pre>Puoi anche eseguire un aggiornamento collettivo simile al seguente:
<pre>PUT /attask/api/v9.0/proj?Umethod=PUT&amp;Updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Edit"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxx","name":" "Test_Project_2_Edit"}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>che restituisce un risultato simile al seguente:
<pre>dati: [ {<br>     ID: "53ff8e15003b461d4560f7f65a440078",<br>     nome: "Test_Project_1_Edit",<br>     objCode: "PROJ",<br>     percentualeCompleta: 0,<br>     scheduledCompletionDate: "2014-08-28T11:00:00:000-0400",<br>     scheduledStartDate: "2014-08-28T11:00:00:000-0400",<br>     priorità: 0,<br>     proiettatoCompletionDate: "2014-08-28T16:16:00:000-0400",<br>     stato: "CUR"<br>},<br>{<br>    ID: "53ff8e19003b46238a58d303608de502",<br>    nome: "Test_Project_2_Edit",<br>    objCode: "PROJ",<br>    percentualeCompleta: 0,<br>    scheduledCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    scheduledStartDate: "2014-08-28T11:00:00:000-0400",<br>    priorità: 0,<br>    proiettatoCompletionDate: "2014-08-28T16:16:00:000-0400",<br>    stato: "CUR"<br>}]</pre>Se desideri che tutte le operazioni vengano eseguite nella stessa transazione, aggiungi "atomic=true" alla chiamata API batch come parametro di richiesta. In questo modo, se una qualsiasi delle operazioni fallisce, tutte le operazioni sono rimandate indietro.

>[!NOTE]
Le operazioni batch atomiche possono restituire solo &quot;successo&quot;: true&quot; o un errore.
