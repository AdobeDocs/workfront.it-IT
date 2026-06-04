---
content-type: api
navigation-topic: api-navigation-topic
title: Rimozione di API interne
description: Rimozione di API interne
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
TQID: https://experienceleague.adobe.com/LGyk8MIATMQj6JHqKmjkeL2pXW-b6xtxo2heMd4h0y4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 241
ht-degree: 4%

---

# Rimozione di API interne

API-Internal è una versione dell’API Adobe Workfront non supportata a causa della sua progettazione e del suo scopo. Sebbene contenga gli aggiornamenti più recenti dell’API Workfront, è soggetta a modifiche senza preavviso e pertanto deve essere utilizzata con cautela nelle integrazioni di produzione. Workfront consiglia vivamente di aggiornare tutte le integrazioni API interne in un’API con versione.

Per ulteriori informazioni sulle versioni supportate dell&#39;API Workfront, vedere [Controllo delle versioni e pianificazione del supporto API](../../wf-api/api/api-version-support-schedule.md).

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
https://<domainname>.my.workfront.com/attask/api-unsupported/proj/4c70...
```

>[!NOTE]
>
>Le chiamate non supportate dall&#39;API omettono la sezione `/api` dell&#39;URL.

L’esempio seguente mostra un URI che chiama la versione 15.0 dell’API:

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
