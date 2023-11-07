---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: API dei webhook dei documenti
description: API dei webhook dei documenti
author: Becky
feature: Workfront API
role: Developer
exl-id: 7ac2c6c8-1cb8-49df-8d63-a6b47ad02a13
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '3646'
ht-degree: 3%

---


# API dei webhook dei documenti

Adobe Workfront Document Webhooks definisce un set di endpoint API attraverso i quali Workfront effettua chiamate API autorizzate a un provider di documenti esterno. Questo consente a chiunque di creare un plug-in middleware per qualsiasi provider di archiviazione dei documenti.

L’esperienza utente per le integrazioni basate su webhook sarà simile a quella delle integrazioni di documenti esistenti, come Google Drive, Box e Dropbox. Ad esempio, un utente di Workfront sarà in grado di eseguire le azioni seguenti:

* Spostarsi nella struttura di cartelle del provider di documenti esterno
* Cerca file
* Collegare i file in Workfront
* Carica file nel provider di documenti esterno
* Visualizza una miniatura per il documento

## Implementazione di riferimento

Per aiutarti a iniziare lo sviluppo di una nuova implementazione di webhook, Workfront fornisce un’implementazione di riferimento. Il codice per questo è disponibile all&#39;indirizzo [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Questa implementazione è basata su Java e consente a Workfront di collegare documenti su un file system di rete.

## Registrazione di un&#39;integrazione webhook

Gli amministratori di Workfront possono aggiungere un’integrazione di webhook personalizzata per la propria società da Configurazione > Documenti > Integrazioni personalizzate in Workfront. Dalla pagina Integrazione personalizzata all’interno di Configurazione, gli amministratori possono visualizzare un elenco delle integrazioni dei webhook dei documenti esistenti. Da questa pagina è possibile aggiungere, modificare, abilitare e disabilitare le integrazioni. Per aggiungere un’integrazione, fai clic sul pulsante &quot;Aggiungi integrazione&quot;.

### Campi disponibili

Quando aggiungi un’integrazione, l’amministratore immetterà i valori per i seguenti campi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome Campo</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nome</td> 
   <td>Il nome di questa integrazione.</td> 
  </tr> 
  <tr> 
   <td>URL API base</td> 
   <td> <p>Posizione dell’API di callback. Quando effettui chiamate al sistema esterno, Workfront si limita ad aggiungere il nome dell’endpoint a questo indirizzo. Ad esempio, se l’amministratore ha immesso l’URL API di base, "https://www.mycompany.com/api/v1", Workfront utilizza il seguente URL per ottenere i metadati di un documento: https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
  </tr> 
  <tr> 
   <td>Parametri di richiesta</td> 
   <td> <p>Valori opzionali da accodare alla stringa di interrogazione di ogni chiamata API. Ad esempio, tipo_di_accesso</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Tipo di autenticazione</td> 
   <td>OAuth2 o ApiKey</td> 
  </tr> 
  <tr> 
   <td>URL autenticazione</td> 
   <td> <p>(Solo OAuth2) L’URL completo utilizzato per l’autenticazione dell’utente. Workfront sposterà gli utenti a questo indirizzo come parte del processo di provisioning OAuth. Nota: Workfront aggiungerà un parametro "state" alla stringa di query. Il provider deve restituire questa proprietà a Workfront aggiungendola all'URI di reindirizzamento di Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>URL endpoint token</td> 
   <td> <p>(Solo OAuth2) L’URL API completo utilizzato per recuperare i token OAuth2. È ospitato dal provider del webhook o dal provider di documenti esterno</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>ID client</td> 
   <td>(Solo OAuth2) L'ID client OAuth2 per questa integrazione</td> 
  </tr> 
  <tr> 
   <td>Segreto client</td> 
   <td> <p>(Solo OAuth2) Il segreto client OAuth2 per questa integrazione</p> </td> 
  </tr> 
  <tr> 
   <td>URI reindirizzamento Workfront</td> 
   <td>  <p>(Solo OAuth2) Questo è un campo di sola lettura ed è generato da Workfront. Questo valore viene utilizzato per registrare questa integrazione con il provider di documenti esterno. Nota: come descritto in precedenza per l’URL di autenticazione, il provider deve aggiungere il parametro "state" e il relativo valore alla stringa di interrogazione durante l’esecuzione del reindirizzamento.</p></td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td>  <p>(Solo ApiKey) Utilizzato per effettuare chiamate API autorizzate al provider del webhook. Chiave API rilasciata dal provider del webhook.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Autenticazione

