---
content-type: api
navigation-topic: api-navigation-topic
title: Utilizzo del flusso PKCE per le applicazioni OAuth 2
description: Utilizzo del flusso PKCE per le applicazioni OAuth 2
author: Becky
feature: Workfront API
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: 5480d6b5e97c4c2e21080bb92ffe255f60ed6f60
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso PKCE

PKCE è un flusso di autorizzazione sicuro che funziona bene con le applicazioni di aggiornamento dinamico come le app mobili, ma è prezioso per tutti i client OAuth2. Invece di un segreto client statico, PKCE utilizza una stringa generata dinamicamente, eliminando il rischio di perdita di un segreto client.

## Panoramica di PKCE

Un flusso PKCE prevede i seguenti passaggi. I passaggi descritti in questa sezione sono riportati a titolo puramente informativo. Per eseguire queste procedure, vedere altre sezioni in questo articolo.

1. Il client crea `code_challenge` trasformando il `code_verifier` utilizzo `S256` crittografia.

1. Il client indirizza il browser alla pagina di accesso OAuth2, insieme al `code_challenge`. È necessario registrare l&#39;app (Client) in modo che OAuth2 possa accettare la richiesta di autorizzazione. Dopo la registrazione, l’app può reindirizzare il browser a OAuth2.

1. Il server di autorizzazione OAuth2 reindirizza la richiesta di autenticazione all&#39;utente.

1. L’utente si autentica utilizzando una delle opzioni di accesso configurate e potrebbe visualizzare una pagina di consenso in cui sono elencate le autorizzazioni che OAuth2 concederà all’applicazione.

1. OAuth2 reindirizza all&#39;applicazione con un `authorization code`.

1. L&#39;applicazione invia questo codice, insieme a `code_verifier`, a OAuth2.

1. Il server di autorizzazione OAuth2 trasforma il `code_verifier` utilizzando `code_challenge_method` dalla richiesta di autorizzazione iniziale e verifica il risultato rispetto al `code_challenge`. Se il valore di entrambe le stringhe corrisponde, il server ha verificato che le richieste provengono dallo stesso client e rilascerà un `access token`.

1. OAuth2 restituisce `access token`, e facoltativamente un `refresh token`.

1. L’applicazione può ora utilizzare questi token per chiamare il server delle risorse, ad esempio un’API per conto dell’utente.

1. Il server delle risorse convalida il token prima di rispondere alla richiesta.


## Configurare l’applicazione

Prima di implementare l’autorizzazione, è necessario registrare l’app in OAuth2 creando un’integrazione di app da Workfront.

Per istruzioni sulla creazione dell&#39;applicazione OAuth2, vedi [Creare un’applicazione web OAuth2 a pagina singola utilizzando PKCE](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) in [Creazione di applicazioni OAuth2 per le integrazioni Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)


## Creare la bozza della chiave per lo scambio di codice

Simile al flusso del codice di autorizzazione standard, l’app inizia reindirizzando il browser dell’utente a quello del server di autorizzazione. `/authorize` endpoint. Tuttavia, in questo caso è anche necessario trasmettere una richiesta di codice.

Il primo passaggio consiste nel generare un codice di validazione e una richiesta di verifica.

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">Verificatore del codice</td>
        <td>
          <p>Stringa casuale URL-safe con una lunghezza minima di 43 caratteri</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Criterio codice</td>
        <td>
          <p>Hash SHA-256 con codifica URL Base64 del codice di validazione</p>
        </td>
      </tr>
    </tbody>
</table>


Devi aggiungere il codice nell’app client per creare il codice di validazione e il codice di autenticazione.

Il codice del generatore PKCE crea un output simile al seguente:

>[!INFO]
>
>**Esempio:**
>
>```
>{
>  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>}
>```

L&#39;app salva `code_verifier` per dopo, e invia `code_challenge` insieme alla richiesta di autorizzazione al server di autorizzazione `/authorize` URL.

## Richiedi un codice di autorizzazione

Se utilizzi il server di autorizzazione personalizzato predefinito, l’URL della richiesta sarà simile al seguente:

>[!INFO]
>
>**Esempio:**
>
>
>```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

Prendi nota dei parametri che vengono passati:

* `client_id` corrisponde all&#39;ID client dell&#39;applicazione OAuth2 creata in durante la configurazione dell&#39;applicazione.

  Per istruzioni, consulta Creare un’applicazione web a pagina singola OAuth2 utilizzando PKCE in Creare applicazioni OAuth2 per le integrazioni Workfront.

* `response_type` è `code`, perché l&#39;applicazione utilizza il tipo di concessione Codice di autorizzazione.

* `redirect_uri` è la posizione di callback a cui viene indirizzato l’agente utente insieme al `code`. Deve corrispondere a uno degli URL di reindirizzamento specificati al momento della creazione dell’applicazione OAuth2.

* `code_challenge_method` è il metodo hash utilizzato per generare la sfida, che è sempre `S256` per applicazioni Workfront Oauth2 che utilizzano PKCE.

* `code_challenge` è la richiesta di verifica del codice utilizzata per PKCE.


## Scambia il codice con i token

Per scambiare il codice di autorizzazione con un token di accesso, trasmettilo al server autorizzazioni `/token` endpoint insieme al `code_verifier`.

>[!INFO]
>
>**Esempio:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> A differenza del normale flusso del codice di autorizzazione, questa chiamata non richiede l’intestazione Autorizzazione con l’ID client e il segreto. Per questo motivo questa versione del flusso del codice di autorizzazione è appropriata per le app native, come le applicazioni mobili o le applicazioni a pagina singola che non dispongono di un back-end.

Prendi nota dei parametri che vengono passati:

* `grant_type` è `authorization_code`, perché l’app utilizza il tipo di concessione Codice di autorizzazione.

* `redirect_uri` deve corrispondere all’URI utilizzato per ottenere il codice di autorizzazione.

* `code` è il codice di autorizzazione ricevuto dall&#39;endpoint /authorize.

* `code_verifier` è il codice di validazione PKCE generato dall’app in [Creare la bozza della chiave per lo scambio di codice](#Create).

* `client_id` identifica il client e deve corrispondere al valore preregistrato in OAuth2.


Se il codice è ancora valido e il codice di validazione corrisponde a, l’applicazione riceve un token di accesso.

>[!INFO]
>
>**Esempio:**
>
>```
>{
>    "access\_token": "eyJhd\[...\]Yozv",
>    "expires\_in": 3600,
>    "token\_type": "Bearer"
>}
>```

## Convalidare il token di accesso

Quando l’applicazione trasmette una richiesta con un token di accesso, il server delle risorse deve convalidarla.

Puoi convalidare il token di accesso con una chiamata API simile alla seguente:

>[!INFO]
>
>**Esempio:**
>
>```
>/attask/api/<api version>/proj/search \\
>  --header 'sessionID: <access\_token>' \\
>```

## Richiedi un token di aggiornamento

Per richiedere un token di aggiornamento, puoi effettuare una chiamata POST all’API, simile alla seguente:

>[!INFO]
>
>**Esempio:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
