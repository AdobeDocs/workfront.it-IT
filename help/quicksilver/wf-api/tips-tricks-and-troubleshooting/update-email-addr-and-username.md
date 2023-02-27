---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: L'aggiornamento a emailAddr non aggiorna il nome utente
description: L'aggiornamento a emailAddr non aggiorna il nome utente
author: Becky
feature: Workfront API
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# L&#39;aggiornamento a emailAddr non aggiorna il nome utente

## Problema

Normalmente, `emailAddr` e `username` sono lo stesso attributo. Pertanto, se modifichi il `emailAddr` l&#39;attributo `username` l&#39;attributo viene aggiornato automaticamente per corrispondere.

Quando il `username` non corrisponde al `emailAddr`, un aggiornamento del `emailAddr` non aggiorna il `username` automaticamente. Questo vale per entrambi `emailAddr` le modifiche vengono effettuate tramite l’interfaccia utente e tramite l’API .

## Causa

La mancata corrispondenza può essere creata in diversi modi:

* Utenti creati prima dell&#39;esistenza della regola di sincronizzazione. Gli account utente molto vecchi potrebbero non avere questi attributi sincronizzati.

* Gli utenti creati tramite SSO in un momento in cui l’indirizzo e-mail Addr in Workfront faceva distinzione tra maiuscole e minuscole. L&#39;opzione di provisioning automatico SSO eseguirà un controllo con distinzione tra maiuscole e minuscole per gli utenti in base agli attributi dell&#39;utente provenienti dal provider di identità. Quando non esisteva una corrispondenza esatta, i servizi di provisioning automatico creavano un nuovo utente. Se un utente esisteva già, era possibile che il nome utente e `emailAddr` non avrebbe lo stesso involucro.

* Utenti che hanno avuto `username` l’attributo è aggiornato direttamente tramite l’API e le relative `emailAddr` non è stato aggiornato. La `username` e `emailAddr` potrebbero non corrispondere.

## Soluzione

Utilizza l’API per modificare il `username` come attributo `emailAddr`. Dopo aver sincronizzato gli attributi, eventuali aggiornamenti al `emailAddr` aggiornerà inoltre `username` da abbinare (quando il campo del nome utente non è incluso nell’aggiornamento).
