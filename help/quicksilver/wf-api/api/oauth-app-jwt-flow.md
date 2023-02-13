---
content-type: api
navigation-topic: api-navigation-topic
title: Utilizzo del flusso JWT per applicazioni OAuth 2 personalizzate
description: Utilizzo del flusso JWT per applicazioni OAuth 2 personalizzate
author: John
feature: Workfront API
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
source-git-commit: 38e957253775f73cee7fe0c0d31bfeedb58ebf53
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Configura e utilizza le applicazioni personalizzate OAuth 2 della tua organizzazione utilizzando il flusso JWT

Al fine di integrarsi con Workfront e consentire alla tua app client di comunicare con Workfront per conto dell’utente, devi:

* Creare un’applicazione OAuth2
* Creare un certificato a chiave pubblica
* Creare un token web JSON (JWT)

## Creare un’applicazione OAuth2

Per istruzioni sulla creazione dell’applicazione OAuth2, consulta [Creare un’applicazione OAuth2 utilizzando l’autenticazione del server (flusso JWT)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) in [Creare applicazioni OAuth2 per le integrazioni Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Creare un certificato a chiave pubblica

Il JWT deve essere firmato e codificato base-64 per essere incluso nella richiesta di accesso. Le librerie JWT forniscono funzioni per eseguire queste attività.

È necessario firmare il token utilizzando la chiave privata per un certificato di firma digitale. In questo caso, puoi utilizzare la chiave privata di qualsiasi certificato associato per firmare il tuo JWT.

L&#39;algoritmo utilizzato è RS256 (firma RSA con SHA-256). Si tratta di un algoritmo asimmetrico che utilizza una coppia di chiavi pubblica/privata. Il provider di identità dispone di una chiave privata (segreta) utilizzata per generare la firma e il consumatore del JWT ottiene una chiave pubblica per convalidare la firma.

Per generare la chiave pubblica, fai **uno** dei seguenti elementi.

* Apri il terminale MacOS/Linux ed esegui il seguente comando, quindi carica `certificate_pub.crt` utilizzando **Aggiungi chiave pubblica** nella configurazione dell’applicazione OAuth2 in Workfront.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* Utilizza la **Generare una coppia di chiavi pubblica/privata** nella configurazione dell’applicazione OAuth2 in Workfront per generare l’RSA.

## Creare un token web JSON

Un token Web JSON per l’autenticazione dell’account di servizio richiede un particolare set di attestazioni e deve essere firmato utilizzando un certificato di firma digitale valido. Si consiglia di utilizzare una delle librerie o degli strumenti disponibili al pubblico per la creazione del JWT.

La tabella seguente contiene informazioni sui campi che possono essere necessari durante la configurazione del token JWT.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">exp</td> 
   <td> <p>Obbligatorio. Il parametro di scadenza è un parametro obbligatorio che misura il tempo assoluto dal 01/01/1970 GMT. Devi accertarti che la data di scadenza sia successiva alla data del problema. Dopo questo periodo, il JWT non è più valido. </p> <p>Nota: Si consiglia di avere un token di breve durata (pochi minuti), in modo che scada presto dopo essere stato scambiato per un token di accesso. Ogni volta che è richiesto un nuovo token di accesso, viene firmato e scambiato un JWT. Si tratta di un approccio più sicuro. Si sconsiglia di utilizzare token più longevi, riutilizzati per ottenere i token di accesso in base alle esigenze.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">iss</td> 
   <td>Obbligatorio. L’emittente è l’ID cliente dai dettagli dell’app OAuth2.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>Obbligatorio. L'oggetto è l'ID utente che ha creato la chiave pubblica nella configurazione.</td> 
  </tr> 
 </tbody> 
</table>

## Scambio JWT per recuperare un token di accesso

1. Invia una richiesta POST a:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. Il corpo della richiesta deve contenere parametri con codifica URL con il tuo ID client, il segreto client e JWT:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
