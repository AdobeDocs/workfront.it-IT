---
content-type: api
navigation-topic: api-navigation-topic
title: Caricamento di file tramite API
description: Caricamento di file tramite API
author: Becky
feature: Workfront API
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Caricamento di file tramite API

Puoi caricare i file utilizzando le API di Workfront con strumenti API, come Postman, o con semplici comandi cURL.

Per caricare i documenti, consulta le istruzioni per **Caricamento di documenti** in Workfront [Comportamento del post](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWF_API%2FGeneral%2Fapi-basics.html). Puoi anche utilizzare queste stesse istruzioni per le richieste cURL.

**Quando utilizzi gli strumenti API per caricare i file, segui queste linee guida:**

* Utilizza l’opzione dello strumento API per caricare il file. Questi sono spesso un **Scegli file** nella schermata della richiesta.

* Utilizza il metodo HTTP di POST per effettuare la richiesta di caricamento del file.

* La richiesta deve dare luogo a una risposta che includa un valore per il relativo handle.

* Utilizza il valore handle, il tipo di oggetto e il valore GUID per l’oggetto objID in un payload JSON per effettuare una chiamata successiva. Questo è per creare l’oggetto per il file, come nell’esempio seguente:

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

Dovresti ricevere un ID per l&#39;oggetto nella risposta.

Per ulteriori informazioni, consulta l’aiuto dello strumento API specifico utilizzato.
