---
title: Panoramica
description: Panoramica
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 1%

---

# Panoramica

**API di verifica Workfront**

L’API Workfront Proof è un semplice servizio HTTP protetto tramite SSL. L’API si propone di fornirti tutte le funzionalità utilizzate nella nostra applicazione.

## Formati supportati

L&#39;interfaccia pubblica è compatibile SOAP 1.1 con il supporto WSDL. Tutte le richieste vengono quindi eseguite utilizzando XML su HTTPS.

## Controllo delle versioni API

Per preservare la compatibilità con le integrazioni client esistenti, abbiamo introdotto il controllo delle versioni API a partire dalla versione 12.1 di. Consulta la sezione  [Aggiornamenti API](http://api.proofhq.com/new-updates) per ulteriori informazioni. Se un metodo o un parametro non contiene informazioni sulla versione, ciò significa che lo troverai come parte dell’API standard, consulta la sezione &quot;Guida introduttiva all’API&quot; di seguito.

## Guida introduttiva all’API

Il punto di ingresso API:

`https://soap.proofhq.com/soap` (nota l’utilizzo di HTTPS)

Il file WSDL è disponibile qui:

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**Questo file WSDL contiene tutte le modifiche apportate fino alla versione 12.1, in seguito alla quale è stato introdotto il controllo delle versioni delle API. Per ulteriori informazioni sulle varie versioni di WSDL e sulle modifiche imminenti, consulta la pagina Aggiornamenti API**

Ogni richiesta API richiede una chiave di sessione. Questa chiave di sessione identifica l’utente di Workfront Proof che esegue le azioni e viene ottenuta chiamando il metodo doLogin() e passando l’indirizzo e-mail e la password dell’utente. Il metodo doLogin() deve essere chiamato solo una volta prima di una sequenza di richieste API. La chiave di sessione rimane attiva per un breve periodo di tempo e viene rinnovata a ogni chiamata del metodo. *A breve verrà aggiunto il supporto per l’autenticazione basata su token.*

Tutte le richieste utilizzano la seguente busta, intestazione e formato del corpo:

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
       ... API function and data inserted here ...
    </soapenv:Body>
    </soapenv:Envelope>
```

## Domande frequenti

Per una raccolta di domande frequenti, visitare [questo](http://api.proofhq.com/faqs) pagina.
