---
content-type: api
navigation-topic: api-navigation-topic
title: Flusso di codice di autorizzazione per le applicazioni OAuth 2 personalizzate
description: Flusso di codice di autorizzazione per le applicazioni OAuth 2 personalizzate
author: John
feature: Workfront API
exl-id: a1ab60c4-4255-4d80-87f1-f36d325254c2
source-git-commit: e67f397ec82858bc489313db963259ce05175428
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---


# Configura e utilizza le applicazioni personalizzate OAuth 2 della tua organizzazione utilizzando il flusso di codice di autorizzazione

Al fine di integrarsi con Workfront e consentire alla tua app client di comunicare con Workfront per conto dell’utente, devi:

* Creare un’applicazione OAuth2
* Configurare l’applicazione di terze parti
* Collegamento alla pagina Autorizza per i tuoi utenti
* Imposta flusso codice autorizzazione: Gli utenti accedono all’istanza Workfront e acconsentono a consentire all’applicazione client di connettersi a Workfront per loro conto. Di conseguenza, ottieni un codice di autorizzazione che scambierai con token di accesso e aggiornamento.
* Imposta Aggiorna flusso token: In questo flusso si utilizza il token di aggiornamento per ottenere un nuovo token di accesso quando il vecchio è scaduto.

## Creare un’applicazione OAuth2

