---
content-type: api
navigation-topic: wf-api
title: Ottieni API per il tempo disponibile degli utenti
description: Ottieni API per il tempo disponibile degli utenti
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
TQID: https://experienceleague.adobe.com/JPvalH2RQRfMeqbYyWXyjyXCx-bdaZwRoR6WDRerZ5U
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 95
ht-degree: 4%

---

# API tempo disponibile per gli utenti

**URI: attask/api/v15.0/user/getUsersAvailableTime**

L’endpoint &quot;users available time&quot; recupera i dati in base al tempo disponibile dell’utente. Questo consente integrazioni per l’aggregazione dei dati in base agli attributi utente e agli intervalli di tempo.

## Richiesta di esempio

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## Parametri di richiesta

* **userIDs**: matrice di stringhe. Obbligatorio. Esempio: `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate**: datetime. stringa. Obbligatorio. Esempio: `"2022-07-10T00:00:00"`.

* **toDate**: datetime. stringa. Obbligatorio. Esempio `"2022-07-20T23:59:59"`.

## Esempio di risposta:

```
{
    "data": {
        "result": {
            "PAVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            },
            "AVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    480.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            }
        }
    }
}
```

## Parametri di risposta

* **AVL**: ore disponibili effettive. Matrice di numeri.
* **PAVL**: ore disponibili per la pianificazione che non includono giorni non lavorativi o indisponibilità dell&#39;utente. Stringa.