I webhook dei documenti di Workfront supportano due diverse forme di autenticazione: OAuth2 e ApiKey. In entrambi i casi, Workfront trasmette i token di autenticazione nell’intestazione quando effettua una chiamata API.

### OAuth2

OAuth2 consente a Workfront di effettuare chiamate API autorizzate a un provider di webhook per conto di un utente. Prima di eseguire questa operazione, l&#39;utente deve connettere l&#39;account del provider di documenti esterno a Workfront e concedere a Workfront

poter agire per loro conto. Questo processo di handshake viene eseguito una sola volta per ogni utente. Ecco come funziona:

1. L’utente inizia a collegare l’integrazione del webhook al proprio account. Attualmente, questo viene fatto facendo clic sul menu a discesa &quot;Aggiungi documento&quot; > &quot;Aggiungi servizio&quot; > Nome dell’integrazione personalizzata.
1. Workfront passa all’utente tramite l’URL di autenticazione, che può richiedere all’utente di accedere al provider di documenti esterno. Questa pagina è ospitata dal provider del webhook o dal sistema esterno di gestione dei documenti. Workfront aggiunge un parametro &quot;state&quot; all’URL di autenticazione. Questo valore deve essere restituito a Workfront aggiungendo lo stesso valore all’URI di ritorno Workfront nel passaggio seguente.
1. Dopo aver effettuato l’accesso al sistema esterno (o se l’utente ha già effettuato l’accesso), viene visualizzata una pagina di &quot;Autenticazione&quot; in cui viene spiegato che Workfront richiede l’accesso per eseguire una serie di azioni per conto dell’utente.
1. Se l’utente fa clic sul pulsante &quot;Consenti&quot;, il browser reindirizzerà all’URI di reindirizzamento di Workfront , aggiungendo &quot;code=`<code>`&quot; alla querystring. In base alla specifica OAuth2, questo token ha una durata breve. La stringa di query deve inoltre avere il seguente stato: &quot;state=`<sent_by_workfront>`&quot;.
1. Workfront elabora questa richiesta e effettua una chiamata API all’URL dell’endpoint del token con il codice di autorizzazione.
1. L’URL dell’endpoint token restituisce un token di aggiornamento e un token di accesso.
1. Workfront memorizza questi token ed esegue il provisioning completo dell’integrazione del webhook per questo utente.
1. Da questo momento in poi, Workfront sarà in grado di effettuare chiamate API autorizzate al provider del webhook. Quando effettui queste chiamate, Workfront invierà il token di accesso nell’intestazione della richiesta HTTP come mostrato di seguito:

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. Se il token di accesso è scaduto, Workfront effettuerà una chiamata all’URL dell’endpoint del token per recuperare un nuovo token di accesso e quindi tenterà di nuovo la chiamata API autorizzata con il nuovo token di accesso.

### ApiKey

Effettuare chiamate API autorizzate a un provider di webhook utilizzando un’ApiKey è molto più semplice di OAuth2. Quando effettui una chiamata API, Workfront passa semplicemente il nome utente ApiKey e Workfront nell’intestazione della richiesta HTTP:

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Il provider del webhook può utilizzare il nome utente per applicare autorizzazioni specifiche dell&#39;utente. Questa funzione è particolarmente utile quando entrambi i sistemi si connettono a LDAP utilizzando Single Sign On (SSO).

### Aggiunta di intestazioni di richiesta (facoltativo)

Oltre a utilizzare i token OAuth2 o un ApiKey per l’autenticazione, Workfront può inviare un set predefinito di intestazioni al provider del webhook per ogni chiamata API. Un amministratore di Workfront può effettuare questa configurazione durante la registrazione o la modifica di un&#39;integrazione di Windows, come descritto nella sezione precedente. Consulta Registrazione di un’integrazione webhook.

Ad esempio, può essere utilizzato per l’autenticazione di base. A questo scopo, l’amministratore di Workfront aggiungerà le seguenti informazioni sull’intestazione della richiesta nella finestra di dialogo Integrazione personalizzata:

   Autorizzazione Base QWxhZGRpbjpvcGVuIHNlc2FtZQ==

