---
content-type: api
navigation-topic: api-navigation-topic
title: Utilizzo del flusso JWT per applicazioni OAuth 2 personalizzate
description: Utilizzo del flusso JWT per applicazioni OAuth 2 personalizzate
author: Becky
feature: Workfront API
role: Developer
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
TQID: https://experienceleague.adobe.com/uxF82lsimZlGpWRe8BEt80-9wb0rnwz7uhBHCI8nAig
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 462
ht-degree: 3%

---

# Configurare e utilizzare le applicazioni OAuth 2 personalizzate dell’organizzazione utilizzando il flusso JWT

Per eseguire l’integrazione con Workfront e consentire all’app client di comunicare con Workfront per conto dell’utente, è necessario:

* Creare un’applicazione OAuth2
* Creare un certificato a chiave pubblica
* Creare un token web JSON (JWT)

## Creare un&#39;applicazione OAuth2

Per istruzioni sulla creazione dell&#39;applicazione OAuth2, vedere [Creare un&#39;applicazione OAuth2 utilizzando l&#39;autenticazione del server (flusso JWT)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) in [Creare applicazioni OAuth2 per le integrazioni Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)

>[!NOTE]
>
>Puoi avere fino a un totale di dieci applicazioni OAuth2 alla volta.

## Creare un certificato a chiave pubblica

Per poter essere incluso nella richiesta di accesso, il JWT deve essere firmato e codificato in base 64. Le librerie JWT forniscono le funzioni necessarie per eseguire queste attività.

Il token deve essere firmato utilizzando la chiave privata per un certificato di firma digitale. In tal caso, puoi utilizzare la chiave privata di qualsiasi certificato associato per firmare il tuo JWT.

L&#39;algoritmo utilizzato è RS256 (firma RSA con SHA-256). Si tratta di un algoritmo asimmetrico che utilizza una coppia di chiavi pubblica/privata. Il provider di identità ha una chiave privata (segreta) utilizzata per generare la firma e il consumatore del JWT ottiene una chiave pubblica per convalidarla.

Per generare la chiave pubblica, eseguire **one** delle operazioni seguenti.

* Apri il terminale MacOS/Linux ed esegui il comando seguente, quindi carica `certificate_pub.crt` utilizzando il pulsante **Aggiungi chiave pubblica** nella configurazione dell&#39;applicazione OAuth2 in Workfront.

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* Utilizza il pulsante **Genera una coppia di chiavi pubblica/privata** nella configurazione dell&#39;applicazione OAuth2 in Workfront per generare l&#39;RSA.

## Creare un token web JSON

Un token web JSON per l’autenticazione dell’account di servizio richiede un set particolare di attestazioni e deve essere firmato utilizzando un certificato di firma digitale valido. È consigliabile utilizzare una delle librerie o degli strumenti disponibili al pubblico per creare il codice JWT.

La tabella seguente contiene informazioni sui campi che potrebbero essere necessari durante la configurazione del token JWT.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">exp</td> 
   <td> <p>Obbligatorio. Il parametro di scadenza è un parametro obbligatorio che misura il tempo assoluto dal 01/01/1970 GMT. Assicurati che la scadenza sia successiva alla data del rilascio. Trascorso questo periodo, il JWT non è più valido. </p> <p>Nota: ti consigliamo di disporre di un token di durata molto breve (pochi minuti), in modo che scada subito dopo essere stato scambiato per un token di accesso. Ogni volta che è necessario un nuovo token di accesso, viene firmato e scambiato un JWT. Si tratta di un approccio più sicuro. È sconsigliato utilizzare token di durata maggiore riutilizzati per ottenere i token di accesso in base alle esigenze.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">iss</td> 
   <td>Obbligatorio. L’emittente è il tuo ID cliente dai dettagli dell’app OAuth2.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>Obbligatorio. L'oggetto è l'ID utente che ha creato la chiave pubblica nella configurazione.</td> 
  </tr> 
 </tbody> 
</table>

## Scambia il JWT per recuperare un token di accesso

1. Invia una richiesta POST a:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. Il corpo della richiesta deve contenere parametri codificati in URL con ID client, Segreto client e JWT:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
