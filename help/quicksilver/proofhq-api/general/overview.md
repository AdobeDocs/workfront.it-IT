---
title: Panoramica
description: Panoramica
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 1%

---

# Panoramica

**Benvenuto nell’API di prova di Workfront**

L’API di prova di Workfront è un semplice servizio HTTP protetto tramite SSL. L’API si propone di fornire tutte le funzionalità utilizzate nella nostra applicazione.

## Formati supportati

L’interfaccia pubblica è compatibile con SOAP 1.1 con il supporto WSDL. Tutte le richieste vengono pertanto eseguite utilizzando XML su HTTPS.

## Controllo delle versioni API

Per preservare la compatibilità con le versioni esistenti dell’integrazione dei client, abbiamo introdotto il controllo delle versioni API a partire dalla versione 12.1. Vedi la  [Aggiornamenti API](http://api.proofhq.com/new-updates) per ulteriori informazioni. Se un metodo o un parametro non dispone di informazioni sulla versione, significa che lo troverai come parte della nostra API standard, consulta la sezione &quot;Guida introduttiva all’API&quot; di seguito.

## Guida introduttiva all’API

Punto di ingresso API:

`https://soap.proofhq.com/soap` (si prega di notare l&#39;uso di HTTPS)

Il WSDL è disponibile qui:

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**Questa WSDL contiene tutte le modifiche fino alla versione 12.1, dopodiché è stato introdotto il controllo delle versioni API. Per ulteriori informazioni sulle varie versioni WSDL e le prossime modifiche, consultate la pagina Aggiornamenti API .**

Ogni richiesta API richiede una chiave di sessione. Questa chiave di sessione identifica l&#39;utente Workfront Proof che esegue le azioni ed è ottenuta chiamando il metodo doLogin() e passando l&#39;indirizzo e-mail e la password dell&#39;utente. Il metodo doLogin() deve essere chiamato solo una volta prima di una sequenza di richieste API. La chiave di sessione rimane attiva per un breve periodo di tempo e viene rinnovata per ogni chiamata del metodo. *Presto verrà aggiunto il supporto per l’autenticazione basata sui token.*

Tutte le richieste utilizzano la busta, l&#39;intestazione e il formato del corpo seguenti:

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
	   ... API function and data inserted here ...
	</soapenv:Body>
	</soapenv:Envelope>
```

## Domande frequenti

Per una serie di domande frequenti, visita [questo](http://api.proofhq.com/faqs) pagina.