dove QWxhZGRpbjpvcGVuIHNlc2FtZQ== è una stringa con codifica base 64 di &quot;username:password&quot;. Consulta Autenticazione di base. Se aggiunto, Workfront lo trasmetterà nell’intestazione della richiesta HTTP, oltre ad altre intestazioni di richiesta:

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## Specifiche API

Di seguito è riportato un elenco di API che il provider del webhook deve implementare per il funzionamento dei webhook dei documenti.

### Recupero token OAuth2 (solo autenticazione OAuth2 necessaria)

Restituisce il token di aggiornamento e il token di accesso OAuth2 per un utente autenticato. Viene richiamato una volta quando l’utente fornisce un provider di documenti. Vengono effettuate chiamate successive per ottenere un token di accesso aggiornato.

HTTP Request POST /any/url

L’URL è configurabile e corrisponde al valore dell’URL dell’endpoint del token nella pagina di configurazione dell’integrazione personalizzata.

**Parametri di query**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome</th> 
   <th>Obbligatorio</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>grant_type</td> 
   <td>sì</td> 
   <td> <p>I valori includono "authorized_code" o "refresh_token". Il valore specificato indica quale dei due parametri verrà trasmesso a questa chiamata API: code o refresh_token.</p> </td> 
  </tr> 
  <tr> 
   <td>codice</td> 
   <td>dipende</td> 
   <td> <p>Il codice di autorizzazione inviato a Workfront subito dopo che l’utente ha fatto clic sul pulsante "Concedi". Questa opzione è necessaria solo quando il tipo di concessione è "authorized_code". Il codice di autorizzazione deve essere di breve durata e scadere generalmente in 10 minuti o meno.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>dipende</td> 
   <td> <p>Questa opzione è necessaria solo quando si effettuano chiamate successive per recuperare un nuovo access_token, dato che il precedente access_token è scaduto. Quando si invia questo valore, impostare il parametro grant_type su "refresh_token".</p> </td> 
  </tr> 
  <tr> 
   <td>client_id</td> 
   <td>sì</td> 
   <td>L’ID client configurato in Workfront per questa integrazione personalizzata.</td> 
  </tr> 
  <tr> 
   <td>client_secret</td> 
   <td>sì</td> 
   <td> Il segreto client configurato in Workfront per questa integrazione personalizzata.</td> 
  </tr> 
 </tbody> 
</table>

 

**Risposta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome</th> 
   <th>Tipo </th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>access_token </td> 
   <td>Stringa</td> 
   <td> <p>Token utilizzato per effettuare chiamate API autorizzate per conto dell’utente. Questa impostazione dovrebbe scadere per evitare chiamate API non autorizzate.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token </td> 
   <td>Stringa</td> 
   <td> <p>Token di lunga durata utilizzato per recuperare un nuovo access_token chiamando questo metodo API.</p> </td> 
  </tr> 
  <tr> 
   <td>expires_in </td> 
   <td>long</td> 
   <td>  <p>(facoltativo) Tempo (in secondi) prima della scadenza del token di accesso, in genere 3.600.</p></td> 
  </tr> 
 </tbody> 
</table>

 

