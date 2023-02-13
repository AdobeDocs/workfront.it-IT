---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Ottieni token OAuth2
description: Ottieni token OAuth2
author: John
feature: Workfront API
exl-id: f3a2630d-d34e-4d36-b2bb-707ba0d3258e
source-git-commit: 492361028e7cf0d886c1f84f437ce9c55bc6603e
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 4%

---


# Ottieni token OAuth2

## Ottenimento dei token OAuth2

Restituisce il token di aggiornamento OAuth2 e il token di accesso per un utente autenticato. Viene richiamato una volta quando l&#39;utente fornisce un provider di documenti. Vengono effettuate chiamate successive per ottenere un token di accesso aggiornato.

**URL**

POST /any/url

L’URL è configurabile e corrisponde al valore dell’URL dell’endpoint token nella pagina di configurazione dell’integrazione personalizzata.

### Parametri query

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
   <td>tipo_sovvenzione</td>
   <td>sì</td>
   <td><p>I valori includono "authorization_code" o "refresh_token". Il valore specificato indica quale dei due parametri verrà passato a questa chiamata API: codice o refresh_token.</p></td>
  </tr>
  <tr>
   <td>codice</td>
   <td>dipende</td>
   <td><p>Il codice di autorizzazione inviato ad Adobe Workfront subito dopo aver fatto clic sul pulsante "Grant". Questo è necessario solo quando il tipo di sovvenzione è "authorization_code". Il codice di autorizzazione dovrebbe essere di breve durata, generalmente con scadenza non superiore a 10 minuti.</p></td>
  </tr>
  <tr>
   <td>refresh_token</td>
   <td>dipende</td>
   <td><p>Questo è necessario solo quando si eseguono chiamate successive per recuperare un nuovo access_token, dato che il precedente access_token è scaduto. Quando invii questo valore, imposta il parametro Grant_type su "refresh_token".</p></td>
  </tr>
  <tr>
   <td>client_id</td>
   <td>sì</td>
   <td>L’ID client configurato in Workfront per questa integrazione personalizzata.</td>
  </tr>
  <tr>
   <td>client_secret</td>
   <td>sì</td>
   <td> Segreto client configurato in Workfront per questa integrazione personalizzata.</td>
  </tr>
 </tbody>
</table>

 

## risposta

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
   <td><p>Token utilizzato per effettuare chiamate API autorizzate per conto dell’utente. Questo dovrebbe scadere per evitare chiamate API non autorizzate.</p></td>
  </tr>
  <tr>
   <td>refresh_token </td>
   <td>Stringa</td>
   <td><p>Token longevo utilizzato per recuperare un nuovo access_token chiamando questo metodo API.</p></td>
  </tr>
  <tr>
   <td>expires_in </td>
   <td>long</td>
   <td><p>(facoltativo) tempo (in secondi) prima della scadenza di access_token, generalmente 3.600.</p></td>
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

## risposta

```
{
access_token:"ad8af5ad5ads759",
refresh_token:"9a0h5d87d808ads",
expires_id:3600
}
```
