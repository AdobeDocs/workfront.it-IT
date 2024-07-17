---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Gestione degli errori dei webhook dei documenti
description: Gestione degli errori dei webhook dei documenti
author: Becky
feature: Workfront API
role: Developer
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Gestione degli errori dei webhook dei documenti

Possono verificarsi problemi durante l’elaborazione delle richieste API. Questo deve essere gestito in modo coerente tra tutti gli endpoint API. Quando si verifica un errore, il provider del webhook deve includere un codice di errore nell’intestazione della risposta. I codici di errore includono:

* 403 - Non consentito. Indica che i token di richiesta sono mancanti o non validi oppure che le credenziali associate ai token non hanno accesso alla risorsa specificata. Per i provider di webhook basati su OAuth, Adobe Workfront tenterà di recuperare i nuovi token di accesso.

* 404 - Non trovato. Indica che il file o la cartella specificata non esiste.

* 500 - Errore interno del server. Qualsiasi altro tipo di errore.

* Descrizione dell’errore nel corpo della risposta utilizzando il seguente formato:

  ```
  {status: "error"
   error: "Sample error message"}
  ```