**Esempio**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```


**Risposta**

```
{
"access_token":"ad8af5ad5ads759", 
"refresh_token":"9a0h5d87d808ads", 
"expires_id":"3600" 
}
```

### Ottieni metadati per file o cartella

Restituisce i metadati per il file o la cartella specificata.

**URL**

GET /metadata?id=[ID documento o cartella]

**Parametri di query**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome </th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>id</td> 
   <td>  <p>ID del file o della cartella, come indicato dal provider del webhook. È diverso dall’ID documento di Workfront. Per ottenere i metadati della directory principale, utilizza il valore "/".</p><p>Nota: la lunghezza massima per l’ID è di 255 caratteri.</p></td> 
  </tr> 
 </tbody> 
</table>

 

**Risposta**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome </th> 
   <th>Tipo </th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title </td> 
   <td>Stringa </td> 
   <td>Nome del documento o della cartella</td> 
  </tr> 
  <tr> 
   <td>tipo </td> 
   <td>Stringa </td> 
   <td>Specifica se l'elemento è un file o una cartella (file o cartella)</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>Stringa </td> 
   <td>ID del file o della cartella.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>Stringa </td> 
   <td> <p>Percorso URL utilizzato da un utente per visualizzare il documento in una finestra del browser. L’URL può essere ospitato dal provider di documenti o dal provider di archiviazione esterno nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>Stringa </td> 
   <td> <p>Percorso URL utilizzato da un utente per scaricare il documento in una finestra del browser. L’URL può essere ospitato dal provider di documenti o dal provider di archiviazione esterno nativo.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>Stringa </td> 
   <td>Tipo MIME del file. (opzionale)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>Stringa </td> 
   <td>Ultima modifica del file (timestamp RFC 3339 formattato)</td> 
  </tr> 
  <tr> 
   <td>dimensione</td> 
   <td>Lungo</td> 
   <td>  Dimensione del file in byte. (opzionale)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Booleano</td> 
   <td>  <p> Indica se il file o la cartella è di sola lettura per l'utente autenticato.(opzionale)</p><p> </p></td> 
  </tr> 
 </tbody> 
</table>

**Esempio:** `https://www.acme.com/api/metadata?id=12345`

**Risposta**

```
{
"title":"My Document", 
"kind":"file"
"id":"12345", 
"viewLink":"https://www.acme.com/viewDocument?id=12345", 
"downloadLink":"https://www.acme.com/downloadDocument?id=12345",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size": "32554694"
}
```

>[!NOTE]
>
>La gestione degli errori deve essere coerente in tutte le chiamate API. Per informazioni dettagliate, consulta la sezione &quot;Gestione degli errori&quot; di seguito.

### Ottenere un elenco di elementi in una cartella

Restituisce i metadati per i file e le cartelle di una determinata cartella.

**URL**

GET/file

**Parametri di query**

| Nome  | Descrizione |
|---|---|
| parentId  | ID cartella. Per ottenere i metadati della directory principale, utilizza il valore &quot;/&quot;. |

{style="table-layout:auto"}

L&#39;API Document Webhooks non supporta attualmente l&#39;impaginazione.

**Risposta**

JSON contenente un elenco di file e cartelle. I metadati per ogni elemento sono gli stessi restituiti dall’endpoint /metadata.

**Esempio:** `https://www.acme.com/api/files?parentId=123456`

**Risposta**

```
[
{
"title":"Folder A",
"kind":"folder",
"id":"2lj23lkj",
"viewLink":"https://www.acme.com/viewDocument?id=2lj23lkj",
"downloadLink":"https://www.acme.com/downloadDocument?id=2lj23lkj",
"mimeType":"",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"" 
},
{
"title":"My Document",
"kind":"file",
"id":"da8cj234"
"viewLink":"https://www.acme.com/viewDocument?id=da8cj234",
"downloadLink":"https://www.acme.com/downloadDocument?id=da8cj234",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"32554694"
},
]
```

### Esegui una ricerca

Restituisce i metadati per i file e le cartelle restituiti da una ricerca. Questa può essere implementata come ricerca full-text o come normale query di database. Workfront chiama l’endpoint /search quando l’utente esegue una ricerca dal browser di file esterno.

**URL**

GET/ricerca

**Parametri di query**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome </th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>query</td> 
   <td>Termine o frase di ricerca.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(facoltativo) ID della cartella da cui è stata eseguita la ricerca. Nota: questo è un segnaposto per una funzione futura in Workfront. Attualmente, Workfront non passa questo parametro. </p> </td> 
  </tr> 
  </tbody> 
</table>

L&#39;API Document Webhooks non supporta attualmente l&#39;impaginazione.

 

**Risposta**

JSON contenente un elenco di metadati per file e cartelle che corrispondono alla query. Che cosa costituisce una &quot;corrispondenza&quot; è determinato dal provider del webhook. Idealmente, dovrebbe eseguire una ricerca full-text. È anche possibile eseguire una ricerca basata sul nome del file.

**Esempio:** `https://www.acme.com/api/search?query=test-query`

**Risposta**

```
[
{ File/Folder Metadata },
{ File/Folder Metadata }
]
```

### Ottenere il contenuto di un documento

Restituisce i byte non elaborati di un documento

**URL**

GET/download

