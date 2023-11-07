---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Messaggio di errore API 400 - Richiesta non valida
description: Messaggio di errore API 400 - Richiesta non valida
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---


# Errore API: &quot;Il server remoto ha restituito un errore (400) Richiesta non valida&quot;

## Problema

Quando tenti di utilizzare l’API per importare un campo personalizzato in un problema, viene visualizzato il seguente errore:

`The remote server returned an error: (400) Bad Request`

## Causa

Questo errore si verifica quando si tenta di importare, tramite l’API, un campo personalizzato da un progetto a cui non è associato un modulo personalizzato con un Argomento coda.

## Soluzione

Aggiungi il modulo personalizzato corretto all’argomento della coda.

Per ulteriori informazioni sugli argomenti relativi alla coda, vedere [Crea argomenti coda](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
