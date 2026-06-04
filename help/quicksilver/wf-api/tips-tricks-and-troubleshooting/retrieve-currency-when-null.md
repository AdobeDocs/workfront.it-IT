---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Recuperare le informazioni sulla valuta per un progetto quando la valuta è null
description: Recuperare le informazioni sulla valuta per un progetto quando la valuta è null
author: Becky
feature: Workfront API
role: Developer
exl-id: 31ed533b-be19-4ccb-aad4-7c78e008b3e9
TQID: https://experienceleague.adobe.com/fWBcEeqoJFK6WzcEE2Ajqv6cdxk0J9IN1CiPPGU6pIg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 121
ht-degree: 9%

---

# Recuperare le informazioni sulla valuta per un progetto quando la valuta è Null (non assegnata)

L’oggetto del progetto con il campo valuta può essere recuperato utilizzando la seguente richiesta:

```
GET /attask/api-internal/project/{{projectID}}?fields=currency
```

Questo restituirebbe il seguente corpo di risposta:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": "EUR"
}
}
}
```

Se la valuta non è impostata per il progetto, questa risposta includerebbe una valuta con il valore `null`:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": null
}
}
}
```

Se è necessaria la valuta per il progetto (ad esempio per i calcoli), è possibile recuperare la valuta predefinita per il cliente:

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

La risposta include la valuta impostata dall’utente come predefinita, che verrebbe utilizzata da tutti i progetti per quel cliente che non hanno la valuta impostata:

```
{
"data": [
{
"ID": "some_customer_id,
"name": "some_customer_name",
"objCode": "CUST",
"currency": "USD"
}
]
}
```