**Parametri di query**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome </th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td> ID del documento.</td> 
  </tr> 
 </tbody> 
</table>

 

**Risposta**

Byte non elaborati del documento.

**Esempio:** `https://www.acme.com/api/download?id=123456`

### Ottenere una miniatura per un documento

Restituisce i byte delle miniature non elaborati per un documento.

**URL**

GET/miniatura

**Parametri di query**

| Nome  | Descrizione |
|---|---|
| id  | ID del documento. |
| dimensione  |  Larghezza della miniatura |

{style="table-layout:auto"}

 

**Risposta**

Byte delle miniature non elaborati.

**Esempio:** `https://www.acme.com/api/thumbnail?id=123456`

### Caricare un file - Parte 1 di 2

Il caricamento di un file in un provider di archiviazione documenti è un processo in due fasi che richiede due endpoint API separati. Workfront avvia il processo di caricamento chiamando /uploadInit. Questo endpoint restituisce un ID documento che viene quindi passato a /upload durante il caricamento dei byte del documento. A seconda del sistema di archiviazione dei documenti sottostante, potrebbe essere necessario creare un documento di lunghezza zero e quindi aggiornare il contenuto del documento in un secondo momento.

Aggiunto alla versione 1.1 di questa specifica, l&#39;ID documento e l&#39;ID versione documento possono essere utilizzati per recuperare informazioni aggiuntive da Workfront. Ad esempio, se il sistema di gestione dei documenti richiede informazioni aggiuntive sul documento, il codice di implementazione del webhook potrebbe utilizzare l’ID del documento per recuperare tali informazioni utilizzando l’API RESTful di Workfront. È buona norma che queste informazioni provengano dai campi dati personalizzati del documento che contengono l&#39;attività, il problema o il progetto.

**URL**

POST /uploadInit

**Parametri di query**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome </th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId </td> 
   <td>ID della cartella principale, come indicato dal provider del webhook.</td> 
  </tr> 
  <tr> 
   <td>nome file </td> 
   <td>Nome del documento</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>ID documento Workfront (aggiunto nella versione 1.1)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>ID versione documento Workfront (aggiunto nella versione 1.1)</td> 
  </tr> 
 </tbody> 
</table>

 

**Risposta**

I metadati del file, come definito dall’endpoint /metadata.

**Esempio:** `https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**Risposta**

`[file_metadata]` include il nuovo ID documento utilizzato dal provider di documenti.

### Caricare un file - Parte 2 di 2

Carica i byte di un documento nel provider del webhook.

**URL**

PUT /upload

**Parametri di query**

| Nome  | Descrizione |
|---|---|
| id  |  ID del documento appena creato. |


 

**Corpo della richiesta**

Byte di contenuto non elaborato per il documento.

**Risposta**

```
{
"result": "success"
}
```

oppure

```
{
"result": "fail"
}
```

**Esempio:** `https://www.acme.com/api/upload?id=1234` *[byte dei documenti inclusi nel flusso di aggiornamento]*

**Risposta**

```
{
"result":"success"
}
```

### Ottieni informazioni sul servizio 

(Data di rilascio: da definire) Restituisce informazioni sul servizio, ad esempio funzioni e funzionalità. Workfront utilizzerà queste informazioni per personalizzare l’interfaccia utente in Workfront. Ad esempio, se l’implementazione del webhook contiene alcune azioni personalizzate, il JSON deve elencare tali operazioni nel JSON. Gli utenti potranno quindi richiamare queste azioni da Workfront.

**URL**

GET /serviceInfo

Parametri di query

Nessuno. Inoltre, le chiamate a questo endpoint non devono richiedere l’autenticazione.

**Risposta**

