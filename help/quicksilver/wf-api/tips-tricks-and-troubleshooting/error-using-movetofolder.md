---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: L'azione MoveToFolder del documento non funziona
description: Quando si utilizza l'azione MoveToFolder del documento, viene restituito un errore 422.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 86c0517443537ec5af640036c290b3a495825fdc
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---


# L&#39;azione MoveToFolder del documento non funziona

## Problema

Quando si utilizza la proprietà `moveToFolder` viene restituito un errore 422.

Oppure

Se si utilizza questa azione tramite il modulo Adobe Authenticator in Workfront Fusion, il documento non viene spostato, ma non vi è alcuna indicazione dell’errore. L’errore è lo stesso, ma il modulo Adobe Authenticator non lo visualizza.

## Soluzione

Una possibile causa di un errore 422 per questa azione è il tentativo di spostare un documento in una cartella collegata in un&#39;altra cartella collegata.

Verificare che il documento che si desidera spostare non si trovi già in una cartella collegata.
