---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Messaggio di errore API 400 Richiesta non valida
description: Messaggio di errore API 400 Richiesta non valida
author: Becky
feature: Workfront API
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---


# Errore API: &quot;Il server remoto ha restituito un errore (400) Bad Request&quot;

## Problema

Viene visualizzato il seguente errore durante il tentativo di utilizzo dell’API per importare un campo personalizzato in un problema:

`The remote server returned an error: (400) Bad Request`

## Causa

Questo errore si verifica quando si tenta di importare, tramite API, un campo personalizzato da un progetto per il quale non è associato un modulo personalizzato a un argomento della coda.

## Soluzione

Aggiungere il modulo personalizzato corretto all&#39;argomento della coda.

Per ulteriori informazioni sugli argomenti della coda, consulta [Crea argomenti coda](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