JSON contenente informazioni su questo servizio

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nome</th> 
   <th>Tipo </th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion </td> 
   <td>Stringa </td> 
   <td>Versione del webhook implementata da questo servizio. Il numero di versione riportato nella parte superiore della specifica.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>Stringa </td> 
   <td>Numero di versione interno per questo servizio. Questo numero è determinato dal provider di servizi webhook ed è utilizzato solo a scopo informativo.<br><br></td> 
  </tr> 
  <tr> 
   <td>editore </td> 
   <td>Stringa </td> 
   <td>Il nome della società che fornisce l’implementazione del webhook.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Stringa </td> 
   <td>Elenco contenente gli endpoint API implementati da questo servizio. Questa può essere utilizzata per garantire che l’interfaccia utente di Workfront rifletta le funzionalità offerte dal provider del webhook. Ogni elemento nell’elenco deve includere il nome del punto finale (ad esempio "search").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Stringa</td> 
   <td>  <p>Elenco contenente le operazioni personalizzate implementate da questo webhook. Ogni voce di elenco include un nome e un nome visualizzato. Il nome visualizzato verrà visualizzato nel menu a discesa "Azioni documento" in Workfront. Facendo clic sull’elemento nel menu a discesa, l’azione viene richiamata nel webhook chiamando l’endpoint /customAction.</p></td> 
  </tr> 
 </tbody> 
</table>

**Esempio:** https://www.acme.com/api/serviceInfo

**Restituisce**

```
{
"webhook version": "1.2", "version": "1.0", "publisher": "Acme, LLC", "availableEndpoints": ["files", "metadata", "search", "download"

"thumbnail", "uploadInit", "upload" ], "customActions" [
{
"name": "archive", "displayName": "Archive" }, {

"name": "doSomethingElse", "displayName": "Do Something" }, ] }
```

### Creare una cartella

(Aggiunto nella versione 1.2) Crea una cartella in una determinata directory.
URL

POST /createFolder

**Parametri di query**

| Nome  | Descrizione |
|---|---|
| parentId  | ID cartella in cui creare la cartella |
| name  | Nome della nuova cartella |

{style="table-layout:auto"}

 

**Risposta**

I metadati per la cartella appena creata, come definito dall’endpoint /metadata.

**Esempio:** `POST https://www.acme.com/api/createFolder`

```
-------------------------------

parentId=1234

name=New Folder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

restituisce

```
{"title":"New Folder", 
 "kind":"folder""id":"5678",
 "viewLink":"",
 "downloadLink":"",
 "mimeType":"",
 "dateModified":"2014­06­05T17:39:45.251Z" 
 "size": "" 
 }
```

### Eliminare un documento o una cartella

(Data di rilascio: da definire) Elimina un documento o una cartella con l’ID specificato nel sistema esterno. L’eliminazione di una cartella ne comporta anche l’eliminazione del contenuto.

URL

PUT /delete

**Parametri di query**

| Nome  | Descrizione |
|---|---|
| documentId  | ID documento da eliminare |
| folderId  |  ID cartella da eliminare |

{style="table-layout:auto"}

Response Stringa JSON che indica l’esito positivo o negativo, come specificato nella sezione Gestione degli errori di seguito.

**Esempio:** PUT https://www.acme.com/api/delete id=1234

restituisce

```
{
"status": "success" 
}
```

restituisce

```
{
"status": "failure", "error": "File not found"
}
```


### Rinominare un documento o una cartella

(Data di rilascio: da definire) Rinomina un documento o una cartella con l’ID specificato nel sistema esterno.

URL

PUT /rename

**Parametri di query**

| Nome  | Descrizione |
|---|---|
| id | ID documento o cartella da rinominare |
| name  | Nuovo nome del documento o della cartella |

{style="table-layout:auto"}

 

risposta

Stringa JSON che indica l’esito positivo o negativo, come specificato nella sezione Gestione degli errori di seguito.

**Esempio:**

`PUT https://www.acme.com/api/rename`

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

```
{
"status": "success" 
}returns
{
"status": "failure", error: "Folder cannot be renamed because a folder with that name already exists." 
}
```

### Eseguire un&#39;azione personalizzata

(Data di rilascio: da definire) Questo endpoint consente a un utente di Workfront (o forse a un evento di flusso di lavoro automatizzato) di eseguire un’azione nel sistema esterno. L’endpoint /customAction accetta un parametro &quot;name&quot; che consente al provider del webhook di implementare più operazioni personalizzate.

Il provider webhook registra le azioni personalizzate con Workfront includendo le azioni nella risposta /serviceInfo in customActions. Workfront carica questo elenco durante la configurazione o l’aggiornamento del provider del webhook in Configurazione > Documenti > Integrazioni personalizzate.\
![](assets/mceclip0-350x262.png)

