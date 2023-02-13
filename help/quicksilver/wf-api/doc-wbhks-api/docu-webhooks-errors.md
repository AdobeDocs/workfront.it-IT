---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Gestione degli errori dei webhook del documento
description: Gestione degli errori dei webhook del documento
author: John
feature: Workfront API
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
source-git-commit: 338cc745a7660ffed8e4d44e19dcadfdc13bc345
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%

---

# Gestione degli errori dei webhook del documento

Possono sorgere problemi durante l’elaborazione delle richieste API. Questo deve essere gestito in modo coerente in tutti gli endpoint API. Quando si verifica un errore, il provider webhook deve includere un codice di errore nell&#39;intestazione della risposta. I codici di errore includono:

* 403 - Vietato. Indica che i token di richiesta sono mancanti o non validi oppure che le credenziali associate ai token non hanno accesso alla risorsa specificata. Per i provider di webhook basati su OAuth, Adobe Workfront tenterà di recuperare nuovi token di accesso.

* 404 - Non trovato. Indica che il file o la cartella specificato non esiste.

* 500 - Errore interno del server. Qualsiasi altro tipo di errore.

* Descrizione dell’errore nel corpo della risposta utilizzando il seguente formato:

   ```
   {status: “error”
    error: “Sample error message”}
   ```
