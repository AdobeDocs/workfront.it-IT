---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Configurazione delle opzioni per OPTASK copyIssue
description: Una spiegazione dei valori interi previsti dall'endpoint copyIssue.
author: Becky
feature: Workfront API
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 93a67b3dbd59f188dad6b060ec93c3f137c981b2
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 6%

---

# Configurazione delle opzioni per OPTASK copyIssue


Una delle proprietà per una chiamata API copyIssue è un campo denominato `options`. Questo campo richiede un numero intero.

Per includere una delle opzioni seguenti, immettere il numero intero corrispondente. Per includere più di un&#39;opzione, immettere la somma dei numeri interi corrispondenti.

| opzione | value* |
|---|---|
| Cancella assegnazioni | 2 |
| Cancella progresso | 4 |
| Cancella documenti | 128 |
| Cancella aggiornamenti | 65536 |
| Cancella autorizzazioni | 524288 |
| Cancella dati personalizzati | 1048576 |

*Tutti i valori sono potenze di 2.

Esempi:

* Per cancellare l’avanzamento della copia del problema, immetti un `options` valore `4`.

* Per cancellare sia l&#39;avanzamento che i documenti, immetti un `options` valore `132`.

   Cancella avanzamento = 4

   Cancella documenti = 128

   4 + 128 = 132
