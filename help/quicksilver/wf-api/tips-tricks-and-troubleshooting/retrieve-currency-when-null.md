---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Recupera le informazioni sulla valuta per un progetto quando la valuta è null
description: Recupera le informazioni sulla valuta per un progetto quando la valuta è null
author: Becky
feature: Workfront API
source-git-commit: a9af457793e123a60172fe4baf5ae5def472b026
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# Recupera le informazioni sulla valuta per un progetto quando la valuta è null (non assegnata)

L&#39;oggetto di progetto con il campo valuta può essere recuperato utilizzando la seguente richiesta:

```
GET /attask/api-internal/project/{{projectID}}?fields=currency
```

Questo restituirà il seguente corpo di risposta:

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

Se la valuta non è impostata per il progetto, questa risposta includerà una valuta con il valore `null`:

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

Se si richiede la valuta per il progetto (ad esempio per i calcoli), è possibile recuperare la valuta predefinita per il cliente:

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

La risposta include la valuta impostata come predefinita dall’utente, che verrà utilizzata da qualsiasi progetto per quel cliente che non ha la valuta impostata:

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
