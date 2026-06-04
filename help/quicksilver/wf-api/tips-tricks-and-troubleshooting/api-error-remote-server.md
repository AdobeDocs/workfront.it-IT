---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Messaggio di errore API 400 - Richiesta non valida
description: Messaggio di errore API 400 - Richiesta non valida
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
TQID: https://experienceleague.adobe.com/19PIdv4u8de0BlasXD0Yy6GssO3vv6Jt8BzcljB-m1w
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 93
ht-degree: 2%

---

# Errore API: &quot;Il server remoto ha restituito un errore (400) Richiesta non valida&quot;

## Problema

Quando tenti di utilizzare l’API per importare un campo personalizzato in un problema, viene visualizzato il seguente errore:

`The remote server returned an error: (400) Bad Request`

## Causa

Questo errore si verifica quando si tenta di importare, tramite l’API, un campo personalizzato da un progetto a cui non è associato un modulo personalizzato con un Argomento coda.

## Soluzione

Aggiungi il modulo personalizzato corretto all’argomento della coda.

Per ulteriori informazioni sugli argomenti della coda, vedere [Creare argomenti della coda](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
