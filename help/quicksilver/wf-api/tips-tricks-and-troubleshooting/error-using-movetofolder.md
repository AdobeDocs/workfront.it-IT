---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: L'azione MoveToFolder del documento non funziona
description: Quando si utilizza l'azione MoveToFolder del documento, viene restituito un errore 422.
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
source-git-commit: 53edc378e000e5b36fe0ce5750b8917fb13cfde1
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# L&#39;azione MoveToFolder del documento non funziona

## Problema

Quando si utilizza l&#39;azione `moveToFolder` dell&#39;oggetto Document, viene restituito un errore 422.

Oppure

Se si utilizza questa azione tramite il modulo Adobe Authenticator in Workfront Fusion, il documento non viene spostato, ma non vi è alcuna indicazione dell’errore. L’errore è lo stesso, ma il modulo Adobe Authenticator non lo visualizza.

## Soluzione

Una possibile causa di un errore 422 per questa azione è il tentativo di spostare un documento in una cartella collegata in un&#39;altra cartella collegata.

Verificare che il documento che si desidera spostare non si trovi già in una cartella collegata.
