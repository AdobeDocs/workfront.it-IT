---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Configurazione opzioni per OPTASK copyIssue
description: Spiegazione dei valori interi previsti dall’endpoint copyIssue.
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 6%

---

# Configurazione opzioni per OPTASK copyIssue


Una delle proprietà per una chiamata API copyIssue è un campo denominato `options`. Questo campo richiede un numero intero.

Per includere una delle opzioni seguenti, immettere il numero intero corrispondente. Per includere più di un&#39;opzione, immettere la somma dei numeri interi corrispondenti.

| opzione | value* |
|---|---|
| Cancella assegnazioni | 2 |
| Annulla avanzamento | 4 |
| Cancella documenti | 128 |
| Cancella aggiornamenti | 65536 |
| Cancella autorizzazioni | 524288 |
| Cancella dati personalizzati | 1048576 |

*Tutti i valori sono potenze di 2.

Esempi:

* Per cancellare l’avanzamento quando copi il problema, immetti un `options` valore di `4`.

* Per cancellare sia l&#39;avanzamento che i documenti, immetti un `options` valore di `132`.

  Annulla avanzamento = 4

  Cancella documenti = 128

  4 + 128 = 132
