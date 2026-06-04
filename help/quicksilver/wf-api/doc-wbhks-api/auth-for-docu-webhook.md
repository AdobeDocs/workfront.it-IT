---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Autenticazione per webhook documenti
description: Autenticazione per webhook documenti
author: Becky
feature: Workfront API
role: Developer
exl-id: 2303c202-27c7-4922-a613-e9824910504c
TQID: https://experienceleague.adobe.com/cRJbyPxBa-US0cV1cHsi43qvV59-AwhPgFjEhWsC1ME
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 439
ht-degree: 3%

---

# Autenticazione per webhook documenti

## Autenticazione

I webhook dei documenti di Adobe Workfront supportano due diverse forme di autenticazione: OAuth2 e ApiKey. In entrambi i casi, Workfront trasmette i token di autenticazione nell’intestazione quando effettua una chiamata API.

### OAuth2

OAuth2 consente a Workfront di effettuare chiamate API autorizzate a un provider di webhook per conto di un utente. Prima di eseguire questa operazione, l&#39;utente deve connettere l&#39;account del provider di documenti esterno a Workfront e concedere a Workfront

poter agire per loro conto. Questo processo di handshake viene eseguito una sola volta per ogni utente. Ecco come funziona:

1. L’utente inizia a collegare l’integrazione del webhook al proprio account. Attualmente, questo viene fatto facendo clic sul menu a discesa &quot;Aggiungi documento&quot; > &quot;Aggiungi servizio&quot; > Nome dell’integrazione personalizzata.
1. Workfront passa all’utente tramite l’URL di autenticazione, che può richiedere all’utente di accedere al provider di documenti esterno. Questa pagina è ospitata dal provider del webhook o dal sistema esterno di gestione dei documenti. Workfront aggiunge un parametro &quot;state&quot; all’URL di autenticazione. Questo valore deve essere restituito a Workfront aggiungendo lo stesso valore all’URI di ritorno Workfront nel passaggio seguente.
1. Dopo aver effettuato l’accesso al sistema esterno (o se l’utente ha già effettuato l’accesso), viene visualizzata una pagina di &quot;Autenticazione&quot; in cui viene spiegato che Workfront richiede l’accesso per eseguire una serie di azioni per conto dell’utente.
1. Se l&#39;utente fa clic sul pulsante &quot;Consenti&quot;, il browser reindirizzerà all&#39;URI di reindirizzamento di Workfront , aggiungendo &quot;code=`<code>`&quot; alla stringa di query. In base alla specifica OAuth2, questo token ha una durata breve. La stringa di query deve inoltre avere il seguente &quot;state=`<sent_by_workfront>`&quot;.
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

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of "username:password". See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
