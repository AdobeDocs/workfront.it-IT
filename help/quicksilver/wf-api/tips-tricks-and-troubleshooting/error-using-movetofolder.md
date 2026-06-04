---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: L’azione MoveToFolder del documento non funziona
description: Quando si utilizza l'azione MoveToFolder del documento, viene restituito un errore 422.
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
TQID: https://experienceleague.adobe.com/UV4VnQEs-jGJau1UqXTLnp7Ak-cmKRpjuJqxgNTF5z8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 121
ht-degree: 11%

---

# L’azione MoveToFolder del documento non funziona

## Problema

Quando si utilizza l&#39;azione `moveToFolder` dell&#39;oggetto Document, viene restituito un errore 422.

Oppure

Se si utilizza questa azione tramite il modulo Adobe Authenticator in Workfront Fusion, il documento non viene spostato, ma non vi è alcuna indicazione dell’errore. L’errore è lo stesso, ma il modulo Adobe Authenticator non lo visualizza.

## Soluzione

Una possibile causa di un errore 422 per questa azione è il tentativo di spostare un documento in una cartella collegata in un&#39;altra cartella collegata.

Verificare che il documento che si desidera spostare non si trovi già in una cartella collegata.