Gli utenti possono attivare l’azione personalizzata selezionando la sezione in &quot;Azioni documento&quot;\
![](assets/mceclip1-350x95.png)

**URL**

GET /customAction

**Parametri di query**

<table style="table-layout:auto">
 <col>
 <col>
 <thead>
  <tr>
   <th>Nome </th>
   <th>Descrizione</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><p>name</p></td>
   <td><p>Identificatore che specifica il tipo di azione da eseguire. Questo valore corrisponde a uno dei valori customAction elencati restituiti dall'endpoint /serviceInfo.</p></td>
  </tr>
  <tr>
   <td>documentId </td>
   <td>ID del documento Workfront per il quale viene eseguita l'azione.</td>
  </tr>
  <tr>
   <td>documentVersionId </td>
   <td> ID versione del documento Workfront per cui viene eseguita l'azione.</td>
  </tr>
 </tbody>
</table>

 

**Risposta**

Stringa JSON che indica l’esito positivo o negativo, come specificato nella sezione Gestione degli errori di seguito. In caso di errore (ossia stato = &quot;errore&quot;), Workfront visualizzerà il messaggio di errore fornito all’utente.

**Esempio:** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30 ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

risposta

```
{
"status": "success" 
}
```


## Gestione degli errori

Possono verificarsi problemi durante l’elaborazione delle richieste API. Questo deve essere gestito in modo coerente tra tutti gli endpoint API. Quando si verifica un errore, il provider del webhook esegue le operazioni seguenti:

* Includi un codice di errore nell’intestazione della risposta. I codici di errore includono:

   * 403 - Non consentito. Indica che i token di richiesta sono mancanti o non validi oppure che le credenziali associate ai token non hanno accesso alla risorsa specificata. Per i provider di webhook basati su OAuth, Workfront tenterà di recuperare i nuovi token di accesso.
   * 404 - Non trovato. Indica che il file o la cartella specificata non esiste.
   * 500 - Errore interno del server. Qualsiasi altro tipo di errore.

* Descrivi l’errore nel corpo della risposta utilizzando il seguente formato:


```
{
"status": "error"
"error": "Sample error message" 
}
```


## Test

Per verificare che l’implementazione del webhook del documento funzioni correttamente, esegui i seguenti test. Si tratta di test manuali che passano attraverso l’interfaccia web di Workfront e colpiscono indirettamente gli endpoint per l’implementazione del webhook.

### Prerequisiti

Per eseguire questi test è necessario disporre dei seguenti elementi:

* Un account Workfront con Advanced Document Management (ADM) abilitato
* Un utente Workfront per questo account con diritti di amministratore di sistema
* Un&#39;istanza del webhook del documento, i cui endpoint HTTP sono accessibili a Workfront

Questi test presuppongono inoltre che sia già stata registrata l’istanza di Document Webhook in Workfront in Configurazione > Documenti > Integrazioni personalizzate.

### Prova 1: eseguire il provisioning del servizio Document Webhook per un utente

Verifica l’URL di autenticazione e l’URL dell’endpoint del token per i provider Webhook basati su OAuth.

1. In Workfront, passare alla pagina principale Documenti facendo clic sul collegamento Documenti nella barra di navigazione superiore.
1. Fai clic sul menu a discesa Aggiungi documenti e seleziona il servizio Document Webhook in Aggiungi servizio.
1. (Solo per i servizi OAuth) Dopo aver completato il passaggio precedente, visualizzerai il caricamento della pagina di autenticazione OAuth2 del servizio in una finestra a comparsa. (Nota: potrebbe essere richiesto di accedere prima al servizio.) Dalla pagina di autenticazione, concedi a Workfront l’accesso all’account dell’utente facendo clic sul pulsante Considera attendibili o Consenti.
1. Verifica che il servizio sia stato aggiunto al menu a discesa Aggiungi documenti. Se inizialmente non è visibile, prova ad aggiornare il browser.

### Test 2: Collegare un documento in Workfront Test dei seguenti endpoint: /files, /metadata

1. In Workfront, passare alla pagina principale Documenti facendo clic sul collegamento Documenti nella barra di navigazione superiore.
1. Selezionare il servizio Web Document in Aggiungi documenti.
1. Dalla finestra modale, passa alla struttura delle cartelle.
1. Verifica la tua capacità di navigare correttamente nella struttura delle cartelle.
1. Selezionare un documento e collegarlo a Workfront

