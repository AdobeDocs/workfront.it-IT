---
content-type: api
navigation-topic: api-navigation-topic
title: Flusso del codice di autorizzazione per le applicazioni OAuth 2 personalizzate
description: Flusso del codice di autorizzazione per le applicazioni OAuth 2 personalizzate
author: Becky
feature: Workfront API
role: Developer
exl-id: a1ab60c4-4255-4d80-87f1-f36d325254c2
source-git-commit: 293b7354e4549e51d78ad1aa75927a21d9044c43
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---


# Configurare e utilizzare le applicazioni OAuth 2 personalizzate della tua organizzazione utilizzando il flusso del codice di autorizzazione

Per eseguire l’integrazione con Workfront e consentire all’app client di comunicare con Workfront per conto dell’utente, è necessario:

* Creare un’applicazione OAuth2
* Configurare l’applicazione di terze parti
* Collegamento alla pagina Autorizza per i tuoi utenti
* Configurare il flusso del codice di autorizzazione: gli utenti accedono all’istanza di Workfront e accettano di consentire all’applicazione client di connettersi a Workfront per loro conto. Di conseguenza, ottieni un codice di autorizzazione che scambierai con i token di accesso e di aggiornamento.
* Configurare il flusso del token di aggiornamento: in questo flusso utilizzi il token di aggiornamento per ottenere un nuovo token di accesso quando quello precedente è scaduto.

## Creare un&#39;applicazione OAuth2

Per istruzioni sulla creazione dell&#39;applicazione OAuth2, vedi [Creare un&#39;applicazione OAuth2 utilizzando le credenziali utente (flusso del codice di autorizzazione)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create3) in [Creazione di applicazioni OAuth2 per le integrazioni Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Collegamento alla pagina Autorizza per i tuoi utenti

Gli utenti devono effettuare l’accesso per autorizzare questa integrazione nel proprio account. La pagina da autorizzare ha un formato specifico, descritto qui. Utilizza queste informazioni per determinare l’indirizzo della pagina di autorizzazione dell’app e fornisci agli utenti tale indirizzo o un collegamento a esso.

* L’URL completo del dominio della tua organizzazione. Esempio:

  ```
  https://myorganization.my.workfront.com
  ```


* `client_id`: questo è l’ID client generato al momento della creazione dell’app OAuth2 in Workfront.

* `redirect_uri`: questo è l’URL di reindirizzamento immesso durante la creazione dell’app. Gli utenti verranno indirizzati a questa pagina dopo aver autorizzato l’app per il loro account.

* `response_type`: questo deve avere il valore `code`.

L’URL per la pagina di autorizzazione è quindi:

```
https://<URL of your organization's domain>/integrations/oauth2/authorize?client_id=<Your ClientID>&redirect_uri=<Your redirect URL>&response_type=code
```

>[!NOTE]
>
>È consigliabile creare un pulsante o un altro collegamento su cui gli utenti possano fare clic per passare a questa pagina.

## Configurare l’applicazione di terze parti

L’applicazione di terze parti potrebbe richiedere la configurazione. La tabella seguente contiene informazioni sui campi che potrebbero essere necessari durante la configurazione dell&#39;applicazione di terze parti.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URI di autorizzazione</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/authorize</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code> https://myorganization.my.workfront.com/integrations/oauth2/authorize</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL token</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/api/v1/token</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Esempio: </b></span></span><code>https://myorganization.my.workfront.com/integrations/oauth2/api/v1/token</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ambiti</td> 
   <td>Non è necessario specificare gli ambiti. </td> 
  </tr> 
 </tbody> 
</table>

## Imposta flusso codice di autorizzazione

![](assets/oauth-2-authorization-code-flow.png)

Per accedere agli utenti con OAuth2, utilizza la procedura seguente:

1. Quando l’utente apre la pagina di autorizzazione, viene reindirizzato alla pagina di accesso di Workfront, in modo che possa accedere a Workfront. Se l’utente dispone di una configurazione SSO, viene aperta la pagina di accesso del provider di identità.

   Se l’utente ha già effettuato l’accesso a Workfront nello stesso browser o ha eseguito correttamente l’accesso a Workfront, viene reindirizzato alla schermata di consenso:

   ![](assets/consent-screen-350x227.png)

1. Se l’utente consente l’accesso, la pagina viene reindirizzata al `redirect_url`. Il reindirizzamento deve includere i seguenti parametri di query:

* `code`: codice di autorizzazione necessario per ottenere il token di accesso/aggiornamento.
* `domain`: dominio della tua organizzazione. Esempio: in `myorganization.my.workfront.com`, il dominio è `myorganization`.
* `lane`: la corsia della richiesta. Esempio: in `myorganization.preview.workfront.com`, la corsia è `preview`.

  >[!IMPORTANT]
  >
  >Il `code` è valido solo per 2 minuti. Pertanto, devi ottenere i token di aggiornamento e di accesso entro tale periodo di tempo.

1. Quando si dispone di un codice, è possibile richiedere l’aggiornamento e accedere ai token inviando il codice insieme alle credenziali dell’app client a `/integrations/oauth2/api/v1/token` endpoint.

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
   > Il segreto client è stato generato durante la registrazione dell’app in Workfront. È necessario conservarlo in un luogo sicuro, perché non può essere recuperato se viene perso.

   Quando tutti i parametri passati sono corretti, l’endpoint token restituisce il seguente payload:

   ```
   {
      "token_type": "sessionID",
      "access_token": "string", // the value of sessionID
      "refresh_token": "string",
      "expires_in": 0,
      "wid": "string"
   }
   ```

   Il token di accesso è uguale a ```sessionID```, e scade nello stesso modo del normale ```sessionID```

   >[!IMPORTANT]
   >
   > Memorizza il token di aggiornamento in un luogo sicuro. Ne avrai bisogno per ottenere un nuovo token di aggiornamento quando quello vecchio è scaduto. Workfront non memorizza il token di aggiornamento.

1. Ora, quando disponi di un token di accesso, puoi effettuare chiamate API a Workfront

   ```
   curl --request GET 'https://<workfront host>/attask/api/v14.0/proj/search \
   --header 'sessionID: <access_token>'
   ```

## Configurare il token di accesso per l’aggiornamento

![](assets/refresh-access-token-flow-350x142.png)

Per aggiornare access_token è necessario eseguire nuovamente una chiamata &quot;POST&quot; all’endpoint del token. Questa volta inviamo un modulo diverso dati come segue:

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
