---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Configurazione opzioni per OPTASK copyIssue
description: Spiegazione dei valori interi previsti dall’endpoint copyIssue.
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
TQID: https://experienceleague.adobe.com/9cDJFoKl6zqpaAvqzpGqzflcbGZNrAWvEnUAFuqD-Rc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 122
ht-degree: 16%

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

* Per cancellare l&#39;avanzamento quando si copia il problema, immettere un valore `options` di `4`.

* Per cancellare sia l&#39;avanzamento che i documenti, immetti un valore `options` di `132`.

  Annulla avanzamento = 4

  Cancella documenti = 128

  4 + 128 = 132
