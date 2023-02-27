---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Autenticazione per i webhook dei documenti
description: Autenticazione per i webhook dei documenti
author: Becky
feature: Workfront API
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Autenticazione per i webhook dei documenti

## Autenticazione

I webhook di documenti Adobe Workfront supportano due diverse forme di autenticazione: OAuth2 e ApiKey. In entrambi i casi, Workfront trasmette i token di autenticazione nell’intestazione quando effettua una chiamata API.

### OAuth2

OAuth2 consente a Workfront di effettuare chiamate API autorizzate a un provider di webhook per conto di un utente. Prima di eseguire questa operazione, l’utente deve collegare il proprio account del provider di documenti esterno a Workfront e concedere a Workfront

accesso ad agire per loro conto. Questo processo di handshake viene eseguito una sola volta per ogni utente. Ecco come funziona:

1. L&#39;utente inizia a collegare l&#39;integrazione webhook al proprio account. Al momento, questo viene fatto facendo clic sul menu a discesa &quot;Aggiungi documento&quot; > &quot;Aggiungi servizio&quot; > Nome integrazione personalizzata.
1. Workfront sposta l’utente nell’URL di autenticazione, che potrebbe richiedere all’utente di accedere al provider di documenti esterno. Questa pagina è ospitata dal provider webhook o dal sistema esterno di gestione dei documenti. Workfront aggiunge un parametro &quot;state&quot; all&#39;URL di autenticazione. Questo valore deve essere restituito a Workfront aggiungendo lo stesso valore all’URI di ritorno Workfront nel passaggio seguente.
1. Dopo aver effettuato l’accesso al sistema esterno (o se l’utente ha già effettuato l’accesso), viene portato a una pagina &quot;Autenticazione&quot;, che spiega che Workfront richiede l’accesso per eseguire una serie di azioni per conto dell’utente.
1. Se l&#39;utente fa clic sul pulsante &quot;Consenti&quot;, il browser reindirizzerà all&#39; URI di reindirizzamento di Workfront , aggiungendo &quot;code=`<code>`&quot; nella stringa query. Secondo la specifica OAuth2, questo token è di breve durata. La stringa di query deve avere anche quanto segue, &quot;state=`<sent_by_workfront>`&quot;.
1. Workfront elabora questa richiesta ed effettua una chiamata API all’URL dell’endpoint token con il codice di autorizzazione.
1. L’URL dell’endpoint del token restituisce un token di aggiornamento e un token di accesso.
1. Workfront memorizza questi token e fornisce l&#39;integrazione del webhook per questo utente.
1. Da questo momento in poi, Workfront sarà in grado di effettuare chiamate API autorizzate al provider webhook. Quando effettui queste chiamate, Workfront invierà il token di accesso nell’intestazione della richiesta HTTP come mostrato di seguito:

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. Se il token di accesso è scaduto, Workfront effettuerà una chiamata all’URL dell’endpoint del token per recuperare un nuovo token di accesso, quindi tenterà di nuovo la chiamata API autorizzata con il nuovo token di accesso.

### ApiKey

Effettuare chiamate API autorizzate a un provider di webhook utilizzando un ApiKey è molto più semplice di OAuth2. Quando effettui una chiamata API, Workfront passerà semplicemente l’ApiKey e il nome utente Workfront nell’intestazione della richiesta HTTP: 

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Il provider Webhook può utilizzare il nome utente per applicare autorizzazioni specifiche per l&#39;utente. Questo funziona meglio quando entrambi i sistemi si connettono a LDAP utilizzando Single Sign On (SSO).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of “username:password”. See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
