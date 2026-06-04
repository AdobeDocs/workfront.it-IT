---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Ottenere token OAuth2
description: Ottenere token OAuth2
author: Becky
feature: Workfront API
role: Developer
exl-id: f3a2630d-d34e-4d36-b2bb-707ba0d3258e
TQID: https://experienceleague.adobe.com/dspQLWwqjYdo3y9Trqv70ylGd1hFE-ynJaBU7-xLyxg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 254
ht-degree: 10%

---

# Ottenere token OAuth2

## Recupero token OAuth2

Restituisce il token di aggiornamento e il token di accesso OAuth2 per un utente autenticato. Viene richiamato una volta quando l’utente fornisce un provider di documenti. Vengono effettuate chiamate successive per ottenere un token di accesso aggiornato.

**URL**

POST/any/url

L’URL è configurabile e corrisponde al valore dell’URL dell’endpoint del token nella pagina di configurazione dell’integrazione personalizzata.

### Parametri di query

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
   <td><p>I valori includono "authorized_code" o "refresh_token". Il valore specificato indica quale dei due parametri verrà trasmesso a questa chiamata API: code o refresh_token.</p></td>
  </tr>
  <tr>
   <td>codice</td>
   <td>dipende</td>
   <td><p>Il codice di autorizzazione inviato ad Adobe Workfront subito dopo che l’utente ha fatto clic sul pulsante "Concedi". Questa opzione è necessaria solo quando il tipo di concessione è "authorized_code". Il codice di autorizzazione deve essere di breve durata e scadere generalmente in 10 minuti o meno.</p></td>
  </tr>
  <tr>
   <td>refresh_token</td>
   <td>dipende</td>
   <td><p>Questa opzione è necessaria solo quando si effettuano chiamate successive per recuperare un nuovo access_token, dato che il precedente access_token è scaduto. Quando si invia questo valore, impostare il parametro grant_type su "refresh_token".</p></td>
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

 

## Risposta

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
   <td><p>Token utilizzato per effettuare chiamate API autorizzate per conto dell’utente. Questa impostazione dovrebbe scadere per evitare chiamate API non autorizzate.</p></td>
  </tr>
  <tr>
   <td>refresh_token </td>
   <td>Stringa</td>
   <td><p>Token di lunga durata utilizzato per recuperare un nuovo access_token chiamando questo metodo API.</p></td>
  </tr>
  <tr>
   <td>expires_in </td>
   <td>lungo</td>
   <td><p>(facoltativo) Tempo (in secondi) prima della scadenza del token di accesso, in genere 3.600.</p></td>
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

## Risposta

```
{
access_token:"ad8af5ad5ads759",
refresh_token:"9a0h5d87d808ads",
expires_id:3600
}
```
