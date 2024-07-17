---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: L’aggiornamento a emailAddr non aggiorna il nome utente
description: L’aggiornamento a emailAddr non aggiorna il nome utente
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# L’aggiornamento a emailAddr non aggiorna il nome utente

## Problema

Normalmente, `emailAddr` e `username` sono lo stesso attributo. Pertanto, se modifichi l&#39;attributo `emailAddr` di un utente, l&#39;attributo `username` viene aggiornato automaticamente in modo che corrisponda.

Quando `username` non corrisponde a `emailAddr`, un aggiornamento a `emailAddr` non aggiorna automaticamente `username`. Ciò vale sia per `emailAddr` modifiche tramite l&#39;interfaccia utente che tramite l&#39;API.

## Causa

La mancata corrispondenza può essere creata in diversi modi:

* Utenti creati prima della regola di sincronizzazione. Gli account utente molto vecchi potrebbero non avere questi attributi sincronizzati.

* Gli utenti creati tramite SSO in un momento in cui l’indirizzo e-mail in Workfront faceva distinzione tra maiuscole e minuscole. L’opzione di provisioning automatico SSO esegue un controllo con distinzione tra maiuscole e minuscole per gli utenti in base agli attributi dell’utente provenienti dal provider di identità. Se non esiste una corrispondenza esatta, i servizi di provisioning automatico creano un nuovo utente. Se un utente esiste già, è possibile che il nome utente e `emailAddr` non abbiano lo stesso carattere maiuscolo/minuscolo.

* Gli utenti che hanno avuto l&#39;attributo `username` aggiornato direttamente tramite l&#39;API e il loro `emailAddr` non è stato aggiornato. `username` e `emailAddr` potrebbero non corrispondere.

## Soluzione

Utilizzare l&#39;API per modificare l&#39;attributo `username` in modo che sia uguale a `emailAddr`. Dopo la sincronizzazione degli attributi, qualsiasi aggiornamento a `emailAddr` aggiornerà anche `username` in modo corrispondente (quando il campo del nome utente non è incluso nell&#39;aggiornamento).
