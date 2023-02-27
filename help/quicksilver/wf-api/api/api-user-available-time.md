---
content-type: api
navigation-topic: wf-api
title: API tempo disponibile per gli utenti
description: API tempo disponibile per gli utenti
author: Becky
feature: Workfront API
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 7%

---

# API tempo disponibile per gli utenti

**URI: attask/api/v15.0/user/getUsersAvailableTime**

L&#39;endpoint temporale disponibile per gli utenti recupera i dati in base al tempo disponibile dell&#39;utente. Questo consente integrazioni per l’aggregazione di dati in base agli attributi utente e agli intervalli di tempo.

## Esempio di richiesta

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## Parametri di richiesta

* **userIDs**: array di stringhe. Obbligatorio. Esempio: `"61a9cc0500002f9fdaa7a6f824f557e1"`.

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

* **AVL**: Ore effettive disponibili. Matrice di numeri.
* **PAVL**: Orari disponibili puri per la pianificazione che non includono giorni non lavorativi o orari di inattività dell’utente. Stringa.
