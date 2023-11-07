---
content-type: api
navigation-topic: api-navigation-topic
title: Obsolescenza di API-Internal
description: Obsolescenza di API-Internal
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Obsolescenza di API-Internal

API-Internal è una versione dell’API Adobe Workfront non supportata a causa della sua progettazione e del suo scopo. Sebbene contenga gli aggiornamenti più recenti dell’API Workfront, è soggetta a modifiche senza preavviso e pertanto deve essere utilizzata con cautela nelle integrazioni di produzione. Workfront consiglia vivamente di aggiornare tutte le integrazioni API interne in un’API con versione.

Per ulteriori informazioni sulle versioni supportate dell’API di Workfront, consulta [Pianificazione del supporto e del controllo delle versioni API](../../wf-api/api/api-version-support-schedule.md).

**Utilizzo di API non supportata**

Se le integrazioni richiedono funzionalità non disponibili in un’API con versione, Workfront consiglia di utilizzare API non supportate. Simile a API-Internal, API-Unsupported non supportato. Non supportato da API include anche le modifiche più recenti all’API Workfront ed è soggetto a modifiche senza preavviso. Workfront ti incoraggia a utilizzare API non supportate nell’ambiente di test in cui puoi esplorare nuove funzionalità e garantire che l’API sia priva di bug.

**Determinazione della versione API in uso**

Puoi determinare la versione dell’API utilizzata dalle integrazioni utilizzando REST per creare un URI che invia una chiamata tramite HTTPS a Workfront e quindi restituisce una risposta JSON.

L’esempio seguente mostra un URI che chiama API-Internal:

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

L’esempio seguente mostra un URI che chiama API-Unsupported:

```
https://<domainname>.my.workfront.com/attask/api/api-unsupported/proj/4c70...
```

L’esempio seguente mostra un URI che chiama la versione 15.0 dell’API:

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
