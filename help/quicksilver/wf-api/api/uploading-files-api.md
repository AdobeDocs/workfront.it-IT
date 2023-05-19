---
content-type: api
navigation-topic: api-navigation-topic
title: Caricamento di file tramite API
description: Caricamento di file tramite API
author: Becky
feature: Workfront API
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: 3db01c329c005570b782ae3445f83b7c44ced676
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Caricamento di file tramite API

Puoi caricare i file utilizzando le API di Workfront con strumenti API, come Postman, o con semplici comandi cURL.

Per caricare i documenti, consulta le istruzioni per **Caricamento di documenti** in Workfront [Comportamento del post](/help/quicksilver/wf-api/general/api-basics.md#post-behavior). Puoi inoltre utilizzare queste stesse istruzioni per le richieste cURL.

**Quando si utilizzano gli strumenti API per caricare i file, attenersi alle seguenti linee guida:**

* Utilizza l’opzione dello strumento API per caricare il file. Questi sono spesso **Scegli file** nella schermata di richiesta.

* Utilizza il metodo HTTP POST per effettuare la richiesta di caricamento del file.

* La richiesta deve tradursi in una risposta che includa un valore per il relativo handle.

* Utilizza il valore handle, il tipo di oggetto e il valore GUID per objID in un payload JSON per effettuare una chiamata successiva. Questo è per la creazione dell’oggetto per il file, come nell’esempio seguente:

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

Dovresti ricevere un ID per l’oggetto nella risposta.

Per ulteriori informazioni, consulta la guida dello strumento API specifico che stai utilizzando.
