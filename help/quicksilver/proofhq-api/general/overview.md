---
title: Panoramica
description: Panoramica
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
TQID: https://experienceleague.adobe.com/WSTkOBXeb30iXwB9jNeaSeAo-6twy3cHfRlTnGf0GXo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 270
ht-degree: 1%

---

# Panoramica

**Benvenuti nell&#39;API Workfront Proof**

L’API Workfront Proof è un semplice servizio HTTP protetto tramite SSL. L’API si propone di fornirti tutte le funzionalità utilizzate nella nostra applicazione.

## Formati supportati

L&#39;interfaccia pubblica è conforme a SOAP 1.1 con il supporto WSDL. Tutte le richieste vengono quindi eseguite utilizzando XML su HTTPS.

## Controllo delle versioni API

Per preservare la compatibilità con le integrazioni client esistenti, abbiamo introdotto il controllo delle versioni API a partire dalla versione 12.1 di. Per ulteriori informazioni, vedere la pagina [Aggiornamenti API](https://api.proofhq.com/new-updates.html). Se un metodo o un parametro non contiene informazioni sulla versione, ciò significa che lo troverai come parte dell’API standard, consulta la sezione &quot;Guida introduttiva all’API&quot; di seguito.

## Guida introduttiva all’API

Il punto di ingresso API:

`https://soap.proofhq.com/soap` (si noti l&#39;utilizzo di HTTPS)

Il file WSDL è disponibile qui:

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**Questo file WSDL contiene tutte le modifiche apportate fino alla versione 12.1, dopo di che è stato introdotto il controllo delle versioni delle API. Per ulteriori informazioni sulle varie versioni di WSDL e sulle modifiche imminenti, vedere la pagina Aggiornamenti API**

Ogni richiesta API richiede una chiave di sessione. Questa chiave di sessione identifica l’utente di Workfront Proof che esegue le azioni e viene ottenuta chiamando il metodo doLogin() e passando l’indirizzo e-mail e la password dell’utente. Il metodo doLogin() deve essere chiamato solo una volta prima di una sequenza di richieste API. La chiave di sessione rimane attiva per un breve periodo di tempo e viene rinnovata a ogni chiamata del metodo. *A breve verrà aggiunto il supporto per l&#39;autenticazione basata su token.*

Tutte le richieste utilizzano la seguente busta, intestazione e formato del corpo:

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
       ... API function and data inserted here ...
    </soapenv:Body>
    </soapenv:Envelope>
```

