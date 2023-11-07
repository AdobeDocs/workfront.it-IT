---
content-type: api
navigation-topic: wf-api
title: Ottieni API per il tempo disponibile degli utenti
description: Ottieni API per il tempo disponibile degli utenti
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 9%

---

# API tempo disponibile per gli utenti

**URI: attask/api/v15.0/user/getUsersAvailableTime**

L’endpoint &quot;users available time&quot; recupera i dati in base al tempo disponibile dell’utente. Questo consente integrazioni per l’aggregazione dei dati in base agli attributi utente e agli intervalli di tempo.

## Richiesta di esempio

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## Parametri di richiesta

* **userIDs**: matrice di stringhe. Obbligatorio. Esempio: `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate**: datetime. stringa. Obbligatorio. Esempio:  `"2022-07-10T00:00:00"`.

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

* **AVL**: ore effettive disponibili. Matrice di numeri.
* **PAVL**: ore esclusivamente disponibili per la pianificazione, esclusi i giorni non lavorativi e il tempo libero dell’utente. Stringa.