Per istruzioni sulla creazione dell’applicazione OAuth2, consulta [Creare un’applicazione OAuth2 utilizzando le credenziali utente (flusso di codice di autorizzazione)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create3) in [Creare applicazioni OAuth2 per le integrazioni Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Collegamento alla pagina Autorizza per i tuoi utenti

Gli utenti devono effettuare l’accesso per autorizzare questa integrazione nel proprio account. La pagina che consente loro di autorizzare ha un formato specifico, descritto qui. Usa queste informazioni per determinare l&#39;indirizzo della pagina di autorizzazione per l&#39;app e fornire agli utenti questo indirizzo o un collegamento ad essa.

* L’URL completo del dominio dell’organizzazione. Esempio:

   ```
   https://myorganization.my.workfront.com
   ```


* `client_id`: Questo è l’ID client generato quando hai creato l’app OAuth2 in Workfront.

* `redirect_uri`: Si tratta dell’URL di reindirizzamento immesso al momento della creazione dell’app. Gli utenti verranno indirizzati a questa pagina dopo aver autorizzato l’app per il loro account.

* `response_type`: Deve avere il valore `code`.

L’URL della pagina di autorizzazione è quindi:

```
https://<URL of your organization's domain>/integrations/oauth2/authorize?client_id=<Your ClientID>&redirect_uri=<Your redirect URL>&response_type=code
```

>[!NOTE]
>
>È consigliabile creare un pulsante o un altro collegamento su cui gli utenti possono fare clic per indirizzarsi a questa pagina.

## Configurare l’applicazione di terze parti

L&#39;applicazione di terze parti può richiedere la configurazione. La tabella seguente contiene informazioni sui campi che possono essere necessari durante la configurazione dell’applicazione di terze parti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URI autorizzazione</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/authorize</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code> https://myorganization.my.workfront.com/integrations/oauth2/authorize</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL token</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/api/v1/token</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>https://myorganization.my.workfront.com/integrations/oauth2/api/v1/token</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ambiti</td> 
   <td>Non è necessario specificare ambiti. </td> 
  </tr> 
 </tbody> 
</table>

## Imposta flusso codice autorizzazione

![](assets/oauth-2-authorization-code-flow-350x194.png)

Per accedere agli utenti con OAuth2, utilizza il seguente processo:

1. Quando l’utente apre la pagina di autorizzazione, viene reindirizzato alla pagina di accesso di Workfront in modo che possa accedere a Workfront. Se l&#39;utente dispone di una configurazione SSO, si aprirà la pagina di accesso del provider di identità.

   Se l’utente ha già effettuato l’accesso a Workfront nello stesso browser o se l’utente ha effettuato correttamente l’accesso a Workfront, viene reindirizzato alla schermata di consenso:

   ![](assets/consent-screen-350x227.png)

1. Se l’utente consente l’accesso, la pagina viene reindirizzata al `redirect_url`. Il reindirizzamento deve includere i seguenti parametri di query:

* `code`: Codice di autorizzazione necessario per ottenere il token di accesso/aggiornamento.
* `domain`: Il dominio della tua organizzazione. Esempio: in `myorganization.my.workfront.com`, il dominio è `myorganization`.
* `lane`: la corsia della richiesta. Esempio: in `myorganization.preview.workfront.com`, la corsia è `preview`.

   >[!IMPORTANT]
   >
   >La `code` è valido solo per 2 minuti. Pertanto, è necessario ottenere i token di aggiornamento e accesso entro tale periodo di tempo.

1. Quando hai un codice, puoi richiedere l’aggiornamento e accedere ai token inviando il codice insieme alle credenziali dell’app client al `/integrations/oauth2/api/v1/token` punto finale.

   L’URL completo della richiesta del token è

   ```
   https://<URL of your organization's domain></span>/integrations/oauth2/api/v1/token
   ```

   **Esempi:**  Esempio di chiamata CURL all’endpoint token:

   Esempio 1

   ```
      curl --location --request POST '**<workfront host>**/integrations/oauth2/api/v1/token' \
      --header 'Authorization: Basic **<base64(client_id:client_secret)>**' \
      --header 'Content-Type: application/json' \
      --data-raw '{
      "code": "**<code>**",
      "grant_type": "**authorization_code**",
      "redirect_uri": "**<redirect_url>**"
      }'
   ```

   Esempio 2

   ```
      curl --location --request POST '**<workfront host>**/integrations/oauth2/api/v1/token' \
      --header 'Content-Type: application/x-www-form-urlencoded' \
      --data-urlencode 'grant_type=**authorization_code**' \
      --data-urlencode 'redirect_uri=**<redirect_url>**' \
      --data-urlencode 'code=**<code>**' \
      --data-urlencode 'client_id=**<client_id>**' \
      --data-urlencode 'client_secret=**<client_secret>**'  
   ```


   >[!IMPORTANT]
   >
   > Il segreto client è stato generato al momento della registrazione dell’app in Workfront. È necessario archiviarlo in un luogo sicuro, perché non può essere recuperato se viene perso.

   Quando tutti i parametri passati sono corretti, l&#39;endpoint token restituisce il seguente payload:

   ```
   {
      "token_type": "sessionID",
      "access_token": "string", // the value of sessionID
      "refresh_token": "string",
      "expires_in": 0,
      "wid": "string"
   }
   ```

   Il token di accesso è lo stesso di ```sessionID```e scade come normale ```sessionID```

   >[!IMPORTANT]
   >
   > Memorizza il token di aggiornamento in un luogo sicuro. Sarà necessario ottenere un nuovo token di aggiornamento quando il vecchio è scaduto. Workfront non memorizza il token di aggiornamento.

1. Ora, quando disponi di un token di accesso, puoi effettuare chiamate API a Workfront

   ```
   curl --request GET 'https://<workfront host>/attask/api/v14.0/proj/search \
   --header 'sessionID: <access_token>'
   ```

## Imposta Aggiorna token di accesso

![](assets/refresh-access-token-flow-350x142.png)

Per aggiornare l&#39;access_token, è necessario eseguire nuovamente una chiamata &quot;POST&quot; all&#39;endpoint del token. Questa volta si inviano i seguenti dati del modulo:

```
curl --location --request POST '<workfront host>/integrations/oauth2/api/v1/token' \
--header 'Authorization: Basic <base64(client_id:client_secret)>' \
--header 'Content-Type: application/json' \
--data-raw '{
   "grant_type": "refresh_token",
   "refresh_token": "<refresh_token>"
}'

###### OR

curl --location --request POST '<workfront host>/integrations/oauth2/api/v1/token' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--data-urlencode 'grant_type=refresh_token' \
--data-urlencode 'redirect_uri=<redirect_url>' \
--data-urlencode 'refresh_token=<refresh_token>' \
--data-urlencode 'client_id=<client_id>' \
--data-urlencode 'client_secret=<client_secret>'
```

Restituisce il seguente risultato:

```
{
  "token_type": "sessionID",
  "access_token": "string", // the value of sessionID
  "refresh_token": "string",
  "expires_in": 0,
  "wid": "string"
}
```

E di nuovo il token di accesso è il `sessionID` che può essere utilizzato per effettuare una richiesta API a Workfront.