### Prova 3: passare a un documento nel sistema di gestione dei contenuti

Verifica i seguenti endpoint: /metadata (in particolare viewLink)

1. Collegare un documento a Workfront
1. Selezionare il documento e fare clic sul collegamento Apri.
1. Verificate che il documento venga aperto in una nuova scheda.

### Prova 4: passare a un documento nel sistema di gestione dei contenuti (con accesso)

Verifica i seguenti endpoint: /metadata (in particolare viewLink)

1. Assicurarsi di essere disconnessi dal sistema di gestione dei contenuti.
1. Collegare un documento a Workfront.
1. Selezionare il documento e fare clic sul collegamento Apri.
1. Verificare che la schermata di accesso del sistema di gestione dei contenuti venga caricata in una nuova scheda.
1. Accedi e verifica di essere reindirizzato al documento

### Prova 5: scarica il documento dal sistema di gestione dei contenuti

Verifica i seguenti endpoint: /metadata (in particolare downloadLink)

1. Collegare un documento a Workfront.
1. Selezionare il documento e fare clic sul collegamento Scarica.
1. Verifica l’inizio del download.

### Prova 6: cercare il contenuto

Verifica i seguenti endpoint: /search

1. In Workfront, passare alla pagina principale Documenti facendo clic sul collegamento Documenti nella barra di navigazione superiore.
1. Selezionare il servizio Web Document in Aggiungi documenti.
1. Dal modale, esegui una ricerca.
1. Verifica che i risultati della ricerca siano corretti.

### Prova 7: inviare il documento da Workfront al sistema di gestione dei contenuti

Verifica i seguenti endpoint: /files, /uploadInit, /upload

1. In Workfront, passare alla pagina principale Documenti facendo clic sul collegamento Documenti nella barra di navigazione superiore.
1. Carica un documento in Workfront dal computer
1. Vai alla pagina dei dettagli del documento
1. Dal menu a discesa Azioni documento, selezionare il servizio Web Document in Invia a...
1. Vai alla cartella di destinazione desiderata e fai clic sul pulsante Salva.
1. Verificare che il documento sia caricato nella posizione corretta nel sistema di gestione dei contenuti.

### Test 8: visualizzare le miniature in Workfront

Verifica i seguenti endpoint: /thumbnail

1. Collegare un documento a Workfront.
1. Selezionare il documento nell&#39;elenco.
1. Verifica che la miniatura venga visualizzata nel pannello di destra.

### Prova 9: recupero dei byte di contenuto

Verifica i seguenti endpoint: /download

1. Collegare un documento a Workfront.
1. Passare alla pagina dei dettagli del documento.
1. Inviare il documento a Workfront selezionando Azioni documento > Invia a... > Workfront. Verrà creata una nuova versione del documento in Workfront.
1. Scaricare il documento da Workfront facendo clic sul collegamento Scarica.

### Prova 10: aggiorna token di accesso (solo provider del webhook OAuth2)

Verifica i seguenti endpoint: URL endpoint token

1. Eseguire il provisioning di un servizio Web Document per un utente
1. Annulla la validità del token di accesso dell’utente 1 )in attesa del timeout oppure 2) annullandolo manualmente nel sistema esterno.
1. Aggiorna il token di accesso in Workfront. A tale scopo, ad esempio, è possibile collegare un documento in Workfront. Se sei riuscito a passare a un documento e a collegarlo, saprai che il token di accesso è stato aggiornato correttamente.

>[!NOTE]
>
>Al momento, l&#39;opzione Invia a non è disponibile per i documenti collegati. Questo verrà aggiunto da Workfront. Puoi testare l’endpoint /download premendo manualmente l’endpoint utilizzando un client REST, ad esempio Postman. In alternativa, è possibile testare l’endpoint /download generando una bozza digitale. Per attivare la verifica digitale, contattare Workfront.

## Versioni

* Versione 1.0 (data di rilascio: maggio 2015)

   * Specifiche iniziali

* Versione 1.1 (data di rilascio: giugno 2015)

   * Aggiornato /uploadInit - Aggiunti documentId e documentVersionId

* Versione 1.2 (data di rilascio: ottobre 2015)

   * Aggiunto /createFolder

