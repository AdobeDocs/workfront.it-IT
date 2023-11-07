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

Normalmente, `emailAddr` e `username` sono lo stesso attributo. Pertanto, se modifichi il `emailAddr` , l&#39;attributo `username` L&#39;attributo viene aggiornato automaticamente in modo che corrisponda.

Quando `username` non corrisponde al `emailAddr`, un aggiornamento del `emailAddr` non aggiorna il `username` automaticamente. Questo è vero per entrambi `emailAddr` modifiche tramite l’interfaccia utente e tramite l’API.

## Causa

La mancata corrispondenza può essere creata in diversi modi:

* Utenti creati prima della regola di sincronizzazione. Gli account utente molto vecchi potrebbero non avere questi attributi sincronizzati.

* Gli utenti creati tramite SSO in un momento in cui l’indirizzo e-mail in Workfront faceva distinzione tra maiuscole e minuscole. L’opzione di provisioning automatico SSO esegue un controllo con distinzione tra maiuscole e minuscole per gli utenti in base agli attributi dell’utente provenienti dal provider di identità. Se non esiste una corrispondenza esatta, i servizi di provisioning automatico creano un nuovo utente. Se un utente esiste già, è possibile che il nome utente e `emailAddr` non avrebbe lo stesso rivestimento.

* Utenti che hanno avuto `username` aggiornamento diretto tramite l’API e i relativi `emailAddr` non è stato aggiornato. Il `username` e `emailAddr` è possibile che non corrispondano.

## Soluzione

Utilizza l’API per modificare la `username` l&#39;attributo deve essere uguale a `emailAddr`. Dopo la sincronizzazione degli attributi, qualsiasi aggiornamento di `emailAddr` aggiorna anche il `username` (quando il campo del nome utente non è incluso nell’aggiornamento).
